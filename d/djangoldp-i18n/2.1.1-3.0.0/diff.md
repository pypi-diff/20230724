# Comparing `tmp/djangoldp_i18n-2.1.1.tar.gz` & `tmp/djangoldp_i18n-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_i18n-2.1.1.tar", last modified: Mon Mar 29 07:56:50 2021, max compression
+gzip compressed data, was "djangoldp_i18n-3.0.0.tar", last modified: Mon Jul 24 21:07:00 2023, max compression
```

## Comparing `djangoldp_i18n-2.1.1.tar` & `djangoldp_i18n-3.0.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-29 07:56:50.000000 djangoldp_i18n-2.1.1/
--rw-rw-rw-   0 root         (0) root         (0)      683 2021-03-29 07:56:50.000000 djangoldp_i18n-2.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2007 2021-03-29 07:56:35.000000 djangoldp_i18n-2.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-29 07:56:50.000000 djangoldp_i18n-2.1.1/djangoldp_i18n/
--rw-rw-rw-   0 root         (0) root         (0)     3828 2021-03-29 07:56:35.000000 djangoldp_i18n-2.1.1/djangoldp_i18n/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)      105 2021-03-29 07:56:35.000000 djangoldp_i18n-2.1.1/djangoldp_i18n/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      475 2021-03-29 07:56:35.000000 djangoldp_i18n-2.1.1/djangoldp_i18n/views.py
--rw-rw-rw-   0 root         (0) root         (0)      166 2021-03-29 07:56:35.000000 djangoldp_i18n-2.1.1/djangoldp_i18n/admin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-29 07:56:50.000000 djangoldp_i18n-2.1.1/djangoldp_i18n/tests/
--rw-rw-rw-   0 root         (0) root         (0)      887 2021-03-29 07:56:35.000000 djangoldp_i18n-2.1.1/djangoldp_i18n/tests/models.py
--rw-rw-rw-   0 root         (0) root         (0)     2491 2021-03-29 07:56:35.000000 djangoldp_i18n-2.1.1/djangoldp_i18n/tests/runner.py
--rw-rw-rw-   0 root         (0) root         (0)      595 2021-03-29 07:56:35.000000 djangoldp_i18n-2.1.1/djangoldp_i18n/tests/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      525 2021-03-29 07:56:35.000000 djangoldp_i18n-2.1.1/djangoldp_i18n/tests/djangoldp_urls.py
--rw-rw-rw-   0 root         (0) root         (0)     9748 2021-03-29 07:56:35.000000 djangoldp_i18n-2.1.1/djangoldp_i18n/tests/tests_post.py
--rw-rw-rw-   0 root         (0) root         (0)     9712 2021-03-29 07:56:35.000000 djangoldp_i18n-2.1.1/djangoldp_i18n/tests/tests_get.py
--rw-rw-rw-   0 root         (0) root         (0)     2320 2021-03-29 07:56:35.000000 djangoldp_i18n-2.1.1/djangoldp_i18n/tests/tests_cache.py
--rw-rw-rw-   0 root         (0) root         (0)      408 2021-03-29 07:56:35.000000 djangoldp_i18n-2.1.1/djangoldp_i18n/tests/translation.py
--rw-rw-rw-   0 root         (0) root         (0)       77 2021-03-29 07:56:35.000000 djangoldp_i18n-2.1.1/djangoldp_i18n/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       45 2021-03-29 07:56:48.000000 djangoldp_i18n-2.1.1/djangoldp_i18n/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      127 2021-03-29 07:56:35.000000 djangoldp_i18n-2.1.1/djangoldp_i18n/djangoldp_settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-29 07:56:50.000000 djangoldp_i18n-2.1.1/djangoldp_i18n.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2021-03-29 07:56:50.000000 djangoldp_i18n-2.1.1/djangoldp_i18n.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2021-03-29 07:56:50.000000 djangoldp_i18n-2.1.1/djangoldp_i18n.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2021-03-29 07:56:50.000000 djangoldp_i18n-2.1.1/djangoldp_i18n.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      686 2021-03-29 07:56:50.000000 djangoldp_i18n-2.1.1/djangoldp_i18n.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     2587 2021-03-29 07:56:50.000000 djangoldp_i18n-2.1.1/djangoldp_i18n.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       60 2021-03-29 07:56:35.000000 djangoldp_i18n-2.1.1/setup.py
--rw-r--r--   0 root         (0) root         (0)     2587 2021-03-29 07:56:50.000000 djangoldp_i18n-2.1.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:07:00.590441 djangoldp_i18n-3.0.0/
+-rw-r--r--   0 root         (0) root         (0)     2329 2023-07-24 21:07:00.590441 djangoldp_i18n-3.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2007 2023-07-24 21:06:40.000000 djangoldp_i18n-3.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:07:00.586441 djangoldp_i18n-3.0.0/djangoldp_i18n/
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-07-24 21:06:57.000000 djangoldp_i18n-3.0.0/djangoldp_i18n/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      166 2023-07-24 21:06:40.000000 djangoldp_i18n-3.0.0/djangoldp_i18n/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      105 2023-07-24 21:06:40.000000 djangoldp_i18n-3.0.0/djangoldp_i18n/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-07-24 21:06:40.000000 djangoldp_i18n-3.0.0/djangoldp_i18n/djangoldp_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     3828 2023-07-24 21:06:40.000000 djangoldp_i18n-3.0.0/djangoldp_i18n/serializers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:07:00.590441 djangoldp_i18n-3.0.0/djangoldp_i18n/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-07-24 21:06:40.000000 djangoldp_i18n-3.0.0/djangoldp_i18n/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      595 2023-07-24 21:06:40.000000 djangoldp_i18n-3.0.0/djangoldp_i18n/tests/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      519 2023-07-24 21:06:40.000000 djangoldp_i18n-3.0.0/djangoldp_i18n/tests/djangoldp_urls.py
+-rw-rw-rw-   0 root         (0) root         (0)      939 2023-07-24 21:06:40.000000 djangoldp_i18n-3.0.0/djangoldp_i18n/tests/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     2530 2023-07-24 21:06:40.000000 djangoldp_i18n-3.0.0/djangoldp_i18n/tests/runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     2320 2023-07-24 21:06:40.000000 djangoldp_i18n-3.0.0/djangoldp_i18n/tests/tests_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     9712 2023-07-24 21:06:40.000000 djangoldp_i18n-3.0.0/djangoldp_i18n/tests/tests_get.py
+-rw-rw-rw-   0 root         (0) root         (0)     9748 2023-07-24 21:06:40.000000 djangoldp_i18n-3.0.0/djangoldp_i18n/tests/tests_post.py
+-rw-rw-rw-   0 root         (0) root         (0)      408 2023-07-24 21:06:40.000000 djangoldp_i18n-3.0.0/djangoldp_i18n/tests/translation.py
+-rw-rw-rw-   0 root         (0) root         (0)      475 2023-07-24 21:06:40.000000 djangoldp_i18n-3.0.0/djangoldp_i18n/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:07:00.590441 djangoldp_i18n-3.0.0/djangoldp_i18n.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2329 2023-07-24 21:07:00.000000 djangoldp_i18n-3.0.0/djangoldp_i18n.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      686 2023-07-24 21:07:00.000000 djangoldp_i18n-3.0.0/djangoldp_i18n.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 21:07:00.000000 djangoldp_i18n-3.0.0/djangoldp_i18n.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-07-24 21:07:00.000000 djangoldp_i18n-3.0.0/djangoldp_i18n.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-24 21:07:00.000000 djangoldp_i18n-3.0.0/djangoldp_i18n.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      683 2023-07-24 21:07:00.590441 djangoldp_i18n-3.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-07-24 21:06:40.000000 djangoldp_i18n-3.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `djangoldp_i18n-2.1.1/setup.cfg` & `djangoldp_i18n-3.0.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 classifiers = 
 	Programming Language :: Python :: 3
 
 [options]
 packages = find:
 include_package_data = true
 install_requires = 
-	djangoldp>=2.1
-	django-modeltranslation==0.13
+	djangoldp~=3.0
+	django-modeltranslation~=0.18
 
 [semantic_release]
 version_source = tag
 version_variable = djangoldp_i18n/__init__.py:__version__
 commit_parser = commit_parser.parse
 
 [egg_info]
```

