# Comparing `tmp/botiverse-0.3.1.tar.gz` & `tmp/botiverse-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botiverse-0.3.1.tar", last modified: Mon Jul 24 15:33:18 2023, max compression
+gzip compressed data, was "botiverse-0.3.2.tar", last modified: Mon Jul 24 15:37:26 2023, max compression
```

## Comparing `botiverse-0.3.1.tar` & `botiverse-0.3.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 15:33:18.501734 botiverse-0.3.1/
--rw-r--r--   0 essam      (501) staff       (20)     1192 2023-07-24 15:33:18.501519 botiverse-0.3.1/PKG-INFO
--rw-r--r--   0 essam      (501) staff       (20)      440 2023-01-31 16:00:25.000000 botiverse-0.3.1/README.md
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 15:33:18.498078 botiverse-0.3.1/botiverse/
--rw-r--r--   0 essam      (501) staff       (20)       84 2023-07-24 13:02:25.000000 botiverse-0.3.1/botiverse/__init__.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 15:33:18.499255 botiverse-0.3.1/botiverse/bots/
--rw-r--r--   0 essam      (501) staff       (20)      407 2023-07-24 15:31:32.000000 botiverse-0.3.1/botiverse/bots/__init__.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 15:33:18.499822 botiverse-0.3.1/botiverse/gui/
--rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-02 09:46:31.000000 botiverse-0.3.1/botiverse/gui/__init__.py
--rw-r--r--   0 essam      (501) staff       (20)     1004 2023-07-24 13:02:01.000000 botiverse-0.3.1/botiverse/gui/gui.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 15:33:18.500188 botiverse-0.3.1/botiverse/models/
--rw-r--r--   0 essam      (501) staff       (20)      559 2023-07-10 23:47:13.000000 botiverse-0.3.1/botiverse/models/__init__.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 15:33:18.500853 botiverse-0.3.1/botiverse/preprocessors/
--rw-r--r--   0 essam      (501) staff       (20)      584 2023-07-24 06:37:23.000000 botiverse-0.3.1/botiverse/preprocessors/__init__.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 15:33:18.499078 botiverse-0.3.1/botiverse.egg-info/
--rw-r--r--   0 essam      (501) staff       (20)     1192 2023-07-24 15:33:18.000000 botiverse-0.3.1/botiverse.egg-info/PKG-INFO
--rw-r--r--   0 essam      (501) staff       (20)      343 2023-07-24 15:33:18.000000 botiverse-0.3.1/botiverse.egg-info/SOURCES.txt
--rw-r--r--   0 essam      (501) staff       (20)        1 2023-07-24 15:33:18.000000 botiverse-0.3.1/botiverse.egg-info/dependency_links.txt
--rw-r--r--   0 essam      (501) staff       (20)       12 2023-07-24 15:33:18.000000 botiverse-0.3.1/botiverse.egg-info/requires.txt
--rw-r--r--   0 essam      (501) staff       (20)       10 2023-07-24 15:33:18.000000 botiverse-0.3.1/botiverse.egg-info/top_level.txt
--rw-r--r--   0 essam      (501) staff       (20)       38 2023-07-24 15:33:18.501804 botiverse-0.3.1/setup.cfg
--rw-r--r--   0 essam      (501) staff       (20)     1995 2023-07-24 15:33:07.000000 botiverse-0.3.1/setup.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 15:37:26.598798 botiverse-0.3.2/
+-rw-r--r--   0 essam      (501) staff       (20)     1192 2023-07-24 15:37:26.598583 botiverse-0.3.2/PKG-INFO
+-rw-r--r--   0 essam      (501) staff       (20)      440 2023-01-31 16:00:25.000000 botiverse-0.3.2/README.md
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 15:37:26.595636 botiverse-0.3.2/botiverse/
+-rw-r--r--   0 essam      (501) staff       (20)       45 2023-07-24 15:35:41.000000 botiverse-0.3.2/botiverse/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 15:37:26.596815 botiverse-0.3.2/botiverse/bots/
+-rw-r--r--   0 essam      (501) staff       (20)      407 2023-07-24 15:31:32.000000 botiverse-0.3.2/botiverse/bots/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 15:37:26.597274 botiverse-0.3.2/botiverse/gui/
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-02 09:46:31.000000 botiverse-0.3.2/botiverse/gui/__init__.py
+-rw-r--r--   0 essam      (501) staff       (20)     1004 2023-07-24 13:02:01.000000 botiverse-0.3.2/botiverse/gui/gui.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 15:37:26.597685 botiverse-0.3.2/botiverse/models/
+-rw-r--r--   0 essam      (501) staff       (20)      559 2023-07-10 23:47:13.000000 botiverse-0.3.2/botiverse/models/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 15:37:26.598093 botiverse-0.3.2/botiverse/preprocessors/
+-rw-r--r--   0 essam      (501) staff       (20)      584 2023-07-24 06:37:23.000000 botiverse-0.3.2/botiverse/preprocessors/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 15:37:26.596642 botiverse-0.3.2/botiverse.egg-info/
+-rw-r--r--   0 essam      (501) staff       (20)     1192 2023-07-24 15:37:26.000000 botiverse-0.3.2/botiverse.egg-info/PKG-INFO
+-rw-r--r--   0 essam      (501) staff       (20)      343 2023-07-24 15:37:26.000000 botiverse-0.3.2/botiverse.egg-info/SOURCES.txt
+-rw-r--r--   0 essam      (501) staff       (20)        1 2023-07-24 15:37:26.000000 botiverse-0.3.2/botiverse.egg-info/dependency_links.txt
+-rw-r--r--   0 essam      (501) staff       (20)       12 2023-07-24 15:37:26.000000 botiverse-0.3.2/botiverse.egg-info/requires.txt
+-rw-r--r--   0 essam      (501) staff       (20)       10 2023-07-24 15:37:26.000000 botiverse-0.3.2/botiverse.egg-info/top_level.txt
+-rw-r--r--   0 essam      (501) staff       (20)       38 2023-07-24 15:37:26.598871 botiverse-0.3.2/setup.cfg
+-rw-r--r--   0 essam      (501) staff       (20)     1995 2023-07-24 15:37:14.000000 botiverse-0.3.2/setup.py
```

### Comparing `botiverse-0.3.1/PKG-INFO` & `botiverse-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botiverse
-Version: 0.3.1
+Version: 0.3.2
 Summary: botiverse is a chatbot library that offers a high-level API to
 Home-page: https://botiverse.readthedocs.io/
 Author: Essam W., Mohamed Saad, Yousef Atef, Karim Taha
 Author-email: essamwisam@outlook.com
 License: GPLv3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `botiverse-0.3.1/botiverse/gui/gui.py` & `botiverse-0.3.2/botiverse/gui/gui.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.1/botiverse/models/__init__.py` & `botiverse-0.3.2/botiverse/models/__init__.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.1/botiverse/preprocessors/__init__.py` & `botiverse-0.3.2/botiverse/preprocessors/__init__.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.1/botiverse.egg-info/PKG-INFO` & `botiverse-0.3.2/botiverse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botiverse
-Version: 0.3.1
+Version: 0.3.2
 Summary: botiverse is a chatbot library that offers a high-level API to
 Home-page: https://botiverse.readthedocs.io/
 Author: Essam W., Mohamed Saad, Yousef Atef, Karim Taha
 Author-email: essamwisam@outlook.com
 License: GPLv3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `botiverse-0.3.1/setup.py` & `botiverse-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     readme = f.read()
 
 # This call to setup() does all the work
 setup(
     name="botiverse",
-    version="0.3.1",
+    version="0.3.2",
     description='''botiverse is a chatbot library that offers a high-level API to
     access a diverse set of chatbot models''',
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://botiverse.readthedocs.io/",
     author="Essam W., Mohamed Saad, Yousef Atef, Karim Taha",
     author_email="essamwisam@outlook.com",
```

