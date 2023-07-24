# Comparing `tmp/google_spreadsheets_exporter-0.3.4.tar.gz` & `tmp/google_spreadsheets_exporter-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_spreadsheets_exporter-0.3.4.tar", last modified: Mon Jul 24 15:34:15 2023, max compression
+gzip compressed data, was "google_spreadsheets_exporter-1.0.0.tar", last modified: Mon Jul 24 16:10:35 2023, max compression
```

## Comparing `google_spreadsheets_exporter-0.3.4.tar` & `google_spreadsheets_exporter-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 15:34:15.681620 google_spreadsheets_exporter-0.3.4/
--rw-rw-rw-   0        0        0       97 2023-07-24 13:56:18.000000 google_spreadsheets_exporter-0.3.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2696 2023-07-24 15:34:15.680622 google_spreadsheets_exporter-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     2576 2023-07-24 15:34:13.000000 google_spreadsheets_exporter-0.3.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-24 15:34:15.662621 google_spreadsheets_exporter-0.3.4/google_spreadsheets_exporter/
--rw-rw-rw-   0        0        0        0 2023-07-23 14:47:50.000000 google_spreadsheets_exporter-0.3.4/google_spreadsheets_exporter/__init__.py
--rw-rw-rw-   0        0        0     1390 2023-07-24 15:17:30.000000 google_spreadsheets_exporter-0.3.4/google_spreadsheets_exporter/exporter.py
--rw-rw-rw-   0        0        0      530 2023-07-23 15:45:17.000000 google_spreadsheets_exporter-0.3.4/google_spreadsheets_exporter/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-24 15:34:15.679619 google_spreadsheets_exporter-0.3.4/google_spreadsheets_exporter.egg-info/
--rw-rw-rw-   0        0        0     2696 2023-07-24 15:34:15.000000 google_spreadsheets_exporter-0.3.4/google_spreadsheets_exporter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      409 2023-07-24 15:34:15.000000 google_spreadsheets_exporter-0.3.4/google_spreadsheets_exporter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 15:34:15.000000 google_spreadsheets_exporter-0.3.4/google_spreadsheets_exporter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-07-24 15:34:15.000000 google_spreadsheets_exporter-0.3.4/google_spreadsheets_exporter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-07-24 15:34:15.000000 google_spreadsheets_exporter-0.3.4/google_spreadsheets_exporter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 15:34:15.681620 google_spreadsheets_exporter-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0      555 2023-07-24 15:34:13.000000 google_spreadsheets_exporter-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 16:10:35.549233 google_spreadsheets_exporter-1.0.0/
+-rw-rw-rw-   0        0        0       97 2023-07-24 13:56:18.000000 google_spreadsheets_exporter-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4188 2023-07-24 16:10:35.548234 google_spreadsheets_exporter-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4068 2023-07-24 16:09:59.000000 google_spreadsheets_exporter-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 16:10:35.526232 google_spreadsheets_exporter-1.0.0/google_spreadsheets_exporter/
+-rw-rw-rw-   0        0        0        0 2023-07-23 14:47:50.000000 google_spreadsheets_exporter-1.0.0/google_spreadsheets_exporter/__init__.py
+-rw-rw-rw-   0        0        0     2043 2023-07-24 16:00:39.000000 google_spreadsheets_exporter-1.0.0/google_spreadsheets_exporter/exporter.py
+-rw-rw-rw-   0        0        0      530 2023-07-23 15:45:17.000000 google_spreadsheets_exporter-1.0.0/google_spreadsheets_exporter/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-24 16:10:35.546234 google_spreadsheets_exporter-1.0.0/google_spreadsheets_exporter.egg-info/
+-rw-rw-rw-   0        0        0     4188 2023-07-24 16:10:35.000000 google_spreadsheets_exporter-1.0.0/google_spreadsheets_exporter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      409 2023-07-24 16:10:35.000000 google_spreadsheets_exporter-1.0.0/google_spreadsheets_exporter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 16:10:35.000000 google_spreadsheets_exporter-1.0.0/google_spreadsheets_exporter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-07-24 16:10:35.000000 google_spreadsheets_exporter-1.0.0/google_spreadsheets_exporter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-07-24 16:10:35.000000 google_spreadsheets_exporter-1.0.0/google_spreadsheets_exporter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 16:10:35.549233 google_spreadsheets_exporter-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      555 2023-07-24 16:10:18.000000 google_spreadsheets_exporter-1.0.0/setup.py
```

### Comparing `google_spreadsheets_exporter-0.3.4/PKG-INFO` & `google_spreadsheets_exporter-1.0.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-Metadata-Version: 2.1
-Name: google_spreadsheets_exporter
-Version: 0.3.4
-Description-Content-Type: text/markdown
-
 # Description
 
 This library lets you export 2D arrays of data into your Google Spreadsheet.
 
 The following code snippet will export "Name" and "David" into your Google Spreadsheet,
 assuming you are all set up on the Google Cloud side.
 
