# Comparing `tmp/geometrout-0.1.0.7.tar.gz` & `tmp/geometrout-0.1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geometrout-0.1.0.7.tar", last modified: Wed May  3 23:35:31 2023, max compression
+gzip compressed data, was "geometrout-0.1.0.8.tar", last modified: Mon Jul 24 21:44:46 2023, max compression
```

## Comparing `geometrout-0.1.0.7.tar` & `geometrout-0.1.0.8.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:35:31.698936 geometrout-0.1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-03 23:35:21.000000 geometrout-0.1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-03 23:35:31.698936 geometrout-0.1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-03 23:35:21.000000 geometrout-0.1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:35:31.698936 geometrout-0.1.0.7/geometrout/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-03 23:35:21.000000 geometrout-0.1.0.7/geometrout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-03 23:35:21.000000 geometrout-0.1.0.7/geometrout/pointcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    21396 2023-05-03 23:35:21.000000 geometrout-0.1.0.7/geometrout/primitive.py
--rw-r--r--   0 runner    (1001) docker     (123)    10592 2023-05-03 23:35:21.000000 geometrout-0.1.0.7/geometrout/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-03 23:35:21.000000 geometrout-0.1.0.7/geometrout/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:35:31.698936 geometrout-0.1.0.7/geometrout.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-03 23:35:31.000000 geometrout-0.1.0.7/geometrout.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-03 23:35:31.000000 geometrout-0.1.0.7/geometrout.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 23:35:31.000000 geometrout-0.1.0.7/geometrout.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-03 23:35:31.000000 geometrout-0.1.0.7/geometrout.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-03 23:35:31.000000 geometrout-0.1.0.7/geometrout.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-03 23:35:21.000000 geometrout-0.1.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-03 23:35:31.698936 geometrout-0.1.0.7/setup.cfg
+drwxrwxr-x   0 fishy     (1000) fishy     (1000)        0 2023-07-24 21:44:46.422310 geometrout-0.1.0.8/
+-rw-rw-r--   0 fishy     (1000) fishy     (1000)     2327 2023-04-14 18:48:20.000000 geometrout-0.1.0.8/LICENSE
+-rw-rw-r--   0 fishy     (1000) fishy     (1000)      578 2023-07-24 21:44:46.422310 geometrout-0.1.0.8/PKG-INFO
+-rw-rw-r--   0 fishy     (1000) fishy     (1000)       85 2023-04-14 18:48:20.000000 geometrout-0.1.0.8/README.md
+drwxrwxr-x   0 fishy     (1000) fishy     (1000)        0 2023-07-24 21:44:46.422310 geometrout-0.1.0.8/geometrout/
+-rw-rw-r--   0 fishy     (1000) fishy     (1000)      100 2023-04-14 18:48:20.000000 geometrout-0.1.0.8/geometrout/__init__.py
+-rw-rw-r--   0 fishy     (1000) fishy     (1000)     1853 2023-04-14 18:48:20.000000 geometrout-0.1.0.8/geometrout/pointcloud.py
+-rw-rw-r--   0 fishy     (1000) fishy     (1000)    21396 2023-07-24 21:44:09.000000 geometrout-0.1.0.8/geometrout/primitive.py
+-rw-rw-r--   0 fishy     (1000) fishy     (1000)    10732 2023-07-24 21:44:09.000000 geometrout-0.1.0.8/geometrout/transform.py
+-rw-rw-r--   0 fishy     (1000) fishy     (1000)     1338 2023-07-24 21:44:09.000000 geometrout-0.1.0.8/geometrout/utils.py
+drwxrwxr-x   0 fishy     (1000) fishy     (1000)        0 2023-07-24 21:44:46.422310 geometrout-0.1.0.8/geometrout.egg-info/
+-rw-rw-r--   0 fishy     (1000) fishy     (1000)      578 2023-07-24 21:44:46.000000 geometrout-0.1.0.8/geometrout.egg-info/PKG-INFO
+-rw-rw-r--   0 fishy     (1000) fishy     (1000)      351 2023-07-24 21:44:46.000000 geometrout-0.1.0.8/geometrout.egg-info/SOURCES.txt
+-rw-rw-r--   0 fishy     (1000) fishy     (1000)        1 2023-07-24 21:44:46.000000 geometrout-0.1.0.8/geometrout.egg-info/dependency_links.txt
+-rw-rw-r--   0 fishy     (1000) fishy     (1000)       20 2023-07-24 21:44:46.000000 geometrout-0.1.0.8/geometrout.egg-info/requires.txt
+-rw-rw-r--   0 fishy     (1000) fishy     (1000)       11 2023-07-24 21:44:46.000000 geometrout-0.1.0.8/geometrout.egg-info/top_level.txt
+-rw-rw-r--   0 fishy     (1000) fishy     (1000)       90 2023-04-14 18:48:20.000000 geometrout-0.1.0.8/pyproject.toml
+-rw-rw-r--   0 fishy     (1000) fishy     (1000)      689 2023-07-24 21:44:46.422310 geometrout-0.1.0.8/setup.cfg
+drwxrwxr-x   0 fishy     (1000) fishy     (1000)        0 2023-07-24 21:44:46.422310 geometrout-0.1.0.8/tests/
+-rw-rw-r--   0 fishy     (1000) fishy     (1000)     1293 2023-07-24 21:44:09.000000 geometrout-0.1.0.8/tests/test_transform.py
```

### Comparing `geometrout-0.1.0.7/LICENSE` & `geometrout-0.1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `geometrout-0.1.0.7/PKG-INFO` & `geometrout-0.1.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geometrout
-Version: 0.1.0.7
+Version: 0.1.0.8
 Summary: A collection of geometric methods and concepts tailored to machine learning for robotics
-Download-URL: https://github.com/fishbotics/geometrout/archive/refs/tags/v0.1.0.7.tar.gz
+Download-URL: https://github.com/fishbotics/geometrout/archive/refs/tags/v0.1.0.8.tar.gz
 License: MIT
 Requires-Python: >=3.6
 License-File: LICENSE
 
 This is a high-performance set of tools used for CPU-based geometric processing in Python. By-in-large, these are simple methods, written with Numpy and Numba. These tools were designed for Machine Learning and Robotics, but could feasibly be used for any 3D processing task.
```

