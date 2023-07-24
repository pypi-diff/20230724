# Comparing `tmp/testgres-1.8.8.tar.gz` & `tmp/testgres-1.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testgres-1.8.8.tar", last modified: Wed Jun  7 02:32:48 2023, max compression
+gzip compressed data, was "testgres-1.8.9.tar", last modified: Mon Jul 24 11:39:41 2023, max compression
```

## Comparing `testgres-1.8.8.tar` & `testgres-1.8.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 pge       (1003) pge       (1003)        0 2023-06-07 02:32:48.621387 testgres-1.8.8/
--rw-rw-r--   0 pge       (1003) pge       (1003)     1106 2023-05-10 11:22:06.000000 testgres-1.8.8/LICENSE
--rw-rw-r--   0 pge       (1003) pge       (1003)      136 2022-02-22 09:57:57.000000 testgres-1.8.8/MANIFEST.in
--rw-rw-r--   0 pge       (1003) pge       (1003)     7198 2023-06-07 02:32:48.621387 testgres-1.8.8/PKG-INFO
--rw-rw-r--   0 pge       (1003) pge       (1003)     5399 2023-05-05 04:23:08.000000 testgres-1.8.8/README.md
--rw-rw-r--   0 pge       (1003) pge       (1003)      160 2023-06-07 02:32:48.621387 testgres-1.8.8/setup.cfg
--rwxrwxr-x   0 pge       (1003) pge       (1003)     1011 2023-06-07 02:28:30.000000 testgres-1.8.8/setup.py
-drwxrwxr-x   0 pge       (1003) pge       (1003)        0 2023-06-07 02:32:48.621387 testgres-1.8.8/testgres/
--rw-rw-r--   0 pge       (1003) pge       (1003)     1519 2023-05-05 04:23:08.000000 testgres-1.8.8/testgres/__init__.py
--rw-rw-r--   0 pge       (1003) pge       (1003)     1524 2022-02-22 09:57:57.000000 testgres-1.8.8/testgres/api.py
--rw-rw-r--   0 pge       (1003) pge       (1003)     5187 2022-05-06 11:01:56.000000 testgres-1.8.8/testgres/backup.py
--rw-rw-r--   0 pge       (1003) pge       (1003)     2195 2022-05-06 11:01:56.000000 testgres-1.8.8/testgres/cache.py
--rw-rw-r--   0 pge       (1003) pge       (1003)     4781 2022-05-06 11:01:56.000000 testgres-1.8.8/testgres/config.py
--rw-rw-r--   0 pge       (1003) pge       (1003)     3080 2022-05-06 11:01:56.000000 testgres-1.8.8/testgres/connection.py
--rw-rw-r--   0 pge       (1003) pge       (1003)      819 2022-02-22 09:57:57.000000 testgres-1.8.8/testgres/consts.py
--rw-rw-r--   0 pge       (1003) pge       (1003)     1749 2022-05-06 11:01:56.000000 testgres-1.8.8/testgres/decorators.py
--rw-rw-r--   0 pge       (1003) pge       (1003)      932 2022-02-22 09:57:57.000000 testgres-1.8.8/testgres/defaults.py
--rw-rw-r--   0 pge       (1003) pge       (1003)     2451 2023-05-05 04:23:08.000000 testgres-1.8.8/testgres/enums.py
--rw-rw-r--   0 pge       (1003) pge       (1003)     1988 2022-02-22 09:57:57.000000 testgres-1.8.8/testgres/exceptions.py
--rw-rw-r--   0 pge       (1003) pge       (1003)     1428 2022-05-06 11:01:56.000000 testgres-1.8.8/testgres/logger.py
--rw-rw-r--   0 pge       (1003) pge       (1003)    51775 2023-06-07 02:28:30.000000 testgres-1.8.8/testgres/node.py
--rw-rw-r--   0 pge       (1003) pge       (1003)     8225 2022-05-06 11:01:56.000000 testgres-1.8.8/testgres/pubsub.py
--rw-rw-r--   0 pge       (1003) pge       (1003)     1547 2022-05-06 11:01:56.000000 testgres-1.8.8/testgres/standby.py
--rw-rw-r--   0 pge       (1003) pge       (1003)     6360 2023-06-07 02:28:30.000000 testgres-1.8.8/testgres/utils.py
-drwxrwxr-x   0 pge       (1003) pge       (1003)        0 2023-06-07 02:32:48.621387 testgres-1.8.8/testgres.egg-info/
--rw-rw-r--   0 pge       (1003) pge       (1003)     7198 2023-06-07 02:32:48.000000 testgres-1.8.8/testgres.egg-info/PKG-INFO
--rw-rw-r--   0 pge       (1003) pge       (1003)      541 2023-06-07 02:32:48.000000 testgres-1.8.8/testgres.egg-info/SOURCES.txt
--rw-rw-r--   0 pge       (1003) pge       (1003)        1 2023-06-07 02:32:48.000000 testgres-1.8.8/testgres.egg-info/dependency_links.txt
--rw-rw-r--   0 pge       (1003) pge       (1003)       49 2023-06-07 02:32:48.000000 testgres-1.8.8/testgres.egg-info/requires.txt
--rw-rw-r--   0 pge       (1003) pge       (1003)        9 2023-06-07 02:32:48.000000 testgres-1.8.8/testgres.egg-info/top_level.txt
-drwxrwxr-x   0 pge       (1003) pge       (1003)        0 2023-06-07 02:32:48.621387 testgres-1.8.8/tests/
--rwxrwxr-x   0 pge       (1003) pge       (1003)    34618 2023-05-05 04:23:08.000000 testgres-1.8.8/tests/test_simple.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:39:41.548547 testgres-1.8.9/
+-rw-rw-r--   0 root         (0) root         (0)     1106 2023-05-10 11:22:06.000000 testgres-1.8.9/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      136 2022-02-22 09:57:57.000000 testgres-1.8.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5753 2023-07-24 11:39:41.548547 testgres-1.8.9/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     5399 2023-05-05 04:23:08.000000 testgres-1.8.9/README.md
+-rw-rw-r--   0 root         (0) root         (0)      160 2023-07-24 11:39:41.552547 testgres-1.8.9/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)     1011 2023-07-24 11:28:45.000000 testgres-1.8.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:39:41.544546 testgres-1.8.9/testgres/
+-rw-rw-r--   0 root         (0) root         (0)     1519 2023-05-05 04:23:08.000000 testgres-1.8.9/testgres/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1524 2022-02-22 09:57:57.000000 testgres-1.8.9/testgres/api.py
+-rw-rw-r--   0 root         (0) root         (0)     5187 2022-05-06 11:01:56.000000 testgres-1.8.9/testgres/backup.py
+-rw-rw-r--   0 root         (0) root         (0)     2195 2022-05-06 11:01:56.000000 testgres-1.8.9/testgres/cache.py
+-rw-rw-r--   0 root         (0) root         (0)     4781 2022-05-06 11:01:56.000000 testgres-1.8.9/testgres/config.py
+-rw-rw-r--   0 root         (0) root         (0)     3080 2022-05-06 11:01:56.000000 testgres-1.8.9/testgres/connection.py
+-rw-rw-r--   0 root         (0) root         (0)      819 2022-02-22 09:57:57.000000 testgres-1.8.9/testgres/consts.py
+-rw-rw-r--   0 root         (0) root         (0)     1749 2022-05-06 11:01:56.000000 testgres-1.8.9/testgres/decorators.py
+-rw-rw-r--   0 root         (0) root         (0)      932 2022-02-22 09:57:57.000000 testgres-1.8.9/testgres/defaults.py
+-rw-rw-r--   0 root         (0) root         (0)     2451 2023-05-05 04:23:08.000000 testgres-1.8.9/testgres/enums.py
+-rw-rw-r--   0 root         (0) root         (0)     1988 2022-02-22 09:57:57.000000 testgres-1.8.9/testgres/exceptions.py
+-rw-rw-r--   0 root         (0) root         (0)     1428 2022-05-06 11:01:56.000000 testgres-1.8.9/testgres/logger.py
+-rw-rw-r--   0 root         (0) root         (0)    51775 2023-06-07 02:28:30.000000 testgres-1.8.9/testgres/node.py
+-rw-rw-r--   0 root         (0) root         (0)     8225 2022-05-06 11:01:56.000000 testgres-1.8.9/testgres/pubsub.py
+-rw-rw-r--   0 root         (0) root         (0)     1547 2022-05-06 11:01:56.000000 testgres-1.8.9/testgres/standby.py
+-rw-rw-r--   0 root         (0) root         (0)     6616 2023-07-24 09:08:31.000000 testgres-1.8.9/testgres/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:39:41.548547 testgres-1.8.9/testgres.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)     5753 2023-07-24 11:39:41.000000 testgres-1.8.9/testgres.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      541 2023-07-24 11:39:41.000000 testgres-1.8.9/testgres.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-07-24 11:39:41.000000 testgres-1.8.9/testgres.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)       49 2023-07-24 11:39:41.000000 testgres-1.8.9/testgres.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)        9 2023-07-24 11:39:41.000000 testgres-1.8.9/testgres.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:39:41.548547 testgres-1.8.9/tests/
+-rwxrwxr-x   0 root         (0) root         (0)    34865 2023-07-24 09:08:31.000000 testgres-1.8.9/tests/test_simple.py
```

### Comparing `testgres-1.8.8/LICENSE` & `testgres-1.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `testgres-1.8.8/README.md` & `testgres-1.8.9/README.md`

 * *Files identical despite different names*

