# Comparing `tmp/google_spreadsheets_exporter-0.3.3.tar.gz` & `tmp/google_spreadsheets_exporter-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_spreadsheets_exporter-0.3.3.tar", last modified: Mon Jul 24 15:29:00 2023, max compression
+gzip compressed data, was "google_spreadsheets_exporter-0.3.4.tar", last modified: Mon Jul 24 15:34:15 2023, max compression
```

## Comparing `google_spreadsheets_exporter-0.3.3.tar` & `google_spreadsheets_exporter-0.3.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 15:29:00.433239 google_spreadsheets_exporter-0.3.3/
--rw-rw-rw-   0        0        0       97 2023-07-24 13:56:18.000000 google_spreadsheets_exporter-0.3.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2912 2023-07-24 15:29:00.432237 google_spreadsheets_exporter-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     2792 2023-07-24 15:28:57.000000 google_spreadsheets_exporter-0.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-24 15:29:00.413236 google_spreadsheets_exporter-0.3.3/google_spreadsheets_exporter/
--rw-rw-rw-   0        0        0        0 2023-07-23 14:47:50.000000 google_spreadsheets_exporter-0.3.3/google_spreadsheets_exporter/__init__.py
--rw-rw-rw-   0        0        0     1390 2023-07-24 15:17:30.000000 google_spreadsheets_exporter-0.3.3/google_spreadsheets_exporter/exporter.py
--rw-rw-rw-   0        0        0      530 2023-07-23 15:45:17.000000 google_spreadsheets_exporter-0.3.3/google_spreadsheets_exporter/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-24 15:29:00.431239 google_spreadsheets_exporter-0.3.3/google_spreadsheets_exporter.egg-info/
--rw-rw-rw-   0        0        0     2912 2023-07-24 15:29:00.000000 google_spreadsheets_exporter-0.3.3/google_spreadsheets_exporter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      409 2023-07-24 15:29:00.000000 google_spreadsheets_exporter-0.3.3/google_spreadsheets_exporter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 15:29:00.000000 google_spreadsheets_exporter-0.3.3/google_spreadsheets_exporter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-07-24 15:29:00.000000 google_spreadsheets_exporter-0.3.3/google_spreadsheets_exporter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-07-24 15:29:00.000000 google_spreadsheets_exporter-0.3.3/google_spreadsheets_exporter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 15:29:00.433239 google_spreadsheets_exporter-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0      555 2023-07-24 15:28:57.000000 google_spreadsheets_exporter-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 15:34:15.681620 google_spreadsheets_exporter-0.3.4/
+-rw-rw-rw-   0        0        0       97 2023-07-24 13:56:18.000000 google_spreadsheets_exporter-0.3.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2696 2023-07-24 15:34:15.680622 google_spreadsheets_exporter-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2576 2023-07-24 15:34:13.000000 google_spreadsheets_exporter-0.3.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 15:34:15.662621 google_spreadsheets_exporter-0.3.4/google_spreadsheets_exporter/
+-rw-rw-rw-   0        0        0        0 2023-07-23 14:47:50.000000 google_spreadsheets_exporter-0.3.4/google_spreadsheets_exporter/__init__.py
+-rw-rw-rw-   0        0        0     1390 2023-07-24 15:17:30.000000 google_spreadsheets_exporter-0.3.4/google_spreadsheets_exporter/exporter.py
+-rw-rw-rw-   0        0        0      530 2023-07-23 15:45:17.000000 google_spreadsheets_exporter-0.3.4/google_spreadsheets_exporter/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-24 15:34:15.679619 google_spreadsheets_exporter-0.3.4/google_spreadsheets_exporter.egg-info/
+-rw-rw-rw-   0        0        0     2696 2023-07-24 15:34:15.000000 google_spreadsheets_exporter-0.3.4/google_spreadsheets_exporter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      409 2023-07-24 15:34:15.000000 google_spreadsheets_exporter-0.3.4/google_spreadsheets_exporter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 15:34:15.000000 google_spreadsheets_exporter-0.3.4/google_spreadsheets_exporter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-07-24 15:34:15.000000 google_spreadsheets_exporter-0.3.4/google_spreadsheets_exporter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-07-24 15:34:15.000000 google_spreadsheets_exporter-0.3.4/google_spreadsheets_exporter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 15:34:15.681620 google_spreadsheets_exporter-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      555 2023-07-24 15:34:13.000000 google_spreadsheets_exporter-0.3.4/setup.py
```

### Comparing `google_spreadsheets_exporter-0.3.3/PKG-INFO` & `google_spreadsheets_exporter-0.3.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,10 @@
-Metadata-Version: 2.1
-Name: google_spreadsheets_exporter
-Version: 0.3.3
-Description-Content-Type: text/markdown
-
 # Description
 
