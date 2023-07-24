# Comparing `tmp/djangoldp_uploader-2.1.2.tar.gz` & `tmp/djangoldp_uploader-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_uploader-2.1.2.tar", last modified: Fri May 14 09:00:17 2021, max compression
+gzip compressed data, was "djangoldp_uploader-3.0.0.tar", last modified: Mon Jul 24 21:25:45 2023, max compression
```

## Comparing `djangoldp_uploader-2.1.2.tar` & `djangoldp_uploader-3.0.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-14 09:00:17.000000 djangoldp_uploader-2.1.2/
--rw-rw-rw-   0 root         (0) root         (0)      607 2021-05-14 09:00:17.000000 djangoldp_uploader-2.1.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      891 2021-05-14 09:00:00.000000 djangoldp_uploader-2.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-14 09:00:17.000000 djangoldp_uploader-2.1.2/djangoldp_uploader.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2021-05-14 09:00:17.000000 djangoldp_uploader-2.1.2/djangoldp_uploader.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2021-05-14 09:00:17.000000 djangoldp_uploader-2.1.2/djangoldp_uploader.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2021-05-14 09:00:17.000000 djangoldp_uploader-2.1.2/djangoldp_uploader.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1573 2021-05-14 09:00:17.000000 djangoldp_uploader-2.1.2/djangoldp_uploader.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      299 2021-05-14 09:00:17.000000 djangoldp_uploader-2.1.2/djangoldp_uploader.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       49 2021-05-14 09:00:00.000000 djangoldp_uploader-2.1.2/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-14 09:00:17.000000 djangoldp_uploader-2.1.2/djangoldp_uploader/
--rw-rw-rw-   0 root         (0) root         (0)      558 2021-05-14 09:00:00.000000 djangoldp_uploader-2.1.2/djangoldp_uploader/models.py
--rw-rw-rw-   0 root         (0) root         (0)      200 2021-05-14 09:00:00.000000 djangoldp_uploader-2.1.2/djangoldp_uploader/forms.py
--rw-rw-rw-   0 root         (0) root         (0)      110 2021-05-14 09:00:00.000000 djangoldp_uploader-2.1.2/djangoldp_uploader/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      956 2021-05-14 09:00:00.000000 djangoldp_uploader-2.1.2/djangoldp_uploader/djangoldp_urls.py
--rw-rw-rw-   0 root         (0) root         (0)     6231 2021-05-14 09:00:00.000000 djangoldp_uploader-2.1.2/djangoldp_uploader/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-14 09:00:17.000000 djangoldp_uploader-2.1.2/djangoldp_uploader/tests/
--rw-rw-rw-   0 root         (0) root         (0)      747 2021-05-14 09:00:00.000000 djangoldp_uploader-2.1.2/djangoldp_uploader/tests/runner.py
--rw-rw-rw-   0 root         (0) root         (0)      851 2021-05-14 09:00:00.000000 djangoldp_uploader-2.1.2/djangoldp_uploader/tests/tests_upload.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-14 09:00:00.000000 djangoldp_uploader-2.1.2/djangoldp_uploader/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-14 09:00:17.000000 djangoldp_uploader-2.1.2/djangoldp_uploader/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      776 2021-05-14 09:00:00.000000 djangoldp_uploader-2.1.2/djangoldp_uploader/migrations/0003_auto_20200522_1521.py
--rw-rw-rw-   0 root         (0) root         (0)      547 2021-05-14 09:00:00.000000 djangoldp_uploader-2.1.2/djangoldp_uploader/migrations/0013_auto_20210210_0913.py
--rw-rw-rw-   0 root         (0) root         (0)      561 2021-05-14 09:00:00.000000 djangoldp_uploader-2.1.2/djangoldp_uploader/migrations/0007_auto_20210128_0724.py
--rw-rw-rw-   0 root         (0) root         (0)      578 2021-05-14 09:00:00.000000 djangoldp_uploader-2.1.2/djangoldp_uploader/migrations/0009_auto_20210202_1510.py
--rw-rw-rw-   0 root         (0) root         (0)     1188 2021-05-14 09:00:00.000000 djangoldp_uploader-2.1.2/djangoldp_uploader/migrations/0006_file.py
--rw-rw-rw-   0 root         (0) root         (0)      415 2021-05-14 09:00:00.000000 djangoldp_uploader-2.1.2/djangoldp_uploader/migrations/0012_file_document.py
--rw-rw-rw-   0 root         (0) root         (0)      575 2021-05-14 09:00:00.000000 djangoldp_uploader-2.1.2/djangoldp_uploader/migrations/0014_auto_20210216_1644.py
--rw-rw-rw-   0 root         (0) root         (0)      540 2021-05-14 09:00:00.000000 djangoldp_uploader-2.1.2/djangoldp_uploader/migrations/0005_auto_20200619_0811.py
--rw-rw-rw-   0 root         (0) root         (0)      500 2021-05-14 09:00:00.000000 djangoldp_uploader-2.1.2/djangoldp_uploader/migrations/0002_document_urlid.py
--rw-rw-rw-   0 root         (0) root         (0)      554 2021-05-14 09:00:00.000000 djangoldp_uploader-2.1.2/djangoldp_uploader/migrations/0004_auto_20200610_1323.py
--rw-rw-rw-   0 root         (0) root         (0)      875 2021-05-14 09:00:00.000000 djangoldp_uploader-2.1.2/djangoldp_uploader/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      575 2021-05-14 09:00:00.000000 djangoldp_uploader-2.1.2/djangoldp_uploader/migrations/0011_auto_20210208_1801.py
--rw-rw-rw-   0 root         (0) root         (0)     1063 2021-05-14 09:00:00.000000 djangoldp_uploader-2.1.2/djangoldp_uploader/migrations/0010_auto_20210208_0918.py
--rw-rw-rw-   0 root         (0) root         (0)      575 2021-05-14 09:00:00.000000 djangoldp_uploader-2.1.2/djangoldp_uploader/migrations/0008_auto_20210202_1058.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-14 09:00:00.000000 djangoldp_uploader-2.1.2/djangoldp_uploader/migrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-14 09:00:17.000000 djangoldp_uploader-2.1.2/djangoldp_uploader/templates/
--rw-rw-rw-   0 root         (0) root         (0)      466 2021-05-14 09:00:00.000000 djangoldp_uploader-2.1.2/djangoldp_uploader/templates/simple_upload.html
--rw-rw-rw-   0 root         (0) root         (0)      286 2021-05-14 09:00:00.000000 djangoldp_uploader-2.1.2/djangoldp_uploader/templates/model_form_upload.html
--rw-rw-rw-   0 root         (0) root         (0)      434 2021-05-14 09:00:00.000000 djangoldp_uploader-2.1.2/djangoldp_uploader/templates/sib_base.html
--rw-rw-rw-   0 root         (0) root         (0)      685 2021-05-14 09:00:00.000000 djangoldp_uploader-2.1.2/djangoldp_uploader/templates/demo_sib.html
--rw-rw-rw-   0 root         (0) root         (0)      650 2021-05-14 09:00:00.000000 djangoldp_uploader-2.1.2/djangoldp_uploader/templates/home.html
--rw-rw-rw-   0 root         (0) root         (0)       50 2021-05-14 09:00:15.000000 djangoldp_uploader-2.1.2/djangoldp_uploader/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       61 2021-05-14 09:00:00.000000 djangoldp_uploader-2.1.2/setup.py
--rw-r--r--   0 root         (0) root         (0)      299 2021-05-14 09:00:17.000000 djangoldp_uploader-2.1.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:25:45.878952 djangoldp_uploader-3.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-07-24 21:25:26.000000 djangoldp_uploader-3.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      260 2023-07-24 21:25:45.878952 djangoldp_uploader-3.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      891 2023-07-24 21:25:26.000000 djangoldp_uploader-3.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:25:45.874952 djangoldp_uploader-3.0.0/djangoldp_uploader/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-07-24 21:25:43.000000 djangoldp_uploader-3.0.0/djangoldp_uploader/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-07-24 21:25:26.000000 djangoldp_uploader-3.0.0/djangoldp_uploader/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      955 2023-07-24 21:25:26.000000 djangoldp_uploader-3.0.0/djangoldp_uploader/djangoldp_urls.py
+-rw-rw-rw-   0 root         (0) root         (0)      200 2023-07-24 21:25:26.000000 djangoldp_uploader-3.0.0/djangoldp_uploader/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:25:45.874952 djangoldp_uploader-3.0.0/djangoldp_uploader/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      875 2023-07-24 21:25:26.000000 djangoldp_uploader-3.0.0/djangoldp_uploader/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      500 2023-07-24 21:25:26.000000 djangoldp_uploader-3.0.0/djangoldp_uploader/migrations/0002_document_urlid.py
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-07-24 21:25:26.000000 djangoldp_uploader-3.0.0/djangoldp_uploader/migrations/0003_auto_20200522_1521.py
+-rw-rw-rw-   0 root         (0) root         (0)      554 2023-07-24 21:25:26.000000 djangoldp_uploader-3.0.0/djangoldp_uploader/migrations/0004_auto_20200610_1323.py
+-rw-rw-rw-   0 root         (0) root         (0)      540 2023-07-24 21:25:26.000000 djangoldp_uploader-3.0.0/djangoldp_uploader/migrations/0005_auto_20200619_0811.py
+-rw-rw-rw-   0 root         (0) root         (0)     1188 2023-07-24 21:25:26.000000 djangoldp_uploader-3.0.0/djangoldp_uploader/migrations/0006_file.py
+-rw-rw-rw-   0 root         (0) root         (0)      561 2023-07-24 21:25:26.000000 djangoldp_uploader-3.0.0/djangoldp_uploader/migrations/0007_auto_20210128_0724.py
+-rw-rw-rw-   0 root         (0) root         (0)      575 2023-07-24 21:25:26.000000 djangoldp_uploader-3.0.0/djangoldp_uploader/migrations/0008_auto_20210202_1058.py
+-rw-rw-rw-   0 root         (0) root         (0)      578 2023-07-24 21:25:26.000000 djangoldp_uploader-3.0.0/djangoldp_uploader/migrations/0009_auto_20210202_1510.py
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2023-07-24 21:25:26.000000 djangoldp_uploader-3.0.0/djangoldp_uploader/migrations/0010_auto_20210208_0918.py
+-rw-rw-rw-   0 root         (0) root         (0)      575 2023-07-24 21:25:26.000000 djangoldp_uploader-3.0.0/djangoldp_uploader/migrations/0011_auto_20210208_1801.py
+-rw-rw-rw-   0 root         (0) root         (0)      415 2023-07-24 21:25:26.000000 djangoldp_uploader-3.0.0/djangoldp_uploader/migrations/0012_file_document.py
+-rw-rw-rw-   0 root         (0) root         (0)      547 2023-07-24 21:25:26.000000 djangoldp_uploader-3.0.0/djangoldp_uploader/migrations/0013_auto_20210210_0913.py
+-rw-rw-rw-   0 root         (0) root         (0)      575 2023-07-24 21:25:26.000000 djangoldp_uploader-3.0.0/djangoldp_uploader/migrations/0014_auto_20210216_1644.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 21:25:26.000000 djangoldp_uploader-3.0.0/djangoldp_uploader/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      558 2023-07-24 21:25:26.000000 djangoldp_uploader-3.0.0/djangoldp_uploader/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:25:45.878952 djangoldp_uploader-3.0.0/djangoldp_uploader/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      685 2023-07-24 21:25:26.000000 djangoldp_uploader-3.0.0/djangoldp_uploader/templates/demo_sib.html
+-rw-rw-rw-   0 root         (0) root         (0)      650 2023-07-24 21:25:26.000000 djangoldp_uploader-3.0.0/djangoldp_uploader/templates/home.html
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-07-24 21:25:26.000000 djangoldp_uploader-3.0.0/djangoldp_uploader/templates/model_form_upload.html
+-rw-rw-rw-   0 root         (0) root         (0)      434 2023-07-24 21:25:26.000000 djangoldp_uploader-3.0.0/djangoldp_uploader/templates/sib_base.html
+-rw-rw-rw-   0 root         (0) root         (0)      466 2023-07-24 21:25:26.000000 djangoldp_uploader-3.0.0/djangoldp_uploader/templates/simple_upload.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:25:45.878952 djangoldp_uploader-3.0.0/djangoldp_uploader/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 21:25:26.000000 djangoldp_uploader-3.0.0/djangoldp_uploader/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      747 2023-07-24 21:25:26.000000 djangoldp_uploader-3.0.0/djangoldp_uploader/tests/runner.py
+-rw-rw-rw-   0 root         (0) root         (0)      851 2023-07-24 21:25:26.000000 djangoldp_uploader-3.0.0/djangoldp_uploader/tests/tests_upload.py
+-rw-rw-rw-   0 root         (0) root         (0)     6227 2023-07-24 21:25:26.000000 djangoldp_uploader-3.0.0/djangoldp_uploader/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:25:45.874952 djangoldp_uploader-3.0.0/djangoldp_uploader.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      260 2023-07-24 21:25:45.000000 djangoldp_uploader-3.0.0/djangoldp_uploader.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1573 2023-07-24 21:25:45.000000 djangoldp_uploader-3.0.0/djangoldp_uploader.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 21:25:45.000000 djangoldp_uploader-3.0.0/djangoldp_uploader.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-07-24 21:25:45.000000 djangoldp_uploader-3.0.0/djangoldp_uploader.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-24 21:25:45.000000 djangoldp_uploader-3.0.0/djangoldp_uploader.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      607 2023-07-24 21:25:45.878952 djangoldp_uploader-3.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-24 21:25:26.000000 djangoldp_uploader-3.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `djangoldp_uploader-2.1.2/setup.cfg` & `djangoldp_uploader-3.0.0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 description = djangoldp package for file upload
 license = MIT
 
 [options]
 include_package_data = True
 packages = find:
 install_requires = 
-	djangoldp~=2.1
-	validators~=0.12
+	djangoldp~=3.0
+	validators~=0.20
 
 [options.extras_require]
 dev = 
 	factory_boy>=2.11.0
 
 [semantic_release]
 version_source = tag
```