### Comparing `testgres-1.8.8/setup.py` & `testgres-1.8.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     install_requires.append("ipaddress")
 
 # Get contents of README file
 with open('README.md', 'r') as f:
     readme = f.read()
 
 setup(
-    version='1.8.8',
+    version='1.8.9',
     name='testgres',
     packages=['testgres'],
     description='Testing utility for PostgreSQL and its extensions',
     url='https://github.com/postgrespro/testgres',
     long_description=readme,
     long_description_content_type='text/markdown',
     license='PostgreSQL',
```

### Comparing `testgres-1.8.8/testgres/__init__.py` & `testgres-1.8.9/testgres/__init__.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.8/testgres/api.py` & `testgres-1.8.9/testgres/api.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.8/testgres/backup.py` & `testgres-1.8.9/testgres/backup.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.8/testgres/cache.py` & `testgres-1.8.9/testgres/cache.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.8/testgres/config.py` & `testgres-1.8.9/testgres/config.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.8/testgres/connection.py` & `testgres-1.8.9/testgres/connection.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.8/testgres/consts.py` & `testgres-1.8.9/testgres/consts.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.8/testgres/decorators.py` & `testgres-1.8.9/testgres/decorators.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.8/testgres/defaults.py` & `testgres-1.8.9/testgres/defaults.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.8/testgres/enums.py` & `testgres-1.8.9/testgres/enums.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.8/testgres/exceptions.py` & `testgres-1.8.9/testgres/exceptions.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.8/testgres/logger.py` & `testgres-1.8.9/testgres/logger.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.8/testgres/node.py` & `testgres-1.8.9/testgres/node.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.8/testgres/pubsub.py` & `testgres-1.8.9/testgres/pubsub.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.8/testgres/standby.py` & `testgres-1.8.9/testgres/standby.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.8/testgres/utils.py` & `testgres-1.8.9/testgres/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 import os
 import port_for
 import subprocess
 import sys
 import tempfile
 
 from contextlib import contextmanager
-from packaging.version import Version
+from packaging.version import Version, InvalidVersion
+import re
 try:
     from shutil import which as find_executable
 except ImportError:
     from distutils.spawn import find_executable
 from six import iteritems
 
 from .config import testgres_config
@@ -23,16 +24,23 @@
 
 # rows returned by PG_CONFIG
 _pg_config_data = {}
 
 # ports used by nodes
 bound_ports = set()
 
+
 # re-export version type
-PgVer = Version
+class PgVer(Version):
+    def __init__(self, version: str) -> None:
+        try:
+            super().__init__(version)
+        except InvalidVersion:
+            version = re.sub(r"[a-zA-Z].*", "", version)
+            super().__init__(version)
 
 
 def reserve_port():
     """
     Generate a new port and add it to 'bound_ports'.
     """
```

### Comparing `testgres-1.8.8/testgres.egg-info/SOURCES.txt` & `testgres-1.8.9/testgres.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `testgres-1.8.8/tests/test_simple.py` & `testgres-1.8.9/tests/test_simple.py`

 * *Files 2% similar despite different names*

```diff
@@ -897,21 +897,29 @@
     def test_version_management(self):
         a = PgVer('10.0')
         b = PgVer('10')
         c = PgVer('9.6.5')
         d = PgVer('15.0')
         e = PgVer('15rc1')
         f = PgVer('15beta4')
+        h = PgVer('15.3biha')
+        i = PgVer('15.3')
+        g = PgVer('15.3.1bihabeta1')
+        k = PgVer('15.3.1')
 
         self.assertTrue(a == b)
         self.assertTrue(b > c)
         self.assertTrue(a > c)
         self.assertTrue(d > e)
         self.assertTrue(e > f)
         self.assertTrue(d > f)
+        self.assertTrue(h > f)
+        self.assertTrue(h == i)
+        self.assertTrue(g == k)
+        self.assertTrue(g > h)
 
         version = get_pg_version()
         with get_new_node() as node:
             self.assertTrue(isinstance(version, six.string_types))
             self.assertTrue(isinstance(node.version, PgVer))
             self.assertEqual(node.version, PgVer(version))
```

