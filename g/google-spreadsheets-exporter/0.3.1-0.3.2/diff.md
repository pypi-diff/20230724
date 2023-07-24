# Comparing `tmp/google_spreadsheets_exporter-0.3.1.tar.gz` & `tmp/google_spreadsheets_exporter-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_spreadsheets_exporter-0.3.1.tar", last modified: Mon Jul 24 15:21:25 2023, max compression
+gzip compressed data, was "google_spreadsheets_exporter-0.3.2.tar", last modified: Mon Jul 24 15:25:55 2023, max compression
```

## Comparing `google_spreadsheets_exporter-0.3.1.tar` & `google_spreadsheets_exporter-0.3.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 15:21:25.980757 google_spreadsheets_exporter-0.3.1/
--rw-rw-rw-   0        0        0       97 2023-07-24 13:56:18.000000 google_spreadsheets_exporter-0.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2916 2023-07-24 15:21:25.980757 google_spreadsheets_exporter-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     2796 2023-07-24 15:17:30.000000 google_spreadsheets_exporter-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-24 15:21:25.962759 google_spreadsheets_exporter-0.3.1/google_spreadsheets_exporter/
--rw-rw-rw-   0        0        0        0 2023-07-23 14:47:50.000000 google_spreadsheets_exporter-0.3.1/google_spreadsheets_exporter/__init__.py
--rw-rw-rw-   0        0        0     1390 2023-07-24 15:17:30.000000 google_spreadsheets_exporter-0.3.1/google_spreadsheets_exporter/exporter.py
--rw-rw-rw-   0        0        0      530 2023-07-23 15:45:17.000000 google_spreadsheets_exporter-0.3.1/google_spreadsheets_exporter/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-24 15:21:25.979756 google_spreadsheets_exporter-0.3.1/google_spreadsheets_exporter.egg-info/
--rw-rw-rw-   0        0        0     2916 2023-07-24 15:21:25.000000 google_spreadsheets_exporter-0.3.1/google_spreadsheets_exporter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      409 2023-07-24 15:21:25.000000 google_spreadsheets_exporter-0.3.1/google_spreadsheets_exporter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 15:21:25.000000 google_spreadsheets_exporter-0.3.1/google_spreadsheets_exporter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-07-24 15:21:25.000000 google_spreadsheets_exporter-0.3.1/google_spreadsheets_exporter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-07-24 15:21:25.000000 google_spreadsheets_exporter-0.3.1/google_spreadsheets_exporter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 15:21:25.981757 google_spreadsheets_exporter-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      555 2023-07-24 15:21:14.000000 google_spreadsheets_exporter-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 15:25:55.454884 google_spreadsheets_exporter-0.3.2/
+-rw-rw-rw-   0        0        0       97 2023-07-24 13:56:18.000000 google_spreadsheets_exporter-0.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2954 2023-07-24 15:25:55.453884 google_spreadsheets_exporter-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2834 2023-07-24 15:24:47.000000 google_spreadsheets_exporter-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 15:25:55.436893 google_spreadsheets_exporter-0.3.2/google_spreadsheets_exporter/
+-rw-rw-rw-   0        0        0        0 2023-07-23 14:47:50.000000 google_spreadsheets_exporter-0.3.2/google_spreadsheets_exporter/__init__.py
+-rw-rw-rw-   0        0        0     1390 2023-07-24 15:17:30.000000 google_spreadsheets_exporter-0.3.2/google_spreadsheets_exporter/exporter.py
+-rw-rw-rw-   0        0        0      530 2023-07-23 15:45:17.000000 google_spreadsheets_exporter-0.3.2/google_spreadsheets_exporter/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-24 15:25:55.452889 google_spreadsheets_exporter-0.3.2/google_spreadsheets_exporter.egg-info/
+-rw-rw-rw-   0        0        0     2954 2023-07-24 15:25:55.000000 google_spreadsheets_exporter-0.3.2/google_spreadsheets_exporter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      409 2023-07-24 15:25:55.000000 google_spreadsheets_exporter-0.3.2/google_spreadsheets_exporter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 15:25:55.000000 google_spreadsheets_exporter-0.3.2/google_spreadsheets_exporter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-07-24 15:25:55.000000 google_spreadsheets_exporter-0.3.2/google_spreadsheets_exporter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-07-24 15:25:55.000000 google_spreadsheets_exporter-0.3.2/google_spreadsheets_exporter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 15:25:55.454884 google_spreadsheets_exporter-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      555 2023-07-24 15:25:53.000000 google_spreadsheets_exporter-0.3.2/setup.py
```

### Comparing `google_spreadsheets_exporter-0.3.1/PKG-INFO` & `google_spreadsheets_exporter-0.3.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: google_spreadsheets_exporter
-Version: 0.3.1
+Version: 0.3.2
 Description-Content-Type: text/markdown
 
 # Description
 
 This Library lets you export 2D array of data into your Google Spreadsheet.
 
 - In short;
 
     - Before
     <br>
     <br>
