# Comparing `tmp/pyTermUI-1.2.1.tar.gz` & `tmp/pyTermUI-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyTermUI-1.2.1.tar", last modified: Mon Jul 24 09:24:01 2023, max compression
+gzip compressed data, was "pyTermUI-1.2.2.tar", last modified: Mon Jul 24 09:35:05 2023, max compression
```

## Comparing `pyTermUI-1.2.1.tar` & `pyTermUI-1.2.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 09:24:01.506339 pyTermUI-1.2.1/
--rw-rw-rw-   0        0        0    35823 2023-07-17 16:39:42.000000 pyTermUI-1.2.1/LICENSE
--rw-rw-rw-   0        0        0      995 2023-07-24 09:24:01.506339 pyTermUI-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      403 2023-07-24 09:23:00.000000 pyTermUI-1.2.1/README.md
--rw-rw-rw-   0        0        0      681 2023-07-24 09:23:36.000000 pyTermUI-1.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       51 2023-07-23 08:32:03.000000 pyTermUI-1.2.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 09:24:01.506339 pyTermUI-1.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-24 09:24:01.427899 pyTermUI-1.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-24 09:24:01.490629 pyTermUI-1.2.1/src/TermUI/
-drwxrwxrwx   0        0        0        0 2023-07-24 09:24:01.490629 pyTermUI-1.2.1/src/TermUI/Toolkit/
--rw-rw-rw-   0        0        0     1253 2023-07-23 05:57:56.000000 pyTermUI-1.2.1/src/TermUI/Toolkit/asciiart.py
--rw-rw-rw-   0        0        0     2342 2023-07-23 08:27:42.000000 pyTermUI-1.2.1/src/TermUI/Toolkit/hover.py
--rw-rw-rw-   0        0        0        0 2023-07-17 16:39:42.000000 pyTermUI-1.2.1/src/TermUI/__init__.py
--rw-rw-rw-   0        0        0     4142 2023-07-17 16:39:42.000000 pyTermUI-1.2.1/src/TermUI/button.py
--rw-rw-rw-   0        0        0     2488 2023-07-23 06:06:19.000000 pyTermUI-1.2.1/src/TermUI/checkbox.py
--rw-rw-rw-   0        0        0      613 2023-07-17 16:39:42.000000 pyTermUI-1.2.1/src/TermUI/colors.py
--rw-rw-rw-   0        0        0     2515 2023-07-17 16:39:42.000000 pyTermUI-1.2.1/src/TermUI/element.py
--rw-rw-rw-   0        0        0     1434 2023-07-17 16:39:42.000000 pyTermUI-1.2.1/src/TermUI/position.py
--rw-rw-rw-   0        0        0     7204 2023-07-17 16:39:42.000000 pyTermUI-1.2.1/src/TermUI/region.py
--rw-rw-rw-   0        0        0     1754 2023-07-17 16:39:42.000000 pyTermUI-1.2.1/src/TermUI/text.py
--rw-rw-rw-   0        0        0     8954 2023-07-23 08:25:26.000000 pyTermUI-1.2.1/src/TermUI/textbox.py
--rw-rw-rw-   0        0        0     4856 2023-07-23 07:42:44.000000 pyTermUI-1.2.1/src/TermUI/ui.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:24:01.506339 pyTermUI-1.2.1/src/pyTermUI.egg-info/
--rw-rw-rw-   0        0        0      995 2023-07-24 09:24:01.000000 pyTermUI-1.2.1/src/pyTermUI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      499 2023-07-24 09:24:01.000000 pyTermUI-1.2.1/src/pyTermUI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 09:24:01.000000 pyTermUI-1.2.1/src/pyTermUI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-07-24 09:24:01.000000 pyTermUI-1.2.1/src/pyTermUI.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-24 09:24:01.000000 pyTermUI-1.2.1/src/pyTermUI.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 09:35:05.340086 pyTermUI-1.2.2/
+-rw-rw-rw-   0        0        0    35823 2023-07-17 16:39:42.000000 pyTermUI-1.2.2/LICENSE
+-rw-rw-rw-   0        0        0      995 2023-07-24 09:35:05.340086 pyTermUI-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      403 2023-07-24 09:23:00.000000 pyTermUI-1.2.2/README.md
+-rw-rw-rw-   0        0        0      681 2023-07-24 09:31:36.000000 pyTermUI-1.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       51 2023-07-23 08:32:03.000000 pyTermUI-1.2.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 09:35:05.340086 pyTermUI-1.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-24 09:35:05.260666 pyTermUI-1.2.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-24 09:35:05.323893 pyTermUI-1.2.2/src/pyTermUI/
+drwxrwxrwx   0        0        0        0 2023-07-24 09:35:05.340086 pyTermUI-1.2.2/src/pyTermUI/Toolkit/
+-rw-rw-rw-   0        0        0     1253 2023-07-23 05:57:56.000000 pyTermUI-1.2.2/src/pyTermUI/Toolkit/asciiart.py
+-rw-rw-rw-   0        0        0     2342 2023-07-23 08:27:42.000000 pyTermUI-1.2.2/src/pyTermUI/Toolkit/hover.py
+-rw-rw-rw-   0        0        0        0 2023-07-17 16:39:42.000000 pyTermUI-1.2.2/src/pyTermUI/__init__.py
+-rw-rw-rw-   0        0        0     4142 2023-07-17 16:39:42.000000 pyTermUI-1.2.2/src/pyTermUI/button.py
+-rw-rw-rw-   0        0        0     2488 2023-07-23 06:06:19.000000 pyTermUI-1.2.2/src/pyTermUI/checkbox.py
+-rw-rw-rw-   0        0        0      613 2023-07-17 16:39:42.000000 pyTermUI-1.2.2/src/pyTermUI/colors.py
+-rw-rw-rw-   0        0        0     2515 2023-07-17 16:39:42.000000 pyTermUI-1.2.2/src/pyTermUI/element.py
+-rw-rw-rw-   0        0        0     1434 2023-07-17 16:39:42.000000 pyTermUI-1.2.2/src/pyTermUI/position.py
+-rw-rw-rw-   0        0        0     7204 2023-07-17 16:39:42.000000 pyTermUI-1.2.2/src/pyTermUI/region.py
+-rw-rw-rw-   0        0        0     1754 2023-07-17 16:39:42.000000 pyTermUI-1.2.2/src/pyTermUI/text.py
+-rw-rw-rw-   0        0        0     8954 2023-07-23 08:25:26.000000 pyTermUI-1.2.2/src/pyTermUI/textbox.py
+-rw-rw-rw-   0        0        0     4856 2023-07-23 07:42:44.000000 pyTermUI-1.2.2/src/pyTermUI/ui.py
+drwxrwxrwx   0        0        0        0 2023-07-24 09:35:05.340086 pyTermUI-1.2.2/src/pyTermUI.egg-info/
+-rw-rw-rw-   0        0        0      995 2023-07-24 09:35:05.000000 pyTermUI-1.2.2/src/pyTermUI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      523 2023-07-24 09:35:05.000000 pyTermUI-1.2.2/src/pyTermUI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 09:35:05.000000 pyTermUI-1.2.2/src/pyTermUI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-07-24 09:35:05.000000 pyTermUI-1.2.2/src/pyTermUI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-24 09:35:05.000000 pyTermUI-1.2.2/src/pyTermUI.egg-info/top_level.txt
```

### Comparing `pyTermUI-1.2.1/LICENSE` & `pyTermUI-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyTermUI-1.2.1/PKG-INFO` & `pyTermUI-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTermUI
-Version: 1.2.1
+Version: 1.2.2
 Summary: pyTermUI or TermUI is a rapid development user interface library for python command-line interface applications.
 Author-email: iiVeil <zhuebner03@gmail.com>
 Project-URL: Github, https://github.com/iiVeil/TermUi
 Project-URL: Documentation, https://pytermui.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyTermUI-1.2.1/pyproject.toml` & `pyTermUI-1.2.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 dynamic = ["dependencies"]
 name = "pyTermUI"
