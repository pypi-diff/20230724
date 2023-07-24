# Comparing `tmp/openedx-django-require-2.0.0.tar.gz` & `tmp/openedx-django-require-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openedx-django-require-2.0.0.tar", last modified: Fri Nov 11 07:10:06 2022, max compression
+gzip compressed data, was "openedx-django-require-2.1.0.tar", last modified: Mon Jul 24 07:11:36 2023, max compression
```

## Comparing `openedx-django-require-2.0.0.tar` & `openedx-django-require-2.1.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 07:10:06.264471 openedx-django-require-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-11-11 07:10:00.000000 openedx-django-require-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1524 2022-11-11 07:10:00.000000 openedx-django-require-2.0.0/LICENSE-BSD-3c
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-11-11 07:10:00.000000 openedx-django-require-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      759 2022-11-11 07:10:06.264471 openedx-django-require-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9483 2022-11-11 07:10:00.000000 openedx-django-require-2.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 07:10:06.252471 openedx-django-require-2.0.0/openedx_django_require.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      759 2022-11-11 07:10:05.000000 openedx-django-require-2.0.0/openedx_django_require.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      986 2022-11-11 07:10:06.000000 openedx-django-require-2.0.0/openedx_django_require.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 07:10:05.000000 openedx-django-require-2.0.0/openedx_django_require.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-11 07:10:05.000000 openedx-django-require-2.0.0/openedx_django_require.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 07:10:06.252471 openedx-django-require-2.0.0/require/
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-11-11 07:10:00.000000 openedx-django-require-2.0.0/require/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1320 2022-11-11 07:10:00.000000 openedx-django-require-2.0.0/require/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1816 2022-11-11 07:10:00.000000 openedx-django-require-2.0.0/require/environments.py
--rw-r--r--   0 runner    (1001) docker     (121)      666 2022-11-11 07:10:00.000000 openedx-django-require-2.0.0/require/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 07:10:06.252471 openedx-django-require-2.0.0/require/management/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 07:10:00.000000 openedx-django-require-2.0.0/require/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 07:10:06.252471 openedx-django-require-2.0.0/require/management/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 07:10:00.000000 openedx-django-require-2.0.0/require/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3146 2022-11-11 07:10:00.000000 openedx-django-require-2.0.0/require/management/commands/require_init.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 07:10:00.000000 openedx-django-require-2.0.0/require/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 07:10:06.264471 openedx-django-require-2.0.0/require/resources/
--rw-r--r--   0 runner    (1001) docker     (121)    15168 2022-11-11 07:10:00.000000 openedx-django-require-2.0.0/require/resources/almond.js
--rw-r--r--   0 runner    (1001) docker     (121)     2610 2022-11-11 07:10:00.000000 openedx-django-require-2.0.0/require/resources/app.build.js
--rw-r--r--   0 runner    (1001) docker     (121)  6383029 2022-11-11 07:10:00.000000 openedx-django-require-2.0.0/require/resources/compiler.jar
--rw-r--r--   0 runner    (1001) docker     (121)  1142627 2022-11-11 07:10:00.000000 openedx-django-require-2.0.0/require/resources/js.jar
--rw-r--r--   0 runner    (1001) docker     (121)     1732 2022-11-11 07:10:00.000000 openedx-django-require-2.0.0/require/resources/module.build.js
--rw-r--r--   0 runner    (1001) docker     (121)  1193082 2022-11-11 07:10:00.000000 openedx-django-require-2.0.0/require/resources/r.js
--rw-r--r--   0 runner    (1001) docker     (121)    85921 2022-11-11 07:10:00.000000 openedx-django-require-2.0.0/require/resources/require.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 07:10:06.264471 openedx-django-require-2.0.0/require/resources/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     2682 2022-11-11 07:10:00.000000 openedx-django-require-2.0.0/require/resources/tests/app.build.closure.js
--rw-r--r--   0 runner    (1001) docker     (121)     2682 2022-11-11 07:10:00.000000 openedx-django-require-2.0.0/require/resources/tests/app.build.js
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-11-11 07:10:00.000000 openedx-django-require-2.0.0/require/resources/tests/main.js
--rw-r--r--   0 runner    (1001) docker     (121)     1754 2022-11-11 07:10:00.000000 openedx-django-require-2.0.0/require/resources/tests/module.build.closure.js
--rw-r--r--   0 runner    (1001) docker     (121)     1754 2022-11-11 07:10:00.000000 openedx-django-require-2.0.0/require/resources/tests/module.build.js
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-11-11 07:10:00.000000 openedx-django-require-2.0.0/require/resources/tests/util.js
--rw-r--r--   0 runner    (1001) docker     (121)     8566 2022-11-11 07:10:00.000000 openedx-django-require-2.0.0/require/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 07:10:06.264471 openedx-django-require-2.0.0/require/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 07:10:00.000000 openedx-django-require-2.0.0/require/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1378 2022-11-11 07:10:00.000000 openedx-django-require-2.0.0/require/templatetags/require.py
--rw-r--r--   0 runner    (1001) docker     (121)     8902 2022-11-11 07:10:00.000000 openedx-django-require-2.0.0/require/tests.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-11 07:10:06.264471 openedx-django-require-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1206 2022-11-11 07:10:00.000000 openedx-django-require-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 07:11:36.824692 openedx-django-require-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-07-24 07:11:32.000000 openedx-django-require-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-07-24 07:11:32.000000 openedx-django-require-2.1.0/LICENSE-BSD-3c
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-07-24 07:11:32.000000 openedx-django-require-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      798 2023-07-24 07:11:36.824692 openedx-django-require-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     9483 2023-07-24 07:11:32.000000 openedx-django-require-2.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 07:11:36.808690 openedx-django-require-2.1.0/openedx_django_require.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      798 2023-07-24 07:11:36.000000 openedx-django-require-2.1.0/openedx_django_require.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      986 2023-07-24 07:11:36.000000 openedx-django-require-2.1.0/openedx_django_require.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-24 07:11:36.000000 openedx-django-require-2.1.0/openedx_django_require.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-07-24 07:11:36.000000 openedx-django-require-2.1.0/openedx_django_require.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 07:11:36.812690 openedx-django-require-2.1.0/require/
+-rw-r--r--   0 runner    (1001) docker     (122)      153 2023-07-24 07:11:32.000000 openedx-django-require-2.1.0/require/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1320 2023-07-24 07:11:32.000000 openedx-django-require-2.1.0/require/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1816 2023-07-24 07:11:32.000000 openedx-django-require-2.1.0/require/environments.py
+-rw-r--r--   0 runner    (1001) docker     (122)      666 2023-07-24 07:11:32.000000 openedx-django-require-2.1.0/require/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 07:11:36.812690 openedx-django-require-2.1.0/require/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-24 07:11:32.000000 openedx-django-require-2.1.0/require/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 07:11:36.812690 openedx-django-require-2.1.0/require/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-24 07:11:32.000000 openedx-django-require-2.1.0/require/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3146 2023-07-24 07:11:32.000000 openedx-django-require-2.1.0/require/management/commands/require_init.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-24 07:11:32.000000 openedx-django-require-2.1.0/require/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 07:11:36.820691 openedx-django-require-2.1.0/require/resources/
+-rw-r--r--   0 runner    (1001) docker     (122)    15168 2023-07-24 07:11:32.000000 openedx-django-require-2.1.0/require/resources/almond.js
+-rw-r--r--   0 runner    (1001) docker     (122)     2610 2023-07-24 07:11:32.000000 openedx-django-require-2.1.0/require/resources/app.build.js
+-rw-r--r--   0 runner    (1001) docker     (122)  6383029 2023-07-24 07:11:33.000000 openedx-django-require-2.1.0/require/resources/compiler.jar
+-rw-r--r--   0 runner    (1001) docker     (122)  1142627 2023-07-24 07:11:33.000000 openedx-django-require-2.1.0/require/resources/js.jar
+-rw-r--r--   0 runner    (1001) docker     (122)     1732 2023-07-24 07:11:33.000000 openedx-django-require-2.1.0/require/resources/module.build.js
+-rw-r--r--   0 runner    (1001) docker     (122)  1193082 2023-07-24 07:11:33.000000 openedx-django-require-2.1.0/require/resources/r.js
+-rw-r--r--   0 runner    (1001) docker     (122)    85921 2023-07-24 07:11:33.000000 openedx-django-require-2.1.0/require/resources/require.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 07:11:36.824692 openedx-django-require-2.1.0/require/resources/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     2682 2023-07-24 07:11:33.000000 openedx-django-require-2.1.0/require/resources/tests/app.build.closure.js
+-rw-r--r--   0 runner    (1001) docker     (122)     2682 2023-07-24 07:11:33.000000 openedx-django-require-2.1.0/require/resources/tests/app.build.js
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-07-24 07:11:33.000000 openedx-django-require-2.1.0/require/resources/tests/main.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1754 2023-07-24 07:11:33.000000 openedx-django-require-2.1.0/require/resources/tests/module.build.closure.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1754 2023-07-24 07:11:33.000000 openedx-django-require-2.1.0/require/resources/tests/module.build.js
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-07-24 07:11:33.000000 openedx-django-require-2.1.0/require/resources/tests/util.js
+-rw-r--r--   0 runner    (1001) docker     (122)     8563 2023-07-24 07:11:33.000000 openedx-django-require-2.1.0/require/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 07:11:36.824692 openedx-django-require-2.1.0/require/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-24 07:11:33.000000 openedx-django-require-2.1.0/require/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1378 2023-07-24 07:11:33.000000 openedx-django-require-2.1.0/require/templatetags/require.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8902 2023-07-24 07:11:33.000000 openedx-django-require-2.1.0/require/tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-24 07:11:36.824692 openedx-django-require-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1244 2023-07-24 07:11:33.000000 openedx-django-require-2.1.0/setup.py
```

### Comparing `openedx-django-require-2.0.0/LICENSE` & `openedx-django-require-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openedx-django-require-2.0.0/LICENSE-BSD-3c` & `openedx-django-require-2.1.0/LICENSE-BSD-3c`

 * *Files identical despite different names*

### Comparing `openedx-django-require-2.0.0/PKG-INFO` & `openedx-django-require-2.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 1.2
 Name: openedx-django-require
