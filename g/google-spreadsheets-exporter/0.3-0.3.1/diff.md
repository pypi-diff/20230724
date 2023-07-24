# Comparing `tmp/google_spreadsheets_exporter-0.3.tar.gz` & `tmp/google_spreadsheets_exporter-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_spreadsheets_exporter-0.3.tar", last modified: Mon Jul 24 15:18:12 2023, max compression
+gzip compressed data, was "google_spreadsheets_exporter-0.3.1.tar", last modified: Mon Jul 24 15:21:25 2023, max compression
```

## Comparing `google_spreadsheets_exporter-0.3.tar` & `google_spreadsheets_exporter-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 15:18:12.534789 google_spreadsheets_exporter-0.3/
--rw-rw-rw-   0        0        0       97 2023-07-24 13:56:18.000000 google_spreadsheets_exporter-0.3/MANIFEST.in
--rw-rw-rw-   0        0        0       73 2023-07-24 15:18:12.534789 google_spreadsheets_exporter-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2796 2023-07-24 15:17:30.000000 google_spreadsheets_exporter-0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-24 15:18:12.517789 google_spreadsheets_exporter-0.3/google_spreadsheets_exporter/
--rw-rw-rw-   0        0        0        0 2023-07-23 14:47:50.000000 google_spreadsheets_exporter-0.3/google_spreadsheets_exporter/__init__.py
--rw-rw-rw-   0        0        0     1390 2023-07-24 15:17:30.000000 google_spreadsheets_exporter-0.3/google_spreadsheets_exporter/exporter.py
--rw-rw-rw-   0        0        0      530 2023-07-23 15:45:17.000000 google_spreadsheets_exporter-0.3/google_spreadsheets_exporter/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-24 15:18:12.532787 google_spreadsheets_exporter-0.3/google_spreadsheets_exporter.egg-info/
--rw-rw-rw-   0        0        0       73 2023-07-24 15:18:12.000000 google_spreadsheets_exporter-0.3/google_spreadsheets_exporter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      409 2023-07-24 15:18:12.000000 google_spreadsheets_exporter-0.3/google_spreadsheets_exporter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 15:18:12.000000 google_spreadsheets_exporter-0.3/google_spreadsheets_exporter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-07-24 15:18:12.000000 google_spreadsheets_exporter-0.3/google_spreadsheets_exporter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-07-24 15:18:12.000000 google_spreadsheets_exporter-0.3/google_spreadsheets_exporter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 15:18:12.535793 google_spreadsheets_exporter-0.3/setup.cfg
--rw-rw-rw-   0        0        0      372 2023-07-24 15:17:59.000000 google_spreadsheets_exporter-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 15:21:25.980757 google_spreadsheets_exporter-0.3.1/
+-rw-rw-rw-   0        0        0       97 2023-07-24 13:56:18.000000 google_spreadsheets_exporter-0.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2916 2023-07-24 15:21:25.980757 google_spreadsheets_exporter-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2796 2023-07-24 15:17:30.000000 google_spreadsheets_exporter-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 15:21:25.962759 google_spreadsheets_exporter-0.3.1/google_spreadsheets_exporter/
+-rw-rw-rw-   0        0        0        0 2023-07-23 14:47:50.000000 google_spreadsheets_exporter-0.3.1/google_spreadsheets_exporter/__init__.py
+-rw-rw-rw-   0        0        0     1390 2023-07-24 15:17:30.000000 google_spreadsheets_exporter-0.3.1/google_spreadsheets_exporter/exporter.py
+-rw-rw-rw-   0        0        0      530 2023-07-23 15:45:17.000000 google_spreadsheets_exporter-0.3.1/google_spreadsheets_exporter/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-24 15:21:25.979756 google_spreadsheets_exporter-0.3.1/google_spreadsheets_exporter.egg-info/
+-rw-rw-rw-   0        0        0     2916 2023-07-24 15:21:25.000000 google_spreadsheets_exporter-0.3.1/google_spreadsheets_exporter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      409 2023-07-24 15:21:25.000000 google_spreadsheets_exporter-0.3.1/google_spreadsheets_exporter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 15:21:25.000000 google_spreadsheets_exporter-0.3.1/google_spreadsheets_exporter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-07-24 15:21:25.000000 google_spreadsheets_exporter-0.3.1/google_spreadsheets_exporter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-07-24 15:21:25.000000 google_spreadsheets_exporter-0.3.1/google_spreadsheets_exporter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 15:21:25.981757 google_spreadsheets_exporter-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      555 2023-07-24 15:21:14.000000 google_spreadsheets_exporter-0.3.1/setup.py
```

### Comparing `google_spreadsheets_exporter-0.3/README.md` & `google_spreadsheets_exporter-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `google_spreadsheets_exporter-0.3/google_spreadsheets_exporter/exporter.py` & `google_spreadsheets_exporter-0.3.1/google_spreadsheets_exporter/exporter.py`

 * *Files identical despite different names*

### Comparing `google_spreadsheets_exporter-0.3/google_spreadsheets_exporter/utils.py` & `google_spreadsheets_exporter-0.3.1/google_spreadsheets_exporter/utils.py`

 * *Files identical despite different names*

