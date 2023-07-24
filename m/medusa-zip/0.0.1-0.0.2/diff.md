# Comparing `tmp/medusa-zip-0.0.1.tar.gz` & `tmp/medusa-zip-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medusa-zip-0.0.1.tar", last modified: Sun Jul 23 22:32:49 2023, max compression
+gzip compressed data, was "medusa-zip-0.0.2.tar", last modified: Mon Jul 24 00:35:40 2023, max compression
```

## Comparing `medusa-zip-0.0.1.tar` & `medusa-zip-0.0.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:32:49.726214 medusa-zip-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-23 22:32:49.726214 medusa-zip-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:32:49.718214 medusa-zip-0.0.1/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/cli/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:32:49.718214 medusa-zip-0.0.1/cli/src/
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/cli/src/crawl.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/cli/src/destination.rs
--rw-r--r--   0 runner    (1001) docker     (123)    11227 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/cli/src/main.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/cli/src/merge.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/cli/src/util.rs
--rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/cli/src/zip.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:32:49.718214 medusa-zip-0.0.1/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/lib/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:32:49.718214 medusa-zip-0.0.1/lib/src/
--rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/lib/src/crawl.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/lib/src/destination.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/lib/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/lib/src/merge.rs
--rw-r--r--   0 runner    (1001) docker     (123)    27895 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/lib/src/zip.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:32:49.722214 medusa-zip-0.0.1/py/
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/py/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/py/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:32:49.722214 medusa-zip-0.0.1/py/medusa_zip/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/py/medusa_zip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/py/medusa_zip/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/py/medusa_zip/crawl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/py/medusa_zip/crawl.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/py/medusa_zip/destination.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/py/medusa_zip/destination.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/py/medusa_zip/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/py/medusa_zip/merge.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/py/medusa_zip/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/py/medusa_zip/zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/py/medusa_zip/zip.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:32:49.726214 medusa-zip-0.0.1/py/medusa_zip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-23 22:32:49.000000 medusa-zip-0.0.1/py/medusa_zip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-23 22:32:49.000000 medusa-zip-0.0.1/py/medusa_zip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 22:32:49.000000 medusa-zip-0.0.1/py/medusa_zip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 22:32:49.000000 medusa-zip-0.0.1/py/medusa_zip.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-23 22:32:49.000000 medusa-zip-0.0.1/py/medusa_zip.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-23 22:32:49.000000 medusa-zip-0.0.1/py/medusa_zip.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:32:49.726214 medusa-zip-0.0.1/py/src/
--rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/py/src/crawl.rs
--rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/py/src/destination.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/py/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/py/src/merge.rs
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/py/src/util.rs
--rw-r--r--   0 runner    (1001) docker     (123)    18240 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/py/src/zip.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 22:32:49.726214 medusa-zip-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-23 22:32:41.000000 medusa-zip-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:35:40.288502 medusa-zip-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-24 00:35:40.288502 medusa-zip-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:35:40.284501 medusa-zip-0.0.2/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/cli/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:35:40.284501 medusa-zip-0.0.2/cli/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/cli/src/crawl.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/cli/src/destination.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    11227 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/cli/src/main.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/cli/src/merge.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/cli/src/util.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/cli/src/zip.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:35:40.284501 medusa-zip-0.0.2/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/lib/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:35:40.284501 medusa-zip-0.0.2/lib/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/lib/src/crawl.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/lib/src/destination.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/lib/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/lib/src/merge.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    27895 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/lib/src/zip.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:35:40.284501 medusa-zip-0.0.2/py/
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/py/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/py/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:35:40.288502 medusa-zip-0.0.2/py/medusa_zip/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/py/medusa_zip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/py/medusa_zip/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/py/medusa_zip/crawl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/py/medusa_zip/crawl.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/py/medusa_zip/destination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/py/medusa_zip/destination.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/py/medusa_zip/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/py/medusa_zip/merge.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/py/medusa_zip/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/py/medusa_zip/zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/py/medusa_zip/zip.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:35:40.288502 medusa-zip-0.0.2/py/medusa_zip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-24 00:35:40.000000 medusa-zip-0.0.2/py/medusa_zip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-24 00:35:40.000000 medusa-zip-0.0.2/py/medusa_zip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 00:35:40.000000 medusa-zip-0.0.2/py/medusa_zip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 00:35:39.000000 medusa-zip-0.0.2/py/medusa_zip.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-24 00:35:40.000000 medusa-zip-0.0.2/py/medusa_zip.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-24 00:35:40.000000 medusa-zip-0.0.2/py/medusa_zip.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:35:40.288502 medusa-zip-0.0.2/py/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/py/src/crawl.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/py/src/destination.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/py/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/py/src/merge.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/py/src/util.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    18240 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/py/src/zip.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 00:35:40.288502 medusa-zip-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/setup.py
```

### Comparing `medusa-zip-0.0.1/Cargo.toml` & `medusa-zip-0.0.2/Cargo.toml`

 * *Files 18% similar despite different names*

```diff
@@ -15,29 +15,28 @@
 displaydoc              = "0.2.4"
 regex                   = "1"
 thiserror               = "1.0.30"
 time                    = { version = "0.3.23", features = ["local-offset", "parsing"] }
 tokio                   = "1.29"
 
 [workspace.dependencies.zip]
