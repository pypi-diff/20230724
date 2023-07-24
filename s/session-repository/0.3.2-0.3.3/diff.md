# Comparing `tmp/session-repository-0.3.2.tar.gz` & `tmp/session-repository-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "session-repository-0.3.2.tar", last modified: Mon Jul 24 16:35:31 2023, max compression
+gzip compressed data, was "session-repository-0.3.3.tar", last modified: Mon Jul 24 19:18:07 2023, max compression
```

## Comparing `session-repository-0.3.2.tar` & `session-repository-0.3.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 16:35:31.462655 session-repository-0.3.2/
--rw-rw-rw-   0        0        0      599 2023-07-24 16:35:31.460617 session-repository-0.3.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-24 16:35:31.410279 session-repository-0.3.2/session_repository/
--rw-rw-rw-   0        0        0      191 2023-07-18 08:45:38.000000 session-repository-0.3.2/session_repository/__init__.py
--rw-rw-rw-   0        0        0      583 2023-07-13 16:45:09.000000 session-repository-0.3.2/session_repository/enum.py
-drwxrwxrwx   0        0        0        0 2023-07-24 16:35:31.454614 session-repository-0.3.2/session_repository/models/
--rw-rw-rw-   0        0        0     9559 2023-07-24 16:33:49.000000 session-repository-0.3.2/session_repository/models/repository.py
--rw-rw-rw-   0        0        0      496 2023-07-18 09:04:38.000000 session-repository-0.3.2/session_repository/models/service.py
--rw-rw-rw-   0        0        0     9499 2023-07-13 16:52:30.000000 session-repository-0.3.2/session_repository/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-24 16:35:31.441720 session-repository-0.3.2/session_repository.egg-info/
--rw-rw-rw-   0        0        0      599 2023-07-24 16:35:31.000000 session-repository-0.3.2/session_repository.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      380 2023-07-24 16:35:31.000000 session-repository-0.3.2/session_repository.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 16:35:31.000000 session-repository-0.3.2/session_repository.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-24 16:35:31.000000 session-repository-0.3.2/session_repository.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-24 16:35:31.000000 session-repository-0.3.2/session_repository.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 16:35:31.463822 session-repository-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0      877 2023-07-24 16:34:32.000000 session-repository-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 19:18:07.472547 session-repository-0.3.3/
+-rw-rw-rw-   0        0        0      599 2023-07-24 19:18:07.447488 session-repository-0.3.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-24 19:18:07.294151 session-repository-0.3.3/session_repository/
+-rw-rw-rw-   0        0        0      191 2023-07-18 08:45:38.000000 session-repository-0.3.3/session_repository/__init__.py
+-rw-rw-rw-   0        0        0      583 2023-07-13 16:45:09.000000 session-repository-0.3.3/session_repository/enum.py
+drwxrwxrwx   0        0        0        0 2023-07-24 19:18:07.440371 session-repository-0.3.3/session_repository/models/
+-rw-rw-rw-   0        0        0     9559 2023-07-24 16:33:49.000000 session-repository-0.3.3/session_repository/models/repository.py
+-rw-rw-rw-   0        0        0      496 2023-07-18 09:04:38.000000 session-repository-0.3.3/session_repository/models/service.py
+-rw-rw-rw-   0        0        0     9582 2023-07-24 19:16:34.000000 session-repository-0.3.3/session_repository/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-24 19:18:07.418950 session-repository-0.3.3/session_repository.egg-info/
+-rw-rw-rw-   0        0        0      599 2023-07-24 19:18:06.000000 session-repository-0.3.3/session_repository.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      380 2023-07-24 19:18:06.000000 session-repository-0.3.3/session_repository.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 19:18:06.000000 session-repository-0.3.3/session_repository.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-24 19:18:06.000000 session-repository-0.3.3/session_repository.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-24 19:18:06.000000 session-repository-0.3.3/session_repository.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 19:18:07.473557 session-repository-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      877 2023-07-24 19:17:00.000000 session-repository-0.3.3/setup.py
```

### Comparing `session-repository-0.3.2/PKG-INFO` & `session-repository-0.3.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: session-repository
-Version: 0.3.2
+Version: 0.3.3
 Summary: A project to have a base repository class to permform select/insert/update/delete with dynamtic syntaxe
 Home-page: https://github.com/Impro02/session-repository
-Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.3.2.tar.gz
+Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.3.3.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `session-repository-0.3.2/session_repository/enum.py` & `session-repository-0.3.3/session_repository/enum.py`

 * *Files identical despite different names*

### Comparing `session-repository-0.3.2/session_repository/models/repository.py` & `session-repository-0.3.3/session_repository/models/repository.py`

 * *Files identical despite different names*

### Comparing `session-repository-0.3.2/session_repository/utils.py` & `session-repository-0.3.3/session_repository/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,14 +245,18 @@
                         for condition in v:
                             conditions.append(key.has(condition))
                     case Operators.ANY:
                         v = get_filters(
                             v,
                             with_optional=with_optional,
                         )
+
+                        if len(v) == 0:
+                            continue
+
                         conditions.append(key.any(and_(*v)))
 
     return conditions
 
 
 def get_filters(
     filters: _FilterType,
```

### Comparing `session-repository-0.3.2/session_repository.egg-info/PKG-INFO` & `session-repository-0.3.3/session_repository.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: session-repository
-Version: 0.3.2
+Version: 0.3.3
 Summary: A project to have a base repository class to permform select/insert/update/delete with dynamtic syntaxe
 Home-page: https://github.com/Impro02/session-repository
-Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.3.2.tar.gz
+Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.3.3.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `session-repository-0.3.2/setup.py` & `session-repository-0.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.3.2"
+version = "0.3.3"
 
 setup(
     name="session-repository",
     version=version,
     packages=[
         "session_repository",
         "session_repository.models",
```

