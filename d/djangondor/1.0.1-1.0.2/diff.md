# Comparing `tmp/djangondor-1.0.1.tar.gz` & `tmp/djangondor-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangondor-1.0.1.tar", last modified: Sun Jul 23 22:25:54 2023, max compression
+gzip compressed data, was "djangondor-1.0.2.tar", last modified: Mon Jul 24 07:38:27 2023, max compression
```

## Comparing `djangondor-1.0.1.tar` & `djangondor-1.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 22:25:54.900786 djangondor-1.0.1/
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     1103 2023-07-21 07:05:22.000000 djangondor-1.0.1/LICENSE
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     1279 2023-07-23 22:25:54.900786 djangondor-1.0.1/PKG-INFO
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      394 2023-07-23 22:23:20.000000 djangondor-1.0.1/README.rst
-drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 22:25:54.896787 djangondor-1.0.1/djangondor/
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 20:57:03.000000 djangondor-1.0.1/djangondor/__init__.py
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       63 2023-07-23 20:57:03.000000 djangondor-1.0.1/djangondor/admin.py
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      152 2023-07-23 20:57:03.000000 djangondor-1.0.1/djangondor/apps.py
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      645 2023-07-23 12:18:10.000000 djangondor-1.0.1/djangondor/collections.py
-drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 22:25:54.900786 djangondor-1.0.1/djangondor/migrations/
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 20:57:03.000000 djangondor-1.0.1/djangondor/migrations/__init__.py
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       57 2023-07-23 20:57:03.000000 djangondor-1.0.1/djangondor/models.py
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     2800 2023-07-21 07:32:44.000000 djangondor-1.0.1/djangondor/requests.py
-drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 22:25:54.900786 djangondor-1.0.1/djangondor/templatetags/
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 11:24:34.000000 djangondor-1.0.1/djangondor/templatetags/__init__.py
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      410 2023-07-23 11:25:18.000000 djangondor-1.0.1/djangondor/templatetags/djangondor_collection_tags.py
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     1601 2023-07-23 11:22:38.000000 djangondor-1.0.1/djangondor/templatetags/djangondor_path_tags.py
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       60 2023-07-23 20:57:03.000000 djangondor-1.0.1/djangondor/tests.py
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      909 2023-07-21 07:30:17.000000 djangondor-1.0.1/djangondor/time.py
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       63 2023-07-23 20:57:03.000000 djangondor-1.0.1/djangondor/views.py
-drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 22:25:54.900786 djangondor-1.0.1/djangondor.egg-info/
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     1279 2023-07-23 22:25:54.000000 djangondor-1.0.1/djangondor.egg-info/PKG-INFO
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      584 2023-07-23 22:25:54.000000 djangondor-1.0.1/djangondor.egg-info/SOURCES.txt
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)        1 2023-07-23 22:25:54.000000 djangondor-1.0.1/djangondor.egg-info/dependency_links.txt
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       12 2023-07-23 22:25:54.000000 djangondor-1.0.1/djangondor.egg-info/requires.txt
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       11 2023-07-23 22:25:54.000000 djangondor-1.0.1/djangondor.egg-info/top_level.txt
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       89 2023-07-23 21:09:19.000000 djangondor-1.0.1/pyproject.toml
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      894 2023-07-23 22:25:54.900786 djangondor-1.0.1/setup.cfg
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       38 2023-07-23 21:11:32.000000 djangondor-1.0.1/setup.py
+drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-24 07:38:27.802236 djangondor-1.0.2/
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     1103 2023-07-21 07:05:22.000000 djangondor-1.0.2/LICENSE
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      883 2023-07-24 07:38:27.806236 djangondor-1.0.2/PKG-INFO
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      349 2023-07-24 07:35:28.000000 djangondor-1.0.2/README.rst
+drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-24 07:38:27.802236 djangondor-1.0.2/djangondor/
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 20:57:03.000000 djangondor-1.0.2/djangondor/__init__.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       63 2023-07-23 20:57:03.000000 djangondor-1.0.2/djangondor/admin.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      152 2023-07-23 20:57:03.000000 djangondor-1.0.2/djangondor/apps.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      645 2023-07-23 12:18:10.000000 djangondor-1.0.2/djangondor/collections.py
+drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-24 07:38:27.802236 djangondor-1.0.2/djangondor/migrations/
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 20:57:03.000000 djangondor-1.0.2/djangondor/migrations/__init__.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      822 2023-07-24 06:11:18.000000 djangondor-1.0.2/djangondor/models.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     3417 2023-07-24 05:04:05.000000 djangondor-1.0.2/djangondor/requests.py
+drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-24 07:38:27.802236 djangondor-1.0.2/djangondor/templatetags/
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 11:24:34.000000 djangondor-1.0.2/djangondor/templatetags/__init__.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      410 2023-07-23 11:25:18.000000 djangondor-1.0.2/djangondor/templatetags/djangondor_collection_tags.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     1601 2023-07-23 11:22:38.000000 djangondor-1.0.2/djangondor/templatetags/djangondor_path_tags.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       60 2023-07-23 20:57:03.000000 djangondor-1.0.2/djangondor/tests.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      909 2023-07-21 07:30:17.000000 djangondor-1.0.2/djangondor/time.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       63 2023-07-23 20:57:03.000000 djangondor-1.0.2/djangondor/views.py
+drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-24 07:38:27.802236 djangondor-1.0.2/djangondor.egg-info/
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      883 2023-07-24 07:38:27.000000 djangondor-1.0.2/djangondor.egg-info/PKG-INFO
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      584 2023-07-24 07:38:27.000000 djangondor-1.0.2/djangondor.egg-info/SOURCES.txt
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)        1 2023-07-24 07:38:27.000000 djangondor-1.0.2/djangondor.egg-info/dependency_links.txt
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       12 2023-07-24 07:38:27.000000 djangondor-1.0.2/djangondor.egg-info/requires.txt
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       11 2023-07-24 07:38:27.000000 djangondor-1.0.2/djangondor.egg-info/top_level.txt
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       89 2023-07-23 21:09:19.000000 djangondor-1.0.2/pyproject.toml
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      893 2023-07-24 07:38:27.806236 djangondor-1.0.2/setup.cfg
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       54 2023-07-24 07:05:11.000000 djangondor-1.0.2/setup.py
```

### Comparing `djangondor-1.0.1/LICENSE` & `djangondor-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `djangondor-1.0.1/PKG-INFO` & `djangondor-1.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangondor
-Version: 1.0.1
+Version: 1.0.2
 Summary: A collection of django utilities.
 Home-page: https://github.com/dalitsosakala/djangondor
 Author: Dalitso Sakala
 Author-email: dalitso.1sc@gmail.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -17,27 +17,7 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 License-File: LICENSE
-
-==========
-Djangondor
-==========
-
-Djangondor is a collection Django utilities.
-
-Detailed documentation is in the "docs" directory.
-
-Quick start
------------
-
-1. Add "djangondor" to your INSTALLED_APPS setting like this::
-
-    INSTALLED_APPS = [
-        ...,
-        "djangondor",
-    ]
-
-2. See the documentation at <https://github.com/DalitsoSakala/djangondor/blob/main/djangondor/docs/INDEX.md>
```

