# Comparing `tmp/medusa-zip-0.0.2.tar.gz` & `tmp/medusa-zip-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medusa-zip-0.0.2.tar", last modified: Mon Jul 24 00:35:40 2023, max compression
+gzip compressed data, was "medusa-zip-0.0.5.tar", last modified: Mon Jul 24 03:50:39 2023, max compression
```

## Comparing `medusa-zip-0.0.2.tar` & `medusa-zip-0.0.5.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:35:40.288502 medusa-zip-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-24 00:35:40.288502 medusa-zip-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:35:40.284501 medusa-zip-0.0.2/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/cli/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:35:40.284501 medusa-zip-0.0.2/cli/src/
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/cli/src/crawl.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/cli/src/destination.rs
--rw-r--r--   0 runner    (1001) docker     (123)    11227 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/cli/src/main.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/cli/src/merge.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/cli/src/util.rs
--rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/cli/src/zip.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:35:40.284501 medusa-zip-0.0.2/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/lib/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:35:40.284501 medusa-zip-0.0.2/lib/src/
--rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/lib/src/crawl.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/lib/src/destination.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/lib/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/lib/src/merge.rs
--rw-r--r--   0 runner    (1001) docker     (123)    27895 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/lib/src/zip.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:35:40.284501 medusa-zip-0.0.2/py/
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/py/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/py/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:35:40.288502 medusa-zip-0.0.2/py/medusa_zip/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/py/medusa_zip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/py/medusa_zip/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/py/medusa_zip/crawl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/py/medusa_zip/crawl.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/py/medusa_zip/destination.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/py/medusa_zip/destination.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/py/medusa_zip/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/py/medusa_zip/merge.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/py/medusa_zip/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/py/medusa_zip/zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/py/medusa_zip/zip.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:35:40.288502 medusa-zip-0.0.2/py/medusa_zip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-24 00:35:40.000000 medusa-zip-0.0.2/py/medusa_zip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-24 00:35:40.000000 medusa-zip-0.0.2/py/medusa_zip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 00:35:40.000000 medusa-zip-0.0.2/py/medusa_zip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 00:35:39.000000 medusa-zip-0.0.2/py/medusa_zip.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-24 00:35:40.000000 medusa-zip-0.0.2/py/medusa_zip.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-24 00:35:40.000000 medusa-zip-0.0.2/py/medusa_zip.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:35:40.288502 medusa-zip-0.0.2/py/src/
--rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/py/src/crawl.rs
--rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/py/src/destination.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/py/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/py/src/merge.rs
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/py/src/util.rs
--rw-r--r--   0 runner    (1001) docker     (123)    18240 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/py/src/zip.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 00:35:40.288502 medusa-zip-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-24 00:35:30.000000 medusa-zip-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:50:39.694787 medusa-zip-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-24 03:50:30.000000 medusa-zip-0.0.5/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-07-24 03:50:30.000000 medusa-zip-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-24 03:50:30.000000 medusa-zip-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-24 03:50:39.694787 medusa-zip-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-24 03:50:30.000000 medusa-zip-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:50:39.686787 medusa-zip-0.0.5/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-24 03:50:30.000000 medusa-zip-0.0.5/cli/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:50:39.690787 medusa-zip-0.0.5/cli/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-07-24 03:50:30.000000 medusa-zip-0.0.5/cli/src/crawl.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-24 03:50:30.000000 medusa-zip-0.0.5/cli/src/destination.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    11227 2023-07-24 03:50:30.000000 medusa-zip-0.0.5/cli/src/main.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-24 03:50:30.000000 medusa-zip-0.0.5/cli/src/merge.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-24 03:50:30.000000 medusa-zip-0.0.5/cli/src/util.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-07-24 03:50:30.000000 medusa-zip-0.0.5/cli/src/zip.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:50:39.690787 medusa-zip-0.0.5/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-24 03:50:30.000000 medusa-zip-0.0.5/lib/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:50:39.690787 medusa-zip-0.0.5/lib/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-07-24 03:50:30.000000 medusa-zip-0.0.5/lib/src/crawl.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-07-24 03:50:30.000000 medusa-zip-0.0.5/lib/src/destination.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-24 03:50:30.000000 medusa-zip-0.0.5/lib/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-07-24 03:50:30.000000 medusa-zip-0.0.5/lib/src/merge.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    27895 2023-07-24 03:50:30.000000 medusa-zip-0.0.5/lib/src/zip.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:50:39.690787 medusa-zip-0.0.5/py/
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-24 03:50:30.000000 medusa-zip-0.0.5/py/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-24 03:50:30.000000 medusa-zip-0.0.5/py/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:50:39.690787 medusa-zip-0.0.5/py/medusa_zip/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-24 03:50:30.000000 medusa-zip-0.0.5/py/medusa_zip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-24 03:50:30.000000 medusa-zip-0.0.5/py/medusa_zip/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-24 03:50:30.000000 medusa-zip-0.0.5/py/medusa_zip/crawl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-24 03:50:30.000000 medusa-zip-0.0.5/py/medusa_zip/crawl.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-24 03:50:30.000000 medusa-zip-0.0.5/py/medusa_zip/destination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-24 03:50:30.000000 medusa-zip-0.0.5/py/medusa_zip/destination.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-24 03:50:30.000000 medusa-zip-0.0.5/py/medusa_zip/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-24 03:50:30.000000 medusa-zip-0.0.5/py/medusa_zip/merge.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 03:50:30.000000 medusa-zip-0.0.5/py/medusa_zip/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-24 03:50:30.000000 medusa-zip-0.0.5/py/medusa_zip/zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-07-24 03:50:30.000000 medusa-zip-0.0.5/py/medusa_zip/zip.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:50:39.690787 medusa-zip-0.0.5/py/medusa_zip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-24 03:50:39.000000 medusa-zip-0.0.5/py/medusa_zip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-24 03:50:39.000000 medusa-zip-0.0.5/py/medusa_zip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 03:50:39.000000 medusa-zip-0.0.5/py/medusa_zip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 03:50:39.000000 medusa-zip-0.0.5/py/medusa_zip.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-24 03:50:39.000000 medusa-zip-0.0.5/py/medusa_zip.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-24 03:50:39.000000 medusa-zip-0.0.5/py/medusa_zip.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:50:39.694787 medusa-zip-0.0.5/py/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-07-24 03:50:30.000000 medusa-zip-0.0.5/py/src/crawl.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-07-24 03:50:30.000000 medusa-zip-0.0.5/py/src/destination.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-07-24 03:50:30.000000 medusa-zip-0.0.5/py/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-07-24 03:50:30.000000 medusa-zip-0.0.5/py/src/merge.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-24 03:50:30.000000 medusa-zip-0.0.5/py/src/util.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    18240 2023-07-24 03:50:30.000000 medusa-zip-0.0.5/py/src/zip.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-24 03:50:30.000000 medusa-zip-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 03:50:39.694787 medusa-zip-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-24 03:50:30.000000 medusa-zip-0.0.5/setup.py
```

### Comparing `medusa-zip-0.0.2/Cargo.toml` & `medusa-zip-0.0.5/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 git                     = "https://github.com/cosmicexplorer/zip"
 rev                     = "79f818a8929b37eee6e7bf0e9284daa157a91aa7"
 package                 = "zip-merge"
 default-features        = false
 features                = ["deflate", "time", "rayon", "merge"]
 
 [workspace.package]
