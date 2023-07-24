# Comparing `tmp/marqo-1.0.0.tar.gz` & `tmp/marqo-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marqo-1.0.0.tar", last modified: Fri Jul 21 05:03:38 2023, max compression
+gzip compressed data, was "marqo-1.1.0.tar", last modified: Mon Jul 24 07:09:36 2023, max compression
```

## Comparing `marqo-1.0.0.tar` & `marqo-1.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:03:38.649696 marqo-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-07-21 05:03:25.000000 marqo-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21541 2023-07-21 05:03:38.649696 marqo-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21088 2023-07-21 05:03:25.000000 marqo-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-21 05:03:25.000000 marqo-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 05:03:38.649696 marqo-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-21 05:03:25.000000 marqo-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:03:38.645696 marqo-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:03:38.649696 marqo-1.0.0/src/marqo/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-21 05:03:25.000000 marqo-1.0.0/src/marqo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-07-21 05:03:25.000000 marqo-1.0.0/src/marqo/_httprequests.py
--rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-07-21 05:03:25.000000 marqo-1.0.0/src/marqo/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-21 05:03:25.000000 marqo-1.0.0/src/marqo/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-21 05:03:25.000000 marqo-1.0.0/src/marqo/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-21 05:03:25.000000 marqo-1.0.0/src/marqo/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-07-21 05:03:25.000000 marqo-1.0.0/src/marqo/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    25202 2023-07-21 05:03:25.000000 marqo-1.0.0/src/marqo/index.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-21 05:03:25.000000 marqo-1.0.0/src/marqo/marqo_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-21 05:03:25.000000 marqo-1.0.0/src/marqo/marqo_url_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-21 05:03:25.000000 marqo-1.0.0/src/marqo/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-21 05:03:25.000000 marqo-1.0.0/src/marqo/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-21 05:03:25.000000 marqo-1.0.0/src/marqo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:03:38.649696 marqo-1.0.0/src/marqo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21541 2023-07-21 05:03:38.000000 marqo-1.0.0/src/marqo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-21 05:03:38.000000 marqo-1.0.0/src/marqo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 05:03:38.000000 marqo-1.0.0/src/marqo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-21 05:03:38.000000 marqo-1.0.0/src/marqo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 05:03:38.000000 marqo-1.0.0/src/marqo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:09:36.437403 marqo-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-07-24 07:09:25.000000 marqo-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21541 2023-07-24 07:09:36.437403 marqo-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21088 2023-07-24 07:09:25.000000 marqo-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-24 07:09:25.000000 marqo-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 07:09:36.437403 marqo-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-24 07:09:25.000000 marqo-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:09:36.429403 marqo-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:09:36.433403 marqo-1.1.0/src/marqo/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-24 07:09:25.000000 marqo-1.1.0/src/marqo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-07-24 07:09:25.000000 marqo-1.1.0/src/marqo/_httprequests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-07-24 07:09:25.000000 marqo-1.1.0/src/marqo/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-24 07:09:25.000000 marqo-1.1.0/src/marqo/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-24 07:09:25.000000 marqo-1.1.0/src/marqo/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-24 07:09:25.000000 marqo-1.1.0/src/marqo/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-07-24 07:09:25.000000 marqo-1.1.0/src/marqo/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25545 2023-07-24 07:09:25.000000 marqo-1.1.0/src/marqo/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-24 07:09:25.000000 marqo-1.1.0/src/marqo/marqo_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-24 07:09:25.000000 marqo-1.1.0/src/marqo/marqo_url_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-24 07:09:25.000000 marqo-1.1.0/src/marqo/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-24 07:09:25.000000 marqo-1.1.0/src/marqo/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-24 07:09:25.000000 marqo-1.1.0/src/marqo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:09:36.437403 marqo-1.1.0/src/marqo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21541 2023-07-24 07:09:36.000000 marqo-1.1.0/src/marqo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-24 07:09:36.000000 marqo-1.1.0/src/marqo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 07:09:36.000000 marqo-1.1.0/src/marqo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-24 07:09:36.000000 marqo-1.1.0/src/marqo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 07:09:36.000000 marqo-1.1.0/src/marqo.egg-info/top_level.txt
```

### Comparing `marqo-1.0.0/LICENSE` & `marqo-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `marqo-1.0.0/PKG-INFO` & `marqo-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marqo
-Version: 1.0.0
+Version: 1.1.0
 Summary: Tensor search for humans
 Author: marqo org
 Author-email: org@marqo.io
 Keywords: search python marqo opensearch tensor neural semantic vector embedding
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: marqo Version: 1.0.0 Summary: Tensor search for
+Metadata-Version: 2.1 Name: marqo Version: 1.1.0 Summary: Tensor search for
 humans Author: marqo org Author-email: org@marqo.io Keywords: search python
 marqo opensearch tensor neural semantic vector embedding Classifier:
 Programming Language :: Python :: 3.8 Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
 LICENSE
           [https://uploads-ssl.webflow.com/62dfa8e3960a6e2b47dc7fae/
```

