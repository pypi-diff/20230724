# Comparing `tmp/google_spreadsheets_exporter-1.0.0.tar.gz` & `tmp/google_spreadsheets_exporter-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_spreadsheets_exporter-1.0.0.tar", last modified: Mon Jul 24 16:10:35 2023, max compression
+gzip compressed data, was "google_spreadsheets_exporter-1.0.2.tar", last modified: Mon Jul 24 17:28:43 2023, max compression
```

## Comparing `google_spreadsheets_exporter-1.0.0.tar` & `google_spreadsheets_exporter-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 16:10:35.549233 google_spreadsheets_exporter-1.0.0/
--rw-rw-rw-   0        0        0       97 2023-07-24 13:56:18.000000 google_spreadsheets_exporter-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4188 2023-07-24 16:10:35.548234 google_spreadsheets_exporter-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4068 2023-07-24 16:09:59.000000 google_spreadsheets_exporter-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-24 16:10:35.526232 google_spreadsheets_exporter-1.0.0/google_spreadsheets_exporter/
--rw-rw-rw-   0        0        0        0 2023-07-23 14:47:50.000000 google_spreadsheets_exporter-1.0.0/google_spreadsheets_exporter/__init__.py
--rw-rw-rw-   0        0        0     2043 2023-07-24 16:00:39.000000 google_spreadsheets_exporter-1.0.0/google_spreadsheets_exporter/exporter.py
--rw-rw-rw-   0        0        0      530 2023-07-23 15:45:17.000000 google_spreadsheets_exporter-1.0.0/google_spreadsheets_exporter/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-24 16:10:35.546234 google_spreadsheets_exporter-1.0.0/google_spreadsheets_exporter.egg-info/
--rw-rw-rw-   0        0        0     4188 2023-07-24 16:10:35.000000 google_spreadsheets_exporter-1.0.0/google_spreadsheets_exporter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      409 2023-07-24 16:10:35.000000 google_spreadsheets_exporter-1.0.0/google_spreadsheets_exporter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 16:10:35.000000 google_spreadsheets_exporter-1.0.0/google_spreadsheets_exporter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-07-24 16:10:35.000000 google_spreadsheets_exporter-1.0.0/google_spreadsheets_exporter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-07-24 16:10:35.000000 google_spreadsheets_exporter-1.0.0/google_spreadsheets_exporter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 16:10:35.549233 google_spreadsheets_exporter-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      555 2023-07-24 16:10:18.000000 google_spreadsheets_exporter-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:28:43.165510 google_spreadsheets_exporter-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-24 17:28:34.000000 google_spreadsheets_exporter-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-24 17:28:34.000000 google_spreadsheets_exporter-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-07-24 17:28:43.165510 google_spreadsheets_exporter-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-07-24 17:28:34.000000 google_spreadsheets_exporter-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:28:43.165510 google_spreadsheets_exporter-1.0.2/google_spreadsheets_exporter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:28:34.000000 google_spreadsheets_exporter-1.0.2/google_spreadsheets_exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-24 17:28:34.000000 google_spreadsheets_exporter-1.0.2/google_spreadsheets_exporter/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-24 17:28:34.000000 google_spreadsheets_exporter-1.0.2/google_spreadsheets_exporter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:28:43.165510 google_spreadsheets_exporter-1.0.2/google_spreadsheets_exporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-07-24 17:28:43.000000 google_spreadsheets_exporter-1.0.2/google_spreadsheets_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-24 17:28:43.000000 google_spreadsheets_exporter-1.0.2/google_spreadsheets_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 17:28:43.000000 google_spreadsheets_exporter-1.0.2/google_spreadsheets_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-24 17:28:43.000000 google_spreadsheets_exporter-1.0.2/google_spreadsheets_exporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-24 17:28:43.000000 google_spreadsheets_exporter-1.0.2/google_spreadsheets_exporter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 17:28:43.165510 google_spreadsheets_exporter-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-24 17:28:34.000000 google_spreadsheets_exporter-1.0.2/setup.py
```

### Comparing `google_spreadsheets_exporter-1.0.0/PKG-INFO` & `google_spreadsheets_exporter-1.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,97 +1,98 @@
-Metadata-Version: 2.1
-Name: google_spreadsheets_exporter
-Version: 1.0.0
-Description-Content-Type: text/markdown
-
-# Description
-
-This library lets you export 2D arrays of data into your Google Spreadsheet.
-
-The following code snippet will export "Name" and "David" into your Google Spreadsheet,
-assuming you are all set up on the Google Cloud side.
-
-If this is not the case, continue to the section 'Complete Guide'
-
-## Quickstart:
-
-Install the library by running
-`pip install google-spreadsheets-exporter`
-
-Include the following code snippet for desired functionality
-
-      from pathlib import Path
-      from google_spreadsheets_exporter.exporter import Exporter
-        
-      BASE_DIR = Path(__file__).resolve() # adjust path to your credentials file filder as needed
-      data = [["Name"],["David"]]
-        
-      exp = Exporter("spreadsheet-id", "sheet-name", data, credentials_file_full_path=os.path.join(BASE_DIR, "creds.json"))
-      exp.export()
-
-## Complete Guide
-
-- Step 1: Set up a Google Sheets API Project
-
-    - Go to the Google Developers Console (https://console.developers.google.com/) and create a new project.
-      - A user for this project has to be created. Note its email.
-    - Enable the Google Sheets API for your project.
-    - Create credentials for your project to access the API. For this purpose, you'll need a service account key, which is a JSON file containing authentication information.
-      - Alternatively you can provide all credentials in a dictionary. For more on this - refer to the "Authenticating with dictionary of credentials" seciton.
-    - The credentials JSON file should be downloaded and included in your project.
-
-
-- Step 2: 
-    - Create a Google sheet from your account
-    - Note down Spreadsheet ID
-      - eg https[]()://docs.google.com/spreadsheets/d/<font color="green">*spreadsheetId-sdvs-dsv*</font>/edit#gid=0/
-    - Share the Spreadsheet with the email of your newly created Google project user.
-  
-
-- Step 3: Include this code snippet in you project
-    - Install the library by running
-      `pip install google-spreadsheets-exporter`
-        
-      Include the following code snippet for desired functionality
-        ````
-      from pathlib import Path
-      from google_spreadsheets_exporter.exporter import Exporter
-        
-      BASE_DIR = Path(__file__).resolve() # adjust path to your credentials file filder as needed
-      data = [["Name"],["David"]]
-        
-      exp = Exporter("spreadsheet-id", "sheet-name", data, credentials_file_full_path=os.path.join(BASE_DIR, "creds.json"))
-      exp.export()
-
-    where `spreadsheet-id` and `sheet-name` has been extracted from Spreadsheet url, `data` is 2D python array and
-    `credentials_file_full_path` is full path to your credentials file.
-
-
-### Authenticating with dictionary of credentials
-
-- You will need to assemble the dictionary of credentials that will match the JSON credentials file.
-    
-Sample dictionary:
-````
-credentials_info = {
-    "type": "service_account",
-    "project_id": "your-project-id",
-    "private_key_id": "your-private-key-id",
-    "private_key": "-----BEGIN PRIVATE KEY-----\n...\n-----END PRIVATE KEY-----\n",
-    "client_email": "your-service-account-email@your-project-id.iam.gserviceaccount.com",
-    "client_id": "your-client-id",
-    "auth_uri": "https://accounts.google.com/o/oauth2/auth",
-    "token_uri": "https://accounts.google.com/o/oauth2/token",
-    "auth_provider_x509_cert_url": "https://www.googleapis.com/oauth2/v1/certs",
-    "client_x509_cert_url": "https://www.googleapis.com/robot/v1/metadata/x509/your-service-account-email%40your-project-id.iam.gserviceaccount.com"
-}
-````
-
-- *Usecase*: Assumed use-case is that the JSON credentials file is downloaded from Google Cloud project
-  and for some reason is disassembled and is put back together at runtime. 
-
-- Once you assemble the dictionary of credentials, you will initialize the Exporter class like so:
-
-    `exp = Exporter("spreadsheet-id", "sheet-name", data, using_credentials_file=False, credentials_dictionary=my_assembled_dict))`
-
-
-Happy exporting.
+Metadata-Version: 2.1
+Name: google_spreadsheets_exporter
+Version: 1.0.2
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Description
+
+This library lets you export 2D arrays of data into your Google Spreadsheet.
+
+The following code snippet will export "Name" and "David" into your Google Spreadsheet,
+assuming you are all set up on the Google Cloud side.
+
+If this is not the case, continue to the section 'Complete Guide'
+
+## Quickstart:
+
+Install the library by running
+`pip install google-spreadsheets-exporter`
+
+Include the following code snippet for desired functionality
+
+      from pathlib import Path
+      from google_spreadsheets_exporter.exporter import Exporter
+        
+      BASE_DIR = Path(__file__).resolve() # adjust path to your credentials file filder as needed
+      data = [["Name"],["David"]]
+        
+      exp = Exporter("spreadsheet-id", "sheet-name", data, credentials_file_full_path=os.path.join(BASE_DIR, "creds.json"))
+      exp.export()
+
+## Complete Guide
+
+- Step 1: Set up a Google Sheets API Project
+
+    - Go to the Google Developers Console (https://console.developers.google.com/) and create a new project.
+      - A user for this project has to be created. Note its email.
+    - Enable the Google Sheets API for your project.
+    - Create credentials for your project to access the API. For this purpose, you'll need a service account key, which is a JSON file containing authentication information.
+      - Alternatively you can provide all credentials in a dictionary. For more on this - refer to the "Authenticating with dictionary of credentials" seciton.
+    - The credentials JSON file should be downloaded and included in your project.
+
+
+- Step 2: 
+    - Create a Google sheet from your account
+    - Note down Spreadsheet ID
+      - eg https[]()://docs.google.com/spreadsheets/d/<font color="green">*spreadsheetId-sdvs-dsv*</font>/edit#gid=0/
+    - Share the Spreadsheet with the email of your newly created Google project user.
+  
+
+- Step 3: Include this code snippet in you project
+    - Install the library by running
+      `pip install google-spreadsheets-exporter`
+        
+      Include the following code snippet for desired functionality
+        ````
+      from pathlib import Path
+      from google_spreadsheets_exporter.exporter import Exporter
+        
+      BASE_DIR = Path(__file__).resolve() # adjust path to your credentials file filder as needed
+      data = [["Name"],["David"]]
+        
+      exp = Exporter("spreadsheet-id", "sheet-name", data, credentials_file_full_path=os.path.join(BASE_DIR, "creds.json"))
+      exp.export()
+
+    where `spreadsheet-id` and `sheet-name` has been extracted from Spreadsheet url, `data` is 2D python array and
+    `credentials_file_full_path` is full path to your credentials file.
+
+
+### Authenticating with dictionary of credentials
+
+- You will need to assemble the dictionary of credentials that will match the JSON credentials file.
+    
+Sample dictionary:
+````
+credentials_info = {
+    "type": "service_account",
+    "project_id": "your-project-id",
+    "private_key_id": "your-private-key-id",
+    "private_key": "-----BEGIN PRIVATE KEY-----\n...\n-----END PRIVATE KEY-----\n",
+    "client_email": "your-service-account-email@your-project-id.iam.gserviceaccount.com",
+    "client_id": "your-client-id",
+    "auth_uri": "https://accounts.google.com/o/oauth2/auth",
+    "token_uri": "https://accounts.google.com/o/oauth2/token",
+    "auth_provider_x509_cert_url": "https://www.googleapis.com/oauth2/v1/certs",
+    "client_x509_cert_url": "https://www.googleapis.com/robot/v1/metadata/x509/your-service-account-email%40your-project-id.iam.gserviceaccount.com"
+}
+````
+
+- *Usecase*: Assumed use-case is that the JSON credentials file is downloaded from Google Cloud project
+  and for some reason is disassembled and is put back together at runtime. 
+
+- Once you assemble the dictionary of credentials, you will initialize the Exporter class like so:
+
+    `exp = Exporter("spreadsheet-id", "sheet-name", data, using_credentials_file=False, credentials_dictionary=my_assembled_dict))`
+
+
+Happy exporting.
```

### Comparing `google_spreadsheets_exporter-1.0.0/README.md` & `google_spreadsheets_exporter-1.0.2/google_spreadsheets_exporter.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,92 +1,98 @@
-# Description
-
-This library lets you export 2D arrays of data into your Google Spreadsheet.
-
-The following code snippet will export "Name" and "David" into your Google Spreadsheet,
-assuming you are all set up on the Google Cloud side.
-
-If this is not the case, continue to the section 'Complete Guide'
-
-## Quickstart:
-
-Install the library by running
-`pip install google-spreadsheets-exporter`
-
-Include the following code snippet for desired functionality
-
-      from pathlib import Path
-      from google_spreadsheets_exporter.exporter import Exporter
-        
-      BASE_DIR = Path(__file__).resolve() # adjust path to your credentials file filder as needed
-      data = [["Name"],["David"]]
-        
-      exp = Exporter("spreadsheet-id", "sheet-name", data, credentials_file_full_path=os.path.join(BASE_DIR, "creds.json"))
-      exp.export()
-
-## Complete Guide
-
-- Step 1: Set up a Google Sheets API Project
-
-    - Go to the Google Developers Console (https://console.developers.google.com/) and create a new project.
-      - A user for this project has to be created. Note its email.
-    - Enable the Google Sheets API for your project.
-    - Create credentials for your project to access the API. For this purpose, you'll need a service account key, which is a JSON file containing authentication information.
-      - Alternatively you can provide all credentials in a dictionary. For more on this - refer to the "Authenticating with dictionary of credentials" seciton.
-    - The credentials JSON file should be downloaded and included in your project.
-
-
-- Step 2: 
-    - Create a Google sheet from your account
-    - Note down Spreadsheet ID
-      - eg https[]()://docs.google.com/spreadsheets/d/<font color="green">*spreadsheetId-sdvs-dsv*</font>/edit#gid=0/
-    - Share the Spreadsheet with the email of your newly created Google project user.
-  
-
-- Step 3: Include this code snippet in you project
-    - Install the library by running
-      `pip install google-spreadsheets-exporter`
-        
-      Include the following code snippet for desired functionality
-        ````
-      from pathlib import Path
-      from google_spreadsheets_exporter.exporter import Exporter
-        
-      BASE_DIR = Path(__file__).resolve() # adjust path to your credentials file filder as needed
-      data = [["Name"],["David"]]
-        
-      exp = Exporter("spreadsheet-id", "sheet-name", data, credentials_file_full_path=os.path.join(BASE_DIR, "creds.json"))
-      exp.export()
-
-    where `spreadsheet-id` and `sheet-name` has been extracted from Spreadsheet url, `data` is 2D python array and
-    `credentials_file_full_path` is full path to your credentials file.
-
-
-### Authenticating with dictionary of credentials
-
-- You will need to assemble the dictionary of credentials that will match the JSON credentials file.
-    
-Sample dictionary:
-````
-credentials_info = {
-    "type": "service_account",
-    "project_id": "your-project-id",
-    "private_key_id": "your-private-key-id",
-    "private_key": "-----BEGIN PRIVATE KEY-----\n...\n-----END PRIVATE KEY-----\n",
-    "client_email": "your-service-account-email@your-project-id.iam.gserviceaccount.com",
-    "client_id": "your-client-id",
-    "auth_uri": "https://accounts.google.com/o/oauth2/auth",
-    "token_uri": "https://accounts.google.com/o/oauth2/token",
-    "auth_provider_x509_cert_url": "https://www.googleapis.com/oauth2/v1/certs",
-    "client_x509_cert_url": "https://www.googleapis.com/robot/v1/metadata/x509/your-service-account-email%40your-project-id.iam.gserviceaccount.com"
-}
-````
-
-- *Usecase*: Assumed use-case is that the JSON credentials file is downloaded from Google Cloud project
-  and for some reason is disassembled and is put back together at runtime. 
-
-- Once you assemble the dictionary of credentials, you will initialize the Exporter class like so:
-
-    `exp = Exporter("spreadsheet-id", "sheet-name", data, using_credentials_file=False, credentials_dictionary=my_assembled_dict))`
-
-
-Happy exporting.
+Metadata-Version: 2.1
+Name: google-spreadsheets-exporter
+Version: 1.0.2
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Description
+
+This library lets you export 2D arrays of data into your Google Spreadsheet.
+
+The following code snippet will export "Name" and "David" into your Google Spreadsheet,
+assuming you are all set up on the Google Cloud side.
+
+If this is not the case, continue to the section 'Complete Guide'
+
+## Quickstart:
+
+Install the library by running
+`pip install google-spreadsheets-exporter`
+
+Include the following code snippet for desired functionality
+
+      from pathlib import Path
+      from google_spreadsheets_exporter.exporter import Exporter
+        
+      BASE_DIR = Path(__file__).resolve() # adjust path to your credentials file filder as needed
+      data = [["Name"],["David"]]
+        
+      exp = Exporter("spreadsheet-id", "sheet-name", data, credentials_file_full_path=os.path.join(BASE_DIR, "creds.json"))
+      exp.export()
+
+## Complete Guide
+
+- Step 1: Set up a Google Sheets API Project
+
+    - Go to the Google Developers Console (https://console.developers.google.com/) and create a new project.
+      - A user for this project has to be created. Note its email.
+    - Enable the Google Sheets API for your project.
+    - Create credentials for your project to access the API. For this purpose, you'll need a service account key, which is a JSON file containing authentication information.
+      - Alternatively you can provide all credentials in a dictionary. For more on this - refer to the "Authenticating with dictionary of credentials" seciton.
+    - The credentials JSON file should be downloaded and included in your project.
+
+
+- Step 2: 
+    - Create a Google sheet from your account
+    - Note down Spreadsheet ID
+      - eg https[]()://docs.google.com/spreadsheets/d/<font color="green">*spreadsheetId-sdvs-dsv*</font>/edit#gid=0/
+    - Share the Spreadsheet with the email of your newly created Google project user.
+  
+
+- Step 3: Include this code snippet in you project
+    - Install the library by running
+      `pip install google-spreadsheets-exporter`
+        
+      Include the following code snippet for desired functionality
+        ````
+      from pathlib import Path
+      from google_spreadsheets_exporter.exporter import Exporter
+        
+      BASE_DIR = Path(__file__).resolve() # adjust path to your credentials file filder as needed
+      data = [["Name"],["David"]]
+        
+      exp = Exporter("spreadsheet-id", "sheet-name", data, credentials_file_full_path=os.path.join(BASE_DIR, "creds.json"))
+      exp.export()
+
+    where `spreadsheet-id` and `sheet-name` has been extracted from Spreadsheet url, `data` is 2D python array and
+    `credentials_file_full_path` is full path to your credentials file.
+
+
+### Authenticating with dictionary of credentials
+
+- You will need to assemble the dictionary of credentials that will match the JSON credentials file.
+    
+Sample dictionary:
+````
+credentials_info = {
+    "type": "service_account",
+    "project_id": "your-project-id",
+    "private_key_id": "your-private-key-id",
+    "private_key": "-----BEGIN PRIVATE KEY-----\n...\n-----END PRIVATE KEY-----\n",
+    "client_email": "your-service-account-email@your-project-id.iam.gserviceaccount.com",
+    "client_id": "your-client-id",
+    "auth_uri": "https://accounts.google.com/o/oauth2/auth",
+    "token_uri": "https://accounts.google.com/o/oauth2/token",
+    "auth_provider_x509_cert_url": "https://www.googleapis.com/oauth2/v1/certs",
+    "client_x509_cert_url": "https://www.googleapis.com/robot/v1/metadata/x509/your-service-account-email%40your-project-id.iam.gserviceaccount.com"
+}
+````
+
+- *Usecase*: Assumed use-case is that the JSON credentials file is downloaded from Google Cloud project
+  and for some reason is disassembled and is put back together at runtime. 
+
+- Once you assemble the dictionary of credentials, you will initialize the Exporter class like so:
+
+    `exp = Exporter("spreadsheet-id", "sheet-name", data, using_credentials_file=False, credentials_dictionary=my_assembled_dict))`
+
+
+Happy exporting.
```

### Comparing `google_spreadsheets_exporter-1.0.0/google_spreadsheets_exporter/exporter.py` & `google_spreadsheets_exporter-1.0.2/google_spreadsheets_exporter/exporter.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-from google.oauth2 import service_account
-from googleapiclient.discovery import build
-
-
-def load_credentials_from_file(credentials):
-    return service_account.Credentials.from_service_account_file(credentials)
-
-
-def load_credentials_from_dictionary(credentials):
-    return service_account.Credentials.from_service_account_info(credentials)
-
-
-class Exporter():
-    def __init__(self,
-                 spreadsheet_id:str,
-                 list_name:str,
-                 data:list,
-                 using_credentials_file:bool=True,
-                 credentials_file_full_path="credentials.json",
-                 credentials_dictionary=None):
-
-        super().__init__()
-        if credentials_dictionary is None:
-            credentials_dictionary = {}
-
-        self.spreadsheet_id = spreadsheet_id
-        self.list_name = list_name
-        self.data = data
-        self.using_credentials_file = using_credentials_file
-        self.creds_file_path = credentials_file_full_path
-        self.credentials_dictionary = credentials_dictionary
-
-        if using_credentials_file:
-            self.credentials = load_credentials_from_file(credentials_file_full_path)
-        else:
-            self.credentials = load_credentials_from_dictionary(credentials_dictionary)
-
-    def export(self):
-        print("exporting data ..")
-        service = build('sheets', 'v4', credentials=self.credentials)
-
-        # Spreadsheet ID - Obtain this from the URL of your Google Sheet
-        spreadsheet_id = self.spreadsheet_id
-
-        # Define the range where you want to insert the data (e.g., 'Sheet1!A1')
-        range_name = self.list_name
-
-        # Call the Sheets API to insert the data into the Google Sheet
-        result = service.spreadsheets().values().update(
-            spreadsheetId=spreadsheet_id,
-            range=range_name,
-            valueInputOption='RAW',
-            body={'values': self.data}
-        ).execute()
-
+from google.oauth2 import service_account
+from googleapiclient.discovery import build
+
+
+def load_credentials_from_file(credentials):
+    return service_account.Credentials.from_service_account_file(credentials)
+
+
+def load_credentials_from_dictionary(credentials):
+    return service_account.Credentials.from_service_account_info(credentials)
+
+
+class Exporter():
+    def __init__(self,
+                 spreadsheet_id:str,
+                 list_name:str,
+                 data:list,
+                 using_credentials_file:bool=True,
+                 credentials_file_full_path="credentials.json",
+                 credentials_dictionary=None):
+
+        super().__init__()
+        if credentials_dictionary is None:
+            credentials_dictionary = {}
+
+        self.spreadsheet_id = spreadsheet_id
+        self.list_name = list_name
+        self.data = data
+        self.using_credentials_file = using_credentials_file
+        self.creds_file_path = credentials_file_full_path
+        self.credentials_dictionary = credentials_dictionary
+
+        if using_credentials_file:
+            self.credentials = load_credentials_from_file(credentials_file_full_path)
+        else:
+            self.credentials = load_credentials_from_dictionary(credentials_dictionary)
+
+    def export(self):
+        print("exporting data ..")
+        service = build('sheets', 'v4', credentials=self.credentials)
+
+        # Spreadsheet ID - Obtain this from the URL of your Google Sheet
+        spreadsheet_id = self.spreadsheet_id
+
+        # Define the range where you want to insert the data (e.g., 'Sheet1!A1')
+        range_name = self.list_name
+
+        # Call the Sheets API to insert the data into the Google Sheet
+        result = service.spreadsheets().values().update(
+            spreadsheetId=spreadsheet_id,
+            range=range_name,
+            valueInputOption='RAW',
+            body={'values': self.data}
+        ).execute()
+
         print(f"{result.get('updatedCells')} cells updated.")
```

### Comparing `google_spreadsheets_exporter-1.0.0/google_spreadsheets_exporter/utils.py` & `google_spreadsheets_exporter-1.0.2/google_spreadsheets_exporter/utils.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from django.conf import settings
-
-# Define the default credentials file path
-DEFAULT_CREDENTIALS_FILE_PATH = 'credentials.json'
-
-# Function to load credentials from a specified file path or the default path
-def load_google_credentials():
-    credentials_file_path = getattr(settings, 'GOOGLE_SPREADSHEET_CREDENTIALS_FILE_PATH', DEFAULT_CREDENTIALS_FILE_PATH)
-    json_key_path = os.path.join(os.path.dirname(__file__), credentials_file_path)
+from django.conf import settings
+
+# Define the default credentials file path
+DEFAULT_CREDENTIALS_FILE_PATH = 'credentials.json'
+
+# Function to load credentials from a specified file path or the default path
+def load_google_credentials():
+    credentials_file_path = getattr(settings, 'GOOGLE_SPREADSHEET_CREDENTIALS_FILE_PATH', DEFAULT_CREDENTIALS_FILE_PATH)
+    json_key_path = os.path.join(os.path.dirname(__file__), credentials_file_path)
     return service_account.Credentials.from_service_account_file(json_key_path)
```

### Comparing `google_spreadsheets_exporter-1.0.0/google_spreadsheets_exporter.egg-info/PKG-INFO` & `google_spreadsheets_exporter-1.0.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,97 +1,92 @@
-Metadata-Version: 2.1
-Name: google-spreadsheets-exporter
-Version: 1.0.0
-Description-Content-Type: text/markdown
-
-# Description
-
-This library lets you export 2D arrays of data into your Google Spreadsheet.
-
-The following code snippet will export "Name" and "David" into your Google Spreadsheet,
-assuming you are all set up on the Google Cloud side.
-
-If this is not the case, continue to the section 'Complete Guide'
-
-## Quickstart:
-
-Install the library by running
-`pip install google-spreadsheets-exporter`
-
-Include the following code snippet for desired functionality
-
-      from pathlib import Path
-      from google_spreadsheets_exporter.exporter import Exporter
-        
-      BASE_DIR = Path(__file__).resolve() # adjust path to your credentials file filder as needed
-      data = [["Name"],["David"]]
-        
-      exp = Exporter("spreadsheet-id", "sheet-name", data, credentials_file_full_path=os.path.join(BASE_DIR, "creds.json"))
-      exp.export()
-
-## Complete Guide
-
-- Step 1: Set up a Google Sheets API Project
-
-    - Go to the Google Developers Console (https://console.developers.google.com/) and create a new project.
-      - A user for this project has to be created. Note its email.
-    - Enable the Google Sheets API for your project.
-    - Create credentials for your project to access the API. For this purpose, you'll need a service account key, which is a JSON file containing authentication information.
-      - Alternatively you can provide all credentials in a dictionary. For more on this - refer to the "Authenticating with dictionary of credentials" seciton.
-    - The credentials JSON file should be downloaded and included in your project.
-
-
-- Step 2: 
-    - Create a Google sheet from your account
-    - Note down Spreadsheet ID
-      - eg https[]()://docs.google.com/spreadsheets/d/<font color="green">*spreadsheetId-sdvs-dsv*</font>/edit#gid=0/
-    - Share the Spreadsheet with the email of your newly created Google project user.
-  
-
-- Step 3: Include this code snippet in you project
-    - Install the library by running
-      `pip install google-spreadsheets-exporter`
-        
-      Include the following code snippet for desired functionality
-        ````
-      from pathlib import Path
-      from google_spreadsheets_exporter.exporter import Exporter
-        
-      BASE_DIR = Path(__file__).resolve() # adjust path to your credentials file filder as needed
-      data = [["Name"],["David"]]
-        
-      exp = Exporter("spreadsheet-id", "sheet-name", data, credentials_file_full_path=os.path.join(BASE_DIR, "creds.json"))
-      exp.export()
-
-    where `spreadsheet-id` and `sheet-name` has been extracted from Spreadsheet url, `data` is 2D python array and
-    `credentials_file_full_path` is full path to your credentials file.
-
-
-### Authenticating with dictionary of credentials
-
-- You will need to assemble the dictionary of credentials that will match the JSON credentials file.
-    
-Sample dictionary:
-````
-credentials_info = {
-    "type": "service_account",
-    "project_id": "your-project-id",
-    "private_key_id": "your-private-key-id",
-    "private_key": "-----BEGIN PRIVATE KEY-----\n...\n-----END PRIVATE KEY-----\n",
-    "client_email": "your-service-account-email@your-project-id.iam.gserviceaccount.com",
-    "client_id": "your-client-id",
-    "auth_uri": "https://accounts.google.com/o/oauth2/auth",
-    "token_uri": "https://accounts.google.com/o/oauth2/token",
-    "auth_provider_x509_cert_url": "https://www.googleapis.com/oauth2/v1/certs",
-    "client_x509_cert_url": "https://www.googleapis.com/robot/v1/metadata/x509/your-service-account-email%40your-project-id.iam.gserviceaccount.com"
-}
-````
-
-- *Usecase*: Assumed use-case is that the JSON credentials file is downloaded from Google Cloud project
-  and for some reason is disassembled and is put back together at runtime. 
-
-- Once you assemble the dictionary of credentials, you will initialize the Exporter class like so:
-
-    `exp = Exporter("spreadsheet-id", "sheet-name", data, using_credentials_file=False, credentials_dictionary=my_assembled_dict))`
-
-
-Happy exporting.
+# Description
+
+This library lets you export 2D arrays of data into your Google Spreadsheet.
+
+The following code snippet will export "Name" and "David" into your Google Spreadsheet,
+assuming you are all set up on the Google Cloud side.
+
+If this is not the case, continue to the section 'Complete Guide'
+
+## Quickstart:
+
+Install the library by running
+`pip install google-spreadsheets-exporter`
+
+Include the following code snippet for desired functionality
+
+      from pathlib import Path
+      from google_spreadsheets_exporter.exporter import Exporter
+        
+      BASE_DIR = Path(__file__).resolve() # adjust path to your credentials file filder as needed
+      data = [["Name"],["David"]]
+        
+      exp = Exporter("spreadsheet-id", "sheet-name", data, credentials_file_full_path=os.path.join(BASE_DIR, "creds.json"))
+      exp.export()
+
+## Complete Guide
+
+- Step 1: Set up a Google Sheets API Project
+
+    - Go to the Google Developers Console (https://console.developers.google.com/) and create a new project.
+      - A user for this project has to be created. Note its email.
+    - Enable the Google Sheets API for your project.
+    - Create credentials for your project to access the API. For this purpose, you'll need a service account key, which is a JSON file containing authentication information.
+      - Alternatively you can provide all credentials in a dictionary. For more on this - refer to the "Authenticating with dictionary of credentials" seciton.
+    - The credentials JSON file should be downloaded and included in your project.
+
+
+- Step 2: 
+    - Create a Google sheet from your account
+    - Note down Spreadsheet ID
+      - eg https[]()://docs.google.com/spreadsheets/d/<font color="green">*spreadsheetId-sdvs-dsv*</font>/edit#gid=0/
+    - Share the Spreadsheet with the email of your newly created Google project user.
+  
+
+- Step 3: Include this code snippet in you project
+    - Install the library by running
+      `pip install google-spreadsheets-exporter`
+        
+      Include the following code snippet for desired functionality
+        ````
+      from pathlib import Path
+      from google_spreadsheets_exporter.exporter import Exporter
+        
+      BASE_DIR = Path(__file__).resolve() # adjust path to your credentials file filder as needed
+      data = [["Name"],["David"]]
+        
+      exp = Exporter("spreadsheet-id", "sheet-name", data, credentials_file_full_path=os.path.join(BASE_DIR, "creds.json"))
+      exp.export()
+
+    where `spreadsheet-id` and `sheet-name` has been extracted from Spreadsheet url, `data` is 2D python array and
+    `credentials_file_full_path` is full path to your credentials file.
+
+
+### Authenticating with dictionary of credentials
+
+- You will need to assemble the dictionary of credentials that will match the JSON credentials file.
+    
+Sample dictionary:
+````
+credentials_info = {
+    "type": "service_account",
+    "project_id": "your-project-id",
+    "private_key_id": "your-private-key-id",
+    "private_key": "-----BEGIN PRIVATE KEY-----\n...\n-----END PRIVATE KEY-----\n",
+    "client_email": "your-service-account-email@your-project-id.iam.gserviceaccount.com",
+    "client_id": "your-client-id",
+    "auth_uri": "https://accounts.google.com/o/oauth2/auth",
+    "token_uri": "https://accounts.google.com/o/oauth2/token",
+    "auth_provider_x509_cert_url": "https://www.googleapis.com/oauth2/v1/certs",
+    "client_x509_cert_url": "https://www.googleapis.com/robot/v1/metadata/x509/your-service-account-email%40your-project-id.iam.gserviceaccount.com"
+}
+````
+
+- *Usecase*: Assumed use-case is that the JSON credentials file is downloaded from Google Cloud project
+  and for some reason is disassembled and is put back together at runtime. 
+
+- Once you assemble the dictionary of credentials, you will initialize the Exporter class like so:
+
+    `exp = Exporter("spreadsheet-id", "sheet-name", data, using_credentials_file=False, credentials_dictionary=my_assembled_dict))`
+
+
+Happy exporting.
```

### Comparing `google_spreadsheets_exporter-1.0.0/setup.py` & `google_spreadsheets_exporter-1.0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from setuptools import setup
-
-with open("README.md", "r", encoding="utf-8") as f:
-    long_description = f.read()
-
-setup(
-    name='google_spreadsheets_exporter',
-    version='1.0.0',
-    packages=['google_spreadsheets_exporter'],
-    install_requires=[
-        'google-api-python-client',
-        'google-auth-httplib2',
-        'google-auth-oauthlib',
-    ],
-    exclude_package_data={'google_spreadsheets_exporter': ['creds.json', 'test.py']},
-    long_description=long_description,
-    long_description_content_type="text/markdown",
+from setuptools import setup
+
+with open("README.md", "r", encoding="utf-8") as f:
+    long_description = f.read()
+
+setup(
+    name='google_spreadsheets_exporter',
+    version='1.0.2',
+    packages=['google_spreadsheets_exporter'],
+    install_requires=[
+        'google-api-python-client',
+        'google-auth-httplib2',
+        'google-auth-oauthlib',
+    ],
+    exclude_package_data={'google_spreadsheets_exporter': ['creds.json', 'test.py']},
+    long_description=long_description,
+    long_description_content_type="text/markdown",
 )
```

