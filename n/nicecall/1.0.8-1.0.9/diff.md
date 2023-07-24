# Comparing `tmp/nicecall-1.0.8.tar.gz` & `tmp/nicecall-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nicecall-1.0.8.tar", last modified: Mon Aug  8 23:51:12 2016, max compression
+gzip compressed data, was "dist/nicecall-1.0.9.tar", last modified: Tue Aug 23 14:06:46 2016, max compression
```

## Comparing `nicecall-1.0.8.tar` & `nicecall-1.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 arsene    (1000) arsene    (1000)        0 2016-08-08 23:51:12.000000 nicecall-1.0.8/
--rw-rw-r--   0 arsene    (1000) arsene    (1000)       59 2016-08-08 23:51:12.000000 nicecall-1.0.8/setup.cfg
--rw-rw-r--   0 arsene    (1000) arsene    (1000)    13533 2016-08-08 23:51:12.000000 nicecall-1.0.8/PKG-INFO
-drwxrwxr-x   0 arsene    (1000) arsene    (1000)        0 2016-08-08 23:51:12.000000 nicecall-1.0.8/nicecall.egg-info/
--rw-rw-r--   0 arsene    (1000) arsene    (1000)      355 2016-08-08 23:51:12.000000 nicecall-1.0.8/nicecall.egg-info/SOURCES.txt
--rw-rw-r--   0 arsene    (1000) arsene    (1000)    13533 2016-08-08 23:51:11.000000 nicecall-1.0.8/nicecall.egg-info/PKG-INFO
--rw-rw-r--   0 arsene    (1000) arsene    (1000)        9 2016-08-08 23:51:11.000000 nicecall-1.0.8/nicecall.egg-info/top_level.txt
--rw-rw-r--   0 arsene    (1000) arsene    (1000)        1 2016-08-08 23:51:11.000000 nicecall-1.0.8/nicecall.egg-info/dependency_links.txt
-drwxrwxr-x   0 arsene    (1000) arsene    (1000)        0 2016-08-08 23:51:12.000000 nicecall-1.0.8/nicecall/
--rw-rw-r--   0 arsene    (1000) arsene    (1000)      630 2016-08-03 01:53:04.000000 nicecall-1.0.8/nicecall/logger.py
--rw-rw-r--   0 arsene    (1000) arsene    (1000)      103 2016-08-03 13:35:47.000000 nicecall-1.0.8/nicecall/filters.py
-drwxrwxr-x   0 arsene    (1000) arsene    (1000)        0 2016-08-08 23:51:12.000000 nicecall-1.0.8/nicecall/tests/
--rw-rw-r--   0 arsene    (1000) arsene    (1000)      106 2016-08-04 23:19:40.000000 nicecall-1.0.8/nicecall/tests/null_process.py
--rw-rw-r--   0 arsene    (1000) arsene    (1000)     1117 2016-08-05 13:59:21.000000 nicecall-1.0.8/nicecall/tests/process_stub.py
--rw-rw-r--   0 arsene    (1000) arsene    (1000)      129 2016-08-04 23:30:54.000000 nicecall-1.0.8/nicecall/tests/__init__.py
--rw-rw-r--   0 arsene    (1000) arsene    (1000)     2042 2016-08-04 23:59:39.000000 nicecall-1.0.8/nicecall/tests/process_mock_context.py
--rw-rw-r--   0 arsene    (1000) arsene    (1000)     4503 2016-08-08 23:26:07.000000 nicecall-1.0.8/nicecall/process.py
--rw-rw-r--   0 arsene    (1000) arsene    (1000)      123 2016-08-05 13:49:49.000000 nicecall-1.0.8/nicecall/__init__.py
--rw-rw-r--   0 arsene    (1000) arsene    (1000)    11207 2016-08-05 14:44:19.000000 nicecall-1.0.8/README.rst
--rw-rw-r--   0 arsene    (1000) arsene    (1000)      585 2016-08-08 23:50:45.000000 nicecall-1.0.8/setup.py
+drwxrwxr-x   0 arsene    (1000) arsene    (1000)        0 2016-08-23 14:06:46.000000 nicecall-1.0.9/
+-rw-rw-r--   0 arsene    (1000) arsene    (1000)       59 2016-08-23 14:06:46.000000 nicecall-1.0.9/setup.cfg
+-rw-rw-r--   0 arsene    (1000) arsene    (1000)    13533 2016-08-23 14:06:46.000000 nicecall-1.0.9/PKG-INFO
+drwxrwxr-x   0 arsene    (1000) arsene    (1000)        0 2016-08-23 14:06:46.000000 nicecall-1.0.9/nicecall.egg-info/
+-rw-rw-r--   0 arsene    (1000) arsene    (1000)      355 2016-08-23 14:06:46.000000 nicecall-1.0.9/nicecall.egg-info/SOURCES.txt
+-rw-rw-r--   0 arsene    (1000) arsene    (1000)    13533 2016-08-23 14:06:45.000000 nicecall-1.0.9/nicecall.egg-info/PKG-INFO
+-rw-rw-r--   0 arsene    (1000) arsene    (1000)        9 2016-08-23 14:06:45.000000 nicecall-1.0.9/nicecall.egg-info/top_level.txt
+-rw-rw-r--   0 arsene    (1000) arsene    (1000)        1 2016-08-23 14:06:45.000000 nicecall-1.0.9/nicecall.egg-info/dependency_links.txt
+drwxrwxr-x   0 arsene    (1000) arsene    (1000)        0 2016-08-23 14:06:46.000000 nicecall-1.0.9/nicecall/
+-rw-rw-r--   0 arsene    (1000) arsene    (1000)      630 2016-08-03 01:53:04.000000 nicecall-1.0.9/nicecall/logger.py
+-rw-rw-r--   0 arsene    (1000) arsene    (1000)      103 2016-08-03 13:35:47.000000 nicecall-1.0.9/nicecall/filters.py
+drwxrwxr-x   0 arsene    (1000) arsene    (1000)        0 2016-08-23 14:06:46.000000 nicecall-1.0.9/nicecall/tests/
+-rw-rw-r--   0 arsene    (1000) arsene    (1000)      106 2016-08-04 23:19:40.000000 nicecall-1.0.9/nicecall/tests/null_process.py
+-rw-rw-r--   0 arsene    (1000) arsene    (1000)     1117 2016-08-05 13:59:21.000000 nicecall-1.0.9/nicecall/tests/process_stub.py
+-rw-rw-r--   0 arsene    (1000) arsene    (1000)      129 2016-08-04 23:30:54.000000 nicecall-1.0.9/nicecall/tests/__init__.py
+-rw-rw-r--   0 arsene    (1000) arsene    (1000)     2042 2016-08-04 23:59:39.000000 nicecall-1.0.9/nicecall/tests/process_mock_context.py
+-rw-rw-r--   0 arsene    (1000) arsene    (1000)     4503 2016-08-23 14:03:59.000000 nicecall-1.0.9/nicecall/process.py
+-rw-rw-r--   0 arsene    (1000) arsene    (1000)      123 2016-08-05 13:49:49.000000 nicecall-1.0.9/nicecall/__init__.py
+-rw-rw-r--   0 arsene    (1000) arsene    (1000)    11207 2016-08-05 14:44:19.000000 nicecall-1.0.9/README.rst
+-rw-rw-r--   0 arsene    (1000) arsene    (1000)      585 2016-08-23 14:05:44.000000 nicecall-1.0.9/setup.py
```

### Comparing `nicecall-1.0.8/PKG-INFO` & `nicecall-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: nicecall
-Version: 1.0.8
+Version: 1.0.9
 Summary: A library which provides a slightly more convinient way to launch processes, compared to Python's subprocess module.
 Home-page: http://go.pelicandd.com/n/python-nicecall
 Author: Arseni Mourzenko
 Author-email: arseni.mourzenko@pelicandd.com
 License: MIT
 Description: While |python-subprocess|_ is great, it may not be the easiest library to use. This is the reason I created ``nicecall``: it allows to do simple tasks with processes very easily.
