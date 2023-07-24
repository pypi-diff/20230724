# Comparing `tmp/google_spreadsheets_exporter-1.0.2.tar.gz` & `tmp/google_spreadsheets_exporter-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_spreadsheets_exporter-1.0.2.tar", last modified: Mon Jul 24 17:28:43 2023, max compression
+gzip compressed data, was "google_spreadsheets_exporter-1.0.4.tar", last modified: Mon Jul 24 17:34:23 2023, max compression
```

## Comparing `google_spreadsheets_exporter-1.0.2.tar` & `google_spreadsheets_exporter-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:28:43.165510 google_spreadsheets_exporter-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-24 17:28:34.000000 google_spreadsheets_exporter-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-24 17:28:34.000000 google_spreadsheets_exporter-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-07-24 17:28:43.165510 google_spreadsheets_exporter-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-07-24 17:28:34.000000 google_spreadsheets_exporter-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:28:43.165510 google_spreadsheets_exporter-1.0.2/google_spreadsheets_exporter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:28:34.000000 google_spreadsheets_exporter-1.0.2/google_spreadsheets_exporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-24 17:28:34.000000 google_spreadsheets_exporter-1.0.2/google_spreadsheets_exporter/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-24 17:28:34.000000 google_spreadsheets_exporter-1.0.2/google_spreadsheets_exporter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:28:43.165510 google_spreadsheets_exporter-1.0.2/google_spreadsheets_exporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-07-24 17:28:43.000000 google_spreadsheets_exporter-1.0.2/google_spreadsheets_exporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-24 17:28:43.000000 google_spreadsheets_exporter-1.0.2/google_spreadsheets_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 17:28:43.000000 google_spreadsheets_exporter-1.0.2/google_spreadsheets_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-24 17:28:43.000000 google_spreadsheets_exporter-1.0.2/google_spreadsheets_exporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-24 17:28:43.000000 google_spreadsheets_exporter-1.0.2/google_spreadsheets_exporter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 17:28:43.165510 google_spreadsheets_exporter-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-24 17:28:34.000000 google_spreadsheets_exporter-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:23.646800 google_spreadsheets_exporter-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-24 17:34:12.000000 google_spreadsheets_exporter-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-24 17:34:12.000000 google_spreadsheets_exporter-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-07-24 17:34:23.646800 google_spreadsheets_exporter-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-07-24 17:34:12.000000 google_spreadsheets_exporter-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:23.646800 google_spreadsheets_exporter-1.0.4/google_spreadsheets_exporter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:12.000000 google_spreadsheets_exporter-1.0.4/google_spreadsheets_exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-24 17:34:12.000000 google_spreadsheets_exporter-1.0.4/google_spreadsheets_exporter/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-24 17:34:12.000000 google_spreadsheets_exporter-1.0.4/google_spreadsheets_exporter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:23.646800 google_spreadsheets_exporter-1.0.4/google_spreadsheets_exporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-07-24 17:34:23.000000 google_spreadsheets_exporter-1.0.4/google_spreadsheets_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-24 17:34:23.000000 google_spreadsheets_exporter-1.0.4/google_spreadsheets_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 17:34:23.000000 google_spreadsheets_exporter-1.0.4/google_spreadsheets_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-24 17:34:23.000000 google_spreadsheets_exporter-1.0.4/google_spreadsheets_exporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-24 17:34:23.000000 google_spreadsheets_exporter-1.0.4/google_spreadsheets_exporter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 17:34:23.646800 google_spreadsheets_exporter-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-24 17:34:12.000000 google_spreadsheets_exporter-1.0.4/setup.py
```

### Comparing `google_spreadsheets_exporter-1.0.2/LICENSE` & `google_spreadsheets_exporter-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `google_spreadsheets_exporter-1.0.2/PKG-INFO` & `google_spreadsheets_exporter-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google_spreadsheets_exporter
-Version: 1.0.2
+Version: 1.0.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Description
 
 This library lets you export 2D arrays of data into your Google Spreadsheet.
```

### Comparing `google_spreadsheets_exporter-1.0.2/README.md` & `google_spreadsheets_exporter-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `google_spreadsheets_exporter-1.0.2/google_spreadsheets_exporter/exporter.py` & `google_spreadsheets_exporter-1.0.4/google_spreadsheets_exporter/exporter.py`

 * *Files identical despite different names*

### Comparing `google_spreadsheets_exporter-1.0.2/google_spreadsheets_exporter/utils.py` & `google_spreadsheets_exporter-1.0.4/google_spreadsheets_exporter/utils.py`

 * *Files identical despite different names*

### Comparing `google_spreadsheets_exporter-1.0.2/google_spreadsheets_exporter.egg-info/PKG-INFO` & `google_spreadsheets_exporter-1.0.4/google_spreadsheets_exporter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-spreadsheets-exporter
-Version: 1.0.2
+Version: 1.0.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Description
 
 This library lets you export 2D arrays of data into your Google Spreadsheet.
```

### Comparing `google_spreadsheets_exporter-1.0.2/setup.py` & `google_spreadsheets_exporter-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='google_spreadsheets_exporter',
-    version='1.0.2',
+    version='1.0.4',
     packages=['google_spreadsheets_exporter'],
     install_requires=[
         'google-api-python-client',
         'google-auth-httplib2',
         'google-auth-oauthlib',
     ],
     exclude_package_data={'google_spreadsheets_exporter': ['creds.json', 'test.py']},
```

