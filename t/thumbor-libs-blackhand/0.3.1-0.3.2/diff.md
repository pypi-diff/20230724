# Comparing `tmp/thumbor_libs_blackhand-0.3.1.tar.gz` & `tmp/thumbor_libs_blackhand-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/thumbor_libs_blackhand-0.3.1.tar", last modified: Mon Jul 24 08:30:26 2023, max compression
+gzip compressed data, was "dist/thumbor_libs_blackhand-0.3.2.tar", last modified: Mon Jul 24 15:12:21 2023, max compression
```

## Comparing `thumbor_libs_blackhand-0.3.1.tar` & `thumbor_libs_blackhand-0.3.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:30:26.000000 thumbor_libs_blackhand-0.3.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:30:26.000000 thumbor_libs_blackhand-0.3.1/thumbor_libs_blackhand/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:30:26.000000 thumbor_libs_blackhand-0.3.1/thumbor_libs_blackhand/loaders/
--rw-rw-r--   0 root         (0) root         (0)      138 2023-07-24 08:20:38.000000 thumbor_libs_blackhand-0.3.1/thumbor_libs_blackhand/loaders/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1910 2023-07-24 08:20:38.000000 thumbor_libs_blackhand-0.3.1/thumbor_libs_blackhand/loaders/mongodb_loader.py
--rw-rw-r--   0 root         (0) root         (0)      533 2023-07-24 08:20:38.000000 thumbor_libs_blackhand-0.3.1/thumbor_libs_blackhand/loaders/spec_http_or_specb_loader.py
--rw-rw-r--   0 root         (0) root         (0)     2521 2023-07-24 08:20:38.000000 thumbor_libs_blackhand-0.3.1/thumbor_libs_blackhand/loaders/specb_file_fallback_file_loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:30:26.000000 thumbor_libs_blackhand-0.3.1/thumbor_libs_blackhand/metrics/
--rw-rw-r--   0 root         (0) root         (0)      138 2023-07-24 08:20:38.000000 thumbor_libs_blackhand-0.3.1/thumbor_libs_blackhand/metrics/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:30:26.000000 thumbor_libs_blackhand-0.3.1/thumbor_libs_blackhand/mongodb/
--rw-rw-r--   0 root         (0) root         (0)     1781 2023-07-24 08:20:38.000000 thumbor_libs_blackhand-0.3.1/thumbor_libs_blackhand/mongodb/pool_result_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:30:26.000000 thumbor_libs_blackhand-0.3.1/thumbor_libs_blackhand/result_storages/
--rw-rw-r--   0 root         (0) root         (0)      138 2023-07-24 08:20:38.000000 thumbor_libs_blackhand-0.3.1/thumbor_libs_blackhand/result_storages/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6672 2023-07-24 08:20:38.000000 thumbor_libs_blackhand-0.3.1/thumbor_libs_blackhand/result_storages/hybrid_result_storage.py
--rw-rw-r--   0 root         (0) root         (0)     3893 2023-07-24 08:20:38.000000 thumbor_libs_blackhand-0.3.1/thumbor_libs_blackhand/result_storages/mongodb_legacy_result_storage.py
--rw-rw-r--   0 root         (0) root         (0)     4217 2023-07-24 08:20:38.000000 thumbor_libs_blackhand-0.3.1/thumbor_libs_blackhand/result_storages/mongodb_legacy_result_storage_fix.py
--rw-rw-r--   0 root         (0) root         (0)     5442 2023-07-24 08:20:38.000000 thumbor_libs_blackhand-0.3.1/thumbor_libs_blackhand/result_storages/mongodb_result_storage.py
--rw-rw-r--   0 root         (0) root         (0)     5781 2023-07-24 08:20:38.000000 thumbor_libs_blackhand-0.3.1/thumbor_libs_blackhand/result_storages/mongodb_result_storage_v3.py
--rw-rw-r--   0 root         (0) root         (0)     3889 2023-07-24 08:20:38.000000 thumbor_libs_blackhand-0.3.1/thumbor_libs_blackhand/result_storages/mongodb_webp_result_storage.py
--rw-rw-r--   0 root         (0) root         (0)     4210 2023-07-24 08:20:38.000000 thumbor_libs_blackhand-0.3.1/thumbor_libs_blackhand/result_storages/mongodb_webp_result_storage_fix.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:30:26.000000 thumbor_libs_blackhand-0.3.1/thumbor_libs_blackhand/storages/
--rw-rw-r--   0 root         (0) root         (0)      138 2023-07-24 08:20:38.000000 thumbor_libs_blackhand-0.3.1/thumbor_libs_blackhand/storages/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4401 2023-07-24 08:20:38.000000 thumbor_libs_blackhand-0.3.1/thumbor_libs_blackhand/storages/mongodb_webp_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:30:26.000000 thumbor_libs_blackhand-0.3.1/thumbor_libs_blackhand/url_signers/
--rw-rw-r--   0 root         (0) root         (0)      138 2023-07-24 08:20:38.000000 thumbor_libs_blackhand-0.3.1/thumbor_libs_blackhand/url_signers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      583 2023-07-24 08:20:38.000000 thumbor_libs_blackhand-0.3.1/thumbor_libs_blackhand/url_signers/base64_hmac_sha1_trim.py
--rw-rw-r--   0 root         (0) root         (0)     1526 2023-07-24 08:20:38.000000 thumbor_libs_blackhand-0.3.1/setup.py
--rw-r--r--   0 root         (0) root         (0)      761 2023-07-24 08:30:26.000000 thumbor_libs_blackhand-0.3.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:12:21.000000 thumbor_libs_blackhand-0.3.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:12:21.000000 thumbor_libs_blackhand-0.3.2/thumbor_libs_blackhand/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:12:21.000000 thumbor_libs_blackhand-0.3.2/thumbor_libs_blackhand/loaders/
+-rw-rw-r--   0 root         (0) root         (0)      138 2023-07-24 15:10:32.000000 thumbor_libs_blackhand-0.3.2/thumbor_libs_blackhand/loaders/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1910 2023-07-24 15:10:32.000000 thumbor_libs_blackhand-0.3.2/thumbor_libs_blackhand/loaders/mongodb_loader.py
+-rw-rw-r--   0 root         (0) root         (0)      533 2023-07-24 15:10:32.000000 thumbor_libs_blackhand-0.3.2/thumbor_libs_blackhand/loaders/spec_http_or_specb_loader.py
+-rw-rw-r--   0 root         (0) root         (0)     2521 2023-07-24 15:10:32.000000 thumbor_libs_blackhand-0.3.2/thumbor_libs_blackhand/loaders/specb_file_fallback_file_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:12:21.000000 thumbor_libs_blackhand-0.3.2/thumbor_libs_blackhand/metrics/
+-rw-rw-r--   0 root         (0) root         (0)      138 2023-07-24 15:10:32.000000 thumbor_libs_blackhand-0.3.2/thumbor_libs_blackhand/metrics/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:12:21.000000 thumbor_libs_blackhand-0.3.2/thumbor_libs_blackhand/mongodb/
+-rw-rw-r--   0 root         (0) root         (0)     1781 2023-07-24 15:10:32.000000 thumbor_libs_blackhand-0.3.2/thumbor_libs_blackhand/mongodb/pool_result_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:12:21.000000 thumbor_libs_blackhand-0.3.2/thumbor_libs_blackhand/result_storages/
+-rw-rw-r--   0 root         (0) root         (0)      138 2023-07-24 15:10:32.000000 thumbor_libs_blackhand-0.3.2/thumbor_libs_blackhand/result_storages/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6672 2023-07-24 15:10:32.000000 thumbor_libs_blackhand-0.3.2/thumbor_libs_blackhand/result_storages/hybrid_result_storage.py
+-rw-rw-r--   0 root         (0) root         (0)     3893 2023-07-24 15:10:32.000000 thumbor_libs_blackhand-0.3.2/thumbor_libs_blackhand/result_storages/mongodb_legacy_result_storage.py
+-rw-rw-r--   0 root         (0) root         (0)     4217 2023-07-24 15:10:32.000000 thumbor_libs_blackhand-0.3.2/thumbor_libs_blackhand/result_storages/mongodb_legacy_result_storage_fix.py
+-rw-rw-r--   0 root         (0) root         (0)     5442 2023-07-24 15:10:32.000000 thumbor_libs_blackhand-0.3.2/thumbor_libs_blackhand/result_storages/mongodb_result_storage.py
+-rw-rw-r--   0 root         (0) root         (0)     6075 2023-07-24 15:10:32.000000 thumbor_libs_blackhand-0.3.2/thumbor_libs_blackhand/result_storages/mongodb_result_storage_v3.py
+-rw-rw-r--   0 root         (0) root         (0)     3889 2023-07-24 15:10:32.000000 thumbor_libs_blackhand-0.3.2/thumbor_libs_blackhand/result_storages/mongodb_webp_result_storage.py
+-rw-rw-r--   0 root         (0) root         (0)     4210 2023-07-24 15:10:32.000000 thumbor_libs_blackhand-0.3.2/thumbor_libs_blackhand/result_storages/mongodb_webp_result_storage_fix.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:12:21.000000 thumbor_libs_blackhand-0.3.2/thumbor_libs_blackhand/storages/
+-rw-rw-r--   0 root         (0) root         (0)      138 2023-07-24 15:10:32.000000 thumbor_libs_blackhand-0.3.2/thumbor_libs_blackhand/storages/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4401 2023-07-24 15:10:32.000000 thumbor_libs_blackhand-0.3.2/thumbor_libs_blackhand/storages/mongodb_webp_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:12:21.000000 thumbor_libs_blackhand-0.3.2/thumbor_libs_blackhand/url_signers/
+-rw-rw-r--   0 root         (0) root         (0)      138 2023-07-24 15:10:32.000000 thumbor_libs_blackhand-0.3.2/thumbor_libs_blackhand/url_signers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      583 2023-07-24 15:10:32.000000 thumbor_libs_blackhand-0.3.2/thumbor_libs_blackhand/url_signers/base64_hmac_sha1_trim.py
+-rw-rw-r--   0 root         (0) root         (0)     1526 2023-07-24 15:10:32.000000 thumbor_libs_blackhand-0.3.2/setup.py
+-rw-r--r--   0 root         (0) root         (0)      761 2023-07-24 15:12:21.000000 thumbor_libs_blackhand-0.3.2/PKG-INFO
```

### Comparing `thumbor_libs_blackhand-0.3.1/thumbor_libs_blackhand/loaders/mongodb_loader.py` & `thumbor_libs_blackhand-0.3.2/thumbor_libs_blackhand/loaders/mongodb_loader.py`

 * *Files identical despite different names*

### Comparing `thumbor_libs_blackhand-0.3.1/thumbor_libs_blackhand/loaders/spec_http_or_specb_loader.py` & `thumbor_libs_blackhand-0.3.2/thumbor_libs_blackhand/loaders/spec_http_or_specb_loader.py`

 * *Files identical despite different names*

### Comparing `thumbor_libs_blackhand-0.3.1/thumbor_libs_blackhand/loaders/specb_file_fallback_file_loader.py` & `thumbor_libs_blackhand-0.3.2/thumbor_libs_blackhand/loaders/specb_file_fallback_file_loader.py`

 * *Files identical despite different names*

### Comparing `thumbor_libs_blackhand-0.3.1/thumbor_libs_blackhand/mongodb/pool_result_storage.py` & `thumbor_libs_blackhand-0.3.2/thumbor_libs_blackhand/mongodb/pool_result_storage.py`

 * *Files identical despite different names*

### Comparing `thumbor_libs_blackhand-0.3.1/thumbor_libs_blackhand/result_storages/hybrid_result_storage.py` & `thumbor_libs_blackhand-0.3.2/thumbor_libs_blackhand/result_storages/hybrid_result_storage.py`

 * *Files identical despite different names*

### Comparing `thumbor_libs_blackhand-0.3.1/thumbor_libs_blackhand/result_storages/mongodb_legacy_result_storage.py` & `thumbor_libs_blackhand-0.3.2/thumbor_libs_blackhand/result_storages/mongodb_legacy_result_storage.py`

 * *Files identical despite different names*

### Comparing `thumbor_libs_blackhand-0.3.1/thumbor_libs_blackhand/result_storages/mongodb_legacy_result_storage_fix.py` & `thumbor_libs_blackhand-0.3.2/thumbor_libs_blackhand/result_storages/mongodb_legacy_result_storage_fix.py`

 * *Files identical despite different names*

### Comparing `thumbor_libs_blackhand-0.3.1/thumbor_libs_blackhand/result_storages/mongodb_result_storage.py` & `thumbor_libs_blackhand-0.3.2/thumbor_libs_blackhand/result_storages/mongodb_result_storage.py`

 * *Files identical despite different names*

### Comparing `thumbor_libs_blackhand-0.3.1/thumbor_libs_blackhand/result_storages/mongodb_result_storage_v3.py` & `thumbor_libs_blackhand-0.3.2/thumbor_libs_blackhand/result_storages/mongodb_result_storage_v3.py`

 * *Files 3% similar despite different names*

```diff
@@ -155,23 +155,32 @@
             'content_length': True,
         })
 
 
         if not stored:
             return None
         
