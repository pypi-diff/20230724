# Comparing `tmp/django_backblaze_b2-4.0.0.tar.gz` & `tmp/django_backblaze_b2-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_backblaze_b2-4.0.0.tar", max compression
+gzip compressed data, was "django_backblaze_b2-4.0.1.tar", max compression
```

## Comparing `django_backblaze_b2-4.0.0.tar` & `django_backblaze_b2-4.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1318 2020-08-25 16:03:37.000000 django_backblaze_b2-4.0.0/LICENSE
--rw-r--r--   0        0        0     8556 2023-07-02 20:36:28.971655 django_backblaze_b2-4.0.0/README.md
--rw-r--r--   0        0        0      264 2020-09-18 05:30:12.000000 django_backblaze_b2-4.0.0/django_backblaze_b2/__init__.py
--rw-r--r--   0        0        0     1024 2023-07-02 20:36:25.735529 django_backblaze_b2-4.0.0/django_backblaze_b2/_decorators.py
--rw-r--r--   0        0        0     2720 2023-07-02 20:36:25.735944 django_backblaze_b2-4.0.0/django_backblaze_b2/b2_file.py
--rw-r--r--   0        0        0     7932 2023-07-02 20:36:25.736279 django_backblaze_b2-4.0.0/django_backblaze_b2/cache_account_info.py
--rw-r--r--   0        0        0     2004 2023-07-02 20:36:25.736571 django_backblaze_b2-4.0.0/django_backblaze_b2/options.py
--rw-r--r--   0        0        0        0 2020-09-18 05:30:12.000000 django_backblaze_b2-4.0.0/django_backblaze_b2/py.typed
--rw-r--r--   0        0        0    12923 2023-07-02 20:36:25.736917 django_backblaze_b2-4.0.0/django_backblaze_b2/storage.py
--rw-r--r--   0        0        0     4727 2023-07-02 20:36:25.737269 django_backblaze_b2-4.0.0/django_backblaze_b2/storages.py
--rw-r--r--   0        0        0      358 2023-07-02 20:36:25.737573 django_backblaze_b2-4.0.0/django_backblaze_b2/urls.py
--rw-r--r--   0        0        0     2167 2023-07-02 20:36:25.737820 django_backblaze_b2-4.0.0/django_backblaze_b2/views.py
--rw-r--r--   0        0        0     2022 2023-07-02 20:36:37.394079 django_backblaze_b2-4.0.0/pyproject.toml
--rw-r--r--   0        0        0    10260 1970-01-01 00:00:00.000000 django_backblaze_b2-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1318 2020-08-25 16:03:37.000000 django_backblaze_b2-4.0.1/LICENSE
+-rw-r--r--   0        0        0     8556 2023-07-02 20:36:28.971655 django_backblaze_b2-4.0.1/README.md
+-rw-r--r--   0        0        0      264 2020-09-18 05:30:12.000000 django_backblaze_b2-4.0.1/django_backblaze_b2/__init__.py
+-rw-r--r--   0        0        0     1024 2023-07-02 20:36:25.735529 django_backblaze_b2-4.0.1/django_backblaze_b2/_decorators.py
+-rw-r--r--   0        0        0     2720 2023-07-24 07:09:19.210475 django_backblaze_b2-4.0.1/django_backblaze_b2/b2_file.py
+-rw-r--r--   0        0        0     7932 2023-07-24 06:59:23.702987 django_backblaze_b2-4.0.1/django_backblaze_b2/cache_account_info.py
+-rw-r--r--   0        0        0     2004 2023-07-02 20:36:25.736571 django_backblaze_b2-4.0.1/django_backblaze_b2/options.py
+-rw-r--r--   0        0        0        0 2020-09-18 05:30:12.000000 django_backblaze_b2-4.0.1/django_backblaze_b2/py.typed
+-rw-r--r--   0        0        0    12923 2023-07-24 07:09:19.210895 django_backblaze_b2-4.0.1/django_backblaze_b2/storage.py
+-rw-r--r--   0        0        0     4727 2023-07-02 20:36:25.737269 django_backblaze_b2-4.0.1/django_backblaze_b2/storages.py
+-rw-r--r--   0        0        0      358 2023-07-02 20:36:25.737573 django_backblaze_b2-4.0.1/django_backblaze_b2/urls.py
+-rw-r--r--   0        0        0     2167 2023-07-02 20:36:25.737820 django_backblaze_b2-4.0.1/django_backblaze_b2/views.py
+-rw-r--r--   0        0        0     2022 2023-07-24 07:10:14.628470 django_backblaze_b2-4.0.1/pyproject.toml
+-rw-r--r--   0        0        0    10260 1970-01-01 00:00:00.000000 django_backblaze_b2-4.0.1/PKG-INFO
```

### Comparing `django_backblaze_b2-4.0.0/LICENSE` & `django_backblaze_b2-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_backblaze_b2-4.0.0/README.md` & `django_backblaze_b2-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `django_backblaze_b2-4.0.0/django_backblaze_b2/_decorators.py` & `django_backblaze_b2-4.0.1/django_backblaze_b2/_decorators.py`

 * *Files identical despite different names*

