# Comparing `tmp/medusa-zip-0.0.0.tar.gz` & `tmp/medusa-zip-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medusa-zip-0.0.0.tar", last modified: Sun Jul 23 21:52:42 2023, max compression
+gzip compressed data, was "medusa-zip-0.0.1.tar", last modified: Sun Jul 23 22:32:49 2023, max compression
```

## Comparing `medusa-zip-0.0.0.tar` & `medusa-zip-0.0.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 cosmicexplorer  (1000) cosmicexplorer  (1000)        0 2023-07-23 21:52:42.802640 medusa-zip-0.0.0/
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)     1430 2023-07-23 20:30:52.000000 medusa-zip-0.0.0/Cargo.toml
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)    11360 2023-06-28 11:07:30.000000 medusa-zip-0.0.0/LICENSE
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)      161 2023-07-23 20:59:06.000000 medusa-zip-0.0.0/MANIFEST.in
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)     1451 2023-07-23 21:52:42.802640 medusa-zip-0.0.0/PKG-INFO
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)     1747 2023-07-20 03:41:28.000000 medusa-zip-0.0.0/README.md
-drwxrwxr-x   0 cosmicexplorer  (1000) cosmicexplorer  (1000)        0 2023-07-23 21:52:42.798640 medusa-zip-0.0.0/cli/
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)     1153 2023-07-23 10:48:46.000000 medusa-zip-0.0.0/cli/Cargo.toml
-drwxrwxr-x   0 cosmicexplorer  (1000) cosmicexplorer  (1000)        0 2023-07-23 21:52:42.798640 medusa-zip-0.0.0/cli/src/
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)     3929 2023-07-23 04:14:47.000000 medusa-zip-0.0.0/cli/src/crawl.rs
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)     1834 2023-07-23 02:51:27.000000 medusa-zip-0.0.0/cli/src/destination.rs
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)    11227 2023-07-23 10:44:34.000000 medusa-zip-0.0.0/cli/src/main.rs
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)     2230 2023-07-23 03:30:34.000000 medusa-zip-0.0.0/cli/src/merge.rs
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)     1236 2023-07-23 02:31:13.000000 medusa-zip-0.0.0/cli/src/util.rs
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)     9444 2023-07-23 20:24:48.000000 medusa-zip-0.0.0/cli/src/zip.rs
-drwxrwxr-x   0 cosmicexplorer  (1000) cosmicexplorer  (1000)        0 2023-07-23 21:52:42.798640 medusa-zip-0.0.0/lib/
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)     1196 2023-07-23 20:22:54.000000 medusa-zip-0.0.0/lib/Cargo.toml
-drwxrwxr-x   0 cosmicexplorer  (1000) cosmicexplorer  (1000)        0 2023-07-23 21:52:42.802640 medusa-zip-0.0.0/lib/src/
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)     8286 2023-07-23 03:34:09.000000 medusa-zip-0.0.0/lib/src/crawl.rs
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)     3879 2023-07-23 02:48:34.000000 medusa-zip-0.0.0/lib/src/destination.rs
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)     5806 2023-07-23 18:55:23.000000 medusa-zip-0.0.0/lib/src/lib.rs
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)     4269 2023-07-23 10:43:28.000000 medusa-zip-0.0.0/lib/src/merge.rs
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)    27895 2023-07-23 20:23:25.000000 medusa-zip-0.0.0/lib/src/zip.rs
-drwxrwxr-x   0 cosmicexplorer  (1000) cosmicexplorer  (1000)        0 2023-07-23 21:52:42.802640 medusa-zip-0.0.0/py/
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)     1320 2023-07-23 18:01:55.000000 medusa-zip-0.0.0/py/Cargo.toml
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)       23 2023-07-20 09:41:22.000000 medusa-zip-0.0.0/py/README.md
-drwxrwxr-x   0 cosmicexplorer  (1000) cosmicexplorer  (1000)        0 2023-07-23 21:52:42.802640 medusa-zip-0.0.0/py/medusa_zip/
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)      226 2023-07-20 12:06:59.000000 medusa-zip-0.0.0/py/medusa_zip/__init__.py
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)      452 2023-07-20 16:40:17.000000 medusa-zip-0.0.0/py/medusa_zip/__init__.pyi
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)      232 2023-07-20 11:52:11.000000 medusa-zip-0.0.0/py/medusa_zip/crawl.py
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)     1410 2023-07-23 10:03:58.000000 medusa-zip-0.0.0/py/medusa_zip/crawl.pyi
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)      238 2023-07-20 18:12:07.000000 medusa-zip-0.0.0/py/medusa_zip/destination.py
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)     1077 2023-07-23 10:06:33.000000 medusa-zip-0.0.0/py/medusa_zip/destination.pyi
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)      232 2023-07-20 15:25:00.000000 medusa-zip-0.0.0/py/medusa_zip/merge.py
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)     1004 2023-07-23 10:21:37.000000 medusa-zip-0.0.0/py/medusa_zip/merge.pyi
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)        0 2023-07-20 10:23:00.000000 medusa-zip-0.0.0/py/medusa_zip/py.typed
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)      230 2023-07-20 19:04:42.000000 medusa-zip-0.0.0/py/medusa_zip/zip.py
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)     3283 2023-07-23 20:23:42.000000 medusa-zip-0.0.0/py/medusa_zip/zip.pyi
-drwxrwxr-x   0 cosmicexplorer  (1000) cosmicexplorer  (1000)        0 2023-07-23 21:52:42.802640 medusa-zip-0.0.0/py/medusa_zip.egg-info/
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)     1451 2023-07-23 21:52:42.000000 medusa-zip-0.0.0/py/medusa_zip.egg-info/PKG-INFO
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)      901 2023-07-23 21:52:42.000000 medusa-zip-0.0.0/py/medusa_zip.egg-info/SOURCES.txt
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)        1 2023-07-23 21:52:42.000000 medusa-zip-0.0.0/py/medusa_zip.egg-info/dependency_links.txt
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)        1 2023-07-23 20:58:25.000000 medusa-zip-0.0.0/py/medusa_zip.egg-info/not-zip-safe
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)       19 2023-07-23 21:52:42.000000 medusa-zip-0.0.0/py/medusa_zip.egg-info/requires.txt
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)       11 2023-07-23 21:52:42.000000 medusa-zip-0.0.0/py/medusa_zip.egg-info/top_level.txt
-drwxrwxr-x   0 cosmicexplorer  (1000) cosmicexplorer  (1000)        0 2023-07-23 21:52:42.802640 medusa-zip-0.0.0/py/src/
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)     7172 2023-07-23 10:41:51.000000 medusa-zip-0.0.0/py/src/crawl.rs
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)     6189 2023-07-23 10:06:15.000000 medusa-zip-0.0.0/py/src/destination.rs
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)     4805 2023-07-23 10:42:12.000000 medusa-zip-0.0.0/py/src/lib.rs
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)     5466 2023-07-23 10:38:28.000000 medusa-zip-0.0.0/py/src/merge.rs
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)      501 2023-07-23 10:34:28.000000 medusa-zip-0.0.0/py/src/util.rs
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)    18240 2023-07-23 20:24:09.000000 medusa-zip-0.0.0/py/src/zip.rs
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)     2003 2023-07-23 21:51:26.000000 medusa-zip-0.0.0/pyproject.toml
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)       38 2023-07-23 21:52:42.802640 medusa-zip-0.0.0/setup.cfg
--rw-rw-r--   0 cosmicexplorer  (1000) cosmicexplorer  (1000)      830 2023-07-23 01:35:45.000000 medusa-zip-0.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:32:49.726214 medusa-zip-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-23 22:32:49.726214 medusa-zip-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:32:49.718214 medusa-zip-0.0.1/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/cli/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:32:49.718214 medusa-zip-0.0.1/cli/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/cli/src/crawl.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/cli/src/destination.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    11227 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/cli/src/main.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/cli/src/merge.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/cli/src/util.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/cli/src/zip.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:32:49.718214 medusa-zip-0.0.1/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/lib/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:32:49.718214 medusa-zip-0.0.1/lib/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/lib/src/crawl.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/lib/src/destination.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/lib/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/lib/src/merge.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    27895 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/lib/src/zip.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:32:49.722214 medusa-zip-0.0.1/py/
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/py/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/py/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:32:49.722214 medusa-zip-0.0.1/py/medusa_zip/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/py/medusa_zip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/py/medusa_zip/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/py/medusa_zip/crawl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/py/medusa_zip/crawl.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/py/medusa_zip/destination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/py/medusa_zip/destination.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/py/medusa_zip/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/py/medusa_zip/merge.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/py/medusa_zip/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/py/medusa_zip/zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/py/medusa_zip/zip.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:32:49.726214 medusa-zip-0.0.1/py/medusa_zip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-23 22:32:49.000000 medusa-zip-0.0.1/py/medusa_zip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-23 22:32:49.000000 medusa-zip-0.0.1/py/medusa_zip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 22:32:49.000000 medusa-zip-0.0.1/py/medusa_zip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 22:32:49.000000 medusa-zip-0.0.1/py/medusa_zip.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-23 22:32:49.000000 medusa-zip-0.0.1/py/medusa_zip.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-23 22:32:49.000000 medusa-zip-0.0.1/py/medusa_zip.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:32:49.726214 medusa-zip-0.0.1/py/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/py/src/crawl.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/py/src/destination.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/py/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/py/src/merge.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/py/src/util.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    18240 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/py/src/zip.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 22:32:49.726214 medusa-zip-0.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/setup.py
```

### Comparing `medusa-zip-0.0.0/Cargo.toml` & `medusa-zip-0.0.1/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 git                     = "https://github.com/cosmicexplorer/zip"
 rev                     = "8ca0ed7041fc2bb44aca16053c4f6d20631a627e"
 default-features        = false
 # TODO: consider aes, bzip2, zstd support?
 features                = ["deflate", "time", "rayon", "merge"]
 
 [workspace.package]
