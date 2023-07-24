# Comparing `tmp/django-webstack-1.2.1.tar.gz` & `tmp/django-webstack-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-webstack-1.2.1.tar", last modified: Mon Jul 24 13:14:51 2023, max compression
+gzip compressed data, was "django-webstack-1.2.2.tar", last modified: Mon Jul 24 14:34:16 2023, max compression
```

## Comparing `django-webstack-1.2.1.tar` & `django-webstack-1.2.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:14:51.527932 django-webstack-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-24 13:14:30.000000 django-webstack-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-24 13:14:30.000000 django-webstack-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-24 13:14:51.527932 django-webstack-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-24 13:14:30.000000 django-webstack-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:14:51.519930 django-webstack-1.2.1/django_webstack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-24 13:14:51.000000 django-webstack-1.2.1/django_webstack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-24 13:14:51.000000 django-webstack-1.2.1/django_webstack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:14:51.000000 django-webstack-1.2.1/django_webstack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-24 13:14:51.000000 django-webstack-1.2.1/django_webstack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-24 13:14:51.000000 django-webstack-1.2.1/django_webstack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 13:14:51.527932 django-webstack-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-24 13:14:30.000000 django-webstack-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:14:51.519930 django-webstack-1.2.1/webstack/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-24 13:14:30.000000 django-webstack-1.2.1/webstack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-24 13:14:30.000000 django-webstack-1.2.1/webstack/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-24 13:14:30.000000 django-webstack-1.2.1/webstack/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:14:51.519930 django-webstack-1.2.1/webstack/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-24 13:14:30.000000 django-webstack-1.2.1/webstack/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-24 13:14:30.000000 django-webstack-1.2.1/webstack/migrations/0002_auto_20230724_1835.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:14:30.000000 django-webstack-1.2.1/webstack/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-07-24 13:14:30.000000 django-webstack-1.2.1/webstack/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:14:51.519930 django-webstack-1.2.1/webstack/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:14:51.519930 django-webstack-1.2.1/webstack/static/webstack/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:14:51.519930 django-webstack-1.2.1/webstack/static/webstack/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:14:51.523931 django-webstack-1.2.1/webstack/static/webstack/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-24 13:14:30.000000 django-webstack-1.2.1/webstack/static/webstack/assets/css/nav.css
--rw-r--r--   0 runner    (1001) docker     (123)   178177 2023-07-24 13:14:30.000000 django-webstack-1.2.1/webstack/static/webstack/assets/css/xenon-components.css
--rw-r--r--   0 runner    (1001) docker     (123)   213030 2023-07-24 13:14:30.000000 django-webstack-1.2.1/webstack/static/webstack/assets/css/xenon-core.css
--rw-r--r--   0 runner    (1001) docker     (123)    58514 2023-07-24 13:14:30.000000 django-webstack-1.2.1/webstack/static/webstack/assets/css/xenon-forms.css
--rw-r--r--   0 runner    (1001) docker     (123)   288245 2023-07-24 13:14:30.000000 django-webstack-1.2.1/webstack/static/webstack/assets/css/xenon-skins.css
--rw-r--r--   0 runner    (1001) docker     (123)   699452 2023-07-24 13:14:30.000000 django-webstack-1.2.1/webstack/static/webstack/assets/css/xenon.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:14:51.523931 django-webstack-1.2.1/webstack/static/webstack/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-24 13:14:30.000000 django-webstack-1.2.1/webstack/static/webstack/assets/images/favicon.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1260 2023-07-24 13:14:30.000000 django-webstack-1.2.1/webstack/static/webstack/assets/images/logo-collapsed@2x.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2435 2023-07-24 13:14:30.000000 django-webstack-1.2.1/webstack/static/webstack/assets/images/logo@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)  1392068 2023-07-24 13:14:30.000000 django-webstack-1.2.1/webstack/static/webstack/assets/images/preview.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:14:51.527932 django-webstack-1.2.1/webstack/static/webstack/assets/js/
--rwxr-xr-x   0 runner    (1001) docker     (123)    98785 2023-07-24 13:14:30.000000 django-webstack-1.2.1/webstack/static/webstack/assets/js/TweenMax.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    24797 2023-07-24 13:14:30.000000 django-webstack-1.2.1/webstack/static/webstack/assets/js/joinable.js
--rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-07-24 13:14:30.000000 django-webstack-1.2.1/webstack/static/webstack/assets/js/lozad.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     1880 2023-07-24 13:14:30.000000 django-webstack-1.2.1/webstack/static/webstack/assets/js/resizeable.js
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-24 13:14:30.000000 django-webstack-1.2.1/webstack/static/webstack/assets/js/xenon-api.js
--rw-r--r--   0 runner    (1001) docker     (123)    44384 2023-07-24 13:14:30.000000 django-webstack-1.2.1/webstack/static/webstack/assets/js/xenon-custom.js
--rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-07-24 13:14:30.000000 django-webstack-1.2.1/webstack/static/webstack/assets/js/xenon-toggles.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:14:51.519930 django-webstack-1.2.1/webstack/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:14:51.527932 django-webstack-1.2.1/webstack/templates/webstack/
--rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-07-24 13:14:30.000000 django-webstack-1.2.1/webstack/templates/webstack/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-24 13:14:30.000000 django-webstack-1.2.1/webstack/templates/webstack/index.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-24 13:14:30.000000 django-webstack-1.2.1/webstack/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-24 13:14:30.000000 django-webstack-1.2.1/webstack/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-24 13:14:30.000000 django-webstack-1.2.1/webstack/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:34:16.921580 django-webstack-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-24 14:34:01.000000 django-webstack-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-24 14:34:01.000000 django-webstack-1.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-24 14:34:16.921580 django-webstack-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-24 14:34:01.000000 django-webstack-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:34:16.909580 django-webstack-1.2.2/django_webstack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-24 14:34:16.000000 django-webstack-1.2.2/django_webstack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-24 14:34:16.000000 django-webstack-1.2.2/django_webstack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 14:34:16.000000 django-webstack-1.2.2/django_webstack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-24 14:34:16.000000 django-webstack-1.2.2/django_webstack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-24 14:34:16.000000 django-webstack-1.2.2/django_webstack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 14:34:16.921580 django-webstack-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-24 14:34:01.000000 django-webstack-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:34:16.913580 django-webstack-1.2.2/webstack/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:34:16.913580 django-webstack-1.2.2/webstack/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/migrations/0002_auto_20230724_1835.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:34:16.905579 django-webstack-1.2.2/webstack/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:34:16.905579 django-webstack-1.2.2/webstack/static/webstack/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:34:16.905579 django-webstack-1.2.2/webstack/static/webstack/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:34:16.917580 django-webstack-1.2.2/webstack/static/webstack/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/static/webstack/assets/css/nav.css
+-rw-r--r--   0 runner    (1001) docker     (123)   178177 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/static/webstack/assets/css/xenon-components.css
+-rw-r--r--   0 runner    (1001) docker     (123)   213030 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/static/webstack/assets/css/xenon-core.css
+-rw-r--r--   0 runner    (1001) docker     (123)    58514 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/static/webstack/assets/css/xenon-forms.css
+-rw-r--r--   0 runner    (1001) docker     (123)   288245 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/static/webstack/assets/css/xenon-skins.css
+-rw-r--r--   0 runner    (1001) docker     (123)   699452 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/static/webstack/assets/css/xenon.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:34:16.917580 django-webstack-1.2.2/webstack/static/webstack/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/static/webstack/assets/images/favicon.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1260 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/static/webstack/assets/images/logo-collapsed@2x.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2435 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/static/webstack/assets/images/logo@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1392068 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/static/webstack/assets/images/preview.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:34:16.921580 django-webstack-1.2.2/webstack/static/webstack/assets/js/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    98785 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/static/webstack/assets/js/TweenMax.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24797 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/static/webstack/assets/js/joinable.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/static/webstack/assets/js/lozad.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1880 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/static/webstack/assets/js/resizeable.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/static/webstack/assets/js/xenon-api.js
+-rw-r--r--   0 runner    (1001) docker     (123)    44384 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/static/webstack/assets/js/xenon-custom.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/static/webstack/assets/js/xenon-toggles.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:34:16.905579 django-webstack-1.2.2/webstack/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:34:16.921580 django-webstack-1.2.2/webstack/templates/webstack/
+-rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/templates/webstack/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/templates/webstack/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-24 14:34:01.000000 django-webstack-1.2.2/webstack/views.py
```

### Comparing `django-webstack-1.2.1/LICENSE` & `django-webstack-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.1/PKG-INFO` & `django-webstack-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-webstack
-Version: 1.2.1
+Version: 1.2.2
 Summary: webstack of Django
 Home-page: https://github.com/Hopetree/django-webstack
 Author: Hopetree
 Author-email: zlwork2014@163.com
 Keywords: django webstack navigation
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -61,13 +61,13 @@
 python manage.py migrate
 ```
 
 step 4 添加到路由
 
 ```python
 urlpatterns = [
-    path('nav/', include('webstack.urls')),
+    path('nav/', include(('webstack.urls', 'webstack'), namespace='webstack')),
 ]
 ```
 
 step 5 前往管理界面添加数据即可显示到前台
```

