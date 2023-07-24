# Comparing `tmp/sccd45ra-0.3.tar.gz` & `tmp/sccd45ra-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sccd45ra-0.3.tar", last modified: Tue Jul  4 00:56:06 2023, max compression
+gzip compressed data, was "sccd45ra-0.3.2.tar", last modified: Mon Jul 24 05:11:14 2023, max compression
```

## Comparing `sccd45ra-0.3.tar` & `sccd45ra-0.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 00:56:06.751240 sccd45ra-0.3/
--rw-rw-rw-   0        0        0       53 2023-07-04 00:56:06.751240 sccd45ra-0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-04 00:56:06.740619 sccd45ra-0.3/sccd45ra/
--rw-rw-rw-   0        0        0       38 2023-05-22 18:45:19.000000 sccd45ra-0.3/sccd45ra/__init__.py
--rw-rw-rw-   0        0        0     1038 2023-05-22 19:24:57.000000 sccd45ra-0.3/sccd45ra/cd45ra_infer.py
-drwxrwxrwx   0        0        0        0 2023-07-04 00:56:06.746224 sccd45ra-0.3/sccd45ra/feature/
--rw-rw-rw-   0        0        0   148483 2023-07-04 00:50:28.000000 sccd45ra-0.3/sccd45ra/feature/Supplement Tables.xlsx
-drwxrwxrwx   0        0        0        0 2023-07-04 00:56:06.748223 sccd45ra-0.3/sccd45ra/model/
--rw-rw-rw-   0        0        0  1823659 2023-07-04 00:50:50.000000 sccd45ra-0.3/sccd45ra/model/best_rbf_svm.joblib
-drwxrwxrwx   0        0        0        0 2023-07-04 00:56:06.745255 sccd45ra-0.3/sccd45ra.egg-info/
--rw-rw-rw-   0        0        0       53 2023-07-04 00:56:06.000000 sccd45ra-0.3/sccd45ra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2023-07-04 00:56:06.000000 sccd45ra-0.3/sccd45ra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 00:56:06.000000 sccd45ra-0.3/sccd45ra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2023-07-04 00:56:06.000000 sccd45ra-0.3/sccd45ra.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-04 00:56:06.000000 sccd45ra-0.3/sccd45ra.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 00:56:06.751240 sccd45ra-0.3/setup.cfg
--rw-rw-rw-   0        0        0      312 2023-07-04 00:55:46.000000 sccd45ra-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 05:11:14.440656 sccd45ra-0.3.2/
+-rw-rw-rw-   0        0        0       55 2023-07-24 05:11:14.439658 sccd45ra-0.3.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-24 05:11:14.429711 sccd45ra-0.3.2/sccd45ra/
+-rw-rw-rw-   0        0        0       38 2023-05-22 18:45:19.000000 sccd45ra-0.3.2/sccd45ra/__init__.py
+-rw-rw-rw-   0        0        0     1038 2023-05-22 19:24:57.000000 sccd45ra-0.3.2/sccd45ra/cd45ra_infer.py
+drwxrwxrwx   0        0        0        0 2023-07-24 05:11:14.434695 sccd45ra-0.3.2/sccd45ra/feature/
+-rw-rw-rw-   0        0        0   148483 2023-07-04 00:50:28.000000 sccd45ra-0.3.2/sccd45ra/feature/Supplement Tables.xlsx
+drwxrwxrwx   0        0        0        0 2023-07-24 05:11:14.436689 sccd45ra-0.3.2/sccd45ra/model/
+-rw-rw-rw-   0        0        0  1823659 2023-07-04 00:50:50.000000 sccd45ra-0.3.2/sccd45ra/model/best_rbf_svm.joblib
+drwxrwxrwx   0        0        0        0 2023-07-24 05:11:14.433673 sccd45ra-0.3.2/sccd45ra.egg-info/
+-rw-rw-rw-   0        0        0       55 2023-07-24 05:11:14.000000 sccd45ra-0.3.2/sccd45ra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2023-07-24 05:11:14.000000 sccd45ra-0.3.2/sccd45ra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 05:11:14.000000 sccd45ra-0.3.2/sccd45ra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2023-07-24 05:11:14.000000 sccd45ra-0.3.2/sccd45ra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-24 05:11:14.000000 sccd45ra-0.3.2/sccd45ra.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 05:11:14.440656 sccd45ra-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      314 2023-07-24 05:11:01.000000 sccd45ra-0.3.2/setup.py
```

### Comparing `sccd45ra-0.3/sccd45ra/cd45ra_infer.py` & `sccd45ra-0.3.2/sccd45ra/cd45ra_infer.py`

 * *Files identical despite different names*

### Comparing `sccd45ra-0.3/sccd45ra/feature/Supplement Tables.xlsx` & `sccd45ra-0.3.2/sccd45ra/feature/Supplement Tables.xlsx`

 * *Files identical despite different names*

### Comparing `sccd45ra-0.3/sccd45ra/model/best_rbf_svm.joblib` & `sccd45ra-0.3.2/sccd45ra/model/best_rbf_svm.joblib`

 * *Files identical despite different names*

