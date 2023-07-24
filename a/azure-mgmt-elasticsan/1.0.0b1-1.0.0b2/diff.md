# Comparing `tmp/azure-mgmt-elasticsan-1.0.0b1.zip` & `tmp/azure-mgmt-elasticsan-1.0.0b2.zip`

## zipinfo {}

```diff
@@ -1,57 +1,61 @@
-Zip file size: 83957 bytes, number of entries: 55
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-21 05:32 azure-mgmt-elasticsan-1.0.0b1/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-21 05:32 azure-mgmt-elasticsan-1.0.0b1/azure_mgmt_elasticsan.egg-info/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-21 05:32 azure-mgmt-elasticsan-1.0.0b1/azure/
--rw-rw-r--  2.0 unx     1367 b- defN 22-Oct-21 05:30 azure-mgmt-elasticsan-1.0.0b1/README.md
--rw-rw-r--  2.0 unx     1074 b- defN 22-Oct-21 05:30 azure-mgmt-elasticsan-1.0.0b1/LICENSE
--rw-rw-r--  2.0 unx      216 b- defN 22-Oct-21 05:30 azure-mgmt-elasticsan-1.0.0b1/MANIFEST.in
--rw-rw-r--  2.0 unx     2716 b- defN 22-Oct-21 05:30 azure-mgmt-elasticsan-1.0.0b1/setup.py
--rw-rw-r--  2.0 unx      564 b- defN 22-Oct-21 05:30 azure-mgmt-elasticsan-1.0.0b1/_meta.json
--rw-rw-r--  2.0 unx       62 b- defN 22-Oct-21 05:30 azure-mgmt-elasticsan-1.0.0b1/CHANGELOG.md
--rw-rw-r--  2.0 unx       38 b- defN 22-Oct-21 05:32 azure-mgmt-elasticsan-1.0.0b1/setup.cfg
--rw-rw-r--  2.0 unx     2273 b- defN 22-Oct-21 05:32 azure-mgmt-elasticsan-1.0.0b1/PKG-INFO
--rw-rw-r--  2.0 unx       62 b- defN 22-Oct-21 05:32 azure-mgmt-elasticsan-1.0.0b1/azure_mgmt_elasticsan.egg-info/requires.txt
--rw-rw-r--  2.0 unx        1 b- defN 22-Oct-21 05:32 azure-mgmt-elasticsan-1.0.0b1/azure_mgmt_elasticsan.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx     1785 b- defN 22-Oct-21 05:32 azure-mgmt-elasticsan-1.0.0b1/azure_mgmt_elasticsan.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx        6 b- defN 22-Oct-21 05:32 azure-mgmt-elasticsan-1.0.0b1/azure_mgmt_elasticsan.egg-info/top_level.txt
--rw-rw-r--  2.0 unx        1 b- defN 22-Oct-21 05:32 azure-mgmt-elasticsan-1.0.0b1/azure_mgmt_elasticsan.egg-info/not-zip-safe
--rw-rw-r--  2.0 unx     2273 b- defN 22-Oct-21 05:32 azure-mgmt-elasticsan-1.0.0b1/azure_mgmt_elasticsan.egg-info/PKG-INFO
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-21 05:32 azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/
--rw-rw-r--  2.0 unx       65 b- defN 22-Oct-21 05:30 azure-mgmt-elasticsan-1.0.0b1/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-21 05:32 azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/
--rw-rw-r--  2.0 unx       65 b- defN 22-Oct-21 05:30 azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-21 05:32 azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-21 05:32 azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-21 05:32 azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/models/
--rw-rw-r--  2.0 unx      488 b- defN 22-Oct-21 05:30 azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/_version.py
--rw-rw-r--  2.0 unx       26 b- defN 22-Oct-21 05:30 azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/py.typed
--rw-rw-r--  2.0 unx     5062 b- defN 22-Oct-21 05:30 azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/_elastic_san_management.py
--rw-rw-r--  2.0 unx      674 b- defN 22-Oct-21 05:30 azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/_patch.py
--rw-rw-r--  2.0 unx    77450 b- defN 22-Oct-21 05:30 azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/_serialization.py
--rw-rw-r--  2.0 unx     1169 b- defN 22-Oct-21 05:30 azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/_vendor.py
--rw-rw-r--  2.0 unx     3551 b- defN 22-Oct-21 05:30 azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/_configuration.py
--rw-rw-r--  2.0 unx      908 b- defN 22-Oct-21 05:30 azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-21 05:32 azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/aio/operations/
--rw-rw-r--  2.0 unx     5151 b- defN 22-Oct-21 05:30 azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/aio/_elastic_san_management.py
--rw-rw-r--  2.0 unx      674 b- defN 22-Oct-21 05:30 azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/aio/_patch.py
--rw-rw-r--  2.0 unx     3555 b- defN 22-Oct-21 05:30 azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/aio/_configuration.py
--rw-rw-r--  2.0 unx      855 b- defN 22-Oct-21 05:30 azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/aio/__init__.py
--rw-rw-r--  2.0 unx    39899 b- defN 22-Oct-21 05:30 azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/aio/operations/_elastic_sans_operations.py
--rw-rw-r--  2.0 unx     5815 b- defN 22-Oct-21 05:30 azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/aio/operations/_operations.py
--rw-rw-r--  2.0 unx    39496 b- defN 22-Oct-21 05:30 azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/aio/operations/_volumes_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 22-Oct-21 05:30 azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/aio/operations/_patch.py
--rw-rw-r--  2.0 unx    38190 b- defN 22-Oct-21 05:30 azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/aio/operations/_volume_groups_operations.py
--rw-rw-r--  2.0 unx     1100 b- defN 22-Oct-21 05:30 azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/aio/operations/__init__.py
--rw-rw-r--  2.0 unx     6187 b- defN 22-Oct-21 05:30 azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/aio/operations/_skus_operations.py
--rw-rw-r--  2.0 unx    48562 b- defN 22-Oct-21 05:30 azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/operations/_elastic_sans_operations.py
--rw-rw-r--  2.0 unx     6524 b- defN 22-Oct-21 05:30 azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/operations/_operations.py
--rw-rw-r--  2.0 unx    49956 b- defN 22-Oct-21 05:30 azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/operations/_volumes_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 22-Oct-21 05:30 azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/operations/_patch.py
--rw-rw-r--  2.0 unx    47502 b- defN 22-Oct-21 05:30 azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/operations/_volume_groups_operations.py
--rw-rw-r--  2.0 unx     1100 b- defN 22-Oct-21 05:30 azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/operations/__init__.py
--rw-rw-r--  2.0 unx     7299 b- defN 22-Oct-21 05:30 azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/operations/_skus_operations.py
--rw-rw-r--  2.0 unx    44544 b- defN 22-Oct-21 05:30 azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/models/_models_py3.py
--rw-rw-r--  2.0 unx      674 b- defN 22-Oct-21 05:30 azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/models/_patch.py
--rw-rw-r--  2.0 unx     2545 b- defN 22-Oct-21 05:30 azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/models/_elastic_san_management_enums.py
--rw-rw-r--  2.0 unx     3022 b- defN 22-Oct-21 05:30 azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/models/__init__.py
-55 files, 455894 bytes uncompressed, 72547 bytes compressed:  84.1%
+Zip file size: 102366 bytes, number of entries: 59
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-24 07:51 azure-mgmt-elasticsan-1.0.0b2/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-24 07:51 azure-mgmt-elasticsan-1.0.0b2/azure/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-24 07:51 azure-mgmt-elasticsan-1.0.0b2/azure_mgmt_elasticsan.egg-info/
+-rw-rw-r--  2.0 unx     1408 b- defN 23-Jul-24 07:50 azure-mgmt-elasticsan-1.0.0b2/CHANGELOG.md
+-rw-rw-r--  2.0 unx      216 b- defN 23-Jul-24 07:50 azure-mgmt-elasticsan-1.0.0b2/MANIFEST.in
+-rw-rw-r--  2.0 unx     2153 b- defN 23-Jul-24 07:50 azure-mgmt-elasticsan-1.0.0b2/README.md
+-rw-rw-r--  2.0 unx      628 b- defN 23-Jul-24 07:50 azure-mgmt-elasticsan-1.0.0b2/_meta.json
+-rw-rw-r--  2.0 unx     2846 b- defN 23-Jul-24 07:50 azure-mgmt-elasticsan-1.0.0b2/setup.py
+-rw-rw-r--  2.0 unx     4456 b- defN 23-Jul-24 07:51 azure-mgmt-elasticsan-1.0.0b2/PKG-INFO
+-rw-rw-r--  2.0 unx       38 b- defN 23-Jul-24 07:51 azure-mgmt-elasticsan-1.0.0b2/setup.cfg
+-rw-rw-r--  2.0 unx     1074 b- defN 23-Jul-24 07:50 azure-mgmt-elasticsan-1.0.0b2/LICENSE
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-24 07:51 azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/
+-rw-rw-r--  2.0 unx       65 b- defN 23-Jul-24 07:50 azure-mgmt-elasticsan-1.0.0b2/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-24 07:51 azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/
+-rw-rw-r--  2.0 unx       65 b- defN 23-Jul-24 07:50 azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-24 07:51 azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-24 07:51 azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-24 07:51 azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/models/
+-rw-rw-r--  2.0 unx       26 b- defN 23-Jul-24 07:50 azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/py.typed
+-rw-rw-r--  2.0 unx    78836 b- defN 23-Jul-24 07:50 azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/_serialization.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-24 07:50 azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/_patch.py
+-rw-rw-r--  2.0 unx     5882 b- defN 23-Jul-24 07:50 azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/_elastic_san_mgmt_client.py
+-rw-rw-r--  2.0 unx      901 b- defN 23-Jul-24 07:50 azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/__init__.py
+-rw-rw-r--  2.0 unx     1302 b- defN 23-Jul-24 07:50 azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/_vendor.py
+-rw-rw-r--  2.0 unx     3499 b- defN 23-Jul-24 07:50 azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/_configuration.py
+-rw-rw-r--  2.0 unx      488 b- defN 23-Jul-24 07:50 azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/_version.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-24 07:51 azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/aio/operations/
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-24 07:50 azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/aio/_patch.py
+-rw-rw-r--  2.0 unx     6042 b- defN 23-Jul-24 07:50 azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/aio/_elastic_san_mgmt_client.py
+-rw-rw-r--  2.0 unx      848 b- defN 23-Jul-24 07:50 azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/aio/__init__.py
+-rw-rw-r--  2.0 unx     3547 b- defN 23-Jul-24 07:50 azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/aio/_configuration.py
+-rw-rw-r--  2.0 unx    39727 b- defN 23-Jul-24 07:50 azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/aio/operations/_volumes_operations.py
+-rw-rw-r--  2.0 unx     5045 b- defN 23-Jul-24 07:50 azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/aio/operations/_private_link_resources_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-24 07:50 azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx    28534 b- defN 23-Jul-24 07:50 azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/aio/operations/_private_endpoint_connections_operations.py
+-rw-rw-r--  2.0 unx     1337 b- defN 23-Jul-24 07:50 azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx     6180 b- defN 23-Jul-24 07:50 azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/aio/operations/_skus_operations.py
+-rw-rw-r--  2.0 unx    38440 b- defN 23-Jul-24 07:50 azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/aio/operations/_volume_groups_operations.py
+-rw-rw-r--  2.0 unx    40154 b- defN 23-Jul-24 07:50 azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/aio/operations/_elastic_sans_operations.py
+-rw-rw-r--  2.0 unx     5734 b- defN 23-Jul-24 07:50 azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/aio/operations/_operations.py
+-rw-rw-r--  2.0 unx    49807 b- defN 23-Jul-24 07:50 azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/operations/_volumes_operations.py
+-rw-rw-r--  2.0 unx     6647 b- defN 23-Jul-24 07:50 azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/operations/_private_link_resources_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-24 07:50 azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/operations/_patch.py
+-rw-rw-r--  2.0 unx    35397 b- defN 23-Jul-24 07:50 azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/operations/_private_endpoint_connections_operations.py
+-rw-rw-r--  2.0 unx     1337 b- defN 23-Jul-24 07:50 azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/operations/__init__.py
+-rw-rw-r--  2.0 unx     7305 b- defN 23-Jul-24 07:50 azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/operations/_skus_operations.py
+-rw-rw-r--  2.0 unx    47372 b- defN 23-Jul-24 07:50 azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/operations/_volume_groups_operations.py
+-rw-rw-r--  2.0 unx    48450 b- defN 23-Jul-24 07:50 azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/operations/_elastic_sans_operations.py
+-rw-rw-r--  2.0 unx     6444 b- defN 23-Jul-24 07:50 azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/operations/_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-24 07:50 azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/models/_patch.py
+-rw-rw-r--  2.0 unx     3806 b- defN 23-Jul-24 07:50 azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/models/__init__.py
+-rw-rw-r--  2.0 unx     3286 b- defN 23-Jul-24 07:50 azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/models/_elastic_san_mgmt_client_enums.py
+-rw-rw-r--  2.0 unx    59254 b- defN 23-Jul-24 07:50 azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/models/_models_py3.py
+-rw-rw-r--  2.0 unx     2092 b- defN 23-Jul-24 07:51 azure-mgmt-elasticsan-1.0.0b2/azure_mgmt_elasticsan.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jul-24 07:51 azure-mgmt-elasticsan-1.0.0b2/azure_mgmt_elasticsan.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx        6 b- defN 23-Jul-24 07:51 azure-mgmt-elasticsan-1.0.0b2/azure_mgmt_elasticsan.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jul-24 07:51 azure-mgmt-elasticsan-1.0.0b2/azure_mgmt_elasticsan.egg-info/not-zip-safe
+-rw-rw-r--  2.0 unx      124 b- defN 23-Jul-24 07:51 azure-mgmt-elasticsan-1.0.0b2/azure_mgmt_elasticsan.egg-info/requires.txt
+-rw-rw-r--  2.0 unx     4456 b- defN 23-Jul-24 07:51 azure-mgmt-elasticsan-1.0.0b2/azure_mgmt_elasticsan.egg-info/PKG-INFO
+59 files, 558626 bytes uncompressed, 89806 bytes compressed:  83.9%
```

## zipnote {}

```diff
@@ -1,166 +1,178 @@
-Filename: azure-mgmt-elasticsan-1.0.0b1/
+Filename: azure-mgmt-elasticsan-1.0.0b2/
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure_mgmt_elasticsan.egg-info/
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure/
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure/
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure_mgmt_elasticsan.egg-info/
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/README.md
+Filename: azure-mgmt-elasticsan-1.0.0b2/CHANGELOG.md
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/LICENSE
+Filename: azure-mgmt-elasticsan-1.0.0b2/MANIFEST.in
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/MANIFEST.in
+Filename: azure-mgmt-elasticsan-1.0.0b2/README.md
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/setup.py
+Filename: azure-mgmt-elasticsan-1.0.0b2/_meta.json
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/_meta.json
+Filename: azure-mgmt-elasticsan-1.0.0b2/setup.py
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/CHANGELOG.md
+Filename: azure-mgmt-elasticsan-1.0.0b2/PKG-INFO
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/setup.cfg
+Filename: azure-mgmt-elasticsan-1.0.0b2/setup.cfg
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/PKG-INFO
+Filename: azure-mgmt-elasticsan-1.0.0b2/LICENSE
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure_mgmt_elasticsan.egg-info/requires.txt
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure_mgmt_elasticsan.egg-info/dependency_links.txt
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure/__init__.py
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure_mgmt_elasticsan.egg-info/SOURCES.txt
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure_mgmt_elasticsan.egg-info/top_level.txt
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/__init__.py
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure_mgmt_elasticsan.egg-info/not-zip-safe
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/aio/
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure_mgmt_elasticsan.egg-info/PKG-INFO
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/operations/
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/models/
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure/__init__.py
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/py.typed
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/_serialization.py
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/__init__.py
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/_patch.py
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/aio/
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/_elastic_san_mgmt_client.py
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/operations/
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/__init__.py
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/models/
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/_vendor.py
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/_version.py
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/py.typed
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/_version.py
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/_elastic_san_management.py
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/aio/operations/
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/_patch.py
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/aio/_patch.py
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/_serialization.py
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/aio/_elastic_san_mgmt_client.py
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/_vendor.py
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/aio/__init__.py
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/_configuration.py
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/aio/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/__init__.py
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/aio/operations/_volumes_operations.py
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/aio/operations/
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/aio/operations/_private_link_resources_operations.py
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/aio/_elastic_san_management.py
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/aio/_patch.py
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/aio/operations/_private_endpoint_connections_operations.py
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/aio/_configuration.py
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/aio/__init__.py
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/aio/operations/_skus_operations.py
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/aio/operations/_elastic_sans_operations.py
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/aio/operations/_volume_groups_operations.py
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/aio/operations/_operations.py
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/aio/operations/_elastic_sans_operations.py
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/aio/operations/_volumes_operations.py
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/aio/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/aio/operations/_patch.py
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/operations/_volumes_operations.py
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/aio/operations/_volume_groups_operations.py
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/operations/_private_link_resources_operations.py
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/aio/operations/__init__.py
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/operations/_patch.py
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/aio/operations/_skus_operations.py
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/operations/_private_endpoint_connections_operations.py
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/operations/_elastic_sans_operations.py
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/operations/_operations.py
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/operations/_skus_operations.py
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/operations/_volumes_operations.py
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/operations/_volume_groups_operations.py
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/operations/_patch.py
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/operations/_elastic_sans_operations.py
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/operations/_volume_groups_operations.py
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/operations/__init__.py
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/models/_patch.py
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/operations/_skus_operations.py
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/models/_models_py3.py
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/models/_elastic_san_mgmt_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/models/_patch.py
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/models/_elastic_san_management_enums.py
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure_mgmt_elasticsan.egg-info/SOURCES.txt
 Comment: 
 
-Filename: azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/models/__init__.py
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure_mgmt_elasticsan.egg-info/dependency_links.txt
+Comment: 
+
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure_mgmt_elasticsan.egg-info/top_level.txt
+Comment: 
+
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure_mgmt_elasticsan.egg-info/not-zip-safe
+Comment: 
+
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure_mgmt_elasticsan.egg-info/requires.txt
+Comment: 
+
+Filename: azure-mgmt-elasticsan-1.0.0b2/azure_mgmt_elasticsan.egg-info/PKG-INFO
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-mgmt-elasticsan-1.0.0b1/LICENSE` & `azure-mgmt-elasticsan-1.0.0b2/LICENSE`

 * *Files identical despite different names*