### Comparing `django-webstack-1.2.1/README.md` & `django-webstack-1.2.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -31,13 +31,13 @@
 python manage.py migrate
 ```
 
 step 4 添加到路由
 
 ```python
 urlpatterns = [
-    path('nav/', include('webstack.urls')),
+    path('nav/', include(('webstack.urls', 'webstack'), namespace='webstack')),
 ]
 ```
 
 step 5 前往管理界面添加数据即可显示到前台
```

### Comparing `django-webstack-1.2.1/django_webstack.egg-info/PKG-INFO` & `django-webstack-1.2.2/django_webstack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-webstack
-Version: 1.2.1
+Version: 1.2.2
 Summary: webstack of Django
 Home-page: https://github.com/Hopetree/django-webstack
 Author: Hopetree
 Author-email: zlwork2014@163.com
 Keywords: django webstack navigation
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -61,13 +61,13 @@
 python manage.py migrate
 ```
 
 step 4 添加到路由
 
 ```python
 urlpatterns = [
-    path('nav/', include('webstack.urls')),
+    path('nav/', include(('webstack.urls', 'webstack'), namespace='webstack')),
 ]
 ```
 
 step 5 前往管理界面添加数据即可显示到前台
```

### Comparing `django-webstack-1.2.1/django_webstack.egg-info/SOURCES.txt` & `django-webstack-1.2.2/django_webstack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.1/setup.py` & `django-webstack-1.2.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding:utf-8 -*-
 # Author: https://github.com/Hopetree
 # Date: 2023/7/24
 from setuptools import find_packages, setup
 