### Comparing `marqo-1.0.0/README.md` & `marqo-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `marqo-1.0.0/setup.py` & `marqo-1.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         "packaging"
     ],
     tests_require=[
         "pytest",
         "tox"
     ],
     name="marqo",
-    version="1.0.0",
+    version="1.1.0",
     author="marqo org",
     author_email="org@marqo.io",
     description="Tensor search for humans",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(where="src", exclude=("tests*",)),
     keywords="search python marqo opensearch tensor neural semantic vector embedding",
```

### Comparing `marqo-1.0.0/src/marqo/_httprequests.py` & `marqo-1.1.0/src/marqo/_httprequests.py`

 * *Files identical despite different names*

### Comparing `marqo-1.0.0/src/marqo/client.py` & `marqo-1.1.0/src/marqo/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,16 @@
         sentences_per_chunk=2,
         sentence_overlap=0,
         image_preprocessing_method=None,
         settings_dict=None,
         inference_node_type=None,
         storage_node_type=None,
         inference_node_count=1,
+        storage_node_count=1,
+        replicas_count=0,
     ) -> Dict[str, Any]:
         """Create the index. Please refer to the marqo cloud to see options for inference and storage node types.
 
         Args:
             index_name: name of the index.
             treat_urls_and_pointers_as_images:
             model:
@@ -75,25 +77,28 @@
             image_preprocessing_method:
             settings_dict: if specified, overwrites all other setting
                 parameters, and is passed directly as the index's
                 index_settings
             inference_node_type:
             storage_node_type:
             inference_node_count;
+            storage_node_count:
+            replicas_count:
         Returns:
             Response body, containing information about index creation result
         """
         return Index.create(
             config=self.config, index_name=index_name,
             treat_urls_and_pointers_as_images=treat_urls_and_pointers_as_images,
             model=model, normalize_embeddings=normalize_embeddings,
             sentences_per_chunk=sentences_per_chunk, sentence_overlap=sentence_overlap,
             image_preprocessing_method=image_preprocessing_method,
             settings_dict=settings_dict, inference_node_type=inference_node_type, storage_node_type=storage_node_type,
-            inference_node_count=inference_node_count
+            storage_node_count=storage_node_count, replicas_count=replicas_count,
+            inference_node_count=inference_node_count,
         )
 
     def delete_index(self, index_name: str) -> Dict[str, Any]:
         """Deletes an index
 
         Args:
             index_name: name of the index
```

### Comparing `marqo-1.0.0/src/marqo/config.py` & `marqo-1.1.0/src/marqo/config.py`

 * *Files identical despite different names*

### Comparing `marqo-1.0.0/src/marqo/defaults.py` & `marqo-1.1.0/src/marqo/defaults.py`

 * *Files identical despite different names*

### Comparing `marqo-1.0.0/src/marqo/errors.py` & `marqo-1.1.0/src/marqo/errors.py`

 * *Files identical despite different names*

### Comparing `marqo-1.0.0/src/marqo/index.py` & `marqo-1.1.0/src/marqo/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,16 @@
                sentences_per_chunk=2,
                sentence_overlap=0,
                image_preprocessing_method=None,
                settings_dict: dict = None,
                inference_node_type: str = None,
                storage_node_type: str = None,
                inference_node_count: int = 1,
+               storage_node_count: int = 1,
+               replicas_count: int = 0,
                ) -> Dict[str, Any]:
         """Create the index.
 
         Args:
             config: config instance
             index_name: name of the index.
             treat_urls_and_pointers_as_images:
