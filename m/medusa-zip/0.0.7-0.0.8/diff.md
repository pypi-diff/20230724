# Comparing `tmp/medusa-zip-0.0.7.tar.gz` & `tmp/medusa-zip-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medusa-zip-0.0.7.tar", last modified: Mon Jul 24 14:18:58 2023, max compression
+gzip compressed data, was "medusa-zip-0.0.8.tar", last modified: Mon Jul 24 15:19:28 2023, max compression
```

## Comparing `medusa-zip-0.0.7.tar` & `medusa-zip-0.0.8.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:18:58.194664 medusa-zip-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-24 14:18:58.190664 medusa-zip-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:18:58.186664 medusa-zip-0.0.7/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/cli/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:18:58.186664 medusa-zip-0.0.7/cli/src/
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/cli/src/crawl.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/cli/src/destination.rs
--rw-r--r--   0 runner    (1001) docker     (123)    11227 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/cli/src/main.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/cli/src/merge.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/cli/src/util.rs
--rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/cli/src/zip.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:18:58.186664 medusa-zip-0.0.7/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/lib/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:18:58.186664 medusa-zip-0.0.7/lib/src/
--rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/lib/src/crawl.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/lib/src/destination.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/lib/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/lib/src/merge.rs
--rw-r--r--   0 runner    (1001) docker     (123)    27895 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/lib/src/zip.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:18:58.186664 medusa-zip-0.0.7/py/
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/py/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/py/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:18:58.190664 medusa-zip-0.0.7/py/medusa_zip/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/py/medusa_zip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/py/medusa_zip/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/py/medusa_zip/crawl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/py/medusa_zip/crawl.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/py/medusa_zip/destination.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/py/medusa_zip/destination.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/py/medusa_zip/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/py/medusa_zip/merge.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/py/medusa_zip/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/py/medusa_zip/zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/py/medusa_zip/zip.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:18:58.190664 medusa-zip-0.0.7/py/medusa_zip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-24 14:18:58.000000 medusa-zip-0.0.7/py/medusa_zip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-24 14:18:58.000000 medusa-zip-0.0.7/py/medusa_zip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 14:18:58.000000 medusa-zip-0.0.7/py/medusa_zip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 14:18:57.000000 medusa-zip-0.0.7/py/medusa_zip.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-24 14:18:58.000000 medusa-zip-0.0.7/py/medusa_zip.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-24 14:18:58.000000 medusa-zip-0.0.7/py/medusa_zip.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:18:58.190664 medusa-zip-0.0.7/py/src/
--rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/py/src/crawl.rs
--rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/py/src/destination.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/py/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/py/src/merge.rs
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/py/src/util.rs
--rw-r--r--   0 runner    (1001) docker     (123)    18240 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/py/src/zip.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 14:18:58.194664 medusa-zip-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:19:28.874705 medusa-zip-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-24 15:19:19.000000 medusa-zip-0.0.8/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-07-24 15:19:19.000000 medusa-zip-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-24 15:19:19.000000 medusa-zip-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-24 15:19:28.874705 medusa-zip-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-24 15:19:19.000000 medusa-zip-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:19:28.870705 medusa-zip-0.0.8/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-24 15:19:19.000000 medusa-zip-0.0.8/cli/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:19:28.874705 medusa-zip-0.0.8/cli/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-07-24 15:19:19.000000 medusa-zip-0.0.8/cli/src/crawl.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-24 15:19:19.000000 medusa-zip-0.0.8/cli/src/destination.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    11227 2023-07-24 15:19:19.000000 medusa-zip-0.0.8/cli/src/main.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-24 15:19:19.000000 medusa-zip-0.0.8/cli/src/merge.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-24 15:19:19.000000 medusa-zip-0.0.8/cli/src/util.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-07-24 15:19:19.000000 medusa-zip-0.0.8/cli/src/zip.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:19:28.874705 medusa-zip-0.0.8/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-24 15:19:19.000000 medusa-zip-0.0.8/lib/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:19:28.874705 medusa-zip-0.0.8/lib/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-07-24 15:19:19.000000 medusa-zip-0.0.8/lib/src/crawl.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-07-24 15:19:19.000000 medusa-zip-0.0.8/lib/src/destination.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-24 15:19:19.000000 medusa-zip-0.0.8/lib/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-07-24 15:19:19.000000 medusa-zip-0.0.8/lib/src/merge.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    27895 2023-07-24 15:19:19.000000 medusa-zip-0.0.8/lib/src/zip.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:19:28.874705 medusa-zip-0.0.8/py/
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-24 15:19:19.000000 medusa-zip-0.0.8/py/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-24 15:19:19.000000 medusa-zip-0.0.8/py/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:19:28.874705 medusa-zip-0.0.8/py/medusa_zip/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-24 15:19:19.000000 medusa-zip-0.0.8/py/medusa_zip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-24 15:19:19.000000 medusa-zip-0.0.8/py/medusa_zip/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-24 15:19:19.000000 medusa-zip-0.0.8/py/medusa_zip/crawl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-24 15:19:19.000000 medusa-zip-0.0.8/py/medusa_zip/crawl.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-24 15:19:19.000000 medusa-zip-0.0.8/py/medusa_zip/destination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-24 15:19:19.000000 medusa-zip-0.0.8/py/medusa_zip/destination.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-24 15:19:19.000000 medusa-zip-0.0.8/py/medusa_zip/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-24 15:19:19.000000 medusa-zip-0.0.8/py/medusa_zip/merge.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 15:19:19.000000 medusa-zip-0.0.8/py/medusa_zip/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-24 15:19:19.000000 medusa-zip-0.0.8/py/medusa_zip/zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-07-24 15:19:19.000000 medusa-zip-0.0.8/py/medusa_zip/zip.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:19:28.874705 medusa-zip-0.0.8/py/medusa_zip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-24 15:19:28.000000 medusa-zip-0.0.8/py/medusa_zip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-24 15:19:28.000000 medusa-zip-0.0.8/py/medusa_zip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 15:19:28.000000 medusa-zip-0.0.8/py/medusa_zip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 15:19:28.000000 medusa-zip-0.0.8/py/medusa_zip.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-24 15:19:28.000000 medusa-zip-0.0.8/py/medusa_zip.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-24 15:19:28.000000 medusa-zip-0.0.8/py/medusa_zip.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:19:28.874705 medusa-zip-0.0.8/py/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-07-24 15:19:19.000000 medusa-zip-0.0.8/py/src/crawl.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-07-24 15:19:19.000000 medusa-zip-0.0.8/py/src/destination.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-07-24 15:19:19.000000 medusa-zip-0.0.8/py/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-07-24 15:19:19.000000 medusa-zip-0.0.8/py/src/merge.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-24 15:19:19.000000 medusa-zip-0.0.8/py/src/util.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    18240 2023-07-24 15:19:19.000000 medusa-zip-0.0.8/py/src/zip.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-24 15:19:19.000000 medusa-zip-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 15:19:28.878705 medusa-zip-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-24 15:19:19.000000 medusa-zip-0.0.8/setup.py
```

### Comparing `medusa-zip-0.0.7/Cargo.toml` & `medusa-zip-0.0.8/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 git                     = "https://github.com/cosmicexplorer/zip"
 rev                     = "79f818a8929b37eee6e7bf0e9284daa157a91aa7"
 package                 = "zip-merge"
 default-features        = false
 features                = ["deflate", "time", "rayon", "merge"]
 
 [workspace.package]
