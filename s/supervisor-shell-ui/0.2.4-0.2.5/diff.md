# Comparing `tmp/supervisor-shell-ui-0.2.4.tar.gz` & `tmp/supervisor-shell-ui-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supervisor-shell-ui-0.2.4.tar", last modified: Mon Jul 24 09:50:21 2023, max compression
+gzip compressed data, was "supervisor-shell-ui-0.2.5.tar", last modified: Mon Jul 24 10:03:53 2023, max compression
```

## Comparing `supervisor-shell-ui-0.2.4.tar` & `supervisor-shell-ui-0.2.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:50:21.123114 supervisor-shell-ui-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    34888 2023-07-24 09:50:11.000000 supervisor-shell-ui-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-07-24 09:50:21.123114 supervisor-shell-ui-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-24 09:50:11.000000 supervisor-shell-ui-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 09:50:21.123114 supervisor-shell-ui-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-24 09:50:11.000000 supervisor-shell-ui-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:50:21.119114 supervisor-shell-ui-0.2.4/supervisor_shell_ui/
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-24 09:50:11.000000 supervisor-shell-ui-0.2.4/supervisor_shell_ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-24 09:50:11.000000 supervisor-shell-ui-0.2.4/supervisor_shell_ui/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-24 09:50:11.000000 supervisor-shell-ui-0.2.4/supervisor_shell_ui/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-24 09:50:11.000000 supervisor-shell-ui-0.2.4/supervisor_shell_ui/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-24 09:50:11.000000 supervisor-shell-ui-0.2.4/supervisor_shell_ui/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-07-24 09:50:11.000000 supervisor-shell-ui-0.2.4/supervisor_shell_ui/page.py
--rw-r--r--   0 runner    (1001) docker     (123)    15706 2023-07-24 09:50:11.000000 supervisor-shell-ui-0.2.4/supervisor_shell_ui/page_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-07-24 09:50:11.000000 supervisor-shell-ui-0.2.4/supervisor_shell_ui/page_tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-07-24 09:50:11.000000 supervisor-shell-ui-0.2.4/supervisor_shell_ui/screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-24 09:50:11.000000 supervisor-shell-ui-0.2.4/supervisor_shell_ui/supervisor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:50:21.123114 supervisor-shell-ui-0.2.4/supervisor_shell_ui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-07-24 09:50:21.000000 supervisor-shell-ui-0.2.4/supervisor_shell_ui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-24 09:50:21.000000 supervisor-shell-ui-0.2.4/supervisor_shell_ui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 09:50:21.000000 supervisor-shell-ui-0.2.4/supervisor_shell_ui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-24 09:50:21.000000 supervisor-shell-ui-0.2.4/supervisor_shell_ui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-24 09:50:21.000000 supervisor-shell-ui-0.2.4/supervisor_shell_ui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:03:53.278569 supervisor-shell-ui-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    34888 2023-07-24 10:03:37.000000 supervisor-shell-ui-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-07-24 10:03:53.278569 supervisor-shell-ui-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-24 10:03:37.000000 supervisor-shell-ui-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 10:03:53.282569 supervisor-shell-ui-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-24 10:03:37.000000 supervisor-shell-ui-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:03:53.278569 supervisor-shell-ui-0.2.5/supervisor_shell_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-24 10:03:37.000000 supervisor-shell-ui-0.2.5/supervisor_shell_ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-24 10:03:37.000000 supervisor-shell-ui-0.2.5/supervisor_shell_ui/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-24 10:03:37.000000 supervisor-shell-ui-0.2.5/supervisor_shell_ui/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-24 10:03:37.000000 supervisor-shell-ui-0.2.5/supervisor_shell_ui/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-24 10:03:37.000000 supervisor-shell-ui-0.2.5/supervisor_shell_ui/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-07-24 10:03:37.000000 supervisor-shell-ui-0.2.5/supervisor_shell_ui/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15706 2023-07-24 10:03:37.000000 supervisor-shell-ui-0.2.5/supervisor_shell_ui/page_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-07-24 10:03:37.000000 supervisor-shell-ui-0.2.5/supervisor_shell_ui/page_tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-07-24 10:03:37.000000 supervisor-shell-ui-0.2.5/supervisor_shell_ui/screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-07-24 10:03:37.000000 supervisor-shell-ui-0.2.5/supervisor_shell_ui/supervisor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:03:53.278569 supervisor-shell-ui-0.2.5/supervisor_shell_ui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-07-24 10:03:53.000000 supervisor-shell-ui-0.2.5/supervisor_shell_ui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-24 10:03:53.000000 supervisor-shell-ui-0.2.5/supervisor_shell_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 10:03:53.000000 supervisor-shell-ui-0.2.5/supervisor_shell_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-24 10:03:53.000000 supervisor-shell-ui-0.2.5/supervisor_shell_ui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-24 10:03:53.000000 supervisor-shell-ui-0.2.5/supervisor_shell_ui.egg-info/top_level.txt
```

### Comparing `supervisor-shell-ui-0.2.4/LICENSE` & `supervisor-shell-ui-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `supervisor-shell-ui-0.2.4/PKG-INFO` & `supervisor-shell-ui-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supervisor-shell-ui
-Version: 0.2.4
+Version: 0.2.5
 Summary: A CLI alternative to the built-in web interface of Supervisor, offering a more convenient way to manage processes directly from the terminal.
 Author: Ciprian Mandache
 Author-email: psyb0t@51k.eu
 License: GPL-3.0
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `supervisor-shell-ui-0.2.4/README.md` & `supervisor-shell-ui-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `supervisor-shell-ui-0.2.4/setup.py` & `supervisor-shell-ui-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='supervisor-shell-ui',
-    version='v0.2.4',
+    version='v0.2.5',
     author='Ciprian Mandache',
     author_email='psyb0t@51k.eu',
     description='A CLI alternative to the built-in web interface of Supervisor, offering a more convenient way to manage processes directly from the terminal.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires='>=3.6',
     packages=find_packages(),
```