@@ -32,14 +27,15 @@
 
 - Step 1: Set up a Google Sheets API Project
 
     - Go to the Google Developers Console (https://console.developers.google.com/) and create a new project.
       - A user for this project has to be created. Note its email.
     - Enable the Google Sheets API for your project.
     - Create credentials for your project to access the API. For this purpose, you'll need a service account key, which is a JSON file containing authentication information.
+      - Alternatively you can provide all credentials in a dictionary. For more on this - refer to the "Authenticating with dictionary of credentials" seciton.
     - The credentials JSON file should be downloaded and included in your project.
 
 
 - Step 2: 
     - Create a Google sheet from your account
     - Note down Spreadsheet ID
       - eg https[]()://docs.google.com/spreadsheets/d/<font color="green">*spreadsheetId-sdvs-dsv*</font>/edit#gid=0/
@@ -60,8 +56,37 @@
         
       exp = Exporter("spreadsheet-id", "sheet-name", data, credentials_file_full_path=os.path.join(BASE_DIR, "creds.json"))
       exp.export()
 
     where `spreadsheet-id` and `sheet-name` has been extracted from Spreadsheet url, `data` is 2D python array and
     `credentials_file_full_path` is full path to your credentials file.
 
-Happy exporting.
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

### Comparing `google_spreadsheets_exporter-0.3.4/README.md` & `google_spreadsheets_exporter-1.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+Metadata-Version: 2.1
+Name: google_spreadsheets_exporter
+Version: 1.0.0
+Description-Content-Type: text/markdown
+
 # Description
 
 This library lets you export 2D arrays of data into your Google Spreadsheet.
 
 The following code snippet will export "Name" and "David" into your Google Spreadsheet,
 assuming you are all set up on the Google Cloud side.
 
@@ -27,14 +32,15 @@
 
 - Step 1: Set up a Google Sheets API Project
 
     - Go to the Google Developers Console (https://console.developers.google.com/) and create a new project.
       - A user for this project has to be created. Note its email.
     - Enable the Google Sheets API for your project.
     - Create credentials for your project to access the API. For this purpose, you'll need a service account key, which is a JSON file containing authentication information.
+      - Alternatively you can provide all credentials in a dictionary. For more on this - refer to the "Authenticating with dictionary of credentials" seciton.
     - The credentials JSON file should be downloaded and included in your project.
 
 
 - Step 2: 
     - Create a Google sheet from your account
     - Note down Spreadsheet ID
       - eg https[]()://docs.google.com/spreadsheets/d/<font color="green">*spreadsheetId-sdvs-dsv*</font>/edit#gid=0/
@@ -55,8 +61,37 @@
         
       exp = Exporter("spreadsheet-id", "sheet-name", data, credentials_file_full_path=os.path.join(BASE_DIR, "creds.json"))
       exp.export()
 
     where `spreadsheet-id` and `sheet-name` has been extracted from Spreadsheet url, `data` is 2D python array and
     `credentials_file_full_path` is full path to your credentials file.
 
-Happy exporting.
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

### Comparing `google_spreadsheets_exporter-0.3.4/google_spreadsheets_exporter/utils.py` & `google_spreadsheets_exporter-1.0.0/google_spreadsheets_exporter/utils.py`

 * *Files identical despite different names*

### Comparing `google_spreadsheets_exporter-0.3.4/google_spreadsheets_exporter.egg-info/PKG-INFO` & `google_spreadsheets_exporter-1.0.0/google_spreadsheets_exporter.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-spreadsheets-exporter
-Version: 0.3.4
+Version: 1.0.0
 Description-Content-Type: text/markdown
 
 # Description
 
 This library lets you export 2D arrays of data into your Google Spreadsheet.
 
 The following code snippet will export "Name" and "David" into your Google Spreadsheet,
@@ -32,14 +32,15 @@
 
 - Step 1: Set up a Google Sheets API Project
 
     - Go to the Google Developers Console (https://console.developers.google.com/) and create a new project.
       - A user for this project has to be created. Note its email.
     - Enable the Google Sheets API for your project.
     - Create credentials for your project to access the API. For this purpose, you'll need a service account key, which is a JSON file containing authentication information.
+      - Alternatively you can provide all credentials in a dictionary. For more on this - refer to the "Authenticating with dictionary of credentials" seciton.
     - The credentials JSON file should be downloaded and included in your project.
 
 
 - Step 2: 
     - Create a Google sheet from your account
     - Note down Spreadsheet ID
       - eg https[]()://docs.google.com/spreadsheets/d/<font color="green">*spreadsheetId-sdvs-dsv*</font>/edit#gid=0/
@@ -60,8 +61,37 @@
         
       exp = Exporter("spreadsheet-id", "sheet-name", data, credentials_file_full_path=os.path.join(BASE_DIR, "creds.json"))
       exp.export()
 
     where `spreadsheet-id` and `sheet-name` has been extracted from Spreadsheet url, `data` is 2D python array and
     `credentials_file_full_path` is full path to your credentials file.
 
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
 Happy exporting.
```

### Comparing `google_spreadsheets_exporter-0.3.4/setup.py` & `google_spreadsheets_exporter-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='google_spreadsheets_exporter',
-    version='0.3.4',
+    version='1.0.0',
     packages=['google_spreadsheets_exporter'],
     install_requires=[
         'google-api-python-client',
         'google-auth-httplib2',
         'google-auth-oauthlib',
     ],
     exclude_package_data={'google_spreadsheets_exporter': ['creds.json', 'test.py']},
```

