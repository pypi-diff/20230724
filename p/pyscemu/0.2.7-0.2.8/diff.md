# Comparing `tmp/pyscemu-0.2.7.tar.gz` & `tmp/pyscemu-0.2.8.tar.gz`

## Comparing `pyscemu-0.2.7.tar` & `pyscemu-0.2.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      309 1970-01-01 00:00:00.000000 pyscemu-0.2.7/Cargo.toml
--rw-r--r--   0     1000     1000     2809 2023-04-28 16:18:25.000000 pyscemu-0.2.7/.github/workflows/CI.yml
--rw-r--r--   0     1000     1000      692 2023-04-29 18:18:29.000000 pyscemu-0.2.7/.gitignore
--rw-r--r--   0     1000     1000    11773 2023-07-03 19:42:43.000000 pyscemu-0.2.7/DOCUMENTATION.md
--rw-r--r--   0     1000     1000    10083 2023-05-09 16:58:06.000000 pyscemu-0.2.7/README.md
--rw-r--r--   0     1000     1000     2017 2023-04-30 22:51:14.000000 pyscemu-0.2.7/examples/danabot_rsa.ipynb
--rw-r--r--   0     1000     1000     6831 2023-04-30 22:52:26.000000 pyscemu-0.2.7/examples/raccoon_strings.ipynb
--rw-r--r--   0     1000     1000        0 2023-04-30 16:12:18.000000 pyscemu-0.2.7/examples/scripts/.ipynb_checkpoints/test-checkpoint.py
--rw-r--r--   0     1000     1000      727 2023-04-30 13:08:15.000000 pyscemu-0.2.7/examples/scripts/raccoon_strings.py
--rw-r--r--   0     1000     1000      766 2023-05-09 15:35:14.000000 pyscemu-0.2.7/examples/scripts/test.py
--rw-r--r--   0     1000     1000      561 2023-04-29 17:52:46.000000 pyscemu-0.2.7/examples/scripts/xloader_dexor.py
--rw-r--r--   0     1000     1000      427 2023-05-10 08:13:44.000000 pyscemu-0.2.7/examples/scripts/xloader_keygen.py
--rw-r--r--   0     1000     1000     1757 2023-04-30 15:03:12.000000 pyscemu-0.2.7/examples/xloader_keygen.ipynb
--rw-r--r--   0     1000     1000      433 2023-05-01 11:01:29.000000 pyscemu-0.2.7/pyproject.toml
--rw-r--r--   0     1000     1000    26776 2023-07-03 19:39:30.000000 pyscemu-0.2.7/src/lib.rs
--rw-r--r--   0     1000     1000    32749 2023-07-03 20:01:07.000000 pyscemu-0.2.7/Cargo.lock
--rw-r--r--   0        0        0    10409 1970-01-01 00:00:00.000000 pyscemu-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0      309 1970-01-01 00:00:00.000000 pyscemu-0.2.8/Cargo.toml
+-rw-r--r--   0     1000     1000     2809 2023-04-28 16:18:25.000000 pyscemu-0.2.8/.github/workflows/CI.yml
+-rw-r--r--   0     1000     1000      692 2023-04-29 18:18:29.000000 pyscemu-0.2.8/.gitignore
+-rw-r--r--   0     1000     1000    11773 2023-07-03 19:42:43.000000 pyscemu-0.2.8/DOCUMENTATION.md
+-rw-r--r--   0     1000     1000    10083 2023-05-09 16:58:06.000000 pyscemu-0.2.8/README.md
+-rw-r--r--   0     1000     1000     2017 2023-04-30 22:51:14.000000 pyscemu-0.2.8/examples/danabot_rsa.ipynb
+-rw-r--r--   0     1000     1000     6831 2023-04-30 22:52:26.000000 pyscemu-0.2.8/examples/raccoon_strings.ipynb
+-rw-r--r--   0     1000     1000        0 2023-04-30 16:12:18.000000 pyscemu-0.2.8/examples/scripts/.ipynb_checkpoints/test-checkpoint.py
+-rw-r--r--   0     1000     1000      727 2023-04-30 13:08:15.000000 pyscemu-0.2.8/examples/scripts/raccoon_strings.py
+-rw-r--r--   0     1000     1000      766 2023-05-09 15:35:14.000000 pyscemu-0.2.8/examples/scripts/test.py
+-rw-r--r--   0     1000     1000      561 2023-04-29 17:52:46.000000 pyscemu-0.2.8/examples/scripts/xloader_dexor.py
+-rw-r--r--   0     1000     1000      427 2023-05-10 08:13:44.000000 pyscemu-0.2.8/examples/scripts/xloader_keygen.py
+-rw-r--r--   0     1000     1000     1757 2023-04-30 15:03:12.000000 pyscemu-0.2.8/examples/xloader_keygen.ipynb
+-rw-r--r--   0     1000     1000      433 2023-05-01 11:01:29.000000 pyscemu-0.2.8/pyproject.toml
+-rw-r--r--   0     1000     1000    26776 2023-07-03 19:39:30.000000 pyscemu-0.2.8/src/lib.rs
+-rw-r--r--   0     1000     1000    33592 2023-07-23 22:11:59.000000 pyscemu-0.2.8/Cargo.lock
+-rw-r--r--   0        0        0    10409 1970-01-01 00:00:00.000000 pyscemu-0.2.8/PKG-INFO
```

### Comparing `pyscemu-0.2.7/.github/workflows/CI.yml` & `pyscemu-0.2.8/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.7/.gitignore` & `pyscemu-0.2.8/.gitignore`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.7/DOCUMENTATION.md` & `pyscemu-0.2.8/DOCUMENTATION.md`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.7/README.md` & `pyscemu-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.7/examples/danabot_rsa.ipynb` & `pyscemu-0.2.8/examples/danabot_rsa.ipynb`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.7/examples/raccoon_strings.ipynb` & `pyscemu-0.2.8/examples/raccoon_strings.ipynb`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.7/examples/scripts/raccoon_strings.py` & `pyscemu-0.2.8/examples/scripts/raccoon_strings.py`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.7/examples/scripts/test.py` & `pyscemu-0.2.8/examples/scripts/test.py`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.7/examples/scripts/xloader_dexor.py` & `pyscemu-0.2.8/examples/scripts/xloader_dexor.py`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.7/examples/xloader_keygen.ipynb` & `pyscemu-0.2.8/examples/xloader_keygen.ipynb`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.7/src/lib.rs` & `pyscemu-0.2.8/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.7/Cargo.lock` & `pyscemu-0.2.8/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,20 @@
 [[package]]
 name = "bumpalo"
 version = "3.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9b1ce199063694f33ffb7dd4e0ee620741495c32833cde5aa08f02a0bf96f0c8"
 
 [[package]]
