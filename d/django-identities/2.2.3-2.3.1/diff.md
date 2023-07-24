# Comparing `tmp/django-identities-2.2.3.tar.gz` & `tmp/django-identities-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-identities-2.2.3.tar", last modified: Tue Nov  8 13:11:36 2022, max compression
+gzip compressed data, was "django-identities-2.3.1.tar", last modified: Mon Jul 24 16:01:37 2023, max compression
```

## Comparing `django-identities-2.2.3.tar` & `django-identities-2.3.1.tar`

### file list

```diff
@@ -1,48 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-08 13:11:36.525368 django-identities-2.2.3/
--rw-rw-rw-   0 root         (0) root         (0)      117 2022-11-08 13:11:24.000000 django-identities-2.2.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4654 2022-11-08 13:11:36.525368 django-identities-2.2.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3605 2022-11-08 13:11:24.000000 django-identities-2.2.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-08 13:11:36.516368 django-identities-2.2.3/django_identities.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4654 2022-11-08 13:11:36.000000 django-identities-2.2.3/django_identities.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1224 2022-11-08 13:11:36.000000 django-identities-2.2.3/django_identities.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-08 13:11:36.000000 django-identities-2.2.3/django_identities.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-08 13:11:35.000000 django-identities-2.2.3/django_identities.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      276 2022-11-08 13:11:36.000000 django-identities-2.2.3/django_identities.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2022-11-08 13:11:36.000000 django-identities-2.2.3/django_identities.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-08 13:11:36.519368 django-identities-2.2.3/identities/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-11-08 13:11:24.000000 django-identities-2.2.3/identities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      428 2022-11-08 13:11:24.000000 django-identities-2.2.3/identities/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      173 2022-11-08 13:11:24.000000 django-identities-2.2.3/identities/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     1617 2022-11-08 13:11:24.000000 django-identities-2.2.3/identities/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-08 13:11:36.521368 django-identities-2.2.3/identities/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     8068 2022-11-08 13:11:24.000000 django-identities-2.2.3/identities/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      403 2022-11-08 13:11:24.000000 django-identities-2.2.3/identities/migrations/0002_remove_tech_account.py
--rw-rw-rw-   0 root         (0) root         (0)     4759 2022-11-08 13:11:24.000000 django-identities-2.2.3/identities/migrations/0003_historicaluser.py
--rw-rw-rw-   0 root         (0) root         (0)      475 2022-11-08 13:11:24.000000 django-identities-2.2.3/identities/migrations/0004_alter_historicaluser_id.py
--rw-rw-rw-   0 root         (0) root         (0)     1311 2022-11-08 13:11:24.000000 django-identities-2.2.3/identities/migrations/0005_alter_historicalprofile_options_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-08 13:11:24.000000 django-identities-2.2.3/identities/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1769 2022-11-08 13:11:24.000000 django-identities-2.2.3/identities/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1620 2022-11-08 13:11:24.000000 django-identities-2.2.3/identities/oidc.py
--rw-rw-rw-   0 root         (0) root         (0)     6800 2022-11-08 13:11:24.000000 django-identities-2.2.3/identities/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-08 13:11:24.000000 django-identities-2.2.3/identities/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-08 13:11:36.523368 django-identities-2.2.3/identities/serializers/
--rw-rw-rw-   0 root         (0) root         (0)      345 2022-11-08 13:11:24.000000 django-identities-2.2.3/identities/serializers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5120 2022-11-08 13:11:24.000000 django-identities-2.2.3/identities/serializers/group.py
--rw-rw-rw-   0 root         (0) root         (0)      882 2022-11-08 13:11:24.000000 django-identities-2.2.3/identities/serializers/permission.py
--rw-rw-rw-   0 root         (0) root         (0)      730 2022-11-08 13:11:24.000000 django-identities-2.2.3/identities/serializers/profile.py
--rw-rw-rw-   0 root         (0) root         (0)     3027 2022-11-08 13:11:24.000000 django-identities-2.2.3/identities/serializers/user.py
--rw-rw-rw-   0 root         (0) root         (0)     1424 2022-11-08 13:11:24.000000 django-identities-2.2.3/identities/serializers/userinfo.py
--rw-rw-rw-   0 root         (0) root         (0)      154 2022-11-08 13:11:24.000000 django-identities-2.2.3/identities/serializers/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-08 13:11:36.524368 django-identities-2.2.3/identities/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-08 13:11:24.000000 django-identities-2.2.3/identities/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1460 2022-11-08 13:11:24.000000 django-identities-2.2.3/identities/tests/factories.py
--rw-rw-rw-   0 root         (0) root         (0)      928 2022-11-08 13:11:24.000000 django-identities-2.2.3/identities/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     2803 2022-11-08 13:11:24.000000 django-identities-2.2.3/identities/user_utils.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-11-08 13:11:24.000000 django-identities-2.2.3/identities/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-08 13:11:36.525368 django-identities-2.2.3/identities/views/
--rw-rw-rw-   0 root         (0) root         (0)      225 2022-11-08 13:11:24.000000 django-identities-2.2.3/identities/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      801 2022-11-08 13:11:24.000000 django-identities-2.2.3/identities/views/group.py
--rw-rw-rw-   0 root         (0) root         (0)     3183 2022-11-08 13:11:24.000000 django-identities-2.2.3/identities/views/permission.py
--rw-rw-rw-   0 root         (0) root         (0)     3105 2022-11-08 13:11:24.000000 django-identities-2.2.3/identities/views/user.py
--rw-rw-rw-   0 root         (0) root         (0)     1633 2022-11-08 13:11:24.000000 django-identities-2.2.3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1510 2022-11-08 13:11:36.526368 django-identities-2.2.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 16:01:37.620988 django-identities-2.3.1/
+-rw-rw-rw-   0 root         (0) root         (0)      117 2023-07-24 16:01:27.000000 django-identities-2.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4475 2023-07-24 16:01:37.620988 django-identities-2.3.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3598 2023-07-24 16:01:27.000000 django-identities-2.3.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 16:01:37.615988 django-identities-2.3.1/django_identities.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4475 2023-07-24 16:01:37.000000 django-identities-2.3.1/django_identities.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1296 2023-07-24 16:01:37.000000 django-identities-2.3.1/django_identities.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 16:01:37.000000 django-identities-2.3.1/django_identities.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 16:01:36.000000 django-identities-2.3.1/django_identities.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      310 2023-07-24 16:01:37.000000 django-identities-2.3.1/django_identities.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-24 16:01:37.000000 django-identities-2.3.1/django_identities.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 16:01:37.617988 django-identities-2.3.1/identities/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-07-24 16:01:27.000000 django-identities-2.3.1/identities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      428 2023-07-24 16:01:27.000000 django-identities-2.3.1/identities/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-07-24 16:01:27.000000 django-identities-2.3.1/identities/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     1617 2023-07-24 16:01:27.000000 django-identities-2.3.1/identities/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 16:01:37.618988 django-identities-2.3.1/identities/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     8067 2023-07-24 16:01:27.000000 django-identities-2.3.1/identities/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      403 2023-07-24 16:01:27.000000 django-identities-2.3.1/identities/migrations/0002_remove_tech_account.py
+-rw-rw-rw-   0 root         (0) root         (0)     4758 2023-07-24 16:01:27.000000 django-identities-2.3.1/identities/migrations/0003_historicaluser.py
+-rw-rw-rw-   0 root         (0) root         (0)      474 2023-07-24 16:01:27.000000 django-identities-2.3.1/identities/migrations/0004_alter_historicaluser_id.py
+-rw-rw-rw-   0 root         (0) root         (0)     1310 2023-07-24 16:01:27.000000 django-identities-2.3.1/identities/migrations/0005_alter_historicalprofile_options_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 16:01:27.000000 django-identities-2.3.1/identities/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1769 2023-07-24 16:01:27.000000 django-identities-2.3.1/identities/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1620 2023-07-24 16:01:27.000000 django-identities-2.3.1/identities/oidc.py
+-rw-rw-rw-   0 root         (0) root         (0)     6800 2023-07-24 16:01:27.000000 django-identities-2.3.1/identities/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 16:01:27.000000 django-identities-2.3.1/identities/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 16:01:37.619988 django-identities-2.3.1/identities/serializers/
+-rw-rw-rw-   0 root         (0) root         (0)      345 2023-07-24 16:01:27.000000 django-identities-2.3.1/identities/serializers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5120 2023-07-24 16:01:27.000000 django-identities-2.3.1/identities/serializers/group.py
+-rw-rw-rw-   0 root         (0) root         (0)      882 2023-07-24 16:01:27.000000 django-identities-2.3.1/identities/serializers/permission.py
+-rw-rw-rw-   0 root         (0) root         (0)      730 2023-07-24 16:01:27.000000 django-identities-2.3.1/identities/serializers/profile.py
+-rw-rw-rw-   0 root         (0) root         (0)     3027 2023-07-24 16:01:27.000000 django-identities-2.3.1/identities/serializers/user.py
+-rw-rw-rw-   0 root         (0) root         (0)     1424 2023-07-24 16:01:27.000000 django-identities-2.3.1/identities/serializers/userinfo.py
+-rw-rw-rw-   0 root         (0) root         (0)      154 2023-07-24 16:01:27.000000 django-identities-2.3.1/identities/serializers/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 16:01:37.619988 django-identities-2.3.1/identities/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 16:01:27.000000 django-identities-2.3.1/identities/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1460 2023-07-24 16:01:27.000000 django-identities-2.3.1/identities/tests/factories.py
+-rw-rw-rw-   0 root         (0) root         (0)      928 2023-07-24 16:01:27.000000 django-identities-2.3.1/identities/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     2931 2023-07-24 16:01:27.000000 django-identities-2.3.1/identities/user_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-24 16:01:27.000000 django-identities-2.3.1/identities/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 16:01:37.620988 django-identities-2.3.1/identities/views/
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-07-24 16:01:27.000000 django-identities-2.3.1/identities/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      801 2023-07-24 16:01:27.000000 django-identities-2.3.1/identities/views/group.py
+-rw-rw-rw-   0 root         (0) root         (0)     3183 2023-07-24 16:01:27.000000 django-identities-2.3.1/identities/views/permission.py
+-rw-rw-rw-   0 root         (0) root         (0)     3105 2023-07-24 16:01:27.000000 django-identities-2.3.1/identities/views/user.py
+-rw-rw-rw-   0 root         (0) root         (0)     1590 2023-07-24 16:01:27.000000 django-identities-2.3.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1430 2023-07-24 16:01:37.621988 django-identities-2.3.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 16:01:37.620988 django-identities-2.3.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1217 2023-07-24 16:01:27.000000 django-identities-2.3.1/tests/test_models.py
+-rw-rw-rw-   0 root         (0) root         (0)    10288 2023-07-24 16:01:27.000000 django-identities-2.3.1/tests/test_permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5525 2023-07-24 16:01:27.000000 django-identities-2.3.1/tests/test_user_utils.py
```

### Comparing `django-identities-2.2.3/PKG-INFO` & `django-identities-2.3.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 Metadata-Version: 2.1
 Name: django-identities