### Comparing `djangondor-1.0.1/djangondor/collections.py` & `djangondor-1.0.2/djangondor/collections.py`

 * *Files identical despite different names*

### Comparing `djangondor-1.0.1/djangondor/requests.py` & `djangondor-1.0.2/djangondor/requests.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,72 +1,93 @@
 from django import forms
 from typing import Dict
 from django.http import JsonResponse
 from django.db import models
 
 
-def save_many_and_respond(*models:models.Model,success_status=200,error_status=400):
+def save_many_and_respond(*models: models.Model, success_status=200, error_status=400):
+    """
+    Saves as many models as there are in `*models`.
+    This function returns a `JsonResponse` having a status `success_status` if saving was successful
+    or returns a `JsonResponse` with status `error_status`.
+    """
     try:
         for model in models:
             model.save()
 
     except Exception as e:
         return JsonResponse({"message": e.args[0]}, status=error_status)
-    return JsonResponse({"message": 'saved'}, status=success_status)
-
+    return JsonResponse({"message": "saved"}, status=success_status)
 
 
 def delete_and_respond(model: models.Model):
-    '''
+    """
     Deletes a model and returns a 204 `JsonResponse` response
-    '''
+    """
     try:
         model.delete()
         status = 204
         body = {}
     except:
         status = 400
         body = {"message": "Something is keeping you from deleting this object"}
 
     return JsonResponse(body, status=status)
 
 
 def save_and_respond(
-    model: models.Model,/, serialize_with=None, success_status=200, error_status=400,**kwargs
+    model: models.Model,
+    /,
+    serialize_with=None,
+    success_status=200,
+    error_status=400,
+    **kwargs,
 ):
-    '''
-    Saves a model and return a a json response.
-    '''
+    """
+    Saves a model and return a a `JsonResponse`.
+    The response will have a status of `success_status` if successful or `error_status` if saving
+    did not succeed.
+    """
     try:
-        for key,val in kwargs.items():
-            setattr(model,key,val)
+        for key, val in kwargs.items():
+            setattr(model, key, val)
         model.save()
         return JsonResponse(
             {"message": "saved"} if not serialize_with else serialize_with(model).data,
             status=success_status,
         )
     except Exception as e:
         return JsonResponse({"message": e.args[0]}, status=error_status)
 
 
 def format_form_errors(form: forms.ModelForm):
+    """
+    Attempts to read the error messages in the `form`.
+    """
+
     errors = form.errors.as_data()
     keys = list(errors.keys())
     values = list(errors.values())
-    items = [(keys[i], values[i][0].message) for i in range(0, len(errors))]
+    items = [
+        (keys[i], (values[i][0].message or "").replace("_", " "))
+        for i in range(0, len(errors))
+    ]
     return items
 
 
 def form_error_response(form: forms.ModelForm, status=400):
+    '''
+    Returns a `JsonRespnse` with having a representation of error messages
+    from `format_form_errors`.
+    '''
     return JsonResponse(
         {"message": "%s %s" % format_form_errors(form)[0]}, status=status
     )
 
 
-
 def process_form(
     form: forms.ModelForm, /, set_fields: Dict = None, error_status=400, respond=False
 ):
     """
     Return model that has been saved with `commit=False` when the form has no errors otherwise `None`
     and a `JsonResponse` object with the given `error_status` if the form had errors otherwise None
     The entries in `set_fields` are set on the model just after calling `save(commit=False)` on the form
