# Comparing `tmp/djangondor-1.0.3.tar.gz` & `tmp/djangondor-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangondor-1.0.3.tar", last modified: Mon Jul 24 09:02:25 2023, max compression
+gzip compressed data, was "djangondor-1.0.5.tar", last modified: Mon Jul 24 11:37:12 2023, max compression
```

## Comparing `djangondor-1.0.3.tar` & `djangondor-1.0.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-24 09:02:25.366150 djangondor-1.0.3/
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     1103 2023-07-21 07:05:22.000000 djangondor-1.0.3/LICENSE
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     1234 2023-07-24 09:02:25.366150 djangondor-1.0.3/PKG-INFO
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      349 2023-07-24 07:35:28.000000 djangondor-1.0.3/README.rst
-drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-24 09:02:25.366150 djangondor-1.0.3/djangondor/
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 20:57:03.000000 djangondor-1.0.3/djangondor/__init__.py
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       63 2023-07-23 20:57:03.000000 djangondor-1.0.3/djangondor/admin.py
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      152 2023-07-23 20:57:03.000000 djangondor-1.0.3/djangondor/apps.py
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      645 2023-07-23 12:18:10.000000 djangondor-1.0.3/djangondor/collections.py
-drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-24 09:02:25.366150 djangondor-1.0.3/djangondor/migrations/
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 20:57:03.000000 djangondor-1.0.3/djangondor/migrations/__init__.py
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      822 2023-07-24 06:11:18.000000 djangondor-1.0.3/djangondor/models.py
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     3417 2023-07-24 05:04:05.000000 djangondor-1.0.3/djangondor/processing.py
-drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-24 09:02:25.366150 djangondor-1.0.3/djangondor/templatetags/
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 11:24:34.000000 djangondor-1.0.3/djangondor/templatetags/__init__.py
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      410 2023-07-23 11:25:18.000000 djangondor-1.0.3/djangondor/templatetags/djangondor_collection_tags.py
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     1601 2023-07-23 11:22:38.000000 djangondor-1.0.3/djangondor/templatetags/djangondor_path_tags.py
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       60 2023-07-23 20:57:03.000000 djangondor-1.0.3/djangondor/tests.py
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      909 2023-07-21 07:30:17.000000 djangondor-1.0.3/djangondor/time.py
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       63 2023-07-23 20:57:03.000000 djangondor-1.0.3/djangondor/views.py
-drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-24 09:02:25.366150 djangondor-1.0.3/djangondor.egg-info/
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     1234 2023-07-24 09:02:25.000000 djangondor-1.0.3/djangondor.egg-info/PKG-INFO
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      586 2023-07-24 09:02:25.000000 djangondor-1.0.3/djangondor.egg-info/SOURCES.txt
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)        1 2023-07-24 09:02:25.000000 djangondor-1.0.3/djangondor.egg-info/dependency_links.txt
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       12 2023-07-24 09:02:25.000000 djangondor-1.0.3/djangondor.egg-info/requires.txt
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       11 2023-07-24 09:02:25.000000 djangondor-1.0.3/djangondor.egg-info/top_level.txt
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       89 2023-07-23 21:09:19.000000 djangondor-1.0.3/pyproject.toml
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      894 2023-07-24 09:02:25.370150 djangondor-1.0.3/setup.cfg
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      106 2023-07-24 08:43:55.000000 djangondor-1.0.3/setup.py
+drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-24 11:37:12.113738 djangondor-1.0.5/
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     1103 2023-07-21 07:05:22.000000 djangondor-1.0.5/LICENSE
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     1234 2023-07-24 11:37:12.113738 djangondor-1.0.5/PKG-INFO
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      349 2023-07-24 07:35:28.000000 djangondor-1.0.5/README.rst
+drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-24 11:37:12.109738 djangondor-1.0.5/djangondor/
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 20:57:03.000000 djangondor-1.0.5/djangondor/__init__.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       63 2023-07-23 20:57:03.000000 djangondor-1.0.5/djangondor/admin.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      152 2023-07-23 20:57:03.000000 djangondor-1.0.5/djangondor/apps.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      864 2023-07-24 10:15:33.000000 djangondor-1.0.5/djangondor/collections.py
+drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-24 11:37:12.109738 djangondor-1.0.5/djangondor/migrations/
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 20:57:03.000000 djangondor-1.0.5/djangondor/migrations/__init__.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     1017 2023-07-24 09:39:33.000000 djangondor-1.0.5/djangondor/models.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     3417 2023-07-24 05:04:05.000000 djangondor-1.0.5/djangondor/processing.py
+drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-24 11:37:12.113738 djangondor-1.0.5/djangondor/templatetags/
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 11:24:34.000000 djangondor-1.0.5/djangondor/templatetags/__init__.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      410 2023-07-23 11:25:18.000000 djangondor-1.0.5/djangondor/templatetags/djangondor_collection_tags.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     1601 2023-07-23 11:22:38.000000 djangondor-1.0.5/djangondor/templatetags/djangondor_path_tags.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       60 2023-07-23 20:57:03.000000 djangondor-1.0.5/djangondor/tests.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      909 2023-07-21 07:30:17.000000 djangondor-1.0.5/djangondor/time.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       63 2023-07-23 20:57:03.000000 djangondor-1.0.5/djangondor/views.py
+drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-24 11:37:12.109738 djangondor-1.0.5/djangondor.egg-info/
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     1234 2023-07-24 11:37:12.000000 djangondor-1.0.5/djangondor.egg-info/PKG-INFO
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      586 2023-07-24 11:37:12.000000 djangondor-1.0.5/djangondor.egg-info/SOURCES.txt
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)        1 2023-07-24 11:37:12.000000 djangondor-1.0.5/djangondor.egg-info/dependency_links.txt
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       12 2023-07-24 11:37:12.000000 djangondor-1.0.5/djangondor.egg-info/requires.txt
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       11 2023-07-24 11:37:12.000000 djangondor-1.0.5/djangondor.egg-info/top_level.txt
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       89 2023-07-23 21:09:19.000000 djangondor-1.0.5/pyproject.toml
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      894 2023-07-24 11:37:12.113738 djangondor-1.0.5/setup.cfg
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      106 2023-07-24 08:43:55.000000 djangondor-1.0.5/setup.py
```

### Comparing `djangondor-1.0.3/LICENSE` & `djangondor-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `djangondor-1.0.3/PKG-INFO` & `djangondor-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangondor
-Version: 1.0.3
+Version: 1.0.5
 Summary: A collection of django utilities.
 Home-page: https://github.com/dalitsosakala/djangondor
 Author: Dalitso Sakala
 Author-email: dalitso.1sc@gmail.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `djangondor-1.0.3/djangondor/models.py` & `djangondor-1.0.5/djangondor/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,13 +19,22 @@
 # id=models.UUIDField(**UUID_PK)
 # # is the same as:
 # id=models.UUIDField(primary_key=True, default=uuid.uuid4, editable=False)
 UUID_PK = {"primary_key": True, "default": uuid.uuid4, "editable": False}
 
 
 class BaseTimestampModel(models.Model):
