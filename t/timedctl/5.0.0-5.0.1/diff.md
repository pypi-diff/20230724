# Comparing `tmp/timedctl-5.0.0.tar.gz` & `tmp/timedctl-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timedctl-5.0.0.tar", max compression
+gzip compressed data, was "timedctl-5.0.1.tar", max compression
```

## Comparing `timedctl-5.0.0.tar` & `timedctl-5.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    34454 2023-07-23 23:49:27.165850 timedctl-5.0.0/LICENSE
--rw-r--r--   0        0        0      773 2023-07-23 23:49:27.165850 timedctl-5.0.0/README.md
--rw-r--r--   0        0        0      849 2023-07-23 23:49:55.327557 timedctl-5.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-23 23:49:27.165850 timedctl-5.0.0/timedctl/__init__.py
--rwxr-xr-x   0        0        0    17352 2023-07-23 23:49:27.165850 timedctl-5.0.0/timedctl/timedctl.py
--rw-r--r--   0        0        0     1528 1970-01-01 00:00:00.000000 timedctl-5.0.0/PKG-INFO
+-rw-r--r--   0        0        0    34454 2023-07-23 23:55:15.711716 timedctl-5.0.1/LICENSE
+-rw-r--r--   0        0        0      774 2023-07-23 23:55:15.711716 timedctl-5.0.1/README.md
+-rw-r--r--   0        0        0      849 2023-07-23 23:55:35.735773 timedctl-5.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-23 23:55:15.715716 timedctl-5.0.1/timedctl/__init__.py
+-rwxr-xr-x   0        0        0    17352 2023-07-23 23:55:15.715716 timedctl-5.0.1/timedctl/timedctl.py
+-rw-r--r--   0        0        0     1529 1970-01-01 00:00:00.000000 timedctl-5.0.1/PKG-INFO
```

### Comparing `timedctl-5.0.0/LICENSE` & `timedctl-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `timedctl-5.0.0/README.md` & `timedctl-5.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 Click TUI for [Timed](https://github.com/adfinis/timed-frontend) using [libtimed](https://github.com/adfinis/libtimed).
 
 ## Getting started
 Build the project with `poetry build` and install it with `pip install dist/timedctl-*.whl`. You should now be able to use `timedctl` iin your terminal.
 
 ## Configuration
 Create a config file at `$XDG_CONFIG_HOME/timedctl/config.toml`.
+
 The following values must be set:
 ```toml
 username = "<your username>"
 timed_url = "<timed url>"
 sso_url = "<sso url>"
 sso_realm = "<sso realm>"
 sso_client_id = "<client id>"
```

### Comparing `timedctl-5.0.0/pyproject.toml` & `timedctl-5.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "timedctl"
-version = "5.0.0"
+version = "5.0.1"
 description = "CLI for timed"
 authors = ["Arthur Deierlein <arthur.deierlein@adfinis.com>", "Gian Klug <gian.klug@adfinis.com>"]
 readme = "README.md"
 license = "AGPL-3.0-only"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `timedctl-5.0.0/timedctl/timedctl.py` & `timedctl-5.0.1/timedctl/timedctl.py`

 * *Files identical despite different names*

### Comparing `timedctl-5.0.0/PKG-INFO` & `timedctl-5.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timedctl
-Version: 5.0.0
+Version: 5.0.1
 Summary: CLI for timed
 License: AGPL-3.0-only
 Author: Arthur Deierlein
 Author-email: arthur.deierlein@adfinis.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
@@ -26,14 +26,15 @@
 Click TUI for [Timed](https://github.com/adfinis/timed-frontend) using [libtimed](https://github.com/adfinis/libtimed).
 
 ## Getting started
 Build the project with `poetry build` and install it with `pip install dist/timedctl-*.whl`. You should now be able to use `timedctl` iin your terminal.
 
 ## Configuration
 Create a config file at `$XDG_CONFIG_HOME/timedctl/config.toml`.
+
 The following values must be set:
 ```toml
 username = "<your username>"
 timed_url = "<timed url>"
 sso_url = "<sso url>"
 sso_realm = "<sso realm>"
 sso_client_id = "<client id>"
```