@@ -83,8 +104,7 @@
                 return JsonResponse({"message": "saved"})
             except Exception as e:
                 return JsonResponse({"message": e.args[0]}, status=500)
         return model, None
     elif respond:
         return form_error_response(form)
     return None, form_error_response(form, error_status)
-
```

### Comparing `djangondor-1.0.1/djangondor/templatetags/djangondor_path_tags.py` & `djangondor-1.0.2/djangondor/templatetags/djangondor_path_tags.py`

 * *Files identical despite different names*

### Comparing `djangondor-1.0.1/djangondor/time.py` & `djangondor-1.0.2/djangondor/time.py`

 * *Files identical despite different names*

### Comparing `djangondor-1.0.1/djangondor.egg-info/PKG-INFO` & `djangondor-1.0.2/djangondor.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangondor
-Version: 1.0.1
+Version: 1.0.2
 Summary: A collection of django utilities.
 Home-page: https://github.com/dalitsosakala/djangondor
 Author: Dalitso Sakala
 Author-email: dalitso.1sc@gmail.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -17,27 +17,7 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 License-File: LICENSE
-
-==========
-Djangondor
-==========
-
-Djangondor is a collection Django utilities.
-
-Detailed documentation is in the "docs" directory.
-
-Quick start
------------
-
-1. Add "djangondor" to your INSTALLED_APPS setting like this::
-
-    INSTALLED_APPS = [
-        ...,
-        "djangondor",
-    ]
-
-2. See the documentation at <https://github.com/DalitsoSakala/djangondor/blob/main/djangondor/docs/INDEX.md>
```

### Comparing `djangondor-1.0.1/djangondor.egg-info/SOURCES.txt` & `djangondor-1.0.2/djangondor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangondor-1.0.1/setup.cfg` & `djangondor-1.0.2/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = djangondor
-version = 1.0.1
+version = 1.0.2
 description = A collection of django utilities.
-long_description = file: README.rst
+long_description = file: index.rst
 url = https://github.com/dalitsosakala/djangondor
 author = Dalitso Sakala
 author_email = dalitso.1sc@gmail.com
 license = MIT License
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
```

