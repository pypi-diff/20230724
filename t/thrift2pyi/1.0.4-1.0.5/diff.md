# Comparing `tmp/thrift2pyi-1.0.4.tar.gz` & `tmp/thrift2pyi-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thrift2pyi-1.0.4.tar", last modified: Thu Jun 15 09:04:45 2023, max compression
+gzip compressed data, was "thrift2pyi-1.0.5.tar", last modified: Mon Jul 24 03:28:52 2023, max compression
```

## Comparing `thrift2pyi-1.0.4.tar` & `thrift2pyi-1.0.5.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-06-15 09:04:45.172662 thrift2pyi-1.0.4/
--rw-r--r--   0 bytedance   (502) staff       (20)     1056 2023-06-15 06:01:06.000000 thrift2pyi-1.0.4/LICENSE
--rw-r--r--   0 bytedance   (502) staff       (20)       18 2023-06-15 06:01:06.000000 thrift2pyi-1.0.4/MANIFEST.in
--rw-r--r--   0 bytedance   (502) staff       (20)     3968 2023-06-15 09:04:45.172052 thrift2pyi-1.0.4/PKG-INFO
--rw-r--r--   0 bytedance   (502) staff       (20)     3427 2023-06-15 06:01:06.000000 thrift2pyi-1.0.4/README.md
--rw-r--r--   0 bytedance   (502) staff       (20)       38 2023-06-15 09:04:45.172846 thrift2pyi-1.0.4/setup.cfg
--rw-r--r--   0 bytedance   (502) staff       (20)     1998 2023-06-15 06:01:06.000000 thrift2pyi-1.0.4/setup.py
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-06-15 09:04:45.166404 thrift2pyi-1.0.4/thrift2pyi/
--rw-r--r--   0 bytedance   (502) staff       (20)      264 2023-06-15 06:01:06.000000 thrift2pyi-1.0.4/thrift2pyi/__init__.py
--rw-r--r--   0 bytedance   (502) staff       (20)      239 2023-06-15 06:01:06.000000 thrift2pyi-1.0.4/thrift2pyi/__main__.py
--rw-r--r--   0 bytedance   (502) staff       (20)       63 2023-06-15 06:05:30.000000 thrift2pyi-1.0.4/thrift2pyi/__version__.py
--rw-r--r--   0 bytedance   (502) staff       (20)    10306 2023-06-15 06:10:28.000000 thrift2pyi-1.0.4/thrift2pyi/convert.py
--rw-r--r--   0 bytedance   (502) staff       (20)      215 2023-06-15 06:01:06.000000 thrift2pyi-1.0.4/thrift2pyi/exceptions.py
--rw-r--r--   0 bytedance   (502) staff       (20)      593 2023-06-15 06:01:06.000000 thrift2pyi-1.0.4/thrift2pyi/main.py
--rw-r--r--   0 bytedance   (502) staff       (20)     3080 2023-06-15 06:01:06.000000 thrift2pyi-1.0.4/thrift2pyi/peg.py
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-06-15 09:04:45.171248 thrift2pyi-1.0.4/thrift2pyi.egg-info/
--rw-r--r--   0 bytedance   (502) staff       (20)     3968 2023-06-15 09:04:45.000000 thrift2pyi-1.0.4/thrift2pyi.egg-info/PKG-INFO
--rw-r--r--   0 bytedance   (502) staff       (20)      400 2023-06-15 09:04:45.000000 thrift2pyi-1.0.4/thrift2pyi.egg-info/SOURCES.txt
--rw-r--r--   0 bytedance   (502) staff       (20)        1 2023-06-15 09:04:45.000000 thrift2pyi-1.0.4/thrift2pyi.egg-info/dependency_links.txt
--rw-r--r--   0 bytedance   (502) staff       (20)       52 2023-06-15 09:04:45.000000 thrift2pyi-1.0.4/thrift2pyi.egg-info/entry_points.txt
--rw-r--r--   0 bytedance   (502) staff       (20)      232 2023-06-15 09:04:45.000000 thrift2pyi-1.0.4/thrift2pyi.egg-info/requires.txt
--rw-r--r--   0 bytedance   (502) staff       (20)       11 2023-06-15 09:04:45.000000 thrift2pyi-1.0.4/thrift2pyi.egg-info/top_level.txt
+drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-07-24 03:28:52.778825 thrift2pyi-1.0.5/
+-rw-r--r--   0 bytedance   (502) staff       (20)     1056 2023-06-15 06:01:06.000000 thrift2pyi-1.0.5/LICENSE
+-rw-r--r--   0 bytedance   (502) staff       (20)       18 2023-06-15 06:01:06.000000 thrift2pyi-1.0.5/MANIFEST.in
+-rw-r--r--   0 bytedance   (502) staff       (20)     4128 2023-07-24 03:28:52.778484 thrift2pyi-1.0.5/PKG-INFO
+-rw-r--r--   0 bytedance   (502) staff       (20)     3444 2023-07-24 03:23:39.000000 thrift2pyi-1.0.5/README.md
+-rw-r--r--   0 bytedance   (502) staff       (20)      697 2023-07-24 03:23:39.000000 thrift2pyi-1.0.5/pyproject.toml
+-rw-r--r--   0 bytedance   (502) staff       (20)       38 2023-07-24 03:28:52.778926 thrift2pyi-1.0.5/setup.cfg
+-rw-r--r--   0 bytedance   (502) staff       (20)     1998 2023-06-15 06:01:06.000000 thrift2pyi-1.0.5/setup.py
+drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-07-24 03:28:52.774650 thrift2pyi-1.0.5/thrift2pyi/
+-rw-r--r--   0 bytedance   (502) staff       (20)      264 2023-06-15 06:01:06.000000 thrift2pyi-1.0.5/thrift2pyi/__init__.py
+-rw-r--r--   0 bytedance   (502) staff       (20)      239 2023-06-15 06:01:06.000000 thrift2pyi-1.0.5/thrift2pyi/__main__.py
+-rw-r--r--   0 bytedance   (502) staff       (20)       63 2023-07-24 03:23:39.000000 thrift2pyi-1.0.5/thrift2pyi/__version__.py
+-rw-r--r--   0 bytedance   (502) staff       (20)    10306 2023-07-24 03:19:26.000000 thrift2pyi-1.0.5/thrift2pyi/convert.py
+-rw-r--r--   0 bytedance   (502) staff       (20)      215 2023-06-15 06:01:06.000000 thrift2pyi-1.0.5/thrift2pyi/exceptions.py
+-rw-r--r--   0 bytedance   (502) staff       (20)      593 2023-06-15 06:01:06.000000 thrift2pyi-1.0.5/thrift2pyi/main.py
+-rw-r--r--   0 bytedance   (502) staff       (20)     3080 2023-06-15 06:01:06.000000 thrift2pyi-1.0.5/thrift2pyi/peg.py
+drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-07-24 03:28:52.777766 thrift2pyi-1.0.5/thrift2pyi.egg-info/
+-rw-r--r--   0 bytedance   (502) staff       (20)     4128 2023-07-24 03:28:52.000000 thrift2pyi-1.0.5/thrift2pyi.egg-info/PKG-INFO
+-rw-r--r--   0 bytedance   (502) staff       (20)      415 2023-07-24 03:28:52.000000 thrift2pyi-1.0.5/thrift2pyi.egg-info/SOURCES.txt
+-rw-r--r--   0 bytedance   (502) staff       (20)        1 2023-07-24 03:28:52.000000 thrift2pyi-1.0.5/thrift2pyi.egg-info/dependency_links.txt
+-rw-r--r--   0 bytedance   (502) staff       (20)       52 2023-07-24 03:28:52.000000 thrift2pyi-1.0.5/thrift2pyi.egg-info/entry_points.txt
+-rw-r--r--   0 bytedance   (502) staff       (20)      232 2023-07-24 03:28:52.000000 thrift2pyi-1.0.5/thrift2pyi.egg-info/requires.txt
+-rw-r--r--   0 bytedance   (502) staff       (20)       11 2023-07-24 03:28:52.000000 thrift2pyi-1.0.5/thrift2pyi.egg-info/top_level.txt
```

### Comparing `thrift2pyi-1.0.4/LICENSE` & `thrift2pyi-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `thrift2pyi-1.0.4/PKG-INFO` & `thrift2pyi-1.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: thrift2pyi
-Version: 1.0.4
+Version: 1.0.5
 Summary: convert thrift to pyi
 Author: yanweizhi
-Author-email: yanweizhi@bytedance.com
+Author-email: yanweizhi <yanweizhi@bytedance.com>
+Project-URL: Homepage, https://github.com/pypa/sampleproject
+Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: thrift2pyi
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-
 # thrift2pyi
 convert thrift to pyi
 
 # How to use
 pip install thrift2pyi
 
 thrift2pyi tests/example.thrift
@@ -56,14 +57,15 @@
     11: map<a.A, a.A> K
     12: map<string, bool> L = {}
     13: map<string, list<map<string, a.A>>> M
     14: list<a.A> N
     15: list<string> O
     16: set<i16> P
     17: list<map<string, a.A>> Q
+    18: binary R
 }
 
 enum ExampleEnum {
     A = 0
     B = 1
     C = 2
 }
```