-version = "1.2.1"
+version = "1.2.2"
 authors = [
   { name="iiVeil", email="zhuebner03@gmail.com" },
 ]
 description = "pyTermUI or TermUI is a rapid development user interface library for python command-line interface applications."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pyTermUI-1.2.1/src/TermUI/Toolkit/asciiart.py` & `pyTermUI-1.2.2/src/pyTermUI/Toolkit/asciiart.py`

 * *Files identical despite different names*

### Comparing `pyTermUI-1.2.1/src/TermUI/Toolkit/hover.py` & `pyTermUI-1.2.2/src/pyTermUI/Toolkit/hover.py`

 * *Files identical despite different names*

### Comparing `pyTermUI-1.2.1/src/TermUI/button.py` & `pyTermUI-1.2.2/src/pyTermUI/button.py`

 * *Files identical despite different names*

### Comparing `pyTermUI-1.2.1/src/TermUI/checkbox.py` & `pyTermUI-1.2.2/src/pyTermUI/checkbox.py`

 * *Files identical despite different names*

### Comparing `pyTermUI-1.2.1/src/TermUI/colors.py` & `pyTermUI-1.2.2/src/pyTermUI/colors.py`

 * *Files identical despite different names*

### Comparing `pyTermUI-1.2.1/src/TermUI/element.py` & `pyTermUI-1.2.2/src/pyTermUI/element.py`

 * *Files identical despite different names*

### Comparing `pyTermUI-1.2.1/src/TermUI/position.py` & `pyTermUI-1.2.2/src/pyTermUI/position.py`

 * *Files identical despite different names*

### Comparing `pyTermUI-1.2.1/src/TermUI/region.py` & `pyTermUI-1.2.2/src/pyTermUI/region.py`

 * *Files identical despite different names*

### Comparing `pyTermUI-1.2.1/src/TermUI/text.py` & `pyTermUI-1.2.2/src/pyTermUI/text.py`

 * *Files identical despite different names*

### Comparing `pyTermUI-1.2.1/src/TermUI/textbox.py` & `pyTermUI-1.2.2/src/pyTermUI/textbox.py`

 * *Files identical despite different names*

### Comparing `pyTermUI-1.2.1/src/TermUI/ui.py` & `pyTermUI-1.2.2/src/pyTermUI/ui.py`

 * *Files identical despite different names*

### Comparing `pyTermUI-1.2.1/src/pyTermUI.egg-info/PKG-INFO` & `pyTermUI-1.2.2/src/pyTermUI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTermUI
-Version: 1.2.1
+Version: 1.2.2
 Summary: pyTermUI or TermUI is a rapid development user interface library for python command-line interface applications.
 Author-email: iiVeil <zhuebner03@gmail.com>
 Project-URL: Github, https://github.com/iiVeil/TermUi
 Project-URL: Documentation, https://pytermui.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

