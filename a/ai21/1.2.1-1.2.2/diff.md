# Comparing `tmp/ai21-1.2.1.tar.gz` & `tmp/ai21-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai21-1.2.1.tar", last modified: Mon Jul 17 16:20:04 2023, max compression
+gzip compressed data, was "ai21-1.2.2.tar", last modified: Mon Jul 24 10:32:09 2023, max compression
```

## Comparing `ai21-1.2.1.tar` & `ai21-1.2.2.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-07-17 16:20:04.677141 ai21-1.2.1/
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1065 2023-03-25 06:53:34.000000 ai21-1.2.1/LICENSE
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     4577 2023-07-17 16:20:04.677331 ai21-1.2.1/PKG-INFO
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     3595 2023-07-15 13:04:46.000000 ai21-1.2.1/README.md
-drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-07-17 16:20:04.650141 ai21-1.2.1/ai21/
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     2317 2023-07-17 14:08:40.000000 ai21-1.2.1/ai21/AWS_utils.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      919 2023-07-17 13:50:26.000000 ai21-1.2.1/ai21/__init__.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      971 2023-06-08 14:30:41.000000 ai21-1.2.1/ai21/ai21_object.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     2055 2023-06-08 14:30:41.000000 ai21-1.2.1/ai21/ai21_studio_client.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      473 2023-06-08 14:30:41.000000 ai21-1.2.1/ai21/api_resources.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     2195 2023-07-15 13:04:46.000000 ai21-1.2.1/ai21/bedrock_client.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      250 2023-07-15 13:04:46.000000 ai21-1.2.1/ai21/constants.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     3273 2023-07-15 13:04:46.000000 ai21-1.2.1/ai21/errors.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     4034 2023-06-08 14:30:41.000000 ai21-1.2.1/ai21/http_client.py
-drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-07-17 16:20:04.659741 ai21-1.2.1/ai21/modules/
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)        0 2023-06-08 14:30:41.000000 ai21-1.2.1/ai21/modules/__init__.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1993 2023-07-17 14:08:40.000000 ai21-1.2.1/ai21/modules/completion.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      856 2023-07-17 10:29:52.000000 ai21-1.2.1/ai21/modules/custom_model.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      654 2023-07-17 13:48:31.000000 ai21-1.2.1/ai21/modules/dataset.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      534 2023-07-17 14:08:40.000000 ai21-1.2.1/ai21/modules/destination.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1740 2023-07-17 14:08:40.000000 ai21-1.2.1/ai21/modules/experimental.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      970 2023-07-17 14:08:40.000000 ai21-1.2.1/ai21/modules/gec.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      925 2023-06-08 14:30:41.000000 ai21-1.2.1/ai21/modules/improvements.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1368 2023-07-17 13:48:31.000000 ai21-1.2.1/ai21/modules/library.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      984 2023-07-17 14:08:40.000000 ai21-1.2.1/ai21/modules/paraphrase.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1088 2023-07-17 14:08:40.000000 ai21-1.2.1/ai21/modules/question_answering.py
-drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-07-17 16:20:04.673912 ai21-1.2.1/ai21/modules/resources/
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)        0 2023-06-08 14:30:41.000000 ai21-1.2.1/ai21/modules/resources/__init__.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      585 2023-07-17 10:29:12.000000 ai21-1.2.1/ai21/modules/resources/ai21_module.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      371 2023-06-08 14:30:41.000000 ai21-1.2.1/ai21/modules/resources/creatable_resource.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1793 2023-07-17 14:08:40.000000 ai21-1.2.1/ai21/modules/resources/execution_utils.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      352 2023-06-08 14:30:41.000000 ai21-1.2.1/ai21/modules/resources/listable_resource.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     2059 2023-07-17 10:29:07.000000 ai21-1.2.1/ai21/modules/resources/nlp_task.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      391 2023-07-17 13:52:59.000000 ai21-1.2.1/ai21/modules/resources/retrievable_resource.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      404 2023-07-17 13:52:59.000000 ai21-1.2.1/ai21/modules/resources/updatable_resource.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      480 2023-07-17 13:48:31.000000 ai21-1.2.1/ai21/modules/resources/upload_resource.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      915 2023-06-08 14:30:41.000000 ai21-1.2.1/ai21/modules/segmentation.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1148 2023-07-17 14:08:40.000000 ai21-1.2.1/ai21/modules/summarize.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      693 2023-06-08 14:30:41.000000 ai21-1.2.1/ai21/modules/tokenization.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     3038 2023-06-08 14:30:41.000000 ai21-1.2.1/ai21/utils.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)       22 2023-07-17 16:19:37.000000 ai21-1.2.1/ai21/version.py
-drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-07-17 16:20:04.651239 ai21-1.2.1/ai21.egg-info/
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     4577 2023-07-17 16:20:04.000000 ai21-1.2.1/ai21.egg-info/PKG-INFO
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1139 2023-07-17 16:20:04.000000 ai21-1.2.1/ai21.egg-info/SOURCES.txt
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)        1 2023-07-17 16:20:04.000000 ai21-1.2.1/ai21.egg-info/dependency_links.txt
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)       50 2023-07-17 16:20:04.000000 ai21-1.2.1/ai21.egg-info/requires.txt
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)        5 2023-07-17 16:20:04.000000 ai21-1.2.1/ai21.egg-info/top_level.txt
--rwxr-xr-x   0 amirkoblyansky   (501) staff       (20)      155 2023-07-17 16:20:04.677662 ai21-1.2.1/setup.cfg
--rwxr-xr-x   0 amirkoblyansky   (501) staff       (20)      613 2023-07-17 16:18:28.000000 ai21-1.2.1/setup.py
+drwxr-xr-x   0 haimon     (501) staff       (20)        0 2023-07-24 10:32:09.142168 ai21-1.2.2/
+-rw-r--r--   0 haimon     (501) staff       (20)     1065 2023-07-24 08:05:55.000000 ai21-1.2.2/LICENSE
+-rw-r--r--   0 haimon     (501) staff       (20)     4577 2023-07-24 10:32:09.142324 ai21-1.2.2/PKG-INFO
+-rw-r--r--   0 haimon     (501) staff       (20)     3595 2023-07-24 08:05:55.000000 ai21-1.2.2/README.md
+drwxr-xr-x   0 haimon     (501) staff       (20)        0 2023-07-24 10:32:09.127043 ai21-1.2.2/ai21/
+-rw-r--r--   0 haimon     (501) staff       (20)     2317 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/AWS_utils.py
+-rw-r--r--   0 haimon     (501) staff       (20)      919 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/__init__.py
+-rw-r--r--   0 haimon     (501) staff       (20)      971 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/ai21_object.py
+-rw-r--r--   0 haimon     (501) staff       (20)     2055 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/ai21_studio_client.py
+-rw-r--r--   0 haimon     (501) staff       (20)      473 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/api_resources.py
+-rw-r--r--   0 haimon     (501) staff       (20)     2195 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/bedrock_client.py
+-rw-r--r--   0 haimon     (501) staff       (20)      250 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/constants.py
+-rw-r--r--   0 haimon     (501) staff       (20)     3273 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/errors.py
+-rw-r--r--   0 haimon     (501) staff       (20)     4034 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/http_client.py
+drwxr-xr-x   0 haimon     (501) staff       (20)        0 2023-07-24 10:32:09.133197 ai21-1.2.2/ai21/modules/
+-rw-r--r--   0 haimon     (501) staff       (20)        0 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/__init__.py
+-rw-r--r--   0 haimon     (501) staff       (20)     1993 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/completion.py
+-rw-r--r--   0 haimon     (501) staff       (20)      856 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/custom_model.py
+-rw-r--r--   0 haimon     (501) staff       (20)      658 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/dataset.py
+-rw-r--r--   0 haimon     (501) staff       (20)      534 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/destination.py
+-rw-r--r--   0 haimon     (501) staff       (20)     1740 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/experimental.py
+-rw-r--r--   0 haimon     (501) staff       (20)      970 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/gec.py
+-rw-r--r--   0 haimon     (501) staff       (20)      925 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/improvements.py
+-rw-r--r--   0 haimon     (501) staff       (20)     1463 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/library.py
+-rw-r--r--   0 haimon     (501) staff       (20)      984 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/paraphrase.py
+-rw-r--r--   0 haimon     (501) staff       (20)     1088 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/question_answering.py
+drwxr-xr-x   0 haimon     (501) staff       (20)        0 2023-07-24 10:32:09.141720 ai21-1.2.2/ai21/modules/resources/
+-rw-r--r--   0 haimon     (501) staff       (20)        0 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/resources/__init__.py
+-rw-r--r--   0 haimon     (501) staff       (20)      585 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/resources/ai21_module.py
+-rw-r--r--   0 haimon     (501) staff       (20)      371 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/resources/creatable_resource.py
+-rw-r--r--   0 haimon     (501) staff       (20)      395 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/resources/deletable_resource.py
+-rw-r--r--   0 haimon     (501) staff       (20)     1793 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/resources/execution_utils.py
+-rw-r--r--   0 haimon     (501) staff       (20)      352 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/resources/listable_resource.py
+-rw-r--r--   0 haimon     (501) staff       (20)     2059 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/resources/nlp_task.py
+-rw-r--r--   0 haimon     (501) staff       (20)      391 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/resources/retrievable_resource.py
+-rw-r--r--   0 haimon     (501) staff       (20)      404 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/resources/updatable_resource.py
+-rw-r--r--   0 haimon     (501) staff       (20)      480 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/resources/uploadable_resource.py
+-rw-r--r--   0 haimon     (501) staff       (20)      915 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/segmentation.py
+-rw-r--r--   0 haimon     (501) staff       (20)     1148 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/summarize.py
+-rw-r--r--   0 haimon     (501) staff       (20)      693 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/tokenization.py
+-rw-r--r--   0 haimon     (501) staff       (20)     3038 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/utils.py
+-rw-r--r--   0 haimon     (501) staff       (20)       22 2023-07-24 10:13:17.000000 ai21-1.2.2/ai21/version.py
+drwxr-xr-x   0 haimon     (501) staff       (20)        0 2023-07-24 10:32:09.129269 ai21-1.2.2/ai21.egg-info/
+-rw-r--r--   0 haimon     (501) staff       (20)     4577 2023-07-24 10:32:09.000000 ai21-1.2.2/ai21.egg-info/PKG-INFO
+-rw-r--r--   0 haimon     (501) staff       (20)     1188 2023-07-24 10:32:09.000000 ai21-1.2.2/ai21.egg-info/SOURCES.txt
+-rw-r--r--   0 haimon     (501) staff       (20)        1 2023-07-24 10:32:09.000000 ai21-1.2.2/ai21.egg-info/dependency_links.txt
+-rw-r--r--   0 haimon     (501) staff       (20)       50 2023-07-24 10:32:09.000000 ai21-1.2.2/ai21.egg-info/requires.txt
+-rw-r--r--   0 haimon     (501) staff       (20)        5 2023-07-24 10:32:09.000000 ai21-1.2.2/ai21.egg-info/top_level.txt
+-rwxr-xr-x   0 haimon     (501) staff       (20)      155 2023-07-24 10:32:09.142671 ai21-1.2.2/setup.cfg
+-rwxr-xr-x   0 haimon     (501) staff       (20)      613 2023-07-24 08:05:55.000000 ai21-1.2.2/setup.py
```

### Comparing `ai21-1.2.1/LICENSE` & `ai21-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ai21-1.2.1/PKG-INFO` & `ai21-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai21
-Version: 1.2.1
+Version: 1.2.2
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: ai21 labs
 Author-email: support@ai21.com
 License: MIT
 Description: # AI21 Studio Client
         Python client for the AI21 Studio API