-  ![](https://i.imgur.com/fU64iks.png)
+  ![Empty SpreadSheet](https://i.imgur.com/fU64iks.png)
       <br>
       <br>
     - After export of `[["Name"],["David"]]`
     <br>
     <br>
-  ![](https://i.imgur.com/341Kbkl.png)
+  ![SpreadSheet with data](https://i.imgur.com/341Kbkl.png)
 
 The following code snippet will export "Name" and "David" into your Google Spreadsheet,
 assuming you are all set up on the Google Cloud side.
 
 If this is not the case, continue to the section 'Complete Guide'
 
 ## Quickstart:
```

### Comparing `google_spreadsheets_exporter-0.3.1/README.md` & `google_spreadsheets_exporter-0.3.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 This Library lets you export 2D array of data into your Google Spreadsheet.
 
 - In short;
 
     - Before
     <br>
     <br>
-  ![](https://i.imgur.com/fU64iks.png)
+  ![Empty SpreadSheet](https://i.imgur.com/fU64iks.png)
       <br>
       <br>
     - After export of `[["Name"],["David"]]`
     <br>
     <br>
-  ![](https://i.imgur.com/341Kbkl.png)
+  ![SpreadSheet with data](https://i.imgur.com/341Kbkl.png)
 
 The following code snippet will export "Name" and "David" into your Google Spreadsheet,
 assuming you are all set up on the Google Cloud side.
 
 If this is not the case, continue to the section 'Complete Guide'
 
 ## Quickstart:
```

### Comparing `google_spreadsheets_exporter-0.3.1/google_spreadsheets_exporter/exporter.py` & `google_spreadsheets_exporter-0.3.2/google_spreadsheets_exporter/exporter.py`

 * *Files identical despite different names*

### Comparing `google_spreadsheets_exporter-0.3.1/google_spreadsheets_exporter/utils.py` & `google_spreadsheets_exporter-0.3.2/google_spreadsheets_exporter/utils.py`

 * *Files identical despite different names*

### Comparing `google_spreadsheets_exporter-0.3.1/google_spreadsheets_exporter.egg-info/PKG-INFO` & `google_spreadsheets_exporter-0.3.2/google_spreadsheets_exporter.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: google-spreadsheets-exporter
-Version: 0.3.1
+Version: 0.3.2
 Description-Content-Type: text/markdown
 
 # Description
 
 This Library lets you export 2D array of data into your Google Spreadsheet.
 
 - In short;
 
     - Before
     <br>
     <br>
-  ![](https://i.imgur.com/fU64iks.png)
+  ![Empty SpreadSheet](https://i.imgur.com/fU64iks.png)
       <br>
       <br>
     - After export of `[["Name"],["David"]]`
     <br>
     <br>
-  ![](https://i.imgur.com/341Kbkl.png)
+  ![SpreadSheet with data](https://i.imgur.com/341Kbkl.png)
 
 The following code snippet will export "Name" and "David" into your Google Spreadsheet,
 assuming you are all set up on the Google Cloud side.
 
 If this is not the case, continue to the section 'Complete Guide'
 
 ## Quickstart:
```

### Comparing `google_spreadsheets_exporter-0.3.1/setup.py` & `google_spreadsheets_exporter-0.3.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='google_spreadsheets_exporter',
-    version='0.3.1',
+    version='0.3.2',
     packages=['google_spreadsheets_exporter'],
     install_requires=[
         'google-api-python-client',
         'google-auth-httplib2',
         'google-auth-oauthlib',
     ],
     exclude_package_data={'google_spreadsheets_exporter': ['creds.json', 'test.py']},
```

