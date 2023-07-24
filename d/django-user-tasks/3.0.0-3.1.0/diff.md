# Comparing `tmp/django-user-tasks-3.0.0.tar.gz` & `tmp/django-user-tasks-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-user-tasks-3.0.0.tar", last modified: Wed Feb  9 10:29:10 2022, max compression
+gzip compressed data, was "django-user-tasks-3.1.0.tar", last modified: Mon Jul 24 13:56:15 2023, max compression
```

## Comparing `django-user-tasks-3.0.0.tar` & `django-user-tasks-3.1.0.tar`

### file list

```diff
@@ -1,39 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-09 10:29:10.281869 django-user-tasks-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-02-09 10:29:05.000000 django-user-tasks-3.0.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)     4665 2022-02-09 10:29:05.000000 django-user-tasks-3.0.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-02-09 10:29:05.000000 django-user-tasks-3.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-02-09 10:29:05.000000 django-user-tasks-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     9839 2022-02-09 10:29:10.281869 django-user-tasks-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4382 2022-02-09 10:29:05.000000 django-user-tasks-3.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-09 10:29:10.281869 django-user-tasks-3.0.0/django_user_tasks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9839 2022-02-09 10:29:10.000000 django-user-tasks-3.0.0/django_user_tasks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      858 2022-02-09 10:29:10.000000 django-user-tasks-3.0.0/django_user_tasks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-09 10:29:10.000000 django-user-tasks-3.0.0/django_user_tasks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-09 10:29:10.000000 django-user-tasks-3.0.0/django_user_tasks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-02-09 10:29:10.000000 django-user-tasks-3.0.0/django_user_tasks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-02-09 10:29:10.000000 django-user-tasks-3.0.0/django_user_tasks.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-09 10:29:10.281869 django-user-tasks-3.0.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      314 2022-02-09 10:29:05.000000 django-user-tasks-3.0.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (121)      892 2022-02-09 10:29:05.000000 django-user-tasks-3.0.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (121)      658 2022-02-09 10:29:10.281869 django-user-tasks-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     5204 2022-02-09 10:29:05.000000 django-user-tasks-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-09 10:29:10.281869 django-user-tasks-3.0.0/user_tasks/
--rw-r--r--   0 runner    (1001) docker     (121)      415 2022-02-09 10:29:05.000000 django-user-tasks-3.0.0/user_tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      978 2022-02-09 10:29:05.000000 django-user-tasks-3.0.0/user_tasks/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      451 2022-02-09 10:29:05.000000 django-user-tasks-3.0.0/user_tasks/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     2764 2022-02-09 10:29:05.000000 django-user-tasks-3.0.0/user_tasks/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-02-09 10:29:05.000000 django-user-tasks-3.0.0/user_tasks/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1296 2022-02-09 10:29:05.000000 django-user-tasks-3.0.0/user_tasks/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-09 10:29:10.281869 django-user-tasks-3.0.0/user_tasks/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     3804 2022-02-09 10:29:05.000000 django-user-tasks-3.0.0/user_tasks/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      531 2022-02-09 10:29:05.000000 django-user-tasks-3.0.0/user_tasks/migrations/0002_artifact_file_storage.py
--rw-r--r--   0 runner    (1001) docker     (121)      414 2022-02-09 10:29:05.000000 django-user-tasks-3.0.0/user_tasks/migrations/0003_url_max_length.py
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-02-09 10:29:05.000000 django-user-tasks-3.0.0/user_tasks/migrations/0004_url_textfield.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-09 10:29:05.000000 django-user-tasks-3.0.0/user_tasks/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10824 2022-02-09 10:29:05.000000 django-user-tasks-3.0.0/user_tasks/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     2559 2022-02-09 10:29:05.000000 django-user-tasks-3.0.0/user_tasks/rules.py
--rw-r--r--   0 runner    (1001) docker     (121)     1585 2022-02-09 10:29:05.000000 django-user-tasks-3.0.0/user_tasks/serializers.py
--rw-r--r--   0 runner    (1001) docker     (121)    10670 2022-02-09 10:29:05.000000 django-user-tasks-3.0.0/user_tasks/signals.py
--rw-r--r--   0 runner    (1001) docker     (121)     4440 2022-02-09 10:29:05.000000 django-user-tasks-3.0.0/user_tasks/tasks.py
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-02-09 10:29:05.000000 django-user-tasks-3.0.0/user_tasks/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     3044 2022-02-09 10:29:05.000000 django-user-tasks-3.0.0/user_tasks/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 13:56:15.072883 django-user-tasks-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-07-24 13:56:08.000000 django-user-tasks-3.1.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (122)     4976 2023-07-24 13:56:08.000000 django-user-tasks-3.1.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-07-24 13:56:08.000000 django-user-tasks-3.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-07-24 13:56:08.000000 django-user-tasks-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    10018 2023-07-24 13:56:15.072883 django-user-tasks-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4266 2023-07-24 13:56:08.000000 django-user-tasks-3.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 13:56:15.072883 django-user-tasks-3.1.0/django_user_tasks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    10018 2023-07-24 13:56:15.000000 django-user-tasks-3.1.0/django_user_tasks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      990 2023-07-24 13:56:15.000000 django-user-tasks-3.1.0/django_user_tasks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-24 13:56:15.000000 django-user-tasks-3.1.0/django_user_tasks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-24 13:56:15.000000 django-user-tasks-3.1.0/django_user_tasks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-07-24 13:56:15.000000 django-user-tasks-3.1.0/django_user_tasks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-07-24 13:56:15.000000 django-user-tasks-3.1.0/django_user_tasks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 13:56:15.072883 django-user-tasks-3.1.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      323 2023-07-24 13:56:08.000000 django-user-tasks-3.1.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      892 2023-07-24 13:56:08.000000 django-user-tasks-3.1.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      658 2023-07-24 13:56:15.076883 django-user-tasks-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5208 2023-07-24 13:56:08.000000 django-user-tasks-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 13:56:15.072883 django-user-tasks-3.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1169 2023-07-24 13:56:08.000000 django-user-tasks-3.1.0/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10563 2023-07-24 13:56:08.000000 django-user-tasks-3.1.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12032 2023-07-24 13:56:08.000000 django-user-tasks-3.1.0/tests/test_rest_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5477 2023-07-24 13:56:08.000000 django-user-tasks-3.1.0/tests/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21472 2023-07-24 13:56:08.000000 django-user-tasks-3.1.0/tests/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5702 2023-07-24 13:56:08.000000 django-user-tasks-3.1.0/tests/test_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 13:56:15.072883 django-user-tasks-3.1.0/user_tasks/
+-rw-r--r--   0 runner    (1001) docker     (122)      296 2023-07-24 13:56:08.000000 django-user-tasks-3.1.0/user_tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      924 2023-07-24 13:56:08.000000 django-user-tasks-3.1.0/user_tasks/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      434 2023-07-24 13:56:08.000000 django-user-tasks-3.1.0/user_tasks/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2700 2023-07-24 13:56:08.000000 django-user-tasks-3.1.0/user_tasks/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      169 2023-07-24 13:56:08.000000 django-user-tasks-3.1.0/user_tasks/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1296 2023-07-24 13:56:08.000000 django-user-tasks-3.1.0/user_tasks/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 13:56:15.072883 django-user-tasks-3.1.0/user_tasks/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     3804 2023-07-24 13:56:08.000000 django-user-tasks-3.1.0/user_tasks/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)      531 2023-07-24 13:56:08.000000 django-user-tasks-3.1.0/user_tasks/migrations/0002_artifact_file_storage.py
+-rw-r--r--   0 runner    (1001) docker     (122)      414 2023-07-24 13:56:08.000000 django-user-tasks-3.1.0/user_tasks/migrations/0003_url_max_length.py
+-rw-r--r--   0 runner    (1001) docker     (122)      474 2023-07-24 13:56:08.000000 django-user-tasks-3.1.0/user_tasks/migrations/0004_url_textfield.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-24 13:56:08.000000 django-user-tasks-3.1.0/user_tasks/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10621 2023-07-24 13:56:08.000000 django-user-tasks-3.1.0/user_tasks/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-07-24 13:56:08.000000 django-user-tasks-3.1.0/user_tasks/rules.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1585 2023-07-24 13:56:08.000000 django-user-tasks-3.1.0/user_tasks/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10530 2023-07-24 13:56:08.000000 django-user-tasks-3.1.0/user_tasks/signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4440 2023-07-24 13:56:08.000000 django-user-tasks-3.1.0/user_tasks/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (122)      335 2023-07-24 13:56:08.000000 django-user-tasks-3.1.0/user_tasks/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3009 2023-07-24 13:56:08.000000 django-user-tasks-3.1.0/user_tasks/views.py
```

### Comparing `django-user-tasks-3.0.0/CHANGELOG.rst` & `django-user-tasks-3.1.0/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -10,22 +10,40 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+
+[3.1.0] - 2023-07-21
+~~~~~~~~~~~~~~~~~~~~
+
+Added
++++++
+* Added Django42 support in CI.
+
 Removed
 +++++++