## Comparing `azure-mgmt-elasticsan-1.0.0b1/azure_mgmt_elasticsan.egg-info/SOURCES.txt` & `azure-mgmt-elasticsan-1.0.0b2/azure_mgmt_elasticsan.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -4,39 +4,43 @@
 README.md
 _meta.json
 setup.py
 azure/__init__.py
 azure/mgmt/__init__.py
 azure/mgmt/elasticsan/__init__.py
 azure/mgmt/elasticsan/_configuration.py
-azure/mgmt/elasticsan/_elastic_san_management.py
+azure/mgmt/elasticsan/_elastic_san_mgmt_client.py
 azure/mgmt/elasticsan/_patch.py
 azure/mgmt/elasticsan/_serialization.py
 azure/mgmt/elasticsan/_vendor.py
 azure/mgmt/elasticsan/_version.py
 azure/mgmt/elasticsan/py.typed
 azure/mgmt/elasticsan/aio/__init__.py
 azure/mgmt/elasticsan/aio/_configuration.py
-azure/mgmt/elasticsan/aio/_elastic_san_management.py
+azure/mgmt/elasticsan/aio/_elastic_san_mgmt_client.py
 azure/mgmt/elasticsan/aio/_patch.py
 azure/mgmt/elasticsan/aio/operations/__init__.py
 azure/mgmt/elasticsan/aio/operations/_elastic_sans_operations.py
 azure/mgmt/elasticsan/aio/operations/_operations.py
 azure/mgmt/elasticsan/aio/operations/_patch.py
+azure/mgmt/elasticsan/aio/operations/_private_endpoint_connections_operations.py
+azure/mgmt/elasticsan/aio/operations/_private_link_resources_operations.py
 azure/mgmt/elasticsan/aio/operations/_skus_operations.py
 azure/mgmt/elasticsan/aio/operations/_volume_groups_operations.py
 azure/mgmt/elasticsan/aio/operations/_volumes_operations.py
 azure/mgmt/elasticsan/models/__init__.py
-azure/mgmt/elasticsan/models/_elastic_san_management_enums.py
+azure/mgmt/elasticsan/models/_elastic_san_mgmt_client_enums.py
 azure/mgmt/elasticsan/models/_models_py3.py
 azure/mgmt/elasticsan/models/_patch.py
 azure/mgmt/elasticsan/operations/__init__.py
 azure/mgmt/elasticsan/operations/_elastic_sans_operations.py
 azure/mgmt/elasticsan/operations/_operations.py
 azure/mgmt/elasticsan/operations/_patch.py
+azure/mgmt/elasticsan/operations/_private_endpoint_connections_operations.py
+azure/mgmt/elasticsan/operations/_private_link_resources_operations.py
 azure/mgmt/elasticsan/operations/_skus_operations.py
 azure/mgmt/elasticsan/operations/_volume_groups_operations.py
 azure/mgmt/elasticsan/operations/_volumes_operations.py
 azure_mgmt_elasticsan.egg-info/PKG-INFO
 azure_mgmt_elasticsan.egg-info/SOURCES.txt
 azure_mgmt_elasticsan.egg-info/dependency_links.txt
 azure_mgmt_elasticsan.egg-info/not-zip-safe
```

## Comparing `azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/_elastic_san_management.py` & `azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/_elastic_san_mgmt_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,71 +8,91 @@
 
 from copy import deepcopy
 from typing import Any, TYPE_CHECKING
 
 from azure.core.rest import HttpRequest, HttpResponse
 from azure.mgmt.core import ARMPipelineClient
 
-from . import models
-from ._configuration import ElasticSanManagementConfiguration
+from . import models as _models
+from ._configuration import ElasticSanMgmtClientConfiguration
 from ._serialization import Deserializer, Serializer
-from .operations import ElasticSansOperations, Operations, SkusOperations, VolumeGroupsOperations, VolumesOperations
+from .operations import (
+    ElasticSansOperations,
+    Operations,
+    PrivateEndpointConnectionsOperations,
+    PrivateLinkResourcesOperations,
+    SkusOperations,
+    VolumeGroupsOperations,
+    VolumesOperations,
+)
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials import TokenCredential
 
 
-class ElasticSanManagement:  # pylint: disable=client-accepts-api-version-keyword
-    """ElasticSanManagement.
+class ElasticSanMgmtClient:  # pylint: disable=client-accepts-api-version-keyword,too-many-instance-attributes
+    """ElasticSanMgmtClient.
 
     :ivar operations: Operations operations
     :vartype operations: azure.mgmt.elasticsan.operations.Operations
     :ivar skus: SkusOperations operations
     :vartype skus: azure.mgmt.elasticsan.operations.SkusOperations
     :ivar elastic_sans: ElasticSansOperations operations
     :vartype elastic_sans: azure.mgmt.elasticsan.operations.ElasticSansOperations
     :ivar volume_groups: VolumeGroupsOperations operations
     :vartype volume_groups: azure.mgmt.elasticsan.operations.VolumeGroupsOperations
     :ivar volumes: VolumesOperations operations
     :vartype volumes: azure.mgmt.elasticsan.operations.VolumesOperations
+    :ivar private_endpoint_connections: PrivateEndpointConnectionsOperations operations
+    :vartype private_endpoint_connections:
+     azure.mgmt.elasticsan.operations.PrivateEndpointConnectionsOperations
+    :ivar private_link_resources: PrivateLinkResourcesOperations operations
+    :vartype private_link_resources:
+     azure.mgmt.elasticsan.operations.PrivateLinkResourcesOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
-    :keyword api_version: Api Version. Default value is "2021-11-20-preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2022-12-01-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(
         self,
         credential: "TokenCredential",
         subscription_id: str,
         base_url: str = "https://management.azure.com",
         **kwargs: Any
     ) -> None:
