# Comparing `tmp/workbooky-0.0.2.tar.gz` & `tmp/workbooky-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "workbooky-0.0.2.tar", last modified: Wed May 10 08:06:03 2023, max compression
+gzip compressed data, was "workbooky-0.0.3.tar", last modified: Mon Jul 24 08:30:15 2023, max compression
```

## Comparing `workbooky-0.0.2.tar` & `workbooky-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,23 @@
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-10 08:06:03.285064 workbooky-0.0.2/
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 workbooky-0.0.2/LICENSE.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)      729 2023-05-10 08:06:03.285064 workbooky-0.0.2/PKG-INFO
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)      131 2023-05-10 06:26:57.000000 workbooky-0.0.2/README.md
--rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-05-10 08:06:03.285064 workbooky-0.0.2/setup.cfg
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1173 2023-05-10 06:29:32.000000 workbooky-0.0.2/setup.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-10 08:06:03.285064 workbooky-0.0.2/workbooky/
--rw-r--r--   0 jeff      (1000) jeff      (1001)      130 2023-05-10 06:29:45.000000 workbooky-0.0.2/workbooky/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-05-10 08:05:25.000000 workbooky-0.0.2/workbooky/_version.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-10 08:06:03.285064 workbooky-0.0.2/workbooky/src/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-09 13:37:49.000000 workbooky-0.0.2/workbooky/src/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1516 2023-05-10 08:05:12.000000 workbooky-0.0.2/workbooky/src/workbook.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-10 08:06:03.285064 workbooky-0.0.2/workbooky.egg-info/
--rw-r--r--   0 jeff      (1000) jeff      (1001)      729 2023-05-10 08:06:03.000000 workbooky-0.0.2/workbooky.egg-info/PKG-INFO
--rw-r--r--   0 jeff      (1000) jeff      (1001)      268 2023-05-10 08:06:03.000000 workbooky-0.0.2/workbooky.egg-info/SOURCES.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-05-10 08:06:03.000000 workbooky-0.0.2/workbooky.egg-info/dependency_links.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       10 2023-05-10 08:06:03.000000 workbooky-0.0.2/workbooky.egg-info/top_level.txt
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-07-24 08:30:15.806786 workbooky-0.0.3/
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 workbooky-0.0.3/LICENSE.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      959 2023-07-24 08:30:15.810119 workbooky-0.0.3/PKG-INFO
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)      298 2023-07-22 11:08:39.000000 workbooky-0.0.3/README.md
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-07-24 08:30:15.810119 workbooky-0.0.3/setup.cfg
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1355 2023-07-24 08:28:30.000000 workbooky-0.0.3/setup.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-07-24 08:30:15.806786 workbooky-0.0.3/workbooky/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      130 2023-05-10 06:29:45.000000 workbooky-0.0.3/workbooky/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-07-24 08:22:09.000000 workbooky-0.0.3/workbooky/_version.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-07-24 08:30:15.806786 workbooky-0.0.3/workbooky/src/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-09 13:37:49.000000 workbooky-0.0.3/workbooky/src/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     2713 2023-07-24 08:20:45.000000 workbooky-0.0.3/workbooky/src/workbook.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-07-24 08:30:15.806786 workbooky-0.0.3/workbooky/tests/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-07-23 11:39:09.000000 workbooky-0.0.3/workbooky/tests/__init__.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-07-24 08:30:15.806786 workbooky-0.0.3/workbooky/tests/test_data/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-07-24 07:54:16.000000 workbooky-0.0.3/workbooky/tests/test_data/invalid_workbook.xlsx
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     5381 2023-07-24 08:20:30.000000 workbooky-0.0.3/workbooky/tests/test_data/valid_workbook.xlsx
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1788 2023-07-24 08:21:32.000000 workbooky-0.0.3/workbooky/tests/test_workbook.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-07-24 08:30:15.806786 workbooky-0.0.3/workbooky.egg-info/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      959 2023-07-24 08:30:15.000000 workbooky-0.0.3/workbooky.egg-info/PKG-INFO
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      423 2023-07-24 08:30:15.000000 workbooky-0.0.3/workbooky.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-07-24 08:30:15.000000 workbooky-0.0.3/workbooky.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       10 2023-07-24 08:30:15.000000 workbooky-0.0.3/workbooky.egg-info/top_level.txt
```

### Comparing `workbooky-0.0.2/LICENSE.txt` & `workbooky-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `workbooky-0.0.2/setup.py` & `workbooky-0.0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -34,8 +34,17 @@
     download_url='https://pypi.org/project/bfgdealer/',
 )
 
 install_requires = [
 ]
 
 if __name__ == '__main__':
-    setup(**setup_args, install_requires=install_requires)
+    setup(
+        package_data={
+            'workbooky': [
+                'tests/test_data/*.xlsx',
+                ]
+        },
+        include_package_data=True,
+        **setup_args,
+        install_requires=install_requires
+        )
```

