# Comparing `tmp/svbench-0.7.3.tar.gz` & `tmp/svbench-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svbench-0.7.3.tar", last modified: Fri Jul 21 08:26:30 2023, max compression
+gzip compressed data, was "svbench-0.7.4.tar", last modified: Mon Jul 24 11:28:40 2023, max compression
```

## Comparing `svbench-0.7.3.tar` & `svbench-0.7.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-07-21 08:26:30.417331 svbench-0.7.3/
--rw-r--r--   0 kezcleal   (501) staff       (20)     1069 2019-06-25 15:21:27.000000 svbench-0.7.3/LICENSE.md
--rw-r--r--   0 kezcleal   (501) staff       (20)       33 2020-04-17 10:48:39.000000 svbench-0.7.3/MANIFEST.in
--rw-r--r--   0 kezcleal   (501) staff       (20)      112 2023-07-21 08:26:30.416991 svbench-0.7.3/PKG-INFO
--rw-r--r--   0 kezcleal   (501) staff       (20)      662 2023-05-26 13:36:56.000000 svbench-0.7.3/README.rst
--rw-r--r--   0 kezcleal   (501) staff       (20)       38 2023-07-21 08:26:30.417415 svbench-0.7.3/setup.cfg
--rw-r--r--   0 kezcleal   (501) staff       (20)      487 2023-07-12 11:56:56.000000 svbench-0.7.3/setup.py
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-07-21 08:26:30.404105 svbench-0.7.3/svbench/
--rw-r--r--   0 kezcleal   (501) staff       (20)     6148 2022-04-06 14:34:09.000000 svbench-0.7.3/svbench/.DS_Store
--rw-r--r--   0 kezcleal   (501) staff       (20)       94 2021-04-30 10:31:14.000000 svbench-0.7.3/svbench/__init__.py
--rw-r--r--   0 kezcleal   (501) staff       (20)     1989 2023-07-19 14:28:51.000000 svbench-0.7.3/svbench/cli.py
--rw-r--r--   0 kezcleal   (501) staff       (20)    70673 2023-07-12 16:35:27.000000 svbench-0.7.3/svbench/io_tools.py
--rw-r--r--   0 kezcleal   (501) staff       (20)     2320 2021-04-30 10:40:25.000000 svbench-0.7.3/svbench/loaders.py
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-07-21 08:26:30.416633 svbench-0.7.3/svbench/models/
--rw-r--r--   0 kezcleal   (501) staff       (20)        0 2020-04-17 10:48:39.000000 svbench-0.7.3/svbench/models/__init__.py
--rw-r--r--   0 kezcleal   (501) staff       (20)     8106 2021-12-02 16:05:54.000000 svbench-0.7.3/svbench/quant_tools.py
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-07-21 08:26:30.416214 svbench-0.7.3/svbench.egg-info/
--rw-r--r--   0 kezcleal   (501) staff       (20)      112 2023-07-21 08:26:30.000000 svbench-0.7.3/svbench.egg-info/PKG-INFO
--rw-r--r--   0 kezcleal   (501) staff       (20)      372 2023-07-21 08:26:30.000000 svbench-0.7.3/svbench.egg-info/SOURCES.txt
--rw-r--r--   0 kezcleal   (501) staff       (20)        1 2023-07-21 08:26:30.000000 svbench-0.7.3/svbench.egg-info/dependency_links.txt
--rw-r--r--   0 kezcleal   (501) staff       (20)       45 2023-07-21 08:26:30.000000 svbench-0.7.3/svbench.egg-info/entry_points.txt
--rw-r--r--   0 kezcleal   (501) staff       (20)       50 2023-07-21 08:26:30.000000 svbench-0.7.3/svbench.egg-info/requires.txt
--rw-r--r--   0 kezcleal   (501) staff       (20)        8 2023-07-21 08:26:30.000000 svbench-0.7.3/svbench.egg-info/top_level.txt
+drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-07-24 11:28:40.025525 svbench-0.7.4/
+-rw-r--r--   0 kezcleal   (501) staff       (20)     1069 2019-06-25 15:21:27.000000 svbench-0.7.4/LICENSE.md
+-rw-r--r--   0 kezcleal   (501) staff       (20)       33 2020-04-17 10:48:39.000000 svbench-0.7.4/MANIFEST.in
+-rw-r--r--   0 kezcleal   (501) staff       (20)      112 2023-07-24 11:28:40.025191 svbench-0.7.4/PKG-INFO
+-rw-r--r--   0 kezcleal   (501) staff       (20)      662 2023-05-26 13:36:56.000000 svbench-0.7.4/README.rst
+-rw-r--r--   0 kezcleal   (501) staff       (20)       38 2023-07-24 11:28:40.025607 svbench-0.7.4/setup.cfg
+-rw-r--r--   0 kezcleal   (501) staff       (20)      487 2023-07-24 10:24:49.000000 svbench-0.7.4/setup.py
+drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-07-24 11:28:39.996730 svbench-0.7.4/svbench/
+-rw-r--r--   0 kezcleal   (501) staff       (20)     6148 2022-04-06 14:34:09.000000 svbench-0.7.4/svbench/.DS_Store
+-rw-r--r--   0 kezcleal   (501) staff       (20)       94 2021-04-30 10:31:14.000000 svbench-0.7.4/svbench/__init__.py
+-rw-r--r--   0 kezcleal   (501) staff       (20)     1989 2023-07-19 14:28:51.000000 svbench-0.7.4/svbench/cli.py
+-rw-r--r--   0 kezcleal   (501) staff       (20)    70873 2023-07-24 10:24:34.000000 svbench-0.7.4/svbench/io_tools.py
+-rw-r--r--   0 kezcleal   (501) staff       (20)     2320 2021-04-30 10:40:25.000000 svbench-0.7.4/svbench/loaders.py
+drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-07-24 11:28:40.024855 svbench-0.7.4/svbench/models/
+-rw-r--r--   0 kezcleal   (501) staff       (20)        0 2020-04-17 10:48:39.000000 svbench-0.7.4/svbench/models/__init__.py
+-rw-r--r--   0 kezcleal   (501) staff       (20)     8106 2021-12-02 16:05:54.000000 svbench-0.7.4/svbench/quant_tools.py
+drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-07-24 11:28:40.024400 svbench-0.7.4/svbench.egg-info/
+-rw-r--r--   0 kezcleal   (501) staff       (20)      112 2023-07-24 11:28:39.000000 svbench-0.7.4/svbench.egg-info/PKG-INFO
+-rw-r--r--   0 kezcleal   (501) staff       (20)      372 2023-07-24 11:28:39.000000 svbench-0.7.4/svbench.egg-info/SOURCES.txt
+-rw-r--r--   0 kezcleal   (501) staff       (20)        1 2023-07-24 11:28:39.000000 svbench-0.7.4/svbench.egg-info/dependency_links.txt
+-rw-r--r--   0 kezcleal   (501) staff       (20)       45 2023-07-24 11:28:39.000000 svbench-0.7.4/svbench.egg-info/entry_points.txt
+-rw-r--r--   0 kezcleal   (501) staff       (20)       50 2023-07-24 11:28:39.000000 svbench-0.7.4/svbench.egg-info/requires.txt
+-rw-r--r--   0 kezcleal   (501) staff       (20)        8 2023-07-24 11:28:39.000000 svbench-0.7.4/svbench.egg-info/top_level.txt
```

### Comparing `svbench-0.7.3/LICENSE.md` & `svbench-0.7.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `svbench-0.7.3/README.rst` & `svbench-0.7.4/README.rst`

 * *Files identical despite different names*