-        self._config = ElasticSanManagementConfiguration(
+        self._config = ElasticSanMgmtClientConfiguration(
             credential=credential, subscription_id=subscription_id, **kwargs
         )
-        self._client = ARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
+        self._client: ARMPipelineClient = ARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
 
-        client_models = {k: v for k, v in models.__dict__.items() if isinstance(v, type)}
+        client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
         self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
         self.skus = SkusOperations(self._client, self._config, self._serialize, self._deserialize)
         self.elastic_sans = ElasticSansOperations(self._client, self._config, self._serialize, self._deserialize)
         self.volume_groups = VolumeGroupsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.volumes = VolumesOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.private_endpoint_connections = PrivateEndpointConnectionsOperations(
+            self._client, self._config, self._serialize, self._deserialize
+        )
+        self.private_link_resources = PrivateLinkResourcesOperations(
+            self._client, self._config, self._serialize, self._deserialize
+        )
 
     def _send_request(self, request: HttpRequest, **kwargs: Any) -> HttpResponse:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
         >>> request = HttpRequest("GET", "https://www.example.org/")
         <HttpRequest [GET], url: 'https://www.example.org/'>
@@ -88,19 +108,16 @@
         :rtype: ~azure.core.rest.HttpResponse
         """
 
         request_copy = deepcopy(request)
         request_copy.url = self._client.format_url(request_copy.url)
         return self._client.send_request(request_copy, **kwargs)
 
-    def close(self):
-        # type: () -> None
+    def close(self) -> None:
         self._client.close()
 
-    def __enter__(self):
-        # type: () -> ElasticSanManagement
+    def __enter__(self) -> "ElasticSanMgmtClient":
         self._client.__enter__()
         return self
 
-    def __exit__(self, *exc_details):
-        # type: (Any) -> None
+    def __exit__(self, *exc_details: Any) -> None:
         self._client.__exit__(*exc_details)
```

## Comparing `azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/_patch.py` & `azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/_serialization.py` & `azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/_serialization.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,56 +21,71 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
 # IN THE SOFTWARE.
 #
 # --------------------------------------------------------------------------
 
 # pylint: skip-file
+# pyright: reportUnnecessaryTypeIgnoreComment=false
 
 from base64 import b64decode, b64encode
 import calendar
 import datetime
 import decimal
 import email
 from enum import Enum
 import json
 import logging
 import re
 import sys
 import codecs
+from typing import (
+    Dict,
+    Any,
+    cast,
+    Optional,
+    Union,
+    AnyStr,
+    IO,
+    Mapping,
+    Callable,
+    TypeVar,
+    MutableMapping,
+    Type,
+    List,
+    Mapping,
+)
 
 try:
     from urllib import quote  # type: ignore
 except ImportError:
-    from urllib.parse import quote  # type: ignore
+    from urllib.parse import quote
 import xml.etree.ElementTree as ET
 
-import isodate
-
-from typing import Dict, Any, cast, TYPE_CHECKING
+import isodate  # type: ignore
 
 from azure.core.exceptions import DeserializationError, SerializationError, raise_with_traceback
+from azure.core.serialization import NULL as AzureCoreNull
 
 _BOM = codecs.BOM_UTF8.decode(encoding="utf-8")
 
-if TYPE_CHECKING:
-    from typing import Optional, Union, AnyStr, IO, Mapping
+ModelType = TypeVar("ModelType", bound="Model")
+JSON = MutableMapping[str, Any]
 
 
 class RawDeserializer:
 
     # Accept "text" because we're open minded people...
     JSON_REGEXP = re.compile(r"^(application|text)/([a-z+.]+\+)?json$")
 
     # Name used in context
     CONTEXT_NAME = "deserialized_data"
 
     @classmethod
-    def deserialize_from_text(cls, data, content_type=None):
-        # type: (Optional[Union[AnyStr, IO]], Optional[str]) -> Any
+    def deserialize_from_text(cls, data: Optional[Union[AnyStr, IO]], content_type: Optional[str] = None) -> Any:
         """Decode data according to content-type.
 
         Accept a stream of data as well, but will be load at once in memory for now.
 
         If no content-type, will return the string version (not bytes, not stream)
 
         :param data: Input, could be bytes or stream (will be decoded with UTF8) or text
@@ -128,16 +143,15 @@
                 # The function hack is because Py2.7 messes up with exception
                 # context otherwise.
                 _LOGGER.critical("Wasn't XML not JSON, failing")
                 raise_with_traceback(DeserializationError, "XML is invalid")
         raise DeserializationError("Cannot deserialize content-type: {}".format(content_type))
 
     @classmethod
-    def deserialize_from_http_generics(cls, body_bytes, headers):
-        # type: (Optional[Union[AnyStr, IO]], Mapping) -> Any
+    def deserialize_from_http_generics(cls, body_bytes: Optional[Union[AnyStr, IO]], headers: Mapping) -> Any:
         """Deserialize from HTTP response.
 
         Use bytes and headers to NOT use any requests/aiohttp or whatever
         specific implementation.
         Headers will tested for "content-type"
         """
         # Try to use content-type from headers if available
@@ -156,16 +170,16 @@
         return None
 
 
 try:
     basestring  # type: ignore
     unicode_str = unicode  # type: ignore
 except NameError:
-    basestring = str  # type: ignore
-    unicode_str = str  # type: ignore
+    basestring = str
+    unicode_str = str
 
 _LOGGER = logging.getLogger(__name__)
 
 try:
     _long_type = long  # type: ignore
 except NameError:
     _long_type = int
@@ -184,15 +198,15 @@
 
     def dst(self, dt):
         """No daylight saving for UTC."""
         return datetime.timedelta(hours=1)
 
 
 try:
-    from datetime import timezone as _FixedOffset
+    from datetime import timezone as _FixedOffset  # type: ignore
 except ImportError:  # Python 2.7
 
     class _FixedOffset(datetime.tzinfo):  # type: ignore
         """Fixed offset in minutes east from UTC.
         Copy/pasted from Python doc
         :param datetime.timedelta offset: offset in timedelta format
         """
@@ -215,15 +229,15 @@
         def __getinitargs__(self):
             return (self.__offset,)
 
 
 try:
     from datetime import timezone
 
-    TZ_UTC = timezone.utc  # type: ignore
+    TZ_UTC = timezone.utc
 except ImportError:
     TZ_UTC = UTC()  # type: ignore
 
 _FLATTEN = re.compile(r"(?<!\\)\.")
 
 
 def attribute_transformer(key, attr_desc, value):
@@ -272,79 +286,84 @@
 
 
 class Model(object):
     """Mixin for all client request body/response body models to support
     serialization and deserialization.
     """
 
-    _subtype_map = {}  # type: Dict[str, Dict[str, Any]]
-    _attribute_map = {}  # type: Dict[str, Dict[str, Any]]
-    _validation = {}  # type: Dict[str, Dict[str, Any]]
+    _subtype_map: Dict[str, Dict[str, Any]] = {}
+    _attribute_map: Dict[str, Dict[str, Any]] = {}
+    _validation: Dict[str, Dict[str, Any]] = {}
 
-    def __init__(self, **kwargs):
-        self.additional_properties = {}
+    def __init__(self, **kwargs: Any) -> None:
+        self.additional_properties: Dict[str, Any] = {}
         for k in kwargs:
             if k not in self._attribute_map:
                 _LOGGER.warning("%s is not a known attribute of class %s and will be ignored", k, self.__class__)
             elif k in self._validation and self._validation[k].get("readonly", False):
                 _LOGGER.warning("Readonly attribute %s will be ignored in class %s", k, self.__class__)
             else:
                 setattr(self, k, kwargs[k])
 
-    def __eq__(self, other):
+    def __eq__(self, other: Any) -> bool:
         """Compare objects by comparing all attributes."""
         if isinstance(other, self.__class__):
             return self.__dict__ == other.__dict__
         return False
 
-    def __ne__(self, other):
+    def __ne__(self, other: Any) -> bool:
         """Compare objects by comparing all attributes."""
         return not self.__eq__(other)
 
-    def __str__(self):
+    def __str__(self) -> str:
         return str(self.__dict__)
 
     @classmethod
-    def enable_additional_properties_sending(cls):
+    def enable_additional_properties_sending(cls) -> None:
         cls._attribute_map["additional_properties"] = {"key": "", "type": "{object}"}
 
     @classmethod
-    def is_xml_model(cls):
+    def is_xml_model(cls) -> bool:
         try:
-            cls._xml_map
+            cls._xml_map  # type: ignore
         except AttributeError:
             return False
         return True
 
     @classmethod
     def _create_xml_node(cls):
         """Create XML node."""
         try:
-            xml_map = cls._xml_map
+            xml_map = cls._xml_map  # type: ignore
         except AttributeError:
             xml_map = {}
 
         return _create_xml_node(xml_map.get("name", cls.__name__), xml_map.get("prefix", None), xml_map.get("ns", None))
 
-    def serialize(self, keep_readonly=False, **kwargs):
+    def serialize(self, keep_readonly: bool = False, **kwargs: Any) -> JSON:
         """Return the JSON that would be sent to azure from this model.
 
         This is an alias to `as_dict(full_restapi_key_transformer, keep_readonly=False)`.
 
         If you want XML serialization, you can pass the kwargs is_xml=True.
 
         :param bool keep_readonly: If you want to serialize the readonly attributes
         :returns: A dict JSON compatible object
         :rtype: dict
         """
         serializer = Serializer(self._infer_class_models())
         return serializer._serialize(self, keep_readonly=keep_readonly, **kwargs)
 
-    def as_dict(self, keep_readonly=True, key_transformer=attribute_transformer, **kwargs):
-        """Return a dict that can be JSONify using json.dump.
+    def as_dict(
+        self,
+        keep_readonly: bool = True,
+        key_transformer: Callable[[str, Dict[str, Any], Any], Any] = attribute_transformer,
+        **kwargs: Any
+    ) -> JSON:
+        """Return a dict that can be serialized using json.dump.
 
         Advanced usage might optionally use a callback as parameter:
 
         .. code::python
 
             def my_key_transformer(key, attr_desc, value):
                 return key
@@ -383,41 +402,46 @@
                 raise ValueError("Not Autorest generated code")
         except Exception:
             # Assume it's not Autorest generated (tests?). Add ourselves as dependencies.
             client_models = {cls.__name__: cls}
         return client_models
 
     @classmethod
-    def deserialize(cls, data, content_type=None):
+    def deserialize(cls: Type[ModelType], data: Any, content_type: Optional[str] = None) -> ModelType:
         """Parse a str using the RestAPI syntax and return a model.
 
         :param str data: A str using RestAPI structure. JSON by default.
         :param str content_type: JSON by default, set application/xml if XML.
         :returns: An instance of this model
         :raises: DeserializationError if something went wrong
         """
         deserializer = Deserializer(cls._infer_class_models())
         return deserializer(cls.__name__, data, content_type=content_type)
 
     @classmethod
-    def from_dict(cls, data, key_extractors=None, content_type=None):
+    def from_dict(
+        cls: Type[ModelType],
+        data: Any,
+        key_extractors: Optional[Callable[[str, Dict[str, Any], Any], Any]] = None,
+        content_type: Optional[str] = None,
+    ) -> ModelType:
         """Parse a dict using given key extractor return a model.
 
         By default consider key
         extractors (rest_key_case_insensitive_extractor, attribute_key_case_insensitive_extractor
         and last_rest_key_case_insensitive_extractor)
 
         :param dict data: A dict using RestAPI structure
         :param str content_type: JSON by default, set application/xml if XML.
         :returns: An instance of this model
         :raises: DeserializationError if something went wrong
         """
         deserializer = Deserializer(cls._infer_class_models())
-        deserializer.key_extractors = (
-            [
+        deserializer.key_extractors = (  # type: ignore
+            [  # type: ignore
                 attribute_key_case_insensitive_extractor,
                 rest_key_case_insensitive_extractor,
                 last_rest_key_case_insensitive_extractor,
             ]
             if key_extractors is None
             else key_extractors
         )
@@ -449,15 +473,15 @@
             if subtype_value:
                 # Try to match base class. Can be class name only
                 # (bug to fix in Autorest to support x-ms-discriminator-name)
                 if cls.__name__ == subtype_value:
                     return cls
                 flatten_mapping_type = cls._flatten_subtype(subtype_key, objects)
                 try:
-                    return objects[flatten_mapping_type[subtype_value]]
+                    return objects[flatten_mapping_type[subtype_value]]  # type: ignore
                 except KeyError:
                     _LOGGER.warning(
                         "Subtype value %s has no mapping, use base class %s.",
                         subtype_value,
                         cls.__name__,
                     )
                     break
@@ -517,15 +541,15 @@
         "min_items": lambda x, y: len(x) < y,
         "max_items": lambda x, y: len(x) > y,
         "pattern": lambda x, y: not re.match(y, x, re.UNICODE),
         "unique": lambda x, y: len(x) != len(set(x)),
         "multiple": lambda x, y: x % y != 0,
     }
 
-    def __init__(self, classes=None):
+    def __init__(self, classes: Optional[Mapping[str, Type[ModelType]]] = None):
         self.serialize_type = {
             "iso-8601": Serializer.serialize_iso,
             "rfc-1123": Serializer.serialize_rfc,
             "unix-time": Serializer.serialize_unix,
             "duration": Serializer.serialize_duration,
             "date": Serializer.serialize_date,
             "time": Serializer.serialize_time,
@@ -533,15 +557,15 @@
             "long": Serializer.serialize_long,
             "bytearray": Serializer.serialize_bytearray,
             "base64": Serializer.serialize_base64,
             "object": self.serialize_object,
             "[]": self.serialize_iter,
             "{}": self.serialize_dict,
         }
-        self.dependencies = dict(classes) if classes else {}
+        self.dependencies: Dict[str, Type[ModelType]] = dict(classes) if classes else {}
         self.key_transformer = full_restapi_key_transformer
         self.client_side_validation = True
 
     def _serialize(self, target_obj, data_type=None, **kwargs):
         """Serialize data into a string according to type.
 
         :param target_obj: The data to be serialized.
@@ -601,47 +625,46 @@
                         xml_desc = attr_desc.get("xml", {})
                         xml_name = xml_desc.get("name", attr_desc["key"])
                         xml_prefix = xml_desc.get("prefix", None)
                         xml_ns = xml_desc.get("ns", None)
                         if xml_desc.get("attr", False):
                             if xml_ns:
                                 ET.register_namespace(xml_prefix, xml_ns)
-                                xml_name = "{}{}".format(xml_ns, xml_name)
-                            serialized.set(xml_name, new_attr)
+                                xml_name = "{{{}}}{}".format(xml_ns, xml_name)
+                            serialized.set(xml_name, new_attr)  # type: ignore
                             continue
                         if xml_desc.get("text", False):
-                            serialized.text = new_attr
+                            serialized.text = new_attr  # type: ignore
                             continue
                         if isinstance(new_attr, list):
-                            serialized.extend(new_attr)
+                            serialized.extend(new_attr)  # type: ignore
                         elif isinstance(new_attr, ET.Element):
                             # If the down XML has no XML/Name, we MUST replace the tag with the local tag. But keeping the namespaces.
                             if "name" not in getattr(orig_attr, "_xml_map", {}):
                                 splitted_tag = new_attr.tag.split("}")
                                 if len(splitted_tag) == 2:  # Namespace
                                     new_attr.tag = "}".join([splitted_tag[0], xml_name])
                                 else:
                                     new_attr.tag = xml_name
-                            serialized.append(new_attr)
+                            serialized.append(new_attr)  # type: ignore
                         else:  # That's a basic type
                             # Integrate namespace if necessary
                             local_node = _create_xml_node(xml_name, xml_prefix, xml_ns)
                             local_node.text = unicode_str(new_attr)
-                            serialized.append(local_node)
+                            serialized.append(local_node)  # type: ignore
                     else:  # JSON
-                        for k in reversed(keys):
-                            unflattened = {k: new_attr}
-                            new_attr = unflattened
+                        for k in reversed(keys):  # type: ignore
+                            new_attr = {k: new_attr}
 
                         _new_attr = new_attr
                         _serialized = serialized
-                        for k in keys:
+                        for k in keys:  # type: ignore
                             if k not in _serialized:
-                                _serialized.update(_new_attr)
-                            _new_attr = _new_attr[k]
+                                _serialized.update(_new_attr)  # type: ignore
+                            _new_attr = _new_attr[k]  # type: ignore
                             _serialized = _serialized[k]
                 except ValueError:
                     continue
 
         except (AttributeError, KeyError, TypeError) as err:
             msg = "Attribute {} in object {} cannot be serialized.\n{}".format(attr_name, class_name, str(target_obj))
             raise_with_traceback(SerializationError, msg, err)
@@ -655,31 +678,31 @@
         :param str data_type: The type to be serialized from.
         :rtype: dict
         :raises: SerializationError if serialization fails.
         :raises: ValueError if data is None
         """
 
         # Just in case this is a dict
-        internal_data_type = data_type.strip("[]{}")
-        internal_data_type = self.dependencies.get(internal_data_type, None)
+        internal_data_type_str = data_type.strip("[]{}")
+        internal_data_type = self.dependencies.get(internal_data_type_str, None)
         try:
             is_xml_model_serialization = kwargs["is_xml"]
         except KeyError:
             if internal_data_type and issubclass(internal_data_type, Model):
                 is_xml_model_serialization = kwargs.setdefault("is_xml", internal_data_type.is_xml_model())
             else:
                 is_xml_model_serialization = False
         if internal_data_type and not isinstance(internal_data_type, Enum):
             try:
                 deserializer = Deserializer(self.dependencies)
                 # Since it's on serialization, it's almost sure that format is not JSON REST
                 # We're not able to deal with additional properties for now.
                 deserializer.additional_properties_detection = False
                 if is_xml_model_serialization:
-                    deserializer.key_extractors = [
+                    deserializer.key_extractors = [  # type: ignore
                         attribute_key_case_insensitive_extractor,
                     ]
                 else:
                     deserializer.key_extractors = [
                         rest_key_case_insensitive_extractor,
                         attribute_key_case_insensitive_extractor,
                         last_rest_key_case_insensitive_extractor,
@@ -776,14 +799,16 @@
         :raises: ValueError if data is None
         :raises: SerializationError if serialization fails.
         """
         if data is None:
             raise ValueError("No value for given attribute")
 
         try:
+            if data is AzureCoreNull:
+                return None
             if data_type in self.basic_types.values():
                 return self.serialize_basic(data, data_type, **kwargs)
 
             elif data_type in self.serialize_type:
                 return self.serialize_type[data_type](data, **kwargs)
 
             # If dependencies is empty, try with current data class
@@ -839,15 +864,15 @@
         """
         try:  # If I received an enum, return its value
             return data.value
         except AttributeError:
             pass
 
         try:
-            if isinstance(data, unicode):
+            if isinstance(data, unicode):  # type: ignore
                 # Don't change it, JSON and XML ElementTree are totally able
                 # to serialize correctly u'' strings
                 return data
         except NameError:
             return str(data)
         else:
             return str(data)
@@ -997,18 +1022,18 @@
     @staticmethod
     def serialize_enum(attr, enum_obj=None):
         try:
             result = attr.value
         except AttributeError:
             result = attr
         try:
-            enum_obj(result)
+            enum_obj(result)  # type: ignore
             return result
         except ValueError:
-            for enum_value in enum_obj:
+            for enum_value in enum_obj:  # type: ignore
                 if enum_value.value.lower() == str(attr).lower():
                     return enum_value.value
             error = "{!r} is not valid value for enum {!r}"
             raise SerializationError(error.format(attr, enum_obj))
 
     @staticmethod
     def serialize_bytearray(attr, **kwargs):
@@ -1160,15 +1185,16 @@
 
 
 def rest_key_extractor(attr, attr_desc, data):
     key = attr_desc["key"]
     working_data = data
 
     while "." in key:
-        dict_keys = _FLATTEN.split(key)
+        # Need the cast, as for some reasons "split" is typed as list[str | Any]
+        dict_keys = cast(List[str], _FLATTEN.split(key))
         if len(dict_keys) == 1:
             key = _decode_attribute_map_key(dict_keys[0])
             break
         working_key = _decode_attribute_map_key(dict_keys[0])
         working_data = working_data.get(working_key, data)
         if working_data is None:
             # If at any point while following flatten JSON path see None, it means
@@ -1241,15 +1267,15 @@
     :rtype: tuple
     :returns: A tuple XML name + namespace dict
     """
     internal_type_xml_map = getattr(internal_type, "_xml_map", {})
     xml_name = internal_type_xml_map.get("name", internal_type.__name__)
     xml_ns = internal_type_xml_map.get("ns", None)
     if xml_ns:
-        xml_name = "{}{}".format(xml_ns, xml_name)
+        xml_name = "{{{}}}{}".format(xml_ns, xml_name)
     return xml_name
 
 
 def xml_key_extractor(attr, attr_desc, data):
     if isinstance(data, dict):
         return None
 
@@ -1265,15 +1291,15 @@
     is_wrapped = xml_desc.get("wrapped", False)
     internal_type = attr_desc.get("internalType", None)
     internal_type_xml_map = getattr(internal_type, "_xml_map", {})
 
     # Integrate namespace if necessary
     xml_ns = xml_desc.get("ns", internal_type_xml_map.get("ns", None))
     if xml_ns:
-        xml_name = "{}{}".format(xml_ns, xml_name)
+        xml_name = "{{{}}}{}".format(xml_ns, xml_name)
 
     # If it's an attribute, that's simple
     if xml_desc.get("attr", False):
         return data.get(xml_name)
 
     # If it's x-ms-text, that's simple too
     if xml_desc.get("text", False):
@@ -1331,15 +1357,15 @@
     :ivar list key_extractors: Ordered list of extractors to be used by this deserializer.
     """
 
     basic_types = {str: "str", int: "int", bool: "bool", float: "float"}
 
     valid_date = re.compile(r"\d{4}[-]\d{2}[-]\d{2}T\d{2}:\d{2}:\d{2}" r"\.?\d*Z?[-+]?[\d{2}]?:?[\d{2}]?")
 
-    def __init__(self, classes=None):
+    def __init__(self, classes: Optional[Mapping[str, Type[ModelType]]] = None):
         self.deserialize_type = {
             "iso-8601": Deserializer.deserialize_iso,
             "rfc-1123": Deserializer.deserialize_rfc,
             "unix-time": Deserializer.deserialize_unix,
             "duration": Deserializer.deserialize_duration,
             "date": Deserializer.deserialize_date,
             "time": Deserializer.deserialize_time,
@@ -1351,15 +1377,15 @@
             "[]": self.deserialize_iter,
             "{}": self.deserialize_dict,
         }
         self.deserialize_expected_types = {
             "duration": (isodate.Duration, datetime.timedelta),
             "iso-8601": (datetime.datetime),
         }
-        self.dependencies = dict(classes) if classes else {}
+        self.dependencies: Dict[str, Type[ModelType]] = dict(classes) if classes else {}
         self.key_extractors = [rest_key_extractor, xml_key_extractor]
         # Additional properties only works if the "rest_key_extractor" is used to
         # extract the keys. Making it to work whatever the key extractor is too much
         # complicated, with no real scenario for now.
         # So adding a flag to disable additional properties detection. This flag should be
         # used if your expect the deserialization to NOT come from a JSON REST syntax.
         # Otherwise, result are unexpected
@@ -1412,15 +1438,15 @@
             return self.deserialize_data(data, response)
         elif isinstance(response, type) and issubclass(response, Enum):
             return self.deserialize_enum(data, response)
 
         if data is None:
             return data
         try:
-            attributes = response._attribute_map
+            attributes = response._attribute_map  # type: ignore
             d_attrs = {}
             for attr, attr_desc in attributes.items():
                 # Check empty string. If it's not empty, someone has a real "additionalProperties"...
                 if attr == "additional_properties" and attr_desc["key"] == "":
                     continue
                 raw_value = None
                 # Enhance attr_desc with some dynamic data
@@ -1440,15 +1466,15 @@
                             _LOGGER.warning(msg, found_value, key_extractor, attr)
                             continue
                         raw_value = found_value
 
                 value = self.deserialize_data(raw_value, attr_desc["type"])
                 d_attrs[attr] = value
         except (AttributeError, TypeError, KeyError) as err:
-            msg = "Unable to deserialize to object: " + class_name
+            msg = "Unable to deserialize to object: " + class_name  # type: ignore
             raise_with_traceback(DeserializationError, msg, err)
         else:
             additional_properties = self._build_additional_properties(attributes, data)
             return self._instantiate_model(response, d_attrs, additional_properties)
 
     def _build_additional_properties(self, attribute_map, data):
         if not self.additional_properties_detection:
@@ -1470,40 +1496,40 @@
 
     def _classify_target(self, target, data):
         """Check to see whether the deserialization target object can
         be classified into a subclass.
         Once classification has been determined, initialize object.
 
         :param str target: The target object type to deserialize to.
-        :param str/dict data: The response data to deseralize.
+        :param str/dict data: The response data to deserialize.
         """
         if target is None:
             return None, None
 
         if isinstance(target, basestring):
             try:
                 target = self.dependencies[target]
             except KeyError:
                 return target, target
 
         try:
             target = target._classify(data, self.dependencies)
         except AttributeError:
             pass  # Target is not a Model, no classify
-        return target, target.__class__.__name__
+        return target, target.__class__.__name__  # type: ignore
 
     def failsafe_deserialize(self, target_obj, data, content_type=None):
         """Ignores any errors encountered in deserialization,
         and falls back to not deserializing the object. Recommended
         for use in error deserialization, as we want to return the
         HttpResponseError to users, and not have them deal with
         a deserialization error.
 
         :param str target_obj: The target object type to deserialize to.
-        :param str/dict data: The response data to deseralize.
+        :param str/dict data: The response data to deserialize.
         :param str content_type: Swagger "produces" if available.
         """
         try:
             return self(target_obj, data, content_type=content_type)
         except:
             _LOGGER.debug(
                 "Ran into a deserialization error. Ignoring since this is failsafe deserialization", exc_info=True
@@ -1539,15 +1565,15 @@
             return RawDeserializer.deserialize_from_http_generics(raw_data.text(), raw_data.headers)
 
         # Assume this enough to recognize requests.Response without importing it.
         if hasattr(raw_data, "_content_consumed"):
             return RawDeserializer.deserialize_from_http_generics(raw_data.text, raw_data.headers)
 
         if isinstance(raw_data, (basestring, bytes)) or hasattr(raw_data, "read"):
-            return RawDeserializer.deserialize_from_text(raw_data, content_type)
+            return RawDeserializer.deserialize_from_text(raw_data, content_type)  # type: ignore
         return raw_data
 
     def _instantiate_model(self, response, attrs, additional_properties=None):
         """Instantiate a response model passing in deserialized args.
 
         :param response: The response model class.
         :param d_attrs: The deserialized response attributes.
@@ -1561,15 +1587,15 @@
                 response_obj = response(**kwargs)
                 for attr in readonly:
                     setattr(response_obj, attr, attrs.get(attr))
                 if additional_properties:
                     response_obj.additional_properties = additional_properties
                 return response_obj
             except TypeError as err:
-                msg = "Unable to deserialize {} into model {}. ".format(kwargs, response)
+                msg = "Unable to deserialize {} into model {}. ".format(kwargs, response)  # type: ignore
                 raise DeserializationError(msg + str(err))
         else:
             try:
                 for attr, value in attrs.items():
                     setattr(response, attr, value)
                 return response
             except Exception as exp:
@@ -1743,15 +1769,15 @@
         # We might be here because we have an enum modeled as string,
         # and we try to deserialize a partial dict with enum inside
         if isinstance(data, Enum):
             return data
 
         # Consider this is real string
         try:
-            if isinstance(data, unicode):
+            if isinstance(data, unicode):  # type: ignore
                 return data
         except NameError:
             return str(data)
         else:
             return str(data)
 
     @staticmethod
@@ -1794,58 +1820,58 @@
 
         :param str attr: response string to be deserialized.
         :rtype: bytearray
         :raises: TypeError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
-        return bytearray(b64decode(attr))
+        return bytearray(b64decode(attr))  # type: ignore
 
     @staticmethod
     def deserialize_base64(attr):
         """Deserialize base64 encoded string into string.
 
         :param str attr: response string to be deserialized.
         :rtype: bytearray
         :raises: TypeError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
-        padding = "=" * (3 - (len(attr) + 3) % 4)
-        attr = attr + padding
+        padding = "=" * (3 - (len(attr) + 3) % 4)  # type: ignore
+        attr = attr + padding  # type: ignore
         encoded = attr.replace("-", "+").replace("_", "/")
         return b64decode(encoded)
 
     @staticmethod
     def deserialize_decimal(attr):
         """Deserialize string into Decimal object.
 
         :param str attr: response string to be deserialized.
         :rtype: Decimal
         :raises: DeserializationError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
         try:
-            return decimal.Decimal(attr)
+            return decimal.Decimal(attr)  # type: ignore
         except decimal.DecimalException as err:
             msg = "Invalid decimal {}".format(attr)
             raise_with_traceback(DeserializationError, msg, err)
 
     @staticmethod
     def deserialize_long(attr):
         """Deserialize string into long (Py2) or int (Py3).
 
         :param str attr: response string to be deserialized.
         :rtype: long or int
         :raises: ValueError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
-        return _long_type(attr)
+        return _long_type(attr)  # type: ignore
 
     @staticmethod
     def deserialize_duration(attr):
         """Deserialize ISO-8601 formatted string into TimeDelta object.
 
         :param str attr: response string to be deserialized.
         :rtype: TimeDelta
@@ -1867,45 +1893,45 @@
 
         :param str attr: response string to be deserialized.
         :rtype: Date
         :raises: DeserializationError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
-        if re.search(r"[^\W\d_]", attr, re.I + re.U):
+        if re.search(r"[^\W\d_]", attr, re.I + re.U):  # type: ignore
             raise DeserializationError("Date must have only digits and -. Received: %s" % attr)
         # This must NOT use defaultmonth/defaultday. Using None ensure this raises an exception.
         return isodate.parse_date(attr, defaultmonth=None, defaultday=None)
 
     @staticmethod
     def deserialize_time(attr):
         """Deserialize ISO-8601 formatted string into time object.
 
         :param str attr: response string to be deserialized.
         :rtype: datetime.time
         :raises: DeserializationError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
-        if re.search(r"[^\W\d_]", attr, re.I + re.U):
+        if re.search(r"[^\W\d_]", attr, re.I + re.U):  # type: ignore
             raise DeserializationError("Date must have only digits and -. Received: %s" % attr)
         return isodate.parse_time(attr)
 
     @staticmethod
     def deserialize_rfc(attr):
         """Deserialize RFC-1123 formatted string into Datetime object.
 
         :param str attr: response string to be deserialized.
         :rtype: Datetime
         :raises: DeserializationError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
         try:
-            parsed_date = email.utils.parsedate_tz(attr)
+            parsed_date = email.utils.parsedate_tz(attr)  # type: ignore
             date_obj = datetime.datetime(
                 *parsed_date[:6], tzinfo=_FixedOffset(datetime.timedelta(minutes=(parsed_date[9] or 0) / 60))
             )
             if not date_obj.tzinfo:
                 date_obj = date_obj.astimezone(tz=TZ_UTC)
         except ValueError as err:
             msg = "Cannot deserialize to rfc datetime object."
@@ -1920,15 +1946,15 @@
         :param str attr: response string to be deserialized.
         :rtype: Datetime
         :raises: DeserializationError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
         try:
-            attr = attr.upper()
+            attr = attr.upper()  # type: ignore
             match = Deserializer.valid_date.match(attr)
             if not match:
                 raise ValueError("Invalid datetime string: " + attr)
 
             check_decimal = attr.split(".")
             if len(check_decimal) > 1:
                 decimal_str = ""
@@ -1956,15 +1982,15 @@
         This is represented as seconds.
 
         :param int attr: Object to be serialized.
         :rtype: Datetime
         :raises: DeserializationError if format invalid
         """
         if isinstance(attr, ET.Element):
-            attr = int(attr.text)
+            attr = int(attr.text)  # type: ignore
         try:
             date_obj = datetime.datetime.fromtimestamp(attr, TZ_UTC)
         except ValueError as err:
             msg = "Cannot deserialize to unix datetime object."
             raise_with_traceback(DeserializationError, msg, err)
         else:
             return date_obj
```

## Comparing `azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/_vendor.py` & `azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/_vendor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
+from typing import List, cast
+
 from azure.core.pipeline.transport import HttpRequest
 
 
 def _convert_request(request, files=None):
     data = request.content if not files else None
     request = HttpRequest(method=request.method, url=request.url, headers=request.headers, data=data)
     if files:
@@ -18,10 +20,11 @@
 
 def _format_url_section(template, **kwargs):
     components = template.split("/")
     while components:
         try:
             return template.format(**kwargs)
         except KeyError as key:
-            formatted_components = template.split("/")
+            # Need the cast, as for some reasons "split" is typed as list[str | Any]
+            formatted_components = cast(List[str], template.split("/"))
             components = [c for c in formatted_components if "{}".format(key.args[0]) not in c]
             template = "/".join(components)
```

## Comparing `azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/_configuration.py` & `azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/_configuration.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,49 +15,46 @@
 from ._version import VERSION
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials import TokenCredential
 
 
-class ElasticSanManagementConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
-    """Configuration for ElasticSanManagement.
+class ElasticSanMgmtClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
+    """Configuration for ElasticSanMgmtClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2021-11-20-preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2022-12-01-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, credential: "TokenCredential", subscription_id: str, **kwargs: Any) -> None:
-        super(ElasticSanManagementConfiguration, self).__init__(**kwargs)
-        api_version = kwargs.pop("api_version", "2021-11-20-preview")  # type: str
+        super(ElasticSanMgmtClientConfiguration, self).__init__(**kwargs)
+        api_version: str = kwargs.pop("api_version", "2022-12-01-preview")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
         self.subscription_id = subscription_id
         self.api_version = api_version
         self.credential_scopes = kwargs.pop("credential_scopes", ["https://management.azure.com/.default"])
         kwargs.setdefault("sdk_moniker", "mgmt-elasticsan/{}".format(VERSION))
         self._configure(**kwargs)
 
-    def _configure(
-        self, **kwargs  # type: Any
-    ):
-        # type: (...) -> None
+    def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
         self.http_logging_policy = kwargs.get("http_logging_policy") or ARMHttpLoggingPolicy(**kwargs)
         self.retry_policy = kwargs.get("retry_policy") or policies.RetryPolicy(**kwargs)
         self.custom_hook_policy = kwargs.get("custom_hook_policy") or policies.CustomHookPolicy(**kwargs)
```

## Comparing `azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/__init__.py` & `azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/aio/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,23 +2,22 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-from ._elastic_san_management import ElasticSanManagement
-from ._version import VERSION
-
-__version__ = VERSION
+from ._elastic_san_mgmt_client import ElasticSanMgmtClient
 
 try:
     from ._patch import __all__ as _patch_all
-    from ._patch import *  # type: ignore # pylint: disable=unused-wildcard-import
+    from ._patch import *  # pylint: disable=unused-wildcard-import
 except ImportError:
     _patch_all = []
 from ._patch import patch_sdk as _patch_sdk
 
-__all__ = ["ElasticSanManagement"]
+__all__ = [
+    "ElasticSanMgmtClient",
+]
 __all__.extend([p for p in _patch_all if p not in __all__])
 
 _patch_sdk()
```

## Comparing `azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/aio/_elastic_san_management.py` & `azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/aio/_elastic_san_mgmt_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,71 +8,91 @@
 
 from copy import deepcopy
 from typing import Any, Awaitable, TYPE_CHECKING
 
 from azure.core.rest import AsyncHttpResponse, HttpRequest
 from azure.mgmt.core import AsyncARMPipelineClient
 
-from .. import models
+from .. import models as _models
 from .._serialization import Deserializer, Serializer
-from ._configuration import ElasticSanManagementConfiguration
-from .operations import ElasticSansOperations, Operations, SkusOperations, VolumeGroupsOperations, VolumesOperations
+from ._configuration import ElasticSanMgmtClientConfiguration
+from .operations import (
+    ElasticSansOperations,
+    Operations,
+    PrivateEndpointConnectionsOperations,
+    PrivateLinkResourcesOperations,
+    SkusOperations,
+    VolumeGroupsOperations,
+    VolumesOperations,
+)
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials_async import AsyncTokenCredential
 
 
-class ElasticSanManagement:  # pylint: disable=client-accepts-api-version-keyword
-    """ElasticSanManagement.
+class ElasticSanMgmtClient:  # pylint: disable=client-accepts-api-version-keyword,too-many-instance-attributes
+    """ElasticSanMgmtClient.
 
     :ivar operations: Operations operations
     :vartype operations: azure.mgmt.elasticsan.aio.operations.Operations
     :ivar skus: SkusOperations operations
     :vartype skus: azure.mgmt.elasticsan.aio.operations.SkusOperations
     :ivar elastic_sans: ElasticSansOperations operations
     :vartype elastic_sans: azure.mgmt.elasticsan.aio.operations.ElasticSansOperations
     :ivar volume_groups: VolumeGroupsOperations operations
     :vartype volume_groups: azure.mgmt.elasticsan.aio.operations.VolumeGroupsOperations
     :ivar volumes: VolumesOperations operations
     :vartype volumes: azure.mgmt.elasticsan.aio.operations.VolumesOperations
+    :ivar private_endpoint_connections: PrivateEndpointConnectionsOperations operations
+    :vartype private_endpoint_connections:
+     azure.mgmt.elasticsan.aio.operations.PrivateEndpointConnectionsOperations
+    :ivar private_link_resources: PrivateLinkResourcesOperations operations
+    :vartype private_link_resources:
+     azure.mgmt.elasticsan.aio.operations.PrivateLinkResourcesOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
-    :keyword api_version: Api Version. Default value is "2021-11-20-preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2022-12-01-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(
         self,
         credential: "AsyncTokenCredential",
         subscription_id: str,
         base_url: str = "https://management.azure.com",
         **kwargs: Any
     ) -> None:
-        self._config = ElasticSanManagementConfiguration(
+        self._config = ElasticSanMgmtClientConfiguration(
             credential=credential, subscription_id=subscription_id, **kwargs
         )
-        self._client = AsyncARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
+        self._client: AsyncARMPipelineClient = AsyncARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
 
-        client_models = {k: v for k, v in models.__dict__.items() if isinstance(v, type)}
+        client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
         self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
         self.skus = SkusOperations(self._client, self._config, self._serialize, self._deserialize)
         self.elastic_sans = ElasticSansOperations(self._client, self._config, self._serialize, self._deserialize)
         self.volume_groups = VolumeGroupsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.volumes = VolumesOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.private_endpoint_connections = PrivateEndpointConnectionsOperations(
+            self._client, self._config, self._serialize, self._deserialize
+        )
+        self.private_link_resources = PrivateLinkResourcesOperations(
+            self._client, self._config, self._serialize, self._deserialize
+        )
 
     def _send_request(self, request: HttpRequest, **kwargs: Any) -> Awaitable[AsyncHttpResponse]:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
         >>> request = HttpRequest("GET", "https://www.example.org/")
         <HttpRequest [GET], url: 'https://www.example.org/'>
@@ -91,13 +111,13 @@
         request_copy = deepcopy(request)
         request_copy.url = self._client.format_url(request_copy.url)
         return self._client.send_request(request_copy, **kwargs)
 
     async def close(self) -> None:
         await self._client.close()
 
-    async def __aenter__(self) -> "ElasticSanManagement":
+    async def __aenter__(self) -> "ElasticSanMgmtClient":
         await self._client.__aenter__()
         return self
 
-    async def __aexit__(self, *exc_details) -> None:
+    async def __aexit__(self, *exc_details: Any) -> None:
         await self._client.__aexit__(*exc_details)
```

## Comparing `azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/aio/_patch.py` & `azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/aio/_configuration.py` & `azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/aio/_configuration.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,32 +15,32 @@
 from .._version import VERSION
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials_async import AsyncTokenCredential
 
 
-class ElasticSanManagementConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
-    """Configuration for ElasticSanManagement.
+class ElasticSanMgmtClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
+    """Configuration for ElasticSanMgmtClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2021-11-20-preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2022-12-01-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, credential: "AsyncTokenCredential", subscription_id: str, **kwargs: Any) -> None:
-        super(ElasticSanManagementConfiguration, self).__init__(**kwargs)
-        api_version = kwargs.pop("api_version", "2021-11-20-preview")  # type: str
+        super(ElasticSanMgmtClientConfiguration, self).__init__(**kwargs)
+        api_version: str = kwargs.pop("api_version", "2022-12-01-preview")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
```

## Comparing `azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/aio/__init__.py` & `azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,20 +2,25 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-from ._elastic_san_management import ElasticSanManagement
+from ._elastic_san_mgmt_client import ElasticSanMgmtClient
+from ._version import VERSION
+
+__version__ = VERSION
 
 try:
     from ._patch import __all__ as _patch_all
-    from ._patch import *  # type: ignore # pylint: disable=unused-wildcard-import
+    from ._patch import *  # pylint: disable=unused-wildcard-import
 except ImportError:
     _patch_all = []
 from ._patch import patch_sdk as _patch_sdk
 
-__all__ = ["ElasticSanManagement"]
+__all__ = [
+    "ElasticSanMgmtClient",
+]
 __all__.extend([p for p in _patch_all if p not in __all__])
 
 _patch_sdk()
```

## Comparing `azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/aio/operations/_elastic_sans_operations.py` & `azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/aio/operations/_elastic_sans_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
+from io import IOBase
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -45,15 +46,15 @@
 
 class ElasticSansOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.elasticsan.aio.ElasticSanManagement`'s
+        :class:`~azure.mgmt.elasticsan.aio.ElasticSanMgmtClient`'s
         :attr:`elastic_sans` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
@@ -70,16 +71,16 @@
         :return: An iterator like instance of either ElasticSan or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.elasticsan.models.ElasticSan]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ElasticSanList]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.ElasticSanList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -92,15 +93,15 @@
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
                     template_url=self.list_by_subscription.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
@@ -108,43 +109,46 @@
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
                 request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
                 request.method = "GET"
             return request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("ElasticSanList", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
-                list_of_elem = cls(list_of_elem)
+                list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-                request, stream=False, **kwargs
+            _stream = False
+            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
-                error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
+                error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list_by_subscription.metadata = {"url": "/subscriptions/{subscriptionId}/providers/Microsoft.ElasticSan/elasticSans"}  # type: ignore
+    list_by_subscription.metadata = {
+        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.ElasticSan/elasticSans"
+    }
 
     @distributed_trace
     def list_by_resource_group(self, resource_group_name: str, **kwargs: Any) -> AsyncIterable["_models.ElasticSan"]:
         """Gets a list of ElasticSan in a resource group.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
@@ -153,16 +157,16 @@
         :return: An iterator like instance of either ElasticSan or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.elasticsan.models.ElasticSan]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ElasticSanList]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.ElasticSanList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -176,15 +180,15 @@
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
                     template_url=self.list_by_resource_group.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
@@ -192,43 +196,46 @@
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
                 request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
                 request.method = "GET"
             return request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("ElasticSanList", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
-                list_of_elem = cls(list_of_elem)
+                list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-                request, stream=False, **kwargs
+            _stream = False
+            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
-                error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
+                error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list_by_resource_group.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans"}  # type: ignore
+    list_by_resource_group.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans"
+    }
 
     async def _create_initial(
         self, resource_group_name: str, elastic_san_name: str, parameters: Union[_models.ElasticSan, IO], **kwargs: Any
     ) -> _models.ElasticSan:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -236,22 +243,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ElasticSan]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.ElasticSan] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "ElasticSan")
 
         request = build_create_request(
             resource_group_name=resource_group_name,
             elastic_san_name=elastic_san_name,
@@ -261,39 +268,42 @@
             json=_json,
             content=_content,
             template_url=self._create_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [200, 202]:
+        if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if response.status_code == 200:
             deserialized = self._deserialize("ElasticSan", pipeline_response)
 
-        if response.status_code == 202:
+        if response.status_code == 201:
             deserialized = self._deserialize("ElasticSan", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
+        return deserialized  # type: ignore
 
-    _create_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}"}  # type: ignore
+    _create_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}"
+    }
 
     @overload
     async def begin_create(
         self,
         resource_group_name: str,
         elastic_san_name: str,
         parameters: _models.ElasticSan,
@@ -370,15 +380,15 @@
         """Create ElasticSan.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param elastic_san_name: The name of the ElasticSan. Required.
         :type elastic_san_name: str
-        :param parameters: Elastic San object. Is either a model type or a IO type. Required.
+        :param parameters: Elastic San object. Is either a ElasticSan type or a IO type. Required.
         :type parameters: ~azure.mgmt.elasticsan.models.ElasticSan or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -391,22 +401,22 @@
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.elasticsan.models.ElasticSan]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ElasticSan]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.ElasticSan] = kwargs.pop("cls", None)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = await self._create_initial(  # type: ignore
+            raw_result = await self._create_initial(
                 resource_group_name=resource_group_name,
                 elastic_san_name=elastic_san_name,
                 parameters=parameters,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
@@ -418,32 +428,33 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("ElasticSan", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
         if polling is True:
-            polling_method = cast(
-                AsyncPollingMethod,
-                AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
-            )  # type: AsyncPollingMethod
+            polling_method: AsyncPollingMethod = cast(
+                AsyncPollingMethod, AsyncARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            )
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    begin_create.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}"}  # type: ignore
+    begin_create.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}"
+    }
 
     async def _update_initial(
         self,
         resource_group_name: str,
         elastic_san_name: str,
         parameters: Union[_models.ElasticSanUpdate, IO],
         **kwargs: Any
@@ -455,22 +466,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[Optional[_models.ElasticSan]]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[Optional[_models.ElasticSan]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "ElasticSanUpdate")
 
         request = build_update_request(
             resource_group_name=resource_group_name,
             elastic_san_name=elastic_san_name,
@@ -480,37 +491,44 @@
             json=_json,
             content=_content,
             template_url=self._update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = None
+        response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("ElasticSan", pipeline_response)
 
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, response_headers)
 
         return deserialized
 
-    _update_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}"}  # type: ignore
+    _update_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}"
+    }
 
     @overload
     async def begin_update(
         self,
         resource_group_name: str,
         elastic_san_name: str,
         parameters: _models.ElasticSanUpdate,
@@ -591,15 +609,16 @@
         """Update a Elastic San.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param elastic_san_name: The name of the ElasticSan. Required.
         :type elastic_san_name: str
-        :param parameters: Elastic San object. Is either a model type or a IO type. Required.
+        :param parameters: Elastic San object. Is either a ElasticSanUpdate type or a IO type.
+         Required.
         :type parameters: ~azure.mgmt.elasticsan.models.ElasticSanUpdate or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -612,22 +631,22 @@
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.elasticsan.models.ElasticSan]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ElasticSan]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.ElasticSan] = kwargs.pop("cls", None)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = await self._update_initial(  # type: ignore
+            raw_result = await self._update_initial(
                 resource_group_name=resource_group_name,
                 elastic_san_name=elastic_san_name,
                 parameters=parameters,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
@@ -639,32 +658,33 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("ElasticSan", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
         if polling is True:
-            polling_method = cast(
-                AsyncPollingMethod,
-                AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
-            )  # type: AsyncPollingMethod
+            polling_method: AsyncPollingMethod = cast(
+                AsyncPollingMethod, AsyncARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            )
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    begin_update.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}"}  # type: ignore
+    begin_update.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}"
+    }
 
     async def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, elastic_san_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -672,44 +692,51 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             elastic_san_name=elastic_san_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
+        response_headers = {}
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, None, response_headers)
 
-    _delete_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}"}  # type: ignore
+    _delete_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}"
+    }
 
     @distributed_trace_async
     async def begin_delete(
         self, resource_group_name: str, elastic_san_name: str, **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Delete a Elastic San.
 
@@ -729,19 +756,19 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
                 elastic_san_name=elastic_san_name,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
                 headers=_headers,
@@ -751,32 +778,33 @@
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
                 return cls(pipeline_response, None, {})
 
         if polling is True:
-            polling_method = cast(
-                AsyncPollingMethod,
-                AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
-            )  # type: AsyncPollingMethod
+            polling_method: AsyncPollingMethod = cast(
+                AsyncPollingMethod, AsyncARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            )
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    begin_delete.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}"}  # type: ignore
+    begin_delete.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}"
+    }
 
     @distributed_trace_async
     async def get(self, resource_group_name: str, elastic_san_name: str, **kwargs: Any) -> _models.ElasticSan:
         """Get a ElasticSan.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
@@ -795,41 +823,44 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ElasticSan]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.ElasticSan] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             elastic_san_name=elastic_san_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("ElasticSan", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    get.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}"}  # type: ignore
+    get.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}"
+    }
```

## Comparing `azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/aio/operations/_operations.py` & `azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/aio/operations/_operations.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,43 +35,41 @@
 
 class Operations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.elasticsan.aio.ElasticSanManagement`'s
+        :class:`~azure.mgmt.elasticsan.aio.ElasticSanMgmtClient`'s
         :attr:`operations` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
-    def list(self, **kwargs: Any) -> AsyncIterable["_models.ElasticSanRPOperation"]:
+    def list(self, **kwargs: Any) -> AsyncIterable["_models.Operation"]:
         """Gets a list of ElasticSan operations.
 
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either ElasticSanRPOperation or the result of
-         cls(response)
-        :rtype:
-         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.elasticsan.models.ElasticSanRPOperation]
+        :return: An iterator like instance of either Operation or the result of cls(response)
+        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.elasticsan.models.Operation]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ElasticSanOperationListResult]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.OperationListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -83,15 +81,15 @@
                 request = build_list_request(
                     api_version=api_version,
                     template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
@@ -99,36 +97,37 @@
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
                 request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
                 request.method = "GET"
             return request
 
         async def extract_data(pipeline_response):
-            deserialized = self._deserialize("ElasticSanOperationListResult", pipeline_response)
+            deserialized = self._deserialize("OperationListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
-                list_of_elem = cls(list_of_elem)
+                list_of_elem = cls(list_of_elem)  # type: ignore
             return None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-                request, stream=False, **kwargs
+            _stream = False
+            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
-                error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
+                error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list.metadata = {"url": "/providers/Microsoft.ElasticSan/operations"}  # type: ignore
+    list.metadata = {"url": "/providers/Microsoft.ElasticSan/operations"}
```

## Comparing `azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/aio/operations/_volumes_operations.py` & `azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/aio/operations/_volumes_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
+from io import IOBase
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -44,15 +45,15 @@
 
 class VolumesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.elasticsan.aio.ElasticSanManagement`'s
+        :class:`~azure.mgmt.elasticsan.aio.ElasticSanMgmtClient`'s
         :attr:`volumes` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
@@ -77,22 +78,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.Volume]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.Volume] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "Volume")
 
         request = build_create_request(
             resource_group_name=resource_group_name,
             elastic_san_name=elastic_san_name,
@@ -104,39 +105,42 @@
             json=_json,
             content=_content,
             template_url=self._create_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [200, 202]:
+        if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if response.status_code == 200:
             deserialized = self._deserialize("Volume", pipeline_response)
 
-        if response.status_code == 202:
+        if response.status_code == 201:
             deserialized = self._deserialize("Volume", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
+        return deserialized  # type: ignore
 
-    _create_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}/volumes/{volumeName}"}  # type: ignore
+    _create_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}/volumes/{volumeName}"
+    }
 
     @overload
     async def begin_create(
         self,
         resource_group_name: str,
         elastic_san_name: str,
         volume_group_name: str,
@@ -235,15 +239,15 @@
         :type resource_group_name: str
         :param elastic_san_name: The name of the ElasticSan. Required.
         :type elastic_san_name: str
         :param volume_group_name: The name of the VolumeGroup. Required.
         :type volume_group_name: str
         :param volume_name: The name of the Volume. Required.
         :type volume_name: str
-        :param parameters: Volume object. Is either a model type or a IO type. Required.
+        :param parameters: Volume object. Is either a Volume type or a IO type. Required.
         :type parameters: ~azure.mgmt.elasticsan.models.Volume or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -256,22 +260,22 @@
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.elasticsan.models.Volume]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.Volume]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.Volume] = kwargs.pop("cls", None)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = await self._create_initial(  # type: ignore
+            raw_result = await self._create_initial(
                 resource_group_name=resource_group_name,
                 elastic_san_name=elastic_san_name,
                 volume_group_name=volume_group_name,
                 volume_name=volume_name,
                 parameters=parameters,
                 api_version=api_version,
                 content_type=content_type,
@@ -285,32 +289,33 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("Volume", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
         if polling is True:
-            polling_method = cast(
-                AsyncPollingMethod,
-                AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
-            )  # type: AsyncPollingMethod
+            polling_method: AsyncPollingMethod = cast(
+                AsyncPollingMethod, AsyncARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            )
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    begin_create.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}/volumes/{volumeName}"}  # type: ignore
+    begin_create.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}/volumes/{volumeName}"
+    }
 
     async def _update_initial(
         self,
         resource_group_name: str,
         elastic_san_name: str,
         volume_group_name: str,
         volume_name: str,
@@ -324,22 +329,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[Optional[_models.Volume]]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[Optional[_models.Volume]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "VolumeUpdate")
 
         request = build_update_request(
             resource_group_name=resource_group_name,
             elastic_san_name=elastic_san_name,
@@ -351,37 +356,44 @@
             json=_json,
             content=_content,
             template_url=self._update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = None
+        response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("Volume", pipeline_response)
 
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, response_headers)
 
         return deserialized
 
-    _update_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}/volumes/{volumeName}"}  # type: ignore
+    _update_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}/volumes/{volumeName}"
+    }
 
     @overload
     async def begin_update(
         self,
         resource_group_name: str,
         elastic_san_name: str,
         volume_group_name: str,
@@ -480,15 +492,15 @@
         :type resource_group_name: str
         :param elastic_san_name: The name of the ElasticSan. Required.
         :type elastic_san_name: str
         :param volume_group_name: The name of the VolumeGroup. Required.
         :type volume_group_name: str
         :param volume_name: The name of the Volume. Required.
         :type volume_name: str
-        :param parameters: Volume object. Is either a model type or a IO type. Required.
+        :param parameters: Volume object. Is either a VolumeUpdate type or a IO type. Required.
         :type parameters: ~azure.mgmt.elasticsan.models.VolumeUpdate or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -501,22 +513,22 @@
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.elasticsan.models.Volume]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.Volume]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.Volume] = kwargs.pop("cls", None)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = await self._update_initial(  # type: ignore
+            raw_result = await self._update_initial(
                 resource_group_name=resource_group_name,
                 elastic_san_name=elastic_san_name,
                 volume_group_name=volume_group_name,
                 volume_name=volume_name,
                 parameters=parameters,
                 api_version=api_version,
                 content_type=content_type,
@@ -530,32 +542,33 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("Volume", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
         if polling is True:
-            polling_method = cast(
-                AsyncPollingMethod,
-                AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
-            )  # type: AsyncPollingMethod
+            polling_method: AsyncPollingMethod = cast(
+                AsyncPollingMethod, AsyncARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            )
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    begin_update.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}/volumes/{volumeName}"}  # type: ignore
+    begin_update.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}/volumes/{volumeName}"
+    }
 
     async def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, elastic_san_name: str, volume_group_name: str, volume_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -563,46 +576,53 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             elastic_san_name=elastic_san_name,
             volume_group_name=volume_group_name,
             volume_name=volume_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
+        response_headers = {}
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, None, response_headers)
 
-    _delete_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}/volumes/{volumeName}"}  # type: ignore
+    _delete_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}/volumes/{volumeName}"
+    }
 
     @distributed_trace_async
     async def begin_delete(
         self, resource_group_name: str, elastic_san_name: str, volume_group_name: str, volume_name: str, **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Delete an Volume.
 
@@ -626,19 +646,19 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
                 elastic_san_name=elastic_san_name,
                 volume_group_name=volume_group_name,
                 volume_name=volume_name,
                 api_version=api_version,
@@ -650,32 +670,33 @@
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
                 return cls(pipeline_response, None, {})
 
         if polling is True:
-            polling_method = cast(
-                AsyncPollingMethod,
-                AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
-            )  # type: AsyncPollingMethod
+            polling_method: AsyncPollingMethod = cast(
+                AsyncPollingMethod, AsyncARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            )
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    begin_delete.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}/volumes/{volumeName}"}  # type: ignore
+    begin_delete.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}/volumes/{volumeName}"
+    }
 
     @distributed_trace_async
     async def get(
         self, resource_group_name: str, elastic_san_name: str, volume_group_name: str, volume_name: str, **kwargs: Any
     ) -> _models.Volume:
         """Get an Volume.
 
@@ -700,50 +721,53 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.Volume]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.Volume] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             elastic_san_name=elastic_san_name,
             volume_group_name=volume_group_name,
             volume_name=volume_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("Volume", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    get.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}/volumes/{volumeName}"}  # type: ignore
+    get.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}/volumes/{volumeName}"
+    }
 
     @distributed_trace
     def list_by_volume_group(
         self, resource_group_name: str, elastic_san_name: str, volume_group_name: str, **kwargs: Any
     ) -> AsyncIterable["_models.Volume"]:
         """List Volumes in a VolumeGroup.
 
@@ -758,16 +782,16 @@
         :return: An iterator like instance of either Volume or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.elasticsan.models.Volume]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.VolumeList]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.VolumeList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -783,15 +807,15 @@
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
                     template_url=self.list_by_volume_group.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
@@ -799,36 +823,39 @@
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
                 request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
                 request.method = "GET"
             return request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("VolumeList", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
-                list_of_elem = cls(list_of_elem)
+                list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-                request, stream=False, **kwargs
+            _stream = False
+            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
-                error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
+                error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list_by_volume_group.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}/volumes"}  # type: ignore
+    list_by_volume_group.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}/volumes"
+    }
```

## Comparing `azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/aio/operations/_patch.py` & `azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/aio/operations/_volume_groups_operations.py` & `azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/aio/operations/_volume_groups_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
+from io import IOBase
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -44,15 +45,15 @@
 
 class VolumeGroupsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.elasticsan.aio.ElasticSanManagement`'s
+        :class:`~azure.mgmt.elasticsan.aio.ElasticSanMgmtClient`'s
         :attr:`volume_groups` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
@@ -76,16 +77,16 @@
         :return: An iterator like instance of either VolumeGroup or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.elasticsan.models.VolumeGroup]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.VolumeGroupList]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.VolumeGroupList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -100,15 +101,15 @@
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
                     template_url=self.list_by_elastic_san.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
@@ -116,43 +117,46 @@
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
                 request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
                 request.method = "GET"
             return request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("VolumeGroupList", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
-                list_of_elem = cls(list_of_elem)
+                list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-                request, stream=False, **kwargs
+            _stream = False
+            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
-                error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
+                error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list_by_elastic_san.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumeGroups"}  # type: ignore
+    list_by_elastic_san.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumeGroups"
+    }
 
     async def _create_initial(
         self,
         resource_group_name: str,
         elastic_san_name: str,
         volume_group_name: str,
         parameters: Union[_models.VolumeGroup, IO],
@@ -165,22 +169,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.VolumeGroup]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.VolumeGroup] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "VolumeGroup")
 
         request = build_create_request(
             resource_group_name=resource_group_name,
             elastic_san_name=elastic_san_name,
@@ -191,39 +195,42 @@
             json=_json,
             content=_content,
             template_url=self._create_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [200, 202]:
+        if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if response.status_code == 200:
             deserialized = self._deserialize("VolumeGroup", pipeline_response)
 
-        if response.status_code == 202:
+        if response.status_code == 201:
             deserialized = self._deserialize("VolumeGroup", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
+        return deserialized  # type: ignore
 
-    _create_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}"}  # type: ignore
+    _create_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}"
+    }
 
     @overload
     async def begin_create(
         self,
         resource_group_name: str,
         elastic_san_name: str,
         volume_group_name: str,
@@ -313,15 +320,15 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param elastic_san_name: The name of the ElasticSan. Required.
         :type elastic_san_name: str
         :param volume_group_name: The name of the VolumeGroup. Required.
         :type volume_group_name: str
-        :param parameters: Volume Group object. Is either a model type or a IO type. Required.
+        :param parameters: Volume Group object. Is either a VolumeGroup type or a IO type. Required.
         :type parameters: ~azure.mgmt.elasticsan.models.VolumeGroup or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -334,22 +341,22 @@
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.elasticsan.models.VolumeGroup]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.VolumeGroup]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.VolumeGroup] = kwargs.pop("cls", None)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = await self._create_initial(  # type: ignore
+            raw_result = await self._create_initial(
                 resource_group_name=resource_group_name,
                 elastic_san_name=elastic_san_name,
                 volume_group_name=volume_group_name,
                 parameters=parameters,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
@@ -362,32 +369,33 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("VolumeGroup", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
         if polling is True:
-            polling_method = cast(
-                AsyncPollingMethod,
-                AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
-            )  # type: AsyncPollingMethod
+            polling_method: AsyncPollingMethod = cast(
+                AsyncPollingMethod, AsyncARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            )
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    begin_create.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}"}  # type: ignore
+    begin_create.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}"
+    }
 
     async def _update_initial(
         self,
         resource_group_name: str,
         elastic_san_name: str,
         volume_group_name: str,
         parameters: Union[_models.VolumeGroupUpdate, IO],
@@ -400,22 +408,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[Optional[_models.VolumeGroup]]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[Optional[_models.VolumeGroup]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "VolumeGroupUpdate")
 
         request = build_update_request(
             resource_group_name=resource_group_name,
             elastic_san_name=elastic_san_name,
@@ -426,37 +434,44 @@
             json=_json,
             content=_content,
             template_url=self._update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = None
+        response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("VolumeGroup", pipeline_response)
 
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, response_headers)
 
         return deserialized
 
-    _update_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}"}  # type: ignore
+    _update_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}"
+    }
 
     @overload
     async def begin_update(
         self,
         resource_group_name: str,
         elastic_san_name: str,
         volume_group_name: str,
@@ -546,15 +561,16 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param elastic_san_name: The name of the ElasticSan. Required.
         :type elastic_san_name: str
         :param volume_group_name: The name of the VolumeGroup. Required.
         :type volume_group_name: str
-        :param parameters: Volume Group object. Is either a model type or a IO type. Required.
+        :param parameters: Volume Group object. Is either a VolumeGroupUpdate type or a IO type.
+         Required.
         :type parameters: ~azure.mgmt.elasticsan.models.VolumeGroupUpdate or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -567,22 +583,22 @@
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.elasticsan.models.VolumeGroup]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.VolumeGroup]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.VolumeGroup] = kwargs.pop("cls", None)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = await self._update_initial(  # type: ignore
+            raw_result = await self._update_initial(
                 resource_group_name=resource_group_name,
                 elastic_san_name=elastic_san_name,
                 volume_group_name=volume_group_name,
                 parameters=parameters,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
@@ -595,32 +611,33 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("VolumeGroup", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
         if polling is True:
-            polling_method = cast(
-                AsyncPollingMethod,
-                AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
-            )  # type: AsyncPollingMethod
+            polling_method: AsyncPollingMethod = cast(
+                AsyncPollingMethod, AsyncARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            )
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    begin_update.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}"}  # type: ignore
+    begin_update.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}"
+    }
 
     async def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, elastic_san_name: str, volume_group_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -628,45 +645,52 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             elastic_san_name=elastic_san_name,
             volume_group_name=volume_group_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
+        response_headers = {}
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, None, response_headers)
 
-    _delete_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}"}  # type: ignore
+    _delete_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}"
+    }
 
     @distributed_trace_async
     async def begin_delete(
         self, resource_group_name: str, elastic_san_name: str, volume_group_name: str, **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Delete an VolumeGroup.
 
@@ -688,19 +712,19 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
                 elastic_san_name=elastic_san_name,
                 volume_group_name=volume_group_name,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
@@ -711,32 +735,33 @@
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
                 return cls(pipeline_response, None, {})
 
         if polling is True:
-            polling_method = cast(
-                AsyncPollingMethod,
-                AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
-            )  # type: AsyncPollingMethod
+            polling_method: AsyncPollingMethod = cast(
+                AsyncPollingMethod, AsyncARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            )
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    begin_delete.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}"}  # type: ignore
+    begin_delete.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}"
+    }
 
     @distributed_trace_async
     async def get(
         self, resource_group_name: str, elastic_san_name: str, volume_group_name: str, **kwargs: Any
     ) -> _models.VolumeGroup:
         """Get an VolumeGroups.
 
@@ -759,42 +784,45 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.VolumeGroup]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.VolumeGroup] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             elastic_san_name=elastic_san_name,
             volume_group_name=volume_group_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("VolumeGroup", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    get.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}"}  # type: ignore
+    get.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}"
+    }
```

## Comparing `azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/aio/operations/__init__.py` & `azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/aio/operations/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,21 +7,25 @@
 # --------------------------------------------------------------------------
 
 from ._operations import Operations
 from ._skus_operations import SkusOperations
 from ._elastic_sans_operations import ElasticSansOperations
 from ._volume_groups_operations import VolumeGroupsOperations
 from ._volumes_operations import VolumesOperations
+from ._private_endpoint_connections_operations import PrivateEndpointConnectionsOperations
+from ._private_link_resources_operations import PrivateLinkResourcesOperations
 
 from ._patch import __all__ as _patch_all
-from ._patch import *  # type: ignore # pylint: disable=unused-wildcard-import
+from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "Operations",
     "SkusOperations",
     "ElasticSansOperations",
     "VolumeGroupsOperations",
     "VolumesOperations",
+    "PrivateEndpointConnectionsOperations",
+    "PrivateLinkResourcesOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

## Comparing `azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/aio/operations/_skus_operations.py` & `azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/aio/operations/_skus_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 class SkusOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.elasticsan.aio.ElasticSanManagement`'s
+        :class:`~azure.mgmt.elasticsan.aio.ElasticSanMgmtClient`'s
         :attr:`skus` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
@@ -65,16 +65,16 @@
         :return: An iterator like instance of either SkuInformation or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.elasticsan.models.SkuInformation]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.SkuInformationList]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.SkuInformationList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -88,15 +88,15 @@
                     filter=filter,
                     api_version=api_version,
                     template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
@@ -104,36 +104,37 @@
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
                 request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
                 request.method = "GET"
             return request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("SkuInformationList", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
-                list_of_elem = cls(list_of_elem)
+                list_of_elem = cls(list_of_elem)  # type: ignore
             return None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-                request, stream=False, **kwargs
+            _stream = False
+            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
-                error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
+                error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/providers/Microsoft.ElasticSan/skus"}  # type: ignore
+    list.metadata = {"url": "/subscriptions/{subscriptionId}/providers/Microsoft.ElasticSan/skus"}
```

## Comparing `azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/operations/_elastic_sans_operations.py` & `azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/operations/_elastic_sans_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
+from io import IOBase
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -38,59 +39,54 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_by_subscription_request(subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop("api_version", _params.pop("api-version", "2021-11-20-preview"))  # type: str
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-12-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.ElasticSan/elasticSans")
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_list_by_resource_group_request(resource_group_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop("api_version", _params.pop("api-version", "2021-11-20-preview"))  # type: str
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-12-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name",
-            resource_group_name,
-            "str",
-            max_length=90,
-            min_length=1,
-            pattern=r"^[-\w\._]*[0-9A-Za-z]$",
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
@@ -99,44 +95,39 @@
 
 def build_create_request(
     resource_group_name: str, elastic_san_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop("api_version", _params.pop("api-version", "2021-11-20-preview"))  # type: str
-    content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-12-01-preview"))
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name",
-            resource_group_name,
-            "str",
-            max_length=90,
-            min_length=1,
-            pattern=r"^[-\w\._]*[0-9A-Za-z]$",
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "elasticSanName": _SERIALIZER.url(
             "elastic_san_name",
             elastic_san_name,
             "str",
             max_length=24,
             min_length=3,
             pattern=r"^[A-Za-z0-9]+((-|_)[a-z0-9A-Z]+)*$",
         ),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
@@ -147,44 +138,39 @@
 
 def build_update_request(
     resource_group_name: str, elastic_san_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop("api_version", _params.pop("api-version", "2021-11-20-preview"))  # type: str
-    content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-12-01-preview"))
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name",
-            resource_group_name,
-            "str",
-            max_length=90,
-            min_length=1,
-            pattern=r"^[-\w\._]*[0-9A-Za-z]$",
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "elasticSanName": _SERIALIZER.url(
             "elastic_san_name",
             elastic_san_name,
             "str",
             max_length=24,
             min_length=3,
             pattern=r"^[A-Za-z0-9]+((-|_)[a-z0-9A-Z]+)*$",
         ),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
@@ -195,43 +181,38 @@
 
 def build_delete_request(
     resource_group_name: str, elastic_san_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop("api_version", _params.pop("api-version", "2021-11-20-preview"))  # type: str
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-12-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name",
-            resource_group_name,
-            "str",
-            max_length=90,
-            min_length=1,
-            pattern=r"^[-\w\._]*[0-9A-Za-z]$",
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "elasticSanName": _SERIALIZER.url(
             "elastic_san_name",
             elastic_san_name,
             "str",
             max_length=24,
             min_length=3,
             pattern=r"^[A-Za-z0-9]+((-|_)[a-z0-9A-Z]+)*$",
         ),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
@@ -240,43 +221,38 @@
 
 def build_get_request(
     resource_group_name: str, elastic_san_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop("api_version", _params.pop("api-version", "2021-11-20-preview"))  # type: str
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-12-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name",
-            resource_group_name,
-            "str",
-            max_length=90,
-            min_length=1,
-            pattern=r"^[-\w\._]*[0-9A-Za-z]$",
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "elasticSanName": _SERIALIZER.url(
             "elastic_san_name",
             elastic_san_name,
             "str",
             max_length=24,
             min_length=3,
             pattern=r"^[A-Za-z0-9]+((-|_)[a-z0-9A-Z]+)*$",
         ),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
@@ -285,15 +261,15 @@
 
 class ElasticSansOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.elasticsan.ElasticSanManagement`'s
+        :class:`~azure.mgmt.elasticsan.ElasticSanMgmtClient`'s
         :attr:`elastic_sans` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
@@ -310,16 +286,16 @@
         :return: An iterator like instance of either ElasticSan or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.elasticsan.models.ElasticSan]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ElasticSanList]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.ElasticSanList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -332,15 +308,15 @@
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
                     template_url=self.list_by_subscription.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
@@ -348,43 +324,46 @@
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
                 request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
                 request.method = "GET"
             return request
 
         def extract_data(pipeline_response):
             deserialized = self._deserialize("ElasticSanList", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
-                list_of_elem = cls(list_of_elem)
+                list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-                request, stream=False, **kwargs
+            _stream = False
+            pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
-                error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
+                error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
-    list_by_subscription.metadata = {"url": "/subscriptions/{subscriptionId}/providers/Microsoft.ElasticSan/elasticSans"}  # type: ignore
+    list_by_subscription.metadata = {
+        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.ElasticSan/elasticSans"
+    }
 
     @distributed_trace
     def list_by_resource_group(self, resource_group_name: str, **kwargs: Any) -> Iterable["_models.ElasticSan"]:
         """Gets a list of ElasticSan in a resource group.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
@@ -393,16 +372,16 @@
         :return: An iterator like instance of either ElasticSan or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.elasticsan.models.ElasticSan]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ElasticSanList]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.ElasticSanList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -416,15 +395,15 @@
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
                     template_url=self.list_by_resource_group.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
@@ -432,43 +411,46 @@
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
                 request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
                 request.method = "GET"
             return request
 
         def extract_data(pipeline_response):
             deserialized = self._deserialize("ElasticSanList", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
-                list_of_elem = cls(list_of_elem)
+                list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-                request, stream=False, **kwargs
+            _stream = False
+            pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
-                error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
+                error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
-    list_by_resource_group.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans"}  # type: ignore
+    list_by_resource_group.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans"
+    }
 
     def _create_initial(
         self, resource_group_name: str, elastic_san_name: str, parameters: Union[_models.ElasticSan, IO], **kwargs: Any
     ) -> _models.ElasticSan:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -476,22 +458,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ElasticSan]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.ElasticSan] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "ElasticSan")
 
         request = build_create_request(
             resource_group_name=resource_group_name,
             elastic_san_name=elastic_san_name,
@@ -501,39 +483,42 @@
             json=_json,
             content=_content,
             template_url=self._create_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [200, 202]:
+        if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if response.status_code == 200:
             deserialized = self._deserialize("ElasticSan", pipeline_response)
 
-        if response.status_code == 202:
+        if response.status_code == 201:
             deserialized = self._deserialize("ElasticSan", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
+        return deserialized  # type: ignore
 
-    _create_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}"}  # type: ignore
+    _create_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}"
+    }
 
     @overload
     def begin_create(
         self,
         resource_group_name: str,
         elastic_san_name: str,
         parameters: _models.ElasticSan,
@@ -608,15 +593,15 @@
         """Create ElasticSan.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param elastic_san_name: The name of the ElasticSan. Required.
         :type elastic_san_name: str
-        :param parameters: Elastic San object. Is either a model type or a IO type. Required.
+        :param parameters: Elastic San object. Is either a ElasticSan type or a IO type. Required.
         :type parameters: ~azure.mgmt.elasticsan.models.ElasticSan or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -628,22 +613,22 @@
         :return: An instance of LROPoller that returns either ElasticSan or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.elasticsan.models.ElasticSan]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ElasticSan]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.ElasticSan] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = self._create_initial(  # type: ignore
+            raw_result = self._create_initial(
                 resource_group_name=resource_group_name,
                 elastic_san_name=elastic_san_name,
                 parameters=parameters,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
@@ -655,31 +640,33 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("ElasticSan", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
         if polling is True:
-            polling_method = cast(
-                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
-            )  # type: PollingMethod
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            )
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    begin_create.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}"}  # type: ignore
+    begin_create.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}"
+    }
 
     def _update_initial(
         self,
         resource_group_name: str,
         elastic_san_name: str,
         parameters: Union[_models.ElasticSanUpdate, IO],
         **kwargs: Any
@@ -691,22 +678,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[Optional[_models.ElasticSan]]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[Optional[_models.ElasticSan]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "ElasticSanUpdate")
 
         request = build_update_request(
             resource_group_name=resource_group_name,
             elastic_san_name=elastic_san_name,
@@ -716,37 +703,44 @@
             json=_json,
             content=_content,
             template_url=self._update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = None
+        response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("ElasticSan", pipeline_response)
 
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, response_headers)
 
         return deserialized
 
-    _update_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}"}  # type: ignore
+    _update_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}"
+    }
 
     @overload
     def begin_update(
         self,
         resource_group_name: str,
         elastic_san_name: str,
         parameters: _models.ElasticSanUpdate,
@@ -825,15 +819,16 @@
         """Update a Elastic San.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param elastic_san_name: The name of the ElasticSan. Required.
         :type elastic_san_name: str
-        :param parameters: Elastic San object. Is either a model type or a IO type. Required.
+        :param parameters: Elastic San object. Is either a ElasticSanUpdate type or a IO type.
+         Required.
         :type parameters: ~azure.mgmt.elasticsan.models.ElasticSanUpdate or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -845,22 +840,22 @@
         :return: An instance of LROPoller that returns either ElasticSan or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.elasticsan.models.ElasticSan]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ElasticSan]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.ElasticSan] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = self._update_initial(  # type: ignore
+            raw_result = self._update_initial(
                 resource_group_name=resource_group_name,
                 elastic_san_name=elastic_san_name,
                 parameters=parameters,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
@@ -872,31 +867,33 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("ElasticSan", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
         if polling is True:
-            polling_method = cast(
-                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
-            )  # type: PollingMethod
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            )
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    begin_update.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}"}  # type: ignore
+    begin_update.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}"
+    }
 
     def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, elastic_san_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -904,44 +901,51 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             elastic_san_name=elastic_san_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
+        response_headers = {}
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, None, response_headers)
 
-    _delete_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}"}  # type: ignore
+    _delete_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}"
+    }
 
     @distributed_trace
     def begin_delete(self, resource_group_name: str, elastic_san_name: str, **kwargs: Any) -> LROPoller[None]:
         """Delete a Elastic San.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
@@ -959,19 +963,19 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
                 elastic_san_name=elastic_san_name,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
                 headers=_headers,
@@ -981,31 +985,33 @@
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
                 return cls(pipeline_response, None, {})
 
         if polling is True:
-            polling_method = cast(
-                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
-            )  # type: PollingMethod
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            )
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    begin_delete.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}"}  # type: ignore
+    begin_delete.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}"
+    }
 
     @distributed_trace
     def get(self, resource_group_name: str, elastic_san_name: str, **kwargs: Any) -> _models.ElasticSan:
         """Get a ElasticSan.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
@@ -1024,41 +1030,44 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ElasticSan]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.ElasticSan] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             elastic_san_name=elastic_san_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("ElasticSan", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    get.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}"}  # type: ignore
+    get.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}"
+    }
```

## Comparing `azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/operations/_operations.py` & `azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/operations/_skus_operations.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,96 +23,109 @@
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
-from .._vendor import _convert_request
+from .._vendor import _convert_request, _format_url_section
 
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
-def build_list_request(**kwargs: Any) -> HttpRequest:
+def build_list_request(subscription_id: str, *, filter: Optional[str] = None, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop("api_version", _params.pop("api-version", "2021-11-20-preview"))  # type: str
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-12-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
-    _url = kwargs.pop("template_url", "/providers/Microsoft.ElasticSan/operations")
+    _url = kwargs.pop("template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.ElasticSan/skus")
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+    }
+
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+    if filter is not None:
+        _params["$filter"] = _SERIALIZER.query("filter", filter, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-class Operations:
+class SkusOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.elasticsan.ElasticSanManagement`'s
-        :attr:`operations` attribute.
+        :class:`~azure.mgmt.elasticsan.ElasticSanMgmtClient`'s
+        :attr:`skus` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
-    def list(self, **kwargs: Any) -> Iterable["_models.ElasticSanRPOperation"]:
-        """Gets a list of ElasticSan operations.
+    def list(self, filter: Optional[str] = None, **kwargs: Any) -> Iterable["_models.SkuInformation"]:
+        """List all the available Skus in the region and information related to them.
+
+        List all the available Skus in the region and information related to them.
 
+        :param filter: Specify $filter='location eq :code:`<location>`' to filter on location. Default
+         value is None.
+        :type filter: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either ElasticSanRPOperation or the result of
-         cls(response)
-        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.elasticsan.models.ElasticSanRPOperation]
+        :return: An iterator like instance of either SkuInformation or the result of cls(response)
+        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.elasticsan.models.SkuInformation]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ElasticSanOperationListResult]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.SkuInformationList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
                 request = build_list_request(
+                    subscription_id=self._config.subscription_id,
+                    filter=filter,
                     api_version=api_version,
                     template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
@@ -120,36 +133,37 @@
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
                 request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
                 request.method = "GET"
             return request
 
         def extract_data(pipeline_response):
-            deserialized = self._deserialize("ElasticSanOperationListResult", pipeline_response)
+            deserialized = self._deserialize("SkuInformationList", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
-                list_of_elem = cls(list_of_elem)
+                list_of_elem = cls(list_of_elem)  # type: ignore
             return None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-                request, stream=False, **kwargs
+            _stream = False
+            pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
-                error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
+                error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
-    list.metadata = {"url": "/providers/Microsoft.ElasticSan/operations"}  # type: ignore
+    list.metadata = {"url": "/subscriptions/{subscriptionId}/providers/Microsoft.ElasticSan/skus"}
```

## Comparing `azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/operations/_volumes_operations.py` & `azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/operations/_volumes_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
+from io import IOBase
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -45,32 +46,27 @@
     volume_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop("api_version", _params.pop("api-version", "2021-11-20-preview"))  # type: str
-    content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-12-01-preview"))
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}/volumes/{volumeName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name",
-            resource_group_name,
-            "str",
-            max_length=90,
-            min_length=1,
-            pattern=r"^[-\w\._]*[0-9A-Za-z]$",
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "elasticSanName": _SERIALIZER.url(
             "elastic_san_name",
             elastic_san_name,
             "str",
             max_length=24,
             min_length=3,
@@ -85,15 +81,15 @@
             pattern=r"^[A-Za-z0-9]+((-|_)[a-z0-9A-Z]+)*$",
         ),
         "volumeName": _SERIALIZER.url(
             "volume_name", volume_name, "str", max_length=63, min_length=3, pattern=r"^[a-z0-9]+(-[a-z0-9A-Z]+)*$"
         ),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
@@ -109,32 +105,27 @@
     volume_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop("api_version", _params.pop("api-version", "2021-11-20-preview"))  # type: str
-    content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-12-01-preview"))
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}/volumes/{volumeName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name",
-            resource_group_name,
-            "str",
-            max_length=90,
-            min_length=1,
-            pattern=r"^[-\w\._]*[0-9A-Za-z]$",
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "elasticSanName": _SERIALIZER.url(
             "elastic_san_name",
             elastic_san_name,
             "str",
             max_length=24,
             min_length=3,
@@ -149,15 +140,15 @@
             pattern=r"^[A-Za-z0-9]+((-|_)[a-z0-9A-Z]+)*$",
         ),
         "volumeName": _SERIALIZER.url(
             "volume_name", volume_name, "str", max_length=63, min_length=3, pattern=r"^[a-z0-9]+(-[a-z0-9A-Z]+)*$"
         ),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
@@ -173,31 +164,26 @@
     volume_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop("api_version", _params.pop("api-version", "2021-11-20-preview"))  # type: str
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-12-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}/volumes/{volumeName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name",
-            resource_group_name,
-            "str",
-            max_length=90,
-            min_length=1,
-            pattern=r"^[-\w\._]*[0-9A-Za-z]$",
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "elasticSanName": _SERIALIZER.url(
             "elastic_san_name",
             elastic_san_name,
             "str",
             max_length=24,
             min_length=3,
@@ -212,15 +198,15 @@
             pattern=r"^[A-Za-z0-9]+((-|_)[a-z0-9A-Z]+)*$",
         ),
         "volumeName": _SERIALIZER.url(
             "volume_name", volume_name, "str", max_length=63, min_length=3, pattern=r"^[a-z0-9]+(-[a-z0-9A-Z]+)*$"
         ),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
@@ -234,31 +220,26 @@
     volume_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop("api_version", _params.pop("api-version", "2021-11-20-preview"))  # type: str
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-12-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}/volumes/{volumeName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name",
-            resource_group_name,
-            "str",
-            max_length=90,
-            min_length=1,
-            pattern=r"^[-\w\._]*[0-9A-Za-z]$",
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "elasticSanName": _SERIALIZER.url(
             "elastic_san_name",
             elastic_san_name,
             "str",
             max_length=24,
             min_length=3,
@@ -273,15 +254,15 @@
             pattern=r"^[A-Za-z0-9]+((-|_)[a-z0-9A-Z]+)*$",
         ),
         "volumeName": _SERIALIZER.url(
             "volume_name", volume_name, "str", max_length=63, min_length=3, pattern=r"^[a-z0-9]+(-[a-z0-9A-Z]+)*$"
         ),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
@@ -290,31 +271,26 @@
 
 def build_list_by_volume_group_request(
     resource_group_name: str, elastic_san_name: str, volume_group_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop("api_version", _params.pop("api-version", "2021-11-20-preview"))  # type: str
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-12-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}/volumes",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name",
-            resource_group_name,
-            "str",
-            max_length=90,
-            min_length=1,
-            pattern=r"^[-\w\._]*[0-9A-Za-z]$",
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "elasticSanName": _SERIALIZER.url(
             "elastic_san_name",
             elastic_san_name,
             "str",
             max_length=24,
             min_length=3,
@@ -326,15 +302,15 @@
             "str",
             max_length=63,
             min_length=3,
             pattern=r"^[A-Za-z0-9]+((-|_)[a-z0-9A-Z]+)*$",
         ),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
@@ -343,15 +319,15 @@
 
 class VolumesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.elasticsan.ElasticSanManagement`'s
+        :class:`~azure.mgmt.elasticsan.ElasticSanMgmtClient`'s
         :attr:`volumes` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
@@ -376,22 +352,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.Volume]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.Volume] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "Volume")
 
         request = build_create_request(
             resource_group_name=resource_group_name,
             elastic_san_name=elastic_san_name,
@@ -403,39 +379,42 @@
             json=_json,
             content=_content,
             template_url=self._create_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [200, 202]:
+        if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if response.status_code == 200:
             deserialized = self._deserialize("Volume", pipeline_response)
 
-        if response.status_code == 202:
+        if response.status_code == 201:
             deserialized = self._deserialize("Volume", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
+        return deserialized  # type: ignore
 
-    _create_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}/volumes/{volumeName}"}  # type: ignore
+    _create_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}/volumes/{volumeName}"
+    }
 
     @overload
     def begin_create(
         self,
         resource_group_name: str,
         elastic_san_name: str,
         volume_group_name: str,
@@ -532,15 +511,15 @@
         :type resource_group_name: str
         :param elastic_san_name: The name of the ElasticSan. Required.
         :type elastic_san_name: str
         :param volume_group_name: The name of the VolumeGroup. Required.
         :type volume_group_name: str
         :param volume_name: The name of the Volume. Required.
         :type volume_name: str
-        :param parameters: Volume object. Is either a model type or a IO type. Required.
+        :param parameters: Volume object. Is either a Volume type or a IO type. Required.
         :type parameters: ~azure.mgmt.elasticsan.models.Volume or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -552,22 +531,22 @@
         :return: An instance of LROPoller that returns either Volume or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.elasticsan.models.Volume]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.Volume]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.Volume] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = self._create_initial(  # type: ignore
+            raw_result = self._create_initial(
                 resource_group_name=resource_group_name,
                 elastic_san_name=elastic_san_name,
                 volume_group_name=volume_group_name,
                 volume_name=volume_name,
                 parameters=parameters,
                 api_version=api_version,
                 content_type=content_type,
@@ -581,31 +560,33 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("Volume", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
         if polling is True:
-            polling_method = cast(
-                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
-            )  # type: PollingMethod
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            )
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    begin_create.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}/volumes/{volumeName}"}  # type: ignore
+    begin_create.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}/volumes/{volumeName}"
+    }
 
     def _update_initial(
         self,
         resource_group_name: str,
         elastic_san_name: str,
         volume_group_name: str,
         volume_name: str,
@@ -619,22 +600,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[Optional[_models.Volume]]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[Optional[_models.Volume]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "VolumeUpdate")
 
         request = build_update_request(
             resource_group_name=resource_group_name,
             elastic_san_name=elastic_san_name,
@@ -646,37 +627,44 @@
             json=_json,
             content=_content,
             template_url=self._update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = None
+        response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("Volume", pipeline_response)
 
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, response_headers)
 
         return deserialized
 
-    _update_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}/volumes/{volumeName}"}  # type: ignore
+    _update_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}/volumes/{volumeName}"
+    }
 
     @overload
     def begin_update(
         self,
         resource_group_name: str,
         elastic_san_name: str,
         volume_group_name: str,
@@ -773,15 +761,15 @@
         :type resource_group_name: str
         :param elastic_san_name: The name of the ElasticSan. Required.
         :type elastic_san_name: str
         :param volume_group_name: The name of the VolumeGroup. Required.
         :type volume_group_name: str
         :param volume_name: The name of the Volume. Required.
         :type volume_name: str
-        :param parameters: Volume object. Is either a model type or a IO type. Required.
+        :param parameters: Volume object. Is either a VolumeUpdate type or a IO type. Required.
         :type parameters: ~azure.mgmt.elasticsan.models.VolumeUpdate or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -793,22 +781,22 @@
         :return: An instance of LROPoller that returns either Volume or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.elasticsan.models.Volume]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.Volume]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.Volume] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = self._update_initial(  # type: ignore
+            raw_result = self._update_initial(
                 resource_group_name=resource_group_name,
                 elastic_san_name=elastic_san_name,
                 volume_group_name=volume_group_name,
                 volume_name=volume_name,
                 parameters=parameters,
                 api_version=api_version,
                 content_type=content_type,
@@ -822,31 +810,33 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("Volume", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
         if polling is True:
-            polling_method = cast(
-                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
-            )  # type: PollingMethod
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            )
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    begin_update.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}/volumes/{volumeName}"}  # type: ignore
+    begin_update.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}/volumes/{volumeName}"
+    }
 
     def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, elastic_san_name: str, volume_group_name: str, volume_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -854,46 +844,53 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             elastic_san_name=elastic_san_name,
             volume_group_name=volume_group_name,
             volume_name=volume_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
+        response_headers = {}
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, None, response_headers)
 
-    _delete_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}/volumes/{volumeName}"}  # type: ignore
+    _delete_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}/volumes/{volumeName}"
+    }
 
     @distributed_trace
     def begin_delete(
         self, resource_group_name: str, elastic_san_name: str, volume_group_name: str, volume_name: str, **kwargs: Any
     ) -> LROPoller[None]:
         """Delete an Volume.
 
@@ -917,19 +914,19 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
                 elastic_san_name=elastic_san_name,
                 volume_group_name=volume_group_name,
                 volume_name=volume_name,
                 api_version=api_version,
@@ -941,31 +938,33 @@
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
                 return cls(pipeline_response, None, {})
 
         if polling is True:
-            polling_method = cast(
-                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
-            )  # type: PollingMethod
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            )
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    begin_delete.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}/volumes/{volumeName}"}  # type: ignore
+    begin_delete.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}/volumes/{volumeName}"
+    }
 
     @distributed_trace
     def get(
         self, resource_group_name: str, elastic_san_name: str, volume_group_name: str, volume_name: str, **kwargs: Any
     ) -> _models.Volume:
         """Get an Volume.
 
@@ -990,50 +989,53 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.Volume]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.Volume] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             elastic_san_name=elastic_san_name,
             volume_group_name=volume_group_name,
             volume_name=volume_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("Volume", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    get.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}/volumes/{volumeName}"}  # type: ignore
+    get.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}/volumes/{volumeName}"
+    }
 
     @distributed_trace
     def list_by_volume_group(
         self, resource_group_name: str, elastic_san_name: str, volume_group_name: str, **kwargs: Any
     ) -> Iterable["_models.Volume"]:
         """List Volumes in a VolumeGroup.
 
@@ -1048,16 +1050,16 @@
         :return: An iterator like instance of either Volume or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.elasticsan.models.Volume]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.VolumeList]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.VolumeList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -1073,15 +1075,15 @@
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
                     template_url=self.list_by_volume_group.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
@@ -1089,36 +1091,39 @@
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
                 request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
                 request.method = "GET"
             return request
 
         def extract_data(pipeline_response):
             deserialized = self._deserialize("VolumeList", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
-                list_of_elem = cls(list_of_elem)
+                list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-                request, stream=False, **kwargs
+            _stream = False
+            pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
-                error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
+                error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
-    list_by_volume_group.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}/volumes"}  # type: ignore
+    list_by_volume_group.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}/volumes"
+    }
```

## Comparing `azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/operations/_patch.py` & `azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/operations/_volume_groups_operations.py` & `azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/operations/_volume_groups_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
+from io import IOBase
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -40,43 +41,38 @@
 
 def build_list_by_elastic_san_request(
     resource_group_name: str, elastic_san_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop("api_version", _params.pop("api-version", "2021-11-20-preview"))  # type: str
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-12-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumeGroups",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name",
-            resource_group_name,
-            "str",
-            max_length=90,
-            min_length=1,
-            pattern=r"^[-\w\._]*[0-9A-Za-z]$",
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "elasticSanName": _SERIALIZER.url(
             "elastic_san_name",
             elastic_san_name,
             "str",
             max_length=24,
             min_length=3,
             pattern=r"^[A-Za-z0-9]+((-|_)[a-z0-9A-Z]+)*$",
         ),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
@@ -85,32 +81,27 @@
 
 def build_create_request(
     resource_group_name: str, elastic_san_name: str, volume_group_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop("api_version", _params.pop("api-version", "2021-11-20-preview"))  # type: str
-    content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-12-01-preview"))
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name",
-            resource_group_name,
-            "str",
-            max_length=90,
-            min_length=1,
-            pattern=r"^[-\w\._]*[0-9A-Za-z]$",
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "elasticSanName": _SERIALIZER.url(
             "elastic_san_name",
             elastic_san_name,
             "str",
             max_length=24,
             min_length=3,
@@ -122,15 +113,15 @@
             "str",
             max_length=63,
             min_length=3,
             pattern=r"^[A-Za-z0-9]+((-|_)[a-z0-9A-Z]+)*$",
         ),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
@@ -141,32 +132,27 @@
 
 def build_update_request(
     resource_group_name: str, elastic_san_name: str, volume_group_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop("api_version", _params.pop("api-version", "2021-11-20-preview"))  # type: str
-    content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-12-01-preview"))
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name",
-            resource_group_name,
-            "str",
-            max_length=90,
-            min_length=1,
-            pattern=r"^[-\w\._]*[0-9A-Za-z]$",
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "elasticSanName": _SERIALIZER.url(
             "elastic_san_name",
             elastic_san_name,
             "str",
             max_length=24,
             min_length=3,
@@ -178,15 +164,15 @@
             "str",
             max_length=63,
             min_length=3,
             pattern=r"^[A-Za-z0-9]+((-|_)[a-z0-9A-Z]+)*$",
         ),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
@@ -197,31 +183,26 @@
 
 def build_delete_request(
     resource_group_name: str, elastic_san_name: str, volume_group_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop("api_version", _params.pop("api-version", "2021-11-20-preview"))  # type: str
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-12-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name",
-            resource_group_name,
-            "str",
-            max_length=90,
-            min_length=1,
-            pattern=r"^[-\w\._]*[0-9A-Za-z]$",
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "elasticSanName": _SERIALIZER.url(
             "elastic_san_name",
             elastic_san_name,
             "str",
             max_length=24,
             min_length=3,
@@ -233,15 +214,15 @@
             "str",
             max_length=63,
             min_length=3,
             pattern=r"^[A-Za-z0-9]+((-|_)[a-z0-9A-Z]+)*$",
         ),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
@@ -250,31 +231,26 @@
 
 def build_get_request(
     resource_group_name: str, elastic_san_name: str, volume_group_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop("api_version", _params.pop("api-version", "2021-11-20-preview"))  # type: str
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-12-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name",
-            resource_group_name,
-            "str",
-            max_length=90,
-            min_length=1,
-            pattern=r"^[-\w\._]*[0-9A-Za-z]$",
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "elasticSanName": _SERIALIZER.url(
             "elastic_san_name",
             elastic_san_name,
             "str",
             max_length=24,
             min_length=3,
@@ -286,15 +262,15 @@
             "str",
             max_length=63,
             min_length=3,
             pattern=r"^[A-Za-z0-9]+((-|_)[a-z0-9A-Z]+)*$",
         ),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
@@ -303,15 +279,15 @@
 
 class VolumeGroupsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.elasticsan.ElasticSanManagement`'s
+        :class:`~azure.mgmt.elasticsan.ElasticSanMgmtClient`'s
         :attr:`volume_groups` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
@@ -335,16 +311,16 @@
         :return: An iterator like instance of either VolumeGroup or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.elasticsan.models.VolumeGroup]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.VolumeGroupList]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.VolumeGroupList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -359,15 +335,15 @@
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
                     template_url=self.list_by_elastic_san.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
@@ -375,43 +351,46 @@
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
                 request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
+                request.url = self._client.format_url(request.url)
                 request.method = "GET"
             return request
 
         def extract_data(pipeline_response):
             deserialized = self._deserialize("VolumeGroupList", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
-                list_of_elem = cls(list_of_elem)
+                list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-                request, stream=False, **kwargs
+            _stream = False
+            pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
-                error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
+                error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
-    list_by_elastic_san.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumeGroups"}  # type: ignore
+    list_by_elastic_san.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumeGroups"
+    }
 
     def _create_initial(
         self,
         resource_group_name: str,
         elastic_san_name: str,
         volume_group_name: str,
         parameters: Union[_models.VolumeGroup, IO],
@@ -424,22 +403,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.VolumeGroup]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.VolumeGroup] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "VolumeGroup")
 
         request = build_create_request(
             resource_group_name=resource_group_name,
             elastic_san_name=elastic_san_name,
@@ -450,39 +429,42 @@
             json=_json,
             content=_content,
             template_url=self._create_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [200, 202]:
+        if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if response.status_code == 200:
             deserialized = self._deserialize("VolumeGroup", pipeline_response)
 
-        if response.status_code == 202:
+        if response.status_code == 201:
             deserialized = self._deserialize("VolumeGroup", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
+        return deserialized  # type: ignore
 
-    _create_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}"}  # type: ignore
+    _create_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}"
+    }
 
     @overload
     def begin_create(
         self,
         resource_group_name: str,
         elastic_san_name: str,
         volume_group_name: str,
@@ -572,15 +554,15 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param elastic_san_name: The name of the ElasticSan. Required.
         :type elastic_san_name: str
         :param volume_group_name: The name of the VolumeGroup. Required.
         :type volume_group_name: str
-        :param parameters: Volume Group object. Is either a model type or a IO type. Required.
+        :param parameters: Volume Group object. Is either a VolumeGroup type or a IO type. Required.
         :type parameters: ~azure.mgmt.elasticsan.models.VolumeGroup or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -593,22 +575,22 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.elasticsan.models.VolumeGroup]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.VolumeGroup]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.VolumeGroup] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = self._create_initial(  # type: ignore
+            raw_result = self._create_initial(
                 resource_group_name=resource_group_name,
                 elastic_san_name=elastic_san_name,
                 volume_group_name=volume_group_name,
                 parameters=parameters,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
@@ -621,31 +603,33 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("VolumeGroup", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
         if polling is True:
-            polling_method = cast(
-                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
-            )  # type: PollingMethod
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            )
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    begin_create.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}"}  # type: ignore
+    begin_create.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}"
+    }
 
     def _update_initial(
         self,
         resource_group_name: str,
         elastic_san_name: str,
         volume_group_name: str,
         parameters: Union[_models.VolumeGroupUpdate, IO],
@@ -658,22 +642,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[Optional[_models.VolumeGroup]]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[Optional[_models.VolumeGroup]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "VolumeGroupUpdate")
 
         request = build_update_request(
             resource_group_name=resource_group_name,
             elastic_san_name=elastic_san_name,
@@ -684,37 +668,44 @@
             json=_json,
             content=_content,
             template_url=self._update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = None
+        response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("VolumeGroup", pipeline_response)
 
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, response_headers)
 
         return deserialized
 
-    _update_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}"}  # type: ignore
+    _update_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}"
+    }
 
     @overload
     def begin_update(
         self,
         resource_group_name: str,
         elastic_san_name: str,
         volume_group_name: str,
@@ -804,15 +795,16 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param elastic_san_name: The name of the ElasticSan. Required.
         :type elastic_san_name: str
         :param volume_group_name: The name of the VolumeGroup. Required.
         :type volume_group_name: str
-        :param parameters: Volume Group object. Is either a model type or a IO type. Required.
+        :param parameters: Volume Group object. Is either a VolumeGroupUpdate type or a IO type.
+         Required.
         :type parameters: ~azure.mgmt.elasticsan.models.VolumeGroupUpdate or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -825,22 +817,22 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.elasticsan.models.VolumeGroup]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.VolumeGroup]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.VolumeGroup] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = self._update_initial(  # type: ignore
+            raw_result = self._update_initial(
                 resource_group_name=resource_group_name,
                 elastic_san_name=elastic_san_name,
                 volume_group_name=volume_group_name,
                 parameters=parameters,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
@@ -853,31 +845,33 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("VolumeGroup", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
         if polling is True:
-            polling_method = cast(
-                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
-            )  # type: PollingMethod
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            )
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    begin_update.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}"}  # type: ignore
+    begin_update.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}"
+    }
 
     def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, elastic_san_name: str, volume_group_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -885,45 +879,52 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             elastic_san_name=elastic_san_name,
             volume_group_name=volume_group_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
+        response_headers = {}
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, None, response_headers)
 
-    _delete_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}"}  # type: ignore
+    _delete_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}"
+    }
 
     @distributed_trace
     def begin_delete(
         self, resource_group_name: str, elastic_san_name: str, volume_group_name: str, **kwargs: Any
     ) -> LROPoller[None]:
         """Delete an VolumeGroup.
 
@@ -945,19 +946,19 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
                 elastic_san_name=elastic_san_name,
                 volume_group_name=volume_group_name,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
@@ -968,31 +969,33 @@
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
                 return cls(pipeline_response, None, {})
 
         if polling is True:
-            polling_method = cast(
-                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
-            )  # type: PollingMethod
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            )
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    begin_delete.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}"}  # type: ignore
+    begin_delete.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}"
+    }
 
     @distributed_trace
     def get(
         self, resource_group_name: str, elastic_san_name: str, volume_group_name: str, **kwargs: Any
     ) -> _models.VolumeGroup:
         """Get an VolumeGroups.
 
@@ -1015,42 +1018,45 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.VolumeGroup]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.VolumeGroup] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             elastic_san_name=elastic_san_name,
             volume_group_name=volume_group_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)  # type: ignore
+        request.url = self._client.format_url(request.url)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("VolumeGroup", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    get.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}"}  # type: ignore
+    get.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/volumegroups/{volumeGroupName}"
+    }
```

## Comparing `azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/operations/__init__.py` & `azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/operations/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,21 +7,25 @@
 # --------------------------------------------------------------------------
 
 from ._operations import Operations
 from ._skus_operations import SkusOperations
 from ._elastic_sans_operations import ElasticSansOperations
 from ._volume_groups_operations import VolumeGroupsOperations
 from ._volumes_operations import VolumesOperations
+from ._private_endpoint_connections_operations import PrivateEndpointConnectionsOperations
+from ._private_link_resources_operations import PrivateLinkResourcesOperations
 
 from ._patch import __all__ as _patch_all
-from ._patch import *  # type: ignore # pylint: disable=unused-wildcard-import
+from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "Operations",
     "SkusOperations",
     "ElasticSansOperations",
     "VolumeGroupsOperations",
     "VolumesOperations",
+    "PrivateEndpointConnectionsOperations",
+    "PrivateLinkResourcesOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

## Comparing `azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/operations/_skus_operations.py` & `azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/operations/_private_link_resources_operations.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,26 +2,24 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from typing import Any, Callable, Dict, Iterable, Optional, TypeVar
-import urllib.parse
+from typing import Any, Callable, Dict, Optional, TypeVar
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
     map_error,
 )
-from azure.core.paging import ItemPaged
 from azure.core.pipeline import PipelineResponse
 from azure.core.pipeline.transport import HttpResponse
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
@@ -32,137 +30,130 @@
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
-def build_list_request(subscription_id: str, *, filter: Optional[str] = None, **kwargs: Any) -> HttpRequest:
+def build_list_by_elastic_san_request(
+    resource_group_name: str, elastic_san_name: str, subscription_id: str, **kwargs: Any
+) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop("api_version", _params.pop("api-version", "2021-11-20-preview"))  # type: str
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2022-12-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
-    _url = kwargs.pop("template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.ElasticSan/skus")
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/privateLinkResources",
+    )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "elasticSanName": _SERIALIZER.url(
+            "elastic_san_name",
+            elastic_san_name,
+            "str",
+            max_length=24,
+            min_length=3,
+            pattern=r"^[A-Za-z0-9]+((-|_)[a-z0-9A-Z]+)*$",
+        ),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
-    if filter is not None:
-        _params["$filter"] = _SERIALIZER.query("filter", filter, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-class SkusOperations:
+class PrivateLinkResourcesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.elasticsan.ElasticSanManagement`'s
-        :attr:`skus` attribute.
+        :class:`~azure.mgmt.elasticsan.ElasticSanMgmtClient`'s
+        :attr:`private_link_resources` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
-    def list(self, filter: Optional[str] = None, **kwargs: Any) -> Iterable["_models.SkuInformation"]:
-        """List all the available Skus in the region and information related to them.
-
-        List all the available Skus in the region and information related to them.
-
-        :param filter: Specify $filter='location eq :code:`<location>`' to filter on location. Default
-         value is None.
-        :type filter: str
+    def list_by_elastic_san(
+        self, resource_group_name: str, elastic_san_name: str, **kwargs: Any
+    ) -> _models.PrivateLinkResourceListResult:
+        """Gets the private link resources that need to be created for a elastic San.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param elastic_san_name: The name of the ElasticSan. Required.
+        :type elastic_san_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either SkuInformation or the result of cls(response)
-        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.elasticsan.models.SkuInformation]
+        :return: PrivateLinkResourceListResult or the result of cls(response)
+        :rtype: ~azure.mgmt.elasticsan.models.PrivateLinkResourceListResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        _headers = kwargs.pop("headers", {}) or {}
-        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-        api_version = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))  # type: str
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.SkuInformationList]
-
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
-        def prepare_request(next_link=None):
-            if not next_link:
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-                request = build_list_request(
-                    subscription_id=self._config.subscription_id,
-                    filter=filter,
-                    api_version=api_version,
-                    template_url=self.list.metadata["url"],
-                    headers=_headers,
-                    params=_params,
-                )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
-
-            else:
-                # make call to next link with the client's api-version
-                _parsed_next_link = urllib.parse.urlparse(next_link)
-                _next_request_params = case_insensitive_dict(
-                    {
-                        key: [urllib.parse.quote(v) for v in value]
-                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
-                    }
-                )
-                _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
-                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
-                )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)  # type: ignore
-                request.method = "GET"
-            return request
-
-        def extract_data(pipeline_response):
-            deserialized = self._deserialize("SkuInformationList", pipeline_response)
-            list_of_elem = deserialized.value
-            if cls:
-                list_of_elem = cls(list_of_elem)
-            return None, iter(list_of_elem)
-
-        def get_next(next_link=None):
-            request = prepare_request(next_link)
-
-            pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-                request, stream=False, **kwargs
-            )
-            response = pipeline_response.http_response
-
-            if response.status_code not in [200]:
-                map_error(status_code=response.status_code, response=response, error_map=error_map)
-                error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
-                raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.PrivateLinkResourceListResult] = kwargs.pop("cls", None)
 
-            return pipeline_response
+        request = build_list_by_elastic_san_request(
+            resource_group_name=resource_group_name,
+            elastic_san_name=elastic_san_name,
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            template_url=self.list_by_elastic_san.metadata["url"],
+            headers=_headers,
+            params=_params,
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+        deserialized = self._deserialize("PrivateLinkResourceListResult", pipeline_response)
 
-        return ItemPaged(get_next, extract_data)
+        if cls:
+            return cls(pipeline_response, deserialized, {})
 
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/providers/Microsoft.ElasticSan/skus"}  # type: ignore
+        return deserialized
+
+    list_by_elastic_san.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ElasticSan/elasticSans/{elasticSanName}/privateLinkResources"
+    }
```

## Comparing `azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/models/_patch.py` & `azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/models/_elastic_san_management_enums.py` & `azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/models/_elastic_san_mgmt_client_enums.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,28 +6,34 @@
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from enum import Enum
 from azure.core import CaseInsensitiveEnumMeta
 
 
+class ActionType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """Enum. Indicates the action type. "Internal" refers to actions that are for internal only APIs."""
+
+    INTERNAL = "Internal"
+
+
 class CreatedByType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The type of identity that created the resource."""
 
     USER = "User"
     APPLICATION = "Application"
     MANAGED_IDENTITY = "ManagedIdentity"
     KEY = "Key"
 
 
 class EncryptionType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The type of key used to encrypt the data of the disk."""
 
-    #: Volume is encrypted at rest with Platform managed key. It is the default encryption type.
     ENCRYPTION_AT_REST_WITH_PLATFORM_KEY = "EncryptionAtRestWithPlatformKey"
+    """Volume is encrypted at rest with Platform managed key. It is the default encryption type."""
 
 
 class OperationalStatus(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Operational status of the resource."""
 
     INVALID = "Invalid"
     UNKNOWN = "Unknown"
@@ -35,14 +41,33 @@
     UNHEALTHY = "Unhealthy"
     UPDATING = "Updating"
     RUNNING = "Running"
     STOPPED = "Stopped"
     STOPPED_DEALLOCATED_ = "Stopped (deallocated)"
 
 
+class Origin(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """The intended executor of the operation; as in Resource Based Access Control (RBAC) and audit
+    logs UX. Default value is "user,system".
+    """
+
+    USER = "user"
+    SYSTEM = "system"
+    USER_SYSTEM = "user,system"
+
+
+class PrivateEndpointServiceConnectionStatus(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """The private endpoint connection status."""
+
+    PENDING = "Pending"
+    APPROVED = "Approved"
+    FAILED = "Failed"
+    REJECTED = "Rejected"
+
+
 class ProvisioningStates(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Provisioning state of the iSCSI Target."""
 
     INVALID = "Invalid"
     SUCCEEDED = "Succeeded"
     FAILED = "Failed"
     CANCELED = "Canceled"
@@ -51,25 +76,25 @@
     UPDATING = "Updating"
     DELETING = "Deleting"
 
 
 class SkuName(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The sku name."""
 
-    #: Premium locally redundant storage
     PREMIUM_LRS = "Premium_LRS"
-    #: Premium zone redundant storage
+    """Premium locally redundant storage"""
     PREMIUM_ZRS = "Premium_ZRS"
+    """Premium zone redundant storage"""
 
 
 class SkuTier(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The sku tier."""
 
-    #: Premium Tier
     PREMIUM = "Premium"
+    """Premium Tier"""
 
 
 class State(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Gets the state of virtual network rule."""
 
     PROVISIONING = "provisioning"
     DEPROVISIONING = "deprovisioning"
```

## Comparing `azure-mgmt-elasticsan-1.0.0b1/azure/mgmt/elasticsan/models/__init__.py` & `azure-mgmt-elasticsan-1.0.0b2/azure/mgmt/elasticsan/models/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,23 +4,30 @@
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._models_py3 import ElasticSan
 from ._models_py3 import ElasticSanList
-from ._models_py3 import ElasticSanOperationDisplay
-from ._models_py3 import ElasticSanOperationListResult
-from ._models_py3 import ElasticSanRPOperation
 from ._models_py3 import ElasticSanUpdate
-from ._models_py3 import Error
 from ._models_py3 import ErrorAdditionalInfo
+from ._models_py3 import ErrorDetail
 from ._models_py3 import ErrorResponse
 from ._models_py3 import IscsiTargetInfo
 from ._models_py3 import NetworkRuleSet
+from ._models_py3 import Operation
+from ._models_py3 import OperationDisplay
+from ._models_py3 import OperationListResult
+from ._models_py3 import PrivateEndpoint
+from ._models_py3 import PrivateEndpointConnection
+from ._models_py3 import PrivateEndpointConnectionListResult
+from ._models_py3 import PrivateLinkResource
+from ._models_py3 import PrivateLinkResourceListResult
+from ._models_py3 import PrivateLinkServiceConnectionState
+from ._models_py3 import ProxyResource
 from ._models_py3 import Resource
 from ._models_py3 import SKUCapability
 from ._models_py3 import Sku
 from ._models_py3 import SkuInformation
 from ._models_py3 import SkuInformationList
 from ._models_py3 import SkuLocationInfo
 from ._models_py3 import SourceCreationData
@@ -30,38 +37,48 @@
 from ._models_py3 import Volume
 from ._models_py3 import VolumeGroup
 from ._models_py3 import VolumeGroupList
 from ._models_py3 import VolumeGroupUpdate
 from ._models_py3 import VolumeList
 from ._models_py3 import VolumeUpdate
 
-from ._elastic_san_management_enums import CreatedByType
-from ._elastic_san_management_enums import EncryptionType
-from ._elastic_san_management_enums import OperationalStatus
-from ._elastic_san_management_enums import ProvisioningStates
-from ._elastic_san_management_enums import SkuName
-from ._elastic_san_management_enums import SkuTier
-from ._elastic_san_management_enums import State
-from ._elastic_san_management_enums import StorageTargetType
+from ._elastic_san_mgmt_client_enums import ActionType
+from ._elastic_san_mgmt_client_enums import CreatedByType
+from ._elastic_san_mgmt_client_enums import EncryptionType
+from ._elastic_san_mgmt_client_enums import OperationalStatus
+from ._elastic_san_mgmt_client_enums import Origin
+from ._elastic_san_mgmt_client_enums import PrivateEndpointServiceConnectionStatus
+from ._elastic_san_mgmt_client_enums import ProvisioningStates
+from ._elastic_san_mgmt_client_enums import SkuName
+from ._elastic_san_mgmt_client_enums import SkuTier
+from ._elastic_san_mgmt_client_enums import State
+from ._elastic_san_mgmt_client_enums import StorageTargetType
 from ._patch import __all__ as _patch_all
-from ._patch import *  # type: ignore # pylint: disable=unused-wildcard-import
+from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "ElasticSan",
     "ElasticSanList",
-    "ElasticSanOperationDisplay",
-    "ElasticSanOperationListResult",
-    "ElasticSanRPOperation",
     "ElasticSanUpdate",
-    "Error",
     "ErrorAdditionalInfo",
+    "ErrorDetail",
     "ErrorResponse",
     "IscsiTargetInfo",
     "NetworkRuleSet",
+    "Operation",
+    "OperationDisplay",
+    "OperationListResult",
+    "PrivateEndpoint",
+    "PrivateEndpointConnection",
+    "PrivateEndpointConnectionListResult",
+    "PrivateLinkResource",
+    "PrivateLinkResourceListResult",
+    "PrivateLinkServiceConnectionState",
+    "ProxyResource",
     "Resource",
     "SKUCapability",
     "Sku",
     "SkuInformation",
     "SkuInformationList",
     "SkuLocationInfo",
     "SourceCreationData",
@@ -70,17 +87,20 @@
     "VirtualNetworkRule",
     "Volume",
     "VolumeGroup",
     "VolumeGroupList",
     "VolumeGroupUpdate",
     "VolumeList",
     "VolumeUpdate",
+    "ActionType",
     "CreatedByType",
     "EncryptionType",
     "OperationalStatus",
+    "Origin",
+    "PrivateEndpointServiceConnectionStatus",
     "ProvisioningStates",
     "SkuName",
     "SkuTier",
     "State",
     "StorageTargetType",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
```

