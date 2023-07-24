# Comparing `tmp/medusa-zip-0.0.6.tar.gz` & `tmp/medusa-zip-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medusa-zip-0.0.6.tar", last modified: Mon Jul 24 05:54:16 2023, max compression
+gzip compressed data, was "medusa-zip-0.0.7.tar", last modified: Mon Jul 24 14:18:58 2023, max compression
```

## Comparing `medusa-zip-0.0.6.tar` & `medusa-zip-0.0.7.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:54:16.061228 medusa-zip-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-24 05:54:04.000000 medusa-zip-0.0.6/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-07-24 05:54:04.000000 medusa-zip-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-24 05:54:04.000000 medusa-zip-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-24 05:54:16.061228 medusa-zip-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-24 05:54:04.000000 medusa-zip-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:54:16.053228 medusa-zip-0.0.6/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-24 05:54:04.000000 medusa-zip-0.0.6/cli/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:54:16.057228 medusa-zip-0.0.6/cli/src/
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-07-24 05:54:04.000000 medusa-zip-0.0.6/cli/src/crawl.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-24 05:54:04.000000 medusa-zip-0.0.6/cli/src/destination.rs
--rw-r--r--   0 runner    (1001) docker     (123)    11227 2023-07-24 05:54:04.000000 medusa-zip-0.0.6/cli/src/main.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-24 05:54:04.000000 medusa-zip-0.0.6/cli/src/merge.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-24 05:54:04.000000 medusa-zip-0.0.6/cli/src/util.rs
--rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-07-24 05:54:04.000000 medusa-zip-0.0.6/cli/src/zip.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:54:16.057228 medusa-zip-0.0.6/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-24 05:54:04.000000 medusa-zip-0.0.6/lib/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:54:16.057228 medusa-zip-0.0.6/lib/src/
--rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-07-24 05:54:04.000000 medusa-zip-0.0.6/lib/src/crawl.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-07-24 05:54:04.000000 medusa-zip-0.0.6/lib/src/destination.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-24 05:54:04.000000 medusa-zip-0.0.6/lib/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-07-24 05:54:04.000000 medusa-zip-0.0.6/lib/src/merge.rs
--rw-r--r--   0 runner    (1001) docker     (123)    27895 2023-07-24 05:54:04.000000 medusa-zip-0.0.6/lib/src/zip.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:54:16.057228 medusa-zip-0.0.6/py/
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-24 05:54:04.000000 medusa-zip-0.0.6/py/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-24 05:54:04.000000 medusa-zip-0.0.6/py/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:54:16.057228 medusa-zip-0.0.6/py/medusa_zip/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-24 05:54:04.000000 medusa-zip-0.0.6/py/medusa_zip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-24 05:54:04.000000 medusa-zip-0.0.6/py/medusa_zip/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-24 05:54:04.000000 medusa-zip-0.0.6/py/medusa_zip/crawl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-24 05:54:04.000000 medusa-zip-0.0.6/py/medusa_zip/crawl.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-24 05:54:04.000000 medusa-zip-0.0.6/py/medusa_zip/destination.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-24 05:54:04.000000 medusa-zip-0.0.6/py/medusa_zip/destination.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-24 05:54:04.000000 medusa-zip-0.0.6/py/medusa_zip/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-24 05:54:04.000000 medusa-zip-0.0.6/py/medusa_zip/merge.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 05:54:04.000000 medusa-zip-0.0.6/py/medusa_zip/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-24 05:54:04.000000 medusa-zip-0.0.6/py/medusa_zip/zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-07-24 05:54:04.000000 medusa-zip-0.0.6/py/medusa_zip/zip.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:54:16.061228 medusa-zip-0.0.6/py/medusa_zip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-24 05:54:16.000000 medusa-zip-0.0.6/py/medusa_zip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-24 05:54:16.000000 medusa-zip-0.0.6/py/medusa_zip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 05:54:16.000000 medusa-zip-0.0.6/py/medusa_zip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 05:54:15.000000 medusa-zip-0.0.6/py/medusa_zip.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-24 05:54:16.000000 medusa-zip-0.0.6/py/medusa_zip.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-24 05:54:16.000000 medusa-zip-0.0.6/py/medusa_zip.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:54:16.061228 medusa-zip-0.0.6/py/src/
--rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-07-24 05:54:04.000000 medusa-zip-0.0.6/py/src/crawl.rs
--rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-07-24 05:54:04.000000 medusa-zip-0.0.6/py/src/destination.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-07-24 05:54:04.000000 medusa-zip-0.0.6/py/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-07-24 05:54:04.000000 medusa-zip-0.0.6/py/src/merge.rs
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-24 05:54:04.000000 medusa-zip-0.0.6/py/src/util.rs
--rw-r--r--   0 runner    (1001) docker     (123)    18240 2023-07-24 05:54:04.000000 medusa-zip-0.0.6/py/src/zip.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-24 05:54:04.000000 medusa-zip-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 05:54:16.061228 medusa-zip-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-24 05:54:04.000000 medusa-zip-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:18:58.194664 medusa-zip-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-24 14:18:58.190664 medusa-zip-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:18:58.186664 medusa-zip-0.0.7/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/cli/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:18:58.186664 medusa-zip-0.0.7/cli/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/cli/src/crawl.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/cli/src/destination.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    11227 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/cli/src/main.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/cli/src/merge.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/cli/src/util.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/cli/src/zip.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:18:58.186664 medusa-zip-0.0.7/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/lib/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:18:58.186664 medusa-zip-0.0.7/lib/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/lib/src/crawl.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/lib/src/destination.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/lib/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/lib/src/merge.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    27895 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/lib/src/zip.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:18:58.186664 medusa-zip-0.0.7/py/
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/py/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/py/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:18:58.190664 medusa-zip-0.0.7/py/medusa_zip/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/py/medusa_zip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/py/medusa_zip/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/py/medusa_zip/crawl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/py/medusa_zip/crawl.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/py/medusa_zip/destination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/py/medusa_zip/destination.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/py/medusa_zip/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/py/medusa_zip/merge.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/py/medusa_zip/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/py/medusa_zip/zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/py/medusa_zip/zip.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:18:58.190664 medusa-zip-0.0.7/py/medusa_zip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-24 14:18:58.000000 medusa-zip-0.0.7/py/medusa_zip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-24 14:18:58.000000 medusa-zip-0.0.7/py/medusa_zip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 14:18:58.000000 medusa-zip-0.0.7/py/medusa_zip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 14:18:57.000000 medusa-zip-0.0.7/py/medusa_zip.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-24 14:18:58.000000 medusa-zip-0.0.7/py/medusa_zip.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-24 14:18:58.000000 medusa-zip-0.0.7/py/medusa_zip.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:18:58.190664 medusa-zip-0.0.7/py/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/py/src/crawl.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/py/src/destination.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/py/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/py/src/merge.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/py/src/util.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    18240 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/py/src/zip.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 14:18:58.194664 medusa-zip-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-24 14:18:47.000000 medusa-zip-0.0.7/setup.py
```

### Comparing `medusa-zip-0.0.6/Cargo.toml` & `medusa-zip-0.0.7/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 git                     = "https://github.com/cosmicexplorer/zip"
 rev                     = "79f818a8929b37eee6e7bf0e9284daa157a91aa7"
 package                 = "zip-merge"
 default-features        = false
 features                = ["deflate", "time", "rayon", "merge"]
 
 [workspace.package]
