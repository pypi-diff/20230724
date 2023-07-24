# Comparing `tmp/libtimed-0.4.1.tar.gz` & `tmp/libtimed-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libtimed-0.4.1.tar", max compression
+gzip compressed data, was "libtimed-0.4.2.tar", max compression
```

## Comparing `libtimed-0.4.1.tar` & `libtimed-0.4.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    34454 2023-07-24 07:04:48.375942 libtimed-0.4.1/LICENSE
--rw-r--r--   0        0        0      750 2023-07-24 07:04:48.375942 libtimed-0.4.1/README.md
--rw-r--r--   0        0        0     1307 2023-07-24 07:04:49.379943 libtimed-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1376 2023-07-24 07:04:48.375942 libtimed-0.4.1/src/libtimed/__init__.py
--rw-r--r--   0        0        0     9536 2023-07-24 07:04:48.375942 libtimed-0.4.1/src/libtimed/models.py
--rw-r--r--   0        0        0     4555 2023-07-24 07:04:48.375942 libtimed-0.4.1/src/libtimed/oidc.py
--rw-r--r--   0        0        0     6134 2023-07-24 07:04:48.375942 libtimed-0.4.1/src/libtimed/transforms.py
--rw-r--r--   0        0        0     1313 1970-01-01 00:00:00.000000 libtimed-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    34454 2023-07-24 17:03:31.205715 libtimed-0.4.2/LICENSE
+-rw-r--r--   0        0        0      750 2023-07-24 17:03:31.205715 libtimed-0.4.2/README.md
+-rw-r--r--   0        0        0     1307 2023-07-24 17:03:32.089727 libtimed-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1376 2023-07-24 17:03:31.205715 libtimed-0.4.2/src/libtimed/__init__.py
+-rw-r--r--   0        0        0     9536 2023-07-24 17:03:31.205715 libtimed-0.4.2/src/libtimed/models.py
+-rw-r--r--   0        0        0     4555 2023-07-24 17:03:31.205715 libtimed-0.4.2/src/libtimed/oidc.py
+-rw-r--r--   0        0        0     6195 2023-07-24 17:03:31.205715 libtimed-0.4.2/src/libtimed/transforms.py
+-rw-r--r--   0        0        0     1313 1970-01-01 00:00:00.000000 libtimed-0.4.2/PKG-INFO
```

### Comparing `libtimed-0.4.1/LICENSE` & `libtimed-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `libtimed-0.4.1/README.md` & `libtimed-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `libtimed-0.4.1/pyproject.toml` & `libtimed-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libtimed"
-version = "0.4.1"
+version = "0.4.2"
 description = "Library to intreact with timed webapp."
 authors = [
   "Arthur Deierlein <arthur.deierlein@adfinis.com>",
   "Gian Klug <gian.klug@adfinis.com>",
 ]
 readme = "README.md"
 packages = [{ include = "libtimed", from = "src" }]
```

### Comparing `libtimed-0.4.1/src/libtimed/__init__.py` & `libtimed-0.4.2/src/libtimed/__init__.py`

 * *Files identical despite different names*

### Comparing `libtimed-0.4.1/src/libtimed/models.py` & `libtimed-0.4.2/src/libtimed/models.py`

 * *Files identical despite different names*

### Comparing `libtimed-0.4.1/src/libtimed/oidc.py` & `libtimed-0.4.2/src/libtimed/oidc.py`

 * *Files identical despite different names*

### Comparing `libtimed-0.4.1/src/libtimed/transforms.py` & `libtimed-0.4.2/src/libtimed/transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,14 +87,16 @@
         self,
         value: Union[int, str, RelationShipProperty, None],
         is_filter=False,
         client=None,
     ) -> Union[dict, str, None]:
         if not value:
             return {"data": None}
+        if isinstance(value, dict):
+            return value
         data = {}
         if isinstance(value, RelationShipProperty):
             if not client:
                 raise SerializationError(
                     "Client has to be passed when using a property"
                 )
             try:
```

### Comparing `libtimed-0.4.1/PKG-INFO` & `libtimed-0.4.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libtimed
-Version: 0.4.1
+Version: 0.4.2
 Summary: Library to intreact with timed webapp.
 Author: Arthur Deierlein
 Author-email: arthur.deierlein@adfinis.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

