# Comparing `tmp/django-choices-1.7.2.tar.gz` & `tmp/django-choices-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-choices-1.7.2.tar", last modified: Mon Jul 12 13:03:24 2021, max compression
+gzip compressed data, was "django-choices-2.0.0.tar", last modified: Mon Jul 24 16:47:35 2023, max compression
```

## Comparing `django-choices-1.7.2.tar` & `django-choices-2.0.0.tar`

### file list

```diff
@@ -1,20 +1,26 @@
-drwxr-xr-x   0 bbt       (1001) users      (985)        0 2021-07-12 13:03:24.824471 django-choices-1.7.2/
--rw-r--r--   0 bbt       (1001) users      (985)     1059 2017-01-28 12:26:59.000000 django-choices-1.7.2/LICENSE
--rw-r--r--   0 bbt       (1001) users      (985)       20 2017-01-28 12:26:59.000000 django-choices-1.7.2/MANIFEST.in
--rw-r--r--   0 bbt       (1001) users      (985)     5313 2021-07-12 13:03:24.824471 django-choices-1.7.2/PKG-INFO
--rw-r--r--   0 bbt       (1001) users      (985)     4087 2021-07-12 13:00:03.000000 django-choices-1.7.2/README.rst
-drwxr-xr-x   0 bbt       (1001) users      (985)        0 2021-07-12 13:03:24.824471 django-choices-1.7.2/django_choices.egg-info/
--rw-r--r--   0 bbt       (1001) users      (985)     5313 2021-07-12 13:03:24.000000 django-choices-1.7.2/django_choices.egg-info/PKG-INFO
--rw-r--r--   0 bbt       (1001) users      (985)      377 2021-07-12 13:03:24.000000 django-choices-1.7.2/django_choices.egg-info/SOURCES.txt
--rw-r--r--   0 bbt       (1001) users      (985)        1 2021-07-12 13:03:24.000000 django-choices-1.7.2/django_choices.egg-info/dependency_links.txt
--rw-r--r--   0 bbt       (1001) users      (985)       25 2021-07-12 13:03:24.000000 django-choices-1.7.2/django_choices.egg-info/requires.txt
--rw-r--r--   0 bbt       (1001) users      (985)       10 2021-07-12 13:03:24.000000 django-choices-1.7.2/django_choices.egg-info/top_level.txt
-drwxr-xr-x   0 bbt       (1001) users      (985)        0 2021-07-12 13:03:24.824471 django-choices-1.7.2/djchoices/
--rw-r--r--   0 bbt       (1001) users      (985)      267 2021-07-12 12:25:18.000000 django-choices-1.7.2/djchoices/__init__.py
--rw-r--r--   0 bbt       (1001) users      (985)     6467 2021-07-12 12:25:18.000000 django-choices-1.7.2/djchoices/choices.py
-drwxr-xr-x   0 bbt       (1001) users      (985)        0 2021-07-12 13:03:24.824471 django-choices-1.7.2/djchoices/tests/
--rw-r--r--   0 bbt       (1001) users      (985)        0 2019-05-02 14:41:39.000000 django-choices-1.7.2/djchoices/tests/__init__.py
--rw-r--r--   0 bbt       (1001) users      (985)     9688 2021-07-12 12:25:18.000000 django-choices-1.7.2/djchoices/tests/test_choices.py
--rw-r--r--   0 bbt       (1001) users      (985)      624 2021-07-12 12:25:18.000000 django-choices-1.7.2/djchoices/tests/test_private_api.py
--rw-r--r--   0 bbt       (1001) users      (985)      334 2021-07-12 13:03:24.824471 django-choices-1.7.2/setup.cfg
--rw-r--r--   0 bbt       (1001) users      (985)     1550 2021-07-12 13:02:15.000000 django-choices-1.7.2/setup.py
+drwxr-xr-x   0 bbt       (1001) users      (985)        0 2023-07-24 16:47:35.243322 django-choices-2.0.0/
+-rw-r--r--   0 bbt       (1001) users      (985)     1059 2017-01-28 12:26:59.000000 django-choices-2.0.0/LICENSE
+-rw-r--r--   0 bbt       (1001) users      (985)       20 2017-01-28 12:26:59.000000 django-choices-2.0.0/MANIFEST.in
+-rw-r--r--   0 bbt       (1001) users      (985)     3523 2023-07-24 16:47:35.243322 django-choices-2.0.0/PKG-INFO
+-rw-r--r--   0 bbt       (1001) users      (985)     2622 2023-07-24 16:42:28.000000 django-choices-2.0.0/README.rst
+drwxr-xr-x   0 bbt       (1001) users      (985)        0 2023-07-24 16:47:35.243322 django-choices-2.0.0/django_choices.egg-info/
+-rw-r--r--   0 bbt       (1001) users      (985)     3523 2023-07-24 16:47:35.000000 django-choices-2.0.0/django_choices.egg-info/PKG-INFO
+-rw-r--r--   0 bbt       (1001) users      (985)      555 2023-07-24 16:47:35.000000 django-choices-2.0.0/django_choices.egg-info/SOURCES.txt
+-rw-r--r--   0 bbt       (1001) users      (985)        1 2023-07-24 16:47:35.000000 django-choices-2.0.0/django_choices.egg-info/dependency_links.txt
+-rw-r--r--   0 bbt       (1001) users      (985)       12 2023-07-24 16:47:35.000000 django-choices-2.0.0/django_choices.egg-info/requires.txt
+-rw-r--r--   0 bbt       (1001) users      (985)       10 2023-07-24 16:47:35.000000 django-choices-2.0.0/django_choices.egg-info/top_level.txt
+drwxr-xr-x   0 bbt       (1001) users      (985)        0 2023-07-24 16:47:35.243322 django-choices-2.0.0/djchoices/
+-rw-r--r--   0 bbt       (1001) users      (985)      267 2021-07-12 12:25:18.000000 django-choices-2.0.0/djchoices/__init__.py
+-rw-r--r--   0 bbt       (1001) users      (985)     6387 2023-07-24 16:42:28.000000 django-choices-2.0.0/djchoices/choices.py
+drwxr-xr-x   0 bbt       (1001) users      (985)        0 2023-07-24 16:47:35.243322 django-choices-2.0.0/djchoices/management/
+-rw-r--r--   0 bbt       (1001) users      (985)        0 2023-07-24 16:42:28.000000 django-choices-2.0.0/djchoices/management/__init__.py
+drwxr-xr-x   0 bbt       (1001) users      (985)        0 2023-07-24 16:47:35.243322 django-choices-2.0.0/djchoices/management/commands/
+-rw-r--r--   0 bbt       (1001) users      (985)        0 2023-07-24 16:42:28.000000 django-choices-2.0.0/djchoices/management/commands/__init__.py
+-rw-r--r--   0 bbt       (1001) users      (985)     2880 2023-07-24 16:42:28.000000 django-choices-2.0.0/djchoices/management/commands/generate_native_django_choices.py
+drwxr-xr-x   0 bbt       (1001) users      (985)        0 2023-07-24 16:47:35.243322 django-choices-2.0.0/djchoices/tests/
+-rw-r--r--   0 bbt       (1001) users      (985)        0 2019-05-02 14:41:39.000000 django-choices-2.0.0/djchoices/tests/__init__.py
+-rw-r--r--   0 bbt       (1001) users      (985)     9688 2021-07-12 12:25:18.000000 django-choices-2.0.0/djchoices/tests/test_choices.py
+-rw-r--r--   0 bbt       (1001) users      (985)     1132 2023-07-24 16:42:28.000000 django-choices-2.0.0/djchoices/tests/test_native_choices.py
+-rw-r--r--   0 bbt       (1001) users      (985)      624 2021-07-12 12:25:18.000000 django-choices-2.0.0/djchoices/tests/test_private_api.py
+-rw-r--r--   0 bbt       (1001) users      (985)      305 2023-07-24 16:47:35.243322 django-choices-2.0.0/setup.cfg
+-rw-r--r--   0 bbt       (1001) users      (985)     1199 2023-07-24 16:42:28.000000 django-choices-2.0.0/setup.py
```

### Comparing `django-choices-1.7.2/LICENSE` & `django-choices-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-choices-1.7.2/djchoices/choices.py` & `django-choices-2.0.0/djchoices/choices.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,14 @@
-from __future__ import absolute_import, unicode_literals
-
 import re
 from collections import OrderedDict
 
 from django.core.exceptions import ValidationError
 from django.db.models import Case, IntegerField, Value, When
 from django.utils.deconstruct import deconstructible
 