### Comparing `workbooky-0.0.2/workbooky/src/workbook.py` & `workbooky-0.0.3/workbooky/src/workbook.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,76 @@
-"""Methods to validate and open workbook and worksheets."""
+"""Excel workbook and worksheets utilities."""
 import os
+import sys
 from openpyxl import load_workbook, utils as openpyxl_utils
 import zipfile
 from termcolor import cprint
 import colorama
 
 colorama.init()
 
 ERROR_COLOUR = 'red'
+INVALID_EXCEL_FILE = 'is not a valid excel file'
+QUITTING = 'Quitting ...'
+PATH_ERROR = 'File path error'
+WORKBOOK_ERROR = 'Workbook error'
+WORKSHEET_ERROR = 'Worksheet error'
+WORKBOOK_MISSING = 'Cannot find workbook:'
+NAMED_CORRECTLY = 'Is it named correctly?'
+MISSING_SHEET = ': missing sheet in the workbook'
+
 
 class Workbook():
     def __init__(self, workbook_path: str):
         self.path = str(workbook_path)
         self.workbook = self._get_workbook()
+        self.worksheets = {sheet._WorkbookChild__title: sheet for sheet in self.workbook.worksheets}
 
     def _get_workbook(self) -> object:
-        # Return the workbook if it exists, otherwise quit.
+        """Return the workbook if it exists, otherwise quit. """
         if not os.path.isfile(self.path):
-            cprint(f"Cannot find workbook in: {self.path}", ERROR_COLOUR)
-            cprint(f"Is it named correctly?", ERROR_COLOUR)
-            quit()
+            cprint(f"{WORKBOOK_MISSING} {self.path}", ERROR_COLOUR)
+            cprint(f'{NAMED_CORRECTLY}', ERROR_COLOUR)
+            sys.exit(f'{QUITTING} {PATH_ERROR}')
         try:
             workbook = load_workbook(filename=self.path, data_only=True)
             return workbook
         except openpyxl_utils.exceptions.InvalidFileException:
-            cprint(f"{self.path} is not a valid excel file", ERROR_COLOUR)
-            quit()
+            cprint(f"{self.path} {INVALID_EXCEL_FILE}", ERROR_COLOUR)
+            sys.exit(f'{QUITTING} {WORKBOOK_ERROR}')
         except zipfile.BadZipFile:
-            cprint(f"{self.path} is not a valid excel file", ERROR_COLOUR)
-            quit()
+            cprint(f"{self.path} {INVALID_EXCEL_FILE}", ERROR_COLOUR)
+            sys.exit(f'{QUITTING} {WORKBOOK_ERROR}')
+
+    def list_worksheets(self) -> None:
+        "Print worksheet names."
+        print('')
+        print('*'*5, 'Sheets', '*'*5)
+        for sheet in self.worksheets:
+            print(sheet._WorkbookChild__title)
+        print('*'*18)
 
     def get_worksheet(self, sheet_name: str) -> object:
-        # Return the worksheet if it exists, otherwise quit.
+        """Return the worksheet if it exists, otherwise quit."""
         try:
             worksheet = self.workbook[sheet_name]
             return worksheet
         except KeyError:
-            cprint(f"There is no {sheet_name} sheet in the workbook {self.path}", ERROR_COLOUR)
-            quit()
-
-    def save(self) -> None:
-        # Save the workbook
-        self.workbook.save(self.path)
+            msg = f"{sheet_name}{MISSING_SHEET} {self.path}"
+            cprint(msg, ERROR_COLOUR)
+            sys.exit(f'{QUITTING} {WORKSHEET_ERROR}')
+
+    def rows_from_worksheet(self, sheet_name, ignore_first_row=True):
+        """Return all of the rows from a worksheet."""
+        worksheet = self.worksheets[sheet_name]
+        rows = []
+        for row in worksheet.iter_rows(values_only=True):
+            rows.append(row)
+        if ignore_first_row:
+            rows.pop(0)
+        return rows
+
+    def save(self, path=None) -> None:
+        """Save the workbook to the path."""
+        if not path:
+            path = self.path
+        self.workbook.save(path)
```