### Comparing `djangoldp_uploader-2.1.2/README.md` & `djangoldp_uploader-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `djangoldp_uploader-2.1.2/djangoldp_uploader.egg-info/SOURCES.txt` & `djangoldp_uploader-3.0.0/djangoldp_uploader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_uploader-2.1.2/djangoldp_uploader/models.py` & `djangoldp_uploader-3.0.0/djangoldp_uploader/models.py`

 * *Files identical despite different names*

### Comparing `djangoldp_uploader-2.1.2/djangoldp_uploader/djangoldp_urls.py` & `djangoldp_uploader-3.0.0/djangoldp_uploader/djangoldp_urls.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """djangoldp uploader URL Configuration"""
 
 from django.conf import settings
-from django.conf.urls import url
+from django.urls import path, re_path
 from django.conf.urls.static import static
 from django.views.decorators.csrf import csrf_exempt
 
 from djangoldp_uploader import views
 from djangoldp_uploader.views import FileUploadView, FileUploadPostView
 
 urlpatterns = [
-    url(r'^upload/$', csrf_exempt(FileUploadPostView.as_view()), name='upload'),
-    url(r'^upload/(?P<hashcode>[\w|\W-]+)/(?P<filename>[\w|\W-]+).(?P<fileext>[\w]+)$', csrf_exempt(FileUploadView.as_view()), name='upload_xmpp')
+    path('upload/', csrf_exempt(FileUploadPostView.as_view()), name='upload'),
+    re_path(r'^upload/(?P<hashcode>[\w|\W-]+)/(?P<filename>[\w|\W-]+).(?P<fileext>[\w]+)$', csrf_exempt(FileUploadView.as_view()), name='upload_xmpp')
 ]
 
 urlpatterns += static(settings.MEDIA_URL, document_root=settings.MEDIA_ROOT)
 
 if settings.DEBUG:
     urlpatterns += [
-        url(r'^demo/$', views.home, name='home'),
-        url(r'^demo/sib/$', views.demo_sib, name='upload_sib'),
-        url(r'^demo/simple/$', views.upload_view, name='simple_upload'),
-        url(r'^demo/form/$', views.model_form_upload, name='model_form_upload'),
+        path('demo/', views.home, name='home'),
+        path('demo/sib/', views.demo_sib, name='upload_sib'),
+        path('demo/simple/', views.upload_view, name='simple_upload'),
+        path('demo/form/', views.model_form_upload, name='model_form_upload'),
     ]
