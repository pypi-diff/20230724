# Comparing `tmp/nvidia-dali-nightly-cuda110-1.29.0.dev20230721.tar.gz` & `tmp/nvidia-dali-nightly-cuda110-1.29.0.dev20230724.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvidia-dali-nightly-cuda110-1.29.0.dev20230721.tar", last modified: Fri Jul 21 14:05:08 2023, max compression
+gzip compressed data, was "nvidia-dali-nightly-cuda110-1.29.0.dev20230724.tar", last modified: Mon Jul 24 12:04:43 2023, max compression
```

## Comparing `nvidia-dali-nightly-cuda110-1.29.0.dev20230721.tar` & `nvidia-dali-nightly-cuda110-1.29.0.dev20230724.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-21 14:05:08.396661 nvidia-dali-nightly-cuda110-1.29.0.dev20230721/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      459 2023-07-21 14:05:08.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230721/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-07-06 05:01:19.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230721/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       27 2023-07-21 14:05:08.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230721/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-07-21 14:05:08.396661 nvidia-dali-nightly-cuda110-1.29.0.dev20230721/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      286 2023-07-21 14:05:08.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230721/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-21 14:05:08.396661 nvidia-dali-nightly-cuda110-1.29.0.dev20230721/nvidia_dali_nightly_cuda110.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-07-21 14:05:08.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230721/nvidia_dali_nightly_cuda110.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      257 2023-07-21 14:05:08.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230721/nvidia_dali_nightly_cuda110.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-07-21 14:05:08.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230721/nvidia_dali_nightly_cuda110.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-07-21 14:05:08.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230721/nvidia_dali_nightly_cuda110.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-07-21 14:05:08.396661 nvidia-dali-nightly-cuda110-1.29.0.dev20230721/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-07-06 05:01:19.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230721/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-24 12:04:43.688830 nvidia-dali-nightly-cuda110-1.29.0.dev20230724/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      459 2023-07-24 12:04:43.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230724/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-07-06 05:01:19.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230724/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       27 2023-07-24 12:04:43.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230724/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-07-24 12:04:43.688830 nvidia-dali-nightly-cuda110-1.29.0.dev20230724/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      286 2023-07-24 12:04:43.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230724/README.rst
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-24 12:04:43.684830 nvidia-dali-nightly-cuda110-1.29.0.dev20230724/nvidia_dali_nightly_cuda110.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-07-24 12:04:43.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230724/nvidia_dali_nightly_cuda110.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      257 2023-07-24 12:04:43.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230724/nvidia_dali_nightly_cuda110.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-07-24 12:04:43.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230724/nvidia_dali_nightly_cuda110.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-07-24 12:04:43.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230724/nvidia_dali_nightly_cuda110.egg-info/top_level.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-07-24 12:04:43.688830 nvidia-dali-nightly-cuda110-1.29.0.dev20230724/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-07-06 05:01:19.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230724/setup.py
```

### Comparing `nvidia-dali-nightly-cuda110-1.29.0.dev20230721/LICENSE.md` & `nvidia-dali-nightly-cuda110-1.29.0.dev20230724/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nvidia-dali-nightly-cuda110-1.29.0.dev20230721/PKG-INFO` & `nvidia-dali-nightly-cuda110-1.29.0.dev20230724/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-nightly-cuda110
-Version: 1.29.0.dev20230721
+Version: 1.29.0.dev20230724
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `nvidia-dali-nightly-cuda110-1.29.0.dev20230721/nvidia_dali_nightly_cuda110.egg-info/PKG-INFO` & `nvidia-dali-nightly-cuda110-1.29.0.dev20230724/nvidia_dali_nightly_cuda110.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-nightly-cuda110
-Version: 1.29.0.dev20230721
+Version: 1.29.0.dev20230724
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `nvidia-dali-nightly-cuda110-1.29.0.dev20230721/setup.py` & `nvidia-dali-nightly-cuda110-1.29.0.dev20230724/setup.py`

 * *Files identical despite different names*