-version                 = "0.0.7"
+version                 = "0.0.8"
 authors                 = ["Danny McClanahan <dmcC2@hypnicjerk.ai>"]
 edition                 = "2021"
 license                 = "Apache-2.0"
 
 keywords                = ["zip", "file", "archive", "parallel", "io"]
 categories              = ["development-tools::build-utils", "filesystem", "asynchronous", "caching"]
 homepage                = "https://github.com/cosmicexplorer/medusa-zip"
```

### Comparing `medusa-zip-0.0.7/LICENSE` & `medusa-zip-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.7/PKG-INFO` & `medusa-zip-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medusa-zip
-Version: 0.0.7
+Version: 0.0.8
 Summary: High-performance parallelized implementations of common zip file operations.
 Author-email: Danny McClanahan <dmcC2@hypnicjerk.ai>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/cosmicexplorer/medusa-zip
 Project-URL: Repository, https://github.com/cosmicexplorer/medusa-zip
 Project-URL: Bug Tracker, https://github.com/cosmicexplorer/medusa-zip/issues
 Keywords: zip,rust,fs,file,archive,parallel,pyo3
```

### Comparing `medusa-zip-0.0.7/README.md` & `medusa-zip-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.7/cli/Cargo.toml` & `medusa-zip-0.0.8/cli/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 repository.workspace    = true
 description             = "A command-line interface to high-performance parallelized implementations of common zip file operations."
 
 [dependencies]
 clap                    = { version = "4", features = ["derive"] }
 displaydoc.workspace    = true
 eyre                    = "0.6.8"