-version                 = "0.0.0"
+version                 = "0.0.1"
 authors                 = ["Danny McClanahan <dmcC2@hypnicjerk.ai>"]
 edition                 = "2021"
 license                 = "Apache-2.0"
 
 keywords                = ["zip", "file", "archive", "parallel", "i/o"]
 categories              = ["development-tools::build-utils", "filesystem", "asynchronous", "caching"]
 homepage                = "https://github.com/cosmicexplorer/medusa-zip"
```

### Comparing `medusa-zip-0.0.0/LICENSE` & `medusa-zip-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.0/PKG-INFO` & `medusa-zip-0.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medusa-zip
-Version: 0.0.0
+Version: 0.0.1
 Summary: High-performance parallelized implementations of common zip file operations.
 Author-email: Danny McClanahan <dmcC2@hypnicjerk.ai>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/cosmicexplorer/medusa-zip
 Project-URL: Repository, https://github.com/cosmicexplorer/medusa-zip
 Project-URL: Bug Tracker, https://github.com/cosmicexplorer/medusa-zip/issues
 Keywords: zip,rust,fs,file,archive,parallel,pyo3
```

### Comparing `medusa-zip-0.0.0/README.md` & `medusa-zip-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.0/cli/Cargo.toml` & `medusa-zip-0.0.1/cli/Cargo.toml`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.0/cli/src/crawl.rs` & `medusa-zip-0.0.1/cli/src/crawl.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.0/cli/src/destination.rs` & `medusa-zip-0.0.1/cli/src/destination.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.0/cli/src/main.rs` & `medusa-zip-0.0.1/cli/src/main.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.0/cli/src/merge.rs` & `medusa-zip-0.0.1/cli/src/merge.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.0/cli/src/util.rs` & `medusa-zip-0.0.1/cli/src/util.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.0/cli/src/zip.rs` & `medusa-zip-0.0.1/cli/src/zip.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.0/lib/Cargo.toml` & `medusa-zip-0.0.1/lib/Cargo.toml`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.0/lib/src/crawl.rs` & `medusa-zip-0.0.1/lib/src/crawl.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.0/lib/src/destination.rs` & `medusa-zip-0.0.1/lib/src/destination.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.0/lib/src/lib.rs` & `medusa-zip-0.0.1/lib/src/lib.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.0/lib/src/merge.rs` & `medusa-zip-0.0.1/lib/src/merge.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.0/lib/src/zip.rs` & `medusa-zip-0.0.1/lib/src/zip.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.0/py/Cargo.toml` & `medusa-zip-0.0.1/py/Cargo.toml`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.0/py/medusa_zip/crawl.pyi` & `medusa-zip-0.0.1/py/medusa_zip/crawl.pyi`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.0/py/medusa_zip/destination.pyi` & `medusa-zip-0.0.1/py/medusa_zip/destination.pyi`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.0/py/medusa_zip/merge.pyi` & `medusa-zip-0.0.1/py/medusa_zip/merge.pyi`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.0/py/medusa_zip/zip.pyi` & `medusa-zip-0.0.1/py/medusa_zip/zip.pyi`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.0/py/medusa_zip.egg-info/PKG-INFO` & `medusa-zip-0.0.1/py/medusa_zip.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medusa-zip
-Version: 0.0.0
+Version: 0.0.1
 Summary: High-performance parallelized implementations of common zip file operations.
 Author-email: Danny McClanahan <dmcC2@hypnicjerk.ai>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/cosmicexplorer/medusa-zip
 Project-URL: Repository, https://github.com/cosmicexplorer/medusa-zip
 Project-URL: Bug Tracker, https://github.com/cosmicexplorer/medusa-zip/issues
 Keywords: zip,rust,fs,file,archive,parallel,pyo3
```

### Comparing `medusa-zip-0.0.0/py/medusa_zip.egg-info/SOURCES.txt` & `medusa-zip-0.0.1/py/medusa_zip.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.0/py/src/crawl.rs` & `medusa-zip-0.0.1/py/src/crawl.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.0/py/src/destination.rs` & `medusa-zip-0.0.1/py/src/destination.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.0/py/src/lib.rs` & `medusa-zip-0.0.1/py/src/lib.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.0/py/src/merge.rs` & `medusa-zip-0.0.1/py/src/merge.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.0/py/src/zip.rs` & `medusa-zip-0.0.1/py/src/zip.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.0/pyproject.toml` & `medusa-zip-0.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "medusa-zip"
-version = "0.0.0"
+version = "0.0.1"
 description = "High-performance parallelized implementations of common zip file operations."
 license = {text = "Apache-2.0"}
 readme = "py/README.md"
 authors = [
   {name = "Danny McClanahan", email = "dmcC2@hypnicjerk.ai"},
 ]
 keywords = ["zip", "rust", "fs", "file", "archive", "parallel", "pyo3"]
```

### Comparing `medusa-zip-0.0.0/setup.py` & `medusa-zip-0.0.1/setup.py`

 * *Files identical despite different names*