-Version: 2.2.3
+Version: 2.3.1
 Summary: A django app with authentication related functionality, a custom user model and object level permissions / groups.
 Home-page: https://gitlab.com/biomedit/django-identities
 Author: Jarosław Surkont, Gerhard Bräunlich, Robin Engler, Christian Ribeaud, François Martin
 Author-email: jaroslaw.surkont@unibas.ch, gerhard.braeunlich@id.ethz.ch, robin.engler@sib.swiss, christian.ribeaud@karakun.com, francois.martin@karakun.com
 License: LGPL3
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: stubs
+Provides-Extra: dev
 
-[![pipeline status](https://gitlab.com/biomedit/django-identities/badges/master/pipeline.svg)](https://gitlab.com/biomedit/django-identities/-/commits/master)
-[![coverage report](https://gitlab.com/biomedit/django-identities/badges/master/coverage.svg)](https://gitlab.com/biomedit/django-identities/-/commits/master)
+[![pipeline status](https://gitlab.com/biomedit/django-identities/badges/main/pipeline.svg)](https://gitlab.com/biomedit/django-identities/-/commits/main)
+[![coverage report](https://gitlab.com/biomedit/django-identities/badges/main/coverage.svg)](https://gitlab.com/biomedit/django-identities/-/commits/main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![python version](https://img.shields.io/pypi/pyversions/django-identities.svg)](https://pypi.org/project/django-identities)
 [![license](https://img.shields.io/badge/License-LGPLv3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0)
 [![latest version](https://img.shields.io/pypi/v/django-identities.svg)](https://pypi.org/project/django-identities)
 
 # django-identities
 
@@ -32,15 +28,15 @@
 
 This project follows the [semantic versioning specification](https://semver.org/) for its releases.
 
 ## Development
 
 ### Requirements
 
-- Python >=3.7
+- Python >=3.10
 - Django >=3.2
 - django-rest-framework >=3.12
 
 ### Setup
 
 - Create and activate a python3 venv.
 - Install the library in the editable mode `pip install -e .[test,stubs]`
```

#### html2text {}

```diff
@@ -1,41 +1,39 @@
-Metadata-Version: 2.1 Name: django-identities Version: 2.2.3 Summary: A django
+Metadata-Version: 2.1 Name: django-identities Version: 2.3.1 Summary: A django
 app with authentication related functionality, a custom user model and object
 level permissions / groups. Home-page: https://gitlab.com/biomedit/django-
 identities Author: JarosÅaw Surkont, Gerhard BrÃ¤unlich, Robin Engler,
 Christian Ribeaud, FranÃ§ois Martin Author-email: jaroslaw.surkont@unibas.ch,
 gerhard.braeunlich@id.ethz.ch, robin.engler@sib.swiss,
 christian.ribeaud@karakun.com, francois.martin@karakun.com License: LGPL3
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3
-(LGPLv3) Classifier: Operating System :: OS Independent Requires-Python: >=3.7
-Description-Content-Type: text/markdown Provides-Extra: test Provides-Extra:
-stubs [![pipeline status](https://gitlab.com/biomedit/django-identities/badges/
-master/pipeline.svg)](https://gitlab.com/biomedit/django-identities/-/commits/
-master) [![coverage report](https://gitlab.com/biomedit/django-identities/
-badges/master/coverage.svg)](https://gitlab.com/biomedit/django-identities/-/
-commits/master) [![Code style: black](https://img.shields.io/badge/
-code%20style-black-000000.svg)](https://github.com/psf/black) [![python
-version](https://img.shields.io/pypi/pyversions/django-identities.svg)](https:/
-/pypi.org/project/django-identities) [![license](https://img.shields.io/badge/
-License-LGPLv3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0) [![latest
-version](https://img.shields.io/pypi/v/django-identities.svg)](https://
-pypi.org/project/django-identities) # django-identities ## Releases This
-project follows the [semantic versioning specification](https://semver.org/
-) for its releases. ## Development ### Requirements - Python >=3.7 - Django
->=3.2 - django-rest-framework >=3.12 ### Setup - Create and activate a python3
-venv. - Install the library in the editable mode `pip install -e .[test,stubs]`
-- Install dev requirements `pip install -r requirements-dev.txt`. - Install git
-hooks to automatically format code using black with `pre-commit install` ###
-Migrations To create migrations after modifying database models run `./
-manage.py makemigrations` ## Installation ### From git in `requirements.txt` 1.
-To install this package from this git repository, add the `django-identities`
+(LGPLv3) Classifier: Operating System :: OS Independent Requires-Python: >=3.10
+Description-Content-Type: text/markdown Provides-Extra: dev [![pipeline status]
+(https://gitlab.com/biomedit/django-identities/badges/main/pipeline.svg)]
+(https://gitlab.com/biomedit/django-identities/-/commits/main) [![coverage
+report](https://gitlab.com/biomedit/django-identities/badges/main/
+coverage.svg)](https://gitlab.com/biomedit/django-identities/-/commits/main) [!
+[Code style: black](https://img.shields.io/badge/code%20style-black-
+000000.svg)](https://github.com/psf/black) [![python version](https://
+img.shields.io/pypi/pyversions/django-identities.svg)](https://pypi.org/
+project/django-identities) [![license](https://img.shields.io/badge/License-
+LGPLv3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0) [![latest version]
+(https://img.shields.io/pypi/v/django-identities.svg)](https://pypi.org/
+project/django-identities) # django-identities ## Releases This project follows
+the [semantic versioning specification](https://semver.org/) for its releases.
+## Development ### Requirements - Python >=3.10 - Django >=3.2 - django-rest-
+framework >=3.12 ### Setup - Create and activate a python3 venv. - Install the
+library in the editable mode `pip install -e .[test,stubs]` - Install dev
+requirements `pip install -r requirements-dev.txt`. - Install git hooks to
+automatically format code using black with `pre-commit install` ### Migrations
+To create migrations after modifying database models run `./manage.py
+makemigrations` ## Installation ### From git in `requirements.txt` 1. To
+install this package from this git repository, add the `django-identities`
 package to the `requirements.txt` file. 2. Add `guardian` and `identities` to
 `settings.INSTALLED_APPS`: ```python INSTALLED_APPS = ( #... 'guardian',
 'identities', #... ) ``` 3. Add the following to your `settings`, replacing all
 values with `REPLACE` with your configuration: ```python AUTH_USER_MODEL =
 "identities.User" GUARDIAN_MONKEY_PATCH = False
 GUARDIAN_GET_INIT_ANONYMOUS_USER =
 "identities.models.get_anonymous_user_instance" AUTHENTICATION_BACKENDS =
```

### Comparing `django-identities-2.2.3/README.md` & `django-identities-2.3.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-[![pipeline status](https://gitlab.com/biomedit/django-identities/badges/master/pipeline.svg)](https://gitlab.com/biomedit/django-identities/-/commits/master)
-[![coverage report](https://gitlab.com/biomedit/django-identities/badges/master/coverage.svg)](https://gitlab.com/biomedit/django-identities/-/commits/master)
+[![pipeline status](https://gitlab.com/biomedit/django-identities/badges/main/pipeline.svg)](https://gitlab.com/biomedit/django-identities/-/commits/main)
+[![coverage report](https://gitlab.com/biomedit/django-identities/badges/main/coverage.svg)](https://gitlab.com/biomedit/django-identities/-/commits/main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![python version](https://img.shields.io/pypi/pyversions/django-identities.svg)](https://pypi.org/project/django-identities)
 [![license](https://img.shields.io/badge/License-LGPLv3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0)
 [![latest version](https://img.shields.io/pypi/v/django-identities.svg)](https://pypi.org/project/django-identities)
 
 # django-identities
 
@@ -11,15 +11,15 @@
 
 This project follows the [semantic versioning specification](https://semver.org/) for its releases.
 
 ## Development
 
 ### Requirements
 
-- Python >=3.7
+- Python >=3.10
 - Django >=3.2
 - django-rest-framework >=3.12
 
 ### Setup
 
 - Create and activate a python3 venv.
 - Install the library in the editable mode `pip install -e .[test,stubs]`
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
-[![pipeline status](https://gitlab.com/biomedit/django-identities/badges/
-master/pipeline.svg)](https://gitlab.com/biomedit/django-identities/-/commits/
-master) [![coverage report](https://gitlab.com/biomedit/django-identities/
-badges/master/coverage.svg)](https://gitlab.com/biomedit/django-identities/-/
-commits/master) [![Code style: black](https://img.shields.io/badge/
-code%20style-black-000000.svg)](https://github.com/psf/black) [![python
-version](https://img.shields.io/pypi/pyversions/django-identities.svg)](https:/
-/pypi.org/project/django-identities) [![license](https://img.shields.io/badge/
-License-LGPLv3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0) [![latest
-version](https://img.shields.io/pypi/v/django-identities.svg)](https://
-pypi.org/project/django-identities) # django-identities ## Releases This
-project follows the [semantic versioning specification](https://semver.org/
-) for its releases. ## Development ### Requirements - Python >=3.7 - Django
->=3.2 - django-rest-framework >=3.12 ### Setup - Create and activate a python3
-venv. - Install the library in the editable mode `pip install -e .[test,stubs]`
-- Install dev requirements `pip install -r requirements-dev.txt`. - Install git
-hooks to automatically format code using black with `pre-commit install` ###
-Migrations To create migrations after modifying database models run `./
-manage.py makemigrations` ## Installation ### From git in `requirements.txt` 1.
-To install this package from this git repository, add the `django-identities`
+[![pipeline status](https://gitlab.com/biomedit/django-identities/badges/main/
+pipeline.svg)](https://gitlab.com/biomedit/django-identities/-/commits/main) [!
+[coverage report](https://gitlab.com/biomedit/django-identities/badges/main/
+coverage.svg)](https://gitlab.com/biomedit/django-identities/-/commits/main) [!
+[Code style: black](https://img.shields.io/badge/code%20style-black-
+000000.svg)](https://github.com/psf/black) [![python version](https://
+img.shields.io/pypi/pyversions/django-identities.svg)](https://pypi.org/
+project/django-identities) [![license](https://img.shields.io/badge/License-
+LGPLv3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0) [![latest version]
+(https://img.shields.io/pypi/v/django-identities.svg)](https://pypi.org/
+project/django-identities) # django-identities ## Releases This project follows
+the [semantic versioning specification](https://semver.org/) for its releases.
+## Development ### Requirements - Python >=3.10 - Django >=3.2 - django-rest-
+framework >=3.12 ### Setup - Create and activate a python3 venv. - Install the
+library in the editable mode `pip install -e .[test,stubs]` - Install dev
+requirements `pip install -r requirements-dev.txt`. - Install git hooks to
+automatically format code using black with `pre-commit install` ### Migrations
+To create migrations after modifying database models run `./manage.py
+makemigrations` ## Installation ### From git in `requirements.txt` 1. To
+install this package from this git repository, add the `django-identities`
 package to the `requirements.txt` file. 2. Add `guardian` and `identities` to
 `settings.INSTALLED_APPS`: ```python INSTALLED_APPS = ( #... 'guardian',
 'identities', #... ) ``` 3. Add the following to your `settings`, replacing all
 values with `REPLACE` with your configuration: ```python AUTH_USER_MODEL =
 "identities.User" GUARDIAN_MONKEY_PATCH = False
 GUARDIAN_GET_INIT_ANONYMOUS_USER =
 "identities.models.get_anonymous_user_instance" AUTHENTICATION_BACKENDS =
```

### Comparing `django-identities-2.2.3/django_identities.egg-info/PKG-INFO` & `django-identities-2.3.1/django_identities.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 Metadata-Version: 2.1
 Name: django-identities
-Version: 2.2.3
+Version: 2.3.1
 Summary: A django app with authentication related functionality, a custom user model and object level permissions / groups.
 Home-page: https://gitlab.com/biomedit/django-identities
 Author: Jarosław Surkont, Gerhard Bräunlich, Robin Engler, Christian Ribeaud, François Martin
 Author-email: jaroslaw.surkont@unibas.ch, gerhard.braeunlich@id.ethz.ch, robin.engler@sib.swiss, christian.ribeaud@karakun.com, francois.martin@karakun.com
 License: LGPL3
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: stubs
+Provides-Extra: dev
 
-[![pipeline status](https://gitlab.com/biomedit/django-identities/badges/master/pipeline.svg)](https://gitlab.com/biomedit/django-identities/-/commits/master)
-[![coverage report](https://gitlab.com/biomedit/django-identities/badges/master/coverage.svg)](https://gitlab.com/biomedit/django-identities/-/commits/master)
+[![pipeline status](https://gitlab.com/biomedit/django-identities/badges/main/pipeline.svg)](https://gitlab.com/biomedit/django-identities/-/commits/main)
+[![coverage report](https://gitlab.com/biomedit/django-identities/badges/main/coverage.svg)](https://gitlab.com/biomedit/django-identities/-/commits/main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![python version](https://img.shields.io/pypi/pyversions/django-identities.svg)](https://pypi.org/project/django-identities)
 [![license](https://img.shields.io/badge/License-LGPLv3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0)
 [![latest version](https://img.shields.io/pypi/v/django-identities.svg)](https://pypi.org/project/django-identities)
 
 # django-identities
 
@@ -32,15 +28,15 @@
 
 This project follows the [semantic versioning specification](https://semver.org/) for its releases.
 
 ## Development
 
 ### Requirements
 
-- Python >=3.7
+- Python >=3.10
 - Django >=3.2
 - django-rest-framework >=3.12
 
 ### Setup
 
 - Create and activate a python3 venv.
 - Install the library in the editable mode `pip install -e .[test,stubs]`
```

#### html2text {}

```diff
@@ -1,41 +1,39 @@
-Metadata-Version: 2.1 Name: django-identities Version: 2.2.3 Summary: A django
+Metadata-Version: 2.1 Name: django-identities Version: 2.3.1 Summary: A django
 app with authentication related functionality, a custom user model and object
 level permissions / groups. Home-page: https://gitlab.com/biomedit/django-
 identities Author: JarosÅaw Surkont, Gerhard BrÃ¤unlich, Robin Engler,
 Christian Ribeaud, FranÃ§ois Martin Author-email: jaroslaw.surkont@unibas.ch,
 gerhard.braeunlich@id.ethz.ch, robin.engler@sib.swiss,
 christian.ribeaud@karakun.com, francois.martin@karakun.com License: LGPL3
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3
-(LGPLv3) Classifier: Operating System :: OS Independent Requires-Python: >=3.7
-Description-Content-Type: text/markdown Provides-Extra: test Provides-Extra:
-stubs [![pipeline status](https://gitlab.com/biomedit/django-identities/badges/
-master/pipeline.svg)](https://gitlab.com/biomedit/django-identities/-/commits/
-master) [![coverage report](https://gitlab.com/biomedit/django-identities/
-badges/master/coverage.svg)](https://gitlab.com/biomedit/django-identities/-/
-commits/master) [![Code style: black](https://img.shields.io/badge/
-code%20style-black-000000.svg)](https://github.com/psf/black) [![python
-version](https://img.shields.io/pypi/pyversions/django-identities.svg)](https:/
-/pypi.org/project/django-identities) [![license](https://img.shields.io/badge/
-License-LGPLv3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0) [![latest
-version](https://img.shields.io/pypi/v/django-identities.svg)](https://
-pypi.org/project/django-identities) # django-identities ## Releases This
-project follows the [semantic versioning specification](https://semver.org/
-) for its releases. ## Development ### Requirements - Python >=3.7 - Django
->=3.2 - django-rest-framework >=3.12 ### Setup - Create and activate a python3
-venv. - Install the library in the editable mode `pip install -e .[test,stubs]`
-- Install dev requirements `pip install -r requirements-dev.txt`. - Install git
-hooks to automatically format code using black with `pre-commit install` ###
-Migrations To create migrations after modifying database models run `./
-manage.py makemigrations` ## Installation ### From git in `requirements.txt` 1.
-To install this package from this git repository, add the `django-identities`
+(LGPLv3) Classifier: Operating System :: OS Independent Requires-Python: >=3.10
+Description-Content-Type: text/markdown Provides-Extra: dev [![pipeline status]
+(https://gitlab.com/biomedit/django-identities/badges/main/pipeline.svg)]
+(https://gitlab.com/biomedit/django-identities/-/commits/main) [![coverage
+report](https://gitlab.com/biomedit/django-identities/badges/main/
+coverage.svg)](https://gitlab.com/biomedit/django-identities/-/commits/main) [!
+[Code style: black](https://img.shields.io/badge/code%20style-black-
+000000.svg)](https://github.com/psf/black) [![python version](https://
+img.shields.io/pypi/pyversions/django-identities.svg)](https://pypi.org/
+project/django-identities) [![license](https://img.shields.io/badge/License-
+LGPLv3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0) [![latest version]
+(https://img.shields.io/pypi/v/django-identities.svg)](https://pypi.org/
+project/django-identities) # django-identities ## Releases This project follows
+the [semantic versioning specification](https://semver.org/) for its releases.
+## Development ### Requirements - Python >=3.10 - Django >=3.2 - django-rest-
+framework >=3.12 ### Setup - Create and activate a python3 venv. - Install the
+library in the editable mode `pip install -e .[test,stubs]` - Install dev
+requirements `pip install -r requirements-dev.txt`. - Install git hooks to
+automatically format code using black with `pre-commit install` ### Migrations
+To create migrations after modifying database models run `./manage.py
+makemigrations` ## Installation ### From git in `requirements.txt` 1. To
+install this package from this git repository, add the `django-identities`
 package to the `requirements.txt` file. 2. Add `guardian` and `identities` to
 `settings.INSTALLED_APPS`: ```python INSTALLED_APPS = ( #... 'guardian',
 'identities', #... ) ``` 3. Add the following to your `settings`, replacing all
 values with `REPLACE` with your configuration: ```python AUTH_USER_MODEL =
 "identities.User" GUARDIAN_MONKEY_PATCH = False
 GUARDIAN_GET_INIT_ANONYMOUS_USER =
 "identities.models.get_anonymous_user_instance" AUTHENTICATION_BACKENDS =
```

### Comparing `django-identities-2.2.3/django_identities.egg-info/SOURCES.txt` & `django-identities-2.3.1/django_identities.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -33,8 +33,11 @@
 identities/serializers/userinfo.py
 identities/serializers/utils.py
 identities/tests/__init__.py
 identities/tests/factories.py
 identities/views/__init__.py
 identities/views/group.py
 identities/views/permission.py
-identities/views/user.py
+identities/views/user.py
+tests/test_models.py
+tests/test_permissions.py
+tests/test_user_utils.py
```

### Comparing `django-identities-2.2.3/identities/filters.py` & `django-identities-2.3.1/identities/filters.py`

 * *Files identical despite different names*

### Comparing `django-identities-2.2.3/identities/migrations/0001_initial.py` & `django-identities-2.3.1/identities/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import django.db.models.deletion
 import django.utils.timezone
 import guardian.mixins
 import simple_history.models
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = [
         ("auth", "0012_alter_user_first_name_max_length"),
     ]
 
     operations = [
```

### Comparing `django-identities-2.2.3/identities/migrations/0003_historicaluser.py` & `django-identities-2.3.1/identities/migrations/0003_historicaluser.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from django.db import migrations, models
 import django.db.models.deletion
 import django.utils.timezone
 import simple_history.models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("identities", "0002_remove_tech_account"),
     ]
 
     operations = [
         migrations.CreateModel(
             name="HistoricalUser",
```

### Comparing `django-identities-2.2.3/identities/migrations/0005_alter_historicalprofile_options_and_more.py` & `django-identities-2.3.1/identities/migrations/0005_alter_historicalprofile_options_and_more.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 4.0.6 on 2022-11-04 07:36
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("identities", "0004_alter_historicaluser_id"),
     ]
 
     operations = [
         migrations.AlterModelOptions(
             name="historicalprofile",
```

### Comparing `django-identities-2.2.3/identities/models.py` & `django-identities-2.3.1/identities/models.py`

 * *Files identical despite different names*

### Comparing `django-identities-2.2.3/identities/oidc.py` & `django-identities-2.3.1/identities/oidc.py`

 * *Files identical despite different names*

### Comparing `django-identities-2.2.3/identities/permissions.py` & `django-identities-2.3.1/identities/permissions.py`

 * *Files identical despite different names*

### Comparing `django-identities-2.2.3/identities/serializers/group.py` & `django-identities-2.3.1/identities/serializers/group.py`

 * *Files identical despite different names*

### Comparing `django-identities-2.2.3/identities/serializers/permission.py` & `django-identities-2.3.1/identities/serializers/permission.py`

 * *Files identical despite different names*

### Comparing `django-identities-2.2.3/identities/serializers/profile.py` & `django-identities-2.3.1/identities/serializers/profile.py`

 * *Files identical despite different names*

### Comparing `django-identities-2.2.3/identities/serializers/user.py` & `django-identities-2.3.1/identities/serializers/user.py`

 * *Files identical despite different names*

### Comparing `django-identities-2.2.3/identities/serializers/userinfo.py` & `django-identities-2.3.1/identities/serializers/userinfo.py`

 * *Files identical despite different names*

### Comparing `django-identities-2.2.3/identities/tests/factories.py` & `django-identities-2.3.1/identities/tests/factories.py`

 * *Files identical despite different names*

### Comparing `django-identities-2.2.3/identities/urls.py` & `django-identities-2.3.1/identities/urls.py`

 * *Files identical despite different names*

### Comparing `django-identities-2.2.3/identities/views/group.py` & `django-identities-2.3.1/identities/views/group.py`

 * *Files identical despite different names*

### Comparing `django-identities-2.2.3/identities/views/permission.py` & `django-identities-2.3.1/identities/views/permission.py`

 * *Files identical despite different names*

### Comparing `django-identities-2.2.3/identities/views/user.py` & `django-identities-2.3.1/identities/views/user.py`

 * *Files identical despite different names*

### Comparing `django-identities-2.2.3/pyproject.toml` & `django-identities-2.3.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -11,26 +11,26 @@
   "*/wsgi.py",
   "*/asgi.py",
 ]
 
 [tool.tox]
 legacy_tox_ini = '''
 [tox]
-envlist = py{37,38,39,310,311},report
+envlist = py{310,311},report
 isolated_build = true
 
 [testenv]
 setenv =
     SECRET_KEY = test
     USE_LOGGING = False
     PYTHONPATH = tests
     DJANGO_SETTINGS_MODULE = settings
-    py{37,38,39,310,311}: COVERAGE_FILE = .coverage.{envname}
+    py{310,311}: COVERAGE_FILE = .coverage.{envname}
 depends =
-    report: py{37,38,39,310,311}
+    report: py{310,311}
 deps =
     assertpy
     factory_boy
     pylint
     pylint-django
     pytest
     pytest-cov
@@ -63,15 +63,14 @@
 
 [tool.mypy]
 files = ["identities", "tests"]
 plugins = ["mypy_django_plugin.main", "mypy_drf_plugin.main"]
 
 [[tool.mypy.overrides]]
 module = [
-    "assertpy",
     "authlib.*",
     "factory",
     "simple_history.*",
     "guardian.*",
 ]
 ignore_missing_imports = true
```

### Comparing `django-identities-2.2.3/setup.cfg` & `django-identities-2.3.1/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -6,17 +6,14 @@
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Jarosław Surkont, Gerhard Bräunlich, Robin Engler, Christian Ribeaud, François Martin
 author_email = jaroslaw.surkont@unibas.ch, gerhard.braeunlich@id.ethz.ch, robin.engler@sib.swiss, christian.ribeaud@karakun.com, francois.martin@karakun.com
 url = https://gitlab.com/biomedit/django-identities
 classifiers = 
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 	Operating System :: OS Independent
 
 [options]
 install_requires = 
@@ -24,31 +21,32 @@
 	djangorestframework>=3.12
 	django-simple-history>=3.1.1
 	django-guardian>=2.4
 	authlib>=0.15
 	django-drf-utils>=2.0.0
 packages = find:
 zip_safe = False
-python_requires = >=3.7
+python_requires = >=3.10
 
 [options.package_data]
 identities = py.typed
 
 [options.extras_require]
-test = 
-	assertpy
-	factory_boy
-	pytest
+dev = 
+	pylint==2.17.4
+	pylint-django==2.5.3
+	mypy==1.4.1
+	black==23.7.0
+	pytest==7.4.0
 	pytest-django
 	requests
-	pylint
-	pylint-django
-stubs = 
+	bandit==1.7.5
+	pytest-factoryboy==2.5.1
 	django-stubs
-	djangorestframework-stubs[compatible-mypy]>=1.7
+	djangorestframework-stubs
 
 [options.packages.find]
 exclude = 
 	tests
 	tests.*
 
 [egg_info]
```

