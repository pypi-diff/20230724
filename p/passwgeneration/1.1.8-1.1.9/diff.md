# Comparing `tmp/passwgeneration-1.1.8.tar.gz` & `tmp/passwgeneration-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "passwgeneration-1.1.8.tar", last modified: Mon Jul 24 09:24:06 2023, max compression
+gzip compressed data, was "passwgeneration-1.1.9.tar", last modified: Mon Jul 24 09:56:09 2023, max compression
```

## Comparing `passwgeneration-1.1.8.tar` & `passwgeneration-1.1.9.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 09:24:06.465263 passwgeneration-1.1.8/
--rw-rw-r--   0 user      (1000) user      (1000)      734 2023-07-24 09:24:06.465263 passwgeneration-1.1.8/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      368 2023-07-19 21:20:51.000000 passwgeneration-1.1.8/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 09:24:06.461268 passwgeneration-1.1.8/passwgeneration/
--rw-rw-r--   0 user      (1000) user      (1000)       66 2023-07-19 05:32:29.000000 passwgeneration-1.1.8/passwgeneration/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1616 2023-07-24 09:22:16.000000 passwgeneration-1.1.8/passwgeneration/generate_password.py
--rw-rw-r--   0 user      (1000) user      (1000)      854 2023-07-20 09:51:42.000000 passwgeneration-1.1.8/passwgeneration/test_passw.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 09:24:06.465263 passwgeneration-1.1.8/passwgeneration.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      734 2023-07-24 09:24:05.000000 passwgeneration-1.1.8/passwgeneration.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      269 2023-07-24 09:24:06.000000 passwgeneration-1.1.8/passwgeneration.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 09:24:05.000000 passwgeneration-1.1.8/passwgeneration.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       16 2023-07-24 09:24:05.000000 passwgeneration-1.1.8/passwgeneration.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-24 09:24:06.465263 passwgeneration-1.1.8/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1526 2023-07-24 09:23:18.000000 passwgeneration-1.1.8/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 09:56:09.127621 passwgeneration-1.1.9/
+-rw-rw-r--   0 user      (1000) user      (1000)       36 2023-07-24 09:52:39.000000 passwgeneration-1.1.9/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)      734 2023-07-24 09:56:09.127621 passwgeneration-1.1.9/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      368 2023-07-19 21:20:51.000000 passwgeneration-1.1.9/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 09:56:09.123621 passwgeneration-1.1.9/passwgeneration/
+-rw-rw-r--   0 user      (1000) user      (1000)       66 2023-07-19 05:32:29.000000 passwgeneration-1.1.9/passwgeneration/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1616 2023-07-24 09:22:16.000000 passwgeneration-1.1.9/passwgeneration/generate_password.py
+-rw-rw-r--   0 user      (1000) user      (1000)      854 2023-07-20 09:51:42.000000 passwgeneration-1.1.9/passwgeneration/test_passw.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 09:56:09.127621 passwgeneration-1.1.9/passwgeneration.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      734 2023-07-24 09:56:08.000000 passwgeneration-1.1.9/passwgeneration.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      281 2023-07-24 09:56:08.000000 passwgeneration-1.1.9/passwgeneration.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 09:56:08.000000 passwgeneration-1.1.9/passwgeneration.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       16 2023-07-24 09:56:08.000000 passwgeneration-1.1.9/passwgeneration.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-24 09:56:09.127621 passwgeneration-1.1.9/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1557 2023-07-24 09:55:59.000000 passwgeneration-1.1.9/setup.py
```

### Comparing `passwgeneration-1.1.8/PKG-INFO` & `passwgeneration-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: passwgeneration
-Version: 1.1.8
+Version: 1.1.9
 Summary: Python package to generate random passwords of maximum length 12, avoiding names present in specified files.
 Home-page: https://github.com/kanchann23/genUniquePassw
 Author: kanchan
 Author-email: kanchanbora321@gmail.com
 License: MIT
 Keywords: security,password
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `passwgeneration-1.1.8/passwgeneration/generate_password.py` & `passwgeneration-1.1.9/passwgeneration/generate_password.py`

 * *Files identical despite different names*

### Comparing `passwgeneration-1.1.8/passwgeneration/test_passw.py` & `passwgeneration-1.1.9/passwgeneration/test_passw.py`

 * *Files identical despite different names*

### Comparing `passwgeneration-1.1.8/passwgeneration.egg-info/PKG-INFO` & `passwgeneration-1.1.9/passwgeneration.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: passwgeneration
-Version: 1.1.8
+Version: 1.1.9
 Summary: Python package to generate random passwords of maximum length 12, avoiding names present in specified files.
 Home-page: https://github.com/kanchann23/genUniquePassw
 Author: kanchan
 Author-email: kanchanbora321@gmail.com
 License: MIT
 Keywords: security,password
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `passwgeneration-1.1.8/setup.py` & `passwgeneration-1.1.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name='passwgeneration',       # Replace with the name of your package
-    version='1.1.8',                # Replace with the version number of your package
+    version='1.1.9',                # Replace with the version number of your package
     author='kanchan',             # Replace with the author's name
     author_email='kanchanbora321@gmail.com',  # Replace with the author's email
+    include_package_data=True,
     description='Python package to generate random passwords of maximum length 12, avoiding names present in specified files.',
     long_description='generate password',  # Use README.md content or plain text
     long_description_content_type='text/plain',  # Specify the type of long description (text/plain, text/markdown, etc.)
     url='https://github.com/kanchann23/genUniquePassw',  # Replace with the URL of your package's repository
     license='MIT',                  # Replace with the license type of your package
     keywords=['security', 'password'],  # Replace with relevant keywords related to your package
     packages=find_packages(),       # Automatically find and include all packages in the project
```