### Comparing `djangoldp_i18n-2.1.1/README.md` & `djangoldp_i18n-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `djangoldp_i18n-2.1.1/djangoldp_i18n/serializers.py` & `djangoldp_i18n-3.0.0/djangoldp_i18n/serializers.py`

 * *Files identical despite different names*

### Comparing `djangoldp_i18n-2.1.1/djangoldp_i18n/tests/models.py` & `djangoldp_i18n-3.0.0/djangoldp_i18n/tests/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 from djangoldp_i18n.views import I18nLDPViewSet
 
 
 class MultiLingualModel(Model):
     title = models.CharField(max_length=255, blank=True, null=True)
 
     class Meta(Model.Meta):
+        ordering = ['pk']
         depth = 1
         anonymous_perms = ['view', 'add', 'delete', 'change', 'control']
         authenticated_perms = ['inherit']
         owner_perms = ['inherit']
         view_set = I18nLDPViewSet
 
 
 class MultiLingualChild(Model):
     parent = models.ForeignKey(MultiLingualModel, on_delete=models.CASCADE, related_name='children')
     title = models.CharField(max_length=255, blank=True, null=True)
 
     class Meta(Model.Meta):
+        ordering = ['pk']
         anonymous_perms = ['view', 'add', 'delete', 'change', 'control']
         authenticated_perms = ['inherit']
         owner_perms = ['inherit']
         lookup_field = 'id'
         view_set = I18nLDPViewSet
