# Comparing `tmp/r2diaphora-0.3.0.tar.gz` & `tmp/r2diaphora-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r2diaphora-0.3.0.tar", last modified: Thu Jul 13 09:08:13 2023, max compression
+gzip compressed data, was "r2diaphora-0.3.1.tar", last modified: Mon Jul 24 07:50:03 2023, max compression
```

## Comparing `r2diaphora-0.3.0.tar` & `r2diaphora-0.3.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-07-13 09:08:13.488363 r2diaphora-0.3.0/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)    34523 2023-05-16 15:00:43.000000 r2diaphora-0.3.0/LICENSE
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       82 2023-05-16 15:00:43.000000 r2diaphora-0.3.0/MANIFEST.in
--rw-rw-r--   0 fdd       (1000) fdd       (1000)      584 2023-07-13 09:08:13.488363 r2diaphora-0.3.0/PKG-INFO
--rw-rw-r--   0 fdd       (1000) fdd       (1000)     2425 2023-05-16 15:00:43.000000 r2diaphora-0.3.0/README.md
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-07-13 09:08:13.480360 r2diaphora-0.3.0/r2diaphora/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)      404 2023-05-16 15:00:43.000000 r2diaphora-0.3.0/r2diaphora/__init__.py
--rwxrwxr-x   0 fdd       (1000) fdd       (1000)    94459 2023-05-22 08:45:18.000000 r2diaphora-0.3.0/r2diaphora/diaphora.py
--rw-rw-r--   0 fdd       (1000) fdd       (1000)    57599 2023-05-16 15:00:43.000000 r2diaphora-0.3.0/r2diaphora/diaphora_heuristics.py
--rwxrwxr-x   0 fdd       (1000) fdd       (1000)    42812 2023-07-11 08:32:33.000000 r2diaphora-0.3.0/r2diaphora/diaphora_r2.py
--rw-rw-r--   0 fdd       (1000) fdd       (1000)     4604 2023-05-16 15:00:43.000000 r2diaphora-0.3.0/r2diaphora/difflibparser.py
--rw-rw-r--   0 fdd       (1000) fdd       (1000)    13283 2023-05-16 15:00:43.000000 r2diaphora-0.3.0/r2diaphora/html_diff.py
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-07-13 09:08:13.484362 r2diaphora-0.3.0/r2diaphora/idaapi/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)        0 2023-05-16 15:00:43.000000 r2diaphora-0.3.0/r2diaphora/idaapi/__init__.py
--rw-rw-r--   0 fdd       (1000) fdd       (1000)    21956 2023-07-11 12:46:42.000000 r2diaphora-0.3.0/r2diaphora/idaapi/idaapi_to_r2.py
--rw-rw-r--   0 fdd       (1000) fdd       (1000)    77880 2023-05-16 15:00:43.000000 r2diaphora-0.3.0/r2diaphora/idaapi/instructions.py
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-07-13 09:08:13.488363 r2diaphora-0.3.0/r2diaphora/jkutils/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)        0 2023-05-16 15:00:43.000000 r2diaphora-0.3.0/r2diaphora/jkutils/__init__.py
--rw-rw-r--   0 fdd       (1000) fdd       (1000)     6336 2023-05-16 15:00:43.000000 r2diaphora-0.3.0/r2diaphora/jkutils/factor.py
--rw-rw-r--   0 fdd       (1000) fdd       (1000)     6037 2023-05-16 15:00:43.000000 r2diaphora-0.3.0/r2diaphora/jkutils/graph_hashes.py
--rw-rw-r--   0 fdd       (1000) fdd       (1000)    10023 2023-05-16 15:00:43.000000 r2diaphora-0.3.0/r2diaphora/jkutils/kfuzzy.py
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-07-13 09:08:13.488363 r2diaphora-0.3.0/r2diaphora/others/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)        0 2023-05-16 15:00:43.000000 r2diaphora-0.3.0/r2diaphora/others/__init__.py
--rw-rw-r--   0 fdd       (1000) fdd       (1000)     2807 2023-05-16 15:00:43.000000 r2diaphora-0.3.0/r2diaphora/others/tarjan_sort.py
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-07-13 09:08:13.484362 r2diaphora-0.3.0/r2diaphora.egg-info/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)      584 2023-07-13 09:08:13.000000 r2diaphora-0.3.0/r2diaphora.egg-info/PKG-INFO
--rw-rw-r--   0 fdd       (1000) fdd       (1000)      743 2023-07-13 09:08:13.000000 r2diaphora-0.3.0/r2diaphora.egg-info/SOURCES.txt
--rw-rw-r--   0 fdd       (1000) fdd       (1000)        1 2023-07-13 09:08:13.000000 r2diaphora-0.3.0/r2diaphora.egg-info/dependency_links.txt
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       60 2023-07-13 09:08:13.000000 r2diaphora-0.3.0/r2diaphora.egg-info/entry_points.txt
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       91 2023-07-13 09:08:13.000000 r2diaphora-0.3.0/r2diaphora.egg-info/requires.txt
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       11 2023-07-13 09:08:13.000000 r2diaphora-0.3.0/r2diaphora.egg-info/top_level.txt
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-07-13 09:08:13.488363 r2diaphora-0.3.0/scripts/
--rwxrwxr-x   0 fdd       (1000) fdd       (1000)      802 2023-05-16 15:00:43.000000 r2diaphora-0.3.0/scripts/r2diaphora-bulk
--rw-rw-r--   0 fdd       (1000) fdd       (1000)     2231 2023-05-16 15:00:43.000000 r2diaphora-0.3.0/scripts/r2diaphora-db
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       79 2023-07-13 09:08:13.488363 r2diaphora-0.3.0/setup.cfg
--rw-rw-r--   0 fdd       (1000) fdd       (1000)     2226 2023-07-11 12:39:20.000000 r2diaphora-0.3.0/setup.py
+drwxr-xr-x   0 fdd        (501) staff       (20)        0 2023-07-24 07:50:03.597870 r2diaphora-0.3.1/
+-rw-r--r--   0 fdd        (501) staff       (20)    34523 2021-05-17 12:55:35.000000 r2diaphora-0.3.1/LICENSE
+-rw-r--r--   0 fdd        (501) staff       (20)       82 2021-10-20 18:26:44.000000 r2diaphora-0.3.1/MANIFEST.in
+-rw-r--r--   0 fdd        (501) staff       (20)      556 2023-07-24 07:50:03.598015 r2diaphora-0.3.1/PKG-INFO
+-rw-r--r--   0 fdd        (501) staff       (20)     2425 2021-11-09 19:44:19.000000 r2diaphora-0.3.1/README.md
+drwxr-xr-x   0 fdd        (501) staff       (20)        0 2023-07-24 07:50:03.587766 r2diaphora-0.3.1/r2diaphora/
+-rw-r--r--   0 fdd        (501) staff       (20)      404 2021-10-29 12:54:17.000000 r2diaphora-0.3.1/r2diaphora/__init__.py
+-rwxr-xr-x   0 fdd        (501) staff       (20)    94516 2023-07-24 07:49:51.000000 r2diaphora-0.3.1/r2diaphora/diaphora.py
+-rw-r--r--   0 fdd        (501) staff       (20)    57599 2021-10-07 10:12:37.000000 r2diaphora-0.3.1/r2diaphora/diaphora_heuristics.py
+-rwxr-xr-x   0 fdd        (501) staff       (20)    42812 2023-07-24 07:49:51.000000 r2diaphora-0.3.1/r2diaphora/diaphora_r2.py
+-rw-r--r--   0 fdd        (501) staff       (20)     4604 2021-10-11 09:22:38.000000 r2diaphora-0.3.1/r2diaphora/difflibparser.py
+-rw-r--r--   0 fdd        (501) staff       (20)    13283 2021-10-13 14:49:44.000000 r2diaphora-0.3.1/r2diaphora/html_diff.py
+drwxr-xr-x   0 fdd        (501) staff       (20)        0 2023-07-24 07:50:03.591831 r2diaphora-0.3.1/r2diaphora/idaapi/
+-rw-r--r--   0 fdd        (501) staff       (20)        0 2021-10-08 12:02:16.000000 r2diaphora-0.3.1/r2diaphora/idaapi/__init__.py
+-rw-r--r--   0 fdd        (501) staff       (20)    21956 2023-07-24 07:49:51.000000 r2diaphora-0.3.1/r2diaphora/idaapi/idaapi_to_r2.py
+-rw-r--r--   0 fdd        (501) staff       (20)    77880 2021-10-08 12:01:52.000000 r2diaphora-0.3.1/r2diaphora/idaapi/instructions.py
+drwxr-xr-x   0 fdd        (501) staff       (20)        0 2023-07-24 07:50:03.594636 r2diaphora-0.3.1/r2diaphora/jkutils/
+-rw-r--r--   0 fdd        (501) staff       (20)        0 2021-10-07 11:42:52.000000 r2diaphora-0.3.1/r2diaphora/jkutils/__init__.py
+-rw-r--r--   0 fdd        (501) staff       (20)     6336 2021-05-17 12:55:35.000000 r2diaphora-0.3.1/r2diaphora/jkutils/factor.py
+-rw-r--r--   0 fdd        (501) staff       (20)     6037 2023-07-24 07:49:51.000000 r2diaphora-0.3.1/r2diaphora/jkutils/graph_hashes.py
+-rw-r--r--   0 fdd        (501) staff       (20)    10023 2021-05-17 12:55:35.000000 r2diaphora-0.3.1/r2diaphora/jkutils/kfuzzy.py
+drwxr-xr-x   0 fdd        (501) staff       (20)        0 2023-07-24 07:50:03.595763 r2diaphora-0.3.1/r2diaphora/others/
+-rw-r--r--   0 fdd        (501) staff       (20)        0 2021-05-17 12:55:35.000000 r2diaphora-0.3.1/r2diaphora/others/__init__.py
+-rw-r--r--   0 fdd        (501) staff       (20)     2807 2021-09-30 08:22:55.000000 r2diaphora-0.3.1/r2diaphora/others/tarjan_sort.py
+drwxr-xr-x   0 fdd        (501) staff       (20)        0 2023-07-24 07:50:03.590574 r2diaphora-0.3.1/r2diaphora.egg-info/
+-rw-r--r--   0 fdd        (501) staff       (20)      556 2023-07-24 07:50:03.000000 r2diaphora-0.3.1/r2diaphora.egg-info/PKG-INFO
+-rw-r--r--   0 fdd        (501) staff       (20)      743 2023-07-24 07:50:03.000000 r2diaphora-0.3.1/r2diaphora.egg-info/SOURCES.txt
+-rw-r--r--   0 fdd        (501) staff       (20)        1 2023-07-24 07:50:03.000000 r2diaphora-0.3.1/r2diaphora.egg-info/dependency_links.txt
+-rw-r--r--   0 fdd        (501) staff       (20)       59 2023-07-24 07:50:03.000000 r2diaphora-0.3.1/r2diaphora.egg-info/entry_points.txt
+-rw-r--r--   0 fdd        (501) staff       (20)      112 2023-07-24 07:50:03.000000 r2diaphora-0.3.1/r2diaphora.egg-info/requires.txt
+-rw-r--r--   0 fdd        (501) staff       (20)       11 2023-07-24 07:50:03.000000 r2diaphora-0.3.1/r2diaphora.egg-info/top_level.txt
+drwxr-xr-x   0 fdd        (501) staff       (20)        0 2023-07-24 07:50:03.597338 r2diaphora-0.3.1/scripts/
+-rwxr--r--   0 fdd        (501) staff       (20)      802 2021-10-07 11:19:24.000000 r2diaphora-0.3.1/scripts/r2diaphora-bulk
+-rw-r--r--   0 fdd        (501) staff       (20)     2231 2021-11-09 19:44:41.000000 r2diaphora-0.3.1/scripts/r2diaphora-db
+-rw-r--r--   0 fdd        (501) staff       (20)       79 2023-07-24 07:50:03.598588 r2diaphora-0.3.1/setup.cfg
+-rw-r--r--   0 fdd        (501) staff       (20)     2258 2023-07-24 07:49:51.000000 r2diaphora-0.3.1/setup.py
```

### Comparing `r2diaphora-0.3.0/LICENSE` & `r2diaphora-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.3.0/PKG-INFO` & `r2diaphora-0.3.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 Metadata-Version: 2.1
 Name: r2diaphora
