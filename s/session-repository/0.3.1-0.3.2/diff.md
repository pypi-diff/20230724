# Comparing `tmp/session-repository-0.3.1.tar.gz` & `tmp/session-repository-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "session-repository-0.3.1.tar", last modified: Tue Jul 18 09:16:16 2023, max compression
+gzip compressed data, was "session-repository-0.3.2.tar", last modified: Mon Jul 24 16:35:31 2023, max compression
```

## Comparing `session-repository-0.3.1.tar` & `session-repository-0.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 09:16:16.969203 session-repository-0.3.1/
--rw-rw-rw-   0        0        0      599 2023-07-18 09:16:16.965483 session-repository-0.3.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-18 09:16:16.898780 session-repository-0.3.1/session_repository/
--rw-rw-rw-   0        0        0      191 2023-07-18 08:45:38.000000 session-repository-0.3.1/session_repository/__init__.py
--rw-rw-rw-   0        0        0      583 2023-07-13 16:45:09.000000 session-repository-0.3.1/session_repository/enum.py
-drwxrwxrwx   0        0        0        0 2023-07-18 09:16:16.957727 session-repository-0.3.1/session_repository/models/
--rw-rw-rw-   0        0        0     7440 2023-07-18 09:15:21.000000 session-repository-0.3.1/session_repository/models/repository.py
--rw-rw-rw-   0        0        0      496 2023-07-18 09:04:38.000000 session-repository-0.3.1/session_repository/models/service.py
--rw-rw-rw-   0        0        0     9499 2023-07-13 16:52:30.000000 session-repository-0.3.1/session_repository/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-18 09:16:16.940098 session-repository-0.3.1/session_repository.egg-info/
--rw-rw-rw-   0        0        0      599 2023-07-18 09:16:16.000000 session-repository-0.3.1/session_repository.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      380 2023-07-18 09:16:16.000000 session-repository-0.3.1/session_repository.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 09:16:16.000000 session-repository-0.3.1/session_repository.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-18 09:16:16.000000 session-repository-0.3.1/session_repository.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-18 09:16:16.000000 session-repository-0.3.1/session_repository.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 09:16:16.970345 session-repository-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      877 2023-07-18 09:15:28.000000 session-repository-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 16:35:31.462655 session-repository-0.3.2/
+-rw-rw-rw-   0        0        0      599 2023-07-24 16:35:31.460617 session-repository-0.3.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-24 16:35:31.410279 session-repository-0.3.2/session_repository/
+-rw-rw-rw-   0        0        0      191 2023-07-18 08:45:38.000000 session-repository-0.3.2/session_repository/__init__.py
+-rw-rw-rw-   0        0        0      583 2023-07-13 16:45:09.000000 session-repository-0.3.2/session_repository/enum.py
+drwxrwxrwx   0        0        0        0 2023-07-24 16:35:31.454614 session-repository-0.3.2/session_repository/models/
+-rw-rw-rw-   0        0        0     9559 2023-07-24 16:33:49.000000 session-repository-0.3.2/session_repository/models/repository.py
+-rw-rw-rw-   0        0        0      496 2023-07-18 09:04:38.000000 session-repository-0.3.2/session_repository/models/service.py
+-rw-rw-rw-   0        0        0     9499 2023-07-13 16:52:30.000000 session-repository-0.3.2/session_repository/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-24 16:35:31.441720 session-repository-0.3.2/session_repository.egg-info/
+-rw-rw-rw-   0        0        0      599 2023-07-24 16:35:31.000000 session-repository-0.3.2/session_repository.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      380 2023-07-24 16:35:31.000000 session-repository-0.3.2/session_repository.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 16:35:31.000000 session-repository-0.3.2/session_repository.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-24 16:35:31.000000 session-repository-0.3.2/session_repository.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-24 16:35:31.000000 session-repository-0.3.2/session_repository.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 16:35:31.463822 session-repository-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      877 2023-07-24 16:34:32.000000 session-repository-0.3.2/setup.py
```

### Comparing `session-repository-0.3.1/PKG-INFO` & `session-repository-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: session-repository
-Version: 0.3.1
+Version: 0.3.2
 Summary: A project to have a base repository class to permform select/insert/update/delete with dynamtic syntaxe
 Home-page: https://github.com/Impro02/session-repository
-Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.3.1.tar.gz
+Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.3.2.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `session-repository-0.3.1/session_repository/enum.py` & `session-repository-0.3.2/session_repository/enum.py`

 * *Files identical despite different names*

