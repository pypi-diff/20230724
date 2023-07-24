# Comparing `tmp/botiverse-0.1.0.tar.gz` & `tmp/botiverse-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botiverse-0.1.0.tar", last modified: Sat Jul  1 14:09:51 2023, max compression
+gzip compressed data, was "botiverse-0.3.0.tar", last modified: Mon Jul 24 15:13:43 2023, max compression
```

## Comparing `botiverse-0.1.0.tar` & `botiverse-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,19 @@
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-01 14:09:51.829900 botiverse-0.1.0/
--rw-r--r--   0 essam      (501) staff       (20)     1192 2023-07-01 14:09:51.829734 botiverse-0.1.0/PKG-INFO
--rw-r--r--   0 essam      (501) staff       (20)      440 2023-01-31 16:00:25.000000 botiverse-0.1.0/README.md
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-01 14:09:51.826509 botiverse-0.1.0/botiverse/
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-01 14:09:51.828760 botiverse-0.1.0/botiverse/TODS/
--rw-r--r--   0 essam      (501) staff       (20)      977 2023-07-01 06:07:26.000000 botiverse-0.1.0/botiverse/TODS/DNN_TODS.py
--rw-r--r--   0 essam      (501) staff       (20)     4080 2023-07-01 06:07:26.000000 botiverse-0.1.0/botiverse/TODS/TODS.py
--rw-r--r--   0 essam      (501) staff       (20)        0 2023-01-31 14:19:19.000000 botiverse-0.1.0/botiverse/TODS/__init__.py
--rw-r--r--   0 essam      (501) staff       (20)     1345 2023-07-01 06:07:26.000000 botiverse-0.1.0/botiverse/TODS/tods_example.py
--rw-r--r--   0 essam      (501) staff       (20)     7362 2023-07-01 06:07:26.000000 botiverse-0.1.0/botiverse/TODS/utils.py
--rw-r--r--   0 essam      (501) staff       (20)      762 2023-07-01 06:07:26.000000 botiverse-0.1.0/botiverse/TODS/utils2.py
--rw-r--r--   0 essam      (501) staff       (20)      241 2023-07-01 10:10:18.000000 botiverse-0.1.0/botiverse/__init__.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-01 14:09:51.829485 botiverse-0.1.0/botiverse/basic_chatbot/
--rw-r--r--   0 essam      (501) staff       (20)        0 2023-01-31 14:19:10.000000 botiverse-0.1.0/botiverse/basic_chatbot/__init__.py
--rw-r--r--   0 essam      (501) staff       (20)     1099 2023-02-06 15:33:14.000000 botiverse-0.1.0/botiverse/basic_chatbot/basic_chatbot.py
--rw-r--r--   0 essam      (501) staff       (20)       35 2023-02-06 15:31:49.000000 botiverse-0.1.0/botiverse/basic_chatbot/utils.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-01 14:09:51.827394 botiverse-0.1.0/botiverse.egg-info/
--rw-r--r--   0 essam      (501) staff       (20)     1192 2023-07-01 14:09:51.000000 botiverse-0.1.0/botiverse.egg-info/PKG-INFO
--rw-r--r--   0 essam      (501) staff       (20)      471 2023-07-01 14:09:51.000000 botiverse-0.1.0/botiverse.egg-info/SOURCES.txt
--rw-r--r--   0 essam      (501) staff       (20)        1 2023-07-01 14:09:51.000000 botiverse-0.1.0/botiverse.egg-info/dependency_links.txt
--rw-r--r--   0 essam      (501) staff       (20)       12 2023-07-01 14:09:51.000000 botiverse-0.1.0/botiverse.egg-info/requires.txt
--rw-r--r--   0 essam      (501) staff       (20)       10 2023-07-01 14:09:51.000000 botiverse-0.1.0/botiverse.egg-info/top_level.txt
--rw-r--r--   0 essam      (501) staff       (20)       38 2023-07-01 14:09:51.829951 botiverse-0.1.0/setup.cfg
--rw-r--r--   0 essam      (501) staff       (20)     1958 2023-07-01 14:07:32.000000 botiverse-0.1.0/setup.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 15:13:43.499618 botiverse-0.3.0/
+-rw-r--r--   0 essam      (501) staff       (20)     1192 2023-07-24 15:13:43.499372 botiverse-0.3.0/PKG-INFO
+-rw-r--r--   0 essam      (501) staff       (20)      440 2023-01-31 16:00:25.000000 botiverse-0.3.0/README.md
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 15:13:43.496557 botiverse-0.3.0/botiverse/
+-rw-r--r--   0 essam      (501) staff       (20)       84 2023-07-24 13:02:25.000000 botiverse-0.3.0/botiverse/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 15:13:43.498190 botiverse-0.3.0/botiverse/bots/
+-rw-r--r--   0 essam      (501) staff       (20)      344 2023-07-24 13:44:29.000000 botiverse-0.3.0/botiverse/bots/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 15:13:43.498532 botiverse-0.3.0/botiverse/models/
+-rw-r--r--   0 essam      (501) staff       (20)      559 2023-07-10 23:47:13.000000 botiverse-0.3.0/botiverse/models/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 15:13:43.498885 botiverse-0.3.0/botiverse/preprocessors/
+-rw-r--r--   0 essam      (501) staff       (20)      584 2023-07-24 06:37:23.000000 botiverse-0.3.0/botiverse/preprocessors/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 15:13:43.497900 botiverse-0.3.0/botiverse.egg-info/
+-rw-r--r--   0 essam      (501) staff       (20)     1192 2023-07-24 15:13:43.000000 botiverse-0.3.0/botiverse.egg-info/PKG-INFO
+-rw-r--r--   0 essam      (501) staff       (20)      296 2023-07-24 15:13:43.000000 botiverse-0.3.0/botiverse.egg-info/SOURCES.txt
+-rw-r--r--   0 essam      (501) staff       (20)        1 2023-07-24 15:13:43.000000 botiverse-0.3.0/botiverse.egg-info/dependency_links.txt
+-rw-r--r--   0 essam      (501) staff       (20)       12 2023-07-24 15:13:43.000000 botiverse-0.3.0/botiverse.egg-info/requires.txt
+-rw-r--r--   0 essam      (501) staff       (20)       10 2023-07-24 15:13:43.000000 botiverse-0.3.0/botiverse.egg-info/top_level.txt
+-rw-r--r--   0 essam      (501) staff       (20)       38 2023-07-24 15:13:43.499697 botiverse-0.3.0/setup.cfg
+-rw-r--r--   0 essam      (501) staff       (20)     1978 2023-07-24 15:13:10.000000 botiverse-0.3.0/setup.py
```

### Comparing `botiverse-0.1.0/PKG-INFO` & `botiverse-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botiverse
-Version: 0.1.0
+Version: 0.3.0
 Summary: botiverse is a chatbot library that offers a high-level API to
 Home-page: https://botiverse.readthedocs.io/
 Author: Essam W., Mohamed Saad, Yousef Atef, Karim Taha
 Author-email: essamwisam@outlook.com
 License: GPLv3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `botiverse-0.1.0/botiverse.egg-info/PKG-INFO` & `botiverse-0.3.0/botiverse.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botiverse
-Version: 0.1.0
+Version: 0.3.0
 Summary: botiverse is a chatbot library that offers a high-level API to
 Home-page: https://botiverse.readthedocs.io/
 Author: Essam W., Mohamed Saad, Yousef Atef, Karim Taha
 Author-email: essamwisam@outlook.com
 License: GPLv3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `botiverse-0.1.0/setup.py` & `botiverse-0.3.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     readme = f.read()
 
 # This call to setup() does all the work
 setup(
     name="botiverse",
-    version="0.1.0",
+    version="0.3.0",
     description='''botiverse is a chatbot library that offers a high-level API to
     access a diverse set of chatbot models''',
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://botiverse.readthedocs.io/",
     author="Essam W., Mohamed Saad, Yousef Atef, Karim Taha",
     author_email="essamwisam@outlook.com",
@@ -37,15 +37,15 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Operating System :: OS Independent"
     ],
-    packages=["botiverse", "botiverse.basic_chatbot", "botiverse.TODS"],
+    packages=["botiverse", "botiverse.bots", "botiverse.models", "botiverse.preprocessors"],
     include_package_data=True,
     install_requires=["numpy", "torch"]            # just as was in requirements.txt
 )
 
 
 # Steps to upload to PyPI
 # 0 - Increment the version number in setup.py
```

