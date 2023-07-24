# Comparing `tmp/pyrdams-2.1.2.tar.gz` & `tmp/pyrdams-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrdams-2.1.2.tar", last modified: Tue Jan 31 10:47:26 2023, max compression
+gzip compressed data, was "pyrdams-2.1.3.tar", last modified: Mon Jul 24 13:20:04 2023, max compression
```

## Comparing `pyrdams-2.1.2.tar` & `pyrdams-2.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mdalchen   (501) staff       (20)        0 2023-01-31 10:47:26.010480 pyrdams-2.1.2/
--rw-r--r--   0 mdalchen   (501) staff       (20)     5922 2023-01-31 10:47:26.010204 pyrdams-2.1.2/PKG-INFO
--rw-r--r--   0 mdalchen   (501) staff       (20)     5526 2023-01-03 14:13:52.000000 pyrdams-2.1.2/README.md
--rw-r--r--   0 mdalchen   (501) staff       (20)      750 2023-01-03 14:13:52.000000 pyrdams-2.1.2/pyproject.toml
-drwxr-xr-x   0 mdalchen   (501) staff       (20)        0 2023-01-31 10:47:26.009884 pyrdams-2.1.2/pyrdams.egg-info/
--rw-r--r--   0 mdalchen   (501) staff       (20)     5922 2023-01-31 10:47:26.000000 pyrdams-2.1.2/pyrdams.egg-info/PKG-INFO
--rw-r--r--   0 mdalchen   (501) staff       (20)      228 2023-01-31 10:47:26.000000 pyrdams-2.1.2/pyrdams.egg-info/SOURCES.txt
--rw-r--r--   0 mdalchen   (501) staff       (20)        1 2023-01-31 10:47:26.000000 pyrdams-2.1.2/pyrdams.egg-info/dependency_links.txt
--rw-r--r--   0 mdalchen   (501) staff       (20)       44 2023-01-31 10:47:26.000000 pyrdams-2.1.2/pyrdams.egg-info/entry_points.txt
--rw-r--r--   0 mdalchen   (501) staff       (20)        9 2023-01-31 10:47:26.000000 pyrdams-2.1.2/pyrdams.egg-info/requires.txt
--rw-r--r--   0 mdalchen   (501) staff       (20)       13 2023-01-31 10:47:26.000000 pyrdams-2.1.2/pyrdams.egg-info/top_level.txt
--rwxr-xr-x   0 mdalchen   (501) staff       (20)    20065 2023-01-31 10:24:16.000000 pyrdams-2.1.2/rdams_client.py
--rw-r--r--   0 mdalchen   (501) staff       (20)       38 2023-01-31 10:47:26.010565 pyrdams-2.1.2/setup.cfg
+drwxr-xr-x   0 mdalchen   (501) staff       (20)        0 2023-07-24 13:20:04.187635 pyrdams-2.1.3/
+-rw-r--r--   0 mdalchen   (501) staff       (20)     5922 2023-07-24 13:20:04.187367 pyrdams-2.1.3/PKG-INFO
+-rw-r--r--   0 mdalchen   (501) staff       (20)     5526 2023-01-03 14:13:52.000000 pyrdams-2.1.3/README.md
+-rw-r--r--   0 mdalchen   (501) staff       (20)      750 2023-01-03 14:13:52.000000 pyrdams-2.1.3/pyproject.toml
+drwxr-xr-x   0 mdalchen   (501) staff       (20)        0 2023-07-24 13:20:04.187057 pyrdams-2.1.3/pyrdams.egg-info/
+-rw-r--r--   0 mdalchen   (501) staff       (20)     5922 2023-07-24 13:20:04.000000 pyrdams-2.1.3/pyrdams.egg-info/PKG-INFO
+-rw-r--r--   0 mdalchen   (501) staff       (20)      228 2023-07-24 13:20:04.000000 pyrdams-2.1.3/pyrdams.egg-info/SOURCES.txt
+-rw-r--r--   0 mdalchen   (501) staff       (20)        1 2023-07-24 13:20:04.000000 pyrdams-2.1.3/pyrdams.egg-info/dependency_links.txt
+-rw-r--r--   0 mdalchen   (501) staff       (20)       44 2023-07-24 13:20:04.000000 pyrdams-2.1.3/pyrdams.egg-info/entry_points.txt
+-rw-r--r--   0 mdalchen   (501) staff       (20)        9 2023-07-24 13:20:04.000000 pyrdams-2.1.3/pyrdams.egg-info/requires.txt
+-rw-r--r--   0 mdalchen   (501) staff       (20)       13 2023-07-24 13:20:04.000000 pyrdams-2.1.3/pyrdams.egg-info/top_level.txt
+-rwxr-xr-x   0 mdalchen   (501) staff       (20)    20096 2023-07-24 13:15:59.000000 pyrdams-2.1.3/rdams_client.py
+-rw-r--r--   0 mdalchen   (501) staff       (20)       38 2023-07-24 13:20:04.187746 pyrdams-2.1.3/setup.cfg
```

### Comparing `pyrdams-2.1.2/PKG-INFO` & `pyrdams-2.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrdams
-Version: 2.1.2
+Version: 2.1.3
 Summary: Research Data Archive (RDA) python client
 Author-email: Doug Schuster <schuster@ucar.edu>, Riley Conroy <rpconroy@ucar.edu>, Mykhailo Dalchenko <mykhailo.dalchenko@cta-consortium.org>
 Project-URL: Home, https://github.com/NCAR/rda-apps-clients
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 
 # `rdams` for Python
```

### Comparing `pyrdams-2.1.2/README.md` & `pyrdams-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyrdams-2.1.2/pyproject.toml` & `pyrdams-2.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyrdams-2.1.2/pyrdams.egg-info/PKG-INFO` & `pyrdams-2.1.3/pyrdams.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrdams
-Version: 2.1.2
+Version: 2.1.3
 Summary: Research Data Archive (RDA) python client
 Author-email: Doug Schuster <schuster@ucar.edu>, Riley Conroy <rpconroy@ucar.edu>, Mykhailo Dalchenko <mykhailo.dalchenko@cta-consortium.org>
 Project-URL: Home, https://github.com/NCAR/rda-apps-clients
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 
 # `rdams` for Python
```

### Comparing `pyrdams-2.1.2/rdams_client.py` & `pyrdams-2.1.3/rdams_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 rdams -download [RequestIndex]
 rdams -globus_download [RequestIndex]
 rdams -get_control_file_template <dsnnn.n>
 rdams -help
 ```
 """
 
-__version__ = '2.1.2'
+__version__ = '2.1.3'
 __author__ = 'Doug Schuster (schuster@ucar.edu), Riley Conroy (rpconroy@ucar.edu), Mykhailo Dalchenko (mykhailo.dalchenko@cta-consortium.org)'
 
 import sys
 import os
 import requests
 import getpass
 import json
@@ -556,29 +556,29 @@
 
     Args:
         request_idx (str): Request Index, typically a 6-digit integer.
 
     Returns:
         None
     """
-    ret = get_filelist(request_idx)
+    ret = get_filelist(request_idx, out_dir='./')
     if ret['status'] != 'ok':
         return ret
 
     filelist = ret['result']['web_files']
 
     user_auth = get_authentication()
 
     username, password = user_auth
     cookies = get_cookies(username, password)
 
     web_files = list(map(lambda x: x['web_path'], filelist))
 
     # Only download unique files.
-    download_files(set(web_files))
+    download_files(set(web_files), out_dir=out_dir)
     return ret
 
 
 def globus_download(request_idx):
     """Begin a globus transfer.
 
     Args:
```