```

### Comparing `ai21-1.2.1/README.md` & `ai21-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `ai21-1.2.1/ai21/AWS_utils.py` & `ai21-1.2.2/ai21/AWS_utils.py`

 * *Files identical despite different names*

### Comparing `ai21-1.2.1/ai21/__init__.py` & `ai21-1.2.2/ai21/__init__.py`

 * *Files identical despite different names*

### Comparing `ai21-1.2.1/ai21/ai21_object.py` & `ai21-1.2.2/ai21/ai21_object.py`

 * *Files identical despite different names*

### Comparing `ai21-1.2.1/ai21/ai21_studio_client.py` & `ai21-1.2.2/ai21/ai21_studio_client.py`

 * *Files identical despite different names*

### Comparing `ai21-1.2.1/ai21/bedrock_client.py` & `ai21-1.2.2/ai21/bedrock_client.py`

 * *Files identical despite different names*

### Comparing `ai21-1.2.1/ai21/errors.py` & `ai21-1.2.2/ai21/errors.py`

 * *Files identical despite different names*

### Comparing `ai21-1.2.1/ai21/http_client.py` & `ai21-1.2.2/ai21/http_client.py`

 * *Files identical despite different names*

### Comparing `ai21-1.2.1/ai21/modules/completion.py` & `ai21-1.2.2/ai21/modules/completion.py`

 * *Files identical despite different names*