-# path = "/home/cosmicexplorer/tools/zip"
+version                 = "0.6.6"
 git                     = "https://github.com/cosmicexplorer/zip"
-rev                     = "8ca0ed7041fc2bb44aca16053c4f6d20631a627e"
+rev                     = "79f818a8929b37eee6e7bf0e9284daa157a91aa7"
+package                 = "zip-merge"
 default-features        = false
-# TODO: consider aes, bzip2, zstd support?
 features                = ["deflate", "time", "rayon", "merge"]
 
 [workspace.package]
-version                 = "0.0.1"
+version                 = "0.0.2"
 authors                 = ["Danny McClanahan <dmcC2@hypnicjerk.ai>"]
 edition                 = "2021"
 license                 = "Apache-2.0"
 
-keywords                = ["zip", "file", "archive", "parallel", "i/o"]
+keywords                = ["zip", "file", "archive", "parallel", "io"]
 categories              = ["development-tools::build-utils", "filesystem", "asynchronous", "caching"]
 homepage                = "https://github.com/cosmicexplorer/medusa-zip"
 repository              = "https://github.com/cosmicexplorer/medusa-zip"
 
-# FIXME: uncomment this when the build starts working!
-# [profile.release]
-# strip                   = true
-# lto                     = true
+[profile.release]
+strip                   = true
+lto                     = true
```

### Comparing `medusa-zip-0.0.1/LICENSE` & `medusa-zip-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.1/PKG-INFO` & `medusa-zip-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medusa-zip
-Version: 0.0.1
+Version: 0.0.2
 Summary: High-performance parallelized implementations of common zip file operations.
 Author-email: Danny McClanahan <dmcC2@hypnicjerk.ai>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/cosmicexplorer/medusa-zip
 Project-URL: Repository, https://github.com/cosmicexplorer/medusa-zip
 Project-URL: Bug Tracker, https://github.com/cosmicexplorer/medusa-zip/issues
 Keywords: zip,rust,fs,file,archive,parallel,pyo3
@@ -27,11 +27,11 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: asyncio
 Provides-Extra: sync
 License-File: LICENSE
 
-pymedusa
-========
+pymedusa-zip
+============
 
 ???
```

### Comparing `medusa-zip-0.0.1/README.md` & `medusa-zip-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.1/cli/Cargo.toml` & `medusa-zip-0.0.2/cli/Cargo.toml`

 * *Files 15% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 edition.workspace       = true
 license.workspace       = true
 
 keywords.workspace      = true
 categories              = ["development-tools::build-utils", "filesystem", "asynchronous", "caching", "command-line-utilities"]
 homepage.workspace      = true
 repository.workspace    = true
+description             = "A command-line interface to high-performance parallelized implementations of common zip file operations."
 
 [dependencies]
 clap                    = { version = "4", features = ["derive"] }
 displaydoc.workspace    = true
 eyre                    = "0.6.8"
-libmedusa-zip           = { path = "../lib" }
+libmedusa-zip           = { path = "../lib", version = "0.0.2" }
 regex                   = "1"
 serde                   = { version = "1", features = ["derive"] }
 serde_json              = "1.0"
 thiserror.workspace     = true
 time.workspace          = true
 tokio                   = { workspace = true, features = ["io-util", "io-std", "macros", "rt-multi-thread"] }
 zip.workspace           = true
```

### Comparing `medusa-zip-0.0.1/cli/src/crawl.rs` & `medusa-zip-0.0.2/cli/src/crawl.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.1/cli/src/destination.rs` & `medusa-zip-0.0.2/cli/src/destination.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.1/cli/src/main.rs` & `medusa-zip-0.0.2/cli/src/main.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.1/cli/src/merge.rs` & `medusa-zip-0.0.2/cli/src/merge.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.1/cli/src/util.rs` & `medusa-zip-0.0.2/cli/src/util.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.1/cli/src/zip.rs` & `medusa-zip-0.0.2/cli/src/zip.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.1/lib/Cargo.toml` & `medusa-zip-0.0.2/lib/Cargo.toml`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 edition.workspace       = true
 license.workspace       = true
 
 keywords.workspace      = true
 categories.workspace    = true
 homepage.workspace      = true
 repository.workspace    = true