-libmedusa-zip           = { path = "../lib", version = "0.0.7" }
+libmedusa-zip           = { path = "../lib", version = "0.0.8" }
 regex                   = "1"
 serde                   = { version = "1", features = ["derive"] }
 serde_json              = "1.0"
 thiserror.workspace     = true
 time.workspace          = true
 tokio                   = { workspace = true, features = ["io-util", "io-std", "macros", "rt-multi-thread"] }
 zip.workspace           = true
```

### Comparing `medusa-zip-0.0.7/cli/src/crawl.rs` & `medusa-zip-0.0.8/cli/src/crawl.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.7/cli/src/destination.rs` & `medusa-zip-0.0.8/cli/src/destination.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.7/cli/src/main.rs` & `medusa-zip-0.0.8/cli/src/main.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.7/cli/src/merge.rs` & `medusa-zip-0.0.8/cli/src/merge.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.7/cli/src/util.rs` & `medusa-zip-0.0.8/cli/src/util.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.7/cli/src/zip.rs` & `medusa-zip-0.0.8/cli/src/zip.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.7/lib/Cargo.toml` & `medusa-zip-0.0.8/lib/Cargo.toml`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.7/lib/src/crawl.rs` & `medusa-zip-0.0.8/lib/src/crawl.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.7/lib/src/destination.rs` & `medusa-zip-0.0.8/lib/src/destination.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.7/lib/src/lib.rs` & `medusa-zip-0.0.8/lib/src/lib.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.7/lib/src/merge.rs` & `medusa-zip-0.0.8/lib/src/merge.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.7/lib/src/zip.rs` & `medusa-zip-0.0.8/lib/src/zip.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.7/py/Cargo.toml` & `medusa-zip-0.0.8/py/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 description             = "A PyOxidizer interface to high-performance parallelized implementations of common zip file operations."
 
 [lib]
 name                    = "pymedusa_zip"
 crate-type              = ["cdylib"]
 
 [dependencies]
-libmedusa-zip           = { path = "../lib", version = "0.0.7" }
+libmedusa-zip           = { path = "../lib", version = "0.0.8" }
 once_cell               = { version = "1", optional = true }
 pyo3                    = { version = "0.19", features = ["extension-module"] }
 pyo3-asyncio            = { version = "0.19", features = ["tokio-runtime"], optional = true }
 regex.workspace         = true
 time.workspace          = true
 tokio                   = { workspace = true, features = ["rt", "rt-multi-thread"] }
 zip.workspace           = true
```

### Comparing `medusa-zip-0.0.7/py/medusa_zip/crawl.pyi` & `medusa-zip-0.0.8/py/medusa_zip/crawl.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 #
 # Copyright (C) 2023 Danny McClanahan <dmcC2@hypnicjerk.ai>
 # SPDX-License-Identifier: Apache-2.0
 #
 # Licensed under the Apache License, Version 2.0 (see LICENSE).
 
 from pathlib import Path
-from typing import Iterable, Optional
+from typing import Iterable, Optional, Union
 
 from .zip import EntryModifications, MedusaZip, Parallelism, ZipOutputOptions
 
 
 class ResolvedPath:
-  def __init__(self, *, unresolved_path: Path, resolved_path: Path) -> None:
+  def __init__(self, *, unresolved_path: Union[str, Path], resolved_path: Union[str, Path]) -> None:
     ...
 
   @property
   def unresolved_path(self) -> Path: ...
   @property
   def resolved_path(self) -> Path: ...
 
@@ -42,15 +42,19 @@
     ...
 
   @classmethod
   def default(cls) -> 'Ignores': ...
 
 
 class MedusaCrawl:
-  def __init__(self, paths_to_crawl: Iterable[Path], ignores: Optional[Ignores] = None) -> None:
+  def __init__(
+    self,
+    paths_to_crawl: Iterable[Union[str, Path]],
+    ignores: Optional[Ignores] = None,
+  ) -> None:
     ...
 
   @property
   def paths_to_crawl(self) -> Iterable[Path]: ...
   @property
   def ignores(self) -> Ignores: ...
