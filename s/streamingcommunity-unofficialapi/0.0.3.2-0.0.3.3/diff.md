# Comparing `tmp/streamingcommunity_unofficialapi-0.0.3.2.tar.gz` & `tmp/streamingcommunity_unofficialapi-0.0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamingcommunity_unofficialapi-0.0.3.2.tar", last modified: Mon Jul 24 13:09:23 2023, max compression
+gzip compressed data, was "streamingcommunity_unofficialapi-0.0.3.3.tar", last modified: Mon Jul 24 13:14:58 2023, max compression
```

## Comparing `streamingcommunity_unofficialapi-0.0.3.2.tar` & `streamingcommunity_unofficialapi-0.0.3.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:09:23.525708 streamingcommunity_unofficialapi-0.0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-24 13:08:54.000000 streamingcommunity_unofficialapi-0.0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-07-24 13:09:23.525708 streamingcommunity_unofficialapi-0.0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-07-24 13:08:54.000000 streamingcommunity_unofficialapi-0.0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 13:09:23.525708 streamingcommunity_unofficialapi-0.0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-24 13:08:54.000000 streamingcommunity_unofficialapi-0.0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:09:23.525708 streamingcommunity_unofficialapi-0.0.3.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:08:54.000000 streamingcommunity_unofficialapi-0.0.3.2/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7814 2023-07-24 13:08:54.000000 streamingcommunity_unofficialapi-0.0.3.2/src/scuapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:09:23.525708 streamingcommunity_unofficialapi-0.0.3.2/streamingcommunity_unofficialapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-07-24 13:09:23.000000 streamingcommunity_unofficialapi-0.0.3.2/streamingcommunity_unofficialapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-24 13:09:23.000000 streamingcommunity_unofficialapi-0.0.3.2/streamingcommunity_unofficialapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:09:23.000000 streamingcommunity_unofficialapi-0.0.3.2/streamingcommunity_unofficialapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-24 13:09:23.000000 streamingcommunity_unofficialapi-0.0.3.2/streamingcommunity_unofficialapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-24 13:09:23.000000 streamingcommunity_unofficialapi-0.0.3.2/streamingcommunity_unofficialapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:14:58.767580 streamingcommunity_unofficialapi-0.0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-24 13:14:33.000000 streamingcommunity_unofficialapi-0.0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-07-24 13:14:58.767580 streamingcommunity_unofficialapi-0.0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-07-24 13:14:33.000000 streamingcommunity_unofficialapi-0.0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 13:14:58.767580 streamingcommunity_unofficialapi-0.0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-24 13:14:33.000000 streamingcommunity_unofficialapi-0.0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:14:58.767580 streamingcommunity_unofficialapi-0.0.3.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:14:33.000000 streamingcommunity_unofficialapi-0.0.3.3/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7814 2023-07-24 13:14:33.000000 streamingcommunity_unofficialapi-0.0.3.3/src/scuapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:14:58.767580 streamingcommunity_unofficialapi-0.0.3.3/streamingcommunity_unofficialapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-07-24 13:14:58.000000 streamingcommunity_unofficialapi-0.0.3.3/streamingcommunity_unofficialapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-24 13:14:58.000000 streamingcommunity_unofficialapi-0.0.3.3/streamingcommunity_unofficialapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:14:58.000000 streamingcommunity_unofficialapi-0.0.3.3/streamingcommunity_unofficialapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-24 13:14:58.000000 streamingcommunity_unofficialapi-0.0.3.3/streamingcommunity_unofficialapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-24 13:14:58.000000 streamingcommunity_unofficialapi-0.0.3.3/streamingcommunity_unofficialapi.egg-info/top_level.txt
```

### Comparing `streamingcommunity_unofficialapi-0.0.3.2/LICENSE` & `streamingcommunity_unofficialapi-0.0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `streamingcommunity_unofficialapi-0.0.3.2/PKG-INFO` & `streamingcommunity_unofficialapi-0.0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamingcommunity_unofficialapi
-Version: 0.0.3.2
+Version: 0.0.3.3
 Summary: A simple unofficial api for the italian StreamingCommunity website.
 Home-page: https://github.com/Blu-Tiger/streamingcommunity-unofficialapi
 Author: Beqir Stafa
 Author-email: beqirstafa@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `streamingcommunity_unofficialapi-0.0.3.2/README.md` & `streamingcommunity_unofficialapi-0.0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `streamingcommunity_unofficialapi-0.0.3.2/setup.py` & `streamingcommunity_unofficialapi-0.0.3.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,23 +8,18 @@
     author="Beqir Stafa",
     author_email="beqirstafa@gmail.com",
     license='MIT',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Blu-Tiger/streamingcommunity-unofficialapi",
     description="A simple unofficial api for the italian StreamingCommunity website.",
-    version="0.0.3.2",
+    version="0.0.3.3",
     packages=find_packages(),
     install_requires=[
         "setuptools>=61.0",
-        "bs4",
-        "hashlib",
-        "base64",
-        "json",
-        "re",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Topic :: Utilities",
     ],
```

### Comparing `streamingcommunity_unofficialapi-0.0.3.2/src/scuapi.py` & `streamingcommunity_unofficialapi-0.0.3.3/src/scuapi.py`

 * *Files identical despite different names*

### Comparing `streamingcommunity_unofficialapi-0.0.3.2/streamingcommunity_unofficialapi.egg-info/PKG-INFO` & `streamingcommunity_unofficialapi-0.0.3.3/streamingcommunity_unofficialapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamingcommunity-unofficialapi
-Version: 0.0.3.2
+Version: 0.0.3.3
 Summary: A simple unofficial api for the italian StreamingCommunity website.
 Home-page: https://github.com/Blu-Tiger/streamingcommunity-unofficialapi
 Author: Beqir Stafa
 Author-email: beqirstafa@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