+* Removed old versions of celery and drf version from ci.
 
+Chore
++++++
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated
+
+[3.0.0] - 2022-02-09
+~~~~~~~~~~~~~~~~~~~~
+
+Removed
++++++++
 * Removed Python 3.5 support.
 
 Chore
 +++++
-
 * Upgraded celery to latest 5.x version.
 
 [2.2.0] - 2022-01-26
 ~~~~~~~~~~~~~~~~~~~~
 
 Removed
 +++++++
```

### Comparing `django-user-tasks-3.0.0/LICENSE.txt` & `django-user-tasks-3.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-user-tasks-3.0.0/PKG-INFO` & `django-user-tasks-3.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: django-user-tasks
-Version: 3.0.0
+Version: 3.1.0
 Summary: Management of user-triggered asynchronous tasks in Django projects
-Home-page: https://github.com/edx/django-user-tasks
+Home-page: https://github.com/openedx/django-user-tasks
 Author: edX
 Author-email: oscm@edx.org
 License: Apache Software License 2.0
 Keywords: Django edx
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
@@ -24,16 +23,16 @@
 django-user-tasks
 =================
 
 .. image:: https://img.shields.io/pypi/v/django-user-tasks.svg
     :target: https://pypi.python.org/pypi/django-user-tasks/
     :alt: PyPI
 
