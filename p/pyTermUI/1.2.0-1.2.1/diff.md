# Comparing `tmp/pyTermUI-1.2.0.tar.gz` & `tmp/pyTermUI-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyTermUI-1.2.0.tar", last modified: Mon Jul 24 09:21:40 2023, max compression
+gzip compressed data, was "pyTermUI-1.2.1.tar", last modified: Mon Jul 24 09:24:01 2023, max compression
```

## Comparing `pyTermUI-1.2.0.tar` & `pyTermUI-1.2.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 09:21:40.265200 pyTermUI-1.2.0/
--rw-rw-rw-   0        0        0    35823 2023-07-17 16:39:42.000000 pyTermUI-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     1033 2023-07-24 09:21:40.265200 pyTermUI-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      444 2023-07-24 09:17:59.000000 pyTermUI-1.2.0/README.md
--rw-rw-rw-   0        0        0      678 2023-07-24 09:15:11.000000 pyTermUI-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       51 2023-07-23 08:32:03.000000 pyTermUI-1.2.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 09:21:40.265200 pyTermUI-1.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-24 09:21:40.186313 pyTermUI-1.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-24 09:21:40.248967 pyTermUI-1.2.0/src/TermUI/
-drwxrwxrwx   0        0        0        0 2023-07-24 09:21:40.248967 pyTermUI-1.2.0/src/TermUI/Toolkit/
--rw-rw-rw-   0        0        0     1253 2023-07-23 05:57:56.000000 pyTermUI-1.2.0/src/TermUI/Toolkit/asciiart.py
--rw-rw-rw-   0        0        0     2342 2023-07-23 08:27:42.000000 pyTermUI-1.2.0/src/TermUI/Toolkit/hover.py
--rw-rw-rw-   0        0        0        0 2023-07-17 16:39:42.000000 pyTermUI-1.2.0/src/TermUI/__init__.py
--rw-rw-rw-   0        0        0     4142 2023-07-17 16:39:42.000000 pyTermUI-1.2.0/src/TermUI/button.py
--rw-rw-rw-   0        0        0     2488 2023-07-23 06:06:19.000000 pyTermUI-1.2.0/src/TermUI/checkbox.py
--rw-rw-rw-   0        0        0      613 2023-07-17 16:39:42.000000 pyTermUI-1.2.0/src/TermUI/colors.py
--rw-rw-rw-   0        0        0     2515 2023-07-17 16:39:42.000000 pyTermUI-1.2.0/src/TermUI/element.py
--rw-rw-rw-   0        0        0     1434 2023-07-17 16:39:42.000000 pyTermUI-1.2.0/src/TermUI/position.py
--rw-rw-rw-   0        0        0     7204 2023-07-17 16:39:42.000000 pyTermUI-1.2.0/src/TermUI/region.py
--rw-rw-rw-   0        0        0     1754 2023-07-17 16:39:42.000000 pyTermUI-1.2.0/src/TermUI/text.py
--rw-rw-rw-   0        0        0     8954 2023-07-23 08:25:26.000000 pyTermUI-1.2.0/src/TermUI/textbox.py
--rw-rw-rw-   0        0        0     4856 2023-07-23 07:42:44.000000 pyTermUI-1.2.0/src/TermUI/ui.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:21:40.248967 pyTermUI-1.2.0/src/pyTermUI.egg-info/
--rw-rw-rw-   0        0        0     1033 2023-07-24 09:21:40.000000 pyTermUI-1.2.0/src/pyTermUI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      499 2023-07-24 09:21:40.000000 pyTermUI-1.2.0/src/pyTermUI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 09:21:40.000000 pyTermUI-1.2.0/src/pyTermUI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-07-24 09:21:40.000000 pyTermUI-1.2.0/src/pyTermUI.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-24 09:21:40.000000 pyTermUI-1.2.0/src/pyTermUI.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 09:24:01.506339 pyTermUI-1.2.1/
+-rw-rw-rw-   0        0        0    35823 2023-07-17 16:39:42.000000 pyTermUI-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0      995 2023-07-24 09:24:01.506339 pyTermUI-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      403 2023-07-24 09:23:00.000000 pyTermUI-1.2.1/README.md
+-rw-rw-rw-   0        0        0      681 2023-07-24 09:23:36.000000 pyTermUI-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       51 2023-07-23 08:32:03.000000 pyTermUI-1.2.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 09:24:01.506339 pyTermUI-1.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-24 09:24:01.427899 pyTermUI-1.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-24 09:24:01.490629 pyTermUI-1.2.1/src/TermUI/
+drwxrwxrwx   0        0        0        0 2023-07-24 09:24:01.490629 pyTermUI-1.2.1/src/TermUI/Toolkit/
+-rw-rw-rw-   0        0        0     1253 2023-07-23 05:57:56.000000 pyTermUI-1.2.1/src/TermUI/Toolkit/asciiart.py
+-rw-rw-rw-   0        0        0     2342 2023-07-23 08:27:42.000000 pyTermUI-1.2.1/src/TermUI/Toolkit/hover.py
+-rw-rw-rw-   0        0        0        0 2023-07-17 16:39:42.000000 pyTermUI-1.2.1/src/TermUI/__init__.py
+-rw-rw-rw-   0        0        0     4142 2023-07-17 16:39:42.000000 pyTermUI-1.2.1/src/TermUI/button.py
+-rw-rw-rw-   0        0        0     2488 2023-07-23 06:06:19.000000 pyTermUI-1.2.1/src/TermUI/checkbox.py
+-rw-rw-rw-   0        0        0      613 2023-07-17 16:39:42.000000 pyTermUI-1.2.1/src/TermUI/colors.py
+-rw-rw-rw-   0        0        0     2515 2023-07-17 16:39:42.000000 pyTermUI-1.2.1/src/TermUI/element.py
+-rw-rw-rw-   0        0        0     1434 2023-07-17 16:39:42.000000 pyTermUI-1.2.1/src/TermUI/position.py
+-rw-rw-rw-   0        0        0     7204 2023-07-17 16:39:42.000000 pyTermUI-1.2.1/src/TermUI/region.py
+-rw-rw-rw-   0        0        0     1754 2023-07-17 16:39:42.000000 pyTermUI-1.2.1/src/TermUI/text.py
+-rw-rw-rw-   0        0        0     8954 2023-07-23 08:25:26.000000 pyTermUI-1.2.1/src/TermUI/textbox.py
+-rw-rw-rw-   0        0        0     4856 2023-07-23 07:42:44.000000 pyTermUI-1.2.1/src/TermUI/ui.py
+drwxrwxrwx   0        0        0        0 2023-07-24 09:24:01.506339 pyTermUI-1.2.1/src/pyTermUI.egg-info/
+-rw-rw-rw-   0        0        0      995 2023-07-24 09:24:01.000000 pyTermUI-1.2.1/src/pyTermUI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      499 2023-07-24 09:24:01.000000 pyTermUI-1.2.1/src/pyTermUI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 09:24:01.000000 pyTermUI-1.2.1/src/pyTermUI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-07-24 09:24:01.000000 pyTermUI-1.2.1/src/pyTermUI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-24 09:24:01.000000 pyTermUI-1.2.1/src/pyTermUI.egg-info/top_level.txt
```

### Comparing `pyTermUI-1.2.0/LICENSE` & `pyTermUI-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyTermUI-1.2.0/PKG-INFO` & `pyTermUI-1.2.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyTermUI
-Version: 1.2.0
+Version: 1.2.1
 Summary: pyTermUI or TermUI is a rapid development user interface library for python command-line interface applications.
