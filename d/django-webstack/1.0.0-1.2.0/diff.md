# Comparing `tmp/django-webstack-1.0.0.tar.gz` & `tmp/django-webstack-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-webstack-1.0.0.tar", last modified: Mon Jul 24 09:17:38 2023, max compression
+gzip compressed data, was "django-webstack-1.2.0.tar", last modified: Mon Jul 24 10:50:36 2023, max compression
```

## Comparing `django-webstack-1.0.0.tar` & `django-webstack-1.2.0.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:17:38.056146 django-webstack-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-24 09:17:21.000000 django-webstack-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-24 09:17:21.000000 django-webstack-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-24 09:17:38.056146 django-webstack-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-24 09:17:21.000000 django-webstack-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:17:38.052146 django-webstack-1.0.0/django_webstack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-24 09:17:38.000000 django-webstack-1.0.0/django_webstack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-24 09:17:38.000000 django-webstack-1.0.0/django_webstack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 09:17:38.000000 django-webstack-1.0.0/django_webstack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-24 09:17:38.000000 django-webstack-1.0.0/django_webstack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-24 09:17:38.000000 django-webstack-1.0.0/django_webstack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 09:17:38.056146 django-webstack-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-24 09:17:21.000000 django-webstack-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:17:38.052146 django-webstack-1.0.0/webstack/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-24 09:17:21.000000 django-webstack-1.0.0/webstack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-24 09:17:21.000000 django-webstack-1.0.0/webstack/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-24 09:17:21.000000 django-webstack-1.0.0/webstack/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:17:38.052146 django-webstack-1.0.0/webstack/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-24 09:17:21.000000 django-webstack-1.0.0/webstack/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 09:17:21.000000 django-webstack-1.0.0/webstack/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-07-24 09:17:21.000000 django-webstack-1.0.0/webstack/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:17:38.048146 django-webstack-1.0.0/webstack/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:17:38.048146 django-webstack-1.0.0/webstack/static/webstack/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:17:38.048146 django-webstack-1.0.0/webstack/static/webstack/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:17:38.052146 django-webstack-1.0.0/webstack/static/webstack/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-24 09:17:21.000000 django-webstack-1.0.0/webstack/static/webstack/assets/css/nav.css
--rw-r--r--   0 runner    (1001) docker     (123)   178177 2023-07-24 09:17:21.000000 django-webstack-1.0.0/webstack/static/webstack/assets/css/xenon-components.css
--rw-r--r--   0 runner    (1001) docker     (123)   213030 2023-07-24 09:17:21.000000 django-webstack-1.0.0/webstack/static/webstack/assets/css/xenon-core.css
--rw-r--r--   0 runner    (1001) docker     (123)    58514 2023-07-24 09:17:21.000000 django-webstack-1.0.0/webstack/static/webstack/assets/css/xenon-forms.css
--rw-r--r--   0 runner    (1001) docker     (123)   288245 2023-07-24 09:17:21.000000 django-webstack-1.0.0/webstack/static/webstack/assets/css/xenon-skins.css
--rw-r--r--   0 runner    (1001) docker     (123)   699452 2023-07-24 09:17:21.000000 django-webstack-1.0.0/webstack/static/webstack/assets/css/xenon.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:17:38.052146 django-webstack-1.0.0/webstack/static/webstack/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-24 09:17:21.000000 django-webstack-1.0.0/webstack/static/webstack/assets/images/favicon.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1260 2023-07-24 09:17:21.000000 django-webstack-1.0.0/webstack/static/webstack/assets/images/logo-collapsed@2x.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2435 2023-07-24 09:17:21.000000 django-webstack-1.0.0/webstack/static/webstack/assets/images/logo@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)  1392068 2023-07-24 09:17:21.000000 django-webstack-1.0.0/webstack/static/webstack/assets/images/preview.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:17:38.056146 django-webstack-1.0.0/webstack/static/webstack/assets/js/
--rwxr-xr-x   0 runner    (1001) docker     (123)    98785 2023-07-24 09:17:21.000000 django-webstack-1.0.0/webstack/static/webstack/assets/js/TweenMax.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    24797 2023-07-24 09:17:21.000000 django-webstack-1.0.0/webstack/static/webstack/assets/js/joinable.js
--rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-07-24 09:17:21.000000 django-webstack-1.0.0/webstack/static/webstack/assets/js/lozad.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     1880 2023-07-24 09:17:21.000000 django-webstack-1.0.0/webstack/static/webstack/assets/js/resizeable.js
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-24 09:17:21.000000 django-webstack-1.0.0/webstack/static/webstack/assets/js/xenon-api.js
--rw-r--r--   0 runner    (1001) docker     (123)    44384 2023-07-24 09:17:21.000000 django-webstack-1.0.0/webstack/static/webstack/assets/js/xenon-custom.js
--rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-07-24 09:17:21.000000 django-webstack-1.0.0/webstack/static/webstack/assets/js/xenon-toggles.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:17:38.048146 django-webstack-1.0.0/webstack/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:17:38.056146 django-webstack-1.0.0/webstack/templates/webstack/
--rw-r--r--   0 runner    (1001) docker     (123)    10072 2023-07-24 09:17:21.000000 django-webstack-1.0.0/webstack/templates/webstack/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-24 09:17:21.000000 django-webstack-1.0.0/webstack/templates/webstack/index.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-24 09:17:21.000000 django-webstack-1.0.0/webstack/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-24 09:17:21.000000 django-webstack-1.0.0/webstack/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-24 09:17:21.000000 django-webstack-1.0.0/webstack/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:50:36.395600 django-webstack-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-24 10:50:23.000000 django-webstack-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-24 10:50:23.000000 django-webstack-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-24 10:50:36.395600 django-webstack-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-24 10:50:23.000000 django-webstack-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:50:36.383600 django-webstack-1.2.0/django_webstack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-24 10:50:36.000000 django-webstack-1.2.0/django_webstack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-24 10:50:36.000000 django-webstack-1.2.0/django_webstack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 10:50:36.000000 django-webstack-1.2.0/django_webstack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-24 10:50:36.000000 django-webstack-1.2.0/django_webstack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-24 10:50:36.000000 django-webstack-1.2.0/django_webstack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 10:50:36.395600 django-webstack-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-24 10:50:23.000000 django-webstack-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:50:36.387600 django-webstack-1.2.0/webstack/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-24 10:50:23.000000 django-webstack-1.2.0/webstack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-24 10:50:23.000000 django-webstack-1.2.0/webstack/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-24 10:50:23.000000 django-webstack-1.2.0/webstack/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:50:36.387600 django-webstack-1.2.0/webstack/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-24 10:50:23.000000 django-webstack-1.2.0/webstack/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-24 10:50:23.000000 django-webstack-1.2.0/webstack/migrations/0002_auto_20230724_1835.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:50:23.000000 django-webstack-1.2.0/webstack/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-07-24 10:50:23.000000 django-webstack-1.2.0/webstack/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:50:36.383600 django-webstack-1.2.0/webstack/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:50:36.383600 django-webstack-1.2.0/webstack/static/webstack/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:50:36.383600 django-webstack-1.2.0/webstack/static/webstack/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:50:36.391600 django-webstack-1.2.0/webstack/static/webstack/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-24 10:50:23.000000 django-webstack-1.2.0/webstack/static/webstack/assets/css/nav.css
+-rw-r--r--   0 runner    (1001) docker     (123)   178177 2023-07-24 10:50:23.000000 django-webstack-1.2.0/webstack/static/webstack/assets/css/xenon-components.css
+-rw-r--r--   0 runner    (1001) docker     (123)   213030 2023-07-24 10:50:23.000000 django-webstack-1.2.0/webstack/static/webstack/assets/css/xenon-core.css
+-rw-r--r--   0 runner    (1001) docker     (123)    58514 2023-07-24 10:50:23.000000 django-webstack-1.2.0/webstack/static/webstack/assets/css/xenon-forms.css
+-rw-r--r--   0 runner    (1001) docker     (123)   288245 2023-07-24 10:50:23.000000 django-webstack-1.2.0/webstack/static/webstack/assets/css/xenon-skins.css
+-rw-r--r--   0 runner    (1001) docker     (123)   699452 2023-07-24 10:50:23.000000 django-webstack-1.2.0/webstack/static/webstack/assets/css/xenon.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:50:36.391600 django-webstack-1.2.0/webstack/static/webstack/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-24 10:50:23.000000 django-webstack-1.2.0/webstack/static/webstack/assets/images/favicon.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1260 2023-07-24 10:50:23.000000 django-webstack-1.2.0/webstack/static/webstack/assets/images/logo-collapsed@2x.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2435 2023-07-24 10:50:23.000000 django-webstack-1.2.0/webstack/static/webstack/assets/images/logo@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1392068 2023-07-24 10:50:23.000000 django-webstack-1.2.0/webstack/static/webstack/assets/images/preview.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:50:36.395600 django-webstack-1.2.0/webstack/static/webstack/assets/js/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    98785 2023-07-24 10:50:23.000000 django-webstack-1.2.0/webstack/static/webstack/assets/js/TweenMax.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24797 2023-07-24 10:50:23.000000 django-webstack-1.2.0/webstack/static/webstack/assets/js/joinable.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-07-24 10:50:23.000000 django-webstack-1.2.0/webstack/static/webstack/assets/js/lozad.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1880 2023-07-24 10:50:23.000000 django-webstack-1.2.0/webstack/static/webstack/assets/js/resizeable.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-24 10:50:23.000000 django-webstack-1.2.0/webstack/static/webstack/assets/js/xenon-api.js
+-rw-r--r--   0 runner    (1001) docker     (123)    44384 2023-07-24 10:50:23.000000 django-webstack-1.2.0/webstack/static/webstack/assets/js/xenon-custom.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-07-24 10:50:23.000000 django-webstack-1.2.0/webstack/static/webstack/assets/js/xenon-toggles.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:50:36.383600 django-webstack-1.2.0/webstack/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:50:36.395600 django-webstack-1.2.0/webstack/templates/webstack/
+-rw-r--r--   0 runner    (1001) docker     (123)    10072 2023-07-24 10:50:23.000000 django-webstack-1.2.0/webstack/templates/webstack/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-24 10:50:23.000000 django-webstack-1.2.0/webstack/templates/webstack/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-24 10:50:23.000000 django-webstack-1.2.0/webstack/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-24 10:50:23.000000 django-webstack-1.2.0/webstack/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-24 10:50:23.000000 django-webstack-1.2.0/webstack/views.py
```

### Comparing `django-webstack-1.0.0/LICENSE` & `django-webstack-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-webstack-1.0.0/PKG-INFO` & `django-webstack-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-webstack
-Version: 1.0.0
+Version: 1.2.0
 Summary: webstack of Django
 Home-page: https://github.com/Hopetree/django-webstack
 Author: Hopetree
 Author-email: zlwork2014@163.com
 Keywords: django webstack navigation
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

