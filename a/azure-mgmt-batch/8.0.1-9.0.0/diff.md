# Comparing `tmp/azure-mgmt-batch-8.0.1.zip` & `tmp/azure-mgmt-batch-9.0.0.zip`

## zipinfo {}

```diff
@@ -1,54 +1,55 @@
-Zip file size: 124503 bytes, number of entries: 52
-drwxr-xr-x  2.0 unx        0 b- stor 20-May-26 18:56 azure-mgmt-batch-8.0.1/
-drwxr-xr-x  2.0 unx        0 b- stor 20-May-26 18:56 azure-mgmt-batch-8.0.1/azure_mgmt_batch.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 20-May-26 18:56 azure-mgmt-batch-8.0.1/azure/
-drwxr-xr-x  2.0 unx        0 b- stor 20-May-26 18:56 azure-mgmt-batch-8.0.1/tests/
--rw-r--r--  2.0 unx      107 b- defN 20-May-26 18:55 azure-mgmt-batch-8.0.1/MANIFEST.in
--rw-r--r--  2.0 unx     2894 b- defN 20-May-26 18:55 azure-mgmt-batch-8.0.1/setup.py
--rw-r--r--  2.0 unx       67 b- defN 20-May-26 18:56 azure-mgmt-batch-8.0.1/setup.cfg
--rw-r--r--  2.0 unx     6851 b- defN 20-May-26 18:55 azure-mgmt-batch-8.0.1/CHANGELOG.md
--rw-r--r--  2.0 unx    10192 b- defN 20-May-26 18:56 azure-mgmt-batch-8.0.1/PKG-INFO
--rw-r--r--  2.0 unx     1015 b- defN 20-May-26 18:55 azure-mgmt-batch-8.0.1/README.md
--rw-r--r--  2.0 unx     1815 b- defN 20-May-26 18:56 azure-mgmt-batch-8.0.1/azure_mgmt_batch.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx        1 b- defN 20-May-26 18:56 azure-mgmt-batch-8.0.1/azure_mgmt_batch.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx        6 b- defN 20-May-26 18:56 azure-mgmt-batch-8.0.1/azure_mgmt_batch.egg-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 20-May-26 18:56 azure-mgmt-batch-8.0.1/azure_mgmt_batch.egg-info/not-zip-safe
--rw-r--r--  2.0 unx      101 b- defN 20-May-26 18:56 azure-mgmt-batch-8.0.1/azure_mgmt_batch.egg-info/requires.txt
--rw-r--r--  2.0 unx    10192 b- defN 20-May-26 18:56 azure-mgmt-batch-8.0.1/azure_mgmt_batch.egg-info/PKG-INFO
-drwxr-xr-x  2.0 unx        0 b- stor 20-May-26 18:56 azure-mgmt-batch-8.0.1/azure/mgmt/
--rw-r--r--  2.0 unx       65 b- defN 20-May-26 18:55 azure-mgmt-batch-8.0.1/azure/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 20-May-26 18:56 azure-mgmt-batch-8.0.1/azure/mgmt/batch/
--rw-r--r--  2.0 unx       65 b- defN 20-May-26 18:55 azure-mgmt-batch-8.0.1/azure/mgmt/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 20-May-26 18:56 azure-mgmt-batch-8.0.1/azure/mgmt/batch/models/
-drwxr-xr-x  2.0 unx        0 b- stor 20-May-26 18:56 azure-mgmt-batch-8.0.1/azure/mgmt/batch/operations/
--rw-r--r--  2.0 unx     1932 b- defN 20-May-26 18:55 azure-mgmt-batch-8.0.1/azure/mgmt/batch/_configuration.py
--rw-r--r--  2.0 unx     4485 b- defN 20-May-26 18:55 azure-mgmt-batch-8.0.1/azure/mgmt/batch/_batch_management_client.py
--rw-r--r--  2.0 unx      725 b- defN 20-May-26 18:55 azure-mgmt-batch-8.0.1/azure/mgmt/batch/__init__.py
--rw-r--r--  2.0 unx      493 b- defN 20-May-26 18:55 azure-mgmt-batch-8.0.1/azure/mgmt/batch/version.py
--rw-r--r--  2.0 unx   127744 b- defN 20-May-26 18:55 azure-mgmt-batch-8.0.1/azure/mgmt/batch/models/_models_py3.py
--rw-r--r--  2.0 unx   126694 b- defN 20-May-26 18:55 azure-mgmt-batch-8.0.1/azure/mgmt/batch/models/_models.py
--rw-r--r--  2.0 unx    11340 b- defN 20-May-26 18:55 azure-mgmt-batch-8.0.1/azure/mgmt/batch/models/__init__.py
--rw-r--r--  2.0 unx     4027 b- defN 20-May-26 18:55 azure-mgmt-batch-8.0.1/azure/mgmt/batch/models/_paged_models.py
--rw-r--r--  2.0 unx    10581 b- defN 20-May-26 18:55 azure-mgmt-batch-8.0.1/azure/mgmt/batch/models/_batch_management_client_enums.py
--rw-r--r--  2.0 unx    34194 b- defN 20-May-26 18:55 azure-mgmt-batch-8.0.1/azure/mgmt/batch/operations/_batch_account_operations.py
--rw-r--r--  2.0 unx     8742 b- defN 20-May-26 18:55 azure-mgmt-batch-8.0.1/azure/mgmt/batch/operations/_private_link_resource_operations.py
--rw-r--r--  2.0 unx    21093 b- defN 20-May-26 18:55 azure-mgmt-batch-8.0.1/azure/mgmt/batch/operations/_application_package_operations.py
--rw-r--r--  2.0 unx    19052 b- defN 20-May-26 18:55 azure-mgmt-batch-8.0.1/azure/mgmt/batch/operations/_application_operations.py
--rw-r--r--  2.0 unx    32264 b- defN 20-May-26 18:55 azure-mgmt-batch-8.0.1/azure/mgmt/batch/operations/_pool_operations.py
--rw-r--r--  2.0 unx     1313 b- defN 20-May-26 18:55 azure-mgmt-batch-8.0.1/azure/mgmt/batch/operations/__init__.py
--rw-r--r--  2.0 unx     7358 b- defN 20-May-26 18:55 azure-mgmt-batch-8.0.1/azure/mgmt/batch/operations/_location_operations.py
--rw-r--r--  2.0 unx    15957 b- defN 20-May-26 18:55 azure-mgmt-batch-8.0.1/azure/mgmt/batch/operations/_private_endpoint_connection_operations.py
--rw-r--r--  2.0 unx    29742 b- defN 20-May-26 18:55 azure-mgmt-batch-8.0.1/azure/mgmt/batch/operations/_certificate_operations.py
--rw-r--r--  2.0 unx     3926 b- defN 20-May-26 18:55 azure-mgmt-batch-8.0.1/azure/mgmt/batch/operations/_operations.py
-drwxr-xr-x  2.0 unx        0 b- stor 20-May-26 18:56 azure-mgmt-batch-8.0.1/tests/recordings/
--rw-r--r--  2.0 unx     5786 b- defN 20-May-26 18:55 azure-mgmt-batch-8.0.1/tests/mgmt_batch_preparers.py
--rw-r--r--  2.0 unx    23227 b- defN 20-May-26 18:55 azure-mgmt-batch-8.0.1/tests/test_mgmt_batch.py
--rw-r--r--  2.0 unx    29041 b- defN 20-May-26 18:55 azure-mgmt-batch-8.0.1/tests/recordings/test_mgmt_batch.test_mgmt_batch_list_operations.yaml
--rw-r--r--  2.0 unx     8048 b- defN 20-May-26 18:55 azure-mgmt-batch-8.0.1/tests/recordings/test_mgmt_batch.test_mgmt_batch_byos_account.yaml
--rw-r--r--  2.0 unx    20673 b- defN 20-May-26 18:55 azure-mgmt-batch-8.0.1/tests/recordings/test_mgmt_batch.test_mgmt_batch_account.yaml
--rw-r--r--  2.0 unx    26281 b- defN 20-May-26 18:55 azure-mgmt-batch-8.0.1/tests/recordings/test_mgmt_batch.test_mgmt_batch_applications.yaml
--rw-r--r--  2.0 unx    23392 b- defN 20-May-26 18:55 azure-mgmt-batch-8.0.1/tests/recordings/test_mgmt_batch.test_mgmt_batch_pools.yaml
--rw-r--r--  2.0 unx     1166 b- defN 20-May-26 18:55 azure-mgmt-batch-8.0.1/tests/recordings/test_mgmt_batch.test_mgmt_batch_subscription_quota.yaml
--rw-r--r--  2.0 unx    25947 b- defN 20-May-26 18:55 azure-mgmt-batch-8.0.1/tests/recordings/test_mgmt_batch.test_mgmt_batch_certificates.yaml
--rw-r--r--  2.0 unx     4408 b- defN 20-May-26 18:55 azure-mgmt-batch-8.0.1/tests/recordings/test_mgmt_batch.test_mgmt_batch_account_name.yaml
-52 files, 663003 bytes uncompressed, 114303 bytes compressed:  82.8%
+Zip file size: 131347 bytes, number of entries: 53
+drwxr-xr-x  2.0 unx        0 b- stor 20-Jun-01 20:18 azure-mgmt-batch-9.0.0/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Jun-01 20:18 azure-mgmt-batch-9.0.0/azure_mgmt_batch.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Jun-01 20:18 azure-mgmt-batch-9.0.0/azure/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Jun-01 20:18 azure-mgmt-batch-9.0.0/tests/
+-rw-r--r--  2.0 unx      107 b- defN 20-Jun-01 20:17 azure-mgmt-batch-9.0.0/MANIFEST.in
+-rw-r--r--  2.0 unx     2894 b- defN 20-Jun-01 20:17 azure-mgmt-batch-9.0.0/setup.py
+-rw-r--r--  2.0 unx       67 b- defN 20-Jun-01 20:18 azure-mgmt-batch-9.0.0/setup.cfg
+-rw-r--r--  2.0 unx     9124 b- defN 20-Jun-01 20:17 azure-mgmt-batch-9.0.0/CHANGELOG.md
+-rw-r--r--  2.0 unx    12649 b- defN 20-Jun-01 20:18 azure-mgmt-batch-9.0.0/PKG-INFO
+-rw-r--r--  2.0 unx     1015 b- defN 20-Jun-01 20:18 azure-mgmt-batch-9.0.0/README.md
+-rw-r--r--  2.0 unx     1886 b- defN 20-Jun-01 20:18 azure-mgmt-batch-9.0.0/azure_mgmt_batch.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx        1 b- defN 20-Jun-01 20:18 azure-mgmt-batch-9.0.0/azure_mgmt_batch.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx        6 b- defN 20-Jun-01 20:18 azure-mgmt-batch-9.0.0/azure_mgmt_batch.egg-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 20-Jun-01 20:18 azure-mgmt-batch-9.0.0/azure_mgmt_batch.egg-info/not-zip-safe
+-rw-r--r--  2.0 unx      101 b- defN 20-Jun-01 20:18 azure-mgmt-batch-9.0.0/azure_mgmt_batch.egg-info/requires.txt
+-rw-r--r--  2.0 unx    12649 b- defN 20-Jun-01 20:18 azure-mgmt-batch-9.0.0/azure_mgmt_batch.egg-info/PKG-INFO
+drwxr-xr-x  2.0 unx        0 b- stor 20-Jun-01 20:18 azure-mgmt-batch-9.0.0/azure/mgmt/
+-rw-r--r--  2.0 unx       65 b- defN 20-Jun-01 20:17 azure-mgmt-batch-9.0.0/azure/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 20-Jun-01 20:18 azure-mgmt-batch-9.0.0/azure/mgmt/batch/
+-rw-r--r--  2.0 unx       65 b- defN 20-Jun-01 20:17 azure-mgmt-batch-9.0.0/azure/mgmt/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 20-Jun-01 20:18 azure-mgmt-batch-9.0.0/azure/mgmt/batch/models/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Jun-01 20:18 azure-mgmt-batch-9.0.0/azure/mgmt/batch/operations/
+-rw-r--r--  2.0 unx     1932 b- defN 20-Jun-01 20:17 azure-mgmt-batch-9.0.0/azure/mgmt/batch/_configuration.py
+-rw-r--r--  2.0 unx     4485 b- defN 20-Jun-01 20:17 azure-mgmt-batch-9.0.0/azure/mgmt/batch/_batch_management_client.py
+-rw-r--r--  2.0 unx      725 b- defN 20-Jun-01 20:17 azure-mgmt-batch-9.0.0/azure/mgmt/batch/__init__.py
+-rw-r--r--  2.0 unx      493 b- defN 20-Jun-01 20:17 azure-mgmt-batch-9.0.0/azure/mgmt/batch/version.py
+-rw-r--r--  2.0 unx   131146 b- defN 20-Jun-01 20:17 azure-mgmt-batch-9.0.0/azure/mgmt/batch/models/_models_py3.py
+-rw-r--r--  2.0 unx   130111 b- defN 20-Jun-01 20:17 azure-mgmt-batch-9.0.0/azure/mgmt/batch/models/_models.py
+-rw-r--r--  2.0 unx    11518 b- defN 20-Jun-01 20:17 azure-mgmt-batch-9.0.0/azure/mgmt/batch/models/__init__.py
+-rw-r--r--  2.0 unx     4027 b- defN 20-Jun-01 20:17 azure-mgmt-batch-9.0.0/azure/mgmt/batch/models/_paged_models.py
+-rw-r--r--  2.0 unx    11016 b- defN 20-Jun-01 20:17 azure-mgmt-batch-9.0.0/azure/mgmt/batch/models/_batch_management_client_enums.py
+-rw-r--r--  2.0 unx    33960 b- defN 20-Jun-01 20:17 azure-mgmt-batch-9.0.0/azure/mgmt/batch/operations/_batch_account_operations.py
+-rw-r--r--  2.0 unx     8742 b- defN 20-Jun-01 20:17 azure-mgmt-batch-9.0.0/azure/mgmt/batch/operations/_private_link_resource_operations.py
+-rw-r--r--  2.0 unx    21093 b- defN 20-Jun-01 20:17 azure-mgmt-batch-9.0.0/azure/mgmt/batch/operations/_application_package_operations.py
+-rw-r--r--  2.0 unx    19052 b- defN 20-Jun-01 20:17 azure-mgmt-batch-9.0.0/azure/mgmt/batch/operations/_application_operations.py
+-rw-r--r--  2.0 unx    32264 b- defN 20-Jun-01 20:17 azure-mgmt-batch-9.0.0/azure/mgmt/batch/operations/_pool_operations.py
+-rw-r--r--  2.0 unx     1313 b- defN 20-Jun-01 20:17 azure-mgmt-batch-9.0.0/azure/mgmt/batch/operations/__init__.py
+-rw-r--r--  2.0 unx     7358 b- defN 20-Jun-01 20:17 azure-mgmt-batch-9.0.0/azure/mgmt/batch/operations/_location_operations.py
+-rw-r--r--  2.0 unx    15957 b- defN 20-Jun-01 20:17 azure-mgmt-batch-9.0.0/azure/mgmt/batch/operations/_private_endpoint_connection_operations.py
+-rw-r--r--  2.0 unx    29742 b- defN 20-Jun-01 20:17 azure-mgmt-batch-9.0.0/azure/mgmt/batch/operations/_certificate_operations.py
+-rw-r--r--  2.0 unx     3926 b- defN 20-Jun-01 20:17 azure-mgmt-batch-9.0.0/azure/mgmt/batch/operations/_operations.py
+drwxr-xr-x  2.0 unx        0 b- stor 20-Jun-01 20:18 azure-mgmt-batch-9.0.0/tests/recordings/
+-rw-r--r--  2.0 unx     5786 b- defN 20-Jun-01 20:17 azure-mgmt-batch-9.0.0/tests/mgmt_batch_preparers.py
+-rw-r--r--  2.0 unx    27068 b- defN 20-Jun-01 20:17 azure-mgmt-batch-9.0.0/tests/test_mgmt_batch.py
+-rw-r--r--  2.0 unx    29782 b- defN 20-Jun-01 20:17 azure-mgmt-batch-9.0.0/tests/recordings/test_mgmt_batch.test_mgmt_batch_list_operations.yaml
+-rw-r--r--  2.0 unx     8064 b- defN 20-Jun-01 20:17 azure-mgmt-batch-9.0.0/tests/recordings/test_mgmt_batch.test_mgmt_batch_byos_account.yaml
+-rw-r--r--  2.0 unx    21574 b- defN 20-Jun-01 20:17 azure-mgmt-batch-9.0.0/tests/recordings/test_mgmt_batch.test_mgmt_batch_account.yaml
+-rw-r--r--  2.0 unx    26380 b- defN 20-Jun-01 20:17 azure-mgmt-batch-9.0.0/tests/recordings/test_mgmt_batch.test_mgmt_batch_applications.yaml
+-rw-r--r--  2.0 unx    35486 b- defN 20-Jun-01 20:17 azure-mgmt-batch-9.0.0/tests/recordings/test_mgmt_batch.test_mgmt_batch_account_advanced.yaml
+-rw-r--r--  2.0 unx    23692 b- defN 20-Jun-01 20:17 azure-mgmt-batch-9.0.0/tests/recordings/test_mgmt_batch.test_mgmt_batch_pools.yaml
+-rw-r--r--  2.0 unx     1163 b- defN 20-Jun-01 20:17 azure-mgmt-batch-9.0.0/tests/recordings/test_mgmt_batch.test_mgmt_batch_subscription_quota.yaml
+-rw-r--r--  2.0 unx    29650 b- defN 20-Jun-01 20:17 azure-mgmt-batch-9.0.0/tests/recordings/test_mgmt_batch.test_mgmt_batch_certificates.yaml
+-rw-r--r--  2.0 unx     4396 b- defN 20-Jun-01 20:17 azure-mgmt-batch-9.0.0/tests/recordings/test_mgmt_batch.test_mgmt_batch_account_name.yaml
+53 files, 722531 bytes uncompressed, 120885 bytes compressed:  83.3%
```

## zipnote {}

```diff
@@ -1,157 +1,160 @@
-Filename: azure-mgmt-batch-8.0.1/
+Filename: azure-mgmt-batch-9.0.0/
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/azure_mgmt_batch.egg-info/
+Filename: azure-mgmt-batch-9.0.0/azure_mgmt_batch.egg-info/
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/azure/
+Filename: azure-mgmt-batch-9.0.0/azure/
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/tests/
+Filename: azure-mgmt-batch-9.0.0/tests/
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/MANIFEST.in
+Filename: azure-mgmt-batch-9.0.0/MANIFEST.in
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/setup.py
+Filename: azure-mgmt-batch-9.0.0/setup.py
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/setup.cfg
+Filename: azure-mgmt-batch-9.0.0/setup.cfg
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/CHANGELOG.md
+Filename: azure-mgmt-batch-9.0.0/CHANGELOG.md
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/PKG-INFO
+Filename: azure-mgmt-batch-9.0.0/PKG-INFO
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/README.md
+Filename: azure-mgmt-batch-9.0.0/README.md
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/azure_mgmt_batch.egg-info/SOURCES.txt
+Filename: azure-mgmt-batch-9.0.0/azure_mgmt_batch.egg-info/SOURCES.txt
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/azure_mgmt_batch.egg-info/dependency_links.txt
+Filename: azure-mgmt-batch-9.0.0/azure_mgmt_batch.egg-info/dependency_links.txt
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/azure_mgmt_batch.egg-info/top_level.txt
+Filename: azure-mgmt-batch-9.0.0/azure_mgmt_batch.egg-info/top_level.txt
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/azure_mgmt_batch.egg-info/not-zip-safe
+Filename: azure-mgmt-batch-9.0.0/azure_mgmt_batch.egg-info/not-zip-safe
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/azure_mgmt_batch.egg-info/requires.txt
+Filename: azure-mgmt-batch-9.0.0/azure_mgmt_batch.egg-info/requires.txt
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/azure_mgmt_batch.egg-info/PKG-INFO
+Filename: azure-mgmt-batch-9.0.0/azure_mgmt_batch.egg-info/PKG-INFO
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/azure/mgmt/
+Filename: azure-mgmt-batch-9.0.0/azure/mgmt/
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/azure/__init__.py
+Filename: azure-mgmt-batch-9.0.0/azure/__init__.py
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/azure/mgmt/batch/
+Filename: azure-mgmt-batch-9.0.0/azure/mgmt/batch/
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/azure/mgmt/__init__.py
+Filename: azure-mgmt-batch-9.0.0/azure/mgmt/__init__.py
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/azure/mgmt/batch/models/
+Filename: azure-mgmt-batch-9.0.0/azure/mgmt/batch/models/
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/azure/mgmt/batch/operations/
+Filename: azure-mgmt-batch-9.0.0/azure/mgmt/batch/operations/
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/azure/mgmt/batch/_configuration.py
+Filename: azure-mgmt-batch-9.0.0/azure/mgmt/batch/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/azure/mgmt/batch/_batch_management_client.py
+Filename: azure-mgmt-batch-9.0.0/azure/mgmt/batch/_batch_management_client.py
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/azure/mgmt/batch/__init__.py
+Filename: azure-mgmt-batch-9.0.0/azure/mgmt/batch/__init__.py
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/azure/mgmt/batch/version.py
+Filename: azure-mgmt-batch-9.0.0/azure/mgmt/batch/version.py
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/azure/mgmt/batch/models/_models_py3.py
+Filename: azure-mgmt-batch-9.0.0/azure/mgmt/batch/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/azure/mgmt/batch/models/_models.py
+Filename: azure-mgmt-batch-9.0.0/azure/mgmt/batch/models/_models.py
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/azure/mgmt/batch/models/__init__.py
+Filename: azure-mgmt-batch-9.0.0/azure/mgmt/batch/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/azure/mgmt/batch/models/_paged_models.py
+Filename: azure-mgmt-batch-9.0.0/azure/mgmt/batch/models/_paged_models.py
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/azure/mgmt/batch/models/_batch_management_client_enums.py
+Filename: azure-mgmt-batch-9.0.0/azure/mgmt/batch/models/_batch_management_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/azure/mgmt/batch/operations/_batch_account_operations.py
+Filename: azure-mgmt-batch-9.0.0/azure/mgmt/batch/operations/_batch_account_operations.py
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/azure/mgmt/batch/operations/_private_link_resource_operations.py
+Filename: azure-mgmt-batch-9.0.0/azure/mgmt/batch/operations/_private_link_resource_operations.py
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/azure/mgmt/batch/operations/_application_package_operations.py
+Filename: azure-mgmt-batch-9.0.0/azure/mgmt/batch/operations/_application_package_operations.py
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/azure/mgmt/batch/operations/_application_operations.py
+Filename: azure-mgmt-batch-9.0.0/azure/mgmt/batch/operations/_application_operations.py
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/azure/mgmt/batch/operations/_pool_operations.py
+Filename: azure-mgmt-batch-9.0.0/azure/mgmt/batch/operations/_pool_operations.py
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/azure/mgmt/batch/operations/__init__.py
+Filename: azure-mgmt-batch-9.0.0/azure/mgmt/batch/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/azure/mgmt/batch/operations/_location_operations.py
+Filename: azure-mgmt-batch-9.0.0/azure/mgmt/batch/operations/_location_operations.py
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/azure/mgmt/batch/operations/_private_endpoint_connection_operations.py
+Filename: azure-mgmt-batch-9.0.0/azure/mgmt/batch/operations/_private_endpoint_connection_operations.py
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/azure/mgmt/batch/operations/_certificate_operations.py
+Filename: azure-mgmt-batch-9.0.0/azure/mgmt/batch/operations/_certificate_operations.py
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/azure/mgmt/batch/operations/_operations.py
+Filename: azure-mgmt-batch-9.0.0/azure/mgmt/batch/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/tests/recordings/
+Filename: azure-mgmt-batch-9.0.0/tests/recordings/
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/tests/mgmt_batch_preparers.py
+Filename: azure-mgmt-batch-9.0.0/tests/mgmt_batch_preparers.py
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/tests/test_mgmt_batch.py
+Filename: azure-mgmt-batch-9.0.0/tests/test_mgmt_batch.py
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/tests/recordings/test_mgmt_batch.test_mgmt_batch_list_operations.yaml
+Filename: azure-mgmt-batch-9.0.0/tests/recordings/test_mgmt_batch.test_mgmt_batch_list_operations.yaml
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/tests/recordings/test_mgmt_batch.test_mgmt_batch_byos_account.yaml
+Filename: azure-mgmt-batch-9.0.0/tests/recordings/test_mgmt_batch.test_mgmt_batch_byos_account.yaml
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/tests/recordings/test_mgmt_batch.test_mgmt_batch_account.yaml
+Filename: azure-mgmt-batch-9.0.0/tests/recordings/test_mgmt_batch.test_mgmt_batch_account.yaml
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/tests/recordings/test_mgmt_batch.test_mgmt_batch_applications.yaml
+Filename: azure-mgmt-batch-9.0.0/tests/recordings/test_mgmt_batch.test_mgmt_batch_applications.yaml
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/tests/recordings/test_mgmt_batch.test_mgmt_batch_pools.yaml
+Filename: azure-mgmt-batch-9.0.0/tests/recordings/test_mgmt_batch.test_mgmt_batch_account_advanced.yaml
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/tests/recordings/test_mgmt_batch.test_mgmt_batch_subscription_quota.yaml
+Filename: azure-mgmt-batch-9.0.0/tests/recordings/test_mgmt_batch.test_mgmt_batch_pools.yaml
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/tests/recordings/test_mgmt_batch.test_mgmt_batch_certificates.yaml
+Filename: azure-mgmt-batch-9.0.0/tests/recordings/test_mgmt_batch.test_mgmt_batch_subscription_quota.yaml
 Comment: 
 
-Filename: azure-mgmt-batch-8.0.1/tests/recordings/test_mgmt_batch.test_mgmt_batch_account_name.yaml
+Filename: azure-mgmt-batch-9.0.0/tests/recordings/test_mgmt_batch.test_mgmt_batch_certificates.yaml
+Comment: 
+
+Filename: azure-mgmt-batch-9.0.0/tests/recordings/test_mgmt_batch.test_mgmt_batch_account_name.yaml
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-mgmt-batch-8.0.1/setup.py` & `azure-mgmt-batch-9.0.0/setup.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-batch-8.0.1/CHANGELOG.md` & `azure-mgmt-batch-9.0.0/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,37 @@
 # Release History
+## 9.0.0 (2020-05-29)
+### REST API version
+- This version targets REST API version 2020-05-01.
+
+### Features
+- Added ability to access the Batch DataPlane API without needing a public DNS entry for the account via the new `public_network_access` property on `BatchAccount`.
+- Added new `PrivateLinkResource` and `PrivateEndpointConnection` resource types. These are both only used when the `public_network_access` property on `BatchAccount` is set to `Disabled`.
+  - When `public_network_access` is set to `Disabled` a new `PrivateLinkResource` is visible in that account, which can be used to connect to the account using an ARM Private Endpoint in your VNET.
+- Added ability to encrypt `ComputeNode` disk drives using the new `disk_encryption_configuration` property of `VirtualMachineConfiguration`.
+- **[Breaking]** The `id` property of `ImageReference` can now only refer to a Shared Image Gallery image.
+- **[Breaking]** Pools can now be provisioned without a public IP using the new `public_ip_configuration` property of `NetworkConfiguration`.
+  - The `public_ips` property of `NetworkConfiguration` has moved in to `PublicIPAddressConfiguration` as well. This property can only be specified if `IPAddressProvisioningType` is `UserManaged`.
+- Adds a new property `identity` of type `BatchAccountIdentity` to `BatchAccount`. This can be used to configure how customer data is encrypted inside the Batch account.
+    - This new property is configurable at  the account level on create and update through a new `identity` property on `BatchAccountCreateParameters` and `BatchAccountUpdateParameters`
+
+### Fixes
+- [Breaking] Move tags from being an argument on create and update pool parameters to being a part of `BatchAccountCreateParameters` and `BatchAccountUpdateParameters` to properly reflect the REST API
+
+## 8.0.1 (2020-05-26) [Deprecated]
+### Notices
+- This version targeted an invalid REST API. This version does not honor the associated REST API contract.
 
-## 8.0.1 (2020-05-26)
 ### Bugfixes
-- Fix issues in PrivateEndpointConnection get and update methods due to mistakes in the Swagger specification causing validation to fail.
+- Fix issues in PrivateEndpointConnection get and update methods due to mistakes in the Swagger specification causing validation to fail. It is advised to use version 9+ to make use of the features added in this version.
+
+## 8.0.0 (2020-04-10) [Deprecated]
+### Notices
+- This version targeted an invalid REST API. Currently the PrivateEndpoint get() and update() functions do not function correctly. It is advised to use version 9+ to make use of the features added in this version.
 
-## 8.0.0 (2020-04-10)
 ### REST API version
 - This version targets REST API version 2020-03-01.
 
 ### Features
 - Added ability to access the Batch DataPlane API without needing a public DNS entry for the account via the new `public_network_access` property on `BatchAccount`.
 - Added new `PrivateLinkResource` and `PrivateEndpointConnection` resource types. These are both only used when the `public_network_access` property on `BatchAccount` is set to `Disabled`.
   - When `public_network_access` is set to `Disabled` a new `PrivateLinkResource` is visible in that account, which can be used to connect to the account using an ARM Private Endpoint in your VNET.
```

## Comparing `azure-mgmt-batch-8.0.1/PKG-INFO` & `azure-mgmt-batch-9.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-batch
-Version: 8.0.1
+Version: 9.0.0
 Summary: Microsoft Azure Batch Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Description: ## Microsoft Azure SDK for Python
         