```

### Comparing `djangoldp_i18n-2.1.1/djangoldp_i18n/tests/runner.py` & `djangoldp_i18n-3.0.0/djangoldp_i18n/tests/runner.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 config = {
     # add the packages to the reference list
     'ldppackages': ['djangoldp.tests','djangoldp_i18n','djangoldp_i18n.tests'],
 
     # required values for server
     'server': {
         'AUTH_USER_MODEL': 'tests.User',
+        'STORE_ACTIVITIES': 'VERBOSE',
         'REST_FRAMEWORK': {
             'DEFAULT_PAGINATION_CLASS': 'djangoldp.pagination.LDPPagination',
             'PAGE_SIZE': 5
         },
         # map the config of the core settings (avoid asserts to fail)
         'SITE_URL': 'http://happy-dev.fr',
         'BASE_URL': 'http://happy-dev.fr',
```

### Comparing `djangoldp_i18n-2.1.1/djangoldp_i18n/tests/apps.py` & `djangoldp_i18n-3.0.0/djangoldp_i18n/tests/apps.py`

 * *Files identical despite different names*

### Comparing `djangoldp_i18n-2.1.1/djangoldp_i18n/tests/djangoldp_urls.py` & `djangoldp_i18n-3.0.0/djangoldp_i18n/tests/djangoldp_urls.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from django.conf.urls import url
+from django.urls import path
 from djangoldp.permissions import LDPPermissions
 from djangoldp_i18n.tests.models import MultiLingualModel, MultiLingualChild
 from djangoldp_i18n.views import I18nLDPViewSet
 
 urlpatterns = [
-    url(r'^multilingualmodel/', I18nLDPViewSet.urls(
+    path('multilingualmodel/', I18nLDPViewSet.urls(
         model=MultiLingualModel, permission_classes=[LDPPermissions], nested_fields=['children'])),
-    url(r'^multilingualchildren/', I18nLDPViewSet.urls(
+    path('multilingualchildren/', I18nLDPViewSet.urls(
         model=MultiLingualChild, permission_classes=[LDPPermissions], nested_fields=[])),
 ]
```

### Comparing `djangoldp_i18n-2.1.1/djangoldp_i18n/tests/tests_post.py` & `djangoldp_i18n-3.0.0/djangoldp_i18n/tests/tests_post.py`

 * *Files identical despite different names*

### Comparing `djangoldp_i18n-2.1.1/djangoldp_i18n/tests/tests_get.py` & `djangoldp_i18n-3.0.0/djangoldp_i18n/tests/tests_get.py`

 * *Files identical despite different names*

### Comparing `djangoldp_i18n-2.1.1/djangoldp_i18n/tests/tests_cache.py` & `djangoldp_i18n-3.0.0/djangoldp_i18n/tests/tests_cache.py`

 * *Files identical despite different names*

### Comparing `djangoldp_i18n-2.1.1/djangoldp_i18n.egg-info/SOURCES.txt` & `djangoldp_i18n-3.0.0/djangoldp_i18n.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_i18n-2.1.1/djangoldp_i18n.egg-info/PKG-INFO` & `djangoldp_i18n-3.0.0/djangoldp_i18n.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,35 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: djangoldp-i18n
-Version: 2.1.1
+Version: 3.0.0
 Summary: extends Django-Modeltranslation and DjangoLDP's serializer and admin to provide i18n capabilities for DjangoLDP models
-Home-page: UNKNOWN
 Author: Calum Mackervoy
 Author-email: calum@startinblox.com
 License: copyleft CC NC SA
-Description: 
-        # I18nLDPViewSet
-        
-        I18nLDPViewSet overrides DjangoLDP's LDPViewSet to provide serialization using the I18nLDPSerializer, instead of the default LDPSerializer
-        
-        You can activate the custom functionality on your DjangoLDP Model by setting `view_set` in the Model.Meta: https://git.startinblox.com/djangoldp-packages/djangoldp#view_set
-        
-        ## Client-Side
-        
-        If you are using Startin'Blox in your client application, please see the [Startin'Blox docs](https://docs.startinblox.com)
-        
-        If you are writing your own client, a full how-to for requesting from the DjangoLDP viewset is out of the scope of this package README, but the adjustments needed to include a requested language are simple:
-        * for GET requests, simply set the `Accept-Language` header, following the [HTTP spec](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Accept-Language)
-        * for POST requests it is easiest to do the same. For information, it is also possible to submit the langauge in [JSON-LD value-object syntax](https://www.w3.org/TR/json-ld/#value-objects), but the _response_ will be serialized into the HTTP-requested language
-        
-        Both GET and POST requests currently only accommodate serialization in one language per-request. In POST requests this means that you cannot POST multiple language at the same time
-        
-        # I18nLDPSerializer
-        
-        The main functionality of I18n is provided in the serializer, which overrides DjangoLDP's LDPSerializer to select the activated language content and display this in the context of the response
-        
-        The language is selected and the data manipulated automatically, based on the request object in the serializer context. A feature to provide the serialization into a language using a setting (without a request object) is TODO
-        
-        # DjangoLDPI18nAdmin
-        
-        This admin class simply inherits from `DjangoLDPAdmin` from DjangoLDP and `TranslationAdmin` from [Django-Modeltranslation](https://django-modeltranslation.readthedocs.io/en/latest/admin.html) to provide the features from both. It does so without additions
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
+
+
+# I18nLDPViewSet
+
+I18nLDPViewSet overrides DjangoLDP's LDPViewSet to provide serialization using the I18nLDPSerializer, instead of the default LDPSerializer
+
+You can activate the custom functionality on your DjangoLDP Model by setting `view_set` in the Model.Meta: https://git.startinblox.com/djangoldp-packages/djangoldp#view_set
+
+## Client-Side
+
+If you are using Startin'Blox in your client application, please see the [Startin'Blox docs](https://docs.startinblox.com)
+
+If you are writing your own client, a full how-to for requesting from the DjangoLDP viewset is out of the scope of this package README, but the adjustments needed to include a requested language are simple:
+* for GET requests, simply set the `Accept-Language` header, following the [HTTP spec](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Accept-Language)
+* for POST requests it is easiest to do the same. For information, it is also possible to submit the langauge in [JSON-LD value-object syntax](https://www.w3.org/TR/json-ld/#value-objects), but the _response_ will be serialized into the HTTP-requested language
+
+Both GET and POST requests currently only accommodate serialization in one language per-request. In POST requests this means that you cannot POST multiple language at the same time
+
+# I18nLDPSerializer
+
+The main functionality of I18n is provided in the serializer, which overrides DjangoLDP's LDPSerializer to select the activated language content and display this in the context of the response
+
+The language is selected and the data manipulated automatically, based on the request object in the serializer context. A feature to provide the serialization into a language using a setting (without a request object) is TODO
+
+# DjangoLDPI18nAdmin
+
+This admin class simply inherits from `DjangoLDPAdmin` from DjangoLDP and `TranslationAdmin` from [Django-Modeltranslation](https://django-modeltranslation.readthedocs.io/en/latest/admin.html) to provide the features from both. It does so without additions
```

### Comparing `djangoldp_i18n-2.1.1/PKG-INFO` & `djangoldp_i18n-3.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,35 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: djangoldp_i18n
-Version: 2.1.1
+Version: 3.0.0
 Summary: extends Django-Modeltranslation and DjangoLDP's serializer and admin to provide i18n capabilities for DjangoLDP models
-Home-page: UNKNOWN
 Author: Calum Mackervoy
 Author-email: calum@startinblox.com
 License: copyleft CC NC SA
-Description: 
-        # I18nLDPViewSet
-        
-        I18nLDPViewSet overrides DjangoLDP's LDPViewSet to provide serialization using the I18nLDPSerializer, instead of the default LDPSerializer
-        
-        You can activate the custom functionality on your DjangoLDP Model by setting `view_set` in the Model.Meta: https://git.startinblox.com/djangoldp-packages/djangoldp#view_set
-        
-        ## Client-Side
-        
-        If you are using Startin'Blox in your client application, please see the [Startin'Blox docs](https://docs.startinblox.com)
-        
-        If you are writing your own client, a full how-to for requesting from the DjangoLDP viewset is out of the scope of this package README, but the adjustments needed to include a requested language are simple:
-        * for GET requests, simply set the `Accept-Language` header, following the [HTTP spec](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Accept-Language)
-        * for POST requests it is easiest to do the same. For information, it is also possible to submit the langauge in [JSON-LD value-object syntax](https://www.w3.org/TR/json-ld/#value-objects), but the _response_ will be serialized into the HTTP-requested language
-        
-        Both GET and POST requests currently only accommodate serialization in one language per-request. In POST requests this means that you cannot POST multiple language at the same time
-        
-        # I18nLDPSerializer
-        
-        The main functionality of I18n is provided in the serializer, which overrides DjangoLDP's LDPSerializer to select the activated language content and display this in the context of the response
-        
-        The language is selected and the data manipulated automatically, based on the request object in the serializer context. A feature to provide the serialization into a language using a setting (without a request object) is TODO
-        
-        # DjangoLDPI18nAdmin
-        
-        This admin class simply inherits from `DjangoLDPAdmin` from DjangoLDP and `TranslationAdmin` from [Django-Modeltranslation](https://django-modeltranslation.readthedocs.io/en/latest/admin.html) to provide the features from both. It does so without additions
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
+
+
+# I18nLDPViewSet
+
+I18nLDPViewSet overrides DjangoLDP's LDPViewSet to provide serialization using the I18nLDPSerializer, instead of the default LDPSerializer
+
+You can activate the custom functionality on your DjangoLDP Model by setting `view_set` in the Model.Meta: https://git.startinblox.com/djangoldp-packages/djangoldp#view_set
+
+## Client-Side
+
+If you are using Startin'Blox in your client application, please see the [Startin'Blox docs](https://docs.startinblox.com)
+
+If you are writing your own client, a full how-to for requesting from the DjangoLDP viewset is out of the scope of this package README, but the adjustments needed to include a requested language are simple:
+* for GET requests, simply set the `Accept-Language` header, following the [HTTP spec](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Accept-Language)
+* for POST requests it is easiest to do the same. For information, it is also possible to submit the langauge in [JSON-LD value-object syntax](https://www.w3.org/TR/json-ld/#value-objects), but the _response_ will be serialized into the HTTP-requested language
+
+Both GET and POST requests currently only accommodate serialization in one language per-request. In POST requests this means that you cannot POST multiple language at the same time
+
+# I18nLDPSerializer
+
+The main functionality of I18n is provided in the serializer, which overrides DjangoLDP's LDPSerializer to select the activated language content and display this in the context of the response
+
+The language is selected and the data manipulated automatically, based on the request object in the serializer context. A feature to provide the serialization into a language using a setting (without a request object) is TODO
+
+# DjangoLDPI18nAdmin
+
+This admin class simply inherits from `DjangoLDPAdmin` from DjangoLDP and `TranslationAdmin` from [Django-Modeltranslation](https://django-modeltranslation.readthedocs.io/en/latest/admin.html) to provide the features from both. It does so without additions
```