```

### Comparing `medusa-zip-0.0.7/py/medusa_zip/destination.pyi` & `medusa-zip-0.0.8/py/medusa_zip/destination.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Description: ???
 #
 # Copyright (C) 2023 Danny McClanahan <dmcC2@hypnicjerk.ai>
 # SPDX-License-Identifier: Apache-2.0
 #
 # Licensed under the Apache License, Version 2.0 (see LICENSE).
 
-from pathlib import Path
+from pathlib import Path, Union
 from typing import Any
 
 
 class ZipFileWriter:
   @property
   def output_path(self) -> Path: ...
 
@@ -33,12 +33,12 @@
   AppendToNonZip: 'DestinationBehavior'
 
   def __int__(self) -> int: ...
 
   @classmethod
   def default(cls) -> 'DestinationBehavior': ...
 
-  async def initialize(self, path: Path) -> ZipFileWriter:
+  async def initialize(self, path: Union[str, Path]) -> ZipFileWriter:
     ...
 
-  def initialize_sync(self, path: Path) -> ZipFileWriter:
+  def initialize_sync(self, path: Union[str, Path]) -> ZipFileWriter:
     ...
```

### Comparing `medusa-zip-0.0.7/py/medusa_zip/merge.pyi` & `medusa-zip-0.0.8/py/medusa_zip/merge.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,19 @@
 
 from . import EntryName
 from .destination import ZipFileWriter
 from .zip import ModifiedTimeBehavior
 
 
 class MergeGroup:
-  def __init__(self, prefix: Optional[Union[str, EntryName]], sources: Iterable[Path]) -> None:
+  def __init__(
+    self,
+    prefix: Optional[Union[str, EntryName]],
+    sources: Iterable[Union[str, Path]],
+  ) -> None:
     ...
 
   @property
   def prefix(self) -> Optional[EntryName]: ...
   @property
   def sources(self) -> List[Path]: ...
```

### Comparing `medusa-zip-0.0.7/py/medusa_zip/zip.pyi` & `medusa-zip-0.0.8/py/medusa_zip/zip.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -139,12 +139,12 @@
     input_files: Iterable[FileSource],
     zip_options: Optional[ZipOutputOptions] = None,
     modifications: Optional[EntryModifications] = None,
     parallelism: Optional[Parallelism] = None,
   ) -> None:
     ...
 
-  async def zip(output_zip: ZipFileWriter) -> ZipFileWriter:
+  async def zip(self, output_zip: ZipFileWriter) -> ZipFileWriter:
     ...
 
-  def zip_sync(output_zip: ZipFileWriter) -> ZipFileWriter:
+  def zip_sync(self, output_zip: ZipFileWriter) -> ZipFileWriter:
     ...
```

### Comparing `medusa-zip-0.0.7/py/medusa_zip.egg-info/PKG-INFO` & `medusa-zip-0.0.8/py/medusa_zip.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medusa-zip
-Version: 0.0.7
+Version: 0.0.8
 Summary: High-performance parallelized implementations of common zip file operations.
 Author-email: Danny McClanahan <dmcC2@hypnicjerk.ai>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/cosmicexplorer/medusa-zip
 Project-URL: Repository, https://github.com/cosmicexplorer/medusa-zip
 Project-URL: Bug Tracker, https://github.com/cosmicexplorer/medusa-zip/issues
 Keywords: zip,rust,fs,file,archive,parallel,pyo3
```

### Comparing `medusa-zip-0.0.7/py/medusa_zip.egg-info/SOURCES.txt` & `medusa-zip-0.0.8/py/medusa_zip.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.7/py/src/crawl.rs` & `medusa-zip-0.0.8/py/src/crawl.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.7/py/src/destination.rs` & `medusa-zip-0.0.8/py/src/destination.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.7/py/src/lib.rs` & `medusa-zip-0.0.8/py/src/lib.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.7/py/src/merge.rs` & `medusa-zip-0.0.8/py/src/merge.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.7/py/src/zip.rs` & `medusa-zip-0.0.8/py/src/zip.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.7/pyproject.toml` & `medusa-zip-0.0.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "medusa-zip"
-version = "0.0.7"
+version = "0.0.8"
 description = "High-performance parallelized implementations of common zip file operations."
 license = {text = "Apache-2.0"}
 readme = "py/README.md"
 authors = [
   {name = "Danny McClanahan", email = "dmcC2@hypnicjerk.ai"},
 ]
 keywords = ["zip", "rust", "fs", "file", "archive", "parallel", "pyo3"]
```

### Comparing `medusa-zip-0.0.7/setup.py` & `medusa-zip-0.0.8/setup.py`

 * *Files identical despite different names*

