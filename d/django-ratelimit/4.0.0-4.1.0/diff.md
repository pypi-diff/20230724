# Comparing `tmp/django-ratelimit-4.0.0.tar.gz` & `tmp/django-ratelimit-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ratelimit-4.0.0.tar", last modified: Sun Dec  4 03:15:36 2022, max compression
+gzip compressed data, was "django-ratelimit-4.1.0.tar", last modified: Mon Jul 24 20:34:19 2023, max compression
```

## Comparing `django-ratelimit-4.0.0.tar` & `django-ratelimit-4.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 03:15:36.159239 django-ratelimit-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2022-12-04 03:15:13.000000 django-ratelimit-4.0.0/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (123)      557 2022-12-04 03:15:13.000000 django-ratelimit-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       73 2022-12-04 03:15:13.000000 django-ratelimit-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2022-12-04 03:15:36.159239 django-ratelimit-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2022-12-04 03:15:13.000000 django-ratelimit-4.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 03:15:36.159239 django-ratelimit-4.0.0/django_ratelimit/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2022-12-04 03:15:13.000000 django-ratelimit-4.0.0/django_ratelimit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2022-12-04 03:15:13.000000 django-ratelimit-4.0.0/django_ratelimit/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2022-12-04 03:15:13.000000 django-ratelimit-4.0.0/django_ratelimit/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2022-12-04 03:15:13.000000 django-ratelimit-4.0.0/django_ratelimit/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2022-12-04 03:15:13.000000 django-ratelimit-4.0.0/django_ratelimit/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2022-12-04 03:15:13.000000 django-ratelimit-4.0.0/django_ratelimit/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2022-12-04 03:15:13.000000 django-ratelimit-4.0.0/django_ratelimit/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2022-12-04 03:15:13.000000 django-ratelimit-4.0.0/django_ratelimit/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    21689 2022-12-04 03:15:13.000000 django-ratelimit-4.0.0/django_ratelimit/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 03:15:36.159239 django-ratelimit-4.0.0/django_ratelimit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2022-12-04 03:15:36.000000 django-ratelimit-4.0.0/django_ratelimit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      477 2022-12-04 03:15:36.000000 django-ratelimit-4.0.0/django_ratelimit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-04 03:15:36.000000 django-ratelimit-4.0.0/django_ratelimit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2022-12-04 03:15:36.000000 django-ratelimit-4.0.0/django_ratelimit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2022-12-04 03:15:13.000000 django-ratelimit-4.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2022-12-04 03:15:36.159239 django-ratelimit-4.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:34:19.075552 django-ratelimit-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-07-24 20:33:58.000000 django-ratelimit-4.1.0/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-24 20:33:58.000000 django-ratelimit-4.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-24 20:33:58.000000 django-ratelimit-4.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-24 20:34:19.075552 django-ratelimit-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-24 20:33:58.000000 django-ratelimit-4.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:34:19.075552 django-ratelimit-4.1.0/django_ratelimit/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-24 20:33:58.000000 django-ratelimit-4.1.0/django_ratelimit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-24 20:33:58.000000 django-ratelimit-4.1.0/django_ratelimit/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-24 20:33:58.000000 django-ratelimit-4.1.0/django_ratelimit/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7993 2023-07-24 20:33:58.000000 django-ratelimit-4.1.0/django_ratelimit/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-24 20:33:58.000000 django-ratelimit-4.1.0/django_ratelimit/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-24 20:33:58.000000 django-ratelimit-4.1.0/django_ratelimit/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-24 20:33:58.000000 django-ratelimit-4.1.0/django_ratelimit/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-24 20:33:58.000000 django-ratelimit-4.1.0/django_ratelimit/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21689 2023-07-24 20:33:58.000000 django-ratelimit-4.1.0/django_ratelimit/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:34:19.075552 django-ratelimit-4.1.0/django_ratelimit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-24 20:34:19.000000 django-ratelimit-4.1.0/django_ratelimit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-24 20:34:19.000000 django-ratelimit-4.1.0/django_ratelimit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 20:34:19.000000 django-ratelimit-4.1.0/django_ratelimit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-24 20:34:19.000000 django-ratelimit-4.1.0/django_ratelimit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-24 20:33:58.000000 django-ratelimit-4.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-24 20:34:19.075552 django-ratelimit-4.1.0/setup.cfg
```

### Comparing `django-ratelimit-4.0.0/CHANGELOG` & `django-ratelimit-4.1.0/CHANGELOG`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,28 @@
 ==========
 Change Log
 ==========
 
 UNRELEASED
 ==========
 
+v4.1
+====
+
+Additions:
+----------
+
+- Add RATELIMITE_HASH_ALGORITHM setting (#282, #285)
+
+Minor changes:
+--------------
+
+- Fixed links in docs (#277)
+- Test on Django 4.2 (#284)
+
 v4.0
 ====
 
 Breaking changes:
 -----------------
 
 - Renamed the package from ratelimit to django_ratelimit (#226)
```

