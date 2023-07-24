# Comparing `tmp/flams-0.0.7.tar.gz` & `tmp/flams-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flams-0.0.7.tar", last modified: Thu Jul 13 09:15:23 2023, max compression
+gzip compressed data, was "flams-0.0.8.tar", last modified: Mon Jul 24 07:20:54 2023, max compression
```

## Comparing `flams-0.0.7.tar` & `flams-0.0.8.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 u0138113 (1031392) domain users (200513)        0 2023-07-13 09:15:23.523689 flams-0.0.7/
--rw-r--r--   0 u0138113 (1031392) domain users (200513)     1286 2023-07-13 09:08:42.000000 flams-0.0.7/LICENSE
--rw-r--r--   0 u0138113 (1031392) domain users (200513)     7298 2023-07-13 09:15:23.523689 flams-0.0.7/PKG-INFO
--rw-r--r--   0 u0138113 (1031392) domain users (200513)     7038 2023-07-13 09:08:42.000000 flams-0.0.7/README.md
-drwxr-xr-x   0 u0138113 (1031392) domain users (200513)        0 2023-07-13 09:15:23.523689 flams-0.0.7/flams/
--rw-r--r--   0 u0138113 (1031392) domain users (200513)        0 2023-05-09 12:23:21.000000 flams-0.0.7/flams/__init__.py
-drwxr-xr-x   0 u0138113 (1031392) domain users (200513)        0 2023-07-13 09:15:23.523689 flams-0.0.7/flams/databases/
--rw-r--r--   0 u0138113 (1031392) domain users (200513)        0 2023-05-09 12:23:21.000000 flams-0.0.7/flams/databases/__init__.py
--rw-r--r--   0 u0138113 (1031392) domain users (200513)     2827 2023-07-13 09:08:42.000000 flams-0.0.7/flams/databases/cplmv4.py
--rw-r--r--   0 u0138113 (1031392) domain users (200513)     8930 2023-07-13 09:08:42.000000 flams-0.0.7/flams/databases/setup.py
--rw-r--r--   0 u0138113 (1031392) domain users (200513)     3485 2023-07-13 09:08:42.000000 flams-0.0.7/flams/display.py
--rw-r--r--   0 u0138113 (1031392) domain users (200513)     2429 2023-07-13 09:08:42.000000 flams-0.0.7/flams/flams.py
--rw-r--r--   0 u0138113 (1031392) domain users (200513)    13397 2023-07-13 09:08:42.000000 flams-0.0.7/flams/input.py
--rw-r--r--   0 u0138113 (1031392) domain users (200513)    12443 2023-07-13 09:08:42.000000 flams-0.0.7/flams/run_blast.py
--rw-r--r--   0 u0138113 (1031392) domain users (200513)      992 2023-07-13 09:08:42.000000 flams-0.0.7/flams/utils.py
-drwxr-xr-x   0 u0138113 (1031392) domain users (200513)        0 2023-07-13 09:15:23.523689 flams-0.0.7/flams.egg-info/
--rw-r--r--   0 u0138113 (1031392) domain users (200513)     7298 2023-07-13 09:15:23.000000 flams-0.0.7/flams.egg-info/PKG-INFO
--rw-r--r--   0 u0138113 (1031392) domain users (200513)      403 2023-07-13 09:15:23.000000 flams-0.0.7/flams.egg-info/SOURCES.txt
--rw-r--r--   0 u0138113 (1031392) domain users (200513)        1 2023-07-13 09:15:23.000000 flams-0.0.7/flams.egg-info/dependency_links.txt
--rw-r--r--   0 u0138113 (1031392) domain users (200513)       43 2023-07-13 09:15:23.000000 flams-0.0.7/flams.egg-info/entry_points.txt
--rw-r--r--   0 u0138113 (1031392) domain users (200513)      131 2023-07-13 09:15:23.000000 flams-0.0.7/flams.egg-info/requires.txt
--rw-r--r--   0 u0138113 (1031392) domain users (200513)        6 2023-07-13 09:15:23.000000 flams-0.0.7/flams.egg-info/top_level.txt
--rw-r--r--   0 u0138113 (1031392) domain users (200513)      496 2023-07-13 09:15:15.000000 flams-0.0.7/pyproject.toml
--rw-r--r--   0 u0138113 (1031392) domain users (200513)      426 2023-07-13 09:08:36.000000 flams-0.0.7/requirements.txt
--rw-r--r--   0 u0138113 (1031392) domain users (200513)       38 2023-07-13 09:15:23.523689 flams-0.0.7/setup.cfg
+drwxr-xr-x   0 u0138113 (1031392) domain users (200513)        0 2023-07-24 07:20:54.553641 flams-0.0.8/
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)     1286 2023-07-13 09:08:42.000000 flams-0.0.8/LICENSE
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)     7298 2023-07-24 07:20:54.553641 flams-0.0.8/PKG-INFO
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)     7038 2023-07-13 09:08:42.000000 flams-0.0.8/README.md
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)      454 2023-07-24 07:20:08.000000 flams-0.0.8/pyproject.toml
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)      426 2023-07-13 09:08:36.000000 flams-0.0.8/requirements.txt
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)       38 2023-07-24 07:20:54.553641 flams-0.0.8/setup.cfg
+drwxr-xr-x   0 u0138113 (1031392) domain users (200513)        0 2023-07-24 07:20:54.553641 flams-0.0.8/src/
+drwxr-xr-x   0 u0138113 (1031392) domain users (200513)        0 2023-07-24 07:20:54.553641 flams-0.0.8/src/flams/
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)        0 2023-05-09 12:23:21.000000 flams-0.0.8/src/flams/__init__.py
+drwxr-xr-x   0 u0138113 (1031392) domain users (200513)        0 2023-07-24 07:20:54.553641 flams-0.0.8/src/flams/databases/
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)        0 2023-05-09 12:23:21.000000 flams-0.0.8/src/flams/databases/__init__.py
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)     2827 2023-07-13 09:08:42.000000 flams-0.0.8/src/flams/databases/cplmv4.py
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)     8930 2023-07-13 09:08:42.000000 flams-0.0.8/src/flams/databases/setup.py
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)     3485 2023-07-13 09:08:42.000000 flams-0.0.8/src/flams/display.py
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)     2429 2023-07-13 09:08:42.000000 flams-0.0.8/src/flams/flams.py
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)    13397 2023-07-13 09:08:42.000000 flams-0.0.8/src/flams/input.py
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)    12443 2023-07-13 09:08:42.000000 flams-0.0.8/src/flams/run_blast.py
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)      992 2023-07-13 09:08:42.000000 flams-0.0.8/src/flams/utils.py
+drwxr-xr-x   0 u0138113 (1031392) domain users (200513)        0 2023-07-24 07:20:54.553641 flams-0.0.8/src/flams.egg-info/
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)     7298 2023-07-24 07:20:54.000000 flams-0.0.8/src/flams.egg-info/PKG-INFO
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)      463 2023-07-24 07:20:54.000000 flams-0.0.8/src/flams.egg-info/SOURCES.txt
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)        1 2023-07-24 07:20:54.000000 flams-0.0.8/src/flams.egg-info/dependency_links.txt
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)       43 2023-07-24 07:20:54.000000 flams-0.0.8/src/flams.egg-info/entry_points.txt
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)      131 2023-07-24 07:20:54.000000 flams-0.0.8/src/flams.egg-info/requires.txt
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)        6 2023-07-24 07:20:54.000000 flams-0.0.8/src/flams.egg-info/top_level.txt
```

### Comparing `flams-0.0.7/LICENSE` & `flams-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `flams-0.0.7/PKG-INFO` & `flams-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flams
-Version: 0.0.7
+Version: 0.0.8
 Summary: Find Lysine Acylation & other Modification Sites
 Project-URL: repository, https://github.com/hannelorelongin/FLAMS
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FLAMS: Find Lysine Acylations & other Modification Sites
```