-Author-email: iiVeil <email@email.com>
-Project-URL: Homepage, https://github.com/iiVeil/TermUi
+Author-email: iiVeil <zhuebner03@gmail.com>
+Project-URL: Github, https://github.com/iiVeil/TermUi
 Project-URL: Documentation, https://pytermui.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -16,11 +16,10 @@
 
 TermUI is a rapid development user interface library for python command-line applications.
 
 If you would like a reference for the library, D-Word is built on it. You can find it here: https://github.com/iiVeil/D-Word-Password-Manager
 
 Complete documentation available at https://pytermui.readthedocs.io/en/latest/
 
-Github: https//github.com/iiVeil/TermUI
 # Version 1.2
 
 All changelogs can be found in changelog.md on github
```

### Comparing `pyTermUI-1.2.0/src/TermUI/Toolkit/asciiart.py` & `pyTermUI-1.2.1/src/TermUI/Toolkit/asciiart.py`

 * *Files identical despite different names*

### Comparing `pyTermUI-1.2.0/src/TermUI/Toolkit/hover.py` & `pyTermUI-1.2.1/src/TermUI/Toolkit/hover.py`

 * *Files identical despite different names*

### Comparing `pyTermUI-1.2.0/src/TermUI/button.py` & `pyTermUI-1.2.1/src/TermUI/button.py`

 * *Files identical despite different names*

### Comparing `pyTermUI-1.2.0/src/TermUI/checkbox.py` & `pyTermUI-1.2.1/src/TermUI/checkbox.py`

 * *Files identical despite different names*

### Comparing `pyTermUI-1.2.0/src/TermUI/colors.py` & `pyTermUI-1.2.1/src/TermUI/colors.py`

 * *Files identical despite different names*

### Comparing `pyTermUI-1.2.0/src/TermUI/element.py` & `pyTermUI-1.2.1/src/TermUI/element.py`

 * *Files identical despite different names*

### Comparing `pyTermUI-1.2.0/src/TermUI/position.py` & `pyTermUI-1.2.1/src/TermUI/position.py`

 * *Files identical despite different names*

### Comparing `pyTermUI-1.2.0/src/TermUI/region.py` & `pyTermUI-1.2.1/src/TermUI/region.py`

 * *Files identical despite different names*

### Comparing `pyTermUI-1.2.0/src/TermUI/text.py` & `pyTermUI-1.2.1/src/TermUI/text.py`

 * *Files identical despite different names*

### Comparing `pyTermUI-1.2.0/src/TermUI/textbox.py` & `pyTermUI-1.2.1/src/TermUI/textbox.py`

 * *Files identical despite different names*

### Comparing `pyTermUI-1.2.0/src/TermUI/ui.py` & `pyTermUI-1.2.1/src/TermUI/ui.py`

 * *Files identical despite different names*

### Comparing `pyTermUI-1.2.0/src/pyTermUI.egg-info/PKG-INFO` & `pyTermUI-1.2.1/src/pyTermUI.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyTermUI
-Version: 1.2.0
+Version: 1.2.1
 Summary: pyTermUI or TermUI is a rapid development user interface library for python command-line interface applications.
-Author-email: iiVeil <email@email.com>
-Project-URL: Homepage, https://github.com/iiVeil/TermUi
+Author-email: iiVeil <zhuebner03@gmail.com>
+Project-URL: Github, https://github.com/iiVeil/TermUi
 Project-URL: Documentation, https://pytermui.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -16,11 +16,10 @@
 
 TermUI is a rapid development user interface library for python command-line applications.
 
 If you would like a reference for the library, D-Word is built on it. You can find it here: https://github.com/iiVeil/D-Word-Password-Manager
 
 Complete documentation available at https://pytermui.readthedocs.io/en/latest/
 
-Github: https//github.com/iiVeil/TermUI
 # Version 1.2
 
 All changelogs can be found in changelog.md on github
```

