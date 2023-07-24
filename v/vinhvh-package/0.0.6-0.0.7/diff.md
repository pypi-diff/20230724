# Comparing `tmp/vinhvh_package-0.0.6.tar.gz` & `tmp/vinhvh_package-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vinhvh_package-0.0.6.tar", last modified: Sun Jul 23 10:37:24 2023, max compression
+gzip compressed data, was "vinhvh_package-0.0.7.tar", last modified: Mon Jul 24 09:53:23 2023, max compression
```

## Comparing `vinhvh_package-0.0.6.tar` & `vinhvh_package-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-23 10:37:24.873783 vinhvh_package-0.0.6/
--rw-rw-rw-   0        0        0     1091 2023-07-23 05:09:13.000000 vinhvh_package-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      557 2023-07-23 10:37:24.872780 vinhvh_package-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       25 2023-07-23 06:07:00.000000 vinhvh_package-0.0.6/README.md
--rw-rw-rw-   0        0        0      612 2023-07-23 10:36:52.000000 vinhvh_package-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-23 10:37:24.873783 vinhvh_package-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-23 10:37:24.495676 vinhvh_package-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-07-23 10:37:24.852728 vinhvh_package-0.0.6/src/vinhvh_package/
--rw-rw-rw-   0        0        0        0 2023-07-23 06:05:35.000000 vinhvh_package-0.0.6/src/vinhvh_package/__init__.py
--rw-rw-rw-   0        0        0    14125 2023-07-23 10:36:04.000000 vinhvh_package-0.0.6/src/vinhvh_package/vinhvh.py
-drwxrwxrwx   0        0        0        0 2023-07-23 10:37:24.870775 vinhvh_package-0.0.6/src/vinhvh_package.egg-info/
--rw-rw-rw-   0        0        0      557 2023-07-23 10:37:24.000000 vinhvh_package-0.0.6/src/vinhvh_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-07-23 10:37:24.000000 vinhvh_package-0.0.6/src/vinhvh_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-23 10:37:24.000000 vinhvh_package-0.0.6/src/vinhvh_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-23 10:37:24.000000 vinhvh_package-0.0.6/src/vinhvh_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 09:53:23.139003 vinhvh_package-0.0.7/
+-rw-rw-rw-   0        0        0     1091 2023-07-23 05:09:13.000000 vinhvh_package-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      557 2023-07-24 09:53:23.137999 vinhvh_package-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       25 2023-07-23 06:07:00.000000 vinhvh_package-0.0.7/README.md
+-rw-rw-rw-   0        0        0      612 2023-07-24 09:52:48.000000 vinhvh_package-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-24 09:53:23.140004 vinhvh_package-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-24 09:53:23.053272 vinhvh_package-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-07-24 09:53:23.111931 vinhvh_package-0.0.7/src/vinhvh_package/
+-rw-rw-rw-   0        0        0        0 2023-07-23 06:05:35.000000 vinhvh_package-0.0.7/src/vinhvh_package/__init__.py
+-rw-rw-rw-   0        0        0    17789 2023-07-24 05:12:22.000000 vinhvh_package-0.0.7/src/vinhvh_package/test_module.py
+-rw-rw-rw-   0        0        0    17410 2023-07-24 09:52:23.000000 vinhvh_package-0.0.7/src/vinhvh_package/vinhvh.py
+drwxrwxrwx   0        0        0        0 2023-07-24 09:53:23.136997 vinhvh_package-0.0.7/src/vinhvh_package.egg-info/
+-rw-rw-rw-   0        0        0      557 2023-07-24 09:53:23.000000 vinhvh_package-0.0.7/src/vinhvh_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-07-24 09:53:23.000000 vinhvh_package-0.0.7/src/vinhvh_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 09:53:23.000000 vinhvh_package-0.0.7/src/vinhvh_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-24 09:53:23.000000 vinhvh_package-0.0.7/src/vinhvh_package.egg-info/top_level.txt
```

### Comparing `vinhvh_package-0.0.6/LICENSE` & `vinhvh_package-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `vinhvh_package-0.0.6/PKG-INFO` & `vinhvh_package-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vinhvh_package
-Version: 0.0.6
+Version: 0.0.7
 Summary: A small example package
 Author-email: VinhVH <vinhvh89.dc@gmail.com>
 Project-URL: Homepage, https://github.com/VinhVu8x/packaging_tutorial
 Project-URL: Bug Tracker, https://github.com/VinhVu8x/packaging_tutorial/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `vinhvh_package-0.0.6/pyproject.toml` & `vinhvh_package-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vinhvh_package"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="VinhVH", email="vinhvh89.dc@gmail.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `vinhvh_package-0.0.6/src/vinhvh_package/vinhvh.py` & `vinhvh_package-0.0.7/src/vinhvh_package/test_module.py`

 * *Files 16% similar despite different names*