-.. image:: https://github.com/edx/django-user-tasks/workflows/Python%20CI/badge.svg?branch=master
-    :target: https://github.com/edx/django-user-tasks/actions?query=workflow%3A%22Python+CI%22
+.. image:: https://github.com/openedx/django-user-tasks/workflows/Python%20CI/badge.svg?branch=master
+    :target: https://github.com/openedx/django-user-tasks/actions?query=workflow%3A%22Python+CI%22
     :alt: CI
 
 .. image:: http://codecov.io/github/edx/django-user-tasks/coverage.svg?branch=master
     :target: http://codecov.io/github/edx/django-user-tasks?branch=master
     :alt: Codecov
 
 .. image:: https://readthedocs.org/projects/django-user-tasks/badge/?version=latest
@@ -41,15 +40,15 @@
     :alt: Documentation
 
 .. image:: https://img.shields.io/pypi/pyversions/django-user-tasks.svg
     :target: https://pypi.python.org/pypi/django-user-tasks/
     :alt: Supported Python versions
 
 .. image:: https://img.shields.io/github/license/edx/django-user-tasks.svg
-    :target: https://github.com/edx/django-user-tasks/blob/master/LICENSE.txt
+    :target: https://github.com/openedx/django-user-tasks/blob/master/LICENSE.txt
     :alt: License
 
 django-user-tasks is a reusable Django application for managing user-triggered
 asynchronous tasks.  It provides a status page for each such task, which
 includes a meaningful progress indicator if the task is currently being
 executed and provides any appropriate text and/or links for output once the
 task is complete.
