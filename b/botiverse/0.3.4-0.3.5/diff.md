# Comparing `tmp/botiverse-0.3.4.tar.gz` & `tmp/botiverse-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botiverse-0.3.4.tar", last modified: Mon Jul 24 16:00:16 2023, max compression
+gzip compressed data, was "botiverse-0.3.5.tar", last modified: Mon Jul 24 16:23:43 2023, max compression
```

## Comparing `botiverse-0.3.4.tar` & `botiverse-0.3.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 16:00:16.867712 botiverse-0.3.4/
--rw-r--r--   0 essam      (501) staff       (20)     1192 2023-07-24 16:00:16.867494 botiverse-0.3.4/PKG-INFO
--rw-r--r--   0 essam      (501) staff       (20)      440 2023-01-31 16:00:25.000000 botiverse-0.3.4/README.md
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 16:00:16.863877 botiverse-0.3.4/botiverse/
--rw-r--r--   0 essam      (501) staff       (20)       84 2023-07-24 15:57:44.000000 botiverse-0.3.4/botiverse/__init__.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 16:00:16.865314 botiverse-0.3.4/botiverse/bots/
--rw-r--r--   0 essam      (501) staff       (20)      407 2023-07-24 15:31:32.000000 botiverse-0.3.4/botiverse/bots/__init__.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 16:00:16.865785 botiverse-0.3.4/botiverse/gui/
--rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-02 09:46:31.000000 botiverse-0.3.4/botiverse/gui/__init__.py
--rw-r--r--   0 essam      (501) staff       (20)     1004 2023-07-24 13:02:01.000000 botiverse-0.3.4/botiverse/gui/gui.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 16:00:16.866358 botiverse-0.3.4/botiverse/models/
--rw-r--r--   0 essam      (501) staff       (20)      559 2023-07-10 23:47:13.000000 botiverse-0.3.4/botiverse/models/__init__.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 16:00:16.866763 botiverse-0.3.4/botiverse/preprocessors/
--rw-r--r--   0 essam      (501) staff       (20)      584 2023-07-24 06:37:23.000000 botiverse-0.3.4/botiverse/preprocessors/__init__.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 16:00:16.865043 botiverse-0.3.4/botiverse.egg-info/
--rw-r--r--   0 essam      (501) staff       (20)     1192 2023-07-24 16:00:16.000000 botiverse-0.3.4/botiverse.egg-info/PKG-INFO
--rw-r--r--   0 essam      (501) staff       (20)      343 2023-07-24 16:00:16.000000 botiverse-0.3.4/botiverse.egg-info/SOURCES.txt
--rw-r--r--   0 essam      (501) staff       (20)        1 2023-07-24 16:00:16.000000 botiverse-0.3.4/botiverse.egg-info/dependency_links.txt
--rw-r--r--   0 essam      (501) staff       (20)       12 2023-07-24 16:00:16.000000 botiverse-0.3.4/botiverse.egg-info/requires.txt
--rw-r--r--   0 essam      (501) staff       (20)       10 2023-07-24 16:00:16.000000 botiverse-0.3.4/botiverse.egg-info/top_level.txt
--rw-r--r--   0 essam      (501) staff       (20)       38 2023-07-24 16:00:16.867783 botiverse-0.3.4/setup.cfg
--rw-r--r--   0 essam      (501) staff       (20)     1995 2023-07-24 16:00:05.000000 botiverse-0.3.4/setup.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 16:23:43.420411 botiverse-0.3.5/
+-rw-r--r--   0 essam      (501) staff       (20)     1192 2023-07-24 16:23:43.420182 botiverse-0.3.5/PKG-INFO
+-rw-r--r--   0 essam      (501) staff       (20)      440 2023-01-31 16:00:25.000000 botiverse-0.3.5/README.md
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 16:23:43.416896 botiverse-0.3.5/botiverse/
+-rw-r--r--   0 essam      (501) staff       (20)       84 2023-07-24 15:57:44.000000 botiverse-0.3.5/botiverse/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 16:23:43.418365 botiverse-0.3.5/botiverse/bots/
+-rw-r--r--   0 essam      (501) staff       (20)      407 2023-07-24 15:31:32.000000 botiverse-0.3.5/botiverse/bots/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 16:23:43.418882 botiverse-0.3.5/botiverse/gui/
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-02 09:46:31.000000 botiverse-0.3.5/botiverse/gui/__init__.py
+-rw-r--r--   0 essam      (501) staff       (20)     1004 2023-07-24 13:02:01.000000 botiverse-0.3.5/botiverse/gui/gui.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 16:23:43.419255 botiverse-0.3.5/botiverse/models/
+-rw-r--r--   0 essam      (501) staff       (20)      559 2023-07-10 23:47:13.000000 botiverse-0.3.5/botiverse/models/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 16:23:43.419636 botiverse-0.3.5/botiverse/preprocessors/
+-rw-r--r--   0 essam      (501) staff       (20)      584 2023-07-24 06:37:23.000000 botiverse-0.3.5/botiverse/preprocessors/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 16:23:43.418142 botiverse-0.3.5/botiverse.egg-info/
+-rw-r--r--   0 essam      (501) staff       (20)     1192 2023-07-24 16:23:43.000000 botiverse-0.3.5/botiverse.egg-info/PKG-INFO
+-rw-r--r--   0 essam      (501) staff       (20)      343 2023-07-24 16:23:43.000000 botiverse-0.3.5/botiverse.egg-info/SOURCES.txt
+-rw-r--r--   0 essam      (501) staff       (20)        1 2023-07-24 16:23:43.000000 botiverse-0.3.5/botiverse.egg-info/dependency_links.txt
+-rw-r--r--   0 essam      (501) staff       (20)       12 2023-07-24 16:23:43.000000 botiverse-0.3.5/botiverse.egg-info/requires.txt
+-rw-r--r--   0 essam      (501) staff       (20)       10 2023-07-24 16:23:43.000000 botiverse-0.3.5/botiverse.egg-info/top_level.txt
+-rw-r--r--   0 essam      (501) staff       (20)       38 2023-07-24 16:23:43.420488 botiverse-0.3.5/setup.cfg
+-rw-r--r--   0 essam      (501) staff       (20)     2208 2023-07-24 16:23:39.000000 botiverse-0.3.5/setup.py
```

### Comparing `botiverse-0.3.4/PKG-INFO` & `botiverse-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botiverse
-Version: 0.3.4
+Version: 0.3.5
 Summary: botiverse is a chatbot library that offers a high-level API to
 Home-page: https://botiverse.readthedocs.io/
 Author: Essam W., Mohamed Saad, Yousef Atef, Karim Taha
 Author-email: essamwisam@outlook.com
 License: GPLv3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `botiverse-0.3.4/botiverse/gui/gui.py` & `botiverse-0.3.5/botiverse/gui/gui.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.4/botiverse/models/__init__.py` & `botiverse-0.3.5/botiverse/models/__init__.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.4/botiverse/preprocessors/__init__.py` & `botiverse-0.3.5/botiverse/preprocessors/__init__.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.4/botiverse.egg-info/PKG-INFO` & `botiverse-0.3.5/botiverse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botiverse
-Version: 0.3.4
+Version: 0.3.5
 Summary: botiverse is a chatbot library that offers a high-level API to
 Home-page: https://botiverse.readthedocs.io/
 Author: Essam W., Mohamed Saad, Yousef Atef, Karim Taha
 Author-email: essamwisam@outlook.com
 License: GPLv3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