-VERSION = '1.2.1'
+VERSION = '1.2.2'
 
 with open('README.md', 'r', encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(
     name='django-webstack',
     version=VERSION,
```

### Comparing `django-webstack-1.2.1/webstack/admin.py` & `django-webstack-1.2.2/webstack/admin.py`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.1/webstack/migrations/0001_initial.py` & `django-webstack-1.2.2/webstack/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.1/webstack/migrations/0002_auto_20230724_1835.py` & `django-webstack-1.2.2/webstack/migrations/0002_auto_20230724_1835.py`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.1/webstack/models.py` & `django-webstack-1.2.2/webstack/models.py`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.1/webstack/static/webstack/assets/css/nav.css` & `django-webstack-1.2.2/webstack/static/webstack/assets/css/nav.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.1/webstack/static/webstack/assets/css/xenon-components.css` & `django-webstack-1.2.2/webstack/static/webstack/assets/css/xenon-components.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.1/webstack/static/webstack/assets/css/xenon-core.css` & `django-webstack-1.2.2/webstack/static/webstack/assets/css/xenon-core.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.1/webstack/static/webstack/assets/css/xenon-forms.css` & `django-webstack-1.2.2/webstack/static/webstack/assets/css/xenon-forms.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.1/webstack/static/webstack/assets/css/xenon-skins.css` & `django-webstack-1.2.2/webstack/static/webstack/assets/css/xenon-skins.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.1/webstack/static/webstack/assets/css/xenon.css` & `django-webstack-1.2.2/webstack/static/webstack/assets/css/xenon.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.1/webstack/static/webstack/assets/images/favicon.png` & `django-webstack-1.2.2/webstack/static/webstack/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.1/webstack/static/webstack/assets/images/logo-collapsed@2x.png` & `django-webstack-1.2.2/webstack/static/webstack/assets/images/logo-collapsed@2x.png`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.1/webstack/static/webstack/assets/images/logo@2x.png` & `django-webstack-1.2.2/webstack/static/webstack/assets/images/logo@2x.png`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.1/webstack/static/webstack/assets/images/preview.gif` & `django-webstack-1.2.2/webstack/static/webstack/assets/images/preview.gif`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.1/webstack/static/webstack/assets/js/TweenMax.min.js` & `django-webstack-1.2.2/webstack/static/webstack/assets/js/TweenMax.min.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.1/webstack/static/webstack/assets/js/joinable.js` & `django-webstack-1.2.2/webstack/static/webstack/assets/js/joinable.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.1/webstack/static/webstack/assets/js/lozad.js` & `django-webstack-1.2.2/webstack/static/webstack/assets/js/lozad.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.1/webstack/static/webstack/assets/js/resizeable.js` & `django-webstack-1.2.2/webstack/static/webstack/assets/js/resizeable.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.1/webstack/static/webstack/assets/js/xenon-api.js` & `django-webstack-1.2.2/webstack/static/webstack/assets/js/xenon-api.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.1/webstack/static/webstack/assets/js/xenon-custom.js` & `django-webstack-1.2.2/webstack/static/webstack/assets/js/xenon-custom.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.1/webstack/static/webstack/assets/js/xenon-toggles.js` & `django-webstack-1.2.2/webstack/static/webstack/assets/js/xenon-toggles.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.2.1/webstack/templates/webstack/base.html` & `django-webstack-1.2.2/webstack/templates/webstack/base.html`

 * *Files identical despite different names*

