# Comparing `tmp/keyring_pybridge-0.2.0.tar.gz` & `tmp/keyring_pybridge-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyring_pybridge-0.2.0.tar", max compression
+gzip compressed data, was "keyring_pybridge-0.3.0.tar", max compression
```

## Comparing `keyring_pybridge-0.2.0.tar` & `keyring_pybridge-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1181 2023-07-20 21:38:00.373844 keyring_pybridge-0.2.0/README.md
--rw-r--r--   0        0        0       68 2023-07-20 21:38:00.373844 keyring_pybridge-0.2.0/keyring_pybridge/__init__.py
--rw-r--r--   0        0        0     1122 2023-07-20 21:38:00.373844 keyring_pybridge-0.2.0/keyring_pybridge/backend.py
--rw-r--r--   0        0        0      711 2023-07-20 21:38:00.373844 keyring_pybridge-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1699 1970-01-01 00:00:00.000000 keyring_pybridge-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1459 2023-07-24 13:35:26.115597 keyring_pybridge-0.3.0/README.md
+-rw-r--r--   0        0        0       68 2023-07-24 13:35:26.115597 keyring_pybridge-0.3.0/keyring_pybridge/__init__.py
+-rw-r--r--   0        0        0     2127 2023-07-24 13:35:26.115597 keyring_pybridge-0.3.0/keyring_pybridge/backend.py
+-rw-r--r--   0        0        0      729 2023-07-24 13:35:26.115597 keyring_pybridge-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1977 1970-01-01 00:00:00.000000 keyring_pybridge-0.3.0/PKG-INFO
```

### Comparing `keyring_pybridge-0.2.0/pyproject.toml` & `keyring_pybridge-0.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "keyring-pybridge"
-version = "0.2.0"
+version = "0.3.0"
 description = ""
 authors = ["Korijn van Golen <korijn.vangolen@zimmerbiomet.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 keyring = "~24.2.0"
 
 [tool.poetry.group.dev.dependencies]
-ruff = "^0.0.278"
-black = "^23.7.0"
-twine = "^4.0.2"
+ruff = "~0.0.278"
+black = "~23.7.0"
+twine = "~4.0.2"
+pytest = "~7.4.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 select = [
```

### Comparing `keyring_pybridge-0.2.0/PKG-INFO` & `keyring_pybridge-0.3.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keyring-pybridge
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 License: MIT
 Author: Korijn van Golen
 Author-email: korijn.vangolen@zimmerbiomet.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -26,28 +26,27 @@
 
 Then set environment variables to use the backend:
 
 ```
 PYTHON_KEYRING_BACKEND=keyring_pybridge.PyBridgeKeyring
 ```
 
-Or use the programmatic API:
+Finally, you have to point the backend to the secondary python executable that you want to connect to. The keyring package must be installed in that python executable's environment.
 
-```py
-import keyring
-from keyring_pybridge import PyBridgeKeyring
-
-keyring.set_keyring(PyBridgeKeyring())
+```
+KEYRING_PROPERTY_PYTHON=/path/to/python
 ```
 
 ## WSL
 
 The most useful application of this backend is when you are using keyring in a WSL environment, and would like to connect it to the host machine's Windows Credential Manager.
 
 On the host machine, you need to create a python environment and install keyring in it.
 
 Then, in WSL, configure the environment variable `KEYRING_PROPERTY_PYTHON` to point to the python executable with keyring installed:
 
 ```
 KEYRING_PROPERTY_PYTHON=C:\path\to\the\right\python.exe
 ```
 
+Since this library calls the windows binary via a subprocess, this facilitates the context switch to windows that allows keyring to communicate with the Windows Credential Manager. 🎉
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

