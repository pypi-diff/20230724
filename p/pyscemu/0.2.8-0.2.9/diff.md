# Comparing `tmp/pyscemu-0.2.8.tar.gz` & `tmp/pyscemu-0.2.9.tar.gz`

## Comparing `pyscemu-0.2.8.tar` & `pyscemu-0.2.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      309 1970-01-01 00:00:00.000000 pyscemu-0.2.8/Cargo.toml
--rw-r--r--   0     1000     1000     2809 2023-04-28 16:18:25.000000 pyscemu-0.2.8/.github/workflows/CI.yml
--rw-r--r--   0     1000     1000      692 2023-04-29 18:18:29.000000 pyscemu-0.2.8/.gitignore
--rw-r--r--   0     1000     1000    11773 2023-07-03 19:42:43.000000 pyscemu-0.2.8/DOCUMENTATION.md
--rw-r--r--   0     1000     1000    10083 2023-05-09 16:58:06.000000 pyscemu-0.2.8/README.md
--rw-r--r--   0     1000     1000     2017 2023-04-30 22:51:14.000000 pyscemu-0.2.8/examples/danabot_rsa.ipynb
--rw-r--r--   0     1000     1000     6831 2023-04-30 22:52:26.000000 pyscemu-0.2.8/examples/raccoon_strings.ipynb
--rw-r--r--   0     1000     1000        0 2023-04-30 16:12:18.000000 pyscemu-0.2.8/examples/scripts/.ipynb_checkpoints/test-checkpoint.py
--rw-r--r--   0     1000     1000      727 2023-04-30 13:08:15.000000 pyscemu-0.2.8/examples/scripts/raccoon_strings.py
--rw-r--r--   0     1000     1000      766 2023-05-09 15:35:14.000000 pyscemu-0.2.8/examples/scripts/test.py
--rw-r--r--   0     1000     1000      561 2023-04-29 17:52:46.000000 pyscemu-0.2.8/examples/scripts/xloader_dexor.py
--rw-r--r--   0     1000     1000      427 2023-05-10 08:13:44.000000 pyscemu-0.2.8/examples/scripts/xloader_keygen.py
--rw-r--r--   0     1000     1000     1757 2023-04-30 15:03:12.000000 pyscemu-0.2.8/examples/xloader_keygen.ipynb
--rw-r--r--   0     1000     1000      433 2023-05-01 11:01:29.000000 pyscemu-0.2.8/pyproject.toml
--rw-r--r--   0     1000     1000    26776 2023-07-03 19:39:30.000000 pyscemu-0.2.8/src/lib.rs
--rw-r--r--   0     1000     1000    33592 2023-07-23 22:11:59.000000 pyscemu-0.2.8/Cargo.lock
--rw-r--r--   0        0        0    10409 1970-01-01 00:00:00.000000 pyscemu-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      309 1970-01-01 00:00:00.000000 pyscemu-0.2.9/Cargo.toml
+-rw-r--r--   0     1000     1000     2809 2023-04-28 16:18:25.000000 pyscemu-0.2.9/.github/workflows/CI.yml
+-rw-r--r--   0     1000     1000      692 2023-04-29 18:18:29.000000 pyscemu-0.2.9/.gitignore
+-rw-r--r--   0     1000     1000    11773 2023-07-03 19:42:43.000000 pyscemu-0.2.9/DOCUMENTATION.md
+-rw-r--r--   0     1000     1000    10083 2023-05-09 16:58:06.000000 pyscemu-0.2.9/README.md
+-rw-r--r--   0     1000     1000     2017 2023-04-30 22:51:14.000000 pyscemu-0.2.9/examples/danabot_rsa.ipynb
+-rw-r--r--   0     1000     1000     6831 2023-04-30 22:52:26.000000 pyscemu-0.2.9/examples/raccoon_strings.ipynb
+-rw-r--r--   0     1000     1000        0 2023-04-30 16:12:18.000000 pyscemu-0.2.9/examples/scripts/.ipynb_checkpoints/test-checkpoint.py
+-rw-r--r--   0     1000     1000      727 2023-04-30 13:08:15.000000 pyscemu-0.2.9/examples/scripts/raccoon_strings.py
+-rw-r--r--   0     1000     1000      766 2023-05-09 15:35:14.000000 pyscemu-0.2.9/examples/scripts/test.py
+-rw-r--r--   0     1000     1000      561 2023-04-29 17:52:46.000000 pyscemu-0.2.9/examples/scripts/xloader_dexor.py
+-rw-r--r--   0     1000     1000      427 2023-05-10 08:13:44.000000 pyscemu-0.2.9/examples/scripts/xloader_keygen.py
+-rw-r--r--   0     1000     1000     1757 2023-04-30 15:03:12.000000 pyscemu-0.2.9/examples/xloader_keygen.ipynb
+-rw-r--r--   0     1000     1000      433 2023-05-01 11:01:29.000000 pyscemu-0.2.9/pyproject.toml
+-rw-r--r--   0     1000     1000    26776 2023-07-03 19:39:30.000000 pyscemu-0.2.9/src/lib.rs
+-rw-r--r--   0     1000     1000    33592 2023-07-24 08:45:42.000000 pyscemu-0.2.9/Cargo.lock
+-rw-r--r--   0        0        0    10409 1970-01-01 00:00:00.000000 pyscemu-0.2.9/PKG-INFO
```

### Comparing `pyscemu-0.2.8/.github/workflows/CI.yml` & `pyscemu-0.2.9/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.8/.gitignore` & `pyscemu-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.8/DOCUMENTATION.md` & `pyscemu-0.2.9/DOCUMENTATION.md`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.8/README.md` & `pyscemu-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.8/examples/danabot_rsa.ipynb` & `pyscemu-0.2.9/examples/danabot_rsa.ipynb`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.8/examples/raccoon_strings.ipynb` & `pyscemu-0.2.9/examples/raccoon_strings.ipynb`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.8/examples/scripts/raccoon_strings.py` & `pyscemu-0.2.9/examples/scripts/raccoon_strings.py`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.8/examples/scripts/test.py` & `pyscemu-0.2.9/examples/scripts/test.py`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.8/examples/scripts/xloader_dexor.py` & `pyscemu-0.2.9/examples/scripts/xloader_dexor.py`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.8/examples/xloader_keygen.ipynb` & `pyscemu-0.2.9/examples/xloader_keygen.ipynb`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.8/src/lib.rs` & `pyscemu-0.2.9/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.8/Cargo.lock` & `pyscemu-0.2.9/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -412,17 +412,17 @@
 name = "libc"
 version = "0.2.142"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
 
 [[package]]
 name = "libscemu"
-version = "0.12.8"
+version = "0.12.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7725cdb02c968c1b386fe28095a29f52d6024e874f56161c94b55ef7f2d49f37"
+checksum = "64040c208a7778cf2216ef85114f32ad0afabe80eb82914ff6c3a0eb420d0bfd"
 dependencies = [
  "attohttpc",
  "atty",
  "chrono",
  "ctrlc",
  "iced-x86",
  "lazy_static",
@@ -703,15 +703,15 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyscemu"
-version = "0.2.8"
+version = "0.2.9"
 dependencies = [
  "libscemu",
  "pyo3",
 ]
 
 [[package]]
 name = "quote"
```

### Comparing `pyscemu-0.2.8/PKG-INFO` & `pyscemu-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscemu
-Version: 0.2.8
+Version: 0.2.9
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # PYSCEMU
```