```diff
@@ -61,14 +61,120 @@
         print('File selection closed.')
         sys.exit()
     # If the user didn't select any files, return None
     else:
         return None
 
 
+def select_file_2(file: list = None, value: list = None, option: dict = None, checkbox: list = None, mode: str = 'single', title: str = 'File Selector'):
+    """
+    This function create a interface for user with different option input
+
+    Parameters
+    ----------
+    file: (list, optional)
+        File to browse
+    value: (list, optional)
+        Value for input
+    Option: (dict, optional)
+        Combobox for select
+    Checkbox: (list, optional)
+        Option for select
+    Tilte: (str, optional)
+        Name of window
+    """
+    # Set the PySimpleGUI theme
+    sg.theme('Dark Blue 3')
+
+    # Create the layout for the file selector window
+    layout = [[sg.Text('Select values ')]]
+    file_paths = []
+    len_path = 0
+    if file is not None:
+        if mode == 'single':
+            for name in file:
+                layout.append([sg.Text(name + ": ", size=(15, 1),),
+                               sg.InputText(), sg.FileBrowse()])
+        elif mode == 'multi':
+            for name in file:
+                layout.append([sg.Text(name + ": ", size=(15, 1),),
+                               sg.InputText(key=f'{name}'), sg.FilesBrowse()])
+
+    if value is not None:
+        for name in value:
+            layout.append([sg.Text(name + ": ", size=(15, 1),),
+                           sg.InputText()])
+
+    if option is not None:
+        for name, value in option.items():
+            layout.append([sg.Text(name + ': ', size=(15, 1)),
+                          sg.Combo(value, default_value=value[0], size=(43, 1))],)
+
+    if checkbox is not None:
+        for name in checkbox:
+            layout.append([sg.Checkbox(name + ':', default=False)])
+
+    # Add the Submit and Cancel buttons to the layout
+    layout.append([sg.Submit(), sg.Cancel()])
+
+    # Create the file selector window
+    window = sg.Window(title, layout)
+
+    # Wait for the user to interact with the window
+    event, values = window.read()
+
+    # Close the window
+    window.close()
+
+    # Process the user's selection
+    if event == 'Submit':
+
+        if file is not None:
+            # If in single mode, get the file paths from the input fields
+            if mode == 'single':
+                path = [values[i] for i in range(len(file))]
+                len_path += len(file)
+
+            # If in multi mode, get the file paths as a list of lists from the input fields
+            elif mode == 'multi':
+                path = [values[f'{name}'].split(';') for name in file]
+            file_paths += path
+
+        if value is not None:
+            path = [values[i] for i in range(len_path, len_path + len(value))]
+            file_paths += path
+            len_path += len(value)
+
+        if option is not None:
+            path = [values[i] for i in range(len_path, len_path + len(option))]
+            file_paths += path
+            len_path += len(option)
+
+        if checkbox is not None:
+            path = [values[i]
+                    for i in range(len_path, len_path + len(checkbox))]
+            file_paths += path
+            len_path += len(checkbox)
+
+            # Return the list of file paths
+        return file_paths
+
+    # If the user clicked the Cancel button, print a message and exit the program
+    elif event == 'Cancel':
+        print('File selection cancelled.')
+        sys.exit()
+    # If the user closed the window, print a message and exit the program
+    elif event == sg.WIN_CLOSED:
+        print('File selection closed.')
+        sys.exit()
+    # If the user didn't select any files, return None
+    else:
+        return None
+
+
 def select_input_file(names1, names2, mode='single'):
     # Set the PySimpleGUI theme
     sg.theme('Dark Blue 3')
 
     # Create the layout for the file selector window
     layout = [[sg.Text('Choose files ')]]
```

### Comparing `vinhvh_package-0.0.6/src/vinhvh_package.egg-info/PKG-INFO` & `vinhvh_package-0.0.7/src/vinhvh_package.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vinhvh-package
-Version: 0.0.6
+Version: 0.0.7
 Summary: A small example package
 Author-email: VinhVH <vinhvh89.dc@gmail.com>
 Project-URL: Homepage, https://github.com/VinhVu8x/packaging_tutorial
 Project-URL: Bug Tracker, https://github.com/VinhVu8x/packaging_tutorial/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