### Comparing `django-webstack-1.0.0/README.md` & `django-webstack-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `django-webstack-1.0.0/django_webstack.egg-info/PKG-INFO` & `django-webstack-1.2.0/django_webstack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-webstack
-Version: 1.0.0
+Version: 1.2.0
 Summary: webstack of Django
 Home-page: https://github.com/Hopetree/django-webstack
 Author: Hopetree
 Author-email: zlwork2014@163.com
 Keywords: django webstack navigation
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

### Comparing `django-webstack-1.0.0/django_webstack.egg-info/SOURCES.txt` & `django-webstack-1.2.0/django_webstack.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 webstack/admin.py
 webstack/apps.py
 webstack/models.py
 webstack/tests.py
 webstack/urls.py
 webstack/views.py
 webstack/migrations/0001_initial.py
+webstack/migrations/0002_auto_20230724_1835.py
 webstack/migrations/__init__.py
 webstack/static/webstack/assets/css/nav.css
 webstack/static/webstack/assets/css/xenon-components.css
 webstack/static/webstack/assets/css/xenon-core.css
 webstack/static/webstack/assets/css/xenon-forms.css
 webstack/static/webstack/assets/css/xenon-skins.css
 webstack/static/webstack/assets/css/xenon.css
```

### Comparing `django-webstack-1.0.0/setup.py` & `django-webstack-1.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding:utf-8 -*-
 # Author: https://github.com/Hopetree
 # Date: 2023/7/24
 from setuptools import find_packages, setup
 