### Comparing `geometrout-0.1.0.7/geometrout/pointcloud.py` & `geometrout-0.1.0.8/geometrout/pointcloud.py`

 * *Files identical despite different names*

### Comparing `geometrout-0.1.0.7/geometrout/primitive.py` & `geometrout-0.1.0.8/geometrout/primitive.py`

 * *Files identical despite different names*

### Comparing `geometrout-0.1.0.7/geometrout/transform.py` & `geometrout-0.1.0.8/geometrout/transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -309,14 +309,21 @@
         """
         Allows for numpy-style matrix multiplication using `@`
         """
         pos, q = _pose_multiply(self.pos, self.so3.q, other.pos, other.so3.q)
         return SE3(pos, q)
 
     @property
+    def quaternion(self):
+        """
+        Returns the underlying quaternion object
+        """
+        return self.so3.q
+
+    @property
     def inverse(self):
         """
         :return: The inverse transformation
         """
         pos, q = _pose_inverse(self.pos, self.so3.q)
         return SE3(pos, q)
```

### Comparing `geometrout-0.1.0.7/geometrout/utils.py` & `geometrout-0.1.0.8/geometrout/utils.py`

 * *Files identical despite different names*

### Comparing `geometrout-0.1.0.7/geometrout.egg-info/PKG-INFO` & `geometrout-0.1.0.8/geometrout.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geometrout
-Version: 0.1.0.7
+Version: 0.1.0.8
 Summary: A collection of geometric methods and concepts tailored to machine learning for robotics
-Download-URL: https://github.com/fishbotics/geometrout/archive/refs/tags/v0.1.0.7.tar.gz
+Download-URL: https://github.com/fishbotics/geometrout/archive/refs/tags/v0.1.0.8.tar.gz
 License: MIT
 Requires-Python: >=3.6
 License-File: LICENSE
 
 This is a high-performance set of tools used for CPU-based geometric processing in Python. By-in-large, these are simple methods, written with Numpy and Numba. These tools were designed for Machine Learning and Robotics, but could feasibly be used for any 3D processing task.
```

### Comparing `geometrout-0.1.0.7/setup.cfg` & `geometrout-0.1.0.8/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = geometrout
-version = 0.1.0.7
+version = 0.1.0.8
 description = A collection of geometric methods and concepts tailored to machine learning for robotics
 long_description = This is a high-performance set of tools used for CPU-based geometric processing in Python. By-in-large, these are simple methods, written with Numpy and Numba. These tools were designed for Machine Learning and Robotics, but could feasibly be used for any 3D processing task.
 license = MIT
-download_url = https://github.com/fishbotics/geometrout/archive/refs/tags/v0.1.0.7.tar.gz
+download_url = https://github.com/fishbotics/geometrout/archive/refs/tags/v0.1.0.8.tar.gz
 
 [options]
 packages = geometrout
 python_requires = >=3.6
 install_requires = 
 	numpy
 	numba >= 0.56.4
```