@@ -74,14 +76,16 @@
             image_preprocessing_method:
             settings_dict: if specified, overwrites all other setting
                 parameters, and is passed directly as the index's
                 index_settings
             inference_node_type: inference type for the index
             storage_node_type: storage type for the index
             inference_node_count: number of inference nodes for the index
+            storage_node_count: number of storage nodes for the index
+            replicas_count: number of replicas for the index
         Returns:
             Response body, containing information about index creation result
         """
         req = HttpRequests(config)
 
         if settings_dict is not None and settings_dict:
             return req.post(f"indexes/{index_name}", body=settings_dict)
@@ -99,15 +103,17 @@
             cl_text_preprocessing['split_length'] = sentences_per_chunk
             cl_img_preprocessing = cl_ix_defaults['image_preprocessing']
             cl_img_preprocessing['patch_method'] = image_preprocessing_method
             if not config.cluster_is_marqo:
                 return req.post(f"indexes/{index_name}", body=cl_settings)
             cl_settings['inference_type'] = inference_node_type
             cl_settings['storage_class'] = storage_node_type
-            cl_settings['inference_node_count'] = inference_node_count
+            cl_settings['number_of_inferences'] = inference_node_count
+            cl_settings['number_of_replicas'] = replicas_count
+            cl_settings['number_of_shards'] = storage_node_count
             response = req.post(f"indexes/{index_name}", body=cl_settings)
             index = Index(config, index_name)
             creation = index.get_status()
             while creation['index_status'] != 'READY':
                 time.sleep(10)
                 creation = index.get_status()
                 mq_logger.info(f"Index creation status: {creation['index_status']}")
```

### Comparing `marqo-1.0.0/src/marqo/marqo_url_resolver.py` & `marqo-1.1.0/src/marqo/marqo_url_resolver.py`

 * *Files identical despite different names*

### Comparing `marqo-1.0.0/src/marqo/models.py` & `marqo-1.1.0/src/marqo/models.py`

 * *Files identical despite different names*

### Comparing `marqo-1.0.0/src/marqo/utils.py` & `marqo-1.1.0/src/marqo/utils.py`

 * *Files identical despite different names*

### Comparing `marqo-1.0.0/src/marqo/version.py` & `marqo-1.1.0/src/marqo/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __marqo_version__ = "1.0.0"
 __marqo_release_page__ = f"https://github.com/marqo-ai/marqo/releases/tag/{__marqo_version__}"
 
-__minimum_supported_marqo_version__ = "0.1.0"
+__minimum_supported_marqo_version__ = "1.0.0"
 
 
 def supported_marqo_version() -> str:
     return f"This Marqo Python client is built for Marqo release ({__marqo_version__}) \n" \
            f"{__marqo_release_page__} \n" \
            f"The minimum supported Marqo version for this client is ({__minimum_supported_marqo_version__}) \n"
```

### Comparing `marqo-1.0.0/src/marqo.egg-info/PKG-INFO` & `marqo-1.1.0/src/marqo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marqo
-Version: 1.0.0
+Version: 1.1.0
 Summary: Tensor search for humans
 Author: marqo org
 Author-email: org@marqo.io
 Keywords: search python marqo opensearch tensor neural semantic vector embedding
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: marqo Version: 1.0.0 Summary: Tensor search for
+Metadata-Version: 2.1 Name: marqo Version: 1.1.0 Summary: Tensor search for
 humans Author: marqo org Author-email: org@marqo.io Keywords: search python
 marqo opensearch tensor neural semantic vector embedding Classifier:
 Programming Language :: Python :: 3.8 Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
 LICENSE
           [https://uploads-ssl.webflow.com/62dfa8e3960a6e2b47dc7fae/
```