### Comparing `ai21-1.2.1/ai21/modules/custom_model.py` & `ai21-1.2.2/ai21/modules/custom_model.py`

 * *Files identical despite different names*

### Comparing `ai21-1.2.1/ai21/modules/dataset.py` & `ai21-1.2.2/ai21/modules/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from ai21.modules.resources.listable_resource import ListableResource
 from ai21.modules.resources.retrievable_resource import RetrievableResource
-from ai21.modules.resources.upload_resource import UploadableResource
+from ai21.modules.resources.uploadable_resource import UploadableResource
 from ai21.utils import validate_mandatory_field
 
 
 class Dataset(UploadableResource, RetrievableResource, ListableResource):
 
     MODULE_NAME = 'dataset'
```

### Comparing `ai21-1.2.1/ai21/modules/destination.py` & `ai21-1.2.2/ai21/modules/destination.py`

 * *Files identical despite different names*

### Comparing `ai21-1.2.1/ai21/modules/experimental.py` & `ai21-1.2.2/ai21/modules/experimental.py`

 * *Files identical despite different names*

### Comparing `ai21-1.2.1/ai21/modules/gec.py` & `ai21-1.2.2/ai21/modules/gec.py`

 * *Files identical despite different names*

### Comparing `ai21-1.2.1/ai21/modules/improvements.py` & `ai21-1.2.2/ai21/modules/improvements.py`

 * *Files identical despite different names*

### Comparing `ai21-1.2.1/ai21/modules/library.py` & `ai21-1.2.2/ai21/modules/library.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,21 @@
+from ai21.modules.resources.deletable_resource import DeletableResource
 from ai21.modules.resources.execution_utils import execute_studio_request
 from ai21.utils import validate_mandatory_field
 
 from ai21.modules.resources.nlp_task import NLPTask
 
 from ai21.modules.resources.listable_resource import ListableResource
 from ai21.modules.resources.retrievable_resource import RetrievableResource
 from ai21.modules.resources.updatable_resource import UpdatableResource