-version                 = "0.0.6"
+version                 = "0.0.7"
 authors                 = ["Danny McClanahan <dmcC2@hypnicjerk.ai>"]
 edition                 = "2021"
 license                 = "Apache-2.0"
 
 keywords                = ["zip", "file", "archive", "parallel", "io"]
 categories              = ["development-tools::build-utils", "filesystem", "asynchronous", "caching"]
 homepage                = "https://github.com/cosmicexplorer/medusa-zip"
```

### Comparing `medusa-zip-0.0.6/LICENSE` & `medusa-zip-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.6/PKG-INFO` & `medusa-zip-0.0.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medusa-zip
-Version: 0.0.6
+Version: 0.0.7
 Summary: High-performance parallelized implementations of common zip file operations.
 Author-email: Danny McClanahan <dmcC2@hypnicjerk.ai>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/cosmicexplorer/medusa-zip
 Project-URL: Repository, https://github.com/cosmicexplorer/medusa-zip
 Project-URL: Bug Tracker, https://github.com/cosmicexplorer/medusa-zip/issues
 Keywords: zip,rust,fs,file,archive,parallel,pyo3
@@ -15,22 +15,28 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Rust
 Classifier: Operating System :: POSIX
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: File Formats
 Classifier: Topic :: System :: Archiving :: Compression
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Topic :: System :: Software Distribution
+Classifier: Topic :: System :: Filesystems
 Classifier: Topic :: Utilities
+Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: asyncio
 Provides-Extra: sync
 License-File: LICENSE
 
 pymedusa-zip
```

### Comparing `medusa-zip-0.0.6/README.md` & `medusa-zip-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.6/cli/Cargo.toml` & `medusa-zip-0.0.7/cli/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 repository.workspace    = true
 description             = "A command-line interface to high-performance parallelized implementations of common zip file operations."
 
 [dependencies]
 clap                    = { version = "4", features = ["derive"] }
 displaydoc.workspace    = true
 eyre                    = "0.6.8"
-libmedusa-zip           = { path = "../lib", version = "0.0.6" }
+libmedusa-zip           = { path = "../lib", version = "0.0.7" }
 regex                   = "1"
 serde                   = { version = "1", features = ["derive"] }
 serde_json              = "1.0"
 thiserror.workspace     = true
 time.workspace          = true
 tokio                   = { workspace = true, features = ["io-util", "io-std", "macros", "rt-multi-thread"] }
 zip.workspace           = true
```

### Comparing `medusa-zip-0.0.6/cli/src/crawl.rs` & `medusa-zip-0.0.7/cli/src/crawl.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.6/cli/src/destination.rs` & `medusa-zip-0.0.7/cli/src/destination.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.6/cli/src/main.rs` & `medusa-zip-0.0.7/cli/src/main.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.6/cli/src/merge.rs` & `medusa-zip-0.0.7/cli/src/merge.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.6/cli/src/util.rs` & `medusa-zip-0.0.7/cli/src/util.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.6/cli/src/zip.rs` & `medusa-zip-0.0.7/cli/src/zip.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.6/lib/Cargo.toml` & `medusa-zip-0.0.7/lib/Cargo.toml`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.6/lib/src/crawl.rs` & `medusa-zip-0.0.7/lib/src/crawl.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.6/lib/src/destination.rs` & `medusa-zip-0.0.7/lib/src/destination.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.6/lib/src/lib.rs` & `medusa-zip-0.0.7/lib/src/lib.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.6/lib/src/merge.rs` & `medusa-zip-0.0.7/lib/src/merge.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.6/lib/src/zip.rs` & `medusa-zip-0.0.7/lib/src/zip.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.6/py/Cargo.toml` & `medusa-zip-0.0.7/py/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 description             = "A PyOxidizer interface to high-performance parallelized implementations of common zip file operations."
 
 [lib]
 name                    = "pymedusa_zip"
 crate-type              = ["cdylib"]
 
 [dependencies]
-libmedusa-zip           = { path = "../lib", version = "0.0.6" }
+libmedusa-zip           = { path = "../lib", version = "0.0.7" }
 once_cell               = { version = "1", optional = true }
 pyo3                    = { version = "0.19", features = ["extension-module"] }
 pyo3-asyncio            = { version = "0.19", features = ["tokio-runtime"], optional = true }
 regex.workspace         = true
 time.workspace          = true
 tokio                   = { workspace = true, features = ["rt", "rt-multi-thread"] }
 zip.workspace           = true
```

