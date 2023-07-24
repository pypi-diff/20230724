# Comparing `tmp/speedtab-0.1.6.6.tar.gz` & `tmp/speedtab-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speedtab-0.1.6.6.tar", max compression
+gzip compressed data, was "speedtab-0.1.7.tar", max compression
```

## Comparing `speedtab-0.1.6.6.tar` & `speedtab-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      567 2023-07-24 15:43:35.768466 speedtab-0.1.6.6/pyproject.toml
--rw-r--r--   0        0        0      354 2023-07-24 13:24:26.057717 speedtab-0.1.6.6/speedtab/__init__.py
--rw-r--r--   0        0        0    53087 2023-07-24 15:43:35.720422 speedtab-0.1.6.6/speedtab/client.py
--rw-r--r--   0        0        0     6520 2023-07-24 13:55:52.073795 speedtab-0.1.6.6/speedtab/enums.py
--rw-r--r--   0        0        0     1848 2023-07-21 13:53:11.575405 speedtab-0.1.6.6/speedtab/formats.py
--rw-r--r--   0        0        0      783 2023-07-24 15:43:44.183059 speedtab-0.1.6.6/setup.py
--rw-r--r--   0        0        0      808 2023-07-24 15:43:44.183059 speedtab-0.1.6.6/PKG-INFO
+-rw-r--r--   0        0        0      565 2023-07-24 16:25:14.147381 speedtab-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      354 2023-07-24 13:24:26.057717 speedtab-0.1.7/speedtab/__init__.py
+-rw-r--r--   0        0        0    53658 2023-07-24 16:25:14.106218 speedtab-0.1.7/speedtab/client.py
+-rw-r--r--   0        0        0     6520 2023-07-24 13:55:52.073795 speedtab-0.1.7/speedtab/enums.py
+-rw-r--r--   0        0        0     1848 2023-07-21 13:53:11.575405 speedtab-0.1.7/speedtab/formats.py
+-rw-r--r--   0        0        0      781 2023-07-24 16:25:19.956258 speedtab-0.1.7/setup.py
+-rw-r--r--   0        0        0      806 2023-07-24 16:25:19.957268 speedtab-0.1.7/PKG-INFO
```

### Comparing `speedtab-0.1.6.6/pyproject.toml` & `speedtab-0.1.7/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "speedtab"
-version = "0.1.6.6"
+version = "0.1.7"
 description = "Convenient wrapper for working with Google Spreadsheets"
 authors = ["Bogdan Gergel <bogger147@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/BoggerSancho/SpeedTab-beta"
 repository = "https://github.com/BoggerSancho/SpeedTab-beta"
 
 [tool.poetry.dependencies]
```

### Comparing `speedtab-0.1.6.6/speedtab/client.py` & `speedtab-0.1.7/speedtab/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,23 +217,24 @@
                     },
                     'sheetId': sheet_id,
                 },
                 'fields': 'gridProperties.rowCount, gridProperties.columnCount',
             }}, None))
 
     def _get_metadata(self):
-        metadata = self.connect_v4.spreadsheets().get(spreadsheetId=self.spreadsheet_id).execute()
+        self.metadata = self.connect_v4.spreadsheets().get(spreadsheetId=self.spreadsheet_id).execute()
         self.sheets = dict(
             [(properties.get('title'), {
                 'max_column': properties.get('gridProperties').get('columnCount'),
                 'max_row': properties.get('gridProperties').get('rowCount'),
                 'sheetId': properties.get('sheetId'),
                 'position': properties.get('index'),
                 'charts': [chart.get('chartId') for chart in charts],
-            }) for properties, charts in [(sheet.get('properties'), sheet.get('charts', [])) for sheet in metadata.get('sheets')]]
+                'conditional_formats': len(conditional_formats),
+            }) for properties, charts, conditional_formats in [(sheet.get('properties'), sheet.get('charts', []), sheet.get('conditionalFormats', [])) for sheet in self.metadata.get('sheets')]]
         )
 
     def sheets_list(self):
         return list(self.sheets.keys())
 
     def exec(self):
         batch_update_chart_list = []
@@ -301,75 +302,75 @@
 
             fh = io.FileIO(output, mode='w')
 
             downloader = MediaIoBaseDownload(fh, request)
             done = False
             while done is False:
                 status, done = downloader.next_chunk()
-                print("Download %d%%." % int(status.progress() * 100))
+                print('Download %d%%.' % int(status.progress() * 100))
 
         except HttpError as error:
             print(F'An error occurred: {error}')
 
     def export_as_excel(self, output: str):
         try:
             request = self.connect_v3.files().export_media(fileId=self.spreadsheet_id, mimeType='application/vnd.openxmlformats-officedocument.spreadsheetml.sheet')
 
             fh = io.FileIO(output, mode='w')
 
             downloader = MediaIoBaseDownload(fh, request)
             done = False
             while done is False:
                 status, done = downloader.next_chunk()
-                print("Download %d%%." % int(status.progress() * 100))
+                print('Download %d%%.' % int(status.progress() * 100))
 
         except HttpError as error:
             print(F'An error occurred: {error}')
 
     def export_as_open_document(self, output: str):
         try:
             request = self.connect_v3.files().export_media(fileId=self.spreadsheet_id, mimeType='application/x-vnd.oasis.opendocument.spreadsheet')
 
             fh = io.FileIO(output, mode='w')
 
             downloader = MediaIoBaseDownload(fh, request)
             done = False
             while done is False:
                 status, done = downloader.next_chunk()