```

### Comparing `djangoldp_uploader-2.1.2/djangoldp_uploader/views.py` & `djangoldp_uploader-3.0.0/djangoldp_uploader/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         return HttpResponse(status=403)
 
 
 class FileUploadPostView(APIView):
     def dispatch(self, request, *args, **kwargs):
         request.csrf_processing_done = True
         response = super().dispatch(request, *args, **kwargs)
-        response["Access-Control-Allow-Origin"] = request.META.get('HTTP_ORIGIN')
+        response["Access-Control-Allow-Origin"] = request.headers.get('origin')
         response["Access-Control-Allow-Methods"] = "POST,OPTIONS"
         response["Access-Control-Allow-Headers"] = "authorization, Content-Type, if-match, accept, sentry-trace, dpop"
         response["Access-Control-Expose-Headers"] = "Location, User"
         response["Access-Control-Allow-Credentials"] = 'true'
 
         return response
 
@@ -106,15 +106,15 @@
 class FileUploadView(APIView):
     parser_classes = (FileUploadParser,)
 
     def dispatch(self, request, *args, **kwargs):
         request.csrf_processing_done = True
         '''overriden dispatch method to append some custom headers'''
         response = super().dispatch(request, *args, **kwargs)
-        response["Access-Control-Allow-Origin"] = request.META.get('HTTP_ORIGIN')
+        response["Access-Control-Allow-Origin"] = request.headers.get('origin')
         response["Access-Control-Allow-Methods"] = "GET,POST,PUT,OPTIONS"
         response["Access-Control-Allow-Headers"] = "authorization, Content-Type, if-match, accept, sentry-trace, dpop"
         response["Access-Control-Expose-Headers"] = "Location, User"
         response["Access-Control-Allow-Credentials"] = 'true'
 
         return response