-        filter={
+        try:
+            #self.context.config.MONGO_RESULT_STORAGE_MAXCACHESIZE
+            dedup = self.context.config.MONGO_RESULT_STORAGE_DEDUP
+        except:
+            dedup = False
+        
+        if not dedup:
+          logger.debug("Deduplication OFF")  
+        else:
+          filter={
             'path': key
-        }
-        sort=list({
+          }
+          sort=list({
             'created_at': -1
-        }.items())
-        skip=1
-        obj = self.storage.find(filter=filter, skip=skip)
-        async for doc in obj:
+          }.items())
+          skip=1
+          obj = self.storage.find(filter=filter, skip=skip)
+          async for doc in obj:
             logger.info("Deduplication %s", key)
             self.storage.delete_one({"_id": doc["_id"]})
 
 
         metadata = stored['metadata']
         metadata['LastModified'] = stored['created_at'].replace(
             tzinfo=pytz.utc
```

### Comparing `thumbor_libs_blackhand-0.3.1/thumbor_libs_blackhand/result_storages/mongodb_webp_result_storage.py` & `thumbor_libs_blackhand-0.3.2/thumbor_libs_blackhand/result_storages/mongodb_webp_result_storage.py`

 * *Files identical despite different names*

### Comparing `thumbor_libs_blackhand-0.3.1/thumbor_libs_blackhand/result_storages/mongodb_webp_result_storage_fix.py` & `thumbor_libs_blackhand-0.3.2/thumbor_libs_blackhand/result_storages/mongodb_webp_result_storage_fix.py`

 * *Files identical despite different names*

### Comparing `thumbor_libs_blackhand-0.3.1/thumbor_libs_blackhand/storages/mongodb_webp_storage.py` & `thumbor_libs_blackhand-0.3.2/thumbor_libs_blackhand/storages/mongodb_webp_storage.py`

 * *Files identical despite different names*

### Comparing `thumbor_libs_blackhand-0.3.1/thumbor_libs_blackhand/url_signers/base64_hmac_sha1_trim.py` & `thumbor_libs_blackhand-0.3.2/thumbor_libs_blackhand/url_signers/base64_hmac_sha1_trim.py`

 * *Files identical despite different names*

### Comparing `thumbor_libs_blackhand-0.3.1/setup.py` & `thumbor_libs_blackhand-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # http://www.opensource.org/licenses/mit-license
 
 
 from distutils.core import setup
 
 setup(
     name = "thumbor_libs_blackhand",
-    version = "0.3.1",
+    version = "0.3.2",
     description = "libs thumbor",
     author = "Bertrand Thill",
     author_email = "github@blackhand.org",
     keywords = ["thumbor", "fallback", "images", "nfs", "mongodb"],
     license = 'GNU',
     url = 'https://github.com/Bkhand/thumbor_libs_blackhand',
     packages=[
```

### Comparing `thumbor_libs_blackhand-0.3.1/PKG-INFO` & `thumbor_libs_blackhand-0.3.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: thumbor_libs_blackhand
-Version: 0.3.1
+Version: 0.3.2
 Summary: libs thumbor
 Home-page: https://github.com/Bkhand/thumbor_libs_blackhand
 Author: Bertrand Thill
 Author-email: github@blackhand.org
 License: GNU
 Description: This module enable mongodb support and fallback for thumbor.
```

