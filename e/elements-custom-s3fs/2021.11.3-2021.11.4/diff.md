# Comparing `tmp/elements-custom-s3fs-2021.11.3.tar.gz` & `tmp/elements-custom-s3fs-2021.11.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elements-custom-s3fs-2021.11.3.tar", last modified: Mon Jul 24 15:11:23 2023, max compression
+gzip compressed data, was "elements-custom-s3fs-2021.11.4.tar", last modified: Mon Jul 24 15:12:24 2023, max compression
```

## Comparing `elements-custom-s3fs-2021.11.3.tar` & `elements-custom-s3fs-2021.11.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-07-24 15:11:23.972797 elements-custom-s3fs-2021.11.3/
--rw-r--r--   0 eugene     (501) staff       (20)     1505 2022-12-23 13:05:34.000000 elements-custom-s3fs-2021.11.3/LICENSE.txt
--rw-r--r--   0 eugene     (501) staff       (20)      225 2022-12-23 13:05:34.000000 elements-custom-s3fs-2021.11.3/MANIFEST.in
--rw-r--r--   0 eugene     (501) staff       (20)     1356 2023-07-24 15:11:23.973080 elements-custom-s3fs-2021.11.3/PKG-INFO
--rw-r--r--   0 eugene     (501) staff       (20)      620 2022-12-23 13:05:34.000000 elements-custom-s3fs-2021.11.3/README.rst
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-07-24 15:11:23.965488 elements-custom-s3fs-2021.11.3/docs/
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-07-24 15:11:23.968427 elements-custom-s3fs-2021.11.3/docs/source/
--rw-r--r--   0 eugene     (501) staff       (20)      860 2022-12-23 13:05:34.000000 elements-custom-s3fs-2021.11.3/docs/source/api.rst
--rw-r--r--   0 eugene     (501) staff       (20)     2667 2023-07-24 15:09:43.000000 elements-custom-s3fs-2021.11.3/docs/source/changelog.rst
--rw-r--r--   0 eugene     (501) staff       (20)     9189 2023-07-24 15:09:43.000000 elements-custom-s3fs-2021.11.3/docs/source/index.rst
--rw-r--r--   0 eugene     (501) staff       (20)      530 2022-12-23 13:05:34.000000 elements-custom-s3fs-2021.11.3/docs/source/install.rst
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-07-24 15:11:23.969494 elements-custom-s3fs-2021.11.3/elements_custom_s3fs.egg-info/
--rw-r--r--   0 eugene     (501) staff       (20)     1356 2023-07-24 15:11:23.000000 elements-custom-s3fs-2021.11.3/elements_custom_s3fs.egg-info/PKG-INFO
--rw-r--r--   0 eugene     (501) staff       (20)      629 2023-07-24 15:11:23.000000 elements-custom-s3fs-2021.11.3/elements_custom_s3fs.egg-info/SOURCES.txt
--rw-r--r--   0 eugene     (501) staff       (20)        1 2023-07-24 15:11:23.000000 elements-custom-s3fs-2021.11.3/elements_custom_s3fs.egg-info/dependency_links.txt
--rw-r--r--   0 eugene     (501) staff       (20)        1 2022-12-23 13:39:18.000000 elements-custom-s3fs-2021.11.3/elements_custom_s3fs.egg-info/not-zip-safe
--rw-r--r--   0 eugene     (501) staff       (20)      120 2023-07-24 15:11:23.000000 elements-custom-s3fs-2021.11.3/elements_custom_s3fs.egg-info/requires.txt
--rw-r--r--   0 eugene     (501) staff       (20)        5 2023-07-24 15:11:23.000000 elements-custom-s3fs-2021.11.3/elements_custom_s3fs.egg-info/top_level.txt
--rw-r--r--   0 eugene     (501) staff       (20)       48 2023-07-24 15:09:57.000000 elements-custom-s3fs-2021.11.3/requirements.txt
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-07-24 15:11:23.974607 elements-custom-s3fs-2021.11.3/s3fs/
--rw-r--r--   0 eugene     (501) staff       (20)      160 2022-12-23 13:05:34.000000 elements-custom-s3fs-2021.11.3/s3fs/__init__.py
--rw-r--r--   0 eugene     (501) staff       (20)      501 2023-07-24 15:11:23.974868 elements-custom-s3fs-2021.11.3/s3fs/_version.py
--rw-r--r--   0 eugene     (501) staff       (20)    72588 2023-07-24 15:09:43.000000 elements-custom-s3fs-2021.11.3/s3fs/core.py
--rw-r--r--   0 eugene     (501) staff       (20)     7712 2023-07-24 15:09:43.000000 elements-custom-s3fs-2021.11.3/s3fs/errors.py
--rw-r--r--   0 eugene     (501) staff       (20)      237 2022-12-23 13:05:34.000000 elements-custom-s3fs-2021.11.3/s3fs/mapping.py
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-07-24 15:11:23.972228 elements-custom-s3fs-2021.11.3/s3fs/tests/
--rw-r--r--   0 eugene     (501) staff       (20)        0 2022-12-23 13:05:34.000000 elements-custom-s3fs-2021.11.3/s3fs/tests/__init__.py
--rw-r--r--   0 eugene     (501) staff       (20)     2859 2022-12-23 13:05:34.000000 elements-custom-s3fs-2021.11.3/s3fs/tests/test_mapping.py
--rw-r--r--   0 eugene     (501) staff       (20)    68408 2023-07-24 15:09:43.000000 elements-custom-s3fs-2021.11.3/s3fs/tests/test_s3fs.py
--rw-r--r--   0 eugene     (501) staff       (20)      370 2022-12-23 13:05:34.000000 elements-custom-s3fs-2021.11.3/s3fs/tests/test_utils.py
--rw-r--r--   0 eugene     (501) staff       (20)     5919 2023-07-24 15:09:43.000000 elements-custom-s3fs-2021.11.3/s3fs/utils.py
--rw-r--r--   0 eugene     (501) staff       (20)     1286 2023-07-24 15:11:23.974221 elements-custom-s3fs-2021.11.3/setup.cfg
--rwxr-xr-x   0 eugene     (501) staff       (20)     1424 2023-07-24 15:11:10.000000 elements-custom-s3fs-2021.11.3/setup.py
--rw-r--r--   0 eugene     (501) staff       (20)    78212 2023-07-24 15:09:43.000000 elements-custom-s3fs-2021.11.3/versioneer.py
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-07-24 15:12:24.360661 elements-custom-s3fs-2021.11.4/
+-rw-r--r--   0 eugene     (501) staff       (20)     1505 2022-12-23 13:05:34.000000 elements-custom-s3fs-2021.11.4/LICENSE.txt
+-rw-r--r--   0 eugene     (501) staff       (20)      225 2022-12-23 13:05:34.000000 elements-custom-s3fs-2021.11.4/MANIFEST.in
+-rw-r--r--   0 eugene     (501) staff       (20)     1356 2023-07-24 15:12:24.360731 elements-custom-s3fs-2021.11.4/PKG-INFO
+-rw-r--r--   0 eugene     (501) staff       (20)      620 2022-12-23 13:05:34.000000 elements-custom-s3fs-2021.11.4/README.rst
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-07-24 15:12:24.354998 elements-custom-s3fs-2021.11.4/docs/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-07-24 15:12:24.357398 elements-custom-s3fs-2021.11.4/docs/source/
+-rw-r--r--   0 eugene     (501) staff       (20)      860 2022-12-23 13:05:34.000000 elements-custom-s3fs-2021.11.4/docs/source/api.rst
+-rw-r--r--   0 eugene     (501) staff       (20)     2667 2023-07-24 15:09:43.000000 elements-custom-s3fs-2021.11.4/docs/source/changelog.rst
+-rw-r--r--   0 eugene     (501) staff       (20)     9189 2023-07-24 15:09:43.000000 elements-custom-s3fs-2021.11.4/docs/source/index.rst
+-rw-r--r--   0 eugene     (501) staff       (20)      530 2022-12-23 13:05:34.000000 elements-custom-s3fs-2021.11.4/docs/source/install.rst
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-07-24 15:12:24.358418 elements-custom-s3fs-2021.11.4/elements_custom_s3fs.egg-info/
+-rw-r--r--   0 eugene     (501) staff       (20)     1356 2023-07-24 15:12:24.000000 elements-custom-s3fs-2021.11.4/elements_custom_s3fs.egg-info/PKG-INFO
+-rw-r--r--   0 eugene     (501) staff       (20)      629 2023-07-24 15:12:24.000000 elements-custom-s3fs-2021.11.4/elements_custom_s3fs.egg-info/SOURCES.txt
+-rw-r--r--   0 eugene     (501) staff       (20)        1 2023-07-24 15:12:24.000000 elements-custom-s3fs-2021.11.4/elements_custom_s3fs.egg-info/dependency_links.txt
+-rw-r--r--   0 eugene     (501) staff       (20)        1 2022-12-23 13:39:18.000000 elements-custom-s3fs-2021.11.4/elements_custom_s3fs.egg-info/not-zip-safe
+-rw-r--r--   0 eugene     (501) staff       (20)      120 2023-07-24 15:12:24.000000 elements-custom-s3fs-2021.11.4/elements_custom_s3fs.egg-info/requires.txt
+-rw-r--r--   0 eugene     (501) staff       (20)        5 2023-07-24 15:12:24.000000 elements-custom-s3fs-2021.11.4/elements_custom_s3fs.egg-info/top_level.txt
+-rw-r--r--   0 eugene     (501) staff       (20)       48 2023-07-24 15:12:14.000000 elements-custom-s3fs-2021.11.4/requirements.txt
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-07-24 15:12:24.361357 elements-custom-s3fs-2021.11.4/s3fs/
+-rw-r--r--   0 eugene     (501) staff       (20)      160 2022-12-23 13:05:34.000000 elements-custom-s3fs-2021.11.4/s3fs/__init__.py
+-rw-r--r--   0 eugene     (501) staff       (20)      501 2023-07-24 15:12:24.361386 elements-custom-s3fs-2021.11.4/s3fs/_version.py
+-rw-r--r--   0 eugene     (501) staff       (20)    72588 2023-07-24 15:09:43.000000 elements-custom-s3fs-2021.11.4/s3fs/core.py
+-rw-r--r--   0 eugene     (501) staff       (20)     7712 2023-07-24 15:09:43.000000 elements-custom-s3fs-2021.11.4/s3fs/errors.py
+-rw-r--r--   0 eugene     (501) staff       (20)      237 2022-12-23 13:05:34.000000 elements-custom-s3fs-2021.11.4/s3fs/mapping.py
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-07-24 15:12:24.360512 elements-custom-s3fs-2021.11.4/s3fs/tests/
+-rw-r--r--   0 eugene     (501) staff       (20)        0 2022-12-23 13:05:34.000000 elements-custom-s3fs-2021.11.4/s3fs/tests/__init__.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2859 2022-12-23 13:05:34.000000 elements-custom-s3fs-2021.11.4/s3fs/tests/test_mapping.py
+-rw-r--r--   0 eugene     (501) staff       (20)    68408 2023-07-24 15:09:43.000000 elements-custom-s3fs-2021.11.4/s3fs/tests/test_s3fs.py
+-rw-r--r--   0 eugene     (501) staff       (20)      370 2022-12-23 13:05:34.000000 elements-custom-s3fs-2021.11.4/s3fs/tests/test_utils.py
+-rw-r--r--   0 eugene     (501) staff       (20)     5919 2023-07-24 15:09:43.000000 elements-custom-s3fs-2021.11.4/s3fs/utils.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1286 2023-07-24 15:12:24.361231 elements-custom-s3fs-2021.11.4/setup.cfg
+-rwxr-xr-x   0 eugene     (501) staff       (20)     1424 2023-07-24 15:11:10.000000 elements-custom-s3fs-2021.11.4/setup.py
+-rw-r--r--   0 eugene     (501) staff       (20)    78212 2023-07-24 15:09:43.000000 elements-custom-s3fs-2021.11.4/versioneer.py
```

### Comparing `elements-custom-s3fs-2021.11.3/LICENSE.txt` & `elements-custom-s3fs-2021.11.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `elements-custom-s3fs-2021.11.3/PKG-INFO` & `elements-custom-s3fs-2021.11.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elements-custom-s3fs
-Version: 2021.11.3
+Version: 2021.11.4
 Summary: Convenient Filesystem interface over S3
 Home-page: http://github.com/fsspec/s3fs/
 Maintainer: Martin Durant
 Maintainer-email: mdurant@continuum.io
 License: BSD
 Keywords: s3,boto
 Classifier: Development Status :: 4 - Beta
```