-This Library lets you export 2D array of data into your Google Spreadsheet.
-
-In short;
-
-- Before
-<br>
-<br>
-![Empty SpreadSheet](https://i.imgur.com/fU64iks.png)
-<br>
-<br>
-- After export of `[["Name"],["David"]]`
-<br>
-<br>
-![SpreadSheet with data](https://i.imgur.com/341Kbkl.png)
+This library lets you export 2D arrays of data into your Google Spreadsheet.
 
 The following code snippet will export "Name" and "David" into your Google Spreadsheet,
 assuming you are all set up on the Google Cloud side.
 
 If this is not the case, continue to the section 'Complete Guide'
 
 ## Quickstart:
@@ -73,8 +55,8 @@
         
       exp = Exporter("spreadsheet-id", "sheet-name", data, credentials_file_full_path=os.path.join(BASE_DIR, "creds.json"))
       exp.export()
 
     where `spreadsheet-id` and `sheet-name` has been extracted from Spreadsheet url, `data` is 2D python array and
     `credentials_file_full_path` is full path to your credentials file.
 
-Happy exporting.
+Happy exporting.
```

### Comparing `google_spreadsheets_exporter-0.3.3/README.md` & `google_spreadsheets_exporter-0.3.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,15 @@
-# Description
-
-This Library lets you export 2D array of data into your Google Spreadsheet.
+Metadata-Version: 2.1
+Name: google_spreadsheets_exporter
+Version: 0.3.4
+Description-Content-Type: text/markdown
 
-In short;
+# Description
 
-- Before
-<br>
-<br>
-![Empty SpreadSheet](https://i.imgur.com/fU64iks.png)
-<br>
-<br>
-- After export of `[["Name"],["David"]]`
-<br>
-<br>
-![SpreadSheet with data](https://i.imgur.com/341Kbkl.png)
+This library lets you export 2D arrays of data into your Google Spreadsheet.
 
 The following code snippet will export "Name" and "David" into your Google Spreadsheet,
 assuming you are all set up on the Google Cloud side.
 
 If this is not the case, continue to the section 'Complete Guide'
 
 ## Quickstart:
@@ -68,8 +60,8 @@
         
       exp = Exporter("spreadsheet-id", "sheet-name", data, credentials_file_full_path=os.path.join(BASE_DIR, "creds.json"))
       exp.export()
 
     where `spreadsheet-id` and `sheet-name` has been extracted from Spreadsheet url, `data` is 2D python array and
     `credentials_file_full_path` is full path to your credentials file.
 
-Happy exporting.
+Happy exporting.
```

### Comparing `google_spreadsheets_exporter-0.3.3/google_spreadsheets_exporter/exporter.py` & `google_spreadsheets_exporter-0.3.4/google_spreadsheets_exporter/exporter.py`

 * *Files identical despite different names*

### Comparing `google_spreadsheets_exporter-0.3.3/google_spreadsheets_exporter/utils.py` & `google_spreadsheets_exporter-0.3.4/google_spreadsheets_exporter/utils.py`

 * *Files identical despite different names*

### Comparing `google_spreadsheets_exporter-0.3.3/google_spreadsheets_exporter.egg-info/PKG-INFO` & `google_spreadsheets_exporter-0.3.4/google_spreadsheets_exporter.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,15 @@
 Metadata-Version: 2.1
 Name: google-spreadsheets-exporter
-Version: 0.3.3
+Version: 0.3.4
 Description-Content-Type: text/markdown
 
 # Description
 
-This Library lets you export 2D array of data into your Google Spreadsheet.
-
-In short;
-
-- Before
-<br>
-<br>
-![Empty SpreadSheet](https://i.imgur.com/fU64iks.png)
-<br>
-<br>
-- After export of `[["Name"],["David"]]`
-<br>
-<br>
-![SpreadSheet with data](https://i.imgur.com/341Kbkl.png)
+This library lets you export 2D arrays of data into your Google Spreadsheet.
 
 The following code snippet will export "Name" and "David" into your Google Spreadsheet,
 assuming you are all set up on the Google Cloud side.
 
 If this is not the case, continue to the section 'Complete Guide'
 
 ## Quickstart:
```

### Comparing `google_spreadsheets_exporter-0.3.3/setup.py` & `google_spreadsheets_exporter-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='google_spreadsheets_exporter',
-    version='0.3.3',
+    version='0.3.4',
     packages=['google_spreadsheets_exporter'],
     install_requires=[
         'google-api-python-client',
         'google-auth-httplib2',
         'google-auth-oauthlib',
     ],
     exclude_package_data={'google_spreadsheets_exporter': ['creds.json', 'test.py']},
```