### Comparing `session-repository-0.3.1/session_repository/models/repository.py` & `session-repository-0.3.2/session_repository/models/repository.py`

 * *Files 20% similar despite different names*

```diff
@@ -69,14 +69,29 @@
         model,
         filters: Optional[_FilterType] = None,
         optional_filters: Optional[_FilterType] = None,
         disabled_relationships: Optional[Dict[InstrumentedAttribute, Any]] = None,
         current_session: Optional[Session] = None,
     ) -> Optional[Any]:
         query = current_session.query(model)
+
+        return self._select_query(
+            query=query,
+            filters=filters,
+            optional_filters=optional_filters,
+            disabled_relationships=disabled_relationships,
+        )
+
+    def _select_query(
+        self,
+        query: Query,
+        filters: Optional[_FilterType] = None,
+        optional_filters: Optional[_FilterType] = None,
+        disabled_relationships: Optional[Dict[InstrumentedAttribute, Any]] = None,
+    ) -> Optional[Any]:
         query = apply_no_load(
             query=query,
             relationship_dict=disabled_relationships,
         )
         query = apply_filters(
             query=query,
             filter_dict=filters,
@@ -105,14 +120,37 @@
         disabled_relationships: Optional[Dict[InstrumentedAttribute, Any]] = None,
         order_by: Optional[Union[List[str], str]] = None,
         direction: Optional[str] = None,
         limit: int = None,
         current_session: Optional[Session] = None,
     ) -> List:
         query = current_session.query(model)
+
+        return self._select_all_query(
+            query=query,
+            model=model,
+            filters=filters,
+            optional_filters=optional_filters,
+            disabled_relationships=disabled_relationships,
+            order_by=order_by,
+            direction=direction,
+            limit=limit,
+        )
+
+    def _select_all_query(
+        self,
+        query: Query,
+        model,
+        filters: Optional[_FilterType] = None,
+        optional_filters: Optional[_FilterType] = None,
+        disabled_relationships: Optional[Dict[InstrumentedAttribute, Any]] = None,
+        order_by: Optional[Union[List[str], str]] = None,
+        direction: Optional[str] = None,
+        limit: int = None,
+    ) -> List:
         query = apply_no_load(
             query=query,
             relationship_dict=disabled_relationships,
         )
         query = apply_filters(
             query=query,
             filter_dict=filters,
@@ -154,14 +192,41 @@
         disabled_relationships: Optional[Dict[InstrumentedAttribute, Any]] = None,
         order_by: Optional[Union[List[str], str]] = None,
         direction: Optional[str] = None,
         limit: int = None,
         current_session: Optional[Session] = None,
     ) -> Tuple[List, str]:
         query = current_session.query(model)
+
+        return self._select_paginate_query(
+            query=query,
+            model=model,
+            page=page,
+            per_page=per_page,
+            filters=filters,
+            optional_filters=optional_filters,
+            disabled_relationships=disabled_relationships,
+            order_by=order_by,
+            direction=direction,
+            limit=limit,
+        )
+
+    def _select_paginate_query(
+        self,
+        query: Query,
+        model,
+        page: int,
+        per_page: int,
+        filters: Optional[_FilterType] = None,
+        optional_filters: Optional[_FilterType] = None,
+        disabled_relationships: Optional[Dict[InstrumentedAttribute, Any]] = None,
+        order_by: Optional[Union[List[str], str]] = None,
+        direction: Optional[str] = None,
+        limit: int = None,
+    ) -> Tuple[List, str]:
         query = apply_no_load(
             query=query,
             relationship_dict=disabled_relationships,
         )
         query = apply_filters(
             query=query,
             filter_dict=filters,
```

### Comparing `session-repository-0.3.1/session_repository/utils.py` & `session-repository-0.3.2/session_repository/utils.py`

 * *Files identical despite different names*

### Comparing `session-repository-0.3.1/session_repository.egg-info/PKG-INFO` & `session-repository-0.3.2/session_repository.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: session-repository
-Version: 0.3.1
+Version: 0.3.2
 Summary: A project to have a base repository class to permform select/insert/update/delete with dynamtic syntaxe
 Home-page: https://github.com/Impro02/session-repository
-Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.3.1.tar.gz
+Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.3.2.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `session-repository-0.3.1/setup.py` & `session-repository-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.3.1"
+version = "0.3.2"
 
 setup(
     name="session-repository",
     version=version,
     packages=[
         "session_repository",
         "session_repository.models",
```

