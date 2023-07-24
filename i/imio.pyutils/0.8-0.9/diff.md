# Comparing `tmp/imio.pyutils-0.8.tar.gz` & `tmp/imio.pyutils-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/imio.pyutils-0.8.tar", last modified: Wed Jul 19 13:17:40 2017, max compression
+gzip compressed data, was "dist/imio.pyutils-0.9.tar", last modified: Fri Jul 28 11:59:14 2017, max compression
```

## Comparing `imio.pyutils-0.8.tar` & `imio.pyutils-0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2017-07-19 13:17:40.000000 imio.pyutils-0.8/
--rw-rw-r--   0 sge       (1000) sge       (1000)       38 2017-07-19 13:17:40.000000 imio.pyutils-0.8/setup.cfg
--rw-rw-r--   0 sge       (1000) sge       (1000)     2518 2017-07-19 13:17:40.000000 imio.pyutils-0.8/PKG-INFO
--rw-rw-r--   0 sge       (1000) sge       (1000)      933 2017-07-19 13:17:39.000000 imio.pyutils-0.8/setup.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      657 2017-07-19 13:17:39.000000 imio.pyutils-0.8/README.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)       14 2017-07-19 13:17:39.000000 imio.pyutils-0.8/MANIFEST.in
--rw-rw-r--   0 sge       (1000) sge       (1000)      807 2017-07-19 13:17:39.000000 imio.pyutils-0.8/CHANGES.rst
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2017-07-19 13:17:40.000000 imio.pyutils-0.8/imio.pyutils.egg-info/
--rw-rw-r--   0 sge       (1000) sge       (1000)        5 2017-07-19 13:17:40.000000 imio.pyutils-0.8/imio.pyutils.egg-info/top_level.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)       11 2017-07-19 13:17:40.000000 imio.pyutils-0.8/imio.pyutils.egg-info/requires.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)        1 2017-07-19 13:17:40.000000 imio.pyutils-0.8/imio.pyutils.egg-info/not-zip-safe
--rw-rw-r--   0 sge       (1000) sge       (1000)        5 2017-07-19 13:17:40.000000 imio.pyutils-0.8/imio.pyutils.egg-info/namespace_packages.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)       37 2017-07-19 13:17:40.000000 imio.pyutils-0.8/imio.pyutils.egg-info/entry_points.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)        1 2017-07-19 13:17:40.000000 imio.pyutils-0.8/imio.pyutils.egg-info/dependency_links.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)      450 2017-07-19 13:17:40.000000 imio.pyutils-0.8/imio.pyutils.egg-info/SOURCES.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)     2518 2017-07-19 13:17:40.000000 imio.pyutils-0.8/imio.pyutils.egg-info/PKG-INFO
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2017-07-19 13:17:40.000000 imio.pyutils-0.8/imio/
--rw-rw-r--   0 sge       (1000) sge       (1000)      244 2017-07-19 13:17:39.000000 imio.pyutils-0.8/imio/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2017-07-19 13:17:40.000000 imio.pyutils-0.8/imio/pyutils/
--rw-rw-r--   0 sge       (1000) sge       (1000)     7735 2017-07-19 13:17:39.000000 imio.pyutils-0.8/imio/pyutils/system.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     4695 2017-07-19 13:17:39.000000 imio.pyutils-0.8/imio/pyutils/postgres.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1383 2017-07-19 13:17:39.000000 imio.pyutils-0.8/imio/pyutils/bs.py
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2017-07-19 13:17:39.000000 imio.pyutils-0.8/imio/pyutils/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2017-07-28 11:59:14.000000 imio.pyutils-0.9/
+-rw-rw-r--   0 sge       (1000) sge       (1000)       38 2017-07-28 11:59:14.000000 imio.pyutils-0.9/setup.cfg
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2643 2017-07-28 11:59:14.000000 imio.pyutils-0.9/PKG-INFO
+-rw-rw-r--   0 sge       (1000) sge       (1000)      933 2017-07-28 11:59:14.000000 imio.pyutils-0.9/setup.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      657 2017-07-28 11:59:14.000000 imio.pyutils-0.9/README.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)       14 2017-07-28 11:59:14.000000 imio.pyutils-0.9/MANIFEST.in
+-rw-rw-r--   0 sge       (1000) sge       (1000)      884 2017-07-28 11:59:14.000000 imio.pyutils-0.9/CHANGES.rst
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2017-07-28 11:59:14.000000 imio.pyutils-0.9/imio.pyutils.egg-info/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        5 2017-07-28 11:59:14.000000 imio.pyutils-0.9/imio.pyutils.egg-info/top_level.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)       11 2017-07-28 11:59:14.000000 imio.pyutils-0.9/imio.pyutils.egg-info/requires.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)        1 2017-07-28 11:59:14.000000 imio.pyutils-0.9/imio.pyutils.egg-info/not-zip-safe
+-rw-rw-r--   0 sge       (1000) sge       (1000)        5 2017-07-28 11:59:14.000000 imio.pyutils-0.9/imio.pyutils.egg-info/namespace_packages.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)       37 2017-07-28 11:59:14.000000 imio.pyutils-0.9/imio.pyutils.egg-info/entry_points.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)        1 2017-07-28 11:59:14.000000 imio.pyutils-0.9/imio.pyutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)      450 2017-07-28 11:59:14.000000 imio.pyutils-0.9/imio.pyutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2643 2017-07-28 11:59:14.000000 imio.pyutils-0.9/imio.pyutils.egg-info/PKG-INFO
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2017-07-28 11:59:14.000000 imio.pyutils-0.9/imio/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      244 2017-07-28 11:59:14.000000 imio.pyutils-0.9/imio/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2017-07-28 11:59:14.000000 imio.pyutils-0.9/imio/pyutils/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     8679 2017-07-28 11:59:14.000000 imio.pyutils-0.9/imio/pyutils/system.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     4695 2017-07-28 11:59:14.000000 imio.pyutils-0.9/imio/pyutils/postgres.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1383 2017-07-28 11:59:14.000000 imio.pyutils-0.9/imio/pyutils/bs.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2017-07-28 11:59:14.000000 imio.pyutils-0.9/imio/pyutils/__init__.py
```

### Comparing `imio.pyutils-0.8/PKG-INFO` & `imio.pyutils-0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: imio.pyutils
-Version: 0.8
+Version: 0.9
 Summary: Some python useful methods
 Home-page: http://github.com/imio/imio.pyutils/
 Author: IMIO
 Author-email: support@imio.be
 License: GPL
 Description: .. contents::
         