### Comparing `thrift2pyi-1.0.4/README.md` & `thrift2pyi-1.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     11: map<a.A, a.A> K
     12: map<string, bool> L = {}
     13: map<string, list<map<string, a.A>>> M
     14: list<a.A> N
     15: list<string> O
     16: set<i16> P
     17: list<map<string, a.A>> Q
+    18: binary R
 }
 
 enum ExampleEnum {
     A = 0
     B = 1
     C = 2
 }
```

### Comparing `thrift2pyi-1.0.4/setup.py` & `thrift2pyi-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `thrift2pyi-1.0.4/thrift2pyi/convert.py` & `thrift2pyi-1.0.5/thrift2pyi/convert.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -56,14 +56,16 @@
                 return "bool"
             elif thrift_type in [TType.BYTE, TType.I08, TType.I16, TType.I32, TType.I64]:
                 return "int"
             elif thrift_type in [TType.STRING, TType.UTF7]:
                 return "str"
             elif thrift_type in [TType.DOUBLE]:
                 return "float"
+            elif thrift_type in [TType.BINARY]:
+                return "bytes"
             else:
                 raise Thrift2pyiException("do not type support %s" % thrift_type)
         else:
             thrift_type, nest = args
             if thrift_type == TType.STRUCT:
                 # (12, 'I', <class 'base.Base'>, False)
                 if nest.__module__ == self.thrift.__name__:
@@ -77,16 +79,14 @@
                 return "List[%s]" % self._get_type(nest)
             elif thrift_type == TType.MAP:
                 self._imports["typing"].add("Dict")
                 return "Dict[%s,%s]" % (self._get_type(nest[0]), self._get_type(nest[1]))
             elif thrift_type == TType.SET:
                 self._imports["typing"].add("Set")
                 return "Set[%s]" % self._get_type(nest)
-            elif thrift_type in [TType.BINARY]:
-                return "bytes"
             elif thrift_type == TType.I32:
                 return u(nest.__name__)
             else:
                 raise Thrift2pyiException("do not type support %s" % thrift_type)
 
     def _spec2type(self, spec):
         if len(spec) == 3:
```