@@ -109,18 +108,15 @@
 Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
-
-Even though they were written with ``edx-platform`` in mind, the guidelines
-should be followed for Open edX code in general.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org.
 
 Getting Help
@@ -144,22 +140,40 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+
+[3.1.0] - 2023-07-21
+~~~~~~~~~~~~~~~~~~~~
+
+Added
++++++
+* Added Django42 support in CI.
+
 Removed
 +++++++
+* Removed old versions of celery and drf version from ci.
 
+Chore
++++++
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated
+
+[3.0.0] - 2022-02-09
+~~~~~~~~~~~~~~~~~~~~
+
+Removed
++++++++
 * Removed Python 3.5 support.
 
 Chore
 +++++
-
 * Upgraded celery to latest 5.x version.
 
 [2.2.0] - 2022-01-26
 ~~~~~~~~~~~~~~~~~~~~
 
 Removed
 +++++++
@@ -396,9 +410,7 @@
 [0.1.0] - 2016-10-07
 ~~~~~~~~~~~~~~~~~~~~
 
 Added
 +++++
 
 * First attempt to release on PyPI.
-
-
```

### Comparing `django-user-tasks-3.0.0/README.rst` & `django-user-tasks-3.1.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 django-user-tasks
 =================
 
 .. image:: https://img.shields.io/pypi/v/django-user-tasks.svg
     :target: https://pypi.python.org/pypi/django-user-tasks/
     :alt: PyPI
 
-.. image:: https://github.com/edx/django-user-tasks/workflows/Python%20CI/badge.svg?branch=master
-    :target: https://github.com/edx/django-user-tasks/actions?query=workflow%3A%22Python+CI%22
+.. image:: https://github.com/openedx/django-user-tasks/workflows/Python%20CI/badge.svg?branch=master
+    :target: https://github.com/openedx/django-user-tasks/actions?query=workflow%3A%22Python+CI%22
     :alt: CI
 
 .. image:: http://codecov.io/github/edx/django-user-tasks/coverage.svg?branch=master
     :target: http://codecov.io/github/edx/django-user-tasks?branch=master
     :alt: Codecov
 
 .. image:: https://readthedocs.org/projects/django-user-tasks/badge/?version=latest
@@ -18,15 +18,15 @@
     :alt: Documentation
 
 .. image:: https://img.shields.io/pypi/pyversions/django-user-tasks.svg
     :target: https://pypi.python.org/pypi/django-user-tasks/
     :alt: Supported Python versions
 
 .. image:: https://img.shields.io/github/license/edx/django-user-tasks.svg
-    :target: https://github.com/edx/django-user-tasks/blob/master/LICENSE.txt
+    :target: https://github.com/openedx/django-user-tasks/blob/master/LICENSE.txt
     :alt: License
 
 django-user-tasks is a reusable Django application for managing user-triggered
 asynchronous tasks.  It provides a status page for each such task, which
 includes a meaningful progress indicator if the task is currently being
 executed and provides any appropriate text and/or links for output once the
 task is complete.
@@ -86,18 +86,15 @@
 Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
-
-Even though they were written with ``edx-platform`` in mind, the guidelines
-should be followed for Open edX code in general.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org.
 
 Getting Help
```

### Comparing `django-user-tasks-3.0.0/django_user_tasks.egg-info/PKG-INFO` & `django-user-tasks-3.1.0/django_user_tasks.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: django-user-tasks
-Version: 3.0.0
+Version: 3.1.0
 Summary: Management of user-triggered asynchronous tasks in Django projects
-Home-page: https://github.com/edx/django-user-tasks
+Home-page: https://github.com/openedx/django-user-tasks
 Author: edX
 Author-email: oscm@edx.org
 License: Apache Software License 2.0
 Keywords: Django edx
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
@@ -24,16 +23,16 @@
 django-user-tasks
 =================
 
 .. image:: https://img.shields.io/pypi/v/django-user-tasks.svg
     :target: https://pypi.python.org/pypi/django-user-tasks/
     :alt: PyPI
 
