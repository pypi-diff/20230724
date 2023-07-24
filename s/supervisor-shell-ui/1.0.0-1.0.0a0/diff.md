# Comparing `tmp/supervisor-shell-ui-1.0.0.tar.gz` & `tmp/supervisor-shell-ui-1.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supervisor-shell-ui-1.0.0.tar", last modified: Sun Jul 23 23:38:47 2023, max compression
+gzip compressed data, was "supervisor-shell-ui-1.0.0a0.tar", last modified: Sun Jul 23 22:50:57 2023, max compression
```

## Comparing `supervisor-shell-ui-1.0.0.tar` & `supervisor-shell-ui-1.0.0a0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:38:47.228561 supervisor-shell-ui-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34888 2023-07-23 23:38:36.000000 supervisor-shell-ui-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-23 23:38:47.228561 supervisor-shell-ui-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-07-23 23:38:36.000000 supervisor-shell-ui-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 23:38:47.228561 supervisor-shell-ui-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-23 23:38:36.000000 supervisor-shell-ui-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:38:47.228561 supervisor-shell-ui-1.0.0/supervisor_shell_ui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-23 23:38:47.000000 supervisor-shell-ui-1.0.0/supervisor_shell_ui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-23 23:38:47.000000 supervisor-shell-ui-1.0.0/supervisor_shell_ui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 23:38:47.000000 supervisor-shell-ui-1.0.0/supervisor_shell_ui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-23 23:38:47.000000 supervisor-shell-ui-1.0.0/supervisor_shell_ui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 23:38:47.000000 supervisor-shell-ui-1.0.0/supervisor_shell_ui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:50:57.239919 supervisor-shell-ui-1.0.0a0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34888 2023-07-23 22:50:37.000000 supervisor-shell-ui-1.0.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-07-23 22:50:57.239919 supervisor-shell-ui-1.0.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-07-23 22:50:37.000000 supervisor-shell-ui-1.0.0a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 22:50:57.239919 supervisor-shell-ui-1.0.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-23 22:50:37.000000 supervisor-shell-ui-1.0.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:50:57.239919 supervisor-shell-ui-1.0.0a0/supervisor_shell_ui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-07-23 22:50:57.000000 supervisor-shell-ui-1.0.0a0/supervisor_shell_ui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-23 22:50:57.000000 supervisor-shell-ui-1.0.0a0/supervisor_shell_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 22:50:57.000000 supervisor-shell-ui-1.0.0a0/supervisor_shell_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-23 22:50:57.000000 supervisor-shell-ui-1.0.0a0/supervisor_shell_ui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 22:50:57.000000 supervisor-shell-ui-1.0.0a0/supervisor_shell_ui.egg-info/top_level.txt
```

### Comparing `supervisor-shell-ui-1.0.0/LICENSE` & `supervisor-shell-ui-1.0.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `supervisor-shell-ui-1.0.0/PKG-INFO` & `supervisor-shell-ui-1.0.0a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supervisor-shell-ui
-Version: 1.0.0
+Version: 1.0.0a0
 Summary: A command-line alternative to the built-in web interface of Supervisor, a system for controlling processes, to manage them more conveniently.
 Author: Ciprian Mandache
 Author-email: psyb0t@51k.eu
 License: GPL-3.0
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `supervisor-shell-ui-1.0.0/README.md` & `supervisor-shell-ui-1.0.0a0/README.md`

 * *Files identical despite different names*

### Comparing `supervisor-shell-ui-1.0.0/setup.py` & `supervisor-shell-ui-1.0.0a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='supervisor-shell-ui',
-    version='v1.0.0',
+    version='v1.0.0-alpha',
     author='Ciprian Mandache',
     author_email='psyb0t@51k.eu',
     description='A command-line alternative to the built-in web interface of Supervisor, a system for controlling processes, to manage them more conveniently.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires='>=3.6',
     packages=find_packages(),
```

### Comparing `supervisor-shell-ui-1.0.0/supervisor_shell_ui.egg-info/PKG-INFO` & `supervisor-shell-ui-1.0.0a0/supervisor_shell_ui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supervisor-shell-ui
-Version: 1.0.0
+Version: 1.0.0a0
 Summary: A command-line alternative to the built-in web interface of Supervisor, a system for controlling processes, to manage them more conveniently.
 Author: Ciprian Mandache
 Author-email: psyb0t@51k.eu
 License: GPL-3.0
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