### Comparing `flams-0.0.7/README.md` & `flams-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `flams-0.0.7/flams/databases/cplmv4.py` & `flams-0.0.8/src/flams/databases/cplmv4.py`

 * *Files identical despite different names*

### Comparing `flams-0.0.7/flams/databases/setup.py` & `flams-0.0.8/src/flams/databases/setup.py`

 * *Files identical despite different names*

### Comparing `flams-0.0.7/flams/display.py` & `flams-0.0.8/src/flams/display.py`

 * *Files identical despite different names*

### Comparing `flams-0.0.7/flams/flams.py` & `flams-0.0.8/src/flams/flams.py`

 * *Files identical despite different names*

### Comparing `flams-0.0.7/flams/input.py` & `flams-0.0.8/src/flams/input.py`

 * *Files identical despite different names*

### Comparing `flams-0.0.7/flams/run_blast.py` & `flams-0.0.8/src/flams/run_blast.py`

 * *Files identical despite different names*

### Comparing `flams-0.0.7/flams/utils.py` & `flams-0.0.8/src/flams/utils.py`

 * *Files identical despite different names*

### Comparing `flams-0.0.7/flams.egg-info/PKG-INFO` & `flams-0.0.8/src/flams.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flams
-Version: 0.0.7
+Version: 0.0.8
 Summary: Find Lysine Acylation & other Modification Sites
 Project-URL: repository, https://github.com/hannelorelongin/FLAMS
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FLAMS: Find Lysine Acylations & other Modification Sites
```

