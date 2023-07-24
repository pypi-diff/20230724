# Comparing `tmp/genUniquePassw-1.1.4.tar.gz` & `tmp/genUniquePassw-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genUniquePassw-1.1.4.tar", last modified: Wed Jul 19 05:21:19 2023, max compression
+gzip compressed data, was "genUniquePassw-1.1.5.tar", last modified: Wed Jul 19 05:21:55 2023, max compression
```

## Comparing `genUniquePassw-1.1.4.tar` & `genUniquePassw-1.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-19 05:21:19.965974 genUniquePassw-1.1.4/
--rw-rw-r--   0 user      (1000) user      (1000)      733 2023-07-19 05:21:19.965974 genUniquePassw-1.1.4/PKG-INFO
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-19 05:21:19.965974 genUniquePassw-1.1.4/genUniquePassw.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      733 2023-07-19 05:21:19.000000 genUniquePassw-1.1.4/genUniquePassw.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      209 2023-07-19 05:21:19.000000 genUniquePassw-1.1.4/genUniquePassw.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-19 05:21:19.000000 genUniquePassw-1.1.4/genUniquePassw.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        8 2023-07-19 05:21:19.000000 genUniquePassw-1.1.4/genUniquePassw.egg-info/top_level.txt
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-19 05:21:19.965974 genUniquePassw-1.1.4/package/
--rw-rw-r--   0 user      (1000) user      (1000)       67 2023-07-19 05:17:45.000000 genUniquePassw-1.1.4/package/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1118 2023-07-19 05:07:20.000000 genUniquePassw-1.1.4/package/generate_password.py
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-19 05:21:19.965974 genUniquePassw-1.1.4/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1525 2023-07-19 04:53:36.000000 genUniquePassw-1.1.4/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-19 05:21:55.810797 genUniquePassw-1.1.5/
+-rw-rw-r--   0 user      (1000) user      (1000)      733 2023-07-19 05:21:55.810797 genUniquePassw-1.1.5/PKG-INFO
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-19 05:21:55.806797 genUniquePassw-1.1.5/genUniquePassw.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      733 2023-07-19 05:21:55.000000 genUniquePassw-1.1.5/genUniquePassw.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      209 2023-07-19 05:21:55.000000 genUniquePassw-1.1.5/genUniquePassw.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-19 05:21:55.000000 genUniquePassw-1.1.5/genUniquePassw.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        8 2023-07-19 05:21:55.000000 genUniquePassw-1.1.5/genUniquePassw.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-19 05:21:55.806797 genUniquePassw-1.1.5/package/
+-rw-rw-r--   0 user      (1000) user      (1000)       67 2023-07-19 05:17:45.000000 genUniquePassw-1.1.5/package/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1118 2023-07-19 05:07:20.000000 genUniquePassw-1.1.5/package/generate_password.py
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-19 05:21:55.810797 genUniquePassw-1.1.5/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1525 2023-07-19 05:21:43.000000 genUniquePassw-1.1.5/setup.py
```

### Comparing `genUniquePassw-1.1.4/PKG-INFO` & `genUniquePassw-1.1.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genUniquePassw
-Version: 1.1.4
+Version: 1.1.5
 Summary: Python package to generate random passwords of maximum length 12, avoiding names present in specified files.
 Home-page: https://github.com/kanchann23/genUniquePassw
 Author: kanchan
 Author-email: kanchanbora321@gmail.com
 License: MIT
 Keywords: security,password
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `genUniquePassw-1.1.4/genUniquePassw.egg-info/PKG-INFO` & `genUniquePassw-1.1.5/genUniquePassw.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genUniquePassw
-Version: 1.1.4
+Version: 1.1.5
 Summary: Python package to generate random passwords of maximum length 12, avoiding names present in specified files.
 Home-page: https://github.com/kanchann23/genUniquePassw
 Author: kanchan
 Author-email: kanchanbora321@gmail.com
 License: MIT
 Keywords: security,password
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `genUniquePassw-1.1.4/package/generate_password.py` & `genUniquePassw-1.1.5/package/generate_password.py`

 * *Files identical despite different names*

### Comparing `genUniquePassw-1.1.4/setup.py` & `genUniquePassw-1.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='genUniquePassw',       # Replace with the name of your package
-    version='1.1.4',                # Replace with the version number of your package
+    version='1.1.5',                # Replace with the version number of your package
     author='kanchan',             # Replace with the author's name
     author_email='kanchanbora321@gmail.com',  # Replace with the author's email
     description='Python package to generate random passwords of maximum length 12, avoiding names present in specified files.',
     long_description='generate password',  # Use README.md content or plain text
     long_description_content_type='text/plain',  # Specify the type of long description (text/plain, text/markdown, etc.)
     url='https://github.com/kanchann23/genUniquePassw',  # Replace with the URL of your package's repository
     license='MIT',                  # Replace with the license type of your package
```

