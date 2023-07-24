# Comparing `tmp/pygination-0.0.8.tar.gz` & `tmp/pygination-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygination-0.0.8.tar", last modified: Thu Feb 10 22:50:45 2022, max compression
+gzip compressed data, was "pygination-0.0.9.tar", last modified: Mon Feb 21 17:29:46 2022, max compression
```

## Comparing `pygination-0.0.8.tar` & `pygination-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 juandanielmorales   (501) staff       (20)        0 2022-02-10 22:50:45.059819 pygination-0.0.8/
--rw-r--r--   0 juandanielmorales   (501) staff       (20)     1061 2022-01-26 13:36:30.000000 pygination-0.0.8/LICENSE.txt
--rw-r--r--   0 juandanielmorales   (501) staff       (20)     1273 2022-02-10 22:50:45.059968 pygination-0.0.8/PKG-INFO
--rw-r--r--   0 juandanielmorales   (501) staff       (20)      638 2022-01-27 16:51:41.000000 pygination-0.0.8/README.md
--rw-r--r--   0 juandanielmorales   (501) staff       (20)       79 2022-02-10 22:50:45.060510 pygination-0.0.8/setup.cfg
--rw-r--r--   0 juandanielmorales   (501) staff       (20)     1755 2022-02-10 22:50:23.000000 pygination-0.0.8/setup.py
-drwxr-xr-x   0 juandanielmorales   (501) staff       (20)        0 2022-02-10 22:50:45.052704 pygination-0.0.8/src/
-drwxr-xr-x   0 juandanielmorales   (501) staff       (20)        0 2022-02-10 22:50:45.056894 pygination-0.0.8/src/pygination/
--rw-r--r--   0 juandanielmorales   (501) staff       (20)       67 2022-01-27 22:46:36.000000 pygination-0.0.8/src/pygination/__init__.py
--rw-r--r--   0 juandanielmorales   (501) staff       (20)       88 2022-01-27 21:49:22.000000 pygination-0.0.8/src/pygination/errors.py
-drwxr-xr-x   0 juandanielmorales   (501) staff       (20)        0 2022-02-10 22:50:45.059545 pygination-0.0.8/src/pygination/models/
--rw-r--r--   0 juandanielmorales   (501) staff       (20)       59 2022-01-27 22:46:36.000000 pygination-0.0.8/src/pygination/models/__init__.py
--rw-r--r--   0 juandanielmorales   (501) staff       (20)      423 2022-01-27 21:49:14.000000 pygination-0.0.8/src/pygination/models/page_model.py
--rw-r--r--   0 juandanielmorales   (501) staff       (20)        0 2022-01-27 22:32:46.000000 pygination-0.0.8/src/pygination/py.typed
--rw-r--r--   0 juandanielmorales   (501) staff       (20)     1819 2022-02-10 22:49:43.000000 pygination-0.0.8/src/pygination/pygination.py
-drwxr-xr-x   0 juandanielmorales   (501) staff       (20)        0 2022-02-10 22:50:45.058934 pygination-0.0.8/src/pygination.egg-info/
--rw-r--r--   0 juandanielmorales   (501) staff       (20)     1273 2022-02-10 22:50:44.000000 pygination-0.0.8/src/pygination.egg-info/PKG-INFO
--rw-r--r--   0 juandanielmorales   (501) staff       (20)      404 2022-02-10 22:50:44.000000 pygination-0.0.8/src/pygination.egg-info/SOURCES.txt
--rw-r--r--   0 juandanielmorales   (501) staff       (20)        1 2022-02-10 22:50:44.000000 pygination-0.0.8/src/pygination.egg-info/dependency_links.txt
--rw-r--r--   0 juandanielmorales   (501) staff       (20)       20 2022-02-10 22:50:44.000000 pygination-0.0.8/src/pygination.egg-info/requires.txt
--rw-r--r--   0 juandanielmorales   (501) staff       (20)       11 2022-02-10 22:50:44.000000 pygination-0.0.8/src/pygination.egg-info/top_level.txt
+drwxr-xr-x   0 juandanielmorales   (501) staff       (20)        0 2022-02-21 17:29:46.946314 pygination-0.0.9/
+-rw-r--r--   0 juandanielmorales   (501) staff       (20)     1061 2022-01-26 13:36:30.000000 pygination-0.0.9/LICENSE.txt
+-rw-r--r--   0 juandanielmorales   (501) staff       (20)     1273 2022-02-21 17:29:46.946434 pygination-0.0.9/PKG-INFO
+-rw-r--r--   0 juandanielmorales   (501) staff       (20)      638 2022-01-27 16:51:41.000000 pygination-0.0.9/README.md
+-rw-r--r--   0 juandanielmorales   (501) staff       (20)       79 2022-02-21 17:29:46.946987 pygination-0.0.9/setup.cfg
+-rw-r--r--   0 juandanielmorales   (501) staff       (20)     1755 2022-02-21 17:28:16.000000 pygination-0.0.9/setup.py
+drwxr-xr-x   0 juandanielmorales   (501) staff       (20)        0 2022-02-21 17:29:46.940331 pygination-0.0.9/src/
+drwxr-xr-x   0 juandanielmorales   (501) staff       (20)        0 2022-02-21 17:29:46.943546 pygination-0.0.9/src/pygination/
+-rw-r--r--   0 juandanielmorales   (501) staff       (20)       67 2022-01-27 22:46:36.000000 pygination-0.0.9/src/pygination/__init__.py
+-rw-r--r--   0 juandanielmorales   (501) staff       (20)       88 2022-01-27 21:49:22.000000 pygination-0.0.9/src/pygination/errors.py
+drwxr-xr-x   0 juandanielmorales   (501) staff       (20)        0 2022-02-21 17:29:46.946066 pygination-0.0.9/src/pygination/models/
+-rw-r--r--   0 juandanielmorales   (501) staff       (20)       59 2022-01-27 22:46:36.000000 pygination-0.0.9/src/pygination/models/__init__.py
+-rw-r--r--   0 juandanielmorales   (501) staff       (20)      423 2022-01-27 21:49:14.000000 pygination-0.0.9/src/pygination/models/page_model.py
+-rw-r--r--   0 juandanielmorales   (501) staff       (20)        0 2022-01-27 22:32:46.000000 pygination-0.0.9/src/pygination/py.typed
+-rw-r--r--   0 juandanielmorales   (501) staff       (20)     1974 2022-02-21 14:39:24.000000 pygination-0.0.9/src/pygination/pygination.py
+drwxr-xr-x   0 juandanielmorales   (501) staff       (20)        0 2022-02-21 17:29:46.945367 pygination-0.0.9/src/pygination.egg-info/
+-rw-r--r--   0 juandanielmorales   (501) staff       (20)     1273 2022-02-21 17:29:46.000000 pygination-0.0.9/src/pygination.egg-info/PKG-INFO
+-rw-r--r--   0 juandanielmorales   (501) staff       (20)      404 2022-02-21 17:29:46.000000 pygination-0.0.9/src/pygination.egg-info/SOURCES.txt
+-rw-r--r--   0 juandanielmorales   (501) staff       (20)        1 2022-02-21 17:29:46.000000 pygination-0.0.9/src/pygination.egg-info/dependency_links.txt
+-rw-r--r--   0 juandanielmorales   (501) staff       (20)       20 2022-02-21 17:29:46.000000 pygination-0.0.9/src/pygination.egg-info/requires.txt
+-rw-r--r--   0 juandanielmorales   (501) staff       (20)       11 2022-02-21 17:29:46.000000 pygination-0.0.9/src/pygination.egg-info/top_level.txt
```

### Comparing `pygination-0.0.8/LICENSE.txt` & `pygination-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pygination-0.0.8/PKG-INFO` & `pygination-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygination
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simple pagination for pydantic models and SQLAlchemy Query objects
 Home-page: https://github.com/jdmoralesar/pygination
 Author: Enerbit
 Author-email: jdmoralesar@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jdmoralesar/pygination/archive/refs/tags/0.0.1.tar.gz
 Keywords: python pagination