```

### Comparing `nicecall-1.0.8/nicecall.egg-info/PKG-INFO` & `nicecall-1.0.9/nicecall.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: nicecall
-Version: 1.0.8
+Version: 1.0.9
 Summary: A library which provides a slightly more convinient way to launch processes, compared to Python's subprocess module.
 Home-page: http://go.pelicandd.com/n/python-nicecall
 Author: Arseni Mourzenko
 Author-email: arseni.mourzenko@pelicandd.com
 License: MIT
 Description: While |python-subprocess|_ is great, it may not be the easiest library to use. This is the reason I created ``nicecall``: it allows to do simple tasks with processes very easily.
```

### Comparing `nicecall-1.0.8/nicecall/logger.py` & `nicecall-1.0.9/nicecall/logger.py`

 * *Files identical despite different names*

### Comparing `nicecall-1.0.8/nicecall/tests/process_stub.py` & `nicecall-1.0.9/nicecall/tests/process_stub.py`

 * *Files identical despite different names*

### Comparing `nicecall-1.0.8/nicecall/tests/process_mock_context.py` & `nicecall-1.0.9/nicecall/tests/process_mock_context.py`

 * *Files identical despite different names*

### Comparing `nicecall-1.0.8/nicecall/process.py` & `nicecall-1.0.9/nicecall/process.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
             exitcode = process.returncode
             if exitcode:
                 logger.warning(
                     "“%s” failed with exit code %s." % (log_command, exitcode))
 
             if exitcode != 0 and self._raise_if_error:
-                raise subprocess.CalledProcessError(args[0], exitcode)
+                raise subprocess.CalledProcessError(exitcode, args[0])
 
             return exitcode
 
     def read_stdout(self, args):
         stdout = []
         self.on_stdout(stdout.append).raise_if_error().execute(args)
         return stdout
```

### Comparing `nicecall-1.0.8/README.rst` & `nicecall-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `nicecall-1.0.8/setup.py` & `nicecall-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 import setuptools
 
 setuptools.setup(
     name="nicecall",
-    version="1.0.8",
+    version="1.0.9",
     description="A library which provides a slightly more convinient way to "
                 "launch processes, compared to Python's subprocess module.",
     long_description=open("README.rst").read(),
     author="Arseni Mourzenko",
     author_email="arseni.mourzenko@pelicandd.com",
     url="http://go.pelicandd.com/n/python-nicecall",
     license="MIT",
```