-Version: 2.0.0
+Version: 2.1.0
 Summary: A Django staticfiles post-processor for optimizing with RequireJS.
 Home-page: https://github.com/etianen/django-require
 Author: Dave Hall
 Author-email: dave@etianen.com
 Maintainer: edX
 License: BSD
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP
```

### Comparing `openedx-django-require-2.0.0/README.rst` & `openedx-django-require-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `openedx-django-require-2.0.0/openedx_django_require.egg-info/PKG-INFO` & `openedx-django-require-2.1.0/openedx_django_require.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 1.2
 Name: openedx-django-require
-Version: 2.0.0
+Version: 2.1.0
 Summary: A Django staticfiles post-processor for optimizing with RequireJS.
 Home-page: https://github.com/etianen/django-require
 Author: Dave Hall
 Author-email: dave@etianen.com
 Maintainer: edX
 License: BSD
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP
```

### Comparing `openedx-django-require-2.0.0/openedx_django_require.egg-info/SOURCES.txt` & `openedx-django-require-2.1.0/openedx_django_require.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openedx-django-require-2.0.0/require/conf.py` & `openedx-django-require-2.1.0/require/conf.py`

 * *Files identical despite different names*

### Comparing `openedx-django-require-2.0.0/require/environments.py` & `openedx-django-require-2.1.0/require/environments.py`

 * *Files identical despite different names*