-version                 = "0.0.2"
+version                 = "0.0.5"
 authors                 = ["Danny McClanahan <dmcC2@hypnicjerk.ai>"]
 edition                 = "2021"
 license                 = "Apache-2.0"
 
 keywords                = ["zip", "file", "archive", "parallel", "io"]
 categories              = ["development-tools::build-utils", "filesystem", "asynchronous", "caching"]
 homepage                = "https://github.com/cosmicexplorer/medusa-zip"
 repository              = "https://github.com/cosmicexplorer/medusa-zip"
 
-[profile.release]
-strip                   = true
-lto                     = true
+# [profile.release]
+# strip                   = true
+# lto                     = true
```

### Comparing `medusa-zip-0.0.2/LICENSE` & `medusa-zip-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.2/PKG-INFO` & `medusa-zip-0.0.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medusa-zip
-Version: 0.0.2
+Version: 0.0.5
 Summary: High-performance parallelized implementations of common zip file operations.
 Author-email: Danny McClanahan <dmcC2@hypnicjerk.ai>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/cosmicexplorer/medusa-zip
 Project-URL: Repository, https://github.com/cosmicexplorer/medusa-zip
 Project-URL: Bug Tracker, https://github.com/cosmicexplorer/medusa-zip/issues
 Keywords: zip,rust,fs,file,archive,parallel,pyo3
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Rust
 Classifier: Operating System :: POSIX
+Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: File Formats
 Classifier: Topic :: System :: Archiving :: Compression
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Topic :: System :: Software Distribution
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
```

### Comparing `medusa-zip-0.0.2/README.md` & `medusa-zip-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.2/cli/Cargo.toml` & `medusa-zip-0.0.5/cli/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 repository.workspace    = true
 description             = "A command-line interface to high-performance parallelized implementations of common zip file operations."
 
 [dependencies]
 clap                    = { version = "4", features = ["derive"] }
 displaydoc.workspace    = true
 eyre                    = "0.6.8"
-libmedusa-zip           = { path = "../lib", version = "0.0.2" }
+libmedusa-zip           = { path = "../lib", version = "0.0.5" }
 regex                   = "1"
 serde                   = { version = "1", features = ["derive"] }
 serde_json              = "1.0"
 thiserror.workspace     = true
 time.workspace          = true
 tokio                   = { workspace = true, features = ["io-util", "io-std", "macros", "rt-multi-thread"] }
 zip.workspace           = true
```

### Comparing `medusa-zip-0.0.2/cli/src/crawl.rs` & `medusa-zip-0.0.5/cli/src/crawl.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.2/cli/src/destination.rs` & `medusa-zip-0.0.5/cli/src/destination.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.2/cli/src/main.rs` & `medusa-zip-0.0.5/cli/src/main.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.2/cli/src/merge.rs` & `medusa-zip-0.0.5/cli/src/merge.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.2/cli/src/util.rs` & `medusa-zip-0.0.5/cli/src/util.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.2/cli/src/zip.rs` & `medusa-zip-0.0.5/cli/src/zip.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.2/lib/Cargo.toml` & `medusa-zip-0.0.5/lib/Cargo.toml`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.2/lib/src/crawl.rs` & `medusa-zip-0.0.5/lib/src/crawl.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.2/lib/src/destination.rs` & `medusa-zip-0.0.5/lib/src/destination.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.2/lib/src/lib.rs` & `medusa-zip-0.0.5/lib/src/lib.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.2/lib/src/merge.rs` & `medusa-zip-0.0.5/lib/src/merge.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.2/lib/src/zip.rs` & `medusa-zip-0.0.5/lib/src/zip.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.2/py/Cargo.toml` & `medusa-zip-0.0.5/py/Cargo.toml`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 description             = "A PyOxidizer interface to high-performance parallelized implementations of common zip file operations."
 
 [lib]
 name                    = "pymedusa_zip"
 crate-type              = ["cdylib"]
 
 [dependencies]
-libmedusa-zip           = { path = "../lib", version = "0.0.2" }
+libmedusa-zip           = { path = "../lib", version = "0.0.5" }
 once_cell               = { version = "1", optional = true }
 pyo3                    = { version = "0.19", features = ["extension-module"] }
 pyo3-asyncio            = { version = "0.19", features = ["tokio-runtime"], optional = true }
 regex.workspace         = true
 time.workspace          = true
 tokio                   = { workspace = true, features = ["rt", "rt-multi-thread"] }
 zip.workspace           = true