-Version: 0.3.0
+Version: 0.3.1
 Summary: radare2 port of diaphora
 Home-page: https://github.com/FernandoDoming/r2diaphora
 Author: Fernando Domínguez
 Author-email: fernando.dom.del@gmail.com
 License: GNU GPL v3
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `r2diaphora-0.3.0/README.md` & `r2diaphora-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.3.0/r2diaphora/diaphora.py` & `r2diaphora-0.3.1/r2diaphora/diaphora.py`

 * *Files 0% similar despite different names*

```diff
@@ -867,16 +867,17 @@
             ("name", 1024),
             ("mangled_function", 1024),
             ("prototype", 1024),
             ("prototype2", 1024),
         ]
         for size_limit in size_limits:
             idx = self.get_fn_prop_index(size_limit[0])
-            if idx == -1:
+            if idx == -1 or idx >= len(props) or not isinstance(props[idx], str):
                 continue
+
             props[idx] = props[idx][0:size_limit[1]]
 
     def get_fn_prop_index(self, key):
         keys = self.get_fn_prop_keys()
         idx = -1
         try:
             idx = keys.index(key)
```

### Comparing `r2diaphora-0.3.0/r2diaphora/diaphora_heuristics.py` & `r2diaphora-0.3.1/r2diaphora/diaphora_heuristics.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.3.0/r2diaphora/diaphora_r2.py` & `r2diaphora-0.3.1/r2diaphora/diaphora_r2.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.3.0/r2diaphora/difflibparser.py` & `r2diaphora-0.3.1/r2diaphora/difflibparser.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.3.0/r2diaphora/html_diff.py` & `r2diaphora-0.3.1/r2diaphora/html_diff.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.3.0/r2diaphora/idaapi/idaapi_to_r2.py` & `r2diaphora-0.3.1/r2diaphora/idaapi/idaapi_to_r2.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.3.0/r2diaphora/idaapi/instructions.py` & `r2diaphora-0.3.1/r2diaphora/idaapi/instructions.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.3.0/r2diaphora/jkutils/factor.py` & `r2diaphora-0.3.1/r2diaphora/jkutils/factor.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.3.0/r2diaphora/jkutils/graph_hashes.py` & `r2diaphora-0.3.1/r2diaphora/jkutils/graph_hashes.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.3.0/r2diaphora/jkutils/kfuzzy.py` & `r2diaphora-0.3.1/r2diaphora/jkutils/kfuzzy.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.3.0/r2diaphora/others/tarjan_sort.py` & `r2diaphora-0.3.1/r2diaphora/others/tarjan_sort.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.3.0/r2diaphora.egg-info/PKG-INFO` & `r2diaphora-0.3.1/r2diaphora.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 Metadata-Version: 2.1
 Name: r2diaphora