-                print("Download %d%%." % int(status.progress() * 100))
+                print('Download %d%%.' % int(status.progress() * 100))
 
         except HttpError as error:
             print(F'An error occurred: {error}')
 
     def export_as_pdf(self, output: str):
         try:
             request = self.connect_v3.files().export_media(fileId=self.spreadsheet_id, mimeType='application/pdf')
 
             fh = io.FileIO(output, mode='w')
 
             downloader = MediaIoBaseDownload(fh, request)
             done = False
             while done is False:
                 status, done = downloader.next_chunk()
-                print("Download %d%%." % int(status.progress() * 100))
+                print('Download %d%%.' % int(status.progress() * 100))
 
         except HttpError as error:
             print(F'An error occurred: {error}')
 
     def export_as_csv(self, output: str):
         try:
             request = self.connect_v3.files().export_media(fileId=self.spreadsheet_id, mimeType='text/csv')
 
             fh = io.FileIO(output, mode='w')
 
             downloader = MediaIoBaseDownload(fh, request)
             done = False
             while done is False:
                 status, done = downloader.next_chunk()
-                print("Download %d%%." % int(status.progress() * 100))
+                print('Download %d%%.' % int(status.progress() * 100))
 
         except HttpError as error:
             print(F'An error occurred: {error}')
 
 
 class Range:
     def __init__(self, sheet_id, _task_queue, work_zone, start_data_cell, base, data_cell):
@@ -715,17 +716,17 @@
                 },
                 'fields': 'gridProperties.hideGridlines',
             }
         }, self.work_zone))
         return self
 
     def insert_empty(self, axis: Union[str, int] = 0, inherit_from_before: bool = True):
-        """
+        '''
         Function to add rows and columns to selected range.
-        """
+        '''
         axis = axis.upper() if isinstance(axis, str) else DIMENSION.get(axis)
         self._task_queue.append(Task('clear', self._increment_task(), self.sheet_id, {
                 'insertDimension': {
                     'range': {
                         'sheetId': self.sheet_id,
                         'dimension': axis,
                         'startIndex': self.work_zone.get('startRowIndex') if axis == 'ROWS' else self.work_zone.get('startColumnIndex'),
@@ -780,18 +781,18 @@
                     },
                     'fields': 'userEnteredFormat, userEnteredValue',
                     'rows': copied_data
                 }}, self.work_zone))
         return self
 
     def set_background_color(self, color: Color = Color((255, 255, 255)), condition: BooleanCondition = None):
-        """
+        '''
         Function to set cell background color of Google Sheet
         :param color: background color in Color format
-        """
+        '''
 
         if condition:
             self._task_queue.append(Task('format', self._increment_task(), self.sheet_id, {
                 'addConditionalFormatRule': {
                     'rule': {
                         'ranges': [self.work_zone],
                         'booleanRule': {
@@ -1034,14 +1035,25 @@
             self._task_queue.append(Task('format', self._increment_task(), self.sheet_id, {
                     'deleteEmbeddedObject': {
                         'objectId': chart_id
                     }}, self.work_zone))
 
         return self
 
+    def delete_all_conditionals(self):
+        for i in range(self.sheets.get(self.sheet_name).get('conditional_formats') - 1, -1, -1):
+            self._task_queue.append(Task('format', self._increment_task(), self.sheet_id, {
+                'deleteConditionalFormatRule': {
+                    'sheetId': self.sheet_id,
+                    'index': i
+                }
+            }, self.work_zone))
+
+        return self
+
 
 class Client:
     def __init__(self, token_path='token.json'):
         self.token_path = token_path
         self.credentials = Credentials.from_authorized_user_file(self.token_path, SCOPES)
         self.list_of_spreadsheets = []
         self.connect_v4 = self._connect_v4()
@@ -1083,15 +1095,15 @@
                          connect_v3=self.connect_v3)
         self.list_of_spreadsheets.append(ss)
         return ss
 
     def create_folder(self, folder_name: str, parent_id: str = None):
         return self.connect_v3.files().create(body={
             'name': folder_name,
-            'mimeType': "application/vnd.google-apps.folder",
+            'mimeType': 'application/vnd.google-apps.folder',
             'parents': [parent_id] if parent_id else None,
         }, supportsAllDrives=True).execute()['id']
 
     def rename_folder(self, fileId, name):
         self.connect_v3.files().update(body={
             'name': name,
         }, fileId=fileId, supportsAllDrives=True).execute()
```

### Comparing `speedtab-0.1.6.6/speedtab/enums.py` & `speedtab-0.1.7/speedtab/enums.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.1.6.6/speedtab/formats.py` & `speedtab-0.1.7/speedtab/formats.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.1.6.6/setup.py` & `speedtab-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['google-api-python-client>=2.58.0,<3.0.0',
  'google-auth-httplib2>=0.1.0,<0.2.0',
  'google-auth-oauthlib>=0.5.2,<0.6.0']
 
 setup_kwargs = {
     'name': 'speedtab',
-    'version': '0.1.6.6',
+    'version': '0.1.7',
     'description': 'Convenient wrapper for working with Google Spreadsheets',
     'long_description': None,
     'author': 'Bogdan Gergel',
     'author_email': 'bogger147@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/BoggerSancho/SpeedTab-beta',
```

### Comparing `speedtab-0.1.6.6/PKG-INFO` & `speedtab-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedtab
-Version: 0.1.6.6
+Version: 0.1.7
 Summary: Convenient wrapper for working with Google Spreadsheets
 Home-page: https://github.com/BoggerSancho/SpeedTab-beta
 License: MIT
 Author: Bogdan Gergel
 Author-email: bogger147@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