+description             = "High-performance parallelized implementations of common zip file operations."
 
 [dependencies]
 async-recursion         = "1"
 cfg-if                  = "1.0"
 displaydoc.workspace    = true
 futures                 = "0.3"
 once_cell               = "1"
```

### Comparing `medusa-zip-0.0.1/lib/src/crawl.rs` & `medusa-zip-0.0.2/lib/src/crawl.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.1/lib/src/destination.rs` & `medusa-zip-0.0.2/lib/src/destination.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.1/lib/src/lib.rs` & `medusa-zip-0.0.2/lib/src/lib.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.1/lib/src/merge.rs` & `medusa-zip-0.0.2/lib/src/merge.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.1/lib/src/zip.rs` & `medusa-zip-0.0.2/lib/src/zip.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.1/py/Cargo.toml` & `medusa-zip-0.0.2/py/Cargo.toml`

 * *Files 9% similar despite different names*

```diff
@@ -5,21 +5,22 @@
 edition.workspace       = true
 license.workspace       = true
 
 keywords.workspace      = true
 categories              = ["development-tools::build-utils", "filesystem", "asynchronous", "caching", "api-bindings"]
 homepage.workspace      = true
 repository.workspace    = true
+description             = "A PyOxidizer interface to high-performance parallelized implementations of common zip file operations."
 
 [lib]
 name                    = "pymedusa_zip"
 crate-type              = ["cdylib"]
 
 [dependencies]
-libmedusa-zip           = { path = "../lib" }
+libmedusa-zip           = { path = "../lib", version = "0.0.2" }
 once_cell               = { version = "1", optional = true }
 pyo3                    = { version = "0.19", features = ["extension-module"] }
 pyo3-asyncio            = { version = "0.19", features = ["tokio-runtime"], optional = true }
 regex.workspace         = true
 time.workspace          = true
 tokio                   = { workspace = true, features = ["rt", "rt-multi-thread"] }
 zip.workspace           = true
```

### Comparing `medusa-zip-0.0.1/py/medusa_zip/crawl.pyi` & `medusa-zip-0.0.2/py/medusa_zip/crawl.pyi`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.1/py/medusa_zip/destination.pyi` & `medusa-zip-0.0.2/py/medusa_zip/destination.pyi`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.1/py/medusa_zip/merge.pyi` & `medusa-zip-0.0.2/py/medusa_zip/merge.pyi`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.1/py/medusa_zip/zip.pyi` & `medusa-zip-0.0.2/py/medusa_zip/zip.pyi`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.1/py/medusa_zip.egg-info/PKG-INFO` & `medusa-zip-0.0.2/py/medusa_zip.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medusa-zip
-Version: 0.0.1
+Version: 0.0.2
 Summary: High-performance parallelized implementations of common zip file operations.
 Author-email: Danny McClanahan <dmcC2@hypnicjerk.ai>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/cosmicexplorer/medusa-zip
 Project-URL: Repository, https://github.com/cosmicexplorer/medusa-zip
 Project-URL: Bug Tracker, https://github.com/cosmicexplorer/medusa-zip/issues
 Keywords: zip,rust,fs,file,archive,parallel,pyo3
@@ -27,11 +27,11 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: asyncio
 Provides-Extra: sync
 License-File: LICENSE
 
-pymedusa
-========
+pymedusa-zip
+============
 
 ???
```

### Comparing `medusa-zip-0.0.1/py/medusa_zip.egg-info/SOURCES.txt` & `medusa-zip-0.0.2/py/medusa_zip.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.1/py/src/crawl.rs` & `medusa-zip-0.0.2/py/src/crawl.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.1/py/src/destination.rs` & `medusa-zip-0.0.2/py/src/destination.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.1/py/src/lib.rs` & `medusa-zip-0.0.2/py/src/lib.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.1/py/src/merge.rs` & `medusa-zip-0.0.2/py/src/merge.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.1/py/src/zip.rs` & `medusa-zip-0.0.2/py/src/zip.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.1/pyproject.toml` & `medusa-zip-0.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "medusa-zip"
-version = "0.0.1"
+version = "0.0.2"
 description = "High-performance parallelized implementations of common zip file operations."
 license = {text = "Apache-2.0"}
 readme = "py/README.md"
 authors = [
   {name = "Danny McClanahan", email = "dmcC2@hypnicjerk.ai"},
 ]
 keywords = ["zip", "rust", "fs", "file", "archive", "parallel", "pyo3"]
```

### Comparing `medusa-zip-0.0.1/setup.py` & `medusa-zip-0.0.2/setup.py`

 * *Files identical despite different names*