```

### Comparing `djangoldp_uploader-2.1.2/djangoldp_uploader/tests/runner.py` & `djangoldp_uploader-3.0.0/djangoldp_uploader/tests/runner.py`

 * *Files identical despite different names*

### Comparing `djangoldp_uploader-2.1.2/djangoldp_uploader/tests/tests_upload.py` & `djangoldp_uploader-3.0.0/djangoldp_uploader/tests/tests_upload.py`

 * *Files identical despite different names*

### Comparing `djangoldp_uploader-2.1.2/djangoldp_uploader/migrations/0003_auto_20200522_1521.py` & `djangoldp_uploader-3.0.0/djangoldp_uploader/migrations/0003_auto_20200522_1521.py`

 * *Files identical despite different names*

### Comparing `djangoldp_uploader-2.1.2/djangoldp_uploader/migrations/0013_auto_20210210_0913.py` & `djangoldp_uploader-3.0.0/djangoldp_uploader/migrations/0013_auto_20210210_0913.py`

 * *Files identical despite different names*

### Comparing `djangoldp_uploader-2.1.2/djangoldp_uploader/migrations/0007_auto_20210128_0724.py` & `djangoldp_uploader-3.0.0/djangoldp_uploader/migrations/0007_auto_20210128_0724.py`

 * *Files identical despite different names*

### Comparing `djangoldp_uploader-2.1.2/djangoldp_uploader/migrations/0009_auto_20210202_1510.py` & `djangoldp_uploader-3.0.0/djangoldp_uploader/migrations/0009_auto_20210202_1510.py`

 * *Files identical despite different names*

### Comparing `djangoldp_uploader-2.1.2/djangoldp_uploader/migrations/0006_file.py` & `djangoldp_uploader-3.0.0/djangoldp_uploader/migrations/0006_file.py`

 * *Files identical despite different names*

### Comparing `djangoldp_uploader-2.1.2/djangoldp_uploader/migrations/0014_auto_20210216_1644.py` & `djangoldp_uploader-3.0.0/djangoldp_uploader/migrations/0014_auto_20210216_1644.py`

 * *Files identical despite different names*

### Comparing `djangoldp_uploader-2.1.2/djangoldp_uploader/migrations/0005_auto_20200619_0811.py` & `djangoldp_uploader-3.0.0/djangoldp_uploader/migrations/0005_auto_20200619_0811.py`

 * *Files identical despite different names*

### Comparing `djangoldp_uploader-2.1.2/djangoldp_uploader/migrations/0004_auto_20200610_1323.py` & `djangoldp_uploader-3.0.0/djangoldp_uploader/migrations/0004_auto_20200610_1323.py`

 * *Files identical despite different names*

### Comparing `djangoldp_uploader-2.1.2/djangoldp_uploader/migrations/0001_initial.py` & `djangoldp_uploader-3.0.0/djangoldp_uploader/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_uploader-2.1.2/djangoldp_uploader/migrations/0011_auto_20210208_1801.py` & `djangoldp_uploader-3.0.0/djangoldp_uploader/migrations/0011_auto_20210208_1801.py`

 * *Files identical despite different names*

### Comparing `djangoldp_uploader-2.1.2/djangoldp_uploader/migrations/0010_auto_20210208_0918.py` & `djangoldp_uploader-3.0.0/djangoldp_uploader/migrations/0010_auto_20210208_0918.py`

 * *Files identical despite different names*

### Comparing `djangoldp_uploader-2.1.2/djangoldp_uploader/migrations/0008_auto_20210202_1058.py` & `djangoldp_uploader-3.0.0/djangoldp_uploader/migrations/0008_auto_20210202_1058.py`

 * *Files identical despite different names*

### Comparing `djangoldp_uploader-2.1.2/djangoldp_uploader/templates/demo_sib.html` & `djangoldp_uploader-3.0.0/djangoldp_uploader/templates/demo_sib.html`

 * *Files identical despite different names*

### Comparing `djangoldp_uploader-2.1.2/djangoldp_uploader/templates/home.html` & `djangoldp_uploader-3.0.0/djangoldp_uploader/templates/home.html`

 * *Files identical despite different names*