-VERSION = '1.0.0'
+VERSION = '1.2.0'
 
 with open('README.md', 'r', encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(
     name='django-webstack',
     version=VERSION,
```

### Comparing `django-webstack-1.0.0/webstack/admin.py` & `django-webstack-1.2.0/webstack/admin.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,12 +24,13 @@
     search_fields = ['name', 'father__name']
     autocomplete_fields = ['father']
 
 
 @admin.register(NavigationSite)
 class NavigationSiteAdmin(admin.ModelAdmin):
     date_hierarchy = 'create_date'
-    list_display = ('id', 'name', 'link', 'create_date', 'menu', 'sort_order')
+    list_display = ('id', 'name', 'link',
+                    'create_date', 'menu', 'sort_order', 'is_show', 'not_show_reason')
     list_display_links = ('name',)
     list_filter = ('create_date', 'sort_order', 'menu')
     list_editable = ('menu', 'sort_order')
     autocomplete_fields = ['menu']
```

### Comparing `django-webstack-1.0.0/webstack/migrations/0001_initial.py` & `django-webstack-1.2.0/webstack/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-webstack-1.0.0/webstack/models.py` & `django-webstack-1.2.0/webstack/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,29 +31,29 @@
     def get_second_menu_list(self):
         return SecondMenu.objects.filter(father=self).exclude(name=self.name).order_by('sort_order')
 
     def has_site(self):
         """判断一级菜单下面是否有网站"""
         num = 0
         for second_menu in self.second_menus.all():
-            num += second_menu.navigation_sites.count()
+            num += NavigationSite.objects.filter(menu=second_menu, is_show=True).count()
         return num
 
 
 class SecondMenu(BaseMenu):
     father = models.ForeignKey(FirstMenu, verbose_name='父菜单', on_delete=models.PROTECT,
                                related_name='second_menus')
 
     class Meta:
         verbose_name = '二级菜单'
         verbose_name_plural = verbose_name
         ordering = ['sort_order']
 
     def get_site_list(self):
-        return NavigationSite.objects.filter(menu=self).order_by('sort_order')
+        return NavigationSite.objects.filter(menu=self, is_show=True).order_by('sort_order')
 
 
 class NavigationSite(models.Model):
     name = models.CharField('名称', max_length=30)
     description = models.CharField('描述', max_length=100)
     link = models.URLField('网站地址', max_length=150)
     sort_order = models.IntegerField('排序', default=99, help_text='自定义排序')
@@ -61,14 +61,16 @@
     update_date = models.DateTimeField(verbose_name='修改时间', auto_now=True)
     logo = ProcessedImageField(upload_to='web/upload/%Y/%m/%d/',
                                default='web/default/default.png',
                                verbose_name='Logo',
                                processors=[ResizeToFill(50, 50)],
                                help_text='上传图片大小建议使用1:1的宽高比，为了清晰度原始图片宽度应该超过50px'
                                )
+    is_show = models.BooleanField('是否展示', blank=True, null=True, default=True)
+    not_show_reason = models.CharField('禁用原因', max_length=50, blank=True, null=True)
 
     menu = models.ForeignKey(SecondMenu, verbose_name='所属二级菜单', on_delete=models.PROTECT,
                              related_name='navigation_sites')
 
     class Meta:
         verbose_name = '导航网站'
         verbose_name_plural = verbose_name
```

### Comparing `django-webstack-1.0.0/webstack/static/webstack/assets/css/nav.css` & `django-webstack-1.2.0/webstack/static/webstack/assets/css/nav.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.0.0/webstack/static/webstack/assets/css/xenon-components.css` & `django-webstack-1.2.0/webstack/static/webstack/assets/css/xenon-components.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.0.0/webstack/static/webstack/assets/css/xenon-core.css` & `django-webstack-1.2.0/webstack/static/webstack/assets/css/xenon-core.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.0.0/webstack/static/webstack/assets/css/xenon-forms.css` & `django-webstack-1.2.0/webstack/static/webstack/assets/css/xenon-forms.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.0.0/webstack/static/webstack/assets/css/xenon-skins.css` & `django-webstack-1.2.0/webstack/static/webstack/assets/css/xenon-skins.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.0.0/webstack/static/webstack/assets/css/xenon.css` & `django-webstack-1.2.0/webstack/static/webstack/assets/css/xenon.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.0.0/webstack/static/webstack/assets/images/favicon.png` & `django-webstack-1.2.0/webstack/static/webstack/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `django-webstack-1.0.0/webstack/static/webstack/assets/images/logo-collapsed@2x.png` & `django-webstack-1.2.0/webstack/static/webstack/assets/images/logo-collapsed@2x.png`

 * *Files identical despite different names*

### Comparing `django-webstack-1.0.0/webstack/static/webstack/assets/images/logo@2x.png` & `django-webstack-1.2.0/webstack/static/webstack/assets/images/logo@2x.png`

 * *Files identical despite different names*

### Comparing `django-webstack-1.0.0/webstack/static/webstack/assets/images/preview.gif` & `django-webstack-1.2.0/webstack/static/webstack/assets/images/preview.gif`

 * *Files identical despite different names*

### Comparing `django-webstack-1.0.0/webstack/static/webstack/assets/js/TweenMax.min.js` & `django-webstack-1.2.0/webstack/static/webstack/assets/js/TweenMax.min.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.0.0/webstack/static/webstack/assets/js/joinable.js` & `django-webstack-1.2.0/webstack/static/webstack/assets/js/joinable.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.0.0/webstack/static/webstack/assets/js/lozad.js` & `django-webstack-1.2.0/webstack/static/webstack/assets/js/lozad.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.0.0/webstack/static/webstack/assets/js/resizeable.js` & `django-webstack-1.2.0/webstack/static/webstack/assets/js/resizeable.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.0.0/webstack/static/webstack/assets/js/xenon-api.js` & `django-webstack-1.2.0/webstack/static/webstack/assets/js/xenon-api.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.0.0/webstack/static/webstack/assets/js/xenon-custom.js` & `django-webstack-1.2.0/webstack/static/webstack/assets/js/xenon-custom.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.0.0/webstack/static/webstack/assets/js/xenon-toggles.js` & `django-webstack-1.2.0/webstack/static/webstack/assets/js/xenon-toggles.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.0.0/webstack/templates/webstack/base.html` & `django-webstack-1.2.0/webstack/templates/webstack/base.html`

 * *Files identical despite different names*

### Comparing `django-webstack-1.0.0/webstack/templates/webstack/index.html` & `django-webstack-1.2.0/webstack/templates/webstack/index.html`

 * *Files identical despite different names*