### Comparing `django_backblaze_b2-4.0.0/django_backblaze_b2/b2_file.py` & `django_backblaze_b2-4.0.1/django_backblaze_b2/b2_file.py`

 * *Files identical despite different names*

### Comparing `django_backblaze_b2-4.0.0/django_backblaze_b2/cache_account_info.py` & `django_backblaze_b2-4.0.1/django_backblaze_b2/cache_account_info.py`

 * *Files identical despite different names*

### Comparing `django_backblaze_b2-4.0.0/django_backblaze_b2/options.py` & `django_backblaze_b2-4.0.1/django_backblaze_b2/options.py`

 * *Files identical despite different names*

### Comparing `django_backblaze_b2-4.0.0/django_backblaze_b2/storage.py` & `django_backblaze_b2-4.0.1/django_backblaze_b2/storage.py`

 * *Files identical despite different names*

### Comparing `django_backblaze_b2-4.0.0/django_backblaze_b2/storages.py` & `django_backblaze_b2-4.0.1/django_backblaze_b2/storages.py`

 * *Files identical despite different names*

### Comparing `django_backblaze_b2-4.0.0/django_backblaze_b2/views.py` & `django_backblaze_b2-4.0.1/django_backblaze_b2/views.py`

 * *Files identical despite different names*

### Comparing `django_backblaze_b2-4.0.0/pyproject.toml` & `django_backblaze_b2-4.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.black]
 line-length = 120
 
 [tool.poetry]
 name = "django-backblaze-b2"
-version = "4.0.0"
+version = "4.0.1"
 description = "A Django app to use backblaze b2 as storage."
 authors = ["Etienne H <django_backblaze_b2@internet-e-mail.com>"]
 maintainers = ["Etienne H <django_backblaze_b2@internet-e-mail.com>"]
 license = "BSD-2-Clause"
 readme = "README.md"
 homepage = "https://github.com/ehossack/django-backblaze-b2/"
 repository = "https://github.com/ehossack/django-backblaze-b2/"
@@ -48,23 +48,23 @@
 python = "^3.7.1"
 b2sdk = ">=1.11.0"
 django = ">=3.2"
 typing-extensions = "^4.0.1"
 
 [tool.poetry.dev-dependencies]
 isort = "^5.11.5"
-pytest = "^7.3"
+pytest = "^7.4"
 mypy = ">=0.8"
 black = "^23.3"
 django-stubs = "^4.2.0"
 flake8 = "^5.0"
-pytest-cov = "^4.0"
+pytest-cov = "^4.1"
 pytest-django = "^4.5"
 pytest-pythonpath = "^0.7"
-docutils = "^0.19"
+docutils = "^0.20"
 toml = "^0.10.2"
 
 [tool.poetry.group.dev.dependencies]
 pep8-naming = "^0.13.3"
 
 [build-system]
 requires = ["poetry>=1.2.0"]
```

### Comparing `django_backblaze_b2-4.0.0/PKG-INFO` & `django_backblaze_b2-4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-backblaze-b2
-Version: 4.0.0
+Version: 4.0.1
 Summary: A Django app to use backblaze b2 as storage.
 Home-page: https://github.com/ehossack/django-backblaze-b2/
 License: BSD-2-Clause
 Keywords: django,storage,backblaze,b2,cloud
 Author: Etienne H
 Author-email: django_backblaze_b2@internet-e-mail.com
 Maintainer: Etienne H
```