### Comparing `openedx-django-require-2.0.0/require/helpers.py` & `openedx-django-require-2.1.0/require/helpers.py`

 * *Files identical despite different names*

### Comparing `openedx-django-require-2.0.0/require/management/commands/require_init.py` & `openedx-django-require-2.1.0/require/management/commands/require_init.py`

 * *Files identical despite different names*

### Comparing `openedx-django-require-2.0.0/require/resources/almond.js` & `openedx-django-require-2.1.0/require/resources/almond.js`

 * *Files identical despite different names*

### Comparing `openedx-django-require-2.0.0/require/resources/app.build.js` & `openedx-django-require-2.1.0/require/resources/app.build.js`

 * *Files identical despite different names*

### Comparing `openedx-django-require-2.0.0/require/resources/compiler.jar` & `openedx-django-require-2.1.0/require/resources/compiler.jar`

 * *Files identical despite different names*

### Comparing `openedx-django-require-2.0.0/require/resources/js.jar` & `openedx-django-require-2.1.0/require/resources/js.jar`

 * *Files identical despite different names*

### Comparing `openedx-django-require-2.0.0/require/resources/module.build.js` & `openedx-django-require-2.1.0/require/resources/module.build.js`

 * *Files identical despite different names*

### Comparing `openedx-django-require-2.0.0/require/resources/r.js` & `openedx-django-require-2.1.0/require/resources/r.js`

 * *Files identical despite different names*