```

### Comparing `pygination-0.0.8/README.md` & `pygination-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pygination-0.0.8/setup.py` & `pygination-0.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from io import open
 from os import path
 
 # Always prefer setuptools over distutils
 from setuptools import find_packages, setup
 
 
-VERSION = "0.0.8"
+VERSION = "0.0.9"
 NAME = "pygination"
 AUTHOR = "Enerbit"
 AUTHOR_EMAIL = "jdmoralesar@gmail.com"
 DESCRIPTION = "Simple pagination for pydantic models and SQLAlchemy Query objects"
 PROJECT_URL = "https://github.com/jdmoralesar/pygination"
 DOWNLOAD_URL = "https://github.com/jdmoralesar/pygination/archive/refs/tags/0.0.1.tar.gz"
```

### Comparing `pygination-0.0.8/src/pygination/pygination.py` & `pygination-0.0.9/src/pygination/pygination.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,17 @@
         self.next_page = None
         self.has_previous = page > 0
         if self.has_previous:
             self.previous_page = page - 1
         previous_items = page * size
         self.has_next = previous_items + len(items) < total
 
+        if self.has_next and len(self.items) < self.size:
+            raise PaginationError("Invalid query. There are duplicate entries in this page of the query.")
+
         if self.has_next:
             self.next_page = page + 1
         self.total = total
 
     def __repr__(self) -> str:
         repr_string_list = []
         if self.has_previous:
@@ -44,11 +47,11 @@
 
 
 def paginate(query: Query, page: int, size: int) -> Page:
     if page < 0:
         raise AttributeError("page needs to be >= 0")
     if size <= 0:
         raise AttributeError("size needs to be >= 1")
-    total = query.order_by(None).distinct().count()
+    total = query.order_by(None).count()
     query_page = page * size
     items = query.limit(size).offset(query_page).all()
     return Page(items, page, size, total)
```

### Comparing `pygination-0.0.8/src/pygination.egg-info/PKG-INFO` & `pygination-0.0.9/src/pygination.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygination
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simple pagination for pydantic models and SQLAlchemy Query objects
 Home-page: https://github.com/jdmoralesar/pygination
 Author: Enerbit
 Author-email: jdmoralesar@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jdmoralesar/pygination/archive/refs/tags/0.0.1.tar.gz
 Keywords: python pagination
```