### Comparing `elements-custom-s3fs-2021.11.3/README.rst` & `elements-custom-s3fs-2021.11.4/README.rst`

 * *Files identical despite different names*

### Comparing `elements-custom-s3fs-2021.11.3/docs/source/api.rst` & `elements-custom-s3fs-2021.11.4/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `elements-custom-s3fs-2021.11.3/docs/source/changelog.rst` & `elements-custom-s3fs-2021.11.4/docs/source/changelog.rst`

 * *Files identical despite different names*

### Comparing `elements-custom-s3fs-2021.11.3/docs/source/index.rst` & `elements-custom-s3fs-2021.11.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `elements-custom-s3fs-2021.11.3/docs/source/install.rst` & `elements-custom-s3fs-2021.11.4/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `elements-custom-s3fs-2021.11.3/elements_custom_s3fs.egg-info/PKG-INFO` & `elements-custom-s3fs-2021.11.4/elements_custom_s3fs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elements-custom-s3fs
-Version: 2021.11.3
+Version: 2021.11.4
 Summary: Convenient Filesystem interface over S3
 Home-page: http://github.com/fsspec/s3fs/
 Maintainer: Martin Durant
 Maintainer-email: mdurant@continuum.io
 License: BSD
 Keywords: s3,boto
 Classifier: Development Status :: 4 - Beta
