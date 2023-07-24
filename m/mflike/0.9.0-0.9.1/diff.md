# Comparing `tmp/mflike-0.9.0.tar.gz` & `tmp/mflike-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mflike-0.9.0.tar", last modified: Mon Jul 10 12:38:28 2023, max compression
+gzip compressed data, was "mflike-0.9.1.tar", last modified: Mon Jul 24 11:23:29 2023, max compression
```

## Comparing `mflike-0.9.0.tar` & `mflike-0.9.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:38:28.271775 mflike-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-10 12:38:24.000000 mflike-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-10 12:38:24.000000 mflike-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-07-10 12:38:28.271775 mflike-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-10 12:38:24.000000 mflike-0.9.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:38:28.271775 mflike-0.9.0/mflike/
--rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-07-10 12:38:24.000000 mflike-0.9.0/mflike/MFLike.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-10 12:38:24.000000 mflike-0.9.0/mflike/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-10 12:38:28.271775 mflike-0.9.0/mflike/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13748 2023-07-10 12:38:24.000000 mflike-0.9.0/mflike/mflike.py
--rw-r--r--   0 runner    (1001) docker     (123)    18736 2023-07-10 12:38:24.000000 mflike-0.9.0/mflike/theoryforge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:38:28.271775 mflike-0.9.0/mflike.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-07-10 12:38:28.000000 mflike-0.9.0/mflike.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-10 12:38:28.000000 mflike-0.9.0/mflike.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 12:38:28.000000 mflike-0.9.0/mflike.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-10 12:38:28.000000 mflike-0.9.0/mflike.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 12:38:28.000000 mflike-0.9.0/mflike.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 12:38:28.000000 mflike-0.9.0/mflike.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-10 12:38:28.271775 mflike-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-10 12:38:24.000000 mflike-0.9.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-07-10 12:38:24.000000 mflike-0.9.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:23:29.442476 mflike-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-24 11:23:23.000000 mflike-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-24 11:23:23.000000 mflike-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-07-24 11:23:29.442476 mflike-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-24 11:23:23.000000 mflike-0.9.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:23:29.442476 mflike-0.9.1/mflike/
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-07-24 11:23:23.000000 mflike-0.9.1/mflike/MFLike.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-24 11:23:23.000000 mflike-0.9.1/mflike/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-24 11:23:29.442476 mflike-0.9.1/mflike/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13748 2023-07-24 11:23:23.000000 mflike-0.9.1/mflike/mflike.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18736 2023-07-24 11:23:23.000000 mflike-0.9.1/mflike/theoryforge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:23:29.442476 mflike-0.9.1/mflike.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-07-24 11:23:29.000000 mflike-0.9.1/mflike.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-24 11:23:29.000000 mflike-0.9.1/mflike.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 11:23:29.000000 mflike-0.9.1/mflike.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-24 11:23:29.000000 mflike-0.9.1/mflike.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 11:23:29.000000 mflike-0.9.1/mflike.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 11:23:29.000000 mflike-0.9.1/mflike.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-24 11:23:29.442476 mflike-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-24 11:23:23.000000 mflike-0.9.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-07-24 11:23:23.000000 mflike-0.9.1/versioneer.py
```

### Comparing `mflike-0.9.0/LICENSE` & `mflike-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mflike-0.9.0/PKG-INFO` & `mflike-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: mflike
-Version: 0.9.0
+Version: 0.9.1
 Summary: SO LAT multi-frequency likelihood for cobaya
 Home-page: https://github.com/simonsobs/LAT_MFLike
 Author: Simons Observatory Collaboration Power Spectrum Group aka so_ps 1 & 2
 License: BSD license
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.5
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 =============================
 LAT Multifrequency Likelihood
 =============================
```

### Comparing `mflike-0.9.0/README.rst` & `mflike-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `mflike-0.9.0/mflike/MFLike.yaml` & `mflike-0.9.1/mflike/MFLike.yaml`

 * *Files identical despite different names*

### Comparing `mflike-0.9.0/mflike/mflike.py` & `mflike-0.9.1/mflike/mflike.py`

 * *Files identical despite different names*

### Comparing `mflike-0.9.0/mflike/theoryforge.py` & `mflike-0.9.1/mflike/theoryforge.py`

 * *Files identical despite different names*

### Comparing `mflike-0.9.0/mflike.egg-info/PKG-INFO` & `mflike-0.9.1/mflike.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: mflike
-Version: 0.9.0
+Version: 0.9.1
 Summary: SO LAT multi-frequency likelihood for cobaya
 Home-page: https://github.com/simonsobs/LAT_MFLike
 Author: Simons Observatory Collaboration Power Spectrum Group aka so_ps 1 & 2
 License: BSD license
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.5
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 =============================
 LAT Multifrequency Likelihood
 =============================
```

### Comparing `mflike-0.9.0/setup.py` & `mflike-0.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,26 +13,26 @@
     url="https://github.com/simonsobs/LAT_MFLike",
     description="SO LAT multi-frequency likelihood for cobaya",
     long_description=readme,
     long_description_content_type="text/x-rst",
     license="BSD license",
     zip_safe=True,
     packages=find_packages(),
-    python_requires=">=3.5",
+    python_requires=">=3.8",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
     install_requires=[
         "fgspectra>=1.1.0",
         "syslibrary>=0.1.0",
-        "cobaya>=3.1.0",
-        "sacc>=0.4.2",
+        "cobaya>=3.3.0",
+        "sacc>=0.9.0",
     ],
     package_data={"mflike": ["MFLike.yaml"]},
 )
```

### Comparing `mflike-0.9.0/versioneer.py` & `mflike-0.9.1/versioneer.py`

 * *Files identical despite different names*