-.. image:: https://github.com/edx/django-user-tasks/workflows/Python%20CI/badge.svg?branch=master
-    :target: https://github.com/edx/django-user-tasks/actions?query=workflow%3A%22Python+CI%22
+.. image:: https://github.com/openedx/django-user-tasks/workflows/Python%20CI/badge.svg?branch=master
+    :target: https://github.com/openedx/django-user-tasks/actions?query=workflow%3A%22Python+CI%22
     :alt: CI
 
 .. image:: http://codecov.io/github/edx/django-user-tasks/coverage.svg?branch=master
     :target: http://codecov.io/github/edx/django-user-tasks?branch=master
     :alt: Codecov
 
 .. image:: https://readthedocs.org/projects/django-user-tasks/badge/?version=latest
@@ -41,15 +40,15 @@
     :alt: Documentation
 
 .. image:: https://img.shields.io/pypi/pyversions/django-user-tasks.svg
     :target: https://pypi.python.org/pypi/django-user-tasks/
     :alt: Supported Python versions
 
 .. image:: https://img.shields.io/github/license/edx/django-user-tasks.svg
-    :target: https://github.com/edx/django-user-tasks/blob/master/LICENSE.txt
+    :target: https://github.com/openedx/django-user-tasks/blob/master/LICENSE.txt
     :alt: License
 
 django-user-tasks is a reusable Django application for managing user-triggered
 asynchronous tasks.  It provides a status page for each such task, which
 includes a meaningful progress indicator if the task is currently being
 executed and provides any appropriate text and/or links for output once the
 task is complete.
@@ -109,18 +108,15 @@
 Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
-
-Even though they were written with ``edx-platform`` in mind, the guidelines
-should be followed for Open edX code in general.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org.
 
 Getting Help
@@ -144,22 +140,40 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+
+[3.1.0] - 2023-07-21
+~~~~~~~~~~~~~~~~~~~~
+
+Added
++++++
+* Added Django42 support in CI.
+
 Removed
 +++++++
+* Removed old versions of celery and drf version from ci.
 
+Chore
++++++
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated
+
+[3.0.0] - 2022-02-09
+~~~~~~~~~~~~~~~~~~~~
+
+Removed
++++++++
 * Removed Python 3.5 support.
 
 Chore
 +++++
-
 * Upgraded celery to latest 5.x version.
 
 [2.2.0] - 2022-01-26
 ~~~~~~~~~~~~~~~~~~~~
 
 Removed
 +++++++
@@ -396,9 +410,7 @@
 [0.1.0] - 2016-10-07
 ~~~~~~~~~~~~~~~~~~~~
 
 Added
 +++++
 
 * First attempt to release on PyPI.
-
-
```

### Comparing `django-user-tasks-3.0.0/django_user_tasks.egg-info/SOURCES.txt` & `django-user-tasks-3.1.0/django_user_tasks.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -9,14 +9,20 @@
 django_user_tasks.egg-info/SOURCES.txt
 django_user_tasks.egg-info/dependency_links.txt
 django_user_tasks.egg-info/not-zip-safe
 django_user_tasks.egg-info/requires.txt
 django_user_tasks.egg-info/top_level.txt
 requirements/base.in
 requirements/constraints.txt
+tests/test_admin.py
+tests/test_models.py
+tests/test_rest_api.py
+tests/test_serializers.py
+tests/test_signals.py
+tests/test_tasks.py
 user_tasks/__init__.py
 user_tasks/admin.py
 user_tasks/apps.py
 user_tasks/conf.py
 user_tasks/exceptions.py
 user_tasks/filters.py
 user_tasks/models.py
