# Comparing `tmp/chungus-0.0.0.tar.gz` & `tmp/chungus-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chungus-0.0.0.tar", last modified: Sat Jul 22 20:16:58 2023, max compression
+gzip compressed data, was "chungus-1.0.0.tar", last modified: Mon Jul 24 03:14:32 2023, max compression
```

## Comparing `chungus-0.0.0.tar` & `chungus-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 20:16:58.941261 chungus-0.0.0/
--rw-rw-rw-   0        0        0      790 2023-07-22 20:10:44.000000 chungus-0.0.0/LICENSE
--rw-rw-rw-   0        0        0     3070 2023-07-22 20:16:58.936208 chungus-0.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-22 20:16:58.832708 chungus-0.0.0/chungus/
--rw-rw-rw-   0        0        0        0 2023-07-16 00:51:01.000000 chungus-0.0.0/chungus/__init__.py
--rw-rw-rw-   0        0        0     7876 2023-07-22 20:05:43.000000 chungus-0.0.0/chungus/chungus.py
-drwxrwxrwx   0        0        0        0 2023-07-22 20:16:58.933209 chungus-0.0.0/chungus.egg-info/
--rw-rw-rw-   0        0        0     3070 2023-07-22 20:16:58.000000 chungus-0.0.0/chungus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      179 2023-07-22 20:16:58.000000 chungus-0.0.0/chungus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 20:16:58.000000 chungus-0.0.0/chungus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-22 20:16:58.000000 chungus-0.0.0/chungus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-22 20:16:58.943261 chungus-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0      593 2023-07-22 20:16:40.000000 chungus-0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 03:14:31.982571 chungus-1.0.0/
+-rw-rw-rw-   0        0        0      790 2023-07-22 20:10:44.000000 chungus-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     3077 2023-07-24 03:14:31.981565 chungus-1.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-24 03:14:31.808898 chungus-1.0.0/chungus/
+-rw-rw-rw-   0        0        0        0 2023-07-16 00:51:01.000000 chungus-1.0.0/chungus/__init__.py
+-rw-rw-rw-   0        0        0     9919 2023-07-24 03:12:08.000000 chungus-1.0.0/chungus/chungus.py
+drwxrwxrwx   0        0        0        0 2023-07-24 03:14:31.977562 chungus-1.0.0/chungus.egg-info/
+-rw-rw-rw-   0        0        0     3077 2023-07-24 03:14:30.000000 chungus-1.0.0/chungus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      179 2023-07-24 03:14:31.000000 chungus-1.0.0/chungus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 03:14:30.000000 chungus-1.0.0/chungus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-24 03:14:30.000000 chungus-1.0.0/chungus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 03:14:31.983564 chungus-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      600 2023-07-24 03:12:56.000000 chungus-1.0.0/setup.py
```

### Comparing `chungus-0.0.0/LICENSE` & `chungus-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chungus-0.0.0/PKG-INFO` & `chungus-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: chungus
-Version: 0.0.0
-Summary: Chunky Module
+Version: 1.0.0
+Summary: Updated, more chunky
 Author: PyModuleDev
 Author-email: pxcom@mail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `chungus-0.0.0/chungus.egg-info/PKG-INFO` & `chungus-1.0.0/chungus.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: chungus
-Version: 0.0.0
-Summary: Chunky Module
+Version: 1.0.0
+Summary: Updated, more chunky
 Author: PyModuleDev
 Author-email: pxcom@mail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `chungus-0.0.0/setup.py` & `chungus-1.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup
 
 with open("READ.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="chungus",
-    version="0.0.0",
+    version="1.0.0",
     author="PyModuleDev",
     author_email="pxcom@mail.com",
-    description="Chunky Module",
+    description="Updated, more chunky",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["chungus"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3"
```

