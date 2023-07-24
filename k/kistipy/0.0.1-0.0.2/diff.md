# Comparing `tmp/kistipy-0.0.1.tar.gz` & `tmp/kistipy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kistipy-0.0.1.tar", last modified: Mon Jul 24 06:57:13 2023, max compression
+gzip compressed data, was "kistipy-0.0.2.tar", last modified: Mon Jul 24 07:05:27 2023, max compression
```

## Comparing `kistipy-0.0.1.tar` & `kistipy-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,9 @@
-drwxr-xr-x   0 hmc123     (501) staff       (20)        0 2023-07-24 06:57:13.320946 kistipy-0.0.1/
--rw-r--r--   0 hmc123     (501) staff       (20)     3381 2023-07-24 06:57:13.320554 kistipy-0.0.1/PKG-INFO
--rw-r--r--   0 hmc123     (501) staff       (20)     3014 2023-07-24 04:41:04.000000 kistipy-0.0.1/README.md
-drwxr-xr-x   0 hmc123     (501) staff       (20)        0 2023-07-24 06:57:13.318127 kistipy-0.0.1/kistipy/
--rw-r--r--   0 hmc123     (501) staff       (20)      187 2023-07-17 12:06:24.000000 kistipy-0.0.1/kistipy/__init__.py
-drwxr-xr-x   0 hmc123     (501) staff       (20)        0 2023-07-24 06:57:13.320041 kistipy-0.0.1/kistipy.egg-info/
--rw-r--r--   0 hmc123     (501) staff       (20)     3381 2023-07-24 06:57:12.000000 kistipy-0.0.1/kistipy.egg-info/PKG-INFO
--rw-r--r--   0 hmc123     (501) staff       (20)      162 2023-07-24 06:57:13.000000 kistipy-0.0.1/kistipy.egg-info/SOURCES.txt
--rw-r--r--   0 hmc123     (501) staff       (20)        1 2023-07-24 06:57:12.000000 kistipy-0.0.1/kistipy.egg-info/dependency_links.txt
--rw-r--r--   0 hmc123     (501) staff       (20)        8 2023-07-24 06:57:13.000000 kistipy-0.0.1/kistipy.egg-info/top_level.txt
--rw-r--r--   0 hmc123     (501) staff       (20)       38 2023-07-24 06:57:13.321058 kistipy-0.0.1/setup.cfg
--rw-r--r--   0 hmc123     (501) staff       (20)      568 2023-07-24 06:56:20.000000 kistipy-0.0.1/setup.py
+drwxr-xr-x   0 hmc123     (501) staff       (20)        0 2023-07-24 07:05:27.614865 kistipy-0.0.2/
+-rw-r--r--   0 hmc123     (501) staff       (20)     3381 2023-07-24 07:05:27.614631 kistipy-0.0.2/PKG-INFO
+drwxr-xr-x   0 hmc123     (501) staff       (20)        0 2023-07-24 07:05:27.614314 kistipy-0.0.2/kistipy.egg-info/
+-rw-r--r--   0 hmc123     (501) staff       (20)     3381 2023-07-24 07:05:27.000000 kistipy-0.0.2/kistipy.egg-info/PKG-INFO
+-rw-r--r--   0 hmc123     (501) staff       (20)      132 2023-07-24 07:05:27.000000 kistipy-0.0.2/kistipy.egg-info/SOURCES.txt
+-rw-r--r--   0 hmc123     (501) staff       (20)        1 2023-07-24 07:05:27.000000 kistipy-0.0.2/kistipy.egg-info/dependency_links.txt
+-rw-r--r--   0 hmc123     (501) staff       (20)        1 2023-07-24 07:05:27.000000 kistipy-0.0.2/kistipy.egg-info/top_level.txt
+-rw-r--r--   0 hmc123     (501) staff       (20)       38 2023-07-24 07:05:27.614948 kistipy-0.0.2/setup.cfg
+-rw-r--r--   0 hmc123     (501) staff       (20)      576 2023-07-24 07:05:01.000000 kistipy-0.0.2/setup.py
```

### Comparing `kistipy-0.0.1/PKG-INFO` & `kistipy-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kistipy
-Version: 0.0.1
+Version: 0.0.2
 Summary: kistipy
 Home-page: https://github.com/prosopher/kistipy
 Author: prosopher
 Author-email: prosopher@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `kistipy-0.0.1/README.md` & `kistipy-0.0.2/kistipy.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: kistipy
+Version: 0.0.2
+Summary: kistipy
+Home-page: https://github.com/prosopher/kistipy
+Author: prosopher
+Author-email: prosopher@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9.12
+Description-Content-Type: text/markdown
+
 # kistipy
 
 ![basic-test](https://github.com/prosopher/kistipy/workflows/basic-test/badge.svg)
 
 # Installation
 
 ```python
@@ -90,7 +104,9 @@
 * [특허 분야 자동분류 데이터](https://www.aihub.or.kr/aihubdata/data/view.do?currMenu=115&topMenu=100&aihubDataSe=realm&dataSetSn=547)
 
     - Data 생성
     ```python
     from kistipy import Data
     data = Data(name='특허자동분류', split='train')
     ```
+
+
```

### Comparing `kistipy-0.0.1/setup.py` & `kistipy-0.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
-with open("README.md", "r") as fh:
+with open("kistipy/README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="kistipy",
-    version="0.0.1",
+    version="0.0.2",
     author="prosopher",
     author_email="prosopher@gmail.com",
     description="kistipy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/prosopher/kistipy",
     packages=setuptools.find_packages(),
```