```

### Comparing `elements-custom-s3fs-2021.11.3/elements_custom_s3fs.egg-info/SOURCES.txt` & `elements-custom-s3fs-2021.11.4/elements_custom_s3fs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elements-custom-s3fs-2021.11.3/s3fs/core.py` & `elements-custom-s3fs-2021.11.4/s3fs/core.py`

 * *Files identical despite different names*

### Comparing `elements-custom-s3fs-2021.11.3/s3fs/errors.py` & `elements-custom-s3fs-2021.11.4/s3fs/errors.py`

 * *Files identical despite different names*

### Comparing `elements-custom-s3fs-2021.11.3/s3fs/tests/test_mapping.py` & `elements-custom-s3fs-2021.11.4/s3fs/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `elements-custom-s3fs-2021.11.3/s3fs/tests/test_s3fs.py` & `elements-custom-s3fs-2021.11.4/s3fs/tests/test_s3fs.py`

 * *Files identical despite different names*

### Comparing `elements-custom-s3fs-2021.11.3/s3fs/utils.py` & `elements-custom-s3fs-2021.11.4/s3fs/utils.py`

 * *Files identical despite different names*

### Comparing `elements-custom-s3fs-2021.11.3/setup.cfg` & `elements-custom-s3fs-2021.11.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `elements-custom-s3fs-2021.11.3/setup.py` & `elements-custom-s3fs-2021.11.4/setup.py`

 * *Files identical despite different names*

### Comparing `elements-custom-s3fs-2021.11.3/versioneer.py` & `elements-custom-s3fs-2021.11.4/versioneer.py`

 * *Files identical despite different names*