```

### Comparing `medusa-zip-0.0.2/py/medusa_zip/crawl.pyi` & `medusa-zip-0.0.5/py/medusa_zip/crawl.pyi`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.2/py/medusa_zip/destination.pyi` & `medusa-zip-0.0.5/py/medusa_zip/destination.pyi`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.2/py/medusa_zip/merge.pyi` & `medusa-zip-0.0.5/py/medusa_zip/merge.pyi`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.2/py/medusa_zip/zip.pyi` & `medusa-zip-0.0.5/py/medusa_zip/zip.pyi`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.2/py/medusa_zip.egg-info/PKG-INFO` & `medusa-zip-0.0.5/py/medusa_zip.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medusa-zip
-Version: 0.0.2
+Version: 0.0.5
 Summary: High-performance parallelized implementations of common zip file operations.
 Author-email: Danny McClanahan <dmcC2@hypnicjerk.ai>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/cosmicexplorer/medusa-zip
 Project-URL: Repository, https://github.com/cosmicexplorer/medusa-zip
 Project-URL: Bug Tracker, https://github.com/cosmicexplorer/medusa-zip/issues
 Keywords: zip,rust,fs,file,archive,parallel,pyo3
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Rust
 Classifier: Operating System :: POSIX
+Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: File Formats
 Classifier: Topic :: System :: Archiving :: Compression
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Topic :: System :: Software Distribution
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
```

### Comparing `medusa-zip-0.0.2/py/medusa_zip.egg-info/SOURCES.txt` & `medusa-zip-0.0.5/py/medusa_zip.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.2/py/src/crawl.rs` & `medusa-zip-0.0.5/py/src/crawl.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.2/py/src/destination.rs` & `medusa-zip-0.0.5/py/src/destination.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.2/py/src/lib.rs` & `medusa-zip-0.0.5/py/src/lib.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.2/py/src/merge.rs` & `medusa-zip-0.0.5/py/src/merge.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.2/py/src/zip.rs` & `medusa-zip-0.0.5/py/src/zip.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.2/pyproject.toml` & `medusa-zip-0.0.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "medusa-zip"
-version = "0.0.2"
+version = "0.0.5"
 description = "High-performance parallelized implementations of common zip file operations."
 license = {text = "Apache-2.0"}
 readme = "py/README.md"
 authors = [
   {name = "Danny McClanahan", email = "dmcC2@hypnicjerk.ai"},
 ]
 keywords = ["zip", "rust", "fs", "file", "archive", "parallel", "pyo3"]
@@ -14,17 +14,18 @@
   "Development Status :: 2 - Pre-Alpha",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  # "Programming Language :: Python :: 3.12",
   "Programming Language :: Rust",
   "Operating System :: POSIX",
-  # "Operating System :: MacOS :: MacOS X",
+  "Operating System :: MacOS :: MacOS X",
   # "Operating System :: Microsoft :: Windows",
   "Topic :: Software Development :: Build Tools",
   "Topic :: File Formats",
   "Topic :: System :: Archiving :: Compression",
   "Topic :: System :: Archiving :: Packaging",
   "Topic :: System :: Software Distribution",
   "Topic :: Utilities",
@@ -51,14 +52,10 @@
 [tool.isort]
 profile = "hug"
 src_paths = ["py"]
 lines_after_imports = 2
 
 [tool.cibuildwheel]
 container-engine = "podman"
-before-all = "curl https://sh.rustup.rs -sSf | sh -s -- -y"
+before-all = "curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- --default-toolchain nightly -y"
 environment = { PATH="$HOME/.cargo/bin:$PATH" }
 build-verbosity = 3
-# skip = ["cp37-*", "cp38-*", "cp39-*", "cp310-*", "pp*", "*musllinux*"]
-
-[tool.cibuildwheel.linux]
-archs = ["auto64"]
```

### Comparing `medusa-zip-0.0.2/setup.py` & `medusa-zip-0.0.5/setup.py`

 * *Files identical despite different names*