-from ai21.modules.resources.upload_resource import UploadableResource
+from ai21.modules.resources.uploadable_resource import UploadableResource
 
 
 class Library:
-    class Files(UploadableResource, RetrievableResource, ListableResource, UpdatableResource):
+    class Files(UploadableResource, RetrievableResource, ListableResource, UpdatableResource, DeletableResource):
         MODULE_NAME = 'library/files'
 
         @classmethod
         def upload(cls, file_path: str, **params):
             return super().upload(file_path=file_path, file_param_name='file', **params)
 
     class Answer(NLPTask):
```

### Comparing `ai21-1.2.1/ai21/modules/paraphrase.py` & `ai21-1.2.2/ai21/modules/paraphrase.py`

 * *Files identical despite different names*

### Comparing `ai21-1.2.1/ai21/modules/question_answering.py` & `ai21-1.2.2/ai21/modules/question_answering.py`

 * *Files identical despite different names*

### Comparing `ai21-1.2.1/ai21/modules/resources/ai21_module.py` & `ai21-1.2.2/ai21/modules/resources/ai21_module.py`

 * *Files identical despite different names*

### Comparing `ai21-1.2.1/ai21/modules/resources/execution_utils.py` & `ai21-1.2.2/ai21/modules/resources/execution_utils.py`

 * *Files identical despite different names*

### Comparing `ai21-1.2.1/ai21/modules/resources/nlp_task.py` & `ai21-1.2.2/ai21/modules/resources/nlp_task.py`

 * *Files identical despite different names*

### Comparing `ai21-1.2.1/ai21/modules/segmentation.py` & `ai21-1.2.2/ai21/modules/segmentation.py`

 * *Files identical despite different names*

### Comparing `ai21-1.2.1/ai21/modules/summarize.py` & `ai21-1.2.2/ai21/modules/summarize.py`

 * *Files identical despite different names*

### Comparing `ai21-1.2.1/ai21/modules/tokenization.py` & `ai21-1.2.2/ai21/modules/tokenization.py`

 * *Files identical despite different names*

### Comparing `ai21-1.2.1/ai21/utils.py` & `ai21-1.2.2/ai21/utils.py`

 * *Files identical despite different names*

### Comparing `ai21-1.2.1/ai21.egg-info/PKG-INFO` & `ai21-1.2.2/ai21.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai21
-Version: 1.2.1
+Version: 1.2.2
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: ai21 labs
 Author-email: support@ai21.com
 License: MIT
 Description: # AI21 Studio Client
         Python client for the AI21 Studio API
```

### Comparing `ai21-1.2.1/ai21.egg-info/SOURCES.txt` & `ai21-1.2.2/ai21.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -31,13 +31,14 @@
 ai21/modules/question_answering.py
 ai21/modules/segmentation.py
 ai21/modules/summarize.py
 ai21/modules/tokenization.py
 ai21/modules/resources/__init__.py
 ai21/modules/resources/ai21_module.py
 ai21/modules/resources/creatable_resource.py
+ai21/modules/resources/deletable_resource.py
 ai21/modules/resources/execution_utils.py
 ai21/modules/resources/listable_resource.py
 ai21/modules/resources/nlp_task.py
 ai21/modules/resources/retrievable_resource.py
 ai21/modules/resources/updatable_resource.py
-ai21/modules/resources/upload_resource.py
+ai21/modules/resources/uploadable_resource.py
```

### Comparing `ai21-1.2.1/setup.py` & `ai21-1.2.2/setup.py`

 * *Files identical despite different names*

