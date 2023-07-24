# Comparing `tmp/pysymbolcheck-2.8.0.tar.gz` & `tmp/pysymbolcheck-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysymbolcheck-2.8.0.tar", last modified: Thu Jun 29 12:13:42 2023, max compression
+gzip compressed data, was "pysymbolcheck-2.8.1.tar", last modified: Mon Jul 24 03:11:51 2023, max compression
```

## Comparing `pysymbolcheck-2.8.0.tar` & `pysymbolcheck-2.8.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:13:42.936204 pysymbolcheck-2.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-29 12:13:19.000000 pysymbolcheck-2.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-29 12:13:19.000000 pysymbolcheck-2.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-06-29 12:13:42.936204 pysymbolcheck-2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-29 12:13:19.000000 pysymbolcheck-2.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-06-29 12:13:19.000000 pysymbolcheck-2.8.0/basic_rules.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:13:42.932204 pysymbolcheck-2.8.0/pysymbolcheck/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:13:19.000000 pysymbolcheck-2.8.0/pysymbolcheck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6507 2023-06-29 12:13:19.000000 pysymbolcheck-2.8.0/pysymbolcheck/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:13:42.936204 pysymbolcheck-2.8.0/pysymbolcheck.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-06-29 12:13:42.000000 pysymbolcheck-2.8.0/pysymbolcheck.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-29 12:13:42.000000 pysymbolcheck-2.8.0/pysymbolcheck.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 12:13:42.000000 pysymbolcheck-2.8.0/pysymbolcheck.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-29 12:13:42.000000 pysymbolcheck-2.8.0/pysymbolcheck.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-29 12:13:42.000000 pysymbolcheck-2.8.0/pysymbolcheck.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 12:13:42.000000 pysymbolcheck-2.8.0/pysymbolcheck.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-29 12:13:19.000000 pysymbolcheck-2.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-29 12:13:42.936204 pysymbolcheck-2.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-29 12:13:42.000000 pysymbolcheck-2.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:11:51.357173 pysymbolcheck-2.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-24 03:11:31.000000 pysymbolcheck-2.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-24 03:11:31.000000 pysymbolcheck-2.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-07-24 03:11:51.357173 pysymbolcheck-2.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-24 03:11:31.000000 pysymbolcheck-2.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-07-24 03:11:31.000000 pysymbolcheck-2.8.1/basic_rules.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:11:51.357173 pysymbolcheck-2.8.1/pysymbolcheck/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 03:11:31.000000 pysymbolcheck-2.8.1/pysymbolcheck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6507 2023-07-24 03:11:31.000000 pysymbolcheck-2.8.1/pysymbolcheck/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:11:51.357173 pysymbolcheck-2.8.1/pysymbolcheck.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-07-24 03:11:51.000000 pysymbolcheck-2.8.1/pysymbolcheck.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-24 03:11:51.000000 pysymbolcheck-2.8.1/pysymbolcheck.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 03:11:51.000000 pysymbolcheck-2.8.1/pysymbolcheck.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-24 03:11:51.000000 pysymbolcheck-2.8.1/pysymbolcheck.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-24 03:11:51.000000 pysymbolcheck-2.8.1/pysymbolcheck.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-24 03:11:51.000000 pysymbolcheck-2.8.1/pysymbolcheck.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-24 03:11:31.000000 pysymbolcheck-2.8.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-24 03:11:51.361173 pysymbolcheck-2.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-24 03:11:51.000000 pysymbolcheck-2.8.1/setup.py
```

### Comparing `pysymbolcheck-2.8.0/LICENSE` & `pysymbolcheck-2.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pysymbolcheck-2.8.0/PKG-INFO` & `pysymbolcheck-2.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysymbolcheck
-Version: 2.8.0
+Version: 2.8.1
 Summary: ELF symbol check
 Home-page: https://github.com/priv-kweihmann/pysymcheck
 Author: Konrad Weihmann
 Author-email: kweihmann@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pysymbolcheck-2.8.0/README.md` & `pysymbolcheck-2.8.1/README.md`

 * *Files identical despite different names*

### Comparing `pysymbolcheck-2.8.0/basic_rules.json` & `pysymbolcheck-2.8.1/basic_rules.json`

 * *Files identical despite different names*

### Comparing `pysymbolcheck-2.8.0/pysymbolcheck/__main__.py` & `pysymbolcheck-2.8.1/pysymbolcheck/__main__.py`

 * *Files identical despite different names*

### Comparing `pysymbolcheck-2.8.0/pysymbolcheck.egg-info/PKG-INFO` & `pysymbolcheck-2.8.1/pysymbolcheck.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysymbolcheck
-Version: 2.8.0
+Version: 2.8.1
 Summary: ELF symbol check
 Home-page: https://github.com/priv-kweihmann/pysymcheck
 Author: Konrad Weihmann
 Author-email: kweihmann@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pysymbolcheck-2.8.0/setup.py` & `pysymbolcheck-2.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 requirements = []
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="pysymbolcheck",
-    version="2.8.0",
+    version="2.8.1",
     author="Konrad Weihmann",
     author_email="kweihmann@outlook.com",
     description="ELF symbol check",
     long_description=_long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/priv-kweihmann/pysymcheck",
     packages=setuptools.find_packages(),
```