```

### Comparing `django-user-tasks-3.0.0/requirements/constraints.txt` & `django-user-tasks-3.1.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `django-user-tasks-3.0.0/setup.cfg` & `django-user-tasks-3.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-user-tasks-3.0.0/setup.py` & `django-user-tasks-3.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,28 +103,28 @@
     name='django-user-tasks',
     version=VERSION,
     description="""Management of user-triggered asynchronous tasks in Django projects""",
     long_description=README + '\n\n' + CHANGELOG,
     long_description_content_type='text/x-rst',
     author='edX',
     author_email='oscm@edx.org',
-    url='https://github.com/edx/django-user-tasks',
+    url='https://github.com/openedx/django-user-tasks',
     packages=[
         'user_tasks',
     ],
     include_package_data=True,
     install_requires=load_requirements('requirements/base.in'),
     license="Apache Software License 2.0",
     zip_safe=False,
     keywords='Django edx',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Framework :: Django',
         'Framework :: Django :: 3.2',
-        'Framework :: Django :: 4.0',
+        'Framework :: Django :: 4.2',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
     ],
 )
```

### Comparing `django-user-tasks-3.0.0/user_tasks/admin.py` & `django-user-tasks-3.1.0/user_tasks/admin.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,35 +3,33 @@
 """
 
 from django.contrib import admin
 
 from .models import UserTaskArtifact, UserTaskStatus
 
 
+@admin.register(UserTaskArtifact)
 class UserTaskArtifactAdmin(admin.ModelAdmin):
     """
     Configuration for UserTaskArtifact admin panel.
     """
 
     list_display = ('created', 'uuid', 'status', 'name', 'text')
     list_filter = ('name',)
     ordering = ('-created',)
     search_fields = ('uuid', 'name', 'text')
     raw_id_fields = ('status',)
 
 
+@admin.register(UserTaskStatus)
 class UserTaskStatusAdmin(admin.ModelAdmin):
     """
     Configuration for UserTaskStatus admin panel.
     """
 
     list_display = ('created', 'uuid', 'state', 'user', 'name')
     list_filter = ('state',)
     ordering = ('-created',)
     search_fields = (
         'uuid', 'task_id', 'task_class', 'name', 'user__username', 'user__email'
     )
     readonly_fields = ('parent', )
-
-
-admin.site.register(UserTaskArtifact, UserTaskArtifactAdmin)
-admin.site.register(UserTaskStatus, UserTaskStatusAdmin)
```

### Comparing `django-user-tasks-3.0.0/user_tasks/conf.py` & `django-user-tasks-3.1.0/user_tasks/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,21 +48,21 @@
         should be configured to run on an appropriate schedule.  Note that the
         age is calculated from task creation, not completion.  The default
         value is 30 days.
         """
         return getattr(django_settings, 'USER_TASKS_MAX_AGE', timedelta(days=30))
 
     @property
-    def USER_TASKS_STATUS_FILTERS(self):  # pylint: disable=invalid-name
+    def USER_TASKS_STATUS_FILTERS(self):
         """
         Tuple containing zero or more filters for UserTaskStatus listing REST API calls.
 
         Each entry should be a Django REST Framework filter backend class
         object, such as ``django_filters.rest_framework.DjangoFilterBackend``.
         The default value contains only ``user_tasks.filters.StatusFilterBackend``,
         which allows superusers to see all task statuses but other users to see only
         those for tasks they triggered themselves.
         """
         return getattr(django_settings, 'USER_TASKS_STATUS_FILTERS', (filters.StatusFilterBackend,))
 
 
