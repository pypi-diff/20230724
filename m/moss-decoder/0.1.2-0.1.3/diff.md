# Comparing `tmp/moss_decoder-0.1.2.tar.gz` & `tmp/moss_decoder-0.1.3.tar.gz`

## Comparing `moss_decoder-0.1.2.tar` & `moss_decoder-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,17 @@
--rw-r--r--   0        0        0      634 1970-01-01 00:00:00.000000 moss_decoder-0.1.2/Cargo.toml
--rw-r--r--   0        0        0     2835 2023-07-21 12:06:59.000000 moss_decoder-0.1.2/.github/workflows/CI.yml
--rw-r--r--   0        0        0      757 2023-07-21 07:38:32.000000 moss_decoder-0.1.2/.gitignore
--rw-r--r--   0        0        0      243 2023-07-21 07:45:09.000000 moss_decoder-0.1.2/README.md
--rw-r--r--   0        0        0  9582576 2023-07-21 12:28:16.000000 moss_decoder-0.1.2/moss_noise.raw
--rw-r--r--   0        0        0      388 2023-07-21 06:30:24.000000 moss_decoder-0.1.2/pyproject.toml
--rw-r--r--   0        0        0  4458776 2023-04-08 05:33:25.000000 moss_decoder-0.1.2/python310.dll
--rw-r--r--   0        0        0    13621 2023-07-21 13:51:04.000000 moss_decoder-0.1.2/src/lib.rs
--rw-r--r--   0        0        0     3685 2023-07-21 11:50:49.000000 moss_decoder-0.1.2/src/moss_protocol.rs
--rw-r--r--   0        0        0     7427 2023-07-21 13:52:28.000000 moss_decoder-0.1.2/Cargo.lock
--rw-r--r--   0        0        0      768 1970-01-01 00:00:00.000000 moss_decoder-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      962 1970-01-01 00:00:00.000000 moss_decoder-0.1.3/Cargo.toml
+-rw-r--r--   0     1001      123     2835 2023-07-24 12:50:35.000000 moss_decoder-0.1.3/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      713 2023-07-24 12:50:35.000000 moss_decoder-0.1.3/.gitignore
+-rw-r--r--   0     1001      123     1395 2023-07-24 12:50:35.000000 moss_decoder-0.1.3/README.md
+-rw-r--r--   0     1001      123      641 2023-07-24 12:50:35.000000 moss_decoder-0.1.3/pyproject.toml
+-rw-r--r--   0     1001      123  4458776 2023-07-24 12:50:35.000000 moss_decoder-0.1.3/python310.dll
+-rw-r--r--   0     1001      123     4806 2023-07-24 12:50:35.000000 moss_decoder-0.1.3/src/lib.rs
+-rw-r--r--   0     1001      123     1039 2023-07-24 12:50:35.000000 moss_decoder-0.1.3/src/moss_protocol/moss_hit.rs
+-rw-r--r--   0     1001      123     1220 2023-07-24 12:50:35.000000 moss_decoder-0.1.3/src/moss_protocol/moss_packet.rs
+-rw-r--r--   0     1001      123     1536 2023-07-24 12:50:35.000000 moss_decoder-0.1.3/src/moss_protocol.rs
+-rw-r--r--   0     1001      123     2773 2023-07-24 12:50:35.000000 moss_decoder-0.1.3/tests/integration.py
+-rw-r--r--   0     1001      123     4416 2023-07-24 12:50:35.000000 moss_decoder-0.1.3/tests/integration_test.rs
+-rw-r--r--   0     1001      123  9582576 2023-07-24 12:50:35.000000 moss_decoder-0.1.3/tests/moss_noise.raw
+-rwxr-xr-x   0     1001      123      660 2023-07-24 12:50:35.000000 moss_decoder-0.1.3/tests/performance_dev_py.sh
+-rwxr-xr-x   0     1001      123      620 2023-07-24 12:50:35.000000 moss_decoder-0.1.3/tests/performance_prod_py.sh
+-rw-r--r--   0     1001      123     8066 2023-07-24 12:50:35.000000 moss_decoder-0.1.3/Cargo.lock
+-rw-r--r--   0        0        0     1949 1970-01-01 00:00:00.000000 moss_decoder-0.1.3/PKG-INFO
```

### Comparing `moss_decoder-0.1.2/.github/workflows/CI.yml` & `moss_decoder-0.1.3/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.1.2/moss_noise.raw` & `moss_decoder-0.1.3/tests/moss_noise.raw`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.1.2/python310.dll` & `moss_decoder-0.1.3/python310.dll`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.1.2/Cargo.lock` & `moss_decoder-0.1.3/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,20 @@
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
+name = "diff"
+version = "0.1.13"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "56254986775e3233ffa9c4d7d3faaf6d36a2c09d30b20687e9f88bc8bafc16c8"
+
+[[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "libc"
@@ -49,16 +55,17 @@
 checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "moss_decoder"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
+ "pretty_assertions",
  "pyo3",
 ]
 
 [[package]]
 name = "once_cell"
 version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -84,14 +91,24 @@
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-targets",
 ]
 
 [[package]]
+name = "pretty_assertions"
+version = "1.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "af7cee1a6c8a5b9208b3cb1061f10c0cb689087b3d8ce85fb9d2dd7a29b6ba66"
+dependencies = [
+ "diff",
+ "yansi",
+]
+
+[[package]]
 name = "proc-macro2"
 version = "1.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "18fb31db3f9bddb2ea821cde30a9f70117e3f119938b5ee630b7403aa6e2ead9"
 dependencies = [
  "unicode-ident",
 ]
@@ -267,7 +284,13 @@
 checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
+
+[[package]]
+name = "yansi"
+version = "0.5.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "09041cd90cf85f7f8b2df60c646f853b7f535ce68f85244eb6731cf89fa498ec"
```

