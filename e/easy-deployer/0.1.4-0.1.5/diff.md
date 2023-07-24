# Comparing `tmp/easy_deployer-0.1.4.tar.gz` & `tmp/easy_deployer-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_deployer-0.1.4.tar", last modified: Mon Jul 24 19:54:09 2023, max compression
+gzip compressed data, was "easy_deployer-0.1.5.tar", last modified: Mon Jul 24 20:09:38 2023, max compression
```

## Comparing `easy_deployer-0.1.4.tar` & `easy_deployer-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 19:54:08.717932 easy_deployer-0.1.4/
--rw-rw-rw-   0        0        0     1086 2021-07-27 13:30:42.000000 easy_deployer-0.1.4/LICENSE.txt
--rw-rw-rw-   0        0        0      888 2023-07-24 19:54:08.716935 easy_deployer-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-07-24 19:18:25.000000 easy_deployer-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-24 19:54:08.698983 easy_deployer-0.1.4/easy_deployer/
--rw-rw-rw-   0        0        0       90 2023-07-24 19:21:46.000000 easy_deployer-0.1.4/easy_deployer/__init__.py
--rw-rw-rw-   0        0        0    26588 2023-07-24 15:55:57.000000 easy_deployer-0.1.4/easy_deployer/github.py
--rw-rw-rw-   0        0        0    11211 2023-07-23 15:15:38.000000 easy_deployer-0.1.4/easy_deployer/heroku.py
--rw-rw-rw-   0        0        0     9304 2023-07-24 19:12:32.000000 easy_deployer-0.1.4/easy_deployer/main.py
--rw-rw-rw-   0        0        0    12360 2023-07-23 15:28:41.000000 easy_deployer-0.1.4/easy_deployer/shared_functions.py
-drwxrwxrwx   0        0        0        0 2023-07-24 19:54:08.715938 easy_deployer-0.1.4/easy_deployer.egg-info/
--rw-rw-rw-   0        0        0      888 2023-07-24 19:54:08.000000 easy_deployer-0.1.4/easy_deployer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-07-24 19:54:08.000000 easy_deployer-0.1.4/easy_deployer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 19:54:08.000000 easy_deployer-0.1.4/easy_deployer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      156 2023-07-24 19:54:08.000000 easy_deployer-0.1.4/easy_deployer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-07-24 19:54:08.000000 easy_deployer-0.1.4/easy_deployer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 19:54:08.718930 easy_deployer-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1424 2023-07-24 19:52:04.000000 easy_deployer-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 20:09:38.195873 easy_deployer-0.1.5/
+-rw-rw-rw-   0        0        0     1086 2021-07-27 13:30:42.000000 easy_deployer-0.1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      910 2023-07-24 20:09:38.193864 easy_deployer-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-07-24 19:18:25.000000 easy_deployer-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 20:09:38.141780 easy_deployer-0.1.5/easy_deployer/
+-rw-rw-rw-   0        0        0       90 2023-07-24 20:04:25.000000 easy_deployer-0.1.5/easy_deployer/__init__.py
+-rw-rw-rw-   0        0        0    26588 2023-07-24 15:55:57.000000 easy_deployer-0.1.5/easy_deployer/github.py
+-rw-rw-rw-   0        0        0    11211 2023-07-23 15:15:38.000000 easy_deployer-0.1.5/easy_deployer/heroku.py
+-rw-rw-rw-   0        0        0     9304 2023-07-24 19:12:32.000000 easy_deployer-0.1.5/easy_deployer/main.py
+-rw-rw-rw-   0        0        0    12360 2023-07-23 15:28:41.000000 easy_deployer-0.1.5/easy_deployer/shared_functions.py
+drwxrwxrwx   0        0        0        0 2023-07-24 20:09:38.154733 easy_deployer-0.1.5/easy_deployer.egg-info/
+-rw-rw-rw-   0        0        0      910 2023-07-24 20:09:38.000000 easy_deployer-0.1.5/easy_deployer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2023-07-24 20:09:38.000000 easy_deployer-0.1.5/easy_deployer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 20:09:38.000000 easy_deployer-0.1.5/easy_deployer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      156 2023-07-24 20:09:38.000000 easy_deployer-0.1.5/easy_deployer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-07-24 20:09:38.000000 easy_deployer-0.1.5/easy_deployer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 20:09:38.196856 easy_deployer-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1456 2023-07-24 20:04:43.000000 easy_deployer-0.1.5/setup.py
```

### Comparing `easy_deployer-0.1.4/LICENSE.txt` & `easy_deployer-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easy_deployer-0.1.4/PKG-INFO` & `easy_deployer-0.1.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: easy_deployer
-Version: 0.1.4
+Version: 0.1.5
+Summary: description
 Home-page: https://github.com/medamine980/easy-deployer
 Author: Mohamed-Amine Benali
 Author-email: benali.medamine2002@gmail.com
 License: MIT
 Keywords: python,github,github-deployer,heroku,heroku-deployer,deploy,easy,easy-deployer,simple,simple-deployer
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `easy_deployer-0.1.4/easy_deployer/github.py` & `easy_deployer-0.1.5/easy_deployer/github.py`

 * *Files identical despite different names*

### Comparing `easy_deployer-0.1.4/easy_deployer/heroku.py` & `easy_deployer-0.1.5/easy_deployer/heroku.py`

 * *Files identical despite different names*

### Comparing `easy_deployer-0.1.4/easy_deployer/main.py` & `easy_deployer-0.1.5/easy_deployer/main.py`

 * *Files identical despite different names*

### Comparing `easy_deployer-0.1.4/easy_deployer/shared_functions.py` & `easy_deployer-0.1.5/easy_deployer/shared_functions.py`

 * *Files identical despite different names*

### Comparing `easy_deployer-0.1.4/easy_deployer.egg-info/PKG-INFO` & `easy_deployer-0.1.5/easy_deployer.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: easy-deployer
-Version: 0.1.4
+Version: 0.1.5
+Summary: description
 Home-page: https://github.com/medamine980/easy-deployer
 Author: Mohamed-Amine Benali
 Author-email: benali.medamine2002@gmail.com
 License: MIT
 Keywords: python,github,github-deployer,heroku,heroku-deployer,deploy,easy,easy-deployer,simple,simple-deployer
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `easy_deployer-0.1.4/setup.py` & `easy_deployer-0.1.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md") as f:
     long_desc = f.read()
 setup(
     name="easy_deployer",
-    version="0.1.4",
+    version="0.1.5",
+    description="description",
     long_description=long_desc,
     long_description_content_type='text/markdown',
     author="Mohamed-Amine Benali",
     author_email="benali.medamine2002@gmail.com",
     url="https://github.com/medamine980/easy-deployer",
     packages=find_packages(exclude=["easy_deployer.dist", "easy_deployer.ignore"]),
     license="MIT",
```