-settings = LazySettings()  # pylint: disable=invalid-name
+settings = LazySettings()
```

### Comparing `django-user-tasks-3.0.0/user_tasks/filters.py` & `django-user-tasks-3.1.0/user_tasks/filters.py`

 * *Files identical despite different names*

### Comparing `django-user-tasks-3.0.0/user_tasks/migrations/0001_initial.py` & `django-user-tasks-3.1.0/user_tasks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-user-tasks-3.0.0/user_tasks/migrations/0002_artifact_file_storage.py` & `django-user-tasks-3.1.0/user_tasks/migrations/0002_artifact_file_storage.py`

 * *Files identical despite different names*

### Comparing `django-user-tasks-3.0.0/user_tasks/models.py` & `django-user-tasks-3.1.0/user_tasks/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -106,26 +106,26 @@
         indication of progress, but not so often as to cause undue burden on
         the database.
         """
         UserTaskStatus.objects.filter(pk=self.id).update(completed_steps=F('completed_steps') + steps,
                                                          modified=now())
         self.refresh_from_db(fields={'completed_steps', 'modified', 'state'})
         if self.parent:
-            self.parent.increment_completed_steps(steps)  # pylint: disable=no-member
+            self.parent.increment_completed_steps(steps)
         # Was a cancellation command recently sent?
         if self.state == self.CANCELED and not self.is_container:
             raise TaskCanceledException
 
     def increment_total_steps(self, steps):
         """Increase the value of :py:attr:`total_steps` by the given number and save."""
         # Assume that other processes may be making concurrent changes
         UserTaskStatus.objects.filter(pk=self.id).update(total_steps=F('total_steps') + steps, modified=now())
         self.refresh_from_db(fields={'total_steps', 'modified'})
         if self.parent:
-            self.parent.increment_total_steps(steps)  # pylint: disable=no-member
+            self.parent.increment_total_steps(steps)
 
     def cancel(self):
         """
         Cancel the associated task if it hasn't already finished running.
         """
         if self.is_container:
             children = UserTaskStatus.objects.filter(parent=self)
@@ -153,15 +153,15 @@
         represents a container for multiple parallel tasks.
         """
         with transaction.atomic():
             UserTaskArtifact.objects.create(status=self, name='Error', text=message)
             self.state = UserTaskStatus.FAILED
             self.save(update_fields={'state', 'modified'})
         if self.parent:
-            self.parent.fail(message)  # pylint: disable=no-member
+            self.parent.fail(message)
 
     def retry(self):
         """
         Update the status to reflect that a problem was encountered and the task will be retried later.
         """
         # Note that a retry does not affect the state of a containing task
         # grouping; it's effectively still in progress
@@ -172,15 +172,15 @@
     def set_name(self, name):
         """
         Give the specified name to this status and all of its ancestors.
         """
         self.name = name
         self.save(update_fields={'name', 'modified'})
         if self.parent:
