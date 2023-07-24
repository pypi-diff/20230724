# Comparing `tmp/botiverse-0.3.0.tar.gz` & `tmp/botiverse-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botiverse-0.3.0.tar", last modified: Mon Jul 24 15:13:43 2023, max compression
+gzip compressed data, was "botiverse-0.3.1.tar", last modified: Mon Jul 24 15:33:18 2023, max compression
```

## Comparing `botiverse-0.3.0.tar` & `botiverse-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 15:13:43.499618 botiverse-0.3.0/
--rw-r--r--   0 essam      (501) staff       (20)     1192 2023-07-24 15:13:43.499372 botiverse-0.3.0/PKG-INFO
--rw-r--r--   0 essam      (501) staff       (20)      440 2023-01-31 16:00:25.000000 botiverse-0.3.0/README.md
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 15:13:43.496557 botiverse-0.3.0/botiverse/
--rw-r--r--   0 essam      (501) staff       (20)       84 2023-07-24 13:02:25.000000 botiverse-0.3.0/botiverse/__init__.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 15:13:43.498190 botiverse-0.3.0/botiverse/bots/
--rw-r--r--   0 essam      (501) staff       (20)      344 2023-07-24 13:44:29.000000 botiverse-0.3.0/botiverse/bots/__init__.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 15:13:43.498532 botiverse-0.3.0/botiverse/models/
--rw-r--r--   0 essam      (501) staff       (20)      559 2023-07-10 23:47:13.000000 botiverse-0.3.0/botiverse/models/__init__.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 15:13:43.498885 botiverse-0.3.0/botiverse/preprocessors/
--rw-r--r--   0 essam      (501) staff       (20)      584 2023-07-24 06:37:23.000000 botiverse-0.3.0/botiverse/preprocessors/__init__.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 15:13:43.497900 botiverse-0.3.0/botiverse.egg-info/
--rw-r--r--   0 essam      (501) staff       (20)     1192 2023-07-24 15:13:43.000000 botiverse-0.3.0/botiverse.egg-info/PKG-INFO
--rw-r--r--   0 essam      (501) staff       (20)      296 2023-07-24 15:13:43.000000 botiverse-0.3.0/botiverse.egg-info/SOURCES.txt
--rw-r--r--   0 essam      (501) staff       (20)        1 2023-07-24 15:13:43.000000 botiverse-0.3.0/botiverse.egg-info/dependency_links.txt
--rw-r--r--   0 essam      (501) staff       (20)       12 2023-07-24 15:13:43.000000 botiverse-0.3.0/botiverse.egg-info/requires.txt
--rw-r--r--   0 essam      (501) staff       (20)       10 2023-07-24 15:13:43.000000 botiverse-0.3.0/botiverse.egg-info/top_level.txt
--rw-r--r--   0 essam      (501) staff       (20)       38 2023-07-24 15:13:43.499697 botiverse-0.3.0/setup.cfg
--rw-r--r--   0 essam      (501) staff       (20)     1978 2023-07-24 15:13:10.000000 botiverse-0.3.0/setup.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 15:33:18.501734 botiverse-0.3.1/
+-rw-r--r--   0 essam      (501) staff       (20)     1192 2023-07-24 15:33:18.501519 botiverse-0.3.1/PKG-INFO
+-rw-r--r--   0 essam      (501) staff       (20)      440 2023-01-31 16:00:25.000000 botiverse-0.3.1/README.md
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 15:33:18.498078 botiverse-0.3.1/botiverse/
+-rw-r--r--   0 essam      (501) staff       (20)       84 2023-07-24 13:02:25.000000 botiverse-0.3.1/botiverse/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 15:33:18.499255 botiverse-0.3.1/botiverse/bots/
+-rw-r--r--   0 essam      (501) staff       (20)      407 2023-07-24 15:31:32.000000 botiverse-0.3.1/botiverse/bots/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 15:33:18.499822 botiverse-0.3.1/botiverse/gui/
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-02 09:46:31.000000 botiverse-0.3.1/botiverse/gui/__init__.py
+-rw-r--r--   0 essam      (501) staff       (20)     1004 2023-07-24 13:02:01.000000 botiverse-0.3.1/botiverse/gui/gui.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 15:33:18.500188 botiverse-0.3.1/botiverse/models/
+-rw-r--r--   0 essam      (501) staff       (20)      559 2023-07-10 23:47:13.000000 botiverse-0.3.1/botiverse/models/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 15:33:18.500853 botiverse-0.3.1/botiverse/preprocessors/
+-rw-r--r--   0 essam      (501) staff       (20)      584 2023-07-24 06:37:23.000000 botiverse-0.3.1/botiverse/preprocessors/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 15:33:18.499078 botiverse-0.3.1/botiverse.egg-info/
+-rw-r--r--   0 essam      (501) staff       (20)     1192 2023-07-24 15:33:18.000000 botiverse-0.3.1/botiverse.egg-info/PKG-INFO
+-rw-r--r--   0 essam      (501) staff       (20)      343 2023-07-24 15:33:18.000000 botiverse-0.3.1/botiverse.egg-info/SOURCES.txt
+-rw-r--r--   0 essam      (501) staff       (20)        1 2023-07-24 15:33:18.000000 botiverse-0.3.1/botiverse.egg-info/dependency_links.txt
+-rw-r--r--   0 essam      (501) staff       (20)       12 2023-07-24 15:33:18.000000 botiverse-0.3.1/botiverse.egg-info/requires.txt
+-rw-r--r--   0 essam      (501) staff       (20)       10 2023-07-24 15:33:18.000000 botiverse-0.3.1/botiverse.egg-info/top_level.txt
+-rw-r--r--   0 essam      (501) staff       (20)       38 2023-07-24 15:33:18.501804 botiverse-0.3.1/setup.cfg
+-rw-r--r--   0 essam      (501) staff       (20)     1995 2023-07-24 15:33:07.000000 botiverse-0.3.1/setup.py
```

### Comparing `botiverse-0.3.0/PKG-INFO` & `botiverse-0.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botiverse
-Version: 0.3.0
+Version: 0.3.1
 Summary: botiverse is a chatbot library that offers a high-level API to
 Home-page: https://botiverse.readthedocs.io/
 Author: Essam W., Mohamed Saad, Yousef Atef, Karim Taha
 Author-email: essamwisam@outlook.com
 License: GPLv3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `botiverse-0.3.0/botiverse/models/__init__.py` & `botiverse-0.3.1/botiverse/models/__init__.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.0/botiverse/preprocessors/__init__.py` & `botiverse-0.3.1/botiverse/preprocessors/__init__.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.0/botiverse.egg-info/PKG-INFO` & `botiverse-0.3.1/botiverse.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botiverse
-Version: 0.3.0
+Version: 0.3.1
 Summary: botiverse is a chatbot library that offers a high-level API to
 Home-page: https://botiverse.readthedocs.io/
 Author: Essam W., Mohamed Saad, Yousef Atef, Karim Taha
 Author-email: essamwisam@outlook.com
 License: GPLv3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `botiverse-0.3.0/setup.py` & `botiverse-0.3.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     readme = f.read()
 
 # This call to setup() does all the work
 setup(
     name="botiverse",
-    version="0.3.0",
+    version="0.3.1",
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
-    packages=["botiverse", "botiverse.bots", "botiverse.models", "botiverse.preprocessors"],
+    packages=["botiverse", "botiverse.bots", "botiverse.models", "botiverse.preprocessors", "botiverse.gui"],
     include_package_data=True,
     install_requires=["numpy", "torch"]            # just as was in requirements.txt
 )
 
 
 # Steps to upload to PyPI
 # 0 - Increment the version number in setup.py
```