-    '''Inherit this model to add time stamps to your models'''
+    """Inherit this model to add time stamps to your models"""
+
     updated_at = models.DateTimeField(auto_now=True)
     created_at = models.DateTimeField(auto_now_add=True, editable=False)
 
     class Meta:
         abstract = True
+
+
+class UUIDBaseTimestampModel(BaseTimestampModel):
+    """Inherit this model to add have a uuid pk andtimestamp"""
+    id = models.UUIDField(**UUID_PK)
+
+    class Meta:
+        abstract = True
```

### Comparing `djangondor-1.0.3/djangondor/processing.py` & `djangondor-1.0.5/djangondor/processing.py`

 * *Files identical despite different names*

### Comparing `djangondor-1.0.3/djangondor/templatetags/djangondor_path_tags.py` & `djangondor-1.0.5/djangondor/templatetags/djangondor_path_tags.py`

 * *Files identical despite different names*

### Comparing `djangondor-1.0.3/djangondor/time.py` & `djangondor-1.0.5/djangondor/time.py`

 * *Files identical despite different names*

### Comparing `djangondor-1.0.3/djangondor.egg-info/PKG-INFO` & `djangondor-1.0.5/djangondor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangondor
-Version: 1.0.3
+Version: 1.0.5
 Summary: A collection of django utilities.
 Home-page: https://github.com/dalitsosakala/djangondor
 Author: Dalitso Sakala
 Author-email: dalitso.1sc@gmail.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `djangondor-1.0.3/djangondor.egg-info/SOURCES.txt` & `djangondor-1.0.5/djangondor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangondor-1.0.3/setup.cfg` & `djangondor-1.0.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = djangondor
-version = 1.0.3
+version = 1.0.5
 description = A collection of django utilities.
 long_description = file: README.rst
 url = https://github.com/dalitsosakala/djangondor
 author = Dalitso Sakala
 author_email = dalitso.1sc@gmail.com
 license = MIT License
 classifiers =
```