+name = "byteorder"
+version = "1.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
+
+[[package]]
 name = "bytes"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89b2fd2a0dcf38d7971e2194b6b6eebab45ae01067456a7fd93d5547a61b70be"
 
 [[package]]
 name = "cc"
@@ -136,14 +142,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b540bd8bc810d3885c6ea91e2018302f68baba2129ab3e88f32389ee9370880d"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
+name = "crunchy"
+version = "0.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7a81dae078cea95a014a339291cec439d2f232ebe854a9d672b796c6afafa9b7"
+
+[[package]]
 name = "ctrlc"
 version = "3.2.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bbcf33c2a618cbe41ee43ae6e9f2e48368cd9f9db2896f10167d8d762679f639"
 dependencies = [
  "nix",
  "windows-sys 0.45.0",
@@ -286,14 +298,20 @@
 [[package]]
 name = "hermit-abi"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
 
 [[package]]
+name = "hex"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7f24254aa9a54b5c858eaee2f5bccdb46aaf0e486a595ed5fd8f86ba55232a70"
+
+[[package]]
 name = "http"
 version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bd6effc99afb63425aff9b05836f029929e345a6148a14b7ecd5ab67af944482"
 dependencies = [
  "bytes",
  "fnv",
@@ -322,17 +340,17 @@
 dependencies = [
  "cxx",
  "cxx-build",
 ]
 
 [[package]]
 name = "iced-x86"
-version = "1.18.0"
+version = "1.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1dd04b950d75b3498320253b17fb92745b2cc79ead8814aede2f7c1bab858bec"
+checksum = "cdd366a53278429c028367e0ba22a46cab6d565a57afb959f06e92c7a69e7828"
 dependencies = [
  "lazy_static",
 ]
 
 [[package]]
 name = "idna"
 version = "0.3.0"
@@ -394,27 +412,28 @@
 name = "libc"
 version = "0.2.142"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
 
 [[package]]
 name = "libscemu"
-version = "0.12.7"
+version = "0.12.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8eedf686dbb13ada4843b35ab8590fff629c2823e6c30bd22a8b35ef5bc8c24c"
+checksum = "7725cdb02c968c1b386fe28095a29f52d6024e874f56161c94b55ef7f2d49f37"
 dependencies = [
  "attohttpc",
  "atty",
  "chrono",
  "ctrlc",
  "iced-x86",
  "lazy_static",
  "md5",
  "rand",
  "scan_fmt",
+ "uint",
 ]
 
 [[package]]
 name = "link-cplusplus"
 version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ecd207c9c713c34f95a097a5b029ac2ce6010530c7b49d7fea24d977dede04f5"
@@ -684,15 +703,15 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyscemu"
-version = "0.2.7"
+version = "0.2.8"
 dependencies = [
  "libscemu",
  "pyo3",
 ]
 
 [[package]]
 name = "quote"
@@ -926,14 +945,26 @@
 [[package]]
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
+name = "uint"
+version = "0.9.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "76f64bba2c53b04fcab63c01a7d7427eadc821e3bc48c34dc9ba29c501164b52"
+dependencies = [
+ "byteorder",
+ "crunchy",
+ "hex",
+ "static_assertions",
+]
+
+[[package]]
 name = "unicode-bidi"
 version = "0.3.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "92888ba5573ff080736b3648696b70cafad7d250551175acbaa4e0385b3e1460"
 
 [[package]]
 name = "unicode-ident"
```

### Comparing `pyscemu-0.2.7/PKG-INFO` & `pyscemu-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscemu
-Version: 0.2.7
+Version: 0.2.8
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # PYSCEMU
```