### Comparing `svbench-0.7.3/svbench/.DS_Store` & `svbench-0.7.4/svbench/.DS_Store`

 * *Files identical despite different names*

### Comparing `svbench-0.7.3/svbench/cli.py` & `svbench-0.7.4/svbench/cli.py`

 * *Files identical despite different names*

### Comparing `svbench-0.7.3/svbench/io_tools.py` & `svbench-0.7.4/svbench/io_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -812,14 +812,15 @@
 
         if allowed_chroms:
             if not isinstance(allowed_chroms, set):
                 allowed_chroms = set(allowed_chroms)
 
         new_cols = []
         unique_ids = set([])
+        ignore_mates = set([])
 
         if path in "-stdin":
             temp = StringIO()
             for line in stdin:
                 temp.write(line)
             temp.seek(0)
             self.temp = temp  # Used when writing output
@@ -858,14 +859,19 @@
 
             if allowed_chroms is not None and chrom not in allowed_chroms:
                 continue
 
             if "#" in chrom:
                 continue
 
+            if "MATEID" in r.INFO:
+                if r.INFO["MATEID"] in ignore_mates:
+                    continue
+                ignore_mates.add(r.INFO["MATEID"])
+
             start = int(r.POS)
 
             if ol_tree and chrom in ol_tree:
                 if any(ol_tree[chrom].ncls.find_overlap(start, start + 1)):
                     ol_start = True
                 if not ol_start and include_if == "both":
                     not_in_include += 1
```

### Comparing `svbench-0.7.3/svbench/loaders.py` & `svbench-0.7.4/svbench/loaders.py`

 * *Files identical despite different names*

### Comparing `svbench-0.7.3/svbench/quant_tools.py` & `svbench-0.7.4/svbench/quant_tools.py`

 * *Files identical despite different names*

