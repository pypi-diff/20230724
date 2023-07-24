# Comparing `tmp/djangondor-1.0.5.tar.gz` & `tmp/djangondor-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangondor-1.0.5.tar", last modified: Mon Jul 24 11:37:12 2023, max compression
+gzip compressed data, was "djangondor-1.1.0.tar", last modified: Mon Jul 24 19:49:31 2023, max compression
```

## Comparing `djangondor-1.0.5.tar` & `djangondor-1.1.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-24 11:37:12.113738 djangondor-1.0.5/
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     1103 2023-07-21 07:05:22.000000 djangondor-1.0.5/LICENSE
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     1234 2023-07-24 11:37:12.113738 djangondor-1.0.5/PKG-INFO
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      349 2023-07-24 07:35:28.000000 djangondor-1.0.5/README.rst
-drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-24 11:37:12.109738 djangondor-1.0.5/djangondor/
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 20:57:03.000000 djangondor-1.0.5/djangondor/__init__.py
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       63 2023-07-23 20:57:03.000000 djangondor-1.0.5/djangondor/admin.py
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      152 2023-07-23 20:57:03.000000 djangondor-1.0.5/djangondor/apps.py
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      864 2023-07-24 10:15:33.000000 djangondor-1.0.5/djangondor/collections.py
-drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-24 11:37:12.109738 djangondor-1.0.5/djangondor/migrations/
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 20:57:03.000000 djangondor-1.0.5/djangondor/migrations/__init__.py
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     1017 2023-07-24 09:39:33.000000 djangondor-1.0.5/djangondor/models.py
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     3417 2023-07-24 05:04:05.000000 djangondor-1.0.5/djangondor/processing.py
-drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-24 11:37:12.113738 djangondor-1.0.5/djangondor/templatetags/
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 11:24:34.000000 djangondor-1.0.5/djangondor/templatetags/__init__.py
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      410 2023-07-23 11:25:18.000000 djangondor-1.0.5/djangondor/templatetags/djangondor_collection_tags.py
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     1601 2023-07-23 11:22:38.000000 djangondor-1.0.5/djangondor/templatetags/djangondor_path_tags.py
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       60 2023-07-23 20:57:03.000000 djangondor-1.0.5/djangondor/tests.py
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      909 2023-07-21 07:30:17.000000 djangondor-1.0.5/djangondor/time.py
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       63 2023-07-23 20:57:03.000000 djangondor-1.0.5/djangondor/views.py
-drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-24 11:37:12.109738 djangondor-1.0.5/djangondor.egg-info/
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     1234 2023-07-24 11:37:12.000000 djangondor-1.0.5/djangondor.egg-info/PKG-INFO
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      586 2023-07-24 11:37:12.000000 djangondor-1.0.5/djangondor.egg-info/SOURCES.txt
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)        1 2023-07-24 11:37:12.000000 djangondor-1.0.5/djangondor.egg-info/dependency_links.txt
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       12 2023-07-24 11:37:12.000000 djangondor-1.0.5/djangondor.egg-info/requires.txt
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       11 2023-07-24 11:37:12.000000 djangondor-1.0.5/djangondor.egg-info/top_level.txt
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       89 2023-07-23 21:09:19.000000 djangondor-1.0.5/pyproject.toml
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      894 2023-07-24 11:37:12.113738 djangondor-1.0.5/setup.cfg
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      106 2023-07-24 08:43:55.000000 djangondor-1.0.5/setup.py
+drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-24 19:49:31.219409 djangondor-1.1.0/
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     1103 2023-07-21 07:05:22.000000 djangondor-1.1.0/LICENSE
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     1234 2023-07-24 19:49:31.219409 djangondor-1.1.0/PKG-INFO
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      349 2023-07-24 07:35:28.000000 djangondor-1.1.0/README.rst
+drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-24 19:49:31.215409 djangondor-1.1.0/djangondor/
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 20:57:03.000000 djangondor-1.1.0/djangondor/__init__.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       63 2023-07-23 20:57:03.000000 djangondor-1.1.0/djangondor/admin.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      152 2023-07-23 20:57:03.000000 djangondor-1.1.0/djangondor/apps.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      864 2023-07-24 10:15:33.000000 djangondor-1.1.0/djangondor/collections.py
+drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-24 19:49:31.219409 djangondor-1.1.0/djangondor/migrations/
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 20:57:03.000000 djangondor-1.1.0/djangondor/migrations/__init__.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     1294 2023-07-24 19:46:10.000000 djangondor-1.1.0/djangondor/models.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     3417 2023-07-24 05:04:05.000000 djangondor-1.1.0/djangondor/processing.py
+drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-24 19:49:31.219409 djangondor-1.1.0/djangondor/templatetags/
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 11:24:34.000000 djangondor-1.1.0/djangondor/templatetags/__init__.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      410 2023-07-23 11:25:18.000000 djangondor-1.1.0/djangondor/templatetags/djangondor_collection_tags.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     1601 2023-07-23 11:22:38.000000 djangondor-1.1.0/djangondor/templatetags/djangondor_path_tags.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       60 2023-07-23 20:57:03.000000 djangondor-1.1.0/djangondor/tests.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      909 2023-07-21 07:30:17.000000 djangondor-1.1.0/djangondor/time.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       63 2023-07-23 20:57:03.000000 djangondor-1.1.0/djangondor/views.py
+drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-24 19:49:31.219409 djangondor-1.1.0/djangondor.egg-info/
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     1234 2023-07-24 19:49:31.000000 djangondor-1.1.0/djangondor.egg-info/PKG-INFO
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      586 2023-07-24 19:49:31.000000 djangondor-1.1.0/djangondor.egg-info/SOURCES.txt
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)        1 2023-07-24 19:49:31.000000 djangondor-1.1.0/djangondor.egg-info/dependency_links.txt
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       12 2023-07-24 19:49:31.000000 djangondor-1.1.0/djangondor.egg-info/requires.txt
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       11 2023-07-24 19:49:31.000000 djangondor-1.1.0/djangondor.egg-info/top_level.txt
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       89 2023-07-23 21:09:19.000000 djangondor-1.1.0/pyproject.toml
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      894 2023-07-24 19:49:31.219409 djangondor-1.1.0/setup.cfg
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      106 2023-07-24 08:43:55.000000 djangondor-1.1.0/setup.py
```

### Comparing `djangondor-1.0.5/LICENSE` & `djangondor-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `djangondor-1.0.5/PKG-INFO` & `djangondor-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangondor
-Version: 1.0.5
+Version: 1.1.0
 Summary: A collection of django utilities.
 Home-page: https://github.com/dalitsosakala/djangondor
 Author: Dalitso Sakala
 Author-email: dalitso.1sc@gmail.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `djangondor-1.0.5/djangondor/collections.py` & `djangondor-1.1.0/djangondor/collections.py`

 * *Files identical despite different names*

### Comparing `djangondor-1.0.5/djangondor/models.py` & `djangondor-1.1.0/djangondor/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,34 +7,42 @@
 # NULLABLE
 # USAGE
 # =====
 # description = models.CharField(max_length=200,**NULLABLE)
 # # is the same as:
 # description = models.CharField(max_length=200,null=True,default=None,blank=True)
 NULLABLE = {"null": True, "default": None, "blank": True}