-Version: 0.3.0
+Version: 0.3.1
 Summary: radare2 port of diaphora
 Home-page: https://github.com/FernandoDoming/r2diaphora
 Author: Fernando Domínguez
 Author-email: fernando.dom.del@gmail.com
 License: GNU GPL v3
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `r2diaphora-0.3.0/r2diaphora.egg-info/SOURCES.txt` & `r2diaphora-0.3.1/r2diaphora.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.3.0/scripts/r2diaphora-bulk` & `r2diaphora-0.3.1/scripts/r2diaphora-bulk`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.3.0/scripts/r2diaphora-db` & `r2diaphora-0.3.1/scripts/r2diaphora-db`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.3.0/setup.py` & `r2diaphora-0.3.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                 copy_tree(
                     dir_path,
                     os.path.join(os.path.expanduser("~"), ".r2diaphora", "signatures", "flirt", d)
                 )
 
 setup(
     name="r2diaphora",
-    version="0.3.0",
+    version="0.3.1",
     description="radare2 port of diaphora",
     url="https://github.com/FernandoDoming/r2diaphora",
     author="Fernando Domínguez",
     author_email="fernando.dom.del@gmail.com",
     license="GNU GPL v3",
     packages=[
         "r2diaphora",
@@ -51,14 +51,15 @@
     ],
     install_requires=[
         "chardet>=4.0.0",
         "r2pipe>=1.6.3",
         "colorama>=0.4.4",
         "yattag>=1.14.0",
         "mysql-connector-python>=8.0.26",
+        "python-magic>=0.4.27",
     ],
 
     classifiers=[
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
```

