# Comparing `tmp/google_spreadsheets_exporter-0.2.tar.gz` & `tmp/google_spreadsheets_exporter-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_spreadsheets_exporter-0.2.tar", last modified: Mon Jul 24 14:08:27 2023, max compression
+gzip compressed data, was "google_spreadsheets_exporter-0.3.tar", last modified: Mon Jul 24 15:18:12 2023, max compression
```

## Comparing `google_spreadsheets_exporter-0.2.tar` & `google_spreadsheets_exporter-0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 14:08:27.074205 google_spreadsheets_exporter-0.2/
--rw-rw-rw-   0        0        0       97 2023-07-24 13:56:18.000000 google_spreadsheets_exporter-0.2/MANIFEST.in
--rw-rw-rw-   0        0        0       73 2023-07-24 14:08:27.073204 google_spreadsheets_exporter-0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-24 14:08:27.063206 google_spreadsheets_exporter-0.2/google_spreadsheets_exporter/
--rw-rw-rw-   0        0        0        0 2023-07-23 14:47:50.000000 google_spreadsheets_exporter-0.2/google_spreadsheets_exporter/__init__.py
--rw-rw-rw-   0        0        0      369 2023-07-24 13:45:30.000000 google_spreadsheets_exporter-0.2/google_spreadsheets_exporter/data_handler.py
--rw-rw-rw-   0        0        0     1631 2023-07-24 13:45:30.000000 google_spreadsheets_exporter-0.2/google_spreadsheets_exporter/exporter.py
--rw-rw-rw-   0        0        0      530 2023-07-23 15:45:17.000000 google_spreadsheets_exporter-0.2/google_spreadsheets_exporter/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-24 14:08:27.072207 google_spreadsheets_exporter-0.2/google_spreadsheets_exporter.egg-info/
--rw-rw-rw-   0        0        0       73 2023-07-24 14:08:26.000000 google_spreadsheets_exporter-0.2/google_spreadsheets_exporter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      444 2023-07-24 14:08:27.000000 google_spreadsheets_exporter-0.2/google_spreadsheets_exporter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 14:08:26.000000 google_spreadsheets_exporter-0.2/google_spreadsheets_exporter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-07-24 14:08:26.000000 google_spreadsheets_exporter-0.2/google_spreadsheets_exporter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-07-24 14:08:26.000000 google_spreadsheets_exporter-0.2/google_spreadsheets_exporter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 14:08:27.074205 google_spreadsheets_exporter-0.2/setup.cfg
--rw-rw-rw-   0        0        0      372 2023-07-24 14:01:32.000000 google_spreadsheets_exporter-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 15:18:12.534789 google_spreadsheets_exporter-0.3/
+-rw-rw-rw-   0        0        0       97 2023-07-24 13:56:18.000000 google_spreadsheets_exporter-0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0       73 2023-07-24 15:18:12.534789 google_spreadsheets_exporter-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2796 2023-07-24 15:17:30.000000 google_spreadsheets_exporter-0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 15:18:12.517789 google_spreadsheets_exporter-0.3/google_spreadsheets_exporter/
+-rw-rw-rw-   0        0        0        0 2023-07-23 14:47:50.000000 google_spreadsheets_exporter-0.3/google_spreadsheets_exporter/__init__.py
+-rw-rw-rw-   0        0        0     1390 2023-07-24 15:17:30.000000 google_spreadsheets_exporter-0.3/google_spreadsheets_exporter/exporter.py
+-rw-rw-rw-   0        0        0      530 2023-07-23 15:45:17.000000 google_spreadsheets_exporter-0.3/google_spreadsheets_exporter/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-24 15:18:12.532787 google_spreadsheets_exporter-0.3/google_spreadsheets_exporter.egg-info/
+-rw-rw-rw-   0        0        0       73 2023-07-24 15:18:12.000000 google_spreadsheets_exporter-0.3/google_spreadsheets_exporter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      409 2023-07-24 15:18:12.000000 google_spreadsheets_exporter-0.3/google_spreadsheets_exporter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 15:18:12.000000 google_spreadsheets_exporter-0.3/google_spreadsheets_exporter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-07-24 15:18:12.000000 google_spreadsheets_exporter-0.3/google_spreadsheets_exporter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-07-24 15:18:12.000000 google_spreadsheets_exporter-0.3/google_spreadsheets_exporter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 15:18:12.535793 google_spreadsheets_exporter-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      372 2023-07-24 15:17:59.000000 google_spreadsheets_exporter-0.3/setup.py
```

### Comparing `google_spreadsheets_exporter-0.2/google_spreadsheets_exporter/exporter.py` & `google_spreadsheets_exporter-0.3/google_spreadsheets_exporter/exporter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,35 @@
-import os
-
 from google.oauth2 import service_account
 from googleapiclient.discovery import build
 
-from data_handler import DataHandler
-
 
 def load_credentials(credentials_file_full_path):
     return service_account.Credentials.from_service_account_file(credentials_file_full_path)
 
 
 class Exporter():
     def __init__(self, spreadsheet_id:str, list_name:str, data:list, credentials_file_full_path="credentials.json"):
         super().__init__()
         self.spreadsheet_id = spreadsheet_id
-        self.data = data
         self.list_name = list_name
+        self.data = data
         self.creds_file_path = credentials_file_full_path
-        self.handler = DataHandler()
 
         self.credentials = load_credentials(credentials_file_full_path)
 
-    def export_all_model_data(self):
+    def export(self):
         print("exporting data ..")
         service = build('sheets', 'v4', credentials=self.credentials)
 
         # Spreadsheet ID - Obtain this from the URL of your Google Sheet
         spreadsheet_id = self.spreadsheet_id
 
         # Define the range where you want to insert the data (e.g., 'Sheet1!A1')
         range_name = self.list_name
 
-        # Prepare the data to be written to the Google Sheet
-        # data = self.handler.collect_data_for_spreadsheet(self.data)
-
         # Call the Sheets API to insert the data into the Google Sheet
         result = service.spreadsheets().values().update(
             spreadsheetId=spreadsheet_id,
             range=range_name,
             valueInputOption='RAW',
             body={'values': self.data}
         ).execute()
```

### Comparing `google_spreadsheets_exporter-0.2/google_spreadsheets_exporter/utils.py` & `google_spreadsheets_exporter-0.3/google_spreadsheets_exporter/utils.py`

 * *Files identical despite different names*