+NULLABLE_CHARFIELD = {**NULLABLE, "max_length": 100}
 
 
 # UUID_PK
 # USAGE
 # =====
 # id=models.UUIDField(**UUID_PK)
 # # is the same as:
 # id=models.UUIDField(primary_key=True, default=uuid.uuid4, editable=False)
 UUID_PK = {"primary_key": True, "default": uuid.uuid4, "editable": False}
 
 
+def make_choices(*entries):
+    """Make choices to passed to model field `choices` attribute. Each entry has the form `(entry,entry)`"""
+    return [(value, value) for value in entries]
+
+
 class BaseTimestampModel(models.Model):
     """Inherit this model to add time stamps to your models"""
 
     updated_at = models.DateTimeField(auto_now=True)
     created_at = models.DateTimeField(auto_now_add=True, editable=False)
 
     class Meta:
         abstract = True
+        ordering = ("updated_at",)
 
 
 class UUIDBaseTimestampModel(BaseTimestampModel):
     """Inherit this model to add have a uuid pk andtimestamp"""
+
     id = models.UUIDField(**UUID_PK)
 
     class Meta:
         abstract = True
```

### Comparing `djangondor-1.0.5/djangondor/processing.py` & `djangondor-1.1.0/djangondor/processing.py`

 * *Files identical despite different names*

### Comparing `djangondor-1.0.5/djangondor/templatetags/djangondor_path_tags.py` & `djangondor-1.1.0/djangondor/templatetags/djangondor_path_tags.py`

 * *Files identical despite different names*

### Comparing `djangondor-1.0.5/djangondor/time.py` & `djangondor-1.1.0/djangondor/time.py`

 * *Files identical despite different names*

### Comparing `djangondor-1.0.5/djangondor.egg-info/PKG-INFO` & `djangondor-1.1.0/djangondor.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangondor
-Version: 1.0.5
+Version: 1.1.0
 Summary: A collection of django utilities.
 Home-page: https://github.com/dalitsosakala/djangondor
 Author: Dalitso Sakala
 Author-email: dalitso.1sc@gmail.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `djangondor-1.0.5/djangondor.egg-info/SOURCES.txt` & `djangondor-1.1.0/djangondor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangondor-1.0.5/setup.cfg` & `djangondor-1.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = djangondor
-version = 1.0.5
+version = 1.1.0
 description = A collection of django utilities.
 long_description = file: README.rst
 url = https://github.com/dalitsosakala/djangondor
 author = Dalitso Sakala
 author_email = dalitso.1sc@gmail.com
 license = MIT License
 classifiers =
```

