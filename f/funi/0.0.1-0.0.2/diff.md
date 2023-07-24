# Comparing `tmp/funi-0.0.1.tar.gz` & `tmp/funi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funi-0.0.1.tar", last modified: Fri Jul 21 15:30:13 2023, max compression
+gzip compressed data, was "funi-0.0.2.tar", last modified: Mon Jul 24 10:36:11 2023, max compression
```

## Comparing `funi-0.0.1.tar` & `funi-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:30:13.364379 funi-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-21 15:30:05.000000 funi-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-21 15:30:13.364379 funi-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-21 15:30:05.000000 funi-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:30:13.364379 funi-0.0.1/funi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-21 15:30:13.000000 funi-0.0.1/funi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-21 15:30:13.000000 funi-0.0.1/funi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 15:30:13.000000 funi-0.0.1/funi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 15:30:13.000000 funi-0.0.1/funi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 15:30:13.000000 funi-0.0.1/funi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-21 15:30:13.000000 funi-0.0.1/funi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-21 15:30:05.000000 funi-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 15:30:13.364379 funi-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-21 15:30:05.000000 funi-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:30:13.364379 funi-0.0.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-21 15:30:05.000000 funi-0.0.1/src/pyfuni.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:30:13.364379 funi-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-21 15:30:05.000000 funi-0.0.1/tests/test_funi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:36:11.842009 funi-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-24 10:36:02.000000 funi-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-24 10:36:11.838009 funi-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-24 10:36:02.000000 funi-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:36:11.838009 funi-0.0.2/funi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-24 10:36:11.000000 funi-0.0.2/funi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-24 10:36:11.000000 funi-0.0.2/funi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 10:36:11.000000 funi-0.0.2/funi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 10:36:11.000000 funi-0.0.2/funi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 10:36:11.000000 funi-0.0.2/funi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-24 10:36:11.000000 funi-0.0.2/funi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-24 10:36:02.000000 funi-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 10:36:11.842009 funi-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-24 10:36:02.000000 funi-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:36:11.838009 funi-0.0.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-24 10:36:02.000000 funi-0.0.2/src/pyfuni.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:36:11.838009 funi-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-07-24 10:36:02.000000 funi-0.0.2/tests/test_funi.py
```

### Comparing `funi-0.0.1/LICENSE` & `funi-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `funi-0.0.1/PKG-INFO` & `funi-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funi
-Version: 0.0.1
+Version: 0.0.2
 Summary: Find unique float arrays
 Home-page: https://github.com/tataratat/funi
 Author: Jaewook Lee
 Author-email: jaewooklee042@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `funi-0.0.1/README.md` & `funi-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `funi-0.0.1/funi.egg-info/PKG-INFO` & `funi-0.0.2/funi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funi
-Version: 0.0.1
+Version: 0.0.2
 Summary: Find unique float arrays
 Home-page: https://github.com/tataratat/funi
 Author: Jaewook Lee
 Author-email: jaewooklee042@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `funi-0.0.1/setup.py` & `funi-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pybind11.setup_helpers import Pybind11Extension, build_ext
 from setuptools import setup
 
 with open("README.md") as f:
     readme = f.read()
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 
 ext_modules = [
     Pybind11Extension(
         "funi",
         ["src/pyfuni.cpp"],
         include_dirs=["src"],
         extra_compile_args=["-O3"],
```

### Comparing `funi-0.0.1/tests/test_funi.py` & `funi-0.0.2/tests/test_funi.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 
 import numpy as np
 
-import funi
+import funi  # isort:skip
 
 
 class FuniTest(unittest.TestCase):
     def setUp(self):
         # stack 100 x 3 arrays 3 times then shuffle
         q = np.random.rand(100, 3)
         self.q = np.vstack((q, q, q))
@@ -19,15 +19,15 @@
         unique_s, ids_s, inv_s = funi.unique_rows(self.q, tol, True, "l")
 
         # mapping check
         assert np.allclose(self.q[ids_s], unique_s)
         assert np.allclose(self.q, unique_s[inv_s])
 
         # sortedness check
-        assert ~np.all(np.diff(ids_s) < 0)
+        assert np.all(np.diff(ids_s) > 0)
 
         # not sorted
         # sorted indices
         unique_ns, ids_ns, inv_ns = funi.unique_rows(self.q, tol, False, "l")
 
         # mapping check
         assert np.allclose(self.q[ids_ns], unique_ns)
@@ -38,20 +38,30 @@
         unique_s, ids_s, inv_s = funi.unique_rows(self.q, tol, True, "a")
 
         # mapping check
         assert np.allclose(self.q[ids_s], unique_s)
         assert np.allclose(self.q, unique_s[inv_s])
 
         # sortedness check
-        assert ~np.all(np.diff(ids_s) < 0)
+        assert np.all(np.diff(ids_s) > 0)
 
         # not sorted
         # sorted indices
         unique_ns, ids_ns, inv_ns = funi.unique_rows(self.q, tol, False, "a")
 
         # mapping check
         assert np.allclose(self.q[ids_ns], unique_ns)
         assert np.allclose(self.q, unique_ns[inv_ns])
 
+    def test_cross_compare(self):
+        # Compare the results against each other
+        tol = 1e-10
+        a_unique_s, a_ids_s, a_inv_s = funi.unique_rows(self.q, tol, True, "a")
+        l_unique_s, l_ids_s, l_inv_s = funi.unique_rows(self.q, tol, True, "l")
+
+        assert np.allclose(a_unique_s, l_unique_s)
+        assert np.all(a_ids_s == l_ids_s)
+        assert np.all(a_inv_s == l_inv_s)
+
 
 if __name__ == "__main__":
     unittest.main()
```