### Comparing `django-ratelimit-4.0.0/LICENSE` & `django-ratelimit-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-ratelimit-4.0.0/PKG-INFO` & `django-ratelimit-4.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ratelimit
-Version: 4.0.0
+Version: 4.1.0
 Summary: Cache-based rate-limiting for Django.
 Author-email: James Socol <me@jamessocol.com>
 License: Copyright (c) 2022, James Socol
         
         Licensed under the Apache License, Version 2.0 (the "License");
         you may not use this file except in compliance with the License.
         You may obtain a copy of the License at
@@ -13,15 +13,15 @@
         
         Unless required by applicable law or agreed to in writing, software
         distributed under the License is distributed on an "AS IS" BASIS,
         WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
         See the License for the specific language governing permissions and
         limitations under the License.
         
-Project-URL: Homepage, https://github.com/jsocol/pystatsd
+Project-URL: Homepage, https://github.com/jsocol/django-ratelimit
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `django-ratelimit-4.0.0/README.rst` & `django-ratelimit-4.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-ratelimit-4.0.0/django_ratelimit/checks.py` & `django-ratelimit-4.1.0/django_ratelimit/checks.py`

 * *Files identical despite different names*

### Comparing `django-ratelimit-4.0.0/django_ratelimit/core.py` & `django-ratelimit-4.1.0/django_ratelimit/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -136,15 +136,20 @@
     if methods is not None:
         if methods == ALL:
             methods = ''
         elif isinstance(methods, (list, tuple)):
             methods = ''.join(sorted([m.upper() for m in methods]))
         parts.append(methods)
     prefix = getattr(settings, 'RATELIMIT_CACHE_PREFIX', 'rl:')
-    return prefix + hashlib.md5(''.join(parts).encode('utf-8')).hexdigest()
+    attr = getattr(settings, 'RATELIMIT_HASH_ALGORITHM', hashlib.sha256)
+    algo_cls = (import_string(f'{attr}')
+                if isinstance(attr, str)
+                else attr
+                )
+    return prefix + algo_cls(''.join(parts).encode('utf-8')).hexdigest()
 
 
 def is_ratelimited(request, group=None, fn=None, key=None, rate=None,
                    method=ALL, increment=False):
     usage = get_usage(request, group, fn, key, rate, method, increment)
     if usage is None:
         return False
```

### Comparing `django-ratelimit-4.0.0/django_ratelimit/decorators.py` & `django-ratelimit-4.1.0/django_ratelimit/decorators.py`

 * *Files identical despite different names*

### Comparing `django-ratelimit-4.0.0/django_ratelimit/middleware.py` & `django-ratelimit-4.1.0/django_ratelimit/middleware.py`

 * *Files identical despite different names*

### Comparing `django-ratelimit-4.0.0/django_ratelimit/tests.py` & `django-ratelimit-4.1.0/django_ratelimit/tests.py`

 * *Files identical despite different names*

### Comparing `django-ratelimit-4.0.0/django_ratelimit.egg-info/PKG-INFO` & `django-ratelimit-4.1.0/django_ratelimit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ratelimit
-Version: 4.0.0
+Version: 4.1.0
 Summary: Cache-based rate-limiting for Django.
 Author-email: James Socol <me@jamessocol.com>
 License: Copyright (c) 2022, James Socol
         
         Licensed under the Apache License, Version 2.0 (the "License");
         you may not use this file except in compliance with the License.
         You may obtain a copy of the License at
@@ -13,15 +13,15 @@
         
         Unless required by applicable law or agreed to in writing, software
         distributed under the License is distributed on an "AS IS" BASIS,
         WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
         See the License for the specific language governing permissions and
         limitations under the License.
         
-Project-URL: Homepage, https://github.com/jsocol/pystatsd
+Project-URL: Homepage, https://github.com/jsocol/django-ratelimit
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `django-ratelimit-4.0.0/pyproject.toml` & `django-ratelimit-4.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django-ratelimit"
-version = "4.0.0"
+version = "4.1.0"
 authors = [{name = "James Socol", email = "me@jamessocol.com"}]
 requires-python = ">= 3.7"
 license = {file = "LICENSE"}
 description = "Cache-based rate-limiting for Django."
 readme = "README.rst"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -22,15 +22,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Framework :: Django",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
-urls = {Homepage = "https://github.com/jsocol/pystatsd"}
+urls = {Homepage = "https://github.com/jsocol/django-ratelimit"}
 
 [tool.distutils.bdist_wheel]
 universal = 1
 
 [tool.setuptools]
 include-package-data = true
```