### Comparing `supervisor-shell-ui-0.2.4/supervisor_shell_ui/__init__.py` & `supervisor-shell-ui-0.2.5/supervisor_shell_ui/__init__.py`

 * *Files identical despite different names*

### Comparing `supervisor-shell-ui-0.2.4/supervisor_shell_ui/common.py` & `supervisor-shell-ui-0.2.5/supervisor_shell_ui/common.py`

 * *Files identical despite different names*

### Comparing `supervisor-shell-ui-0.2.4/supervisor_shell_ui/config.py` & `supervisor-shell-ui-0.2.5/supervisor_shell_ui/config.py`

 * *Files identical despite different names*

### Comparing `supervisor-shell-ui-0.2.4/supervisor_shell_ui/keys.py` & `supervisor-shell-ui-0.2.5/supervisor_shell_ui/keys.py`

 * *Files identical despite different names*

### Comparing `supervisor-shell-ui-0.2.4/supervisor_shell_ui/main.py` & `supervisor-shell-ui-0.2.5/supervisor_shell_ui/main.py`

 * *Files identical despite different names*

### Comparing `supervisor-shell-ui-0.2.4/supervisor_shell_ui/page.py` & `supervisor-shell-ui-0.2.5/supervisor_shell_ui/page.py`

 * *Files identical despite different names*

### Comparing `supervisor-shell-ui-0.2.4/supervisor_shell_ui/page_main.py` & `supervisor-shell-ui-0.2.5/supervisor_shell_ui/page_main.py`

 * *Files identical despite different names*

### Comparing `supervisor-shell-ui-0.2.4/supervisor_shell_ui/page_tail.py` & `supervisor-shell-ui-0.2.5/supervisor_shell_ui/page_tail.py`

 * *Files identical despite different names*

### Comparing `supervisor-shell-ui-0.2.4/supervisor_shell_ui/screen.py` & `supervisor-shell-ui-0.2.5/supervisor_shell_ui/screen.py`

 * *Files identical despite different names*

### Comparing `supervisor-shell-ui-0.2.4/supervisor_shell_ui/supervisor.py` & `supervisor-shell-ui-0.2.5/supervisor_shell_ui/supervisor.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,18 +24,21 @@
 
 LOG_SOURCE_STDOUT = "stdout"
 LOG_SOURCE_STDERR = "stderr"
 
 
 def exec(command, *args):
     command_args = ['supervisorctl', command] + list(args)
-    output = subprocess.check_output(
-        command_args, stderr=subprocess.STDOUT).decode('utf-8')
-
-    return output.strip()
+    try:
+        output = subprocess.check_output(
+            command_args, stderr=subprocess.STDOUT).decode('utf-8')
+        return output.strip()
+    except subprocess.CalledProcessError as e:
+        error_message = e.output.decode('utf-8')
+        raise Exception(f"command failed with error: {error_message}")
 
 
 def get_processes():
     try:
         output = exec('status')
     except subprocess.CalledProcessError as e:
         output = e.output.decode('utf-8')
```

### Comparing `supervisor-shell-ui-0.2.4/supervisor_shell_ui.egg-info/PKG-INFO` & `supervisor-shell-ui-0.2.5/supervisor_shell_ui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supervisor-shell-ui
-Version: 0.2.4
+Version: 0.2.5
 Summary: A CLI alternative to the built-in web interface of Supervisor, offering a more convenient way to manage processes directly from the terminal.
 Author: Ciprian Mandache
 Author-email: psyb0t@51k.eu
 License: GPL-3.0
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `supervisor-shell-ui-0.2.4/supervisor_shell_ui.egg-info/SOURCES.txt` & `supervisor-shell-ui-0.2.5/supervisor_shell_ui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

