# Comparing `tmp/elsdk-0.1.1.tar.gz` & `tmp/elsdk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elsdk-0.1.1.tar", last modified: Mon Jul 24 13:39:58 2023, max compression
+gzip compressed data, was "elsdk-0.1.2.tar", last modified: Mon Jul 24 13:43:21 2023, max compression
```

## Comparing `elsdk-0.1.1.tar` & `elsdk-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 reset      (501) staff       (20)        0 2023-07-24 13:39:58.717990 elsdk-0.1.1/
--rw-r--r--   0 reset      (501) staff       (20)      286 2023-07-24 13:39:58.718074 elsdk-0.1.1/PKG-INFO
--rw-r--r--   0 reset      (501) staff       (20)      310 2023-07-24 13:38:42.000000 elsdk-0.1.1/README.md
--rw-r--r--   0 reset      (501) staff       (20)      863 2023-07-24 13:39:58.718887 elsdk-0.1.1/setup.cfg
--rw-r--r--   0 reset      (501) staff       (20)      666 2023-07-24 13:39:24.000000 elsdk-0.1.1/setup.py
-drwxr-xr-x   0 reset      (501) staff       (20)        0 2023-07-24 13:39:58.713607 elsdk-0.1.1/src/
-drwxr-xr-x   0 reset      (501) staff       (20)        0 2023-07-24 13:39:58.715897 elsdk-0.1.1/src/elsdk/
--rw-r--r--   0 reset      (501) staff       (20)      390 2023-07-24 09:36:37.000000 elsdk-0.1.1/src/elsdk/__init__.py
--rw-r--r--   0 reset      (501) staff       (20)      726 2023-07-24 09:41:39.000000 elsdk-0.1.1/src/elsdk/events.py
--rw-r--r--   0 reset      (501) staff       (20)       80 2023-07-24 09:00:49.000000 elsdk-0.1.1/src/elsdk/infra.py
--rw-r--r--   0 reset      (501) staff       (20)      305 2023-07-24 09:41:39.000000 elsdk-0.1.1/src/elsdk/invite.py
--rw-r--r--   0 reset      (501) staff       (20)      361 2023-07-24 09:41:39.000000 elsdk-0.1.1/src/elsdk/session.py
--rw-r--r--   0 reset      (501) staff       (20)       80 2023-07-24 09:41:39.000000 elsdk-0.1.1/src/elsdk/state.py
-drwxr-xr-x   0 reset      (501) staff       (20)        0 2023-07-24 13:39:58.717743 elsdk-0.1.1/src/elsdk/utils/
--rw-r--r--   0 reset      (501) staff       (20)        0 2023-07-24 09:03:52.000000 elsdk-0.1.1/src/elsdk/utils/__init__.py
--rw-r--r--   0 reset      (501) staff       (20)        0 2023-07-24 08:56:33.000000 elsdk-0.1.1/src/elsdk/utils/common.py
--rw-r--r--   0 reset      (501) staff       (20)      617 2023-07-24 09:06:31.000000 elsdk-0.1.1/src/elsdk/utils/exceptions.py
--rw-r--r--   0 reset      (501) staff       (20)     1158 2023-07-24 08:36:45.000000 elsdk-0.1.1/src/elsdk/utils/log.py
-drwxr-xr-x   0 reset      (501) staff       (20)        0 2023-07-24 13:39:58.717056 elsdk-0.1.1/src/elsdk.egg-info/
--rw-r--r--   0 reset      (501) staff       (20)      286 2023-07-24 13:39:58.000000 elsdk-0.1.1/src/elsdk.egg-info/PKG-INFO
--rw-r--r--   0 reset      (501) staff       (20)      452 2023-07-24 13:39:58.000000 elsdk-0.1.1/src/elsdk.egg-info/SOURCES.txt
--rw-r--r--   0 reset      (501) staff       (20)        1 2023-07-24 13:39:58.000000 elsdk-0.1.1/src/elsdk.egg-info/dependency_links.txt
--rw-r--r--   0 reset      (501) staff       (20)        1 2023-07-24 08:44:10.000000 elsdk-0.1.1/src/elsdk.egg-info/not-zip-safe
--rw-r--r--   0 reset      (501) staff       (20)      100 2023-07-24 13:39:58.000000 elsdk-0.1.1/src/elsdk.egg-info/requires.txt
--rw-r--r--   0 reset      (501) staff       (20)        6 2023-07-24 13:39:58.000000 elsdk-0.1.1/src/elsdk.egg-info/top_level.txt
+drwxr-xr-x   0 reset      (501) staff       (20)        0 2023-07-24 13:43:21.129161 elsdk-0.1.2/
+-rw-r--r--   0 reset      (501) staff       (20)      343 2023-07-24 13:43:21.129232 elsdk-0.1.2/PKG-INFO
+-rw-r--r--   0 reset      (501) staff       (20)      310 2023-07-24 13:38:42.000000 elsdk-0.1.2/README.md
+-rw-r--r--   0 reset      (501) staff       (20)      863 2023-07-24 13:43:21.129718 elsdk-0.1.2/setup.cfg
+-rw-r--r--   0 reset      (501) staff       (20)      748 2023-07-24 13:43:13.000000 elsdk-0.1.2/setup.py
+drwxr-xr-x   0 reset      (501) staff       (20)        0 2023-07-24 13:43:21.124910 elsdk-0.1.2/src/
+drwxr-xr-x   0 reset      (501) staff       (20)        0 2023-07-24 13:43:21.127117 elsdk-0.1.2/src/elsdk/
+-rw-r--r--   0 reset      (501) staff       (20)      390 2023-07-24 09:36:37.000000 elsdk-0.1.2/src/elsdk/__init__.py
+-rw-r--r--   0 reset      (501) staff       (20)      726 2023-07-24 09:41:39.000000 elsdk-0.1.2/src/elsdk/events.py
+-rw-r--r--   0 reset      (501) staff       (20)       80 2023-07-24 09:00:49.000000 elsdk-0.1.2/src/elsdk/infra.py
+-rw-r--r--   0 reset      (501) staff       (20)      305 2023-07-24 09:41:39.000000 elsdk-0.1.2/src/elsdk/invite.py
+-rw-r--r--   0 reset      (501) staff       (20)      361 2023-07-24 09:41:39.000000 elsdk-0.1.2/src/elsdk/session.py
+-rw-r--r--   0 reset      (501) staff       (20)       80 2023-07-24 09:41:39.000000 elsdk-0.1.2/src/elsdk/state.py
+drwxr-xr-x   0 reset      (501) staff       (20)        0 2023-07-24 13:43:21.128931 elsdk-0.1.2/src/elsdk/utils/
+-rw-r--r--   0 reset      (501) staff       (20)        0 2023-07-24 09:03:52.000000 elsdk-0.1.2/src/elsdk/utils/__init__.py
+-rw-r--r--   0 reset      (501) staff       (20)        0 2023-07-24 08:56:33.000000 elsdk-0.1.2/src/elsdk/utils/common.py
+-rw-r--r--   0 reset      (501) staff       (20)      617 2023-07-24 09:06:31.000000 elsdk-0.1.2/src/elsdk/utils/exceptions.py
+-rw-r--r--   0 reset      (501) staff       (20)     1158 2023-07-24 08:36:45.000000 elsdk-0.1.2/src/elsdk/utils/log.py
+drwxr-xr-x   0 reset      (501) staff       (20)        0 2023-07-24 13:43:21.128309 elsdk-0.1.2/src/elsdk.egg-info/
+-rw-r--r--   0 reset      (501) staff       (20)      343 2023-07-24 13:43:21.000000 elsdk-0.1.2/src/elsdk.egg-info/PKG-INFO
+-rw-r--r--   0 reset      (501) staff       (20)      452 2023-07-24 13:43:21.000000 elsdk-0.1.2/src/elsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 reset      (501) staff       (20)        1 2023-07-24 13:43:21.000000 elsdk-0.1.2/src/elsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 reset      (501) staff       (20)        1 2023-07-24 08:44:10.000000 elsdk-0.1.2/src/elsdk.egg-info/not-zip-safe
+-rw-r--r--   0 reset      (501) staff       (20)      100 2023-07-24 13:43:21.000000 elsdk-0.1.2/src/elsdk.egg-info/requires.txt
+-rw-r--r--   0 reset      (501) staff       (20)        6 2023-07-24 13:43:21.000000 elsdk-0.1.2/src/elsdk.egg-info/top_level.txt
```

### Comparing `elsdk-0.1.1/setup.cfg` & `elsdk-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `elsdk-0.1.1/setup.py` & `elsdk-0.1.2/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 # Third Party Library
 from setuptools import find_packages, setup
 
 setup(
     name="elsdk",
-    version="0.1.1",
+    version="0.1.2",
     description="SDK for Scheduling and Managing EL Platform",
     author="EinstonLabs",
     author_email="info@einstonlabs.com",
     keywords="elp,einston,sdk",
     license="All Rights Reserved by Einston Labs",
     url="https://einstonlabs.com",
     python_requires="~=3.8",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     zip_safe=False,
+    project_urls={
+        'Documentation': 'https://docs.einstonlabs.com'
+    },
     install_requires=[
         "requests==2.31.0",
         "pycryptodome==3.18.0",
         "PyJWT==2.7.0",
         "python-dateutil==2.8.2",
         "python-json-logger==2.0.7",
     ]
```

### Comparing `elsdk-0.1.1/src/elsdk/events.py` & `elsdk-0.1.2/src/elsdk/events.py`

 * *Files identical despite different names*

### Comparing `elsdk-0.1.1/src/elsdk/utils/exceptions.py` & `elsdk-0.1.2/src/elsdk/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `elsdk-0.1.1/src/elsdk/utils/log.py` & `elsdk-0.1.2/src/elsdk/utils/log.py`

 * *Files identical despite different names*