-            self.parent.set_name(name)  # pylint: disable=no-member
+            self.parent.set_name(name)
 
     def set_state(self, custom_state):
         """
         Set the state to a custom in-progress value.
 
         This can be done to indicate which stage of a long task is currently
         being executed, like "Sending email messages".
@@ -189,16 +189,16 @@
             status = UserTaskStatus.objects.select_for_update().get(pk=self.id)
             if status.state == UserTaskStatus.CANCELED and not self.is_container:
                 raise TaskCanceledException
             status.state = custom_state
             status.save(update_fields={'state', 'modified'})
             self.state = status.state
             self.modified = status.modified
-        if self.parent and self.parent.task_class != 'celery.group':  # pylint: disable=no-member
-            self.parent.set_state(custom_state)  # pylint: disable=no-member
+        if self.parent and self.parent.task_class != 'celery.group':
+            self.parent.set_state(custom_state)
 
     @property
     def state_text(self):
         """
         Get the translation into the current language of the current state of this status instance.
         """
         return self.STATE_TRANSLATIONS.get(self.state, self.state)
@@ -210,15 +210,15 @@
         if self.completed_steps < self.total_steps:
             self.increment_completed_steps(self.total_steps - self.completed_steps)
         self.state = UserTaskStatus.SUCCEEDED
         self.save(update_fields={'state', 'modified'})
         if self.parent_id:
             query = UserTaskStatus.objects.filter(~Q(state=UserTaskStatus.SUCCEEDED), parent__pk=self.parent_id)
             if not query.exists():
-                self.parent.succeed()  # pylint: disable=no-member
+                self.parent.succeed()
 
     def __str__(self):
         """
         Get a string representation of this task.
         """
         return f'<UserTaskStatus: {self.name}>'
```

### Comparing `django-user-tasks-3.0.0/user_tasks/rules.py` & `django-user-tasks-3.1.0/user_tasks/rules.py`

 * *Files identical despite different names*

### Comparing `django-user-tasks-3.0.0/user_tasks/serializers.py` & `django-user-tasks-3.1.0/user_tasks/serializers.py`

 * *Files identical despite different names*

### Comparing `django-user-tasks-3.0.0/user_tasks/signals.py` & `django-user-tasks-3.1.0/user_tasks/signals.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from .models import UserTaskStatus
 from .tasks import UserTaskMixin
 
 LOGGER = logging.getLogger(__name__)
 
 
 @before_task_publish.connect
-def create_user_task(sender=None, body=None, **kwargs):  # pylint: disable=unused-argument
+def create_user_task(sender=None, body=None, **kwargs):
     """
     Create a :py:class:`UserTaskStatus` record for each :py:class:`UserTaskMixin`.
 
     Also creates a :py:class:`UserTaskStatus` for each chain, chord, or group containing
     the new :py:class:`UserTaskMixin`.
     """
     try:
@@ -186,15 +186,15 @@
         get_user_model().objects.get(pk=user_id)
     except (ValueError, get_user_model().DoesNotExist) as import_exception:
         raise TypeError(f'Invalid user_id: {user_id}') from import_exception
     return user_id
 
 
 @task_prerun.connect
-def start_user_task(sender=None, **kwargs):  # pylint: disable=unused-argument
+def start_user_task(sender=None, **kwargs):
     """
     Update the status record when execution of a :py:class:`UserTaskMixin` begins.
     """
     try:
         current_connection = transaction.get_connection()
     except Exception:  # pylint: disable=broad-except
         current_connection = None
@@ -225,24 +225,24 @@
         if not isinstance(exception, TaskCanceledException):
             # Don't include traceback, since this is intended for end users
             sender.status.fail(str(exception))
         user_task_stopped.send_robust(sender=UserTaskStatus, status=sender.status)
 
 
 @task_retry.connect
-def retrying_task(sender=None, **kwargs):  # pylint: disable=unused-argument
+def retrying_task(sender=None, **kwargs):
     """
     Update the status record to reflect that a retry is pending.
     """
     if isinstance(sender, UserTaskMixin):
         sender.status.retry()
 
 
 @task_success.connect
-def task_succeeded(sender=None, **kwargs):  # pylint: disable=unused-argument
+def task_succeeded(sender=None, **kwargs):
     """
     Update the status record accordingly when a :py:class:`UserTaskMixin` finishes successfully.
     """
     if isinstance(sender, UserTaskMixin):
         status = sender.status
         # Failed tasks with good exception handling did not succeed just because they ended cleanly
         if status.state not in (UserTaskStatus.CANCELED, UserTaskStatus.FAILED, UserTaskStatus.RETRYING):
```

### Comparing `django-user-tasks-3.0.0/user_tasks/tasks.py` & `django-user-tasks-3.1.0/user_tasks/tasks.py`

 * *Files identical despite different names*

### Comparing `django-user-tasks-3.0.0/user_tasks/views.py` & `django-user-tasks-3.1.0/user_tasks/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     filter_backends = settings.USER_TASKS_STATUS_FILTERS
     lookup_field = 'uuid'
     permission_classes = (DjangoObjectPermissionsIncludingView,)
     queryset = UserTaskStatus.objects.order_by('-created')
     serializer_class = StatusSerializer
 
     @action(detail=True, methods=['post'])
-    def cancel(self, request, *args, **kwargs):  # pylint: disable=unused-argument
+    def cancel(self, request, *args, **kwargs):
         """
         Cancel the task associated with the specified status record.
 
         Arguments:
             request (Request): A POST including a task status record ID
 
         Returns:
```