@@ -33,20 +33,43 @@
         If you encounter any bugs or have suggestions, please file an issue in
         the [Issues](https://github.com/Azure/azure-sdk-for-python/issues)
         section of the project.
         
         ![image](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-batch%2FREADME.png)
         
         # Release History
+        ## 9.0.0 (2020-05-29)
+        ### REST API version
+        - This version targets REST API version 2020-05-01.
+        
+        ### Features
+        - Added ability to access the Batch DataPlane API without needing a public DNS entry for the account via the new `public_network_access` property on `BatchAccount`.
+        - Added new `PrivateLinkResource` and `PrivateEndpointConnection` resource types. These are both only used when the `public_network_access` property on `BatchAccount` is set to `Disabled`.
+          - When `public_network_access` is set to `Disabled` a new `PrivateLinkResource` is visible in that account, which can be used to connect to the account using an ARM Private Endpoint in your VNET.
+        - Added ability to encrypt `ComputeNode` disk drives using the new `disk_encryption_configuration` property of `VirtualMachineConfiguration`.
+        - **[Breaking]** The `id` property of `ImageReference` can now only refer to a Shared Image Gallery image.
+        - **[Breaking]** Pools can now be provisioned without a public IP using the new `public_ip_configuration` property of `NetworkConfiguration`.
+          - The `public_ips` property of `NetworkConfiguration` has moved in to `PublicIPAddressConfiguration` as well. This property can only be specified if `IPAddressProvisioningType` is `UserManaged`.
+        - Adds a new property `identity` of type `BatchAccountIdentity` to `BatchAccount`. This can be used to configure how customer data is encrypted inside the Batch account.
+            - This new property is configurable at  the account level on create and update through a new `identity` property on `BatchAccountCreateParameters` and `BatchAccountUpdateParameters`
+        
+        ### Fixes
+        - [Breaking] Move tags from being an argument on create and update pool parameters to being a part of `BatchAccountCreateParameters` and `BatchAccountUpdateParameters` to properly reflect the REST API
+        
+        ## 8.0.1 (2020-05-26) [Deprecated]
+        ### Notices
+        - This version targeted an invalid REST API. This version does not honor the associated REST API contract.
         
-        ## 8.0.1 (2020-05-26)
         ### Bugfixes
-        - Fix issues in PrivateEndpointConnection get and update methods due to mistakes in the Swagger specification causing validation to fail.
+        - Fix issues in PrivateEndpointConnection get and update methods due to mistakes in the Swagger specification causing validation to fail. It is advised to use version 9+ to make use of the features added in this version.
+        
+        ## 8.0.0 (2020-04-10) [Deprecated]
+        ### Notices
+        - This version targeted an invalid REST API. Currently the PrivateEndpoint get() and update() functions do not function correctly. It is advised to use version 9+ to make use of the features added in this version.
         
-        ## 8.0.0 (2020-04-10)
         ### REST API version
         - This version targets REST API version 2020-03-01.
         
         ### Features
         - Added ability to access the Batch DataPlane API without needing a public DNS entry for the account via the new `public_network_access` property on `BatchAccount`.
         - Added new `PrivateLinkResource` and `PrivateEndpointConnection` resource types. These are both only used when the `public_network_access` property on `BatchAccount` is set to `Disabled`.
           - When `public_network_access` is set to `Disabled` a new `PrivateLinkResource` is visible in that account, which can be used to connect to the account using an ARM Private Endpoint in your VNET.
```

## Comparing `azure-mgmt-batch-8.0.1/README.md` & `azure-mgmt-batch-9.0.0/README.md`

 * *Files identical despite different names*

## Comparing `azure-mgmt-batch-8.0.1/azure_mgmt_batch.egg-info/SOURCES.txt` & `azure-mgmt-batch-9.0.0/azure_mgmt_batch.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 azure_mgmt_batch.egg-info/dependency_links.txt
 azure_mgmt_batch.egg-info/not-zip-safe
 azure_mgmt_batch.egg-info/requires.txt
 azure_mgmt_batch.egg-info/top_level.txt
 tests/mgmt_batch_preparers.py
 tests/test_mgmt_batch.py
 tests/recordings/test_mgmt_batch.test_mgmt_batch_account.yaml
+tests/recordings/test_mgmt_batch.test_mgmt_batch_account_advanced.yaml
 tests/recordings/test_mgmt_batch.test_mgmt_batch_account_name.yaml
 tests/recordings/test_mgmt_batch.test_mgmt_batch_applications.yaml
 tests/recordings/test_mgmt_batch.test_mgmt_batch_byos_account.yaml
 tests/recordings/test_mgmt_batch.test_mgmt_batch_certificates.yaml
 tests/recordings/test_mgmt_batch.test_mgmt_batch_list_operations.yaml
 tests/recordings/test_mgmt_batch.test_mgmt_batch_pools.yaml
 tests/recordings/test_mgmt_batch.test_mgmt_batch_subscription_quota.yaml
```

## Comparing `azure-mgmt-batch-8.0.1/azure_mgmt_batch.egg-info/PKG-INFO` & `azure-mgmt-batch-9.0.0/azure_mgmt_batch.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-batch
-Version: 8.0.1
+Version: 9.0.0
 Summary: Microsoft Azure Batch Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Description: ## Microsoft Azure SDK for Python
         
@@ -33,20 +33,43 @@
         If you encounter any bugs or have suggestions, please file an issue in
         the [Issues](https://github.com/Azure/azure-sdk-for-python/issues)
         section of the project.
         
         ![image](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-batch%2FREADME.png)
         
         # Release History
+        ## 9.0.0 (2020-05-29)
+        ### REST API version
+        - This version targets REST API version 2020-05-01.
+        
+        ### Features
+        - Added ability to access the Batch DataPlane API without needing a public DNS entry for the account via the new `public_network_access` property on `BatchAccount`.
+        - Added new `PrivateLinkResource` and `PrivateEndpointConnection` resource types. These are both only used when the `public_network_access` property on `BatchAccount` is set to `Disabled`.
+          - When `public_network_access` is set to `Disabled` a new `PrivateLinkResource` is visible in that account, which can be used to connect to the account using an ARM Private Endpoint in your VNET.
+        - Added ability to encrypt `ComputeNode` disk drives using the new `disk_encryption_configuration` property of `VirtualMachineConfiguration`.
+        - **[Breaking]** The `id` property of `ImageReference` can now only refer to a Shared Image Gallery image.
+        - **[Breaking]** Pools can now be provisioned without a public IP using the new `public_ip_configuration` property of `NetworkConfiguration`.
+          - The `public_ips` property of `NetworkConfiguration` has moved in to `PublicIPAddressConfiguration` as well. This property can only be specified if `IPAddressProvisioningType` is `UserManaged`.
+        - Adds a new property `identity` of type `BatchAccountIdentity` to `BatchAccount`. This can be used to configure how customer data is encrypted inside the Batch account.
+            - This new property is configurable at  the account level on create and update through a new `identity` property on `BatchAccountCreateParameters` and `BatchAccountUpdateParameters`
+        
+        ### Fixes
+        - [Breaking] Move tags from being an argument on create and update pool parameters to being a part of `BatchAccountCreateParameters` and `BatchAccountUpdateParameters` to properly reflect the REST API
+        
+        ## 8.0.1 (2020-05-26) [Deprecated]
+        ### Notices
+        - This version targeted an invalid REST API. This version does not honor the associated REST API contract.
         
-        ## 8.0.1 (2020-05-26)
         ### Bugfixes
-        - Fix issues in PrivateEndpointConnection get and update methods due to mistakes in the Swagger specification causing validation to fail.
+        - Fix issues in PrivateEndpointConnection get and update methods due to mistakes in the Swagger specification causing validation to fail. It is advised to use version 9+ to make use of the features added in this version.
+        
+        ## 8.0.0 (2020-04-10) [Deprecated]
+        ### Notices
+        - This version targeted an invalid REST API. Currently the PrivateEndpoint get() and update() functions do not function correctly. It is advised to use version 9+ to make use of the features added in this version.
         
-        ## 8.0.0 (2020-04-10)
         ### REST API version
         - This version targets REST API version 2020-03-01.
         
         ### Features
         - Added ability to access the Batch DataPlane API without needing a public DNS entry for the account via the new `public_network_access` property on `BatchAccount`.
         - Added new `PrivateLinkResource` and `PrivateEndpointConnection` resource types. These are both only used when the `public_network_access` property on `BatchAccount` is set to `Disabled`.
           - When `public_network_access` is set to `Disabled` a new `PrivateLinkResource` is visible in that account, which can be used to connect to the account using an ARM Private Endpoint in your VNET.
```

## Comparing `azure-mgmt-batch-8.0.1/azure/mgmt/batch/_configuration.py` & `azure-mgmt-batch-9.0.0/azure/mgmt/batch/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-batch-8.0.1/azure/mgmt/batch/_batch_management_client.py` & `azure-mgmt-batch-9.0.0/azure/mgmt/batch/_batch_management_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     def __init__(
             self, credentials, subscription_id, base_url=None):
 
         self.config = BatchManagementClientConfiguration(credentials, subscription_id, base_url)
         super(BatchManagementClient, self).__init__(self.config.credentials, self.config)
 
         client_models = {k: v for k, v in models.__dict__.items() if isinstance(v, type)}
-        self.api_version = '2020-03-01'
+        self.api_version = '2020-05-01'
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
 
         self.batch_account = BatchAccountOperations(
             self._client, self.config, self._serialize, self._deserialize)
         self.application_package = ApplicationPackageOperations(
             self._client, self.config, self._serialize, self._deserialize)
```

## Comparing `azure-mgmt-batch-8.0.1/azure/mgmt/batch/__init__.py` & `azure-mgmt-batch-9.0.0/azure/mgmt/batch/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-batch-8.0.1/azure/mgmt/batch/models/_models_py3.py` & `azure-mgmt-batch-9.0.0/azure/mgmt/batch/models/_models_py3.py`

 * *Files 2% similar despite different names*

```diff
@@ -566,14 +566,17 @@
      associated with the Batch account
     :vartype private_endpoint_connections:
      list[~azure.mgmt.batch.models.PrivateEndpointConnection]
     :ivar auto_storage: The properties and status of any auto-storage account
      associated with the Batch account.
     :vartype auto_storage: ~azure.mgmt.batch.models.AutoStorageProperties
     :ivar encryption: The encryption configuration for the Batch account.
+     Configures how customer data is encrypted inside the Batch account. By
+     default, accounts are encrypted using a Microsoft managed key. For
+     additional control, a customer-managed key can be used instead.
     :vartype encryption: ~azure.mgmt.batch.models.EncryptionProperties
     :ivar dedicated_core_quota: The dedicated core quota for the Batch
      account. For accounts with PoolAllocationMode set to UserSubscription,
      quota is managed on the subscription so this value is not returned.
     :vartype dedicated_core_quota: int
     :ivar low_priority_core_quota: The low-priority core quota for the Batch
      account. For accounts with PoolAllocationMode set to UserSubscription,
@@ -597,14 +600,16 @@
      account, and the old dedicatedCoreQuota does not apply.
     :vartype dedicated_core_quota_per_vm_family_enforced: bool
     :ivar pool_quota: The pool quota for the Batch account.
     :vartype pool_quota: int
     :ivar active_job_and_job_schedule_quota: The active job and job schedule
      quota for the Batch account.
     :vartype active_job_and_job_schedule_quota: int
+    :param identity: The identity of the Batch account.
+    :type identity: ~azure.mgmt.batch.models.BatchAccountIdentity
     """
 
     _validation = {
         'id': {'readonly': True},
         'name': {'readonly': True},
         'type': {'readonly': True},
         'location': {'readonly': True},
@@ -641,17 +646,18 @@
         'encryption': {'key': 'properties.encryption', 'type': 'EncryptionProperties'},
         'dedicated_core_quota': {'key': 'properties.dedicatedCoreQuota', 'type': 'int'},
         'low_priority_core_quota': {'key': 'properties.lowPriorityCoreQuota', 'type': 'int'},
         'dedicated_core_quota_per_vm_family': {'key': 'properties.dedicatedCoreQuotaPerVMFamily', 'type': '[VirtualMachineFamilyCoreQuota]'},
         'dedicated_core_quota_per_vm_family_enforced': {'key': 'properties.dedicatedCoreQuotaPerVMFamilyEnforced', 'type': 'bool'},
         'pool_quota': {'key': 'properties.poolQuota', 'type': 'int'},
         'active_job_and_job_schedule_quota': {'key': 'properties.activeJobAndJobScheduleQuota', 'type': 'int'},
+        'identity': {'key': 'identity', 'type': 'BatchAccountIdentity'},
     }
 
-    def __init__(self, **kwargs) -> None:
+    def __init__(self, *, identity=None, **kwargs) -> None:
         super(BatchAccount, self).__init__(**kwargs)
         self.account_endpoint = None
         self.provisioning_state = None
         self.pool_allocation_mode = None
         self.key_vault_reference = None
         self.public_network_access = None
         self.private_endpoint_connections = None
@@ -659,14 +665,15 @@
         self.encryption = None
         self.dedicated_core_quota = None
         self.low_priority_core_quota = None
         self.dedicated_core_quota_per_vm_family = None
         self.dedicated_core_quota_per_vm_family_enforced = None
         self.pool_quota = None
         self.active_job_and_job_schedule_quota = None
+        self.identity = identity
 
 
 class BatchAccountCreateParameters(Model):
     """Parameters supplied to the Create operation.
 
     All required parameters must be populated in order to send to Azure.
 
@@ -690,40 +697,87 @@
     :type key_vault_reference: ~azure.mgmt.batch.models.KeyVaultReference
     :param public_network_access: The network access type for accessing Azure
      Batch account. If not specified, the default value is 'enabled'. Possible
      values include: 'Enabled', 'Disabled'. Default value: "Enabled" .
     :type public_network_access: str or
      ~azure.mgmt.batch.models.PublicNetworkAccessType
     :param encryption: The encryption configuration for the Batch account.
+     Configures how customer data is encrypted inside the Batch account. By
+     default, accounts are encrypted using a Microsoft managed key. For
+     additional control, a customer-managed key can be used instead.
     :type encryption: ~azure.mgmt.batch.models.EncryptionProperties
+    :param identity: The identity of the Batch account.
+    :type identity: ~azure.mgmt.batch.models.BatchAccountIdentity
     """
 
     _validation = {
         'location': {'required': True},
     }
 
     _attribute_map = {
         'location': {'key': 'location', 'type': 'str'},
         'tags': {'key': 'tags', 'type': '{str}'},
         'auto_storage': {'key': 'properties.autoStorage', 'type': 'AutoStorageBaseProperties'},
         'pool_allocation_mode': {'key': 'properties.poolAllocationMode', 'type': 'PoolAllocationMode'},
         'key_vault_reference': {'key': 'properties.keyVaultReference', 'type': 'KeyVaultReference'},
         'public_network_access': {'key': 'properties.publicNetworkAccess', 'type': 'PublicNetworkAccessType'},
         'encryption': {'key': 'properties.encryption', 'type': 'EncryptionProperties'},
+        'identity': {'key': 'identity', 'type': 'BatchAccountIdentity'},
     }
 
-    def __init__(self, *, location: str, tags=None, auto_storage=None, pool_allocation_mode=None, key_vault_reference=None, public_network_access="Enabled", encryption=None, **kwargs) -> None:
+    def __init__(self, *, location: str, tags=None, auto_storage=None, pool_allocation_mode=None, key_vault_reference=None, public_network_access="Enabled", encryption=None, identity=None, **kwargs) -> None:
         super(BatchAccountCreateParameters, self).__init__(**kwargs)
         self.location = location
         self.tags = tags
         self.auto_storage = auto_storage
         self.pool_allocation_mode = pool_allocation_mode
         self.key_vault_reference = key_vault_reference
         self.public_network_access = public_network_access
         self.encryption = encryption
+        self.identity = identity
+
+
+class BatchAccountIdentity(Model):
+    """The identity of the Batch account, if configured. This is only used when
+    the user specifies 'Microsoft.KeyVault' as their Batch account encryption
+    configuration.
+
+    Variables are only populated by the server, and will be ignored when
+    sending a request.
+
+    All required parameters must be populated in order to send to Azure.
+
+    :ivar principal_id: The principal id of the Batch account. This property
+     will only be provided for a system assigned identity.
+    :vartype principal_id: str
+    :ivar tenant_id: The tenant id associated with the Batch account. This
+     property will only be provided for a system assigned identity.
+    :vartype tenant_id: str
+    :param type: Required. The type of identity used for the Batch account.
+     Possible values include: 'SystemAssigned', 'None'
+    :type type: str or ~azure.mgmt.batch.models.ResourceIdentityType
+    """
+
+    _validation = {
+        'principal_id': {'readonly': True},
+        'tenant_id': {'readonly': True},
+        'type': {'required': True},
+    }
+
+    _attribute_map = {
+        'principal_id': {'key': 'principalId', 'type': 'str'},
+        'tenant_id': {'key': 'tenantId', 'type': 'str'},
+        'type': {'key': 'type', 'type': 'ResourceIdentityType'},
+    }
+
+    def __init__(self, *, type, **kwargs) -> None:
+        super(BatchAccountIdentity, self).__init__(**kwargs)
+        self.principal_id = None
+        self.tenant_id = None
+        self.type = type
 
 
 class BatchAccountKeys(Model):
     """A set of Azure Batch account keys.
 
     Variables are only populated by the server, and will be ignored when
     sending a request.
@@ -782,28 +836,35 @@
     """Parameters for updating an Azure Batch account.
 
     :param tags: The user-specified tags associated with the account.
     :type tags: dict[str, str]
     :param auto_storage: The properties related to the auto-storage account.
     :type auto_storage: ~azure.mgmt.batch.models.AutoStorageBaseProperties
     :param encryption: The encryption configuration for the Batch account.
+     Configures how customer data is encrypted inside the Batch account. By
+     default, accounts are encrypted using a Microsoft managed key. For
+     additional control, a customer-managed key can be used instead.
     :type encryption: ~azure.mgmt.batch.models.EncryptionProperties
+    :param identity: The identity of the Batch account.
+    :type identity: ~azure.mgmt.batch.models.BatchAccountIdentity
     """
 
     _attribute_map = {
         'tags': {'key': 'tags', 'type': '{str}'},
         'auto_storage': {'key': 'properties.autoStorage', 'type': 'AutoStorageBaseProperties'},
         'encryption': {'key': 'properties.encryption', 'type': 'EncryptionProperties'},
+        'identity': {'key': 'identity', 'type': 'BatchAccountIdentity'},
     }
 
-    def __init__(self, *, tags=None, auto_storage=None, encryption=None, **kwargs) -> None:
+    def __init__(self, *, tags=None, auto_storage=None, encryption=None, identity=None, **kwargs) -> None:
         super(BatchAccountUpdateParameters, self).__init__(**kwargs)
         self.tags = tags
         self.auto_storage = auto_storage
         self.encryption = encryption
+        self.identity = identity
 
 
 class BatchLocationQuota(Model):
     """Quotas associated with a Batch region for a particular subscription.
 
     Variables are only populated by the server, and will be ignored when
     sending a request.
@@ -1462,15 +1523,17 @@
 
     def __init__(self, *, targets=None, **kwargs) -> None:
         super(DiskEncryptionConfiguration, self).__init__(**kwargs)
         self.targets = targets
 
 
 class EncryptionProperties(Model):
-    """EncryptionProperties.
+    """Configures how customer data is encrypted inside the Batch account. By
+    default, accounts are encrypted using a Microsoft managed key. For
+    additional control, a customer-managed key can be used instead.
 
     :param key_source: Type of the key source. Possible values include:
      'Microsoft.Batch', 'Microsoft.KeyVault'
     :type key_source: str or ~azure.mgmt.batch.models.KeySource
     :param key_vault_properties: Additional details when using
      Microsoft.KeyVault
     :type key_vault_properties: ~azure.mgmt.batch.models.KeyVaultProperties
@@ -1662,18 +1725,24 @@
         self.backend_port = backend_port
         self.frontend_port_range_start = frontend_port_range_start
         self.frontend_port_range_end = frontend_port_range_end
         self.network_security_group_rules = network_security_group_rules
 
 
 class KeyVaultProperties(Model):
-    """KeyVaultProperties.
+    """KeyVault configuration when using an encryption KeySource of
+    Microsoft.KeyVault.
 
     :param key_identifier: Full path to the versioned secret. Example
-     https://mykeyvault.vault.azure.net/keys/testkey/6e34a81fef704045975661e297a4c053
+     https://mykeyvault.vault.azure.net/keys/testkey/6e34a81fef704045975661e297a4c053.
+     To be usable the following prerequisites must be met:
+     The Batch Account has a System Assigned identity
+     The account identity has been granted Key/Get, Key/Unwrap and Key/Wrap
+     permissions
+     The KeyVault has soft-delete and purge protection enabled
     :type key_identifier: str
     """
 
     _attribute_map = {
         'key_identifier': {'key': 'keyIdentifier', 'type': 'str'},
     }
```

## Comparing `azure-mgmt-batch-8.0.1/azure/mgmt/batch/models/_models.py` & `azure-mgmt-batch-9.0.0/azure/mgmt/batch/models/_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -566,14 +566,17 @@
      associated with the Batch account
     :vartype private_endpoint_connections:
      list[~azure.mgmt.batch.models.PrivateEndpointConnection]
     :ivar auto_storage: The properties and status of any auto-storage account
      associated with the Batch account.
     :vartype auto_storage: ~azure.mgmt.batch.models.AutoStorageProperties
     :ivar encryption: The encryption configuration for the Batch account.
+     Configures how customer data is encrypted inside the Batch account. By
+     default, accounts are encrypted using a Microsoft managed key. For
+     additional control, a customer-managed key can be used instead.
     :vartype encryption: ~azure.mgmt.batch.models.EncryptionProperties
     :ivar dedicated_core_quota: The dedicated core quota for the Batch
      account. For accounts with PoolAllocationMode set to UserSubscription,
      quota is managed on the subscription so this value is not returned.
     :vartype dedicated_core_quota: int
     :ivar low_priority_core_quota: The low-priority core quota for the Batch
      account. For accounts with PoolAllocationMode set to UserSubscription,
@@ -597,14 +600,16 @@
      account, and the old dedicatedCoreQuota does not apply.
     :vartype dedicated_core_quota_per_vm_family_enforced: bool
     :ivar pool_quota: The pool quota for the Batch account.
     :vartype pool_quota: int
     :ivar active_job_and_job_schedule_quota: The active job and job schedule
      quota for the Batch account.
     :vartype active_job_and_job_schedule_quota: int
+    :param identity: The identity of the Batch account.
+    :type identity: ~azure.mgmt.batch.models.BatchAccountIdentity
     """
 
     _validation = {
         'id': {'readonly': True},
         'name': {'readonly': True},
         'type': {'readonly': True},
         'location': {'readonly': True},
@@ -641,14 +646,15 @@
         'encryption': {'key': 'properties.encryption', 'type': 'EncryptionProperties'},
         'dedicated_core_quota': {'key': 'properties.dedicatedCoreQuota', 'type': 'int'},
         'low_priority_core_quota': {'key': 'properties.lowPriorityCoreQuota', 'type': 'int'},
         'dedicated_core_quota_per_vm_family': {'key': 'properties.dedicatedCoreQuotaPerVMFamily', 'type': '[VirtualMachineFamilyCoreQuota]'},
         'dedicated_core_quota_per_vm_family_enforced': {'key': 'properties.dedicatedCoreQuotaPerVMFamilyEnforced', 'type': 'bool'},
         'pool_quota': {'key': 'properties.poolQuota', 'type': 'int'},
         'active_job_and_job_schedule_quota': {'key': 'properties.activeJobAndJobScheduleQuota', 'type': 'int'},
+        'identity': {'key': 'identity', 'type': 'BatchAccountIdentity'},
     }
 
     def __init__(self, **kwargs):
         super(BatchAccount, self).__init__(**kwargs)
         self.account_endpoint = None
         self.provisioning_state = None
         self.pool_allocation_mode = None
@@ -659,14 +665,15 @@
         self.encryption = None
         self.dedicated_core_quota = None
         self.low_priority_core_quota = None
         self.dedicated_core_quota_per_vm_family = None
         self.dedicated_core_quota_per_vm_family_enforced = None
         self.pool_quota = None
         self.active_job_and_job_schedule_quota = None
+        self.identity = kwargs.get('identity', None)
 
 
 class BatchAccountCreateParameters(Model):
     """Parameters supplied to the Create operation.
 
     All required parameters must be populated in order to send to Azure.
 
@@ -690,40 +697,87 @@
     :type key_vault_reference: ~azure.mgmt.batch.models.KeyVaultReference
     :param public_network_access: The network access type for accessing Azure
      Batch account. If not specified, the default value is 'enabled'. Possible
      values include: 'Enabled', 'Disabled'. Default value: "Enabled" .
     :type public_network_access: str or
      ~azure.mgmt.batch.models.PublicNetworkAccessType
     :param encryption: The encryption configuration for the Batch account.
+     Configures how customer data is encrypted inside the Batch account. By
+     default, accounts are encrypted using a Microsoft managed key. For
+     additional control, a customer-managed key can be used instead.
     :type encryption: ~azure.mgmt.batch.models.EncryptionProperties
+    :param identity: The identity of the Batch account.
+    :type identity: ~azure.mgmt.batch.models.BatchAccountIdentity
     """
 
     _validation = {
         'location': {'required': True},
     }
 
     _attribute_map = {
         'location': {'key': 'location', 'type': 'str'},
         'tags': {'key': 'tags', 'type': '{str}'},
         'auto_storage': {'key': 'properties.autoStorage', 'type': 'AutoStorageBaseProperties'},
         'pool_allocation_mode': {'key': 'properties.poolAllocationMode', 'type': 'PoolAllocationMode'},
         'key_vault_reference': {'key': 'properties.keyVaultReference', 'type': 'KeyVaultReference'},
         'public_network_access': {'key': 'properties.publicNetworkAccess', 'type': 'PublicNetworkAccessType'},
         'encryption': {'key': 'properties.encryption', 'type': 'EncryptionProperties'},
+        'identity': {'key': 'identity', 'type': 'BatchAccountIdentity'},
     }
 
     def __init__(self, **kwargs):
         super(BatchAccountCreateParameters, self).__init__(**kwargs)
         self.location = kwargs.get('location', None)
         self.tags = kwargs.get('tags', None)
         self.auto_storage = kwargs.get('auto_storage', None)
         self.pool_allocation_mode = kwargs.get('pool_allocation_mode', None)
         self.key_vault_reference = kwargs.get('key_vault_reference', None)
         self.public_network_access = kwargs.get('public_network_access', "Enabled")
         self.encryption = kwargs.get('encryption', None)
+        self.identity = kwargs.get('identity', None)
+
+
+class BatchAccountIdentity(Model):
+    """The identity of the Batch account, if configured. This is only used when
+    the user specifies 'Microsoft.KeyVault' as their Batch account encryption
+    configuration.
+
+    Variables are only populated by the server, and will be ignored when
+    sending a request.
+
+    All required parameters must be populated in order to send to Azure.
+
+    :ivar principal_id: The principal id of the Batch account. This property
+     will only be provided for a system assigned identity.
+    :vartype principal_id: str
+    :ivar tenant_id: The tenant id associated with the Batch account. This
+     property will only be provided for a system assigned identity.
+    :vartype tenant_id: str
+    :param type: Required. The type of identity used for the Batch account.
+     Possible values include: 'SystemAssigned', 'None'
+    :type type: str or ~azure.mgmt.batch.models.ResourceIdentityType
+    """
+
+    _validation = {
+        'principal_id': {'readonly': True},
+        'tenant_id': {'readonly': True},
+        'type': {'required': True},
+    }
+
+    _attribute_map = {
+        'principal_id': {'key': 'principalId', 'type': 'str'},
+        'tenant_id': {'key': 'tenantId', 'type': 'str'},
+        'type': {'key': 'type', 'type': 'ResourceIdentityType'},
+    }
+
+    def __init__(self, **kwargs):
+        super(BatchAccountIdentity, self).__init__(**kwargs)
+        self.principal_id = None
+        self.tenant_id = None
+        self.type = kwargs.get('type', None)
 
 
 class BatchAccountKeys(Model):
     """A set of Azure Batch account keys.
 
     Variables are only populated by the server, and will be ignored when
     sending a request.
@@ -782,28 +836,35 @@
     """Parameters for updating an Azure Batch account.
 
     :param tags: The user-specified tags associated with the account.
     :type tags: dict[str, str]
     :param auto_storage: The properties related to the auto-storage account.
     :type auto_storage: ~azure.mgmt.batch.models.AutoStorageBaseProperties
     :param encryption: The encryption configuration for the Batch account.
+     Configures how customer data is encrypted inside the Batch account. By
+     default, accounts are encrypted using a Microsoft managed key. For
+     additional control, a customer-managed key can be used instead.
     :type encryption: ~azure.mgmt.batch.models.EncryptionProperties
+    :param identity: The identity of the Batch account.
+    :type identity: ~azure.mgmt.batch.models.BatchAccountIdentity
     """
 
     _attribute_map = {
         'tags': {'key': 'tags', 'type': '{str}'},
         'auto_storage': {'key': 'properties.autoStorage', 'type': 'AutoStorageBaseProperties'},
         'encryption': {'key': 'properties.encryption', 'type': 'EncryptionProperties'},
+        'identity': {'key': 'identity', 'type': 'BatchAccountIdentity'},
     }
 
     def __init__(self, **kwargs):
         super(BatchAccountUpdateParameters, self).__init__(**kwargs)
         self.tags = kwargs.get('tags', None)
         self.auto_storage = kwargs.get('auto_storage', None)
         self.encryption = kwargs.get('encryption', None)
+        self.identity = kwargs.get('identity', None)
 
 
 class BatchLocationQuota(Model):
     """Quotas associated with a Batch region for a particular subscription.
 
     Variables are only populated by the server, and will be ignored when
     sending a request.
@@ -1462,15 +1523,17 @@
 
     def __init__(self, **kwargs):
         super(DiskEncryptionConfiguration, self).__init__(**kwargs)
         self.targets = kwargs.get('targets', None)
 
 
 class EncryptionProperties(Model):
-    """EncryptionProperties.
+    """Configures how customer data is encrypted inside the Batch account. By
+    default, accounts are encrypted using a Microsoft managed key. For
+    additional control, a customer-managed key can be used instead.
 
     :param key_source: Type of the key source. Possible values include:
      'Microsoft.Batch', 'Microsoft.KeyVault'
     :type key_source: str or ~azure.mgmt.batch.models.KeySource
     :param key_vault_properties: Additional details when using
      Microsoft.KeyVault
     :type key_vault_properties: ~azure.mgmt.batch.models.KeyVaultProperties
@@ -1662,18 +1725,24 @@
         self.backend_port = kwargs.get('backend_port', None)
         self.frontend_port_range_start = kwargs.get('frontend_port_range_start', None)
         self.frontend_port_range_end = kwargs.get('frontend_port_range_end', None)
         self.network_security_group_rules = kwargs.get('network_security_group_rules', None)
 
 
 class KeyVaultProperties(Model):
-    """KeyVaultProperties.
+    """KeyVault configuration when using an encryption KeySource of
+    Microsoft.KeyVault.
 
     :param key_identifier: Full path to the versioned secret. Example
-     https://mykeyvault.vault.azure.net/keys/testkey/6e34a81fef704045975661e297a4c053
+     https://mykeyvault.vault.azure.net/keys/testkey/6e34a81fef704045975661e297a4c053.
+     To be usable the following prerequisites must be met:
+     The Batch Account has a System Assigned identity
+     The account identity has been granted Key/Get, Key/Unwrap and Key/Wrap
+     permissions
+     The KeyVault has soft-delete and purge protection enabled
     :type key_identifier: str
     """
 
     _attribute_map = {
         'key_identifier': {'key': 'keyIdentifier', 'type': 'str'},
     }
```

## Comparing `azure-mgmt-batch-8.0.1/azure/mgmt/batch/models/__init__.py` & `azure-mgmt-batch-9.0.0/azure/mgmt/batch/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     from ._models_py3 import AutoStorageBaseProperties
     from ._models_py3 import AutoStorageProperties
     from ._models_py3 import AutoUserSpecification
     from ._models_py3 import AzureBlobFileSystemConfiguration
     from ._models_py3 import AzureFileShareConfiguration
     from ._models_py3 import BatchAccount
     from ._models_py3 import BatchAccountCreateParameters
+    from ._models_py3 import BatchAccountIdentity
     from ._models_py3 import BatchAccountKeys
     from ._models_py3 import BatchAccountRegenerateKeyParameters
     from ._models_py3 import BatchAccountUpdateParameters
     from ._models_py3 import BatchLocationQuota
     from ._models_py3 import Certificate
     from ._models_py3 import CertificateBaseProperties
     from ._models_py3 import CertificateCreateOrUpdateParameters
@@ -90,14 +91,15 @@
     from ._models import AutoStorageBaseProperties
     from ._models import AutoStorageProperties
     from ._models import AutoUserSpecification
     from ._models import AzureBlobFileSystemConfiguration
     from ._models import AzureFileShareConfiguration
     from ._models import BatchAccount
     from ._models import BatchAccountCreateParameters
+    from ._models import BatchAccountIdentity
     from ._models import BatchAccountKeys
     from ._models import BatchAccountRegenerateKeyParameters
     from ._models import BatchAccountUpdateParameters
     from ._models import BatchLocationQuota
     from ._models import Certificate
     from ._models import CertificateBaseProperties
     from ._models import CertificateCreateOrUpdateParameters
@@ -157,14 +159,15 @@
 from ._paged_models import PoolPaged
 from ._paged_models import PrivateEndpointConnectionPaged
 from ._paged_models import PrivateLinkResourcePaged
 from ._batch_management_client_enums import (
     KeySource,
     PoolAllocationMode,
     PublicNetworkAccessType,
+    ResourceIdentityType,
     ProvisioningState,
     PrivateEndpointConnectionProvisioningState,
     PrivateLinkServiceConnectionStatus,
     AccountKeyType,
     PackageState,
     CertificateFormat,
     CertificateProvisioningState,
@@ -201,14 +204,15 @@
     'AutoStorageBaseProperties',
     'AutoStorageProperties',
     'AutoUserSpecification',
     'AzureBlobFileSystemConfiguration',
     'AzureFileShareConfiguration',
     'BatchAccount',
     'BatchAccountCreateParameters',
+    'BatchAccountIdentity',
     'BatchAccountKeys',
     'BatchAccountRegenerateKeyParameters',
     'BatchAccountUpdateParameters',
     'BatchLocationQuota',
     'Certificate',
     'CertificateBaseProperties',
     'CertificateCreateOrUpdateParameters',
@@ -267,14 +271,15 @@
     'CertificatePaged',
     'PrivateLinkResourcePaged',
     'PrivateEndpointConnectionPaged',
     'PoolPaged',
     'KeySource',
     'PoolAllocationMode',
     'PublicNetworkAccessType',
+    'ResourceIdentityType',
     'ProvisioningState',
     'PrivateEndpointConnectionProvisioningState',
     'PrivateLinkServiceConnectionStatus',
     'AccountKeyType',
     'PackageState',
     'CertificateFormat',
     'CertificateProvisioningState',
```

## Comparing `azure-mgmt-batch-8.0.1/azure/mgmt/batch/models/_paged_models.py` & `azure-mgmt-batch-9.0.0/azure/mgmt/batch/models/_paged_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-batch-8.0.1/azure/mgmt/batch/models/_batch_management_client_enums.py` & `azure-mgmt-batch-9.0.0/azure/mgmt/batch/models/_batch_management_client_enums.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,29 +11,35 @@
 
 from enum import Enum
 
 
 class KeySource(str, Enum):
 
     microsoft_batch = "Microsoft.Batch"  #: Batch creates and manages the encryption keys used to protect the account data.
-    microsoft_key_vault = "Microsoft.KeyVault"  #: The encryption keys used to protect the account data are stored in an external key vault.
+    microsoft_key_vault = "Microsoft.KeyVault"  #: The encryption keys used to protect the account data are stored in an external key vault. If this is set then the Batch Account identity must be set to `SystemAssigned` and a valid Key Identifier must also be supplied under the keyVaultProperties.
 
 
 class PoolAllocationMode(str, Enum):
 
     batch_service = "BatchService"  #: Pools will be allocated in subscriptions owned by the Batch service.
     user_subscription = "UserSubscription"  #: Pools will be allocated in a subscription owned by the user.
 
 
 class PublicNetworkAccessType(str, Enum):
 
     enabled = "Enabled"  #: Enables connectivity to Azure Batch through public DNS.
     disabled = "Disabled"  #: Disables public connectivity and enables private connectivity to Azure Batch Service through private endpoint resource.
 
 
+class ResourceIdentityType(str, Enum):
+
+    system_assigned = "SystemAssigned"  #: Batch account has a system assigned identity with it.
+    none = "None"  #: Batch account has no identity associated with it. Setting `None` in update account will remove existing identities.
+
+
 class ProvisioningState(str, Enum):
 
     invalid = "Invalid"  #: The account is in an invalid state.
     creating = "Creating"  #: The account is being created.
     deleting = "Deleting"  #: The account is being deleted.
     succeeded = "Succeeded"  #: The account has been created and is ready for use.
     failed = "Failed"  #: The last operation for the account is failed.
```

## Comparing `azure-mgmt-batch-8.0.1/azure/mgmt/batch/operations/_batch_account_operations.py` & `azure-mgmt-batch-9.0.0/azure/mgmt/batch/operations/_batch_account_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,25 +23,25 @@
 
     You should not instantiate directly this class, but create a Client instance that will create it for you and attach it as attribute.
 
     :param client: Client for service requests.
     :param config: Configuration of service client.
     :param serializer: An object model serializer.
     :param deserializer: An object model deserializer.
-    :ivar api_version: The API version to use for the request. Constant value: "2020-03-01".
+    :ivar api_version: The API version to use for the request. Constant value: "2020-05-01".
     """
 
     models = models
 
     def __init__(self, client, config, serializer, deserializer):
 
         self._client = client
         self._serialize = serializer
         self._deserialize = deserializer
-        self.api_version = "2020-03-01"
+        self.api_version = "2020-05-01"
 
         self.config = config
 
 
     def _create_initial(
             self, resource_group_name, account_name, parameters, custom_headers=None, raw=False, **operation_config):
         # Construct URL
@@ -158,39 +158,35 @@
         if polling is True: polling_method = ARMPolling(lro_delay, **operation_config)
         elif polling is False: polling_method = NoPolling()
         else: polling_method = polling
         return LROPoller(self._client, raw_result, get_long_running_output, polling_method)
     create.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Batch/batchAccounts/{accountName}'}
 
     def update(
-            self, resource_group_name, account_name, tags=None, auto_storage=None, custom_headers=None, raw=False, **operation_config):
+            self, resource_group_name, account_name, parameters, custom_headers=None, raw=False, **operation_config):
         """Updates the properties of an existing Batch account.
 
         :param resource_group_name: The name of the resource group that
          contains the Batch account.
         :type resource_group_name: str
         :param account_name: The name of the Batch account.
         :type account_name: str
-        :param tags: The user-specified tags associated with the account.
-        :type tags: dict[str, str]
-        :param auto_storage: The properties related to the auto-storage
-         account.
-        :type auto_storage: ~azure.mgmt.batch.models.AutoStorageBaseProperties
+        :param parameters: Additional parameters for account update.
+        :type parameters:
+         ~azure.mgmt.batch.models.BatchAccountUpdateParameters
         :param dict custom_headers: headers that will be added to the request
         :param bool raw: returns the direct response alongside the
          deserialized response
         :param operation_config: :ref:`Operation configuration
          overrides<msrest:optionsforoperations>`.
         :return: BatchAccount or ClientRawResponse if raw=true
         :rtype: ~azure.mgmt.batch.models.BatchAccount or
          ~msrest.pipeline.ClientRawResponse
         :raises: :class:`CloudError<msrestazure.azure_exceptions.CloudError>`
         """
-        parameters = models.BatchAccountUpdateParameters(tags=tags, auto_storage=auto_storage)
-
         # Construct URL
         url = self.update.metadata['url']
         path_format_arguments = {
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
             'accountName': self._serialize.url("account_name", account_name, 'str', max_length=24, min_length=3, pattern=r'^[a-zA-Z0-9]+$'),
             'subscriptionId': self._serialize.url("self.config.subscription_id", self.config.subscription_id, 'str')
         }
```

## Comparing `azure-mgmt-batch-8.0.1/azure/mgmt/batch/operations/_private_link_resource_operations.py` & `azure-mgmt-batch-9.0.0/azure/mgmt/batch/operations/_private_link_resource_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,25 +21,25 @@
 
     You should not instantiate directly this class, but create a Client instance that will create it for you and attach it as attribute.
 
     :param client: Client for service requests.
     :param config: Configuration of service client.
     :param serializer: An object model serializer.
     :param deserializer: An object model deserializer.
-    :ivar api_version: The API version to use for the request. Constant value: "2020-03-01".
+    :ivar api_version: The API version to use for the request. Constant value: "2020-05-01".
     """
 
     models = models
 
     def __init__(self, client, config, serializer, deserializer):
 
         self._client = client
         self._serialize = serializer
         self._deserialize = deserializer
-        self.api_version = "2020-03-01"
+        self.api_version = "2020-05-01"
 
         self.config = config
 
     def list_by_batch_account(
             self, resource_group_name, account_name, maxresults=None, custom_headers=None, raw=False, **operation_config):
         """Lists all of the private link resources in the specified account.
```

## Comparing `azure-mgmt-batch-8.0.1/azure/mgmt/batch/operations/_application_package_operations.py` & `azure-mgmt-batch-9.0.0/azure/mgmt/batch/operations/_application_package_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,25 +21,25 @@
 
     You should not instantiate directly this class, but create a Client instance that will create it for you and attach it as attribute.
 
     :param client: Client for service requests.
     :param config: Configuration of service client.
     :param serializer: An object model serializer.
     :param deserializer: An object model deserializer.
-    :ivar api_version: The API version to use for the request. Constant value: "2020-03-01".
+    :ivar api_version: The API version to use for the request. Constant value: "2020-05-01".
     """
 
     models = models
 
     def __init__(self, client, config, serializer, deserializer):
 
         self._client = client
         self._serialize = serializer
         self._deserialize = deserializer
-        self.api_version = "2020-03-01"
+        self.api_version = "2020-05-01"
 
         self.config = config
 
     def activate(
             self, resource_group_name, account_name, application_name, version_name, format, custom_headers=None, raw=False, **operation_config):
         """Activates the specified application package. This should be done after
         the `ApplicationPackage` was created and uploaded. This needs to be
```

## Comparing `azure-mgmt-batch-8.0.1/azure/mgmt/batch/operations/_application_operations.py` & `azure-mgmt-batch-9.0.0/azure/mgmt/batch/operations/_application_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,25 +21,25 @@
 
     You should not instantiate directly this class, but create a Client instance that will create it for you and attach it as attribute.
 
     :param client: Client for service requests.
     :param config: Configuration of service client.
     :param serializer: An object model serializer.
     :param deserializer: An object model deserializer.
-    :ivar api_version: The API version to use for the request. Constant value: "2020-03-01".
+    :ivar api_version: The API version to use for the request. Constant value: "2020-05-01".
     """
 
     models = models
 
     def __init__(self, client, config, serializer, deserializer):
 
         self._client = client
         self._serialize = serializer
         self._deserialize = deserializer
-        self.api_version = "2020-03-01"
+        self.api_version = "2020-05-01"
 
         self.config = config
 
     def create(
             self, resource_group_name, account_name, application_name, parameters=None, custom_headers=None, raw=False, **operation_config):
         """Adds an application to the specified Batch account.
```

## Comparing `azure-mgmt-batch-8.0.1/azure/mgmt/batch/operations/_pool_operations.py` & `azure-mgmt-batch-9.0.0/azure/mgmt/batch/operations/_pool_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,25 +23,25 @@
 
     You should not instantiate directly this class, but create a Client instance that will create it for you and attach it as attribute.
 
     :param client: Client for service requests.
     :param config: Configuration of service client.
     :param serializer: An object model serializer.
     :param deserializer: An object model deserializer.
-    :ivar api_version: The API version to use for the request. Constant value: "2020-03-01".
+    :ivar api_version: The API version to use for the request. Constant value: "2020-05-01".
     """
 
     models = models
 
     def __init__(self, client, config, serializer, deserializer):
 
         self._client = client
         self._serialize = serializer
         self._deserialize = deserializer
-        self.api_version = "2020-03-01"
+        self.api_version = "2020-05-01"
 
         self.config = config
 
     def list_by_batch_account(
             self, resource_group_name, account_name, maxresults=None, select=None, filter=None, custom_headers=None, raw=False, **operation_config):
         """Lists all of the pools in the specified account.
```

## Comparing `azure-mgmt-batch-8.0.1/azure/mgmt/batch/operations/__init__.py` & `azure-mgmt-batch-9.0.0/azure/mgmt/batch/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-batch-8.0.1/azure/mgmt/batch/operations/_location_operations.py` & `azure-mgmt-batch-9.0.0/azure/mgmt/batch/operations/_location_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,25 +21,25 @@
 
     You should not instantiate directly this class, but create a Client instance that will create it for you and attach it as attribute.
 
     :param client: Client for service requests.
     :param config: Configuration of service client.
     :param serializer: An object model serializer.
     :param deserializer: An object model deserializer.
-    :ivar api_version: The API version to use for the request. Constant value: "2020-03-01".
+    :ivar api_version: The API version to use for the request. Constant value: "2020-05-01".
     """
 
     models = models
 
     def __init__(self, client, config, serializer, deserializer):
 
         self._client = client
         self._serialize = serializer
         self._deserialize = deserializer
-        self.api_version = "2020-03-01"
+        self.api_version = "2020-05-01"
 
         self.config = config
 
     def get_quotas(
             self, location_name, custom_headers=None, raw=False, **operation_config):
         """Gets the Batch service quotas for the specified subscription at the
         given location.
```

## Comparing `azure-mgmt-batch-8.0.1/azure/mgmt/batch/operations/_private_endpoint_connection_operations.py` & `azure-mgmt-batch-9.0.0/azure/mgmt/batch/operations/_private_endpoint_connection_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,25 +23,25 @@
 
     You should not instantiate directly this class, but create a Client instance that will create it for you and attach it as attribute.
 
     :param client: Client for service requests.
     :param config: Configuration of service client.
     :param serializer: An object model serializer.
     :param deserializer: An object model deserializer.
-    :ivar api_version: The API version to use for the request. Constant value: "2020-03-01".
+    :ivar api_version: The API version to use for the request. Constant value: "2020-05-01".
     """
 
     models = models
 
     def __init__(self, client, config, serializer, deserializer):
 
         self._client = client
         self._serialize = serializer
         self._deserialize = deserializer
-        self.api_version = "2020-03-01"
+        self.api_version = "2020-05-01"
 
         self.config = config
 
     def list_by_batch_account(
             self, resource_group_name, account_name, maxresults=None, custom_headers=None, raw=False, **operation_config):
         """Lists all of the private endpoint connections in the specified account.
```

## Comparing `azure-mgmt-batch-8.0.1/azure/mgmt/batch/operations/_certificate_operations.py` & `azure-mgmt-batch-9.0.0/azure/mgmt/batch/operations/_certificate_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,25 +23,25 @@
 
     You should not instantiate directly this class, but create a Client instance that will create it for you and attach it as attribute.
 
     :param client: Client for service requests.
     :param config: Configuration of service client.
     :param serializer: An object model serializer.
     :param deserializer: An object model deserializer.
-    :ivar api_version: The API version to use for the request. Constant value: "2020-03-01".
+    :ivar api_version: The API version to use for the request. Constant value: "2020-05-01".
     """
 
     models = models
 
     def __init__(self, client, config, serializer, deserializer):
 
         self._client = client
         self._serialize = serializer
         self._deserialize = deserializer
-        self.api_version = "2020-03-01"
+        self.api_version = "2020-05-01"
 
         self.config = config
 
     def list_by_batch_account(
             self, resource_group_name, account_name, maxresults=None, select=None, filter=None, custom_headers=None, raw=False, **operation_config):
         """Lists all of the certificates in the specified account.
```

## Comparing `azure-mgmt-batch-8.0.1/azure/mgmt/batch/operations/_operations.py` & `azure-mgmt-batch-9.0.0/azure/mgmt/batch/operations/_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,25 +21,25 @@
 
     You should not instantiate directly this class, but create a Client instance that will create it for you and attach it as attribute.
 
     :param client: Client for service requests.
     :param config: Configuration of service client.
     :param serializer: An object model serializer.
     :param deserializer: An object model deserializer.
-    :ivar api_version: The API version to use for the request. Constant value: "2020-03-01".
+    :ivar api_version: The API version to use for the request. Constant value: "2020-05-01".
     """
 
     models = models
 
     def __init__(self, client, config, serializer, deserializer):
 
         self._client = client
         self._serialize = serializer
         self._deserialize = deserializer
-        self.api_version = "2020-03-01"
+        self.api_version = "2020-05-01"
 
         self.config = config
 
     def list(
             self, custom_headers=None, raw=False, **operation_config):
         """Lists available operations for the Microsoft.Batch provider.
```

## Comparing `azure-mgmt-batch-8.0.1/tests/mgmt_batch_preparers.py` & `azure-mgmt-batch-9.0.0/tests/mgmt_batch_preparers.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-batch-8.0.1/tests/test_mgmt_batch.py` & `azure-mgmt-batch-9.0.0/tests/test_mgmt_batch.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import time
 import unittest
 
 import requests
 
 import azure.mgmt.batch
 from azure.mgmt.batch import models
+import azure.mgmt.network.models
 from azure.common.exceptions import CloudError
 from mgmt_batch_preparers import KeyVaultPreparer, SimpleBatchPreparer
 
 from devtools_testutils import (
     AzureMgmtTestCase,
     ResourceGroupPreparer,
     StorageAccountPreparer
@@ -32,31 +33,33 @@
 
     def setUp(self):
         super(MgmtBatchTest, self).setUp()
         self.mgmt_batch_client = self.create_mgmt_client(
             azure.mgmt.batch.BatchManagementClient)
         self.mgmt_keyvault_client = self.create_mgmt_client(
             azure.mgmt.keyvault.KeyVaultManagementClient)
+        self.mgmt_network = self.create_mgmt_client(
+            azure.mgmt.network.NetworkManagementClient)
 
     def _get_account_name(self):
         return self.get_resource_name('batch')[-24:]
 
     def test_mgmt_batch_list_operations(self):
         operations = self.mgmt_batch_client.operations.list()
         all_ops = list(operations)
-        self.assertEqual(len(all_ops), 48)
+        self.assertEqual(len(all_ops), 50)
         self.assertEqual(all_ops[0].name, 'Microsoft.Batch/batchAccounts/providers/Microsoft.Insights/diagnosticSettings/read')
         self.assertEqual(all_ops[0].origin, 'system')
         self.assertEqual(all_ops[0].display.provider, 'Microsoft Batch')
         self.assertEqual(all_ops[0].display.operation, 'Read diagnostic setting')
 
     def test_mgmt_batch_subscription_quota(self):
         quotas = self.mgmt_batch_client.location.get_quotas(AZURE_LOCATION)
         self.assertIsInstance(quotas, models.BatchLocationQuota)
-        self.assertEqual(quotas.account_quota, 3)
+        self.assertEqual(quotas.account_quota, 50)
 
     def test_mgmt_batch_account_name(self):
         # Test Invalid Account Name
         availability = self.mgmt_batch_client.location.check_name_availability(
             AZURE_LOCATION, "randombatchaccount@5^$g9873495873")
         self.assertIsInstance(availability, models.CheckNameAvailabilityResult)
         self.assertFalse(availability.name_available)
@@ -113,16 +116,16 @@
             resource_group.name,
             account_name,
             batch_account)
         account_setup.result()
 
         # Test Get Account
         account = self.mgmt_batch_client.batch_account.get(resource_group.name, account_name)
-        self.assertEqual(account.dedicated_core_quota, 0)
-        self.assertEqual(account.low_priority_core_quota, 0)
+        self.assertEqual(account.dedicated_core_quota, 700)
+        self.assertEqual(account.low_priority_core_quota, 500)
         self.assertEqual(account.pool_quota, 100)
         self.assertEqual(account.pool_allocation_mode.value, 'BatchService')
 
         # Test List Accounts by Resource Group
         accounts = self.mgmt_batch_client.batch_account.list_by_resource_group(resource_group.name)
         self.assertEqual(len(list(accounts)), 1)
 
@@ -136,15 +139,15 @@
         keys = self.mgmt_batch_client.batch_account.regenerate_key(
             resource_group.name, account_name, 'Secondary')
         self.assertIsInstance(keys, models.BatchAccountKeys)
         self.assertFalse(keys.secondary == secondary)
 
         # Test Update Account
         update_tags = {'Name': 'tagName', 'Value': 'tagValue'}
-        updated = self.mgmt_batch_client.batch_account.update(resource_group.name, account_name, update_tags)
+        updated = self.mgmt_batch_client.batch_account.update(resource_group.name, account_name, models.BatchAccountUpdateParameters(tags=update_tags))
         self.assertIsInstance(updated, models.BatchAccount)
         self.assertEqual(updated.tags['Name'], 'tagName')
         self.assertEqual(updated.tags['Value'], 'tagValue')
 
         # Test Delete Account
         response = self.mgmt_batch_client.batch_account.delete(resource_group.name, account_name)
         self.assertIsNone(response.result())
@@ -358,24 +361,26 @@
             scale_settings=models.ScaleSettings(
                 auto_scale=models.AutoScaleSettings(
                     # Change this to a value once accounts get default quotas
                     formula='$TargetDedicatedNodes=0'
                 )
             )
         )
+        if self.is_live:
+            time.sleep(15)
         response = self.mgmt_batch_client.pool.update(
             resource_group.name, batch_account.name, iaas_pool, parameters)
         self.assertIsInstance(response, models.Pool)
 
         # Test Get pool
         pool = self.mgmt_batch_client.pool.get(
             resource_group.name, batch_account.name, iaas_pool)
         self.assertIsInstance(pool, models.Pool)
         self.assertEqual(pool.vm_size, 'STANDARD_A1'),
-        self.assertIsNone(pool.display_name),
+        self.assertIsNotNone(pool.display_name),
         # This assert should be reintroduced when targetDedidicated nodes can be 1+
         # self.assertEqual(pool.allocation_state, models.AllocationState.resizing)
         self.assertEqual(
             pool.deployment_configuration.virtual_machine_configuration.node_agent_sku_id,
             'batch.node.windows amd64')
 
         # Test stop resizing
@@ -389,16 +394,87 @@
         self.assertIsInstance(response, models.Pool)
 
         # Test delete pool
         response = self.mgmt_batch_client.pool.delete(
             resource_group.name, batch_account.name, iaas_pool)
         self.assertIsNone(response.result())
 
-    @ResourceGroupPreparer(location=AZURE_LOCATION)
-    @SimpleBatchPreparer(location=AZURE_LOCATION)
-    def test_mgmt_batch_private_endpoint_and_link(self, resource_group, location, batch_account):
-        result = self.mgmt_batch_client.private_link_resource.list_by_batch_account(
-            resource_group_name=resource_group,
-            account_name=batch_account)
-        result = self.mgmt_batch_client.private_endpoint_connection.list_by_batch_account(
-            resource_group_name=resource_group,
-            account_name=batch_account)
+    @ResourceGroupPreparer(location=AZURE_LOCATION, random_name_enabled=True)
+    def test_mgmt_batch_account_advanced(self, resource_group, location):
+        batch_account_name = self.get_resource_name('batchpendpoint')
+        vnet_name = self.get_resource_name('vnet')
+        subnet_name = self.get_resource_name('subnet')
+        subnet_id = "/subscriptions/{}/resourceGroups/{}/providers/Microsoft.Network/virtualNetworks/{}/subnets/{}".format(
+            self.settings.SUBSCRIPTION_ID,
+            resource_group.name,
+            vnet_name,
+            subnet_name)
+        private_endpoint_name = self.get_resource_name('pe')
+        private_connection_name = self.get_resource_name('pec')
+        private_link_service_id = '/subscriptions/{}/resourceGroups/{}/providers/Microsoft.Batch/batchAccounts/{}'.format(
+            self.settings.SUBSCRIPTION_ID,
+            resource_group.name,
+            batch_account_name)
+        batch_account = models.BatchAccountCreateParameters(
+            location=location,
+            public_network_access='Disabled',
+            identity=models.BatchAccountIdentity(
+                type='SystemAssigned'
+            ))
+        self.mgmt_batch_client.batch_account.create(
+            resource_group_name=resource_group.name,
+            account_name=batch_account_name,
+            parameters=batch_account).result()
+        self.mgmt_network.virtual_networks.create_or_update(
+            resource_group_name=resource_group.name,
+            virtual_network_name=vnet_name,
+            parameters=self.mgmt_network.models().VirtualNetwork(
+                address_space=self.mgmt_network.models().AddressSpace(
+                    address_prefixes=['10.0.0.0/16']),
+                location=location,
+                subnets=[
+                    self.mgmt_network.models().Subnet(
+                        address_prefix='10.0.0.0/24',
+                        name=subnet_name,
+                        private_endpoint_network_policies='Disabled')])
+        ).result()
+        self.mgmt_network.private_endpoints.create_or_update(
+            resource_group_name=resource_group.name,
+            private_endpoint_name=private_endpoint_name,
+            parameters=self.mgmt_network.models().PrivateEndpoint(
+                location=location,
+                subnet=self.mgmt_network.models().Subnet(
+                    id=subnet_id
+                ),
+                manual_private_link_service_connections=[
+                    self.mgmt_network.models().PrivateLinkServiceConnection(
+                        private_link_service_id=private_link_service_id,
+                        group_ids=['batchAccount'],
+                        name=private_connection_name
+                    )]
+            )
+        ).result()
+        private_links = self.mgmt_batch_client.private_link_resource.list_by_batch_account(
+            resource_group_name=resource_group.name,
+            account_name=batch_account_name)
+        private_link = private_links.__next__()
+        self.mgmt_batch_client.private_link_resource.get(
+            resource_group_name=resource_group.name,
+            account_name=batch_account_name,
+            private_link_resource_name=private_link.name)
+        private_endpoints = self.mgmt_batch_client.private_endpoint_connection.list_by_batch_account(
+            resource_group_name=resource_group.name,
+            account_name=batch_account_name)
+
+        private_endpoint = private_endpoints.__next__()
+        self.mgmt_batch_client.private_endpoint_connection.get(
+            resource_group_name=resource_group.name,
+            account_name=batch_account_name,
+            private_endpoint_connection_name=private_endpoint.name)
+        self.mgmt_batch_client.private_endpoint_connection.update(
+            resource_group_name=resource_group.name,
+            account_name=batch_account_name,
+            private_endpoint_connection_name=private_endpoint.name,
+            private_link_service_connection_state=models.PrivateLinkServiceConnectionState(
+                status='Approved',
+                description='Approved for test'
+            )).result()
```

## Comparing `azure-mgmt-batch-8.0.1/tests/recordings/test_mgmt_batch.test_mgmt_batch_list_operations.yaml` & `azure-mgmt-batch-9.0.0/tests/recordings/test_mgmt_batch.test_mgmt_batch_list_operations.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,20 @@
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.11 msrest_azure/0.6.2
-        azure-mgmt-batch/2020-03-01 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: GET
-    uri: https://management.azure.com/providers/Microsoft.Batch/operations?api-version=2020-03-01
+    uri: https://management.azure.com/providers/Microsoft.Batch/operations?api-version=2020-05-01
   response:
     body:
       string: '{"value":[{"name":"Microsoft.Batch/batchAccounts/providers/Microsoft.Insights/diagnosticSettings/read","display":{"provider":"Microsoft
         Batch","resource":"Batch Accounts","operation":"Read diagnostic setting","description":"Gets
         the diagnostic setting for the resource"},"isDataAction":false,"origin":"system"},{"name":"Microsoft.Batch/batchAccounts/providers/Microsoft.Insights/diagnosticSettings/write","display":{"provider":"Microsoft
         Batch","resource":"Batch Accounts","operation":"Write diagnostic setting","description":"Creates
         or updates the diagnostic setting for the resource"},"isDataAction":false,"origin":"system"},{"name":"Microsoft.Batch/batchAccounts/providers/Microsoft.Insights/logDefinitions/read","display":{"provider":"Microsoft
@@ -182,34 +182,40 @@
         endpoint connection","description":"Update an existing Private endpoint connection
         on a Batch account"},"isDataAction":false},{"name":"Microsoft.Batch/batchAccounts/privateEndpointConnections/read","display":{"provider":"Microsoft
         Batch","resource":"PrivateEndpointConnections","operation":"Get or List Private
         endpoint connection","description":"Gets Private endpoint connection or Lists
         Private endpoint connections on a Batch account"},"isDataAction":false},{"name":"Microsoft.Batch/batchAccounts/privateEndpointConnectionResults/read","display":{"provider":"Microsoft
         Batch","resource":"PrivateEndpointConnections","operation":"Get Batch account
         private endpoint connection operation results","description":"Gets the results
-        of a long running Batch account private endpoint connection operation"},"isDataAction":false},{"name":"Microsoft.Batch/batchAccounts/privateEndpointConnectionProxies/write","display":{"provider":"Microsoft
+        of a long running Batch account private endpoint connection operation"},"isDataAction":false},{"name":"Microsoft.Batch/batchAccounts/privateEndpointConnectionProxies/validate/action","display":{"provider":"Microsoft
+        Batch","resource":"PrivateEndpointConnectionProxies","operation":"Validates
+        a Private endpoint connection proxy","description":"Validates a Private endpoint
+        connection proxy on a Batch account"},"isDataAction":false,"origin":"system"},{"name":"Microsoft.Batch/batchAccounts/privateEndpointConnectionProxies/write","display":{"provider":"Microsoft
         Batch","resource":"PrivateEndpointConnectionProxies","operation":"Create or
         Update Private endpoint connection proxy","description":"Create a new Private
         endpoint connection proxy on a Batch account"},"isDataAction":false,"origin":"system"},{"name":"Microsoft.Batch/batchAccounts/privateEndpointConnectionProxies/read","display":{"provider":"Microsoft
         Batch","resource":"PrivateEndpointConnectionProxies","operation":"Get Private
         endpoint connection proxy","description":"Gets Private endpoint connection
+        proxy on a Batch account"},"isDataAction":false,"origin":"system"},{"name":"Microsoft.Batch/batchAccounts/privateEndpointConnectionProxies/delete","display":{"provider":"Microsoft
+        Batch","resource":"PrivateEndpointConnectionProxies","operation":"Delete Private
+        endpoint connection proxy","description":"Delete a Private endpoint connection
         proxy on a Batch account"},"isDataAction":false,"origin":"system"},{"name":"Microsoft.Batch/batchAccounts/privateEndpointConnectionProxyResults/read","display":{"provider":"Microsoft
         Batch","resource":"PrivateEndpointConnectionProxies","operation":"Get Batch
         account private endpoint connection proxy operation results","description":"Gets
         the results of a long running Batch account private endpoint connection proxy
         operation"},"isDataAction":false,"origin":"system"}]}'
     headers:
       cache-control:
       - no-cache
       content-length:
-      - '26529'
+      - '27226'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Fri, 10 Apr 2020 19:07:51 GMT
+      - Fri, 29 May 2020 03:19:45 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
```

## Comparing `azure-mgmt-batch-8.0.1/tests/recordings/test_mgmt_batch.test_mgmt_batch_byos_account.yaml` & `azure-mgmt-batch-9.0.0/tests/recordings/test_mgmt_batch.test_mgmt_batch_byos_account.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -5,30 +5,30 @@
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.11 msrest_azure/0.6.2
-        azure-mgmt-keyvault/2.1.1 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-keyvault/2.2.0 Azure-SDK-For-Python
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_byos_account94171201/providers/Microsoft.KeyVault/vaults/batchthagcx73omz5pmblb7s?api-version=2019-09-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_byos_account94171201/providers/Microsoft.KeyVault/vaults/batchxtk3agb5zuivqarycco?api-version=2019-09-01
   response:
     body:
-      string: '{"id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_byos_account94171201/providers/Microsoft.KeyVault/vaults/batchthagcx73omz5pmblb7s","name":"batchthagcx73omz5pmblb7s","type":"Microsoft.KeyVault/vaults","location":"westcentralus","tags":{},"properties":{"sku":{"family":"A","name":"standard"},"tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47","accessPolicies":[{"tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47","objectId":"f520d84c-3fd3-4cc8-88d4-2ed25b00d27a","permissions":{"keys":["all"],"secrets":["all"]}}],"enabledForDeployment":true,"enabledForDiskEncryption":true,"enabledForTemplateDeployment":true,"enableSoftDelete":true,"vaultUri":"https://batchthagcx73omz5pmblb7s.vault.azure.net/","provisioningState":"Succeeded"}}'
+      string: '{"id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_byos_account94171201/providers/Microsoft.KeyVault/vaults/batchxtk3agb5zuivqarycco","name":"batchxtk3agb5zuivqarycco","type":"Microsoft.KeyVault/vaults","location":"westcentralus","tags":{},"properties":{"sku":{"family":"A","name":"standard"},"tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47","accessPolicies":[{"tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47","objectId":"f520d84c-3fd3-4cc8-88d4-2ed25b00d27a","permissions":{"keys":["all"],"secrets":["all"]}}],"enabledForDeployment":true,"enabledForDiskEncryption":true,"enabledForTemplateDeployment":true,"enableSoftDelete":true,"vaultUri":"https://batchxtk3agb5zuivqarycco.vault.azure.net/","provisioningState":"Succeeded"}}'
     headers:
       cache-control:
       - no-cache
       content-length:
       - '784'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Fri, 10 Apr 2020 21:10:45 GMT
+      - Fri, 29 May 2020 03:11:00 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - Microsoft-IIS/10.0
       strict-transport-security:
@@ -38,15 +38,15 @@
       vary:
       - Accept-Encoding
       x-aspnet-version:
       - 4.0.30319
       x-content-type-options:
       - nosniff
       x-ms-keyvault-service-version:
-      - 1.1.0.276
+      - 1.1.0.281
       x-powered-by:
       - ASP.NET
     status:
       code: 200
       message: OK
 - request:
     body: '{"location": "westcentralus", "properties": {"poolAllocationMode": "UserSubscription",
@@ -59,132 +59,132 @@
       Connection:
       - keep-alive
       Content-Length:
       - '121'
       Content-Type:
       - application/json; charset=utf-8
       User-Agent:
-      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.11 msrest_azure/0.6.2
-        azure-mgmt-batch/2020-03-01 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: PUT
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_byos_account94171201/providers/Microsoft.Batch/batchAccounts/batch94171201?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_byos_account94171201/providers/Microsoft.Batch/batchAccounts/batch94171201?api-version=2020-05-01
   response:
     body:
       string: '{"error":{"code":"InvalidRequestBody","message":"The specified Request
-        Body is not syntactically valid.\nRequestId:c9d69eea-e73a-4155-ae8f-4e07654f8eb7\nTime:2020-04-10T21:10:47.9243110Z","target":"BatchAccount","details":[{"code":"Reason","message":"keyVaultReference
+        Body is not syntactically valid.\nRequestId:00fb2b02-6023-4a60-8135-ce46fb0bc585\nTime:2020-05-29T03:11:02.8471169Z","target":"BatchAccount","details":[{"code":"Reason","message":"keyVaultReference
         must be set if poolAllocationMode is specified as ''UserSubscription'' on
         a PUT request"}]}}'
     headers:
       cache-control:
       - no-cache
       content-length:
       - '359'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Fri, 10 Apr 2020 21:10:48 GMT
+      - Fri, 29 May 2020 03:11:03 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
       - max-age=31536000; includeSubDomains
       x-content-type-options:
       - nosniff
       x-ms-ratelimit-remaining-subscription-writes:
-      - '1198'
+      - '1199'
     status:
       code: 400
       message: The specified Request Body is not syntactically valid.
 - request:
     body: 'b''b\''{"location": "westcentralus", "properties": {"poolAllocationMode":
-      "UserSubscription", "keyVaultReference": {"id": "/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_byos_account94171201/providers/Microsoft.KeyVault/vaults/batchthagcx73omz5pmblb7s",
-      "url": "https://batchthagcx73omz5pmblb7s.vault.azure.net/"}, "publicNetworkAccess":
+      "UserSubscription", "keyVaultReference": {"id": "/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_byos_account94171201/providers/Microsoft.KeyVault/vaults/batchxtk3agb5zuivqarycco",
+      "url": "https://batchxtk3agb5zuivqarycco.vault.azure.net/"}, "publicNetworkAccess":
       "Enabled"}}\'''''
     headers:
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       Content-Length:
       - '394'
       Content-Type:
       - application/json; charset=utf-8
       User-Agent:
-      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.11 msrest_azure/0.6.2
-        azure-mgmt-batch/2020-03-01 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: PUT
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_byos_account94171201/providers/Microsoft.Batch/batchAccounts/batch94171201?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_byos_account94171201/providers/Microsoft.Batch/batchAccounts/batch94171201?api-version=2020-05-01
   response:
     body:
       string: ''
     headers:
       cache-control:
       - no-cache
       content-length:
       - '0'
       date:
-      - Fri, 10 Apr 2020 21:10:50 GMT
+      - Fri, 29 May 2020 03:11:05 GMT
       expires:
       - '-1'
       location:
-      - https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_byos_account94171201/providers/Microsoft.Batch/batchAccounts/batch94171201/operationResults/c690b77c-1b88-46f3-8aaf-ef625c431abb?api-version=2020-03-01
+      - https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_byos_account94171201/providers/Microsoft.Batch/batchAccounts/batch94171201/operationResults/8240d297-9c28-419e-98e6-0cc716099d34?api-version=2020-05-01
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
       - max-age=31536000; includeSubDomains
       x-content-type-options:
       - nosniff
       x-ms-ratelimit-remaining-subscription-writes:
-      - '1197'
+      - '1198'
     status:
       code: 202
       message: Accepted
 - request:
     body: null
     headers:
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.11 msrest_azure/0.6.2
-        azure-mgmt-batch/2020-03-01 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_byos_account94171201/providers/Microsoft.Batch/batchAccounts/batch94171201/operationResults/c690b77c-1b88-46f3-8aaf-ef625c431abb?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_byos_account94171201/providers/Microsoft.Batch/batchAccounts/batch94171201/operationResults/8240d297-9c28-419e-98e6-0cc716099d34?api-version=2020-05-01
   response:
     body:
-      string: '{"id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_byos_account94171201/providers/Microsoft.Batch/batchAccounts/batch94171201","name":"batch94171201","type":"Microsoft.Batch/batchAccounts","location":"westcentralus","properties":{"accountEndpoint":"batch94171201.westcentralus.batch.azure.com","provisioningState":"Succeeded","dedicatedCoreQuotaPerVMFamilyEnforced":false,"poolQuota":100,"activeJobAndJobScheduleQuota":300,"poolAllocationMode":"UserSubscription","keyVaultReference":{"id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_byos_account94171201/providers/Microsoft.KeyVault/vaults/batchthagcx73omz5pmblb7s","url":"https://batchthagcx73omz5pmblb7s.vault.azure.net/"},"publicNetworkAccess":"Enabled","encryption":{"keySource":"Microsoft.Batch"}}}'
+      string: '{"id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_byos_account94171201/providers/Microsoft.Batch/batchAccounts/batch94171201","name":"batch94171201","type":"Microsoft.Batch/batchAccounts","location":"westcentralus","properties":{"accountEndpoint":"batch94171201.westcentralus.batch.azure.com","provisioningState":"Succeeded","dedicatedCoreQuotaPerVMFamilyEnforced":false,"poolQuota":100,"activeJobAndJobScheduleQuota":300,"poolAllocationMode":"UserSubscription","keyVaultReference":{"id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_byos_account94171201/providers/Microsoft.KeyVault/vaults/batchxtk3agb5zuivqarycco","url":"https://batchxtk3agb5zuivqarycco.vault.azure.net/"},"publicNetworkAccess":"Enabled","encryption":{"keySource":"Microsoft.Batch"}},"identity":{"type":"None"}}'
     headers:
       cache-control:
       - no-cache
       content-length:
-      - '864'
+      - '891'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Fri, 10 Apr 2020 21:11:06 GMT
+      - Fri, 29 May 2020 03:11:29 GMT
       etag:
-      - '"0x8D7DD93AF02E362"'
+      - '"0x8D8037DFBFD84B7"'
       expires:
       - '-1'
       last-modified:
-      - Fri, 10 Apr 2020 21:11:06 GMT
+      - Fri, 29 May 2020 03:11:30 GMT
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
       - max-age=31536000; includeSubDomains
       transfer-encoding:
```

## Comparing `azure-mgmt-batch-8.0.1/tests/recordings/test_mgmt_batch.test_mgmt_batch_account.yaml` & `azure-mgmt-batch-9.0.0/tests/recordings/test_mgmt_batch.test_mgmt_batch_account.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -9,34 +9,34 @@
       Connection:
       - keep-alive
       Content-Length:
       - '79'
       Content-Type:
       - application/json; charset=utf-8
       User-Agent:
-      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.11 msrest_azure/0.6.2
-        azure-mgmt-batch/8.0.1 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: PUT
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_account3e1b0fe5/providers/Microsoft.Batch/batchAccounts/batch3e1b0fe5?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_account3e1b0fe5/providers/Microsoft.Batch/batchAccounts/batch3e1b0fe5?api-version=2020-05-01
   response:
     body:
       string: ''
     headers:
       cache-control:
       - no-cache
       content-length:
       - '0'
       date:
-      - Tue, 14 Apr 2020 15:36:58 GMT
+      - Fri, 29 May 2020 17:21:42 GMT
       expires:
       - '-1'
       location:
-      - https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_account3e1b0fe5/providers/Microsoft.Batch/batchAccounts/batch3e1b0fe5/operationResults/a4f17142-743a-4052-ba45-8b09bc57ba33?api-version=2020-03-01
+      - https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_account3e1b0fe5/providers/Microsoft.Batch/batchAccounts/batch3e1b0fe5/operationResults/e725ad4f-6cf4-48de-b64f-188476982eb9?api-version=2020-05-01
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
       - max-age=31536000; includeSubDomains
       x-content-type-options:
@@ -52,36 +52,36 @@
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.11 msrest_azure/0.6.2
-        azure-mgmt-batch/8.0.1 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_account3e1b0fe5/providers/Microsoft.Batch/batchAccounts/batch3e1b0fe5/operationResults/a4f17142-743a-4052-ba45-8b09bc57ba33?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_account3e1b0fe5/providers/Microsoft.Batch/batchAccounts/batch3e1b0fe5/operationResults/e725ad4f-6cf4-48de-b64f-188476982eb9?api-version=2020-05-01
   response:
     body:
-      string: '{"id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_account3e1b0fe5/providers/Microsoft.Batch/batchAccounts/batch3e1b0fe5","name":"batch3e1b0fe5","type":"Microsoft.Batch/batchAccounts","location":"westcentralus","properties":{"accountEndpoint":"batch3e1b0fe5.westcentralus.batch.azure.com","provisioningState":"Succeeded","dedicatedCoreQuota":0,"dedicatedCoreQuotaPerVMFamily":[{"name":"standardAv2Family","coreQuota":0},{"name":"standardDv2Family","coreQuota":0},{"name":"standardDv3Family","coreQuota":0},{"name":"standardEv3Family","coreQuota":0},{"name":"standardDSv2Family","coreQuota":0},{"name":"standardDSv3Family","coreQuota":0},{"name":"standardESv3Family","coreQuota":0},{"name":"standardFFamily","coreQuota":0},{"name":"standardFSFamily","coreQuota":0},{"name":"standardA0_A7Family","coreQuota":0},{"name":"standardA8_A11Family","coreQuota":0},{"name":"standardDFamily","coreQuota":0},{"name":"standardGFamily","coreQuota":0},{"name":"basicAFamily","coreQuota":0},{"name":"standardNVFamily","coreQuota":0},{"name":"standardNVPromoFamily","coreQuota":0},{"name":"standardNCFamily","coreQuota":0},{"name":"standardNCPromoFamily","coreQuota":0},{"name":"standardHFamily","coreQuota":0},{"name":"standardHPromoFamily","coreQuota":0},{"name":"standardMSFamily","coreQuota":0},{"name":"standardDSFamily","coreQuota":0},{"name":"standardGSFamily","coreQuota":0},{"name":"standardLSFamily","coreQuota":0},{"name":"standardNCSv2Family","coreQuota":0},{"name":"standardNDSFamily","coreQuota":0},{"name":"standardNCSv3Family","coreQuota":0},{"name":"standardFSv2Family","coreQuota":0},{"name":"standardHBSFamily","coreQuota":0},{"name":"standardHCSFamily","coreQuota":0},{"name":"standardNVSv3Family","coreQuota":0},{"name":"standardHBrsv2Family","coreQuota":0}],"dedicatedCoreQuotaPerVMFamilyEnforced":false,"lowPriorityCoreQuota":0,"poolQuota":100,"activeJobAndJobScheduleQuota":300,"poolAllocationMode":"BatchService","publicNetworkAccess":"Enabled","encryption":{"keySource":"Microsoft.Batch"}}}'
+      string: '{"id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_account3e1b0fe5/providers/Microsoft.Batch/batchAccounts/batch3e1b0fe5","name":"batch3e1b0fe5","type":"Microsoft.Batch/batchAccounts","location":"westcentralus","properties":{"accountEndpoint":"batch3e1b0fe5.westcentralus.batch.azure.com","provisioningState":"Succeeded","dedicatedCoreQuota":700,"dedicatedCoreQuotaPerVMFamily":[{"name":"standardAv2Family","coreQuota":100},{"name":"standardDv2Family","coreQuota":100},{"name":"standardDv3Family","coreQuota":100},{"name":"standardEv3Family","coreQuota":50},{"name":"standardDSv2Family","coreQuota":100},{"name":"standardDSv3Family","coreQuota":100},{"name":"standardESv3Family","coreQuota":50},{"name":"standardFFamily","coreQuota":50},{"name":"standardFSFamily","coreQuota":50},{"name":"standardA0_A7Family","coreQuota":0},{"name":"standardA8_A11Family","coreQuota":0},{"name":"standardDFamily","coreQuota":0},{"name":"standardGFamily","coreQuota":0},{"name":"basicAFamily","coreQuota":0},{"name":"standardNVFamily","coreQuota":0},{"name":"standardNVPromoFamily","coreQuota":0},{"name":"standardNCFamily","coreQuota":0},{"name":"standardNCPromoFamily","coreQuota":0},{"name":"standardHFamily","coreQuota":0},{"name":"standardHPromoFamily","coreQuota":0},{"name":"standardMSFamily","coreQuota":0},{"name":"standardDSFamily","coreQuota":0},{"name":"standardGSFamily","coreQuota":0},{"name":"standardLSFamily","coreQuota":0},{"name":"standardLSv2Family","coreQuota":0},{"name":"standardNCSv2Family","coreQuota":0},{"name":"standardNDSFamily","coreQuota":0},{"name":"standardNCSv3Family","coreQuota":0},{"name":"standardFSv2Family","coreQuota":0},{"name":"standardHBSFamily","coreQuota":0},{"name":"standardHCSFamily","coreQuota":0},{"name":"standardNVSv3Family","coreQuota":0},{"name":"standardHBrsv2Family","coreQuota":0},{"name":"standardDASv4Family","coreQuota":0},{"name":"standardEAv4Family","coreQuota":0},{"name":"standardEASv4Family","coreQuota":0}],"dedicatedCoreQuotaPerVMFamilyEnforced":false,"lowPriorityCoreQuota":500,"poolQuota":100,"activeJobAndJobScheduleQuota":300,"poolAllocationMode":"BatchService","publicNetworkAccess":"Enabled","encryption":{"keySource":"Microsoft.Batch"}},"identity":{"type":"None"}}'
     headers:
       cache-control:
       - no-cache
       content-length:
-      - '2054'
+      - '2277'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Tue, 14 Apr 2020 15:37:14 GMT
+      - Fri, 29 May 2020 17:21:59 GMT
       etag:
-      - '"0x8D7E089B54CE314"'
+      - '"0x8D803F4CB835E50"'
       expires:
       - '-1'
       last-modified:
-      - Tue, 14 Apr 2020 15:37:15 GMT
+      - Fri, 29 May 2020 17:21:59 GMT
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
       - max-age=31536000; includeSubDomains
       transfer-encoding:
@@ -99,38 +99,38 @@
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.11 msrest_azure/0.6.2
-        azure-mgmt-batch/8.0.1 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_account3e1b0fe5/providers/Microsoft.Batch/batchAccounts/batch3e1b0fe5?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_account3e1b0fe5/providers/Microsoft.Batch/batchAccounts/batch3e1b0fe5?api-version=2020-05-01
   response:
     body:
-      string: '{"id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_account3e1b0fe5/providers/Microsoft.Batch/batchAccounts/batch3e1b0fe5","name":"batch3e1b0fe5","type":"Microsoft.Batch/batchAccounts","location":"westcentralus","properties":{"accountEndpoint":"batch3e1b0fe5.westcentralus.batch.azure.com","provisioningState":"Succeeded","dedicatedCoreQuota":0,"dedicatedCoreQuotaPerVMFamily":[{"name":"standardAv2Family","coreQuota":0},{"name":"standardDv2Family","coreQuota":0},{"name":"standardDv3Family","coreQuota":0},{"name":"standardEv3Family","coreQuota":0},{"name":"standardDSv2Family","coreQuota":0},{"name":"standardDSv3Family","coreQuota":0},{"name":"standardESv3Family","coreQuota":0},{"name":"standardFFamily","coreQuota":0},{"name":"standardFSFamily","coreQuota":0},{"name":"standardA0_A7Family","coreQuota":0},{"name":"standardA8_A11Family","coreQuota":0},{"name":"standardDFamily","coreQuota":0},{"name":"standardGFamily","coreQuota":0},{"name":"basicAFamily","coreQuota":0},{"name":"standardNVFamily","coreQuota":0},{"name":"standardNVPromoFamily","coreQuota":0},{"name":"standardNCFamily","coreQuota":0},{"name":"standardNCPromoFamily","coreQuota":0},{"name":"standardHFamily","coreQuota":0},{"name":"standardHPromoFamily","coreQuota":0},{"name":"standardMSFamily","coreQuota":0},{"name":"standardDSFamily","coreQuota":0},{"name":"standardGSFamily","coreQuota":0},{"name":"standardLSFamily","coreQuota":0},{"name":"standardNCSv2Family","coreQuota":0},{"name":"standardNDSFamily","coreQuota":0},{"name":"standardNCSv3Family","coreQuota":0},{"name":"standardFSv2Family","coreQuota":0},{"name":"standardHBSFamily","coreQuota":0},{"name":"standardHCSFamily","coreQuota":0},{"name":"standardNVSv3Family","coreQuota":0},{"name":"standardHBrsv2Family","coreQuota":0}],"dedicatedCoreQuotaPerVMFamilyEnforced":false,"lowPriorityCoreQuota":0,"poolQuota":100,"activeJobAndJobScheduleQuota":300,"poolAllocationMode":"BatchService","publicNetworkAccess":"Enabled","encryption":{"keySource":"Microsoft.Batch"}}}'
+      string: '{"id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_account3e1b0fe5/providers/Microsoft.Batch/batchAccounts/batch3e1b0fe5","name":"batch3e1b0fe5","type":"Microsoft.Batch/batchAccounts","location":"westcentralus","properties":{"accountEndpoint":"batch3e1b0fe5.westcentralus.batch.azure.com","provisioningState":"Succeeded","dedicatedCoreQuota":700,"dedicatedCoreQuotaPerVMFamily":[{"name":"standardAv2Family","coreQuota":100},{"name":"standardDv2Family","coreQuota":100},{"name":"standardDv3Family","coreQuota":100},{"name":"standardEv3Family","coreQuota":50},{"name":"standardDSv2Family","coreQuota":100},{"name":"standardDSv3Family","coreQuota":100},{"name":"standardESv3Family","coreQuota":50},{"name":"standardFFamily","coreQuota":50},{"name":"standardFSFamily","coreQuota":50},{"name":"standardA0_A7Family","coreQuota":0},{"name":"standardA8_A11Family","coreQuota":0},{"name":"standardDFamily","coreQuota":0},{"name":"standardGFamily","coreQuota":0},{"name":"basicAFamily","coreQuota":0},{"name":"standardNVFamily","coreQuota":0},{"name":"standardNVPromoFamily","coreQuota":0},{"name":"standardNCFamily","coreQuota":0},{"name":"standardNCPromoFamily","coreQuota":0},{"name":"standardHFamily","coreQuota":0},{"name":"standardHPromoFamily","coreQuota":0},{"name":"standardMSFamily","coreQuota":0},{"name":"standardDSFamily","coreQuota":0},{"name":"standardGSFamily","coreQuota":0},{"name":"standardLSFamily","coreQuota":0},{"name":"standardLSv2Family","coreQuota":0},{"name":"standardNCSv2Family","coreQuota":0},{"name":"standardNDSFamily","coreQuota":0},{"name":"standardNCSv3Family","coreQuota":0},{"name":"standardFSv2Family","coreQuota":0},{"name":"standardHBSFamily","coreQuota":0},{"name":"standardHCSFamily","coreQuota":0},{"name":"standardNVSv3Family","coreQuota":0},{"name":"standardHBrsv2Family","coreQuota":0},{"name":"standardDASv4Family","coreQuota":0},{"name":"standardEAv4Family","coreQuota":0},{"name":"standardEASv4Family","coreQuota":0}],"dedicatedCoreQuotaPerVMFamilyEnforced":false,"lowPriorityCoreQuota":500,"poolQuota":100,"activeJobAndJobScheduleQuota":300,"poolAllocationMode":"BatchService","publicNetworkAccess":"Enabled","encryption":{"keySource":"Microsoft.Batch"}},"identity":{"type":"None"}}'
     headers:
       cache-control:
       - no-cache
       content-length:
-      - '2054'
+      - '2277'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Tue, 14 Apr 2020 15:37:14 GMT
+      - Fri, 29 May 2020 17:21:59 GMT
       etag:
-      - '"0x8D7E089ABE20AF0"'
+      - '"0x8D803F4C43800DC"'
       expires:
       - '-1'
       last-modified:
-      - Tue, 14 Apr 2020 15:36:59 GMT
+      - Fri, 29 May 2020 17:21:47 GMT
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
       - max-age=31536000; includeSubDomains
       transfer-encoding:
@@ -148,32 +148,32 @@
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.11 msrest_azure/0.6.2
-        azure-mgmt-batch/8.0.1 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_account3e1b0fe5/providers/Microsoft.Batch/batchAccounts?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_account3e1b0fe5/providers/Microsoft.Batch/batchAccounts?api-version=2020-05-01
   response:
     body:
-      string: '{"value":[{"id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_account3e1b0fe5/providers/Microsoft.Batch/batchAccounts/batch3e1b0fe5","name":"batch3e1b0fe5","type":"Microsoft.Batch/batchAccounts","location":"westcentralus","properties":{"accountEndpoint":"batch3e1b0fe5.westcentralus.batch.azure.com","provisioningState":"Succeeded","dedicatedCoreQuota":0,"dedicatedCoreQuotaPerVMFamily":[{"name":"standardAv2Family","coreQuota":0},{"name":"standardDv2Family","coreQuota":0},{"name":"standardDv3Family","coreQuota":0},{"name":"standardEv3Family","coreQuota":0},{"name":"standardDSv2Family","coreQuota":0},{"name":"standardDSv3Family","coreQuota":0},{"name":"standardESv3Family","coreQuota":0},{"name":"standardFFamily","coreQuota":0},{"name":"standardFSFamily","coreQuota":0},{"name":"standardA0_A7Family","coreQuota":0},{"name":"standardA8_A11Family","coreQuota":0},{"name":"standardDFamily","coreQuota":0},{"name":"standardGFamily","coreQuota":0},{"name":"basicAFamily","coreQuota":0},{"name":"standardNVFamily","coreQuota":0},{"name":"standardNVPromoFamily","coreQuota":0},{"name":"standardNCFamily","coreQuota":0},{"name":"standardNCPromoFamily","coreQuota":0},{"name":"standardHFamily","coreQuota":0},{"name":"standardHPromoFamily","coreQuota":0},{"name":"standardMSFamily","coreQuota":0},{"name":"standardDSFamily","coreQuota":0},{"name":"standardGSFamily","coreQuota":0},{"name":"standardLSFamily","coreQuota":0},{"name":"standardNCSv2Family","coreQuota":0},{"name":"standardNDSFamily","coreQuota":0},{"name":"standardNCSv3Family","coreQuota":0},{"name":"standardFSv2Family","coreQuota":0},{"name":"standardHBSFamily","coreQuota":0},{"name":"standardHCSFamily","coreQuota":0},{"name":"standardNVSv3Family","coreQuota":0},{"name":"standardHBrsv2Family","coreQuota":0}],"dedicatedCoreQuotaPerVMFamilyEnforced":false,"lowPriorityCoreQuota":0,"poolQuota":100,"activeJobAndJobScheduleQuota":300,"poolAllocationMode":"BatchService","publicNetworkAccess":"Enabled","encryption":{"keySource":"Microsoft.Batch"}}}]}'
+      string: '{"value":[{"id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_account3e1b0fe5/providers/Microsoft.Batch/batchAccounts/batch3e1b0fe5","name":"batch3e1b0fe5","type":"Microsoft.Batch/batchAccounts","location":"westcentralus","properties":{"accountEndpoint":"batch3e1b0fe5.westcentralus.batch.azure.com","provisioningState":"Succeeded","dedicatedCoreQuota":700,"dedicatedCoreQuotaPerVMFamily":[{"name":"standardAv2Family","coreQuota":100},{"name":"standardDv2Family","coreQuota":100},{"name":"standardDv3Family","coreQuota":100},{"name":"standardEv3Family","coreQuota":50},{"name":"standardDSv2Family","coreQuota":100},{"name":"standardDSv3Family","coreQuota":100},{"name":"standardESv3Family","coreQuota":50},{"name":"standardFFamily","coreQuota":50},{"name":"standardFSFamily","coreQuota":50},{"name":"standardA0_A7Family","coreQuota":0},{"name":"standardA8_A11Family","coreQuota":0},{"name":"standardDFamily","coreQuota":0},{"name":"standardGFamily","coreQuota":0},{"name":"basicAFamily","coreQuota":0},{"name":"standardNVFamily","coreQuota":0},{"name":"standardNVPromoFamily","coreQuota":0},{"name":"standardNCFamily","coreQuota":0},{"name":"standardNCPromoFamily","coreQuota":0},{"name":"standardHFamily","coreQuota":0},{"name":"standardHPromoFamily","coreQuota":0},{"name":"standardMSFamily","coreQuota":0},{"name":"standardDSFamily","coreQuota":0},{"name":"standardGSFamily","coreQuota":0},{"name":"standardLSFamily","coreQuota":0},{"name":"standardLSv2Family","coreQuota":0},{"name":"standardNCSv2Family","coreQuota":0},{"name":"standardNDSFamily","coreQuota":0},{"name":"standardNCSv3Family","coreQuota":0},{"name":"standardFSv2Family","coreQuota":0},{"name":"standardHBSFamily","coreQuota":0},{"name":"standardHCSFamily","coreQuota":0},{"name":"standardNVSv3Family","coreQuota":0},{"name":"standardHBrsv2Family","coreQuota":0},{"name":"standardDASv4Family","coreQuota":0},{"name":"standardEAv4Family","coreQuota":0},{"name":"standardEASv4Family","coreQuota":0}],"dedicatedCoreQuotaPerVMFamilyEnforced":false,"lowPriorityCoreQuota":500,"poolQuota":100,"activeJobAndJobScheduleQuota":300,"poolAllocationMode":"BatchService","publicNetworkAccess":"Enabled","encryption":{"keySource":"Microsoft.Batch"}},"identity":{"type":"None"}}]}'
     headers:
       cache-control:
       - no-cache
       content-length:
-      - '2066'
+      - '2289'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Tue, 14 Apr 2020 15:37:14 GMT
+      - Fri, 29 May 2020 17:21:59 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
@@ -195,32 +195,32 @@
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       Content-Length:
       - '0'
       User-Agent:
-      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.11 msrest_azure/0.6.2
-        azure-mgmt-batch/8.0.1 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: POST
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_account3e1b0fe5/providers/Microsoft.Batch/batchAccounts/batch3e1b0fe5/listKeys?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_account3e1b0fe5/providers/Microsoft.Batch/batchAccounts/batch3e1b0fe5/listKeys?api-version=2020-05-01
   response:
     body:
-      string: '{"accountName":"batch3e1b0fe5","primary":"+TotCbnKwezopOqQLBkSBt8+6luiAzUmr/2TB4I29h9txnHCFL027szjj7Eo10/kRYD/uH46oZoTVz7EgCDotw==","secondary":"85KlXkMDdlZv3co1wiG1yjwYsj2YbIsObRkaQuGIVbb+s8wxQPwX+evoJ55NPEHjjMefX/I2w8Zev/2h5euc4g=="}'
+      string: '{"accountName":"batch3e1b0fe5","primary":"5oGT4STJ/ZMDakHJT8dDugSqtJ++6rDV9rlAk3OqXTOVDG/uoiyzJ9xSEFIOH0p8X9MHMQKSvubn1BF1MjC/Kg==","secondary":"D5J5LV2W08Lnh9cxltCXg1qjzxYpk2RFoXQs4jP/BkyFrSvNTlf7aAPNjq+Xsc//CpP2k9cZyge0GbF23d5KSQ=="}'
     headers:
       cache-control:
       - no-cache
       content-length:
       - '235'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Tue, 14 Apr 2020 15:37:14 GMT
+      - Fri, 29 May 2020 17:22:00 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
@@ -246,32 +246,32 @@
       Connection:
       - keep-alive
       Content-Length:
       - '24'
       Content-Type:
       - application/json; charset=utf-8
       User-Agent:
-      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.11 msrest_azure/0.6.2
-        azure-mgmt-batch/8.0.1 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: POST
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_account3e1b0fe5/providers/Microsoft.Batch/batchAccounts/batch3e1b0fe5/regenerateKeys?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_account3e1b0fe5/providers/Microsoft.Batch/batchAccounts/batch3e1b0fe5/regenerateKeys?api-version=2020-05-01
   response:
     body:
-      string: '{"accountName":"batch3e1b0fe5","primary":"+TotCbnKwezopOqQLBkSBt8+6luiAzUmr/2TB4I29h9txnHCFL027szjj7Eo10/kRYD/uH46oZoTVz7EgCDotw==","secondary":"muz4FMDwClx0yCr9c+3sp4w26epWlr3eylUNpceTZYk32zuLHvZZ277LaxWPh908mn8e+lrKmvKqtFcLEFga/A=="}'
+      string: '{"accountName":"batch3e1b0fe5","primary":"5oGT4STJ/ZMDakHJT8dDugSqtJ++6rDV9rlAk3OqXTOVDG/uoiyzJ9xSEFIOH0p8X9MHMQKSvubn1BF1MjC/Kg==","secondary":"OU+dyj7ae9N6aJzDWJDkOVTM/8RN9KB/fc08TWCkjUKmIr6x49v9Mvq/W/Q4TnEqWrRzezMgONPPbU2VWqtxkQ=="}'
     headers:
       cache-control:
       - no-cache
       content-length:
       - '235'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Tue, 14 Apr 2020 15:37:14 GMT
+      - Fri, 29 May 2020 17:22:00 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
@@ -297,38 +297,38 @@
       Connection:
       - keep-alive
       Content-Length:
       - '50'
       Content-Type:
       - application/json; charset=utf-8
       User-Agent:
-      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.11 msrest_azure/0.6.2
-        azure-mgmt-batch/8.0.1 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: PATCH
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_account3e1b0fe5/providers/Microsoft.Batch/batchAccounts/batch3e1b0fe5?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_account3e1b0fe5/providers/Microsoft.Batch/batchAccounts/batch3e1b0fe5?api-version=2020-05-01
   response:
     body:
-      string: '{"id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_account3e1b0fe5/providers/Microsoft.Batch/batchAccounts/batch3e1b0fe5","name":"batch3e1b0fe5","type":"Microsoft.Batch/batchAccounts","location":"westcentralus","properties":{"accountEndpoint":"batch3e1b0fe5.westcentralus.batch.azure.com","provisioningState":"Succeeded","dedicatedCoreQuota":0,"dedicatedCoreQuotaPerVMFamily":[{"name":"standardAv2Family","coreQuota":0},{"name":"standardDv2Family","coreQuota":0},{"name":"standardDv3Family","coreQuota":0},{"name":"standardEv3Family","coreQuota":0},{"name":"standardDSv2Family","coreQuota":0},{"name":"standardDSv3Family","coreQuota":0},{"name":"standardESv3Family","coreQuota":0},{"name":"standardFFamily","coreQuota":0},{"name":"standardFSFamily","coreQuota":0},{"name":"standardA0_A7Family","coreQuota":0},{"name":"standardA8_A11Family","coreQuota":0},{"name":"standardDFamily","coreQuota":0},{"name":"standardGFamily","coreQuota":0},{"name":"basicAFamily","coreQuota":0},{"name":"standardNVFamily","coreQuota":0},{"name":"standardNVPromoFamily","coreQuota":0},{"name":"standardNCFamily","coreQuota":0},{"name":"standardNCPromoFamily","coreQuota":0},{"name":"standardHFamily","coreQuota":0},{"name":"standardHPromoFamily","coreQuota":0},{"name":"standardMSFamily","coreQuota":0},{"name":"standardDSFamily","coreQuota":0},{"name":"standardGSFamily","coreQuota":0},{"name":"standardLSFamily","coreQuota":0},{"name":"standardNCSv2Family","coreQuota":0},{"name":"standardNDSFamily","coreQuota":0},{"name":"standardNCSv3Family","coreQuota":0},{"name":"standardFSv2Family","coreQuota":0},{"name":"standardHBSFamily","coreQuota":0},{"name":"standardHCSFamily","coreQuota":0},{"name":"standardNVSv3Family","coreQuota":0},{"name":"standardHBrsv2Family","coreQuota":0}],"dedicatedCoreQuotaPerVMFamilyEnforced":false,"lowPriorityCoreQuota":0,"poolQuota":100,"activeJobAndJobScheduleQuota":300,"poolAllocationMode":"BatchService","publicNetworkAccess":"Enabled","encryption":{"keySource":"Microsoft.Batch"}},"tags":{"Name":"tagName","Value":"tagValue"}}'
+      string: '{"id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_account3e1b0fe5/providers/Microsoft.Batch/batchAccounts/batch3e1b0fe5","name":"batch3e1b0fe5","type":"Microsoft.Batch/batchAccounts","location":"westcentralus","properties":{"accountEndpoint":"batch3e1b0fe5.westcentralus.batch.azure.com","provisioningState":"Succeeded","dedicatedCoreQuota":700,"dedicatedCoreQuotaPerVMFamily":[{"name":"standardAv2Family","coreQuota":100},{"name":"standardDv2Family","coreQuota":100},{"name":"standardDv3Family","coreQuota":100},{"name":"standardEv3Family","coreQuota":50},{"name":"standardDSv2Family","coreQuota":100},{"name":"standardDSv3Family","coreQuota":100},{"name":"standardESv3Family","coreQuota":50},{"name":"standardFFamily","coreQuota":50},{"name":"standardFSFamily","coreQuota":50},{"name":"standardA0_A7Family","coreQuota":0},{"name":"standardA8_A11Family","coreQuota":0},{"name":"standardDFamily","coreQuota":0},{"name":"standardGFamily","coreQuota":0},{"name":"basicAFamily","coreQuota":0},{"name":"standardNVFamily","coreQuota":0},{"name":"standardNVPromoFamily","coreQuota":0},{"name":"standardNCFamily","coreQuota":0},{"name":"standardNCPromoFamily","coreQuota":0},{"name":"standardHFamily","coreQuota":0},{"name":"standardHPromoFamily","coreQuota":0},{"name":"standardMSFamily","coreQuota":0},{"name":"standardDSFamily","coreQuota":0},{"name":"standardGSFamily","coreQuota":0},{"name":"standardLSFamily","coreQuota":0},{"name":"standardLSv2Family","coreQuota":0},{"name":"standardNCSv2Family","coreQuota":0},{"name":"standardNDSFamily","coreQuota":0},{"name":"standardNCSv3Family","coreQuota":0},{"name":"standardFSv2Family","coreQuota":0},{"name":"standardHBSFamily","coreQuota":0},{"name":"standardHCSFamily","coreQuota":0},{"name":"standardNVSv3Family","coreQuota":0},{"name":"standardHBrsv2Family","coreQuota":0},{"name":"standardDASv4Family","coreQuota":0},{"name":"standardEAv4Family","coreQuota":0},{"name":"standardEASv4Family","coreQuota":0}],"dedicatedCoreQuotaPerVMFamilyEnforced":false,"lowPriorityCoreQuota":500,"poolQuota":100,"activeJobAndJobScheduleQuota":300,"poolAllocationMode":"BatchService","publicNetworkAccess":"Enabled","encryption":{"keySource":"Microsoft.Batch"}},"tags":{"Name":"tagName","Value":"tagValue"},"identity":{"type":"None"}}'
     headers:
       cache-control:
       - no-cache
       content-length:
-      - '2099'
+      - '2322'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Tue, 14 Apr 2020 15:37:16 GMT
+      - Fri, 29 May 2020 17:22:01 GMT
       etag:
-      - '"0x8D7E089B62AB538"'
+      - '"0x8D803F4CCA912C1"'
       expires:
       - '-1'
       last-modified:
-      - Tue, 14 Apr 2020 15:37:16 GMT
+      - Fri, 29 May 2020 17:22:01 GMT
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
       - max-age=31536000; includeSubDomains
       transfer-encoding:
@@ -350,34 +350,34 @@
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       Content-Length:
       - '0'
       User-Agent:
-      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.11 msrest_azure/0.6.2
-        azure-mgmt-batch/8.0.1 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: DELETE
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_account3e1b0fe5/providers/Microsoft.Batch/batchAccounts/batch3e1b0fe5?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_account3e1b0fe5/providers/Microsoft.Batch/batchAccounts/batch3e1b0fe5?api-version=2020-05-01
   response:
     body:
       string: ''
     headers:
       cache-control:
       - no-cache
       content-length:
       - '0'
       date:
-      - Tue, 14 Apr 2020 15:37:16 GMT
+      - Fri, 29 May 2020 17:22:02 GMT
       expires:
       - '-1'
       location:
-      - https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.Batch/locations/westcentralus/accountOperationResults/batch3e1b0fe5-1495797e-f9af-436d-ad44-ec39195f19a5?api-version=2020-03-01
+      - https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.Batch/locations/westcentralus/accountOperationResults/batch3e1b0fe5-578db4e6-933d-45c3-b66e-2bac82d319cc?api-version=2020-05-01
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
       - max-age=31536000; includeSubDomains
       x-content-type-options:
@@ -393,28 +393,28 @@
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.11 msrest_azure/0.6.2
-        azure-mgmt-batch/8.0.1 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.Batch/locations/westcentralus/accountOperationResults/batch3e1b0fe5-1495797e-f9af-436d-ad44-ec39195f19a5?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.Batch/locations/westcentralus/accountOperationResults/batch3e1b0fe5-578db4e6-933d-45c3-b66e-2bac82d319cc?api-version=2020-05-01
   response:
     body:
       string: ''
     headers:
       cache-control:
       - no-cache
       content-length:
       - '0'
       date:
-      - Tue, 14 Apr 2020 15:37:32 GMT
+      - Fri, 29 May 2020 17:22:17 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
```

## Comparing `azure-mgmt-batch-8.0.1/tests/recordings/test_mgmt_batch.test_mgmt_batch_applications.yaml` & `azure-mgmt-batch-9.0.0/tests/recordings/test_mgmt_batch.test_mgmt_batch_applications.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,88 +1,89 @@
 interactions:
 - request:
     body: 'b''b\''b\\\''{"location": "westcentralus", "properties": {"autoStorage":
-      {"storageAccountId": "/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Storage/storageAccounts/batch93ef11ff"}}}\\\''\'''''
+      {"storageAccountId": "/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Storage/storageAccounts/batch"},
+      "publicNetworkAccess": "Enabled"}}\\\''\'''''
     headers:
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       Content-Length:
-      - '263'
+      - '297'
       Content-Type:
       - application/json; charset=utf-8
       User-Agent:
-      - python/3.6.6 (Windows-10-10.0.14393-SP0) msrest/0.6.9 msrest_azure/0.4.34
-        azure-mgmt-batch/7.0.0 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: PUT
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch93ef11ff?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch93ef11ff?api-version=2020-05-01
   response:
     body:
       string: ''
     headers:
       cache-control:
       - no-cache
       content-length:
       - '0'
       date:
-      - Tue, 06 Aug 2019 23:08:03 GMT
+      - Fri, 29 May 2020 03:09:39 GMT
       expires:
       - '-1'
       location:
-      - https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch93ef11ff/operationResults/918bbd5e-21a4-4955-9607-e269a0642d16?api-version=2020-03-01
+      - https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch93ef11ff/operationResults/071e7246-031e-4457-aded-d84fa18294bc?api-version=2020-05-01
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
       - max-age=31536000; includeSubDomains
       x-content-type-options:
       - nosniff
       x-ms-ratelimit-remaining-subscription-writes:
-      - '1199'
+      - '1198'
     status:
       code: 202
       message: Accepted
 - request:
     body: null
     headers:
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.6.6 (Windows-10-10.0.14393-SP0) msrest/0.6.9 msrest_azure/0.4.34
-        azure-mgmt-batch/7.0.0 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch93ef11ff/operationResults/918bbd5e-21a4-4955-9607-e269a0642d16?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch93ef11ff/operationResults/071e7246-031e-4457-aded-d84fa18294bc?api-version=2020-05-01
   response:
     body:
-      string: '{"id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch93ef11ff","name":"batch93ef11ff","type":"Microsoft.Batch/batchAccounts","location":"westcentralus","properties":{"accountEndpoint":"batch93ef11ff.westcentralus.batch.azure.com","provisioningState":"Succeeded","dedicatedCoreQuota":700,"dedicatedCoreQuotaPerVMFamily":[{"name":"standardAv2Family","coreQuota":100},{"name":"standardDv2Family","coreQuota":100},{"name":"standardDv3Family","coreQuota":100},{"name":"standardEv3Family","coreQuota":50},{"name":"standardDSv2Family","coreQuota":100},{"name":"standardDSv3Family","coreQuota":100},{"name":"standardESv3Family","coreQuota":50},{"name":"standardFFamily","coreQuota":50},{"name":"standardFSFamily","coreQuota":50},{"name":"standardA0_A7Family","coreQuota":0},{"name":"standardA8_A11Family","coreQuota":0},{"name":"standardDFamily","coreQuota":0},{"name":"standardGFamily","coreQuota":0},{"name":"basicAFamily","coreQuota":0},{"name":"standardNVFamily","coreQuota":0},{"name":"standardNVPromoFamily","coreQuota":0},{"name":"standardNCFamily","coreQuota":0},{"name":"standardNCPromoFamily","coreQuota":0},{"name":"standardHFamily","coreQuota":0},{"name":"standardHPromoFamily","coreQuota":0},{"name":"standardMSFamily","coreQuota":0},{"name":"standardDSFamily","coreQuota":0},{"name":"standardGSFamily","coreQuota":0},{"name":"standardLSFamily","coreQuota":0},{"name":"standardNCSv2Family","coreQuota":0},{"name":"standardNDSFamily","coreQuota":0},{"name":"standardNCSv3Family","coreQuota":0},{"name":"standardFSv2Family","coreQuota":0},{"name":"standardHBSFamily","coreQuota":0},{"name":"standardHCSFamily","coreQuota":0}],"dedicatedCoreQuotaPerVMFamilyEnforced":false,"lowPriorityCoreQuota":500,"poolQuota":100,"activeJobAndJobScheduleQuota":300,"autoStorage":{"storageAccountId":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Storage/storageAccounts/batch93ef11ff","lastKeySync":"2019-08-06T23:08:03.7821041Z"},"poolAllocationMode":"BatchService"}}'
+      string: '{"id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch","name":"batch","type":"Microsoft.Batch/batchAccounts","location":"westcentralus","properties":{"accountEndpoint":"batch.westcentralus.batch.azure.com","provisioningState":"Succeeded","dedicatedCoreQuota":700,"dedicatedCoreQuotaPerVMFamily":[{"name":"standardAv2Family","coreQuota":100},{"name":"standardDv2Family","coreQuota":100},{"name":"standardDv3Family","coreQuota":100},{"name":"standardEv3Family","coreQuota":50},{"name":"standardDSv2Family","coreQuota":100},{"name":"standardDSv3Family","coreQuota":100},{"name":"standardESv3Family","coreQuota":50},{"name":"standardFFamily","coreQuota":50},{"name":"standardFSFamily","coreQuota":50},{"name":"standardA0_A7Family","coreQuota":0},{"name":"standardA8_A11Family","coreQuota":0},{"name":"standardDFamily","coreQuota":0},{"name":"standardGFamily","coreQuota":0},{"name":"basicAFamily","coreQuota":0},{"name":"standardNVFamily","coreQuota":0},{"name":"standardNVPromoFamily","coreQuota":0},{"name":"standardNCFamily","coreQuota":0},{"name":"standardNCPromoFamily","coreQuota":0},{"name":"standardHFamily","coreQuota":0},{"name":"standardHPromoFamily","coreQuota":0},{"name":"standardMSFamily","coreQuota":0},{"name":"standardDSFamily","coreQuota":0},{"name":"standardGSFamily","coreQuota":0},{"name":"standardLSFamily","coreQuota":0},{"name":"standardLSv2Family","coreQuota":0},{"name":"standardNCSv2Family","coreQuota":0},{"name":"standardNDSFamily","coreQuota":0},{"name":"standardNCSv3Family","coreQuota":0},{"name":"standardFSv2Family","coreQuota":0},{"name":"standardHBSFamily","coreQuota":0},{"name":"standardHCSFamily","coreQuota":0},{"name":"standardNVSv3Family","coreQuota":0},{"name":"standardHBrsv2Family","coreQuota":0},{"name":"standardDASv4Family","coreQuota":0},{"name":"standardEAv4Family","coreQuota":0},{"name":"standardEASv4Family","coreQuota":0}],"dedicatedCoreQuotaPerVMFamilyEnforced":false,"lowPriorityCoreQuota":500,"poolQuota":100,"activeJobAndJobScheduleQuota":300,"autoStorage":{"storageAccountId":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Storage/storageAccounts/batch","lastKeySync":"2020-05-29T03:09:39.4645207Z"},"poolAllocationMode":"BatchService","publicNetworkAccess":"Enabled","encryption":{"keySource":"Microsoft.Batch"}},"identity":{"type":"None"}}'
     headers:
       cache-control:
       - no-cache
       content-length:
-      - '2169'
+      - '2542'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Tue, 06 Aug 2019 23:08:19 GMT
+      - Fri, 29 May 2020 03:09:54 GMT
       etag:
-      - '"0x8D71AC2F8C9C715"'
+      - '"0x8D8037DC34DFE60"'
       expires:
       - '-1'
       last-modified:
-      - Tue, 06 Aug 2019 23:08:19 GMT
+      - Fri, 29 May 2020 03:09:55 GMT
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
       - max-age=31536000; includeSubDomains
       transfer-encoding:
@@ -102,28 +103,28 @@
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       Content-Length:
       - '0'
       User-Agent:
-      - python/3.6.6 (Windows-10-10.0.14393-SP0) msrest/0.6.9 msrest_azure/0.4.34
-        azure-mgmt-batch/7.0.0 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: POST
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch93ef11ff/syncAutoStorageKeys?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch93ef11ff/syncAutoStorageKeys?api-version=2020-05-01
   response:
     body:
       string: ''
     headers:
       cache-control:
       - no-cache
       date:
-      - Tue, 06 Aug 2019 23:08:20 GMT
+      - Fri, 29 May 2020 03:09:55 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
@@ -145,89 +146,89 @@
       Connection:
       - keep-alive
       Content-Length:
       - '76'
       Content-Type:
       - application/json; charset=utf-8
       User-Agent:
-      - python/3.6.6 (Windows-10-10.0.14393-SP0) msrest/0.6.9 msrest_azure/0.4.34
-        azure-mgmt-batch/7.0.0 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: PUT
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch93ef11ff/applications/my_application_id?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch93ef11ff/applications/my_application_id?api-version=2020-05-01
   response:
     body:
-      string: '{"type":"Microsoft.Batch/batchAccounts/applications","id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch93ef11ff/applications/my_application_id","name":"my_application_id","etag":"W/\"0x8D71AC2F94CC825\"","properties":{"displayName":"my_application_name","allowUpdates":true}}'
+      string: '{"type":"Microsoft.Batch/batchAccounts/applications","id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch93ef11ff/applications/my_application_id","name":"my_application_id","etag":"W/\"0x8D8037DC3CF7842\"","properties":{"displayName":"my_application_name","allowUpdates":true}}'
     headers:
       cache-control:
       - no-cache
       content-length:
       - '396'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Tue, 06 Aug 2019 23:08:20 GMT
+      - Fri, 29 May 2020 03:09:55 GMT
       etag:
-      - W/"0x8D71AC2F94CC825"
+      - W/"0x8D8037DC3CF7842"
       expires:
       - '-1'
       last-modified:
-      - Tue, 06 Aug 2019 23:08:20 GMT
+      - Fri, 29 May 2020 03:09:56 GMT
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
       - max-age=31536000; includeSubDomains
       transfer-encoding:
       - chunked
       vary:
       - Accept-Encoding
       x-content-type-options:
       - nosniff
       x-ms-ratelimit-remaining-subscription-writes:
-      - '1198'
+      - '1197'
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers:
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.6.6 (Windows-10-10.0.14393-SP0) msrest/0.6.9 msrest_azure/0.4.34
-        azure-mgmt-batch/7.0.0 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch93ef11ff/applications/my_application_id?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch93ef11ff/applications/my_application_id?api-version=2020-05-01
   response:
     body:
-      string: '{"type":"Microsoft.Batch/batchAccounts/applications","id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch93ef11ff/applications/my_application_id","name":"my_application_id","etag":"W/\"0x8D71AC2F94CC825\"","properties":{"displayName":"my_application_name","allowUpdates":true}}'
+      string: '{"type":"Microsoft.Batch/batchAccounts/applications","id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch93ef11ff/applications/my_application_id","name":"my_application_id","etag":"W/\"0x8D8037DC3CF7842\"","properties":{"displayName":"my_application_name","allowUpdates":true}}'
     headers:
       cache-control:
       - no-cache
       content-length:
       - '396'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Tue, 06 Aug 2019 23:08:21 GMT
+      - Fri, 29 May 2020 03:09:55 GMT
       etag:
-      - W/"0x8D71AC2F94CC825"
+      - W/"0x8D8037DC3CF7842"
       expires:
       - '-1'
       last-modified:
-      - Tue, 06 Aug 2019 23:08:20 GMT
+      - Fri, 29 May 2020 03:09:56 GMT
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
       - max-age=31536000; includeSubDomains
       transfer-encoding:
@@ -245,32 +246,32 @@
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.6.6 (Windows-10-10.0.14393-SP0) msrest/0.6.9 msrest_azure/0.4.34
-        azure-mgmt-batch/7.0.0 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch93ef11ff/applications?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch93ef11ff/applications?api-version=2020-05-01
   response:
     body:
-      string: '{"value":[{"type":"Microsoft.Batch/batchAccounts/applications","id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch93ef11ff/applications/my_application_id","name":"my_application_id","etag":"W/\"0x8D71AC2F94CC825\"","properties":{"displayName":"my_application_name","allowUpdates":true}}]}'
+      string: '{"value":[{"type":"Microsoft.Batch/batchAccounts/applications","id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch93ef11ff/applications/my_application_id","name":"my_application_id","etag":"W/\"0x8D8037DC3CF7842\"","properties":{"displayName":"my_application_name","allowUpdates":true}}]}'
     headers:
       cache-control:
       - no-cache
       content-length:
       - '408'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Tue, 06 Aug 2019 23:08:21 GMT
+      - Fri, 29 May 2020 03:09:56 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
@@ -294,52 +295,52 @@
       Connection:
       - keep-alive
       Content-Length:
       - '0'
       Content-Type:
       - application/json; charset=utf-8
       User-Agent:
-      - python/3.6.6 (Windows-10-10.0.14393-SP0) msrest/0.6.9 msrest_azure/0.4.34
-        azure-mgmt-batch/7.0.0 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: PUT
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch93ef11ff/applications/my_application_id/versions/v1.0?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch93ef11ff/applications/my_application_id/versions/v1.0?api-version=2020-05-01
   response:
     body:
-      string: '{"type":"Microsoft.Batch/batchAccounts/applications/versions","id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch93ef11ff/applications/my_application_id/versions/v1.0","name":"v1.0","etag":"W/\"0x8D71AC2F9F35F71\"","properties":{"storageUrl":"https://batch93ef11ff.blob.core.windows.net/app-my-application-id-b9dfc2b75e089960a922be9b4180a01f29ca0c78/my_application_id-v1.0-ec2f7069-8bae-4ca2-b990-193b749f8d9e?sv=2018-03-28&sr=b&sig=mAWRdMy1EVtDWOl04CDWpkwIsVsOkdm873CI08HK4oA%3D&st=2019-08-06T23%3A03%3A21Z&se=2019-08-07T03%3A08%3A21Z&sp=rw","storageUrlExpiry":"2019-08-07T03:08:21.5743196Z","state":"Pending"}}'
+      string: '{"type":"Microsoft.Batch/batchAccounts/applications/versions","id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch93ef11ff/applications/my_application_id/versions/v1.0","name":"v1.0","etag":"W/\"0x8D8037DC43F8C7F\"","properties":{"storageUrl":"https://batch.blob.core.windows.net/app-my-application-id-8c9495a5c8784e1784ae918de3cf8665/v1.0?sv=2018-03-28&sr=b&sig=Cl1HH0LUt7%2FjHyZrIs7SZSv49%2B4jymCCCkXg3MWyec4%3D&st=2020-05-29T03%3A04%3A57Z&se=2020-05-29T07%3A09%3A57Z&sp=rw","storageUrlExpiry":"2020-05-29T07:09:57.1299157Z","state":"Pending"}}'
     headers:
       cache-control:
       - no-cache
       content-length:
-      - '732'
+      - '673'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Tue, 06 Aug 2019 23:08:21 GMT
+      - Fri, 29 May 2020 03:09:56 GMT
       etag:
-      - W/"0x8D71AC2F9F35F71"
+      - W/"0x8D8037DC43F8C7F"
       expires:
       - '-1'
       last-modified:
-      - Tue, 06 Aug 2019 23:08:21 GMT
+      - Fri, 29 May 2020 03:09:57 GMT
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
       - max-age=31536000; includeSubDomains
       transfer-encoding:
       - chunked
       vary:
       - Accept-Encoding
       x-content-type-options:
       - nosniff
       x-ms-ratelimit-remaining-subscription-writes:
-      - '1197'
+      - '1196'
     status:
       code: 200
       message: OK
 - request:
     body: Hello World
     headers:
       Accept:
@@ -347,33 +348,33 @@
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       Content-Length:
       - '11'
       User-Agent:
-      - python-requests/2.22.0
+      - python-requests/2.23.0
       x-ms-blob-type:
       - BlockBlob
     method: PUT
-    uri: https://batch93ef11ff.blob.core.windows.net/app-my-application-id-b9dfc2b75e089960a922be9b4180a01f29ca0c78/my_application_id-v1.0-ec2f7069-8bae-4ca2-b990-193b749f8d9e?sv=2018-03-28&sr=b&sig=mAWRdMy1EVtDWOl04CDWpkwIsVsOkdm873CI08HK4oA%3D&st=2019-08-06T23%3A03%3A21Z&se=2019-08-07T03%3A08%3A21Z&sp=rw
+    uri: https://batch.blob.core.windows.net/app-my-application-id-8c9495a5c8784e1784ae918de3cf8665/v1.0?sv=2018-03-28&sr=b&sig=Cl1HH0LUt7%2FjHyZrIs7SZSv49%2B4jymCCCkXg3MWyec4%3D&st=2020-05-29T03%3A04%3A57Z&se=2020-05-29T07%3A09%3A57Z&sp=rw
   response:
     body:
       string: ''
     headers:
       content-length:
       - '0'
       content-md5:
       - sQqNsWTgdUEFt6mb5y4/5Q==
       date:
-      - Tue, 06 Aug 2019 23:08:23 GMT
+      - Fri, 29 May 2020 03:09:57 GMT
       etag:
-      - '"0x8D71AC2FAFE2136"'
+      - '"0x8D8037DC5315BF2"'
       last-modified:
-      - Tue, 06 Aug 2019 23:08:23 GMT
+      - Fri, 29 May 2020 03:09:58 GMT
       server:
       - Windows-Azure-Blob/1.0 Microsoft-HTTPAPI/2.0
       x-ms-request-server-encrypted:
       - 'true'
       x-ms-version:
       - '2018-03-28'
     status:
@@ -389,38 +390,38 @@
       Connection:
       - keep-alive
       Content-Length:
       - '17'
       Content-Type:
       - application/json; charset=utf-8
       User-Agent:
-      - python/3.6.6 (Windows-10-10.0.14393-SP0) msrest/0.6.9 msrest_azure/0.4.34
-        azure-mgmt-batch/7.0.0 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: POST
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch93ef11ff/applications/my_application_id/versions/v1.0/activate?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch93ef11ff/applications/my_application_id/versions/v1.0/activate?api-version=2020-05-01
   response:
     body:
-      string: '{"type":"Microsoft.Batch/batchAccounts/applications/versions","id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch93ef11ff/applications/my_application_id/versions/v1.0","name":"v1.0","etag":"W/\"0x8D71AC2FB1F6B6E\"","properties":{"storageUrl":"https://batch93ef11ff.blob.core.windows.net/app-my-application-id-b9dfc2b75e089960a922be9b4180a01f29ca0c78/my_application_id-v1.0-ec2f7069-8bae-4ca2-b990-193b749f8d9e?sv=2018-03-28&sr=b&sig=q1eSJUY%2BWeCnZ1XCckRwFPuzxfjipJVyzGx2y%2Fb62hM%3D&st=2019-08-06T23%3A03%3A23Z&se=2019-08-07T03%3A08%3A23Z&sp=rw","storageUrlExpiry":"2019-08-07T03:08:23.5706989Z","state":"Active","format":"zip","lastActivationTime":"2019-08-06T23:08:23.5272786Z"}}'
+      string: '{"type":"Microsoft.Batch/batchAccounts/applications/versions","id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch93ef11ff/applications/my_application_id/versions/v1.0","name":"v1.0","etag":"W/\"0x8D8037DC55266F8\"","properties":{"storageUrl":"https://batch.blob.core.windows.net/app-my-application-id-8c9495a5c8784e1784ae918de3cf8665/v1.0?sv=2018-03-28&sr=b&sig=PYl5%2BYUTsww2GhaTKV5dkG%2FxeU1Dm8eQd4jCQmJeF4g%3D&st=2020-05-29T03%3A04%3A58Z&se=2020-05-29T07%3A09%3A58Z&sp=rw","storageUrlExpiry":"2020-05-29T07:09:58.9545243Z","state":"Active","format":"zip","lastActivationTime":"2020-05-29T03:09:58.916835Z"}}'
     headers:
       cache-control:
       - no-cache
       content-length:
-      - '802'
+      - '738'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Tue, 06 Aug 2019 23:08:23 GMT
+      - Fri, 29 May 2020 03:09:58 GMT
       etag:
-      - W/"0x8D71AC2FB1F6B6E"
+      - W/"0x8D8037DC55266F8"
       expires:
       - '-1'
       last-modified:
-      - Tue, 06 Aug 2019 23:08:23 GMT
+      - Fri, 29 May 2020 03:09:58 GMT
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
       - max-age=31536000; includeSubDomains
       transfer-encoding:
@@ -445,89 +446,89 @@
       Connection:
       - keep-alive
       Content-Length:
       - '99'
       Content-Type:
       - application/json; charset=utf-8
       User-Agent:
-      - python/3.6.6 (Windows-10-10.0.14393-SP0) msrest/0.6.9 msrest_azure/0.4.34
-        azure-mgmt-batch/7.0.0 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: PATCH
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch93ef11ff/applications/my_application_id?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch93ef11ff/applications/my_application_id?api-version=2020-05-01
   response:
     body:
-      string: '{"type":"Microsoft.Batch/batchAccounts/applications","id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch93ef11ff/applications/my_application_id","name":"my_application_id","etag":"W/\"0x8D71AC2FB4EE876\"","properties":{"displayName":"my_updated_name","allowUpdates":false,"defaultVersion":"v1.0"}}'
+      string: '{"type":"Microsoft.Batch/batchAccounts/applications","id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch93ef11ff/applications/my_application_id","name":"my_application_id","etag":"W/\"0x8D8037DC586037F\"","properties":{"displayName":"my_updated_name","allowUpdates":false,"defaultVersion":"v1.0"}}'
     headers:
       cache-control:
       - no-cache
       content-length:
       - '417'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Tue, 06 Aug 2019 23:08:23 GMT
+      - Fri, 29 May 2020 03:09:58 GMT
       etag:
-      - W/"0x8D71AC2FB4EE876"
+      - W/"0x8D8037DC586037F"
       expires:
       - '-1'
       last-modified:
-      - Tue, 06 Aug 2019 23:08:23 GMT
+      - Fri, 29 May 2020 03:09:59 GMT
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
       - max-age=31536000; includeSubDomains
       transfer-encoding:
       - chunked
       vary:
       - Accept-Encoding
       x-content-type-options:
       - nosniff
       x-ms-ratelimit-remaining-subscription-writes:
-      - '1196'
+      - '1195'
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers:
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.6.6 (Windows-10-10.0.14393-SP0) msrest/0.6.9 msrest_azure/0.4.34
-        azure-mgmt-batch/7.0.0 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch93ef11ff/applications/my_application_id/versions/v1.0?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch93ef11ff/applications/my_application_id/versions/v1.0?api-version=2020-05-01
   response:
     body:
-      string: '{"type":"Microsoft.Batch/batchAccounts/applications/versions","id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch93ef11ff/applications/my_application_id/versions/v1.0","name":"v1.0","etag":"W/\"0x8D71AC2FB1F6B6E\"","properties":{"storageUrl":"https://batch93ef11ff.blob.core.windows.net/app-my-application-id-b9dfc2b75e089960a922be9b4180a01f29ca0c78/my_application_id-v1.0-ec2f7069-8bae-4ca2-b990-193b749f8d9e?sv=2018-03-28&sr=b&sig=OIoy9faSxWf3PIft83Aln6OQvGtMolgIwvejGz7ufp4%3D&st=2019-08-06T23%3A03%3A24Z&se=2019-08-07T03%3A08%3A24Z&sp=r","storageUrlExpiry":"2019-08-07T03:08:24.0635206Z","state":"Active","format":"zip","lastActivationTime":"2019-08-06T23:08:23.5272786Z"}}'
+      string: '{"type":"Microsoft.Batch/batchAccounts/applications/versions","id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch93ef11ff/applications/my_application_id/versions/v1.0","name":"v1.0","etag":"W/\"0x8D8037DC55266F8\"","properties":{"storageUrl":"https://batch.blob.core.windows.net/app-my-application-id-8c9495a5c8784e1784ae918de3cf8665/v1.0?sv=2018-03-28&sr=b&sig=F3ZDnIpEI6KglN9dJg0%2B%2F5g5pcaF4FKF%2FiiqwQMsmXc%3D&st=2020-05-29T03%3A04%3A59Z&se=2020-05-29T07%3A09%3A59Z&sp=r","storageUrlExpiry":"2020-05-29T07:09:59.5298339Z","state":"Active","format":"zip","lastActivationTime":"2020-05-29T03:09:58.916835Z"}}'
     headers:
       cache-control:
       - no-cache
       content-length:
-      - '797'
+      - '739'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Tue, 06 Aug 2019 23:08:24 GMT
+      - Fri, 29 May 2020 03:09:58 GMT
       etag:
-      - W/"0x8D71AC2FB1F6B6E"
+      - W/"0x8D8037DC55266F8"
       expires:
       - '-1'
       last-modified:
-      - Tue, 06 Aug 2019 23:08:23 GMT
+      - Fri, 29 May 2020 03:09:58 GMT
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
       - max-age=31536000; includeSubDomains
       transfer-encoding:
@@ -547,30 +548,30 @@
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       Content-Length:
       - '0'
       User-Agent:
-      - python/3.6.6 (Windows-10-10.0.14393-SP0) msrest/0.6.9 msrest_azure/0.4.34
-        azure-mgmt-batch/7.0.0 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: DELETE
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch93ef11ff/applications/my_application_id/versions/v1.0?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch93ef11ff/applications/my_application_id/versions/v1.0?api-version=2020-05-01
   response:
     body:
       string: ''
     headers:
       cache-control:
       - no-cache
       content-length:
       - '0'
       date:
-      - Tue, 06 Aug 2019 23:08:24 GMT
+      - Fri, 29 May 2020 03:09:59 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
@@ -590,30 +591,30 @@
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       Content-Length:
       - '0'
       User-Agent:
-      - python/3.6.6 (Windows-10-10.0.14393-SP0) msrest/0.6.9 msrest_azure/0.4.34
-        azure-mgmt-batch/7.0.0 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: DELETE
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch93ef11ff/applications/my_application_id?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch93ef11ff/applications/my_application_id?api-version=2020-05-01
   response:
     body:
       string: ''
     headers:
       cache-control:
       - no-cache
       content-length:
       - '0'
       date:
-      - Tue, 06 Aug 2019 23:08:25 GMT
+      - Fri, 29 May 2020 03:09:59 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
@@ -633,34 +634,34 @@
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       Content-Length:
       - '0'
       User-Agent:
-      - python/3.6.6 (Windows-10-10.0.14393-SP0) msrest/0.6.9 msrest_azure/0.4.34
-        azure-mgmt-batch/7.0.0 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: DELETE
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch93ef11ff?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_applications93ef11ff/providers/Microsoft.Batch/batchAccounts/batch93ef11ff?api-version=2020-05-01
   response:
     body:
       string: ''
     headers:
       cache-control:
       - no-cache
       content-length:
       - '0'
       date:
-      - Tue, 06 Aug 2019 23:08:25 GMT
+      - Fri, 29 May 2020 03:09:59 GMT
       expires:
       - '-1'
       location:
-      - https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.Batch/locations/westcentralus/accountOperationResults/batch93ef11ff-4cc29555-1661-4a64-b80c-b1939fe353fc?api-version=2020-03-01
+      - https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.Batch/locations/westcentralus/accountOperationResults/batch-acab0ae9-ac1b-402b-b3d3-085eb19db9b6?api-version=2020-05-01
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
       - max-age=31536000; includeSubDomains
       x-content-type-options:
@@ -676,28 +677,28 @@
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.6.6 (Windows-10-10.0.14393-SP0) msrest/0.6.9 msrest_azure/0.4.34
-        azure-mgmt-batch/7.0.0 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.Batch/locations/westcentralus/accountOperationResults/batch93ef11ff-4cc29555-1661-4a64-b80c-b1939fe353fc?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.Batch/locations/westcentralus/accountOperationResults/batch-acab0ae9-ac1b-402b-b3d3-085eb19db9b6?api-version=2020-05-01
   response:
     body:
       string: ''
     headers:
       cache-control:
       - no-cache
       content-length:
       - '0'
       date:
-      - Tue, 06 Aug 2019 23:08:41 GMT
+      - Fri, 29 May 2020 03:10:15 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
```

## Comparing `azure-mgmt-batch-8.0.1/tests/recordings/test_mgmt_batch.test_mgmt_batch_pools.yaml` & `azure-mgmt-batch-9.0.0/tests/recordings/test_mgmt_batch.test_mgmt_batch_pools.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -15,39 +15,39 @@
       Connection:
       - keep-alive
       Content-Length:
       - '573'
       Content-Type:
       - application/json; charset=utf-8
       User-Agent:
-      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.11 msrest_azure/0.6.2
-        azure-mgmt-batch/2020-03-01 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: PUT
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_pools1f5c0f25/providers/Microsoft.Batch/batchAccounts/batch1f5c0f25/pools/test_paas_pool?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_pools1f5c0f25/providers/Microsoft.Batch/batchAccounts/batch1f5c0f25/pools/test_paas_pool?api-version=2020-05-01
   response:
     body:
-      string: '{"id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_pools1f5c0f25/providers/Microsoft.Batch/batchAccounts/batch1f5c0f25/pools/test_paas_pool","name":"test_paas_pool","type":"Microsoft.Batch/batchAccounts/pools","etag":"W/\"0x8D7DD8285302DB0\"","properties":{"lastModified":"2020-04-10T19:08:14.6228656Z","creationTime":"2020-04-10T19:08:14.6228656Z","provisioningState":"Succeeded","provisioningStateTransitionTime":"2020-04-10T19:08:14.6228656Z","allocationState":"Resizing","allocationStateTransitionTime":"2020-04-10T19:08:14.6228656Z","vmSize":"Small","interNodeCommunication":"Disabled","maxTasksPerNode":1,"taskSchedulingPolicy":{"nodeFillType":"Spread"},"deploymentConfiguration":{"cloudServiceConfiguration":{"osFamily":"5","osVersion":"*"}},"scaleSettings":{"fixedScale":{"targetDedicatedNodes":0,"targetLowPriorityNodes":0,"resizeTimeout":"PT15M"}},"startTask":{"commandLine":"cmd.exe
-        /c \"echo hello world\"","resourceFiles":[{"filePath":"filename.txt","httpUrl":"https://blobsource.com"}],"environmentSettings":[{"name":"ENV_VAR","value":"env_value"}],"userIdentity":{"autoUser":{"scope":"Pool","elevationLevel":"Admin"}},"maxTaskRetryCount":0,"waitForSuccess":true},"userAccounts":[{"name":"UserName","elevationLevel":"NonAdmin","windowsUserConfiguration":{"loginMode":"Interactive"}}],"resizeOperationStatus":{"targetDedicatedNodes":0,"nodeDeallocationOption":"Requeue","resizeTimeout":"PT15M","startTime":"2020-04-10T19:08:14.6228656Z"},"currentDedicatedNodes":0,"currentLowPriorityNodes":0}}'
+      string: '{"id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_pools1f5c0f25/providers/Microsoft.Batch/batchAccounts/batch1f5c0f25/pools/test_paas_pool","name":"test_paas_pool","type":"Microsoft.Batch/batchAccounts/pools","etag":"W/\"0x8D803F4E7A7DA36\"","properties":{"displayName":"test_pool","lastModified":"2020-05-29T17:22:46.6366006Z","creationTime":"2020-05-29T17:22:46.6366006Z","provisioningState":"Succeeded","provisioningStateTransitionTime":"2020-05-29T17:22:46.6366006Z","allocationState":"Resizing","allocationStateTransitionTime":"2020-05-29T17:22:46.6366006Z","vmSize":"Small","interNodeCommunication":"Disabled","maxTasksPerNode":1,"taskSchedulingPolicy":{"nodeFillType":"Spread"},"deploymentConfiguration":{"cloudServiceConfiguration":{"osFamily":"5","osVersion":"*"}},"scaleSettings":{"fixedScale":{"targetDedicatedNodes":0,"targetLowPriorityNodes":0,"resizeTimeout":"PT15M"}},"startTask":{"commandLine":"cmd.exe
+        /c \"echo hello world\"","resourceFiles":[{"filePath":"filename.txt","httpUrl":"https://blobsource.com"}],"environmentSettings":[{"name":"ENV_VAR","value":"env_value"}],"userIdentity":{"autoUser":{"scope":"Pool","elevationLevel":"Admin"}},"maxTaskRetryCount":0,"waitForSuccess":true},"userAccounts":[{"name":"UserName","elevationLevel":"NonAdmin","windowsUserConfiguration":{"loginMode":"Interactive"}}],"resizeOperationStatus":{"targetDedicatedNodes":0,"nodeDeallocationOption":"Requeue","resizeTimeout":"PT15M","startTime":"2020-05-29T17:22:46.6366006Z"},"currentDedicatedNodes":0,"currentLowPriorityNodes":0}}'
     headers:
       cache-control:
       - no-cache
       content-length:
-      - '1561'
+      - '1587'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Fri, 10 Apr 2020 19:08:14 GMT
+      - Fri, 29 May 2020 17:22:46 GMT
       etag:
-      - W/"0x8D7DD8285302DB0"
+      - W/"0x8D803F4E7A7DA36"
       expires:
       - '-1'
       last-modified:
-      - Fri, 10 Apr 2020 19:08:14 GMT
+      - Fri, 29 May 2020 17:22:46 GMT
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
       - max-age=31536000; includeSubDomains
       transfer-encoding:
@@ -76,39 +76,39 @@
       Connection:
       - keep-alive
       Content-Length:
       - '447'
       Content-Type:
       - application/json; charset=utf-8
       User-Agent:
-      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.11 msrest_azure/0.6.2
-        azure-mgmt-batch/2020-03-01 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: PUT
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_pools1f5c0f25/providers/Microsoft.Batch/batchAccounts/batch1f5c0f25/pools/test_iaas_pool?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_pools1f5c0f25/providers/Microsoft.Batch/batchAccounts/batch1f5c0f25/pools/test_iaas_pool?api-version=2020-05-01
   response:
     body:
-      string: '{"id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_pools1f5c0f25/providers/Microsoft.Batch/batchAccounts/batch1f5c0f25/pools/test_iaas_pool","name":"test_iaas_pool","type":"Microsoft.Batch/batchAccounts/pools","etag":"W/\"0x8D7DD828572E580\"","properties":{"lastModified":"2020-04-10T19:08:15.0601088Z","creationTime":"2020-04-10T19:08:15.0601088Z","provisioningState":"Succeeded","provisioningStateTransitionTime":"2020-04-10T19:08:15.0601088Z","allocationState":"Resizing","allocationStateTransitionTime":"2020-04-10T19:08:15.0601088Z","vmSize":"STANDARD_A1","interNodeCommunication":"Disabled","maxTasksPerNode":1,"taskSchedulingPolicy":{"nodeFillType":"Spread"},"deploymentConfiguration":{"virtualMachineConfiguration":{"imageReference":{"publisher":"MicrosoftWindowsServer","offer":"WindowsServer","sku":"2016-Datacenter-smalldisk","version":"latest"},"nodeAgentSkuId":"batch.node.windows
-        amd64","windowsConfiguration":{"enableAutomaticUpdates":true}}},"scaleSettings":{"fixedScale":{"targetDedicatedNodes":0,"targetLowPriorityNodes":0,"resizeTimeout":"PT15M"}},"resizeOperationStatus":{"targetDedicatedNodes":0,"nodeDeallocationOption":"Requeue","resizeTimeout":"PT15M","startTime":"2020-04-10T19:08:15.0601088Z"},"currentDedicatedNodes":0,"currentLowPriorityNodes":0}}'
+      string: '{"id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_pools1f5c0f25/providers/Microsoft.Batch/batchAccounts/batch1f5c0f25/pools/test_iaas_pool","name":"test_iaas_pool","type":"Microsoft.Batch/batchAccounts/pools","etag":"W/\"0x8D803F4E7E72D6D\"","properties":{"displayName":"test_pool","lastModified":"2020-05-29T17:22:47.0516077Z","creationTime":"2020-05-29T17:22:47.0516077Z","provisioningState":"Succeeded","provisioningStateTransitionTime":"2020-05-29T17:22:47.0516077Z","allocationState":"Resizing","allocationStateTransitionTime":"2020-05-29T17:22:47.0516077Z","vmSize":"STANDARD_A1","interNodeCommunication":"Disabled","maxTasksPerNode":1,"taskSchedulingPolicy":{"nodeFillType":"Spread"},"deploymentConfiguration":{"virtualMachineConfiguration":{"imageReference":{"publisher":"MicrosoftWindowsServer","offer":"WindowsServer","sku":"2016-Datacenter-smalldisk","version":"latest"},"nodeAgentSkuId":"batch.node.windows
+        amd64","windowsConfiguration":{"enableAutomaticUpdates":true}}},"scaleSettings":{"fixedScale":{"targetDedicatedNodes":0,"targetLowPriorityNodes":0,"resizeTimeout":"PT15M"}},"resizeOperationStatus":{"targetDedicatedNodes":0,"nodeDeallocationOption":"Requeue","resizeTimeout":"PT15M","startTime":"2020-05-29T17:22:47.0516077Z"},"currentDedicatedNodes":0,"currentLowPriorityNodes":0}}'
     headers:
       cache-control:
       - no-cache
       content-length:
-      - '1330'
+      - '1356'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Fri, 10 Apr 2020 19:08:15 GMT
+      - Fri, 29 May 2020 17:22:46 GMT
       etag:
-      - W/"0x8D7DD828572E580"
+      - W/"0x8D803F4E7E72D6D"
       expires:
       - '-1'
       last-modified:
-      - Fri, 10 Apr 2020 19:08:15 GMT
+      - Fri, 29 May 2020 17:22:47 GMT
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
       - max-age=31536000; includeSubDomains
       transfer-encoding:
@@ -128,34 +128,34 @@
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.11 msrest_azure/0.6.2
-        azure-mgmt-batch/2020-03-01 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_pools1f5c0f25/providers/Microsoft.Batch/batchAccounts/batch1f5c0f25/pools?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_pools1f5c0f25/providers/Microsoft.Batch/batchAccounts/batch1f5c0f25/pools?api-version=2020-05-01
   response:
     body:
-      string: '{"value":[{"id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_pools1f5c0f25/providers/Microsoft.Batch/batchAccounts/batch1f5c0f25/pools/test_iaas_pool","name":"test_iaas_pool","type":"Microsoft.Batch/batchAccounts/pools","etag":"W/\"0x8D7DD828572E580\"","properties":{"lastModified":"2020-04-10T19:08:15.0601088Z","creationTime":"2020-04-10T19:08:15.0601088Z","provisioningState":"Succeeded","provisioningStateTransitionTime":"2020-04-10T19:08:15.0601088Z","allocationState":"Resizing","allocationStateTransitionTime":"2020-04-10T19:08:15.0601088Z","vmSize":"STANDARD_A1","interNodeCommunication":"Disabled","maxTasksPerNode":1,"taskSchedulingPolicy":{"nodeFillType":"Spread"},"deploymentConfiguration":{"virtualMachineConfiguration":{"imageReference":{"publisher":"MicrosoftWindowsServer","offer":"WindowsServer","sku":"2016-Datacenter-smalldisk","version":"latest"},"nodeAgentSkuId":"batch.node.windows
-        amd64","windowsConfiguration":{"enableAutomaticUpdates":true}}},"scaleSettings":{"fixedScale":{"targetDedicatedNodes":0,"targetLowPriorityNodes":0,"resizeTimeout":"PT15M"}},"resizeOperationStatus":{"targetDedicatedNodes":0,"nodeDeallocationOption":"Requeue","resizeTimeout":"PT15M","startTime":"2020-04-10T19:08:15.0601088Z"},"currentDedicatedNodes":0,"currentLowPriorityNodes":0}},{"id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_pools1f5c0f25/providers/Microsoft.Batch/batchAccounts/batch1f5c0f25/pools/test_paas_pool","name":"test_paas_pool","type":"Microsoft.Batch/batchAccounts/pools","etag":"W/\"0x8D7DD8285302DB0\"","properties":{"lastModified":"2020-04-10T19:08:14.6228656Z","creationTime":"2020-04-10T19:08:14.6228656Z","provisioningState":"Succeeded","provisioningStateTransitionTime":"2020-04-10T19:08:14.6228656Z","allocationState":"Steady","allocationStateTransitionTime":"2020-04-10T19:08:15.0458344Z","vmSize":"Small","interNodeCommunication":"Disabled","maxTasksPerNode":1,"taskSchedulingPolicy":{"nodeFillType":"Spread"},"deploymentConfiguration":{"cloudServiceConfiguration":{"osFamily":"5","osVersion":"*"}},"scaleSettings":{"fixedScale":{"targetDedicatedNodes":0,"targetLowPriorityNodes":0,"resizeTimeout":"PT15M"}},"startTask":{"commandLine":"cmd.exe
-        /c \"echo hello world\"","resourceFiles":[{"filePath":"filename.txt","httpUrl":"https://blobsource.com"}],"environmentSettings":[{"name":"ENV_VAR","value":"env_value"}],"userIdentity":{"autoUser":{"scope":"Pool","elevationLevel":"Admin"}},"maxTaskRetryCount":0,"waitForSuccess":true},"userAccounts":[{"name":"UserName","elevationLevel":"NonAdmin","windowsUserConfiguration":{"loginMode":"Interactive"}}],"resizeOperationStatus":{"targetDedicatedNodes":0,"nodeDeallocationOption":"Requeue","resizeTimeout":"PT15M","startTime":"2020-04-10T19:08:14.6228656Z"},"currentDedicatedNodes":0,"currentLowPriorityNodes":0}}]}'
+      string: '{"value":[{"id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_pools1f5c0f25/providers/Microsoft.Batch/batchAccounts/batch1f5c0f25/pools/test_iaas_pool","name":"test_iaas_pool","type":"Microsoft.Batch/batchAccounts/pools","etag":"W/\"0x8D803F4E7E72D6D\"","properties":{"displayName":"test_pool","lastModified":"2020-05-29T17:22:47.0516077Z","creationTime":"2020-05-29T17:22:47.0516077Z","provisioningState":"Succeeded","provisioningStateTransitionTime":"2020-05-29T17:22:47.0516077Z","allocationState":"Resizing","allocationStateTransitionTime":"2020-05-29T17:22:47.0516077Z","vmSize":"STANDARD_A1","interNodeCommunication":"Disabled","maxTasksPerNode":1,"taskSchedulingPolicy":{"nodeFillType":"Spread"},"deploymentConfiguration":{"virtualMachineConfiguration":{"imageReference":{"publisher":"MicrosoftWindowsServer","offer":"WindowsServer","sku":"2016-Datacenter-smalldisk","version":"latest"},"nodeAgentSkuId":"batch.node.windows
+        amd64","windowsConfiguration":{"enableAutomaticUpdates":true}}},"scaleSettings":{"fixedScale":{"targetDedicatedNodes":0,"targetLowPriorityNodes":0,"resizeTimeout":"PT15M"}},"resizeOperationStatus":{"targetDedicatedNodes":0,"nodeDeallocationOption":"Requeue","resizeTimeout":"PT15M","startTime":"2020-05-29T17:22:47.0516077Z"},"currentDedicatedNodes":0,"currentLowPriorityNodes":0}},{"id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_pools1f5c0f25/providers/Microsoft.Batch/batchAccounts/batch1f5c0f25/pools/test_paas_pool","name":"test_paas_pool","type":"Microsoft.Batch/batchAccounts/pools","etag":"W/\"0x8D803F4E7A7DA36\"","properties":{"displayName":"test_pool","lastModified":"2020-05-29T17:22:46.6366006Z","creationTime":"2020-05-29T17:22:46.6366006Z","provisioningState":"Succeeded","provisioningStateTransitionTime":"2020-05-29T17:22:46.6366006Z","allocationState":"Resizing","allocationStateTransitionTime":"2020-05-29T17:22:46.6366006Z","vmSize":"Small","interNodeCommunication":"Disabled","maxTasksPerNode":1,"taskSchedulingPolicy":{"nodeFillType":"Spread"},"deploymentConfiguration":{"cloudServiceConfiguration":{"osFamily":"5","osVersion":"*"}},"scaleSettings":{"fixedScale":{"targetDedicatedNodes":0,"targetLowPriorityNodes":0,"resizeTimeout":"PT15M"}},"startTask":{"commandLine":"cmd.exe
+        /c \"echo hello world\"","resourceFiles":[{"filePath":"filename.txt","httpUrl":"https://blobsource.com"}],"environmentSettings":[{"name":"ENV_VAR","value":"env_value"}],"userIdentity":{"autoUser":{"scope":"Pool","elevationLevel":"Admin"}},"maxTaskRetryCount":0,"waitForSuccess":true},"userAccounts":[{"name":"UserName","elevationLevel":"NonAdmin","windowsUserConfiguration":{"loginMode":"Interactive"}}],"resizeOperationStatus":{"targetDedicatedNodes":0,"nodeDeallocationOption":"Requeue","resizeTimeout":"PT15M","startTime":"2020-05-29T17:22:46.6366006Z"},"currentDedicatedNodes":0,"currentLowPriorityNodes":0}}]}'
     headers:
       cache-control:
       - no-cache
       content-length:
-      - '2902'
+      - '2956'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Fri, 10 Apr 2020 19:08:15 GMT
+      - Fri, 29 May 2020 17:22:46 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
@@ -179,39 +179,39 @@
       Connection:
       - keep-alive
       Content-Length:
       - '88'
       Content-Type:
       - application/json; charset=utf-8
       User-Agent:
-      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.11 msrest_azure/0.6.2
-        azure-mgmt-batch/2020-03-01 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: PATCH
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_pools1f5c0f25/providers/Microsoft.Batch/batchAccounts/batch1f5c0f25/pools/test_iaas_pool?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_pools1f5c0f25/providers/Microsoft.Batch/batchAccounts/batch1f5c0f25/pools/test_iaas_pool?api-version=2020-05-01
   response:
     body:
-      string: '{"id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_pools1f5c0f25/providers/Microsoft.Batch/batchAccounts/batch1f5c0f25/pools/test_iaas_pool","name":"test_iaas_pool","type":"Microsoft.Batch/batchAccounts/pools","etag":"W/\"0x8D7DD8285E1F311\"","properties":{"lastModified":"2020-04-10T19:08:15.7879057Z","creationTime":"2020-04-10T19:08:15.0601088Z","provisioningState":"Succeeded","provisioningStateTransitionTime":"2020-04-10T19:08:15.0601088Z","allocationState":"Resizing","allocationStateTransitionTime":"2020-04-10T19:08:15.7879057Z","vmSize":"STANDARD_A1","interNodeCommunication":"Disabled","maxTasksPerNode":1,"taskSchedulingPolicy":{"nodeFillType":"Spread"},"deploymentConfiguration":{"virtualMachineConfiguration":{"imageReference":{"publisher":"MicrosoftWindowsServer","offer":"WindowsServer","sku":"2016-Datacenter-smalldisk","version":"latest"},"nodeAgentSkuId":"batch.node.windows
-        amd64","windowsConfiguration":{"enableAutomaticUpdates":true}}},"scaleSettings":{"autoScale":{"formula":"$TargetDedicatedNodes=0","evaluationInterval":"PT15M"}},"currentDedicatedNodes":0,"currentLowPriorityNodes":0,"autoScaleRun":{"evaluationTime":"2020-04-10T19:08:15.7879057Z","results":"$TargetDedicatedNodes=0;$TargetLowPriorityNodes=0;$NodeDeallocationOption=requeue"}}}'
+      string: '{"id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_pools1f5c0f25/providers/Microsoft.Batch/batchAccounts/batch1f5c0f25/pools/test_iaas_pool","name":"test_iaas_pool","type":"Microsoft.Batch/batchAccounts/pools","etag":"W/\"0x8D803F4F18BD617\"","properties":{"displayName":"test_pool","lastModified":"2020-05-29T17:23:03.2302103Z","creationTime":"2020-05-29T17:22:47.0516077Z","provisioningState":"Succeeded","provisioningStateTransitionTime":"2020-05-29T17:22:47.0516077Z","allocationState":"Resizing","allocationStateTransitionTime":"2020-05-29T17:23:03.2302103Z","vmSize":"STANDARD_A1","interNodeCommunication":"Disabled","maxTasksPerNode":1,"taskSchedulingPolicy":{"nodeFillType":"Spread"},"deploymentConfiguration":{"virtualMachineConfiguration":{"imageReference":{"publisher":"MicrosoftWindowsServer","offer":"WindowsServer","sku":"2016-Datacenter-smalldisk","version":"latest"},"nodeAgentSkuId":"batch.node.windows
+        amd64","windowsConfiguration":{"enableAutomaticUpdates":true}}},"scaleSettings":{"autoScale":{"formula":"$TargetDedicatedNodes=0","evaluationInterval":"PT15M"}},"currentDedicatedNodes":0,"currentLowPriorityNodes":0,"autoScaleRun":{"evaluationTime":"2020-05-29T17:23:03.2302103Z","results":"$TargetDedicatedNodes=0;$TargetLowPriorityNodes=0;$NodeDeallocationOption=requeue"}}}'
     headers:
       cache-control:
       - no-cache
       content-length:
-      - '1324'
+      - '1350'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Fri, 10 Apr 2020 19:08:15 GMT
+      - Fri, 29 May 2020 17:23:02 GMT
       etag:
-      - W/"0x8D7DD8285E1F311"
+      - W/"0x8D803F4F18BD617"
       expires:
       - '-1'
       last-modified:
-      - Fri, 10 Apr 2020 19:08:15 GMT
+      - Fri, 29 May 2020 17:23:03 GMT
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
       - max-age=31536000; includeSubDomains
       transfer-encoding:
@@ -231,39 +231,39 @@
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.11 msrest_azure/0.6.2
-        azure-mgmt-batch/2020-03-01 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_pools1f5c0f25/providers/Microsoft.Batch/batchAccounts/batch1f5c0f25/pools/test_iaas_pool?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_pools1f5c0f25/providers/Microsoft.Batch/batchAccounts/batch1f5c0f25/pools/test_iaas_pool?api-version=2020-05-01
   response:
     body:
-      string: '{"id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_pools1f5c0f25/providers/Microsoft.Batch/batchAccounts/batch1f5c0f25/pools/test_iaas_pool","name":"test_iaas_pool","type":"Microsoft.Batch/batchAccounts/pools","etag":"W/\"0x8D7DD8285E1F311\"","properties":{"lastModified":"2020-04-10T19:08:15.7879057Z","creationTime":"2020-04-10T19:08:15.0601088Z","provisioningState":"Succeeded","provisioningStateTransitionTime":"2020-04-10T19:08:15.0601088Z","allocationState":"Resizing","allocationStateTransitionTime":"2020-04-10T19:08:15.7879057Z","vmSize":"STANDARD_A1","interNodeCommunication":"Disabled","maxTasksPerNode":1,"taskSchedulingPolicy":{"nodeFillType":"Spread"},"deploymentConfiguration":{"virtualMachineConfiguration":{"imageReference":{"publisher":"MicrosoftWindowsServer","offer":"WindowsServer","sku":"2016-Datacenter-smalldisk","version":"latest"},"nodeAgentSkuId":"batch.node.windows
-        amd64","windowsConfiguration":{"enableAutomaticUpdates":true}}},"scaleSettings":{"autoScale":{"formula":"$TargetDedicatedNodes=0","evaluationInterval":"PT15M"}},"currentDedicatedNodes":0,"currentLowPriorityNodes":0,"autoScaleRun":{"evaluationTime":"2020-04-10T19:08:15.7879057Z","results":"$TargetDedicatedNodes=0;$TargetLowPriorityNodes=0;$NodeDeallocationOption=requeue"}}}'
+      string: '{"id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_pools1f5c0f25/providers/Microsoft.Batch/batchAccounts/batch1f5c0f25/pools/test_iaas_pool","name":"test_iaas_pool","type":"Microsoft.Batch/batchAccounts/pools","etag":"W/\"0x8D803F4F18BD617\"","properties":{"displayName":"test_pool","lastModified":"2020-05-29T17:23:03.2302103Z","creationTime":"2020-05-29T17:22:47.0516077Z","provisioningState":"Succeeded","provisioningStateTransitionTime":"2020-05-29T17:22:47.0516077Z","allocationState":"Steady","allocationStateTransitionTime":"2020-05-29T17:23:03.572301Z","vmSize":"STANDARD_A1","interNodeCommunication":"Disabled","maxTasksPerNode":1,"taskSchedulingPolicy":{"nodeFillType":"Spread"},"deploymentConfiguration":{"virtualMachineConfiguration":{"imageReference":{"publisher":"MicrosoftWindowsServer","offer":"WindowsServer","sku":"2016-Datacenter-smalldisk","version":"latest"},"nodeAgentSkuId":"batch.node.windows
+        amd64","windowsConfiguration":{"enableAutomaticUpdates":true}}},"scaleSettings":{"autoScale":{"formula":"$TargetDedicatedNodes=0","evaluationInterval":"PT15M"}},"resizeOperationStatus":{"targetDedicatedNodes":0,"nodeDeallocationOption":"Requeue","resizeTimeout":"PT15M","startTime":"2020-05-29T17:22:47.0516077Z"},"currentDedicatedNodes":0,"currentLowPriorityNodes":0,"autoScaleRun":{"evaluationTime":"2020-05-29T17:23:03.2302103Z","results":"$TargetDedicatedNodes=0;$TargetLowPriorityNodes=0;$NodeDeallocationOption=requeue"}}}'
     headers:
       cache-control:
       - no-cache
       content-length:
-      - '1324'
+      - '1500'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Fri, 10 Apr 2020 19:08:15 GMT
+      - Fri, 29 May 2020 17:23:03 GMT
       etag:
-      - W/"0x8D7DD8285E1F311"
+      - W/"0x8D803F4F18BD617"
       expires:
       - '-1'
       last-modified:
-      - Fri, 10 Apr 2020 19:08:15 GMT
+      - Fri, 29 May 2020 17:23:03 GMT
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
       - max-age=31536000; includeSubDomains
       transfer-encoding:
@@ -283,34 +283,34 @@
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       Content-Length:
       - '0'
       User-Agent:
-      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.11 msrest_azure/0.6.2
-        azure-mgmt-batch/2020-03-01 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: POST
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_pools1f5c0f25/providers/Microsoft.Batch/batchAccounts/batch1f5c0f25/pools/test_iaas_pool/stopResize?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_pools1f5c0f25/providers/Microsoft.Batch/batchAccounts/batch1f5c0f25/pools/test_iaas_pool/stopResize?api-version=2020-05-01
   response:
     body:
       string: '{"error":{"code":"OperationInvalidForCurrentState","message":"The specified
-        operation is not valid for the current state of the resource.\nRequestId:9780a820-83f0-40d7-83d0-a6dfc7c534a4\nTime:2020-04-10T19:08:16.1732721Z","target":"BatchAccount","details":[{"code":"Reason","message":"The
+        operation is not valid for the current state of the resource.\nRequestId:6f2d8aa2-5798-44e2-92f0-0de0b524b64b\nTime:2020-05-29T17:23:03.9595120Z","target":"BatchAccount","details":[{"code":"Reason","message":"The
         specified pool has AutoScale enabled. AutoScale resize cannot be stopped"}]}}'
     headers:
       cache-control:
       - no-cache
       content-length:
       - '366'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Fri, 10 Apr 2020 19:08:16 GMT
+      - Fri, 29 May 2020 17:23:03 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
@@ -330,39 +330,39 @@
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       Content-Length:
       - '0'
       User-Agent:
-      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.11 msrest_azure/0.6.2
-        azure-mgmt-batch/2020-03-01 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: POST
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_pools1f5c0f25/providers/Microsoft.Batch/batchAccounts/batch1f5c0f25/pools/test_iaas_pool/disableAutoScale?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_pools1f5c0f25/providers/Microsoft.Batch/batchAccounts/batch1f5c0f25/pools/test_iaas_pool/disableAutoScale?api-version=2020-05-01
   response:
     body:
-      string: '{"id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_pools1f5c0f25/providers/Microsoft.Batch/batchAccounts/batch1f5c0f25/pools/test_iaas_pool","name":"test_iaas_pool","type":"Microsoft.Batch/batchAccounts/pools","etag":"W/\"0x8D7DD833944235A\"","properties":{"lastModified":"2020-04-10T19:13:16.743561Z","creationTime":"2020-04-10T19:08:15.0601088Z","provisioningState":"Succeeded","provisioningStateTransitionTime":"2020-04-10T19:08:15.0601088Z","allocationState":"Resizing","allocationStateTransitionTime":"2020-04-10T19:13:16.743561Z","vmSize":"STANDARD_A1","interNodeCommunication":"Disabled","maxTasksPerNode":1,"taskSchedulingPolicy":{"nodeFillType":"Spread"},"deploymentConfiguration":{"virtualMachineConfiguration":{"imageReference":{"publisher":"MicrosoftWindowsServer","offer":"WindowsServer","sku":"2016-Datacenter-smalldisk","version":"latest"},"nodeAgentSkuId":"batch.node.windows
+      string: '{"id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_pools1f5c0f25/providers/Microsoft.Batch/batchAccounts/batch1f5c0f25/pools/test_iaas_pool","name":"test_iaas_pool","type":"Microsoft.Batch/batchAccounts/pools","etag":"W/\"0x8D803F5A57A8750\"","properties":{"displayName":"test_pool","lastModified":"2020-05-29T17:28:05.1066704Z","creationTime":"2020-05-29T17:22:47.0516077Z","provisioningState":"Succeeded","provisioningStateTransitionTime":"2020-05-29T17:22:47.0516077Z","allocationState":"Resizing","allocationStateTransitionTime":"2020-05-29T17:28:05.1066704Z","vmSize":"STANDARD_A1","interNodeCommunication":"Disabled","maxTasksPerNode":1,"taskSchedulingPolicy":{"nodeFillType":"Spread"},"deploymentConfiguration":{"virtualMachineConfiguration":{"imageReference":{"publisher":"MicrosoftWindowsServer","offer":"WindowsServer","sku":"2016-Datacenter-smalldisk","version":"latest"},"nodeAgentSkuId":"batch.node.windows
         amd64","windowsConfiguration":{"enableAutomaticUpdates":true}}},"scaleSettings":{"fixedScale":{"targetDedicatedNodes":0,"targetLowPriorityNodes":0,"resizeTimeout":"PT15M"}},"currentDedicatedNodes":0,"currentLowPriorityNodes":0}}'
     headers:
       cache-control:
       - no-cache
       content-length:
-      - '1175'
+      - '1203'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Fri, 10 Apr 2020 19:13:16 GMT
+      - Fri, 29 May 2020 17:28:04 GMT
       etag:
-      - W/"0x8D7DD833944235A"
+      - W/"0x8D803F5A57A8750"
       expires:
       - '-1'
       last-modified:
-      - Fri, 10 Apr 2020 19:13:16 GMT
+      - Fri, 29 May 2020 17:28:05 GMT
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
       - max-age=31536000; includeSubDomains
       transfer-encoding:
@@ -384,34 +384,34 @@
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       Content-Length:
       - '0'
       User-Agent:
-      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.11 msrest_azure/0.6.2
-        azure-mgmt-batch/2020-03-01 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: DELETE
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_pools1f5c0f25/providers/Microsoft.Batch/batchAccounts/batch1f5c0f25/pools/test_iaas_pool?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_pools1f5c0f25/providers/Microsoft.Batch/batchAccounts/batch1f5c0f25/pools/test_iaas_pool?api-version=2020-05-01
   response:
     body:
       string: ''
     headers:
       cache-control:
       - no-cache
       content-length:
       - '0'
       date:
-      - Fri, 10 Apr 2020 19:13:16 GMT
+      - Fri, 29 May 2020 17:28:04 GMT
       expires:
       - '-1'
       location:
-      - https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_pools1f5c0f25/providers/Microsoft.Batch/batchAccounts/batch1f5c0f25/poolOperationResults/delete-test_iaas_pool?api-version=2020-03-01
+      - https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_pools1f5c0f25/providers/Microsoft.Batch/batchAccounts/batch1f5c0f25/poolOperationResults/delete-test_iaas_pool?api-version=2020-05-01
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
       - max-age=31536000; includeSubDomains
       x-content-type-options:
@@ -427,28 +427,28 @@
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.11 msrest_azure/0.6.2
-        azure-mgmt-batch/2020-03-01 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_pools1f5c0f25/providers/Microsoft.Batch/batchAccounts/batch1f5c0f25/poolOperationResults/delete-test_iaas_pool?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_pools1f5c0f25/providers/Microsoft.Batch/batchAccounts/batch1f5c0f25/poolOperationResults/delete-test_iaas_pool?api-version=2020-05-01
   response:
     body:
       string: ''
     headers:
       cache-control:
       - no-cache
       content-length:
       - '0'
       date:
-      - Fri, 10 Apr 2020 19:13:31 GMT
+      - Fri, 29 May 2020 17:28:20 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
```

## Comparing `azure-mgmt-batch-8.0.1/tests/recordings/test_mgmt_batch.test_mgmt_batch_subscription_quota.yaml` & `azure-mgmt-batch-9.0.0/tests/recordings/test_mgmt_batch.test_mgmt_batch_subscription_quota.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -5,32 +5,32 @@
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.11 msrest_azure/0.6.2
-        azure-mgmt-batch/2020-03-01 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.Batch/locations/westcentralus/quotas?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.Batch/locations/westcentralus/quotas?api-version=2020-05-01
   response:
     body:
-      string: '{"accountQuota":3}'
+      string: '{"accountQuota":50}'
     headers:
       cache-control:
       - no-cache
       content-length:
-      - '18'
+      - '19'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Fri, 10 Apr 2020 19:19:08 GMT
+      - Fri, 29 May 2020 03:26:38 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
```

## Comparing `azure-mgmt-batch-8.0.1/tests/recordings/test_mgmt_batch.test_mgmt_batch_certificates.yaml` & `azure-mgmt-batch-9.0.0/tests/recordings/test_mgmt_batch.test_mgmt_batch_certificates.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -11,38 +11,88 @@
       Connection:
       - keep-alive
       Content-Length:
       - '2277'
       Content-Type:
       - application/json; charset=utf-8
       User-Agent:
-      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.11 msrest_azure/0.6.2
-        azure-mgmt-batch/2020-03-01 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: PUT
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_certificates93b711ee/providers/Microsoft.Batch/batchAccounts/batch93b711ee/certificates/SHA1-cff2ab63c8c955aaf71989efa641b906558d9fb7?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_certificates93b711ee/providers/Microsoft.Batch/batchAccounts/batch93b711ee/certificates/SHA1-cff2ab63c8c955aaf71989efa641b906558d9fb7?api-version=2020-05-01
   response:
     body:
-      string: '{"name":"sha1-cff2ab63c8c955aaf71989efa641b906558d9fb7","id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_certificates93b711ee/providers/Microsoft.Batch/batchAccounts/batch93b711ee/certificates/sha1-cff2ab63c8c955aaf71989efa641b906558d9fb7","type":"Microsoft.Batch/batchAccounts/certificates","etag":"W/\"0x8D7DD7F7C425FEE\"","properties":{"thumbprintAlgorithm":"sha1","thumbprint":"cff2ab63c8c955aaf71989efa641b906558d9fb7","provisioningState":"Succeeded","provisioningStateTransitionTime":"2020-04-10T18:46:31.1475385Z","format":"Pfx","publicData":"MIIBrzCCAV2gAwIBAgIQHZGt2k0LCLFKYYCFxlJnkTAJBgUrDgMCHQUAMBYxFDASBgNVBAMTC1Jvb3QgQWdlbmN5MB4XDTE2MDEwMTA3MDAwMFoXDTE4MDEwMTA3MDAwMFowEjEQMA4GA1UEAxMHbm9kZXNkazCBnzANBgkqhkiG9w0BAQEFAAOBjQAwgYkCgYEAuX4XMWyR8cQRCA81TjHOerNOFOpOBj2O8jEdZvqwRlUYgMleEY2OlPd+nalxwlQ9+qbNkNGfjnhIMgiJ5CMlXgdRMF3E6DnMnktmHFG9L0VmQ6Lgt7bhXR8IitRHeYlvy5LJlw6Lcle5Kas2j4ThYjLQbjBMDSXD4HvZNe4UYEUCAwEAAaNLMEkwRwYDVR0BBEAwPoAQEuQJLQYdHU8AjWEh3BZkY6EYMBYxFDASBgNVBAMTC1Jvb3QgQWdlbmN5ghAGN2wAqgBkihHPuNSqXDX0MAkGBSsOAwIdBQADQQB5djPe0G6c3Z8DuR6EQbIhBMTnC0zYPhigq+x1LG83761Ir8PiSy+6oxwCHOaYZyvheW0PByntC/WFwUipfn78"}}'
+      string: '{"error":{"code":"GatewayTimeout","message":"The gateway did not receive
+        a response from ''Microsoft.Batch'' within the specified time period."}}'
+    headers:
+      cache-control:
+      - no-cache
+      connection:
+      - close
+      content-length:
+      - '143'
+      content-type:
+      - application/json; charset=utf-8
+      date:
+      - Fri, 29 May 2020 03:12:19 GMT
+      expires:
+      - '-1'
+      pragma:
+      - no-cache
+      strict-transport-security:
+      - max-age=31536000; includeSubDomains
+      x-content-type-options:
+      - nosniff
+      x-ms-failure-cause:
+      - service
+    status:
+      code: 504
+      message: Gateway Timeout
+- request:
+    body: '{"properties": {"thumbprintAlgorithm": "sha1", "thumbprint": "cff2ab63c8c955aaf71989efa641b906558d9fb7",
+      "format": "Pfx", "data": "MIIGMQIBAzCCBe0GCSqGSIb3DQEHAaCCBd4EggXaMIIF1jCCA8AGCSqGSIb3DQEHAaCCA7EEggOtMIIDqTCCA6UGCyqGSIb3DQEMCgECoIICtjCCArIwHAYKKoZIhvcNAQwBAzAOBAhyd3xCtln3iQICB9AEggKQhe5P10V9iV1BsDlwWT561Yu2hVq3JT8ae/ebx1ZR/gMApVereDKkS9Zg4vFyssusHebbK5pDpU8vfAqle0TM4m7wGsRj453ZorSPUfMpHvQnAOn+2pEpWdMThU7xvZ6DVpwhDOQk9166z+KnKdHGuJKh4haMT7Rw/6xZ1rsBt2423cwTrQVMQyACrEkianpuujubKltN99qRoFAxhQcnYE2KlYKw7lRcExq6mDSYAyk5xJZ1ZFdLj6MAryZroQit/0g5eyhoNEKwWbi8px5j71pRTf7yjN+deMGQKwbGl+3OgaL1UZ5fCjypbVL60kpIBxLZwIJ7p3jJ+q9pbq9zSdzshPYor5lxyUfXqaso/0/91ayNoBzg4hQGh618PhFI6RMGjwkzhB9xk74iweJ9HQyIHf8yx2RCSI22JuCMitPMWSGvOszhbNx3AEDLuiiAOHg391mprEtKZguOIr9LrJwem/YmcHbwyz5YAbZmiseKPkllfC7dafFfCFEkj6R2oegIsZo0pEKYisAXBqT0g+6/jGwuhlZcBo0f7UIZm88iA3MrJCjlXEgV5OcQdoWj+hq0lKEdnhtCKr03AIfukN6+4vjjarZeW1bs0swq0l3XFf5RHa11otshMS4mpewshB9iO9MuKWpRxuxeng4PlKZ/zuBqmPeUrjJ9454oK35Pq+dghfemt7AUpBH/KycDNIZgfdEWUZrRKBGnc519C+RTqxyt5hWL18nJk4LvSd3QKlJ1iyJxClhhb/NWEzPqNdyA5cxen+2T9bd/EqJ2KzRv5/BPVwTQkHH9W/TZElFyvFfOFIW2+03RKbVGw72Mr/0xKZ+awAnEfoU+SL/2Gj2m6PHkqFX2sOCi/tN9EA4xgdswEwYJKoZIhvcNAQkVMQYEBAEAAAAwXQYJKwYBBAGCNxEBMVAeTgBNAGkAYwByAG8AcwBvAGYAdAAgAFMAdAByAG8AbgBnACAAQwByAHkAcAB0AG8AZwByAGEAcABoAGkAYwAgAFAAcgBvAHYAaQBkAGUAcjBlBgkqhkiG9w0BCRQxWB5WAFAAdgBrAFQAbQBwADoANABjAGUANgAwADQAZABhAC0AMAA2ADgAMQAtADQANAAxADUALQBhADIAYwBhAC0ANQA3ADcAMwAwADgAZQA2AGQAOQBhAGMwggIOBgkqhkiG9w0BBwGgggH/BIIB+zCCAfcwggHzBgsqhkiG9w0BDAoBA6CCAcswggHHBgoqhkiG9w0BCRYBoIIBtwSCAbMwggGvMIIBXaADAgECAhAdka3aTQsIsUphgIXGUmeRMAkGBSsOAwIdBQAwFjEUMBIGA1UEAxMLUm9vdCBBZ2VuY3kwHhcNMTYwMTAxMDcwMDAwWhcNMTgwMTAxMDcwMDAwWjASMRAwDgYDVQQDEwdub2Rlc2RrMIGfMA0GCSqGSIb3DQEBAQUAA4GNADCBiQKBgQC5fhcxbJHxxBEIDzVOMc56s04U6k4GPY7yMR1m+rBGVRiAyV4RjY6U936dqXHCVD36ps2Q0Z+OeEgyCInkIyVeB1EwXcToOcyeS2YcUb0vRWZDouC3tuFdHwiK1Ed5iW/LksmXDotyV7kpqzaPhOFiMtBuMEwNJcPge9k17hRgRQIDAQABo0swSTBHBgNVHQEEQDA+gBAS5AktBh0dTwCNYSHcFmRjoRgwFjEUMBIGA1UEAxMLUm9vdCBBZ2VuY3mCEAY3bACqAGSKEc+41KpcNfQwCQYFKw4DAh0FAANBAHl2M97QbpzdnwO5HoRBsiEExOcLTNg+GKCr7HUsbzfvrUivw+JLL7qjHAIc5phnK+F5bQ8HKe0L9YXBSKl+fvwxFTATBgkqhkiG9w0BCRUxBgQEAQAAADA7MB8wBwYFKw4DAhoEFGVtyGMqiBd32fGpzlGZQoRM6UQwBBTI0YHFFqTS4Go8CoLgswn29EiuUQICB9A=",
+      "password": "nodesdk"}}'
+    headers:
+      Accept:
+      - application/json
+      Accept-Encoding:
+      - gzip, deflate
+      Connection:
+      - keep-alive
+      Content-Length:
+      - '2277'
+      Content-Type:
+      - application/json; charset=utf-8
+      User-Agent:
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
+      accept-language:
+      - en-US
+    method: PUT
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_certificates93b711ee/providers/Microsoft.Batch/batchAccounts/batch93b711ee/certificates/SHA1-cff2ab63c8c955aaf71989efa641b906558d9fb7?api-version=2020-05-01
+  response:
+    body:
+      string: '{"name":"sha1-cff2ab63c8c955aaf71989efa641b906558d9fb7","id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_certificates93b711ee/providers/Microsoft.Batch/batchAccounts/batch93b711ee/certificates/sha1-cff2ab63c8c955aaf71989efa641b906558d9fb7","type":"Microsoft.Batch/batchAccounts/certificates","etag":"W/\"0x8D8037E19E957D4\"","properties":{"thumbprintAlgorithm":"sha1","thumbprint":"cff2ab63c8c955aaf71989efa641b906558d9fb7","provisioningState":"Succeeded","provisioningStateTransitionTime":"2020-05-29T03:12:20.8380433Z","format":"Pfx","publicData":"MIIBrzCCAV2gAwIBAgIQHZGt2k0LCLFKYYCFxlJnkTAJBgUrDgMCHQUAMBYxFDASBgNVBAMTC1Jvb3QgQWdlbmN5MB4XDTE2MDEwMTA3MDAwMFoXDTE4MDEwMTA3MDAwMFowEjEQMA4GA1UEAxMHbm9kZXNkazCBnzANBgkqhkiG9w0BAQEFAAOBjQAwgYkCgYEAuX4XMWyR8cQRCA81TjHOerNOFOpOBj2O8jEdZvqwRlUYgMleEY2OlPd+nalxwlQ9+qbNkNGfjnhIMgiJ5CMlXgdRMF3E6DnMnktmHFG9L0VmQ6Lgt7bhXR8IitRHeYlvy5LJlw6Lcle5Kas2j4ThYjLQbjBMDSXD4HvZNe4UYEUCAwEAAaNLMEkwRwYDVR0BBEAwPoAQEuQJLQYdHU8AjWEh3BZkY6EYMBYxFDASBgNVBAMTC1Jvb3QgQWdlbmN5ghAGN2wAqgBkihHPuNSqXDX0MAkGBSsOAwIdBQADQQB5djPe0G6c3Z8DuR6EQbIhBMTnC0zYPhigq+x1LG83761Ir8PiSy+6oxwCHOaYZyvheW0PByntC/WFwUipfn78"}}'
     headers:
       cache-control:
       - no-cache
       content-length:
       - '1189'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Fri, 10 Apr 2020 18:46:31 GMT
+      - Fri, 29 May 2020 03:12:20 GMT
       etag:
-      - W/"0x8D7DD7F7C425FEE"
+      - W/"0x8D8037E19E957D4"
       expires:
       - '-1'
       last-modified:
-      - Fri, 10 Apr 2020 18:46:31 GMT
+      - Fri, 29 May 2020 03:12:20 GMT
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
       - max-age=31536000; includeSubDomains
       transfer-encoding:
@@ -62,32 +112,32 @@
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.11 msrest_azure/0.6.2
-        azure-mgmt-batch/2020-03-01 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_certificates93b711ee/providers/Microsoft.Batch/batchAccounts/batch93b711ee/certificates?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_certificates93b711ee/providers/Microsoft.Batch/batchAccounts/batch93b711ee/certificates?api-version=2020-05-01
   response:
     body:
-      string: '{"value":[{"name":"sha1-cff2ab63c8c955aaf71989efa641b906558d9fb7","id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_certificates93b711ee/providers/Microsoft.Batch/batchAccounts/batch93b711ee/certificates/sha1-cff2ab63c8c955aaf71989efa641b906558d9fb7","type":"Microsoft.Batch/batchAccounts/certificates","etag":"W/\"0x8D7DD7F7C425FEE\"","properties":{"thumbprintAlgorithm":"sha1","thumbprint":"cff2ab63c8c955aaf71989efa641b906558d9fb7","provisioningState":"Succeeded","provisioningStateTransitionTime":"2020-04-10T18:46:31.1475385Z","format":"Pfx","publicData":"MIIBrzCCAV2gAwIBAgIQHZGt2k0LCLFKYYCFxlJnkTAJBgUrDgMCHQUAMBYxFDASBgNVBAMTC1Jvb3QgQWdlbmN5MB4XDTE2MDEwMTA3MDAwMFoXDTE4MDEwMTA3MDAwMFowEjEQMA4GA1UEAxMHbm9kZXNkazCBnzANBgkqhkiG9w0BAQEFAAOBjQAwgYkCgYEAuX4XMWyR8cQRCA81TjHOerNOFOpOBj2O8jEdZvqwRlUYgMleEY2OlPd+nalxwlQ9+qbNkNGfjnhIMgiJ5CMlXgdRMF3E6DnMnktmHFG9L0VmQ6Lgt7bhXR8IitRHeYlvy5LJlw6Lcle5Kas2j4ThYjLQbjBMDSXD4HvZNe4UYEUCAwEAAaNLMEkwRwYDVR0BBEAwPoAQEuQJLQYdHU8AjWEh3BZkY6EYMBYxFDASBgNVBAMTC1Jvb3QgQWdlbmN5ghAGN2wAqgBkihHPuNSqXDX0MAkGBSsOAwIdBQADQQB5djPe0G6c3Z8DuR6EQbIhBMTnC0zYPhigq+x1LG83761Ir8PiSy+6oxwCHOaYZyvheW0PByntC/WFwUipfn78"}}]}'
+      string: '{"value":[{"name":"sha1-cff2ab63c8c955aaf71989efa641b906558d9fb7","id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_certificates93b711ee/providers/Microsoft.Batch/batchAccounts/batch93b711ee/certificates/sha1-cff2ab63c8c955aaf71989efa641b906558d9fb7","type":"Microsoft.Batch/batchAccounts/certificates","etag":"W/\"0x8D8037E19E957D4\"","properties":{"thumbprintAlgorithm":"sha1","thumbprint":"cff2ab63c8c955aaf71989efa641b906558d9fb7","provisioningState":"Succeeded","provisioningStateTransitionTime":"2020-05-29T03:12:20.8380433Z","format":"Pfx","publicData":"MIIBrzCCAV2gAwIBAgIQHZGt2k0LCLFKYYCFxlJnkTAJBgUrDgMCHQUAMBYxFDASBgNVBAMTC1Jvb3QgQWdlbmN5MB4XDTE2MDEwMTA3MDAwMFoXDTE4MDEwMTA3MDAwMFowEjEQMA4GA1UEAxMHbm9kZXNkazCBnzANBgkqhkiG9w0BAQEFAAOBjQAwgYkCgYEAuX4XMWyR8cQRCA81TjHOerNOFOpOBj2O8jEdZvqwRlUYgMleEY2OlPd+nalxwlQ9+qbNkNGfjnhIMgiJ5CMlXgdRMF3E6DnMnktmHFG9L0VmQ6Lgt7bhXR8IitRHeYlvy5LJlw6Lcle5Kas2j4ThYjLQbjBMDSXD4HvZNe4UYEUCAwEAAaNLMEkwRwYDVR0BBEAwPoAQEuQJLQYdHU8AjWEh3BZkY6EYMBYxFDASBgNVBAMTC1Jvb3QgQWdlbmN5ghAGN2wAqgBkihHPuNSqXDX0MAkGBSsOAwIdBQADQQB5djPe0G6c3Z8DuR6EQbIhBMTnC0zYPhigq+x1LG83761Ir8PiSy+6oxwCHOaYZyvheW0PByntC/WFwUipfn78"}}]}'
     headers:
       cache-control:
       - no-cache
       content-length:
       - '1201'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Fri, 10 Apr 2020 18:46:31 GMT
+      - Fri, 29 May 2020 03:12:20 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
@@ -107,38 +157,38 @@
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.11 msrest_azure/0.6.2
-        azure-mgmt-batch/2020-03-01 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_certificates93b711ee/providers/Microsoft.Batch/batchAccounts/batch93b711ee/certificates/SHA1-cff2ab63c8c955aaf71989efa641b906558d9fb7?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_certificates93b711ee/providers/Microsoft.Batch/batchAccounts/batch93b711ee/certificates/SHA1-cff2ab63c8c955aaf71989efa641b906558d9fb7?api-version=2020-05-01
   response:
     body:
-      string: '{"name":"sha1-cff2ab63c8c955aaf71989efa641b906558d9fb7","id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_certificates93b711ee/providers/Microsoft.Batch/batchAccounts/batch93b711ee/certificates/sha1-cff2ab63c8c955aaf71989efa641b906558d9fb7","type":"Microsoft.Batch/batchAccounts/certificates","etag":"W/\"0x8D7DD7F7C425FEE\"","properties":{"thumbprintAlgorithm":"sha1","thumbprint":"cff2ab63c8c955aaf71989efa641b906558d9fb7","provisioningState":"Succeeded","provisioningStateTransitionTime":"2020-04-10T18:46:31.1475385Z","format":"Pfx","publicData":"MIIBrzCCAV2gAwIBAgIQHZGt2k0LCLFKYYCFxlJnkTAJBgUrDgMCHQUAMBYxFDASBgNVBAMTC1Jvb3QgQWdlbmN5MB4XDTE2MDEwMTA3MDAwMFoXDTE4MDEwMTA3MDAwMFowEjEQMA4GA1UEAxMHbm9kZXNkazCBnzANBgkqhkiG9w0BAQEFAAOBjQAwgYkCgYEAuX4XMWyR8cQRCA81TjHOerNOFOpOBj2O8jEdZvqwRlUYgMleEY2OlPd+nalxwlQ9+qbNkNGfjnhIMgiJ5CMlXgdRMF3E6DnMnktmHFG9L0VmQ6Lgt7bhXR8IitRHeYlvy5LJlw6Lcle5Kas2j4ThYjLQbjBMDSXD4HvZNe4UYEUCAwEAAaNLMEkwRwYDVR0BBEAwPoAQEuQJLQYdHU8AjWEh3BZkY6EYMBYxFDASBgNVBAMTC1Jvb3QgQWdlbmN5ghAGN2wAqgBkihHPuNSqXDX0MAkGBSsOAwIdBQADQQB5djPe0G6c3Z8DuR6EQbIhBMTnC0zYPhigq+x1LG83761Ir8PiSy+6oxwCHOaYZyvheW0PByntC/WFwUipfn78"}}'
+      string: '{"name":"sha1-cff2ab63c8c955aaf71989efa641b906558d9fb7","id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_certificates93b711ee/providers/Microsoft.Batch/batchAccounts/batch93b711ee/certificates/sha1-cff2ab63c8c955aaf71989efa641b906558d9fb7","type":"Microsoft.Batch/batchAccounts/certificates","etag":"W/\"0x8D8037E19E957D4\"","properties":{"thumbprintAlgorithm":"sha1","thumbprint":"cff2ab63c8c955aaf71989efa641b906558d9fb7","provisioningState":"Succeeded","provisioningStateTransitionTime":"2020-05-29T03:12:20.8380433Z","format":"Pfx","publicData":"MIIBrzCCAV2gAwIBAgIQHZGt2k0LCLFKYYCFxlJnkTAJBgUrDgMCHQUAMBYxFDASBgNVBAMTC1Jvb3QgQWdlbmN5MB4XDTE2MDEwMTA3MDAwMFoXDTE4MDEwMTA3MDAwMFowEjEQMA4GA1UEAxMHbm9kZXNkazCBnzANBgkqhkiG9w0BAQEFAAOBjQAwgYkCgYEAuX4XMWyR8cQRCA81TjHOerNOFOpOBj2O8jEdZvqwRlUYgMleEY2OlPd+nalxwlQ9+qbNkNGfjnhIMgiJ5CMlXgdRMF3E6DnMnktmHFG9L0VmQ6Lgt7bhXR8IitRHeYlvy5LJlw6Lcle5Kas2j4ThYjLQbjBMDSXD4HvZNe4UYEUCAwEAAaNLMEkwRwYDVR0BBEAwPoAQEuQJLQYdHU8AjWEh3BZkY6EYMBYxFDASBgNVBAMTC1Jvb3QgQWdlbmN5ghAGN2wAqgBkihHPuNSqXDX0MAkGBSsOAwIdBQADQQB5djPe0G6c3Z8DuR6EQbIhBMTnC0zYPhigq+x1LG83761Ir8PiSy+6oxwCHOaYZyvheW0PByntC/WFwUipfn78"}}'
     headers:
       cache-control:
       - no-cache
       content-length:
       - '1189'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Fri, 10 Apr 2020 18:46:31 GMT
+      - Fri, 29 May 2020 03:12:20 GMT
       etag:
-      - W/"0x8D7DD7F7C425FEE"
+      - W/"0x8D8037E19E957D4"
       expires:
       - '-1'
       last-modified:
-      - Fri, 10 Apr 2020 18:46:31 GMT
+      - Fri, 29 May 2020 03:12:20 GMT
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
       - max-age=31536000; includeSubDomains
       transfer-encoding:
@@ -161,38 +211,38 @@
       Connection:
       - keep-alive
       Content-Length:
       - '2171'
       Content-Type:
       - application/json; charset=utf-8
       User-Agent:
-      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.11 msrest_azure/0.6.2
-        azure-mgmt-batch/2020-03-01 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: PATCH
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_certificates93b711ee/providers/Microsoft.Batch/batchAccounts/batch93b711ee/certificates/SHA1-cff2ab63c8c955aaf71989efa641b906558d9fb7?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_certificates93b711ee/providers/Microsoft.Batch/batchAccounts/batch93b711ee/certificates/SHA1-cff2ab63c8c955aaf71989efa641b906558d9fb7?api-version=2020-05-01
   response:
     body:
-      string: '{"name":"sha1-cff2ab63c8c955aaf71989efa641b906558d9fb7","id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_certificates93b711ee/providers/Microsoft.Batch/batchAccounts/batch93b711ee/certificates/sha1-cff2ab63c8c955aaf71989efa641b906558d9fb7","type":"Microsoft.Batch/batchAccounts/certificates","etag":"W/\"0x8D7DD7F7C425FEE\"","properties":{"thumbprintAlgorithm":"sha1","thumbprint":"cff2ab63c8c955aaf71989efa641b906558d9fb7","provisioningState":"Succeeded","provisioningStateTransitionTime":"2020-04-10T18:46:31.1475385Z","format":"Pfx","publicData":"MIIBrzCCAV2gAwIBAgIQHZGt2k0LCLFKYYCFxlJnkTAJBgUrDgMCHQUAMBYxFDASBgNVBAMTC1Jvb3QgQWdlbmN5MB4XDTE2MDEwMTA3MDAwMFoXDTE4MDEwMTA3MDAwMFowEjEQMA4GA1UEAxMHbm9kZXNkazCBnzANBgkqhkiG9w0BAQEFAAOBjQAwgYkCgYEAuX4XMWyR8cQRCA81TjHOerNOFOpOBj2O8jEdZvqwRlUYgMleEY2OlPd+nalxwlQ9+qbNkNGfjnhIMgiJ5CMlXgdRMF3E6DnMnktmHFG9L0VmQ6Lgt7bhXR8IitRHeYlvy5LJlw6Lcle5Kas2j4ThYjLQbjBMDSXD4HvZNe4UYEUCAwEAAaNLMEkwRwYDVR0BBEAwPoAQEuQJLQYdHU8AjWEh3BZkY6EYMBYxFDASBgNVBAMTC1Jvb3QgQWdlbmN5ghAGN2wAqgBkihHPuNSqXDX0MAkGBSsOAwIdBQADQQB5djPe0G6c3Z8DuR6EQbIhBMTnC0zYPhigq+x1LG83761Ir8PiSy+6oxwCHOaYZyvheW0PByntC/WFwUipfn78"}}'
+      string: '{"name":"sha1-cff2ab63c8c955aaf71989efa641b906558d9fb7","id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_certificates93b711ee/providers/Microsoft.Batch/batchAccounts/batch93b711ee/certificates/sha1-cff2ab63c8c955aaf71989efa641b906558d9fb7","type":"Microsoft.Batch/batchAccounts/certificates","etag":"W/\"0x8D8037E19E957D4\"","properties":{"thumbprintAlgorithm":"sha1","thumbprint":"cff2ab63c8c955aaf71989efa641b906558d9fb7","provisioningState":"Succeeded","provisioningStateTransitionTime":"2020-05-29T03:12:20.8380433Z","format":"Pfx","publicData":"MIIBrzCCAV2gAwIBAgIQHZGt2k0LCLFKYYCFxlJnkTAJBgUrDgMCHQUAMBYxFDASBgNVBAMTC1Jvb3QgQWdlbmN5MB4XDTE2MDEwMTA3MDAwMFoXDTE4MDEwMTA3MDAwMFowEjEQMA4GA1UEAxMHbm9kZXNkazCBnzANBgkqhkiG9w0BAQEFAAOBjQAwgYkCgYEAuX4XMWyR8cQRCA81TjHOerNOFOpOBj2O8jEdZvqwRlUYgMleEY2OlPd+nalxwlQ9+qbNkNGfjnhIMgiJ5CMlXgdRMF3E6DnMnktmHFG9L0VmQ6Lgt7bhXR8IitRHeYlvy5LJlw6Lcle5Kas2j4ThYjLQbjBMDSXD4HvZNe4UYEUCAwEAAaNLMEkwRwYDVR0BBEAwPoAQEuQJLQYdHU8AjWEh3BZkY6EYMBYxFDASBgNVBAMTC1Jvb3QgQWdlbmN5ghAGN2wAqgBkihHPuNSqXDX0MAkGBSsOAwIdBQADQQB5djPe0G6c3Z8DuR6EQbIhBMTnC0zYPhigq+x1LG83761Ir8PiSy+6oxwCHOaYZyvheW0PByntC/WFwUipfn78"}}'
     headers:
       cache-control:
       - no-cache
       content-length:
       - '1189'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Fri, 10 Apr 2020 18:46:31 GMT
+      - Fri, 29 May 2020 03:12:20 GMT
       etag:
-      - W/"0x8D7DD7F7C425FEE"
+      - W/"0x8D8037E19E957D4"
       expires:
       - '-1'
       last-modified:
-      - Fri, 10 Apr 2020 18:46:31 GMT
+      - Fri, 29 May 2020 03:12:20 GMT
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
       - max-age=31536000; includeSubDomains
       transfer-encoding:
@@ -214,38 +264,38 @@
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       Content-Length:
       - '0'
       User-Agent:
-      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.11 msrest_azure/0.6.2
-        azure-mgmt-batch/2020-03-01 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: POST
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_certificates93b711ee/providers/Microsoft.Batch/batchAccounts/batch93b711ee/certificates/SHA1-cff2ab63c8c955aaf71989efa641b906558d9fb7/cancelDelete?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_certificates93b711ee/providers/Microsoft.Batch/batchAccounts/batch93b711ee/certificates/SHA1-cff2ab63c8c955aaf71989efa641b906558d9fb7/cancelDelete?api-version=2020-05-01
   response:
     body:
-      string: '{"name":"sha1-cff2ab63c8c955aaf71989efa641b906558d9fb7","id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_certificates93b711ee/providers/Microsoft.Batch/batchAccounts/batch93b711ee/certificates/sha1-cff2ab63c8c955aaf71989efa641b906558d9fb7","type":"Microsoft.Batch/batchAccounts/certificates","etag":"W/\"0x8D7DD7F7C425FEE\"","properties":{"thumbprintAlgorithm":"sha1","thumbprint":"cff2ab63c8c955aaf71989efa641b906558d9fb7","provisioningState":"Succeeded","provisioningStateTransitionTime":"2020-04-10T18:46:31.1475385Z","format":"Pfx","publicData":"MIIBrzCCAV2gAwIBAgIQHZGt2k0LCLFKYYCFxlJnkTAJBgUrDgMCHQUAMBYxFDASBgNVBAMTC1Jvb3QgQWdlbmN5MB4XDTE2MDEwMTA3MDAwMFoXDTE4MDEwMTA3MDAwMFowEjEQMA4GA1UEAxMHbm9kZXNkazCBnzANBgkqhkiG9w0BAQEFAAOBjQAwgYkCgYEAuX4XMWyR8cQRCA81TjHOerNOFOpOBj2O8jEdZvqwRlUYgMleEY2OlPd+nalxwlQ9+qbNkNGfjnhIMgiJ5CMlXgdRMF3E6DnMnktmHFG9L0VmQ6Lgt7bhXR8IitRHeYlvy5LJlw6Lcle5Kas2j4ThYjLQbjBMDSXD4HvZNe4UYEUCAwEAAaNLMEkwRwYDVR0BBEAwPoAQEuQJLQYdHU8AjWEh3BZkY6EYMBYxFDASBgNVBAMTC1Jvb3QgQWdlbmN5ghAGN2wAqgBkihHPuNSqXDX0MAkGBSsOAwIdBQADQQB5djPe0G6c3Z8DuR6EQbIhBMTnC0zYPhigq+x1LG83761Ir8PiSy+6oxwCHOaYZyvheW0PByntC/WFwUipfn78"}}'
+      string: '{"name":"sha1-cff2ab63c8c955aaf71989efa641b906558d9fb7","id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_certificates93b711ee/providers/Microsoft.Batch/batchAccounts/batch93b711ee/certificates/sha1-cff2ab63c8c955aaf71989efa641b906558d9fb7","type":"Microsoft.Batch/batchAccounts/certificates","etag":"W/\"0x8D8037E19E957D4\"","properties":{"thumbprintAlgorithm":"sha1","thumbprint":"cff2ab63c8c955aaf71989efa641b906558d9fb7","provisioningState":"Succeeded","provisioningStateTransitionTime":"2020-05-29T03:12:20.8380433Z","format":"Pfx","publicData":"MIIBrzCCAV2gAwIBAgIQHZGt2k0LCLFKYYCFxlJnkTAJBgUrDgMCHQUAMBYxFDASBgNVBAMTC1Jvb3QgQWdlbmN5MB4XDTE2MDEwMTA3MDAwMFoXDTE4MDEwMTA3MDAwMFowEjEQMA4GA1UEAxMHbm9kZXNkazCBnzANBgkqhkiG9w0BAQEFAAOBjQAwgYkCgYEAuX4XMWyR8cQRCA81TjHOerNOFOpOBj2O8jEdZvqwRlUYgMleEY2OlPd+nalxwlQ9+qbNkNGfjnhIMgiJ5CMlXgdRMF3E6DnMnktmHFG9L0VmQ6Lgt7bhXR8IitRHeYlvy5LJlw6Lcle5Kas2j4ThYjLQbjBMDSXD4HvZNe4UYEUCAwEAAaNLMEkwRwYDVR0BBEAwPoAQEuQJLQYdHU8AjWEh3BZkY6EYMBYxFDASBgNVBAMTC1Jvb3QgQWdlbmN5ghAGN2wAqgBkihHPuNSqXDX0MAkGBSsOAwIdBQADQQB5djPe0G6c3Z8DuR6EQbIhBMTnC0zYPhigq+x1LG83761Ir8PiSy+6oxwCHOaYZyvheW0PByntC/WFwUipfn78"}}'
     headers:
       cache-control:
       - no-cache
       content-length:
       - '1189'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Fri, 10 Apr 2020 18:46:31 GMT
+      - Fri, 29 May 2020 03:12:21 GMT
       etag:
-      - W/"0x8D7DD7F7C425FEE"
+      - W/"0x8D8037E19E957D4"
       expires:
       - '-1'
       last-modified:
-      - Fri, 10 Apr 2020 18:46:31 GMT
+      - Fri, 29 May 2020 03:12:20 GMT
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
       - max-age=31536000; includeSubDomains
       transfer-encoding:
@@ -267,34 +317,34 @@
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       Content-Length:
       - '0'
       User-Agent:
-      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.11 msrest_azure/0.6.2
-        azure-mgmt-batch/2020-03-01 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: DELETE
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_certificates93b711ee/providers/Microsoft.Batch/batchAccounts/batch93b711ee/certificates/SHA1-cff2ab63c8c955aaf71989efa641b906558d9fb7?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_certificates93b711ee/providers/Microsoft.Batch/batchAccounts/batch93b711ee/certificates/SHA1-cff2ab63c8c955aaf71989efa641b906558d9fb7?api-version=2020-05-01
   response:
     body:
       string: ''
     headers:
       cache-control:
       - no-cache
       content-length:
       - '0'
       date:
-      - Fri, 10 Apr 2020 18:46:31 GMT
+      - Fri, 29 May 2020 03:12:21 GMT
       expires:
       - '-1'
       location:
-      - https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_certificates93b711ee/providers/Microsoft.Batch/batchAccounts/batch93b711ee/certificateOperationResults/sha1-cff2ab63c8c955aaf71989efa641b906558d9fb7-8D7DD7F7CDBE058?api-version=2020-03-01
+      - https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_certificates93b711ee/providers/Microsoft.Batch/batchAccounts/batch93b711ee/certificateOperationResults/sha1-cff2ab63c8c955aaf71989efa641b906558d9fb7-8D8037E1AAABFFE?api-version=2020-05-01
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
       - max-age=31536000; includeSubDomains
       x-content-type-options:
@@ -310,32 +360,32 @@
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.11 msrest_azure/0.6.2
-        azure-mgmt-batch/2020-03-01 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_certificates93b711ee/providers/Microsoft.Batch/batchAccounts/batch93b711ee/certificateOperationResults/sha1-cff2ab63c8c955aaf71989efa641b906558d9fb7-8D7DD7F7CDBE058?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_certificates93b711ee/providers/Microsoft.Batch/batchAccounts/batch93b711ee/certificateOperationResults/sha1-cff2ab63c8c955aaf71989efa641b906558d9fb7-8D8037E1AAABFFE?api-version=2020-05-01
   response:
     body:
       string: ''
     headers:
       cache-control:
       - no-cache
       content-length:
       - '0'
       date:
-      - Fri, 10 Apr 2020 18:46:47 GMT
+      - Fri, 29 May 2020 03:12:37 GMT
       expires:
       - '-1'
       location:
-      - https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_certificates93b711ee/providers/Microsoft.Batch/batchAccounts/batch93b711ee/certificateOperationResults/sha1-cff2ab63c8c955aaf71989efa641b906558d9fb7-8d7dd7f7cdbe058?api-version=2020-03-01
+      - https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_certificates93b711ee/providers/Microsoft.Batch/batchAccounts/batch93b711ee/certificateOperationResults/sha1-cff2ab63c8c955aaf71989efa641b906558d9fb7-8d8037e1aaabffe?api-version=2020-05-01
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
       - max-age=31536000; includeSubDomains
       x-content-type-options:
@@ -349,32 +399,32 @@
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.11 msrest_azure/0.6.2
-        azure-mgmt-batch/2020-03-01 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_certificates93b711ee/providers/Microsoft.Batch/batchAccounts/batch93b711ee/certificateOperationResults/sha1-cff2ab63c8c955aaf71989efa641b906558d9fb7-8d7dd7f7cdbe058?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_certificates93b711ee/providers/Microsoft.Batch/batchAccounts/batch93b711ee/certificateOperationResults/sha1-cff2ab63c8c955aaf71989efa641b906558d9fb7-8d8037e1aaabffe?api-version=2020-05-01
   response:
     body:
       string: ''
     headers:
       cache-control:
       - no-cache
       content-length:
       - '0'
       date:
-      - Fri, 10 Apr 2020 18:47:02 GMT
+      - Fri, 29 May 2020 03:12:52 GMT
       expires:
       - '-1'
       location:
-      - https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_certificates93b711ee/providers/Microsoft.Batch/batchAccounts/batch93b711ee/certificateOperationResults/sha1-cff2ab63c8c955aaf71989efa641b906558d9fb7-8d7dd7f7cdbe058?api-version=2020-03-01
+      - https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_certificates93b711ee/providers/Microsoft.Batch/batchAccounts/batch93b711ee/certificateOperationResults/sha1-cff2ab63c8c955aaf71989efa641b906558d9fb7-8d8037e1aaabffe?api-version=2020-05-01
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
       - max-age=31536000; includeSubDomains
       x-content-type-options:
@@ -388,32 +438,32 @@
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.11 msrest_azure/0.6.2
-        azure-mgmt-batch/2020-03-01 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_certificates93b711ee/providers/Microsoft.Batch/batchAccounts/batch93b711ee/certificateOperationResults/sha1-cff2ab63c8c955aaf71989efa641b906558d9fb7-8d7dd7f7cdbe058?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_certificates93b711ee/providers/Microsoft.Batch/batchAccounts/batch93b711ee/certificateOperationResults/sha1-cff2ab63c8c955aaf71989efa641b906558d9fb7-8d8037e1aaabffe?api-version=2020-05-01
   response:
     body:
       string: ''
     headers:
       cache-control:
       - no-cache
       content-length:
       - '0'
       date:
-      - Fri, 10 Apr 2020 18:47:17 GMT
+      - Fri, 29 May 2020 03:13:07 GMT
       expires:
       - '-1'
       location:
-      - https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_certificates93b711ee/providers/Microsoft.Batch/batchAccounts/batch93b711ee/certificateOperationResults/sha1-cff2ab63c8c955aaf71989efa641b906558d9fb7-8d7dd7f7cdbe058?api-version=2020-03-01
+      - https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_certificates93b711ee/providers/Microsoft.Batch/batchAccounts/batch93b711ee/certificateOperationResults/sha1-cff2ab63c8c955aaf71989efa641b906558d9fb7-8d8037e1aaabffe?api-version=2020-05-01
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
       - max-age=31536000; includeSubDomains
       x-content-type-options:
@@ -427,32 +477,32 @@
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.11 msrest_azure/0.6.2
-        azure-mgmt-batch/2020-03-01 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_certificates93b711ee/providers/Microsoft.Batch/batchAccounts/batch93b711ee/certificateOperationResults/sha1-cff2ab63c8c955aaf71989efa641b906558d9fb7-8d7dd7f7cdbe058?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_certificates93b711ee/providers/Microsoft.Batch/batchAccounts/batch93b711ee/certificateOperationResults/sha1-cff2ab63c8c955aaf71989efa641b906558d9fb7-8d8037e1aaabffe?api-version=2020-05-01
   response:
     body:
       string: ''
     headers:
       cache-control:
       - no-cache
       content-length:
       - '0'
       date:
-      - Fri, 10 Apr 2020 18:47:32 GMT
+      - Fri, 29 May 2020 03:13:22 GMT
       expires:
       - '-1'
       location:
-      - https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_certificates93b711ee/providers/Microsoft.Batch/batchAccounts/batch93b711ee/certificateOperationResults/sha1-cff2ab63c8c955aaf71989efa641b906558d9fb7-8d7dd7f7cdbe058?api-version=2020-03-01
+      - https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_certificates93b711ee/providers/Microsoft.Batch/batchAccounts/batch93b711ee/certificateOperationResults/sha1-cff2ab63c8c955aaf71989efa641b906558d9fb7-8d8037e1aaabffe?api-version=2020-05-01
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
       - max-age=31536000; includeSubDomains
       x-content-type-options:
@@ -466,28 +516,28 @@
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.11 msrest_azure/0.6.2
-        azure-mgmt-batch/2020-03-01 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_certificates93b711ee/providers/Microsoft.Batch/batchAccounts/batch93b711ee/certificateOperationResults/sha1-cff2ab63c8c955aaf71989efa641b906558d9fb7-8d7dd7f7cdbe058?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_batch_test_mgmt_batch_certificates93b711ee/providers/Microsoft.Batch/batchAccounts/batch93b711ee/certificateOperationResults/sha1-cff2ab63c8c955aaf71989efa641b906558d9fb7-8d8037e1aaabffe?api-version=2020-05-01
   response:
     body:
       string: ''
     headers:
       cache-control:
       - no-cache
       content-length:
       - '0'
       date:
-      - Fri, 10 Apr 2020 18:47:47 GMT
+      - Fri, 29 May 2020 03:13:37 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
```

## Comparing `azure-mgmt-batch-8.0.1/tests/recordings/test_mgmt_batch.test_mgmt_batch_account_name.yaml` & `azure-mgmt-batch-9.0.0/tests/recordings/test_mgmt_batch.test_mgmt_batch_account_name.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -9,33 +9,33 @@
       Connection:
       - keep-alive
       Content-Length:
       - '86'
       Content-Type:
       - application/json; charset=utf-8
       User-Agent:
-      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.11 msrest_azure/0.6.2
-        azure-mgmt-batch/2020-03-01 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: POST
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.Batch/locations/westcentralus/checkNameAvailability?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.Batch/locations/westcentralus/checkNameAvailability?api-version=2020-05-01
   response:
     body:
       string: '{"nameAvailable":false,"reason":"Invalid","message":"Account name must
         be at least 3 characters and at most 24 characters."}'
     headers:
       cache-control:
       - no-cache
       content-length:
       - '124'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Fri, 10 Apr 2020 18:44:56 GMT
+      - Fri, 29 May 2020 03:09:09 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
@@ -61,33 +61,33 @@
       Connection:
       - keep-alive
       Content-Length:
       - '61'
       Content-Type:
       - application/json; charset=utf-8
       User-Agent:
-      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.11 msrest_azure/0.6.2
-        azure-mgmt-batch/2020-03-01 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: POST
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.Batch/locations/westcentralus/checkNameAvailability?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.Batch/locations/westcentralus/checkNameAvailability?api-version=2020-05-01
   response:
     body:
       string: '{"nameAvailable":false,"reason":"AlreadyExists","message":"An account
         named ''sdktest2'' is already in use."}'
     headers:
       cache-control:
       - no-cache
       content-length:
       - '107'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Fri, 10 Apr 2020 18:44:56 GMT
+      - Fri, 29 May 2020 03:09:09 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
@@ -113,32 +113,32 @@
       Connection:
       - keep-alive
       Content-Length:
       - '66'
       Content-Type:
       - application/json; charset=utf-8
       User-Agent:
-      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.11 msrest_azure/0.6.2
-        azure-mgmt-batch/2020-03-01 Azure-SDK-For-Python
+      - python/3.7.3 (Windows-10-10.0.18362-SP0) msrest/0.6.14 msrest_azure/0.4.34
+        azure-mgmt-batch/9.0.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: POST
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.Batch/locations/westcentralus/checkNameAvailability?api-version=2020-03-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.Batch/locations/westcentralus/checkNameAvailability?api-version=2020-05-01
   response:
     body:
       string: '{"nameAvailable":true}'
     headers:
       cache-control:
       - no-cache
       content-length:
       - '22'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Fri, 10 Apr 2020 18:44:56 GMT
+      - Fri, 29 May 2020 03:09:10 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
```