@@ -42,14 +42,20 @@
         * single or multiple select,
         * insert, update, delete rows,
         * etc.
         
         Changelog
         =========
         
+        0.9 (2017-07-28)
+        ----------------
+        
+        - Added read_csv function.
+          [sgeulette]
+        
         0.8 (2017-07-19)
         ----------------
         
         - runCommand can append to file.
           [sgeulette]
         
         0.7 (2017-06-26)
```

### Comparing `imio.pyutils-0.8/setup.py` & `imio.pyutils-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = '0.8'
+version = '0.9'
 
 setup(name='imio.pyutils',
       version=version,
       description="Some python useful methods",
       long_description=open("README.rst").read() + "\n" + open('CHANGES.rst').read(),
       # Get more strings from
       # http://pypi.python.org/pypi?:action=list_classifiers
```

### Comparing `imio.pyutils-0.8/README.rst` & `imio.pyutils-0.9/README.rst`

 * *Files identical despite different names*

### Comparing `imio.pyutils-0.8/CHANGES.rst` & `imio.pyutils-0.9/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+0.9 (2017-07-28)
+----------------
+
+- Added read_csv function.
+  [sgeulette]
+
 0.8 (2017-07-19)
 ----------------
 
 - runCommand can append to file.
   [sgeulette]
 
 0.7 (2017-06-26)
```

### Comparing `imio.pyutils-0.8/imio.pyutils.egg-info/PKG-INFO` & `imio.pyutils-0.9/imio.pyutils.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: imio.pyutils
-Version: 0.8
+Version: 0.9
 Summary: Some python useful methods
 Home-page: http://github.com/imio/imio.pyutils/
 Author: IMIO
 Author-email: support@imio.be
 License: GPL
 Description: .. contents::
         
@@ -42,14 +42,20 @@
         * single or multiple select,
         * insert, update, delete rows,
         * etc.
         
         Changelog
         =========
         
+        0.9 (2017-07-28)
+        ----------------
+        
+        - Added read_csv function.
+          [sgeulette]
+        
         0.8 (2017-07-19)
         ----------------
         
         - runCommand can append to file.
           [sgeulette]
         
         0.7 (2017-06-26)
```

### Comparing `imio.pyutils-0.8/imio/pyutils/system.py` & `imio.pyutils-0.9/imio/pyutils/system.py`

 * *Files 10% similar despite different names*

```diff
@@ -77,14 +77,45 @@
         lines.append(line)
     thefile.close()
     return lines
 
 #------------------------------------------------------------------------------
 
 
+def read_csv(filename, strip_chars='', replace_dq=True, skip_empty=False, skip_lines=0, **kwargs):
+    """ read a csv file and return lines """
+    lines = []
+    try:
+        thefile = open(filename, 'r')
+    except IOError:
+        error("! Cannot open %s file" % filename)
+        return lines
+    import csv
+    for i, data in enumerate(csv.reader(thefile, **kwargs)):
+        if skip_lines and i < skip_lines:
+            continue
+        replaced = []
+        empty = True
+        for item in data:
+            if replace_dq:
+                item = item.replace('""', '"')
+            if strip_chars:
+                item = item.strip(strip_chars)
+            if item:
+                empty = False
+            replaced.append(item)
+        if skip_empty and empty:
+            continue
+        lines.append(replaced)
+    thefile.close()
+    return lines
+
+#------------------------------------------------------------------------------
+
+
 def read_dir(dirpath, with_path=False, only_folders=False, only_files=False):
     """ Read the dir and return files """
     files = []
     for filename in os.listdir(dirpath):
         if only_folders and not os.path.isdir(os.path.join(dirpath, filename)):
             continue
         if only_files and not os.path.isfile(os.path.join(dirpath, filename)):
```

### Comparing `imio.pyutils-0.8/imio/pyutils/postgres.py` & `imio.pyutils-0.9/imio/pyutils/postgres.py`

 * *Files identical despite different names*

### Comparing `imio.pyutils-0.8/imio/pyutils/bs.py` & `imio.pyutils-0.9/imio/pyutils/bs.py`

 * *Files identical despite different names*