### Comparing `openedx-django-require-2.0.0/require/resources/require.js` & `openedx-django-require-2.1.0/require/resources/require.js`

 * *Files identical despite different names*

### Comparing `openedx-django-require-2.0.0/require/resources/tests/app.build.closure.js` & `openedx-django-require-2.1.0/require/resources/tests/app.build.closure.js`

 * *Files identical despite different names*

### Comparing `openedx-django-require-2.0.0/require/resources/tests/app.build.js` & `openedx-django-require-2.1.0/require/resources/tests/app.build.js`

 * *Files identical despite different names*

### Comparing `openedx-django-require-2.0.0/require/resources/tests/module.build.closure.js` & `openedx-django-require-2.1.0/require/resources/tests/module.build.closure.js`

 * *Files identical despite different names*

### Comparing `openedx-django-require-2.0.0/require/resources/tests/module.build.js` & `openedx-django-require-2.1.0/require/resources/tests/module.build.js`

 * *Files identical despite different names*

### Comparing `openedx-django-require-2.0.0/require/storage.py` & `openedx-django-require-2.1.0/require/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from functools import partial
 from contextlib import closing
 
 from django.core.exceptions import ImproperlyConfigured
 from django.core.files.base import File
 from django.core.files.storage import FileSystemStorage
 from django.contrib.staticfiles.storage import StaticFilesStorage, ManifestStaticFilesStorage
-from django.utils.encoding import force_text
+from django.utils.encoding import force_str
 
 from require.conf import settings as require_settings
 from require.helpers import resolve_require_url
 from require.environments import load_environment
 
 
 class TemporaryCompileEnvironment(object):
@@ -132,17 +132,17 @@
                     raise ImproperlyConfigured("No 'out' option specified for module '{module}' in REQUIRE_STANDALONE_MODULES setting.".format(
                         module = standalone_module
                     ))
             # Update assets with modified ones.
             compiled_storage = FileSystemStorage(env.build_dir)
             # Walk the compiled directory, checking for modified assets.
             for build_dirpath, _, build_filenames in os.walk(env.build_dir):
-                build_dirpath = force_text(build_dirpath)
+                build_dirpath = force_str(build_dirpath)
                 for build_filename in build_filenames:
-                    build_filename = force_text(build_filename)
+                    build_filename = force_str(build_filename)
                     # Determine asset name.
                     build_filepath = os.path.join(build_dirpath, build_filename)
                     build_name = build_filepath[len(env.build_dir)+1:]
                     build_storage_name = build_name.replace(os.sep, "/")
                     # Ignore certain files.
                     if build_storage_name in exclude_names:
                         # Delete from storage, if originally present.
```

### Comparing `openedx-django-require-2.0.0/require/templatetags/require.py` & `openedx-django-require-2.1.0/require/templatetags/require.py`

 * *Files identical despite different names*

### Comparing `openedx-django-require-2.0.0/require/tests.py` & `openedx-django-require-2.1.0/require/tests.py`

 * *Files identical despite different names*

### Comparing `openedx-django-require-2.0.0/setup.py` & `openedx-django-require-2.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         ],
     },
     classifiers = [
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Django",
         "Framework :: Django :: 3.2",
+        "Framework :: Django :: 4.2",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.8",
         "Topic :: Internet :: WWW/HTTP",
     ],
```