### Comparing `thrift2pyi-1.0.4/thrift2pyi/main.py` & `thrift2pyi-1.0.5/thrift2pyi/main.py`

 * *Files identical despite different names*

### Comparing `thrift2pyi-1.0.4/thrift2pyi/peg.py` & `thrift2pyi-1.0.5/thrift2pyi/peg.py`

 * *Files identical despite different names*

### Comparing `thrift2pyi-1.0.4/thrift2pyi.egg-info/PKG-INFO` & `thrift2pyi-1.0.5/thrift2pyi.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: thrift2pyi
-Version: 1.0.4
+Version: 1.0.5
 Summary: convert thrift to pyi
 Author: yanweizhi
-Author-email: yanweizhi@bytedance.com
+Author-email: yanweizhi <yanweizhi@bytedance.com>
+Project-URL: Homepage, https://github.com/pypa/sampleproject
+Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: thrift2pyi
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-
 # thrift2pyi
 convert thrift to pyi
 
 # How to use
 pip install thrift2pyi
 
 thrift2pyi tests/example.thrift
@@ -56,14 +57,15 @@
     11: map<a.A, a.A> K
     12: map<string, bool> L = {}
     13: map<string, list<map<string, a.A>>> M
     14: list<a.A> N
     15: list<string> O
     16: set<i16> P
     17: list<map<string, a.A>> Q
+    18: binary R
 }
 
 enum ExampleEnum {
     A = 0
     B = 1
     C = 2
 }
```