-import six
-
 __all__ = ["ChoiceItem", "DjangoChoices", "C"]
 
 
 # Support Functionality (Not part of public API)
 
 
 class Labels(dict):
@@ -184,15 +180,15 @@
     def __eq__(self, other):
         return isinstance(other, ChoicesValidator) and self.values == other.values
 
     def __ne__(self, other):
         return not (self == other)
 
 
-class DjangoChoices(six.with_metaclass(DjangoChoicesMeta)):
+class DjangoChoices(metaclass=DjangoChoicesMeta):
     order = 0
     choices = ()
     labels = Labels()
     values = {}
     validator = None
 
     @classmethod
```

### Comparing `django-choices-1.7.2/djchoices/tests/test_choices.py` & `django-choices-2.0.0/djchoices/tests/test_choices.py`

 * *Files identical despite different names*

### Comparing `django-choices-1.7.2/djchoices/tests/test_private_api.py` & `django-choices-2.0.0/djchoices/tests/test_private_api.py`

 * *Files identical despite different names*

### Comparing `django-choices-1.7.2/setup.py` & `django-choices-2.0.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,41 +3,33 @@
 from setuptools import find_packages, setup
 
 with open(path.join(path.dirname(__file__), "README.rst")) as f:
     readme = f.read()
 
 setup(
     name="django-choices",
-    version="1.7.2",
+    version="2.0.0",
     license="MIT",
     description="Sanity for the django choices functionality.",
     long_description=readme,
-    install_requires=["Django>=1.11", "six>=1.13.0"],
-    test_suite="runtests.get_suite",
+    install_requires=["Django>=3.2"],
     url="https://github.com/bigjason/django-choices",
     author="Jason Webb",
     author_email="bigjasonwebb@gmail.com,sergeimaertens@gmail.com",
     packages=find_packages(),
     include_package_data=True,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: MIT License",
         "Intended Audience :: Developers",
         "Framework :: Django",
-        "Framework :: Django :: 1.11",
-        "Framework :: Django :: 2.0",
-        "Framework :: Django :: 2.1",
-        "Framework :: Django :: 2.2",
-        "Framework :: Django :: 3.0",
-        "Framework :: Django :: 3.1",
         "Framework :: Django :: 3.2",
-        "Programming Language :: Python :: 2.7",
-        "Programming Language :: Python :: 3.4",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
+        "Framework :: Django :: 4.1",
+        "Framework :: Django :: 4.2",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: PyPy",
     ],
 )
```