### Comparing `medusa-zip-0.0.6/py/medusa_zip/crawl.pyi` & `medusa-zip-0.0.7/py/medusa_zip/crawl.pyi`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.6/py/medusa_zip/destination.pyi` & `medusa-zip-0.0.7/py/medusa_zip/destination.pyi`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.6/py/medusa_zip/merge.pyi` & `medusa-zip-0.0.7/py/medusa_zip/merge.pyi`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.6/py/medusa_zip/zip.pyi` & `medusa-zip-0.0.7/py/medusa_zip/zip.pyi`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.6/py/medusa_zip.egg-info/PKG-INFO` & `medusa-zip-0.0.7/py/medusa_zip.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medusa-zip
-Version: 0.0.6
+Version: 0.0.7
 Summary: High-performance parallelized implementations of common zip file operations.
 Author-email: Danny McClanahan <dmcC2@hypnicjerk.ai>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/cosmicexplorer/medusa-zip
 Project-URL: Repository, https://github.com/cosmicexplorer/medusa-zip
 Project-URL: Bug Tracker, https://github.com/cosmicexplorer/medusa-zip/issues
 Keywords: zip,rust,fs,file,archive,parallel,pyo3
@@ -15,22 +15,28 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Rust
 Classifier: Operating System :: POSIX
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: File Formats
 Classifier: Topic :: System :: Archiving :: Compression
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Topic :: System :: Software Distribution
+Classifier: Topic :: System :: Filesystems
 Classifier: Topic :: Utilities
+Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: asyncio
 Provides-Extra: sync
 License-File: LICENSE
 
 pymedusa-zip
```

### Comparing `medusa-zip-0.0.6/py/medusa_zip.egg-info/SOURCES.txt` & `medusa-zip-0.0.7/py/medusa_zip.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.6/py/src/crawl.rs` & `medusa-zip-0.0.7/py/src/crawl.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.6/py/src/destination.rs` & `medusa-zip-0.0.7/py/src/destination.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.6/py/src/lib.rs` & `medusa-zip-0.0.7/py/src/lib.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.6/py/src/merge.rs` & `medusa-zip-0.0.7/py/src/merge.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.6/py/src/zip.rs` & `medusa-zip-0.0.7/py/src/zip.rs`

 * *Files identical despite different names*

### Comparing `medusa-zip-0.0.6/pyproject.toml` & `medusa-zip-0.0.7/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 [project]
 name = "medusa-zip"
-version = "0.0.6"
+version = "0.0.7"
 description = "High-performance parallelized implementations of common zip file operations."
 license = {text = "Apache-2.0"}
 readme = "py/README.md"
 authors = [
   {name = "Danny McClanahan", email = "dmcC2@hypnicjerk.ai"},
 ]
 keywords = ["zip", "rust", "fs", "file", "archive", "parallel", "pyo3"]
 classifiers = [
   "License :: OSI Approved :: Apache Software License",
   "Intended Audience :: Developers",
   "Development Status :: 2 - Pre-Alpha",
   "Programming Language :: Python :: 3",
-  # "Programming Language :: Python :: 3.6",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
-  # "Programming Language :: Python :: 3.12",
   "Programming Language :: Rust",
   "Operating System :: POSIX",
+  "Operating System :: POSIX :: Linux",
+  "Operating System :: Unix",
   "Operating System :: MacOS :: MacOS X",
   "Operating System :: Microsoft :: Windows",
+  "Programming Language :: Python :: Implementation :: CPython",
+  "Programming Language :: Python :: Implementation :: PyPy",
   "Topic :: Software Development :: Build Tools",
   "Topic :: File Formats",
   "Topic :: System :: Archiving :: Compression",
   "Topic :: System :: Archiving :: Packaging",
   "Topic :: System :: Software Distribution",
+  "Topic :: System :: Filesystems",
   "Topic :: Utilities",
+  "Typing :: Typed",
 ]
 requires-python = ">=3.7"
 
 [project.urls]
 Homepage = "https://github.com/cosmicexplorer/medusa-zip"
 Repository = "https://github.com/cosmicexplorer/medusa-zip"
 "Bug Tracker" = "https://github.com/cosmicexplorer/medusa-zip/issues"
```

### Comparing `medusa-zip-0.0.6/setup.py` & `medusa-zip-0.0.7/setup.py`

 * *Files identical despite different names*

