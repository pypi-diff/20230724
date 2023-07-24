# Comparing `tmp/azure-mgmt-webpubsub-1.1.0b1.zip` & `tmp/azure-mgmt-webpubsub-2.0.0b1.zip`

## zipinfo {}

```diff
@@ -1,65 +1,67 @@
-Zip file size: 128348 bytes, number of entries: 63
-drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-02 05:36 azure-mgmt-webpubsub-1.1.0b1/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-02 05:36 azure-mgmt-webpubsub-1.1.0b1/azure_mgmt_webpubsub.egg-info/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-02 05:36 azure-mgmt-webpubsub-1.1.0b1/azure/
--rw-rw-r--  2.0 unx     1074 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/LICENSE
--rw-rw-r--  2.0 unx      626 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/_meta.json
--rw-rw-r--  2.0 unx     3206 b- defN 22-Nov-02 05:36 azure-mgmt-webpubsub-1.1.0b1/PKG-INFO
--rw-rw-r--  2.0 unx      215 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/MANIFEST.in
--rw-rw-r--  2.0 unx     1000 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/CHANGELOG.md
--rw-rw-r--  2.0 unx     1364 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/README.md
--rw-rw-r--  2.0 unx       38 b- defN 22-Nov-02 05:36 azure-mgmt-webpubsub-1.1.0b1/setup.cfg
--rw-rw-r--  2.0 unx     2774 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/setup.py
--rw-rw-r--  2.0 unx     2508 b- defN 22-Nov-02 05:36 azure-mgmt-webpubsub-1.1.0b1/azure_mgmt_webpubsub.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx     3206 b- defN 22-Nov-02 05:36 azure-mgmt-webpubsub-1.1.0b1/azure_mgmt_webpubsub.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx        1 b- defN 22-Nov-02 05:36 azure-mgmt-webpubsub-1.1.0b1/azure_mgmt_webpubsub.egg-info/not-zip-safe
--rw-rw-r--  2.0 unx        6 b- defN 22-Nov-02 05:36 azure-mgmt-webpubsub-1.1.0b1/azure_mgmt_webpubsub.egg-info/top_level.txt
--rw-rw-r--  2.0 unx      116 b- defN 22-Nov-02 05:36 azure-mgmt-webpubsub-1.1.0b1/azure_mgmt_webpubsub.egg-info/requires.txt
--rw-rw-r--  2.0 unx        1 b- defN 22-Nov-02 05:36 azure-mgmt-webpubsub-1.1.0b1/azure_mgmt_webpubsub.egg-info/dependency_links.txt
-drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-02 05:36 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/
--rw-rw-r--  2.0 unx       65 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-02 05:36 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/
--rw-rw-r--  2.0 unx       65 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-02 05:36 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-02 05:36 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/models/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-02 05:36 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/
--rw-rw-r--  2.0 unx      932 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/__init__.py
--rw-rw-r--  2.0 unx    77450 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/_serialization.py
--rw-rw-r--  2.0 unx     3937 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/_configuration.py
--rw-rw-r--  2.0 unx      674 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/_patch.py
--rw-rw-r--  2.0 unx      488 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/_version.py
--rw-rw-r--  2.0 unx       26 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/py.typed
--rw-rw-r--  2.0 unx     1169 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/_vendor.py
--rw-rw-r--  2.0 unx     7278 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/_web_pub_sub_management_client.py
--rw-rw-r--  2.0 unx     1773 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/operations/__init__.py
--rw-rw-r--  2.0 unx     8226 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_private_link_resources_operations.py
--rw-rw-r--  2.0 unx    32601 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_custom_domains_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/operations/_patch.py
--rw-rw-r--  2.0 unx    35148 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_shared_private_link_resources_operations.py
--rw-rw-r--  2.0 unx    30644 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_custom_certificates_operations.py
--rw-rw-r--  2.0 unx     7527 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/operations/_usages_operations.py
--rw-rw-r--  2.0 unx    32899 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_hubs_operations.py
--rw-rw-r--  2.0 unx     6861 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/operations/_operations.py
--rw-rw-r--  2.0 unx    30140 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_private_endpoint_connections_operations.py
--rw-rw-r--  2.0 unx    84427 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_operations.py
--rw-rw-r--  2.0 unx     6491 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/models/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/models/_patch.py
--rw-rw-r--  2.0 unx     3490 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/models/_web_pub_sub_management_client_enums.py
--rw-rw-r--  2.0 unx   110303 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/models/_models_py3.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-02 05:36 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/operations/
--rw-rw-r--  2.0 unx      879 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/__init__.py
--rw-rw-r--  2.0 unx     3941 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/_configuration.py
--rw-rw-r--  2.0 unx      674 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/_patch.py
--rw-rw-r--  2.0 unx     7383 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/_web_pub_sub_management_client.py
--rw-rw-r--  2.0 unx     1773 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/operations/__init__.py
--rw-rw-r--  2.0 unx     6894 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_private_link_resources_operations.py
--rw-rw-r--  2.0 unx    27120 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_custom_domains_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/operations/_patch.py
--rw-rw-r--  2.0 unx    29113 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_shared_private_link_resources_operations.py
--rw-rw-r--  2.0 unx    24869 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_custom_certificates_operations.py
--rw-rw-r--  2.0 unx     6377 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/operations/_usages_operations.py
--rw-rw-r--  2.0 unx    27390 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_hubs_operations.py
--rw-rw-r--  2.0 unx     6099 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/operations/_operations.py
--rw-rw-r--  2.0 unx    23959 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_private_endpoint_connections_operations.py
--rw-rw-r--  2.0 unx    70183 b- defN 22-Nov-02 05:35 azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_operations.py
-63 files, 737425 bytes uncompressed, 114558 bytes compressed:  84.5%
+Zip file size: 138951 bytes, number of entries: 65
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-24 07:44 azure-mgmt-webpubsub-2.0.0b1/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-24 07:44 azure-mgmt-webpubsub-2.0.0b1/azure_mgmt_webpubsub.egg-info/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-24 07:44 azure-mgmt-webpubsub-2.0.0b1/azure/
+-rw-rw-r--  2.0 unx      626 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/_meta.json
+-rw-rw-r--  2.0 unx       38 b- defN 23-Jul-24 07:44 azure-mgmt-webpubsub-2.0.0b1/setup.cfg
+-rw-rw-r--  2.0 unx     2844 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/setup.py
+-rw-rw-r--  2.0 unx     2158 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/README.md
+-rw-rw-r--  2.0 unx      215 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/MANIFEST.in
+-rw-rw-r--  2.0 unx     4878 b- defN 23-Jul-24 07:44 azure-mgmt-webpubsub-2.0.0b1/PKG-INFO
+-rw-rw-r--  2.0 unx     1074 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/LICENSE
+-rw-rw-r--  2.0 unx     1827 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/CHANGELOG.md
+-rw-rw-r--  2.0 unx        6 b- defN 23-Jul-24 07:44 azure-mgmt-webpubsub-2.0.0b1/azure_mgmt_webpubsub.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx      124 b- defN 23-Jul-24 07:44 azure-mgmt-webpubsub-2.0.0b1/azure_mgmt_webpubsub.egg-info/requires.txt
+-rw-rw-r--  2.0 unx     4878 b- defN 23-Jul-24 07:44 azure-mgmt-webpubsub-2.0.0b1/azure_mgmt_webpubsub.egg-info/PKG-INFO
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jul-24 07:44 azure-mgmt-webpubsub-2.0.0b1/azure_mgmt_webpubsub.egg-info/not-zip-safe
+-rw-rw-r--  2.0 unx     2648 b- defN 23-Jul-24 07:44 azure-mgmt-webpubsub-2.0.0b1/azure_mgmt_webpubsub.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jul-24 07:44 azure-mgmt-webpubsub-2.0.0b1/azure_mgmt_webpubsub.egg-info/dependency_links.txt
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-24 07:44 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/
+-rw-rw-r--  2.0 unx       65 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-24 07:44 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/
+-rw-rw-r--  2.0 unx       65 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-24 07:44 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-24 07:44 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-24 07:44 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/operations/
+-rw-rw-r--  2.0 unx     1302 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/_vendor.py
+-rw-rw-r--  2.0 unx       26 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/py.typed
+-rw-rw-r--  2.0 unx     7517 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/_web_pub_sub_management_client.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/_patch.py
+-rw-rw-r--  2.0 unx      488 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/_version.py
+-rw-rw-r--  2.0 unx     3540 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/_configuration.py
+-rw-rw-r--  2.0 unx      917 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/__init__.py
+-rw-rw-r--  2.0 unx    78836 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/_serialization.py
+-rw-rw-r--  2.0 unx     3650 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/models/_web_pub_sub_management_client_enums.py
+-rw-rw-r--  2.0 unx   118841 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/models/_models_py3.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/models/_patch.py
+-rw-rw-r--  2.0 unx     6661 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/models/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-24 07:44 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/operations/
+-rw-rw-r--  2.0 unx     7689 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/_web_pub_sub_management_client.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/_patch.py
+-rw-rw-r--  2.0 unx     3588 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/_configuration.py
+-rw-rw-r--  2.0 unx      864 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/__init__.py
+-rw-rw-r--  2.0 unx    28234 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_shared_private_link_resources_operations.py
+-rw-rw-r--  2.0 unx    26498 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_hubs_operations.py
+-rw-rw-r--  2.0 unx     6098 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/operations/_usages_operations.py
+-rw-rw-r--  2.0 unx    41010 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_replicas_operations.py
+-rw-rw-r--  2.0 unx     6541 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_private_link_resources_operations.py
+-rw-rw-r--  2.0 unx    71697 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_operations.py
+-rw-rw-r--  2.0 unx     5806 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/operations/_operations.py
+-rw-rw-r--  2.0 unx    26196 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_custom_domains_operations.py
+-rw-rw-r--  2.0 unx    24056 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_custom_certificates_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx     1867 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx    23261 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_private_endpoint_connections_operations.py
+-rw-rw-r--  2.0 unx    34996 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_shared_private_link_resources_operations.py
+-rw-rw-r--  2.0 unx    32734 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_hubs_operations.py
+-rw-rw-r--  2.0 unx     7221 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/operations/_usages_operations.py
+-rw-rw-r--  2.0 unx    51471 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_replicas_operations.py
+-rw-rw-r--  2.0 unx     8061 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_private_link_resources_operations.py
+-rw-rw-r--  2.0 unx    89209 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_operations.py
+-rw-rw-r--  2.0 unx     6520 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/operations/_operations.py
+-rw-rw-r--  2.0 unx    32404 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_custom_domains_operations.py
+-rw-rw-r--  2.0 unx    30558 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_custom_certificates_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/operations/_patch.py
+-rw-rw-r--  2.0 unx     1867 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/operations/__init__.py
+-rw-rw-r--  2.0 unx    30186 b- defN 23-Jul-24 07:43 azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_private_endpoint_connections_operations.py
+65 files, 845228 bytes uncompressed, 124617 bytes compressed:  85.3%
```

## zipnote {}

```diff
@@ -1,190 +1,196 @@
-Filename: azure-mgmt-webpubsub-1.1.0b1/
+Filename: azure-mgmt-webpubsub-2.0.0b1/
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure_mgmt_webpubsub.egg-info/
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure_mgmt_webpubsub.egg-info/
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/LICENSE
+Filename: azure-mgmt-webpubsub-2.0.0b1/_meta.json
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/_meta.json
+Filename: azure-mgmt-webpubsub-2.0.0b1/setup.cfg
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/PKG-INFO
+Filename: azure-mgmt-webpubsub-2.0.0b1/setup.py
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/MANIFEST.in
+Filename: azure-mgmt-webpubsub-2.0.0b1/README.md
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/CHANGELOG.md
+Filename: azure-mgmt-webpubsub-2.0.0b1/MANIFEST.in
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/README.md
+Filename: azure-mgmt-webpubsub-2.0.0b1/PKG-INFO
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/setup.cfg
+Filename: azure-mgmt-webpubsub-2.0.0b1/LICENSE
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/setup.py
+Filename: azure-mgmt-webpubsub-2.0.0b1/CHANGELOG.md
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure_mgmt_webpubsub.egg-info/SOURCES.txt
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure_mgmt_webpubsub.egg-info/top_level.txt
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure_mgmt_webpubsub.egg-info/PKG-INFO
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure_mgmt_webpubsub.egg-info/requires.txt
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure_mgmt_webpubsub.egg-info/not-zip-safe
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure_mgmt_webpubsub.egg-info/PKG-INFO
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure_mgmt_webpubsub.egg-info/top_level.txt
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure_mgmt_webpubsub.egg-info/not-zip-safe
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure_mgmt_webpubsub.egg-info/requires.txt
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure_mgmt_webpubsub.egg-info/SOURCES.txt
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure_mgmt_webpubsub.egg-info/dependency_links.txt
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure_mgmt_webpubsub.egg-info/dependency_links.txt
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/__init__.py
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/__init__.py
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/__init__.py
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/__init__.py
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/operations/
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/models/
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/models/
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/operations/
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/__init__.py
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/_vendor.py
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/_serialization.py
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/py.typed
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/_configuration.py
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/_web_pub_sub_management_client.py
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/_patch.py
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/_patch.py
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/_version.py
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/_version.py
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/py.typed
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/_vendor.py
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/__init__.py
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/_web_pub_sub_management_client.py
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/_serialization.py
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/operations/__init__.py
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/models/_web_pub_sub_management_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_private_link_resources_operations.py
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_custom_domains_operations.py
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/models/_patch.py
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/operations/_patch.py
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_shared_private_link_resources_operations.py
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/operations/
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_custom_certificates_operations.py
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/_web_pub_sub_management_client.py
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/operations/_usages_operations.py
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/_patch.py
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_hubs_operations.py
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/operations/_operations.py
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/__init__.py
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_private_endpoint_connections_operations.py
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_shared_private_link_resources_operations.py
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_operations.py
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_hubs_operations.py
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/models/__init__.py
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/operations/_usages_operations.py
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/models/_patch.py
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_replicas_operations.py
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/models/_web_pub_sub_management_client_enums.py
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_private_link_resources_operations.py
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/models/_models_py3.py
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_operations.py
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/operations/
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/__init__.py
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_custom_domains_operations.py
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/_configuration.py
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_custom_certificates_operations.py
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/_patch.py
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/_web_pub_sub_management_client.py
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/operations/__init__.py
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_private_endpoint_connections_operations.py
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_private_link_resources_operations.py
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_shared_private_link_resources_operations.py
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_custom_domains_operations.py
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_hubs_operations.py
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/operations/_patch.py
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/operations/_usages_operations.py
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_shared_private_link_resources_operations.py
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_replicas_operations.py
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_custom_certificates_operations.py
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_private_link_resources_operations.py
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/operations/_usages_operations.py
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_operations.py
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_hubs_operations.py
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/operations/_operations.py
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_custom_domains_operations.py
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_private_endpoint_connections_operations.py
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_custom_certificates_operations.py
 Comment: 
 
-Filename: azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_operations.py
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/operations/_patch.py
+Comment: 
+
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/operations/__init__.py
+Comment: 
+
+Filename: azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_private_endpoint_connections_operations.py
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-mgmt-webpubsub-1.1.0b1/LICENSE` & `azure-mgmt-webpubsub-2.0.0b1/LICENSE`

 * *Files identical despite different names*

## Comparing `azure-mgmt-webpubsub-1.1.0b1/PKG-INFO` & `azure-mgmt-webpubsub-2.0.0b1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-webpubsub
-Version: 1.1.0b1
+Version: 2.0.0b1
 Summary: Microsoft Azure WebPubSub Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Microsoft Azure SDK for Python
 
@@ -26,36 +27,97 @@
 This package has been tested with Python 3.7+.
 For a more complete view of Azure libraries, see the [azure sdk python release](https://aka.ms/azsdk/python/all).
 
 ## _Disclaimer_
 
 _Azure SDK Python packages support for Python 2.7 has ended 01 January 2022. For more information and questions, please refer to https://github.com/Azure/azure-sdk-for-python/issues/20691_
 
-# Usage
+## Getting started
 
+### Prerequisites
 
-To learn how to use this package, see the [quickstart guide](https://aka.ms/azsdk/python/mgmt)
- 
-For docs and references, see [Python SDK References](https://docs.microsoft.com/python/api/overview/azure/)
-Code samples for this package can be found at [WebPubSub Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com.
-Additional code samples for different Azure services are available at [Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
+- Python 3.7+ is required to use this package.
+- [Azure subscription](https://azure.microsoft.com/free/)
 
+### Install the package
 
-# Provide Feedback
+```bash
+pip install azure-mgmt-webpubsub
+pip install azure-identity
+```
+
+### Authentication
+
+By default, [Azure Active Directory](https://aka.ms/awps/aad) token authentication depends on correct configure of following environment variables.
+
+- `AZURE_CLIENT_ID` for Azure client ID.
+- `AZURE_TENANT_ID` for Azure tenant ID.
+- `AZURE_CLIENT_SECRET` for Azure client secret.
+
+In addition, Azure subscription ID can be configured via environment variable `AZURE_SUBSCRIPTION_ID`.
+
+With above configuration, client can be authenticated by following code:
+
+```python
+from azure.identity import DefaultAzureCredential
+from azure.mgmt.webpubsub import WebPubSubManagementClient
+import os
+
+sub_id = os.getenv("AZURE_SUBSCRIPTION_ID")
+client = WebPubSubManagementClient(credential=DefaultAzureCredential(), subscription_id=sub_id)
+```
+
+## Examples
+
+Code samples for this package can be found at:
+- [Search WebPubSub Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com
+- [Azure Python Mgmt SDK Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
+
+
+## Troubleshooting
+
+## Next steps
+
+## Provide Feedback
 
 If you encounter any bugs or have suggestions, please file an issue in the
 [Issues](https://github.com/Azure/azure-sdk-for-python/issues)
 section of the project. 
 
 
 ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-webpubsub%2FREADME.png)
 
 
 # Release History
 
+## 2.0.0b1 (2023-07-21)
+
+### Features Added
+
+  - Added operation WebPubSubOperations.list_replica_skus
+  - Added operation group WebPubSubReplicasOperations
+  - Model PrivateLinkResource has a new parameter system_data
+  - Model ProxyResource has a new parameter system_data
+  - Model Resource has a new parameter system_data
+  - Model TrackedResource has a new parameter system_data
+  - Model WebPubSubResource has a new parameter kind
+
+### Breaking Changes
+
+  - Parameter location of model TrackedResource is now required
+  - Parameter location of model WebPubSubResource is now required
+
+## 1.1.0 (2023-03-20)
+
+### Features Added
+
+  - Added operation group WebPubSubCustomCertificatesOperations
+  - Added operation group WebPubSubCustomDomainsOperations
+  - Model WebPubSubHubProperties has a new parameter event_listeners
+
 ## 1.1.0b1 (2022-11-02)
 
 ### Features Added
 
   - Added operation group WebPubSubCustomCertificatesOperations
   - Added operation group WebPubSubCustomDomainsOperations
   - Model WebPubSubHubProperties has a new parameter event_listeners
```

## Comparing `azure-mgmt-webpubsub-1.1.0b1/setup.py` & `azure-mgmt-webpubsub-2.0.0b1/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,78 +1,83 @@
 #!/usr/bin/env python
 
-#-------------------------------------------------------------------------
+# -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
-#--------------------------------------------------------------------------
+# --------------------------------------------------------------------------
 
 import re
 import os.path
 from io import open
 from setuptools import find_packages, setup
 
 # Change the PACKAGE_NAME only to change folder and different name
 PACKAGE_NAME = "azure-mgmt-webpubsub"
 PACKAGE_PPRINT_NAME = "WebPubSub Management"
 
 # a-b-c => a/b/c
-package_folder_path = PACKAGE_NAME.replace('-', '/')
+package_folder_path = PACKAGE_NAME.replace("-", "/")
 # a-b-c => a.b.c
-namespace_name = PACKAGE_NAME.replace('-', '.')
+namespace_name = PACKAGE_NAME.replace("-", ".")
 
 # Version extraction inspired from 'requests'
-with open(os.path.join(package_folder_path, 'version.py')
-          if os.path.exists(os.path.join(package_folder_path, 'version.py'))
-          else os.path.join(package_folder_path, '_version.py'), 'r') as fd:
-    version = re.search(r'^VERSION\s*=\s*[\'"]([^\'"]*)[\'"]',
-                        fd.read(), re.MULTILINE).group(1)
+with open(
+    os.path.join(package_folder_path, "version.py")
+    if os.path.exists(os.path.join(package_folder_path, "version.py"))
+    else os.path.join(package_folder_path, "_version.py"),
+    "r",
+) as fd:
+    version = re.search(r'^VERSION\s*=\s*[\'"]([^\'"]*)[\'"]', fd.read(), re.MULTILINE).group(1)
 
 if not version:
-    raise RuntimeError('Cannot find version information')
+    raise RuntimeError("Cannot find version information")
 
-with open('README.md', encoding='utf-8') as f:
+with open("README.md", encoding="utf-8") as f:
     readme = f.read()
-with open('CHANGELOG.md', encoding='utf-8') as f:
+with open("CHANGELOG.md", encoding="utf-8") as f:
     changelog = f.read()
 
 setup(
     name=PACKAGE_NAME,
     version=version,
-    description='Microsoft Azure {} Client Library for Python'.format(PACKAGE_PPRINT_NAME),
-    long_description=readme + '\n\n' + changelog,
-    long_description_content_type='text/markdown',
-    license='MIT License',
-    author='Microsoft Corporation',
-    author_email='azpysdkhelp@microsoft.com',
-    url='https://github.com/Azure/azure-sdk-for-python',
+    description="Microsoft Azure {} Client Library for Python".format(PACKAGE_PPRINT_NAME),
+    long_description=readme + "\n\n" + changelog,
+    long_description_content_type="text/markdown",
+    license="MIT License",
+    author="Microsoft Corporation",
+    author_email="azpysdkhelp@microsoft.com",
+    url="https://github.com/Azure/azure-sdk-for-python",
     keywords="azure, azure sdk",  # update with search keywords relevant to the azure service / product
     classifiers=[
-        'Development Status :: 4 - Beta',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'License :: OSI Approved :: MIT License',
+        "Development Status :: 4 - Beta",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "License :: OSI Approved :: MIT License",
     ],
     zip_safe=False,
-    packages=find_packages(exclude=[
-        'tests',
-        # Exclude packages that will be covered by PEP420 or nspkg
-        'azure',
-        'azure.mgmt',
-    ]),
+    packages=find_packages(
+        exclude=[
+            "tests",
+            # Exclude packages that will be covered by PEP420 or nspkg
+            "azure",
+            "azure.mgmt",
+        ]
+    ),
     include_package_data=True,
     package_data={
-        'pytyped': ['py.typed'],
+        "pytyped": ["py.typed"],
     },
     install_requires=[
-        "msrest>=0.7.1",
+        "isodate<1.0.0,>=0.6.1",
         "azure-common~=1.1",
         "azure-mgmt-core>=1.3.2,<2.0.0",
         "typing-extensions>=4.3.0; python_version<'3.8.0'",
     ],
-    python_requires=">=3.7"
+    python_requires=">=3.7",
 )
```

## Comparing `azure-mgmt-webpubsub-1.1.0b1/azure_mgmt_webpubsub.egg-info/SOURCES.txt` & `azure-mgmt-webpubsub-2.0.0b1/azure_mgmt_webpubsub.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 azure/mgmt/webpubsub/aio/operations/_usages_operations.py
 azure/mgmt/webpubsub/aio/operations/_web_pub_sub_custom_certificates_operations.py
 azure/mgmt/webpubsub/aio/operations/_web_pub_sub_custom_domains_operations.py
 azure/mgmt/webpubsub/aio/operations/_web_pub_sub_hubs_operations.py
 azure/mgmt/webpubsub/aio/operations/_web_pub_sub_operations.py
 azure/mgmt/webpubsub/aio/operations/_web_pub_sub_private_endpoint_connections_operations.py
 azure/mgmt/webpubsub/aio/operations/_web_pub_sub_private_link_resources_operations.py
+azure/mgmt/webpubsub/aio/operations/_web_pub_sub_replicas_operations.py
 azure/mgmt/webpubsub/aio/operations/_web_pub_sub_shared_private_link_resources_operations.py
 azure/mgmt/webpubsub/models/__init__.py
 azure/mgmt/webpubsub/models/_models_py3.py
 azure/mgmt/webpubsub/models/_patch.py
 azure/mgmt/webpubsub/models/_web_pub_sub_management_client_enums.py
 azure/mgmt/webpubsub/operations/__init__.py
 azure/mgmt/webpubsub/operations/_operations.py
@@ -39,14 +40,15 @@
 azure/mgmt/webpubsub/operations/_usages_operations.py
 azure/mgmt/webpubsub/operations/_web_pub_sub_custom_certificates_operations.py
 azure/mgmt/webpubsub/operations/_web_pub_sub_custom_domains_operations.py
 azure/mgmt/webpubsub/operations/_web_pub_sub_hubs_operations.py
 azure/mgmt/webpubsub/operations/_web_pub_sub_operations.py
 azure/mgmt/webpubsub/operations/_web_pub_sub_private_endpoint_connections_operations.py
 azure/mgmt/webpubsub/operations/_web_pub_sub_private_link_resources_operations.py
+azure/mgmt/webpubsub/operations/_web_pub_sub_replicas_operations.py
 azure/mgmt/webpubsub/operations/_web_pub_sub_shared_private_link_resources_operations.py
 azure_mgmt_webpubsub.egg-info/PKG-INFO
 azure_mgmt_webpubsub.egg-info/SOURCES.txt
 azure_mgmt_webpubsub.egg-info/dependency_links.txt
 azure_mgmt_webpubsub.egg-info/not-zip-safe
 azure_mgmt_webpubsub.egg-info/requires.txt
 azure_mgmt_webpubsub.egg-info/top_level.txt
```

## Comparing `azure-mgmt-webpubsub-1.1.0b1/azure_mgmt_webpubsub.egg-info/PKG-INFO` & `azure-mgmt-webpubsub-2.0.0b1/azure_mgmt_webpubsub.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-webpubsub
-Version: 1.1.0b1
+Version: 2.0.0b1
 Summary: Microsoft Azure WebPubSub Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Microsoft Azure SDK for Python
 
@@ -26,36 +27,97 @@
 This package has been tested with Python 3.7+.
 For a more complete view of Azure libraries, see the [azure sdk python release](https://aka.ms/azsdk/python/all).
 
 ## _Disclaimer_
 
 _Azure SDK Python packages support for Python 2.7 has ended 01 January 2022. For more information and questions, please refer to https://github.com/Azure/azure-sdk-for-python/issues/20691_
 
-# Usage
+## Getting started
 
+### Prerequisites
 
-To learn how to use this package, see the [quickstart guide](https://aka.ms/azsdk/python/mgmt)
- 
-For docs and references, see [Python SDK References](https://docs.microsoft.com/python/api/overview/azure/)
-Code samples for this package can be found at [WebPubSub Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com.
-Additional code samples for different Azure services are available at [Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
+- Python 3.7+ is required to use this package.
+- [Azure subscription](https://azure.microsoft.com/free/)
 
+### Install the package
 
-# Provide Feedback
+```bash
+pip install azure-mgmt-webpubsub
+pip install azure-identity
+```
+
+### Authentication
+
+By default, [Azure Active Directory](https://aka.ms/awps/aad) token authentication depends on correct configure of following environment variables.
+
+- `AZURE_CLIENT_ID` for Azure client ID.
+- `AZURE_TENANT_ID` for Azure tenant ID.
+- `AZURE_CLIENT_SECRET` for Azure client secret.
+
+In addition, Azure subscription ID can be configured via environment variable `AZURE_SUBSCRIPTION_ID`.
+
+With above configuration, client can be authenticated by following code:
+
+```python
+from azure.identity import DefaultAzureCredential
+from azure.mgmt.webpubsub import WebPubSubManagementClient
+import os
+
+sub_id = os.getenv("AZURE_SUBSCRIPTION_ID")
+client = WebPubSubManagementClient(credential=DefaultAzureCredential(), subscription_id=sub_id)
+```
+
+## Examples
+
+Code samples for this package can be found at:
+- [Search WebPubSub Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com
+- [Azure Python Mgmt SDK Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
+
+
+## Troubleshooting
+
+## Next steps
+
+## Provide Feedback
 
 If you encounter any bugs or have suggestions, please file an issue in the
 [Issues](https://github.com/Azure/azure-sdk-for-python/issues)
 section of the project. 
 
 
 ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-webpubsub%2FREADME.png)
 
 
 # Release History
 
+## 2.0.0b1 (2023-07-21)
+
+### Features Added
+
+  - Added operation WebPubSubOperations.list_replica_skus
+  - Added operation group WebPubSubReplicasOperations
+  - Model PrivateLinkResource has a new parameter system_data
+  - Model ProxyResource has a new parameter system_data
+  - Model Resource has a new parameter system_data
+  - Model TrackedResource has a new parameter system_data
+  - Model WebPubSubResource has a new parameter kind
+
+### Breaking Changes
+
+  - Parameter location of model TrackedResource is now required
+  - Parameter location of model WebPubSubResource is now required
+
+## 1.1.0 (2023-03-20)
+
+### Features Added
+
+  - Added operation group WebPubSubCustomCertificatesOperations
+  - Added operation group WebPubSubCustomDomainsOperations
+  - Model WebPubSubHubProperties has a new parameter event_listeners
+
 ## 1.1.0b1 (2022-11-02)
 
 ### Features Added
 
   - Added operation group WebPubSubCustomCertificatesOperations
   - Added operation group WebPubSubCustomDomainsOperations
   - Model WebPubSubHubProperties has a new parameter event_listeners
```

## Comparing `azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/__init__.py` & `azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,21 +3,18 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._web_pub_sub_management_client import WebPubSubManagementClient
-from ._version import VERSION
-
-__version__ = VERSION
 
 try:
     from ._patch import __all__ as _patch_all
-    from ._patch import *  # type: ignore # pylint: disable=unused-wildcard-import
+    from ._patch import *  # pylint: disable=unused-wildcard-import
 except ImportError:
     _patch_all = []
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "WebPubSubManagementClient",
 ]
```

## Comparing `azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/_serialization.py` & `azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/_serialization.py`

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

## Comparing `azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/_configuration.py` & `azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/_configuration.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,69 +2,59 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-import sys
 from typing import Any, TYPE_CHECKING
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
 from azure.mgmt.core.policies import ARMChallengeAuthenticationPolicy, ARMHttpLoggingPolicy
 
 from ._version import VERSION
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
-
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials import TokenCredential
 
 
 class WebPubSubManagementClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
     """Configuration for WebPubSubManagementClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
-    :param subscription_id: Gets subscription Id which uniquely identify the Microsoft Azure
-     subscription. The subscription ID forms part of the URI for every service call. Required.
+    :param subscription_id: The ID of the target subscription. The value must be an UUID. Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2022-08-01-preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2023-06-01-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, credential: "TokenCredential", subscription_id: str, **kwargs: Any) -> None:
         super(WebPubSubManagementClientConfiguration, self).__init__(**kwargs)
-        api_version = kwargs.pop("api_version", "2022-08-01-preview")  # type: Literal["2022-08-01-preview"]
+        api_version: str = kwargs.pop("api_version", "2023-06-01-preview")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
         self.subscription_id = subscription_id
         self.api_version = api_version
         self.credential_scopes = kwargs.pop("credential_scopes", ["https://management.azure.com/.default"])
         kwargs.setdefault("sdk_moniker", "mgmt-webpubsub/{}".format(VERSION))
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

## Comparing `azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/_patch.py` & `azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/_vendor.py` & `azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/_vendor.py`

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

## Comparing `azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/_web_pub_sub_management_client.py` & `azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/_web_pub_sub_management_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,26 +8,27 @@
 
 from copy import deepcopy
 from typing import Any, TYPE_CHECKING
 
 from azure.core.rest import HttpRequest, HttpResponse
 from azure.mgmt.core import ARMPipelineClient
 
-from . import models
+from . import models as _models
 from ._configuration import WebPubSubManagementClientConfiguration
 from ._serialization import Deserializer, Serializer
 from .operations import (
     Operations,
     UsagesOperations,
     WebPubSubCustomCertificatesOperations,
     WebPubSubCustomDomainsOperations,
     WebPubSubHubsOperations,
     WebPubSubOperations,
     WebPubSubPrivateEndpointConnectionsOperations,
     WebPubSubPrivateLinkResourcesOperations,
+    WebPubSubReplicasOperations,
     WebPubSubSharedPrivateLinkResourcesOperations,
 )
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials import TokenCredential
 
@@ -52,26 +53,27 @@
     :ivar web_pub_sub_private_endpoint_connections: WebPubSubPrivateEndpointConnectionsOperations
      operations
     :vartype web_pub_sub_private_endpoint_connections:
      azure.mgmt.webpubsub.operations.WebPubSubPrivateEndpointConnectionsOperations
     :ivar web_pub_sub_private_link_resources: WebPubSubPrivateLinkResourcesOperations operations
     :vartype web_pub_sub_private_link_resources:
      azure.mgmt.webpubsub.operations.WebPubSubPrivateLinkResourcesOperations
+    :ivar web_pub_sub_replicas: WebPubSubReplicasOperations operations
+    :vartype web_pub_sub_replicas: azure.mgmt.webpubsub.operations.WebPubSubReplicasOperations
     :ivar web_pub_sub_shared_private_link_resources: WebPubSubSharedPrivateLinkResourcesOperations
      operations
     :vartype web_pub_sub_shared_private_link_resources:
      azure.mgmt.webpubsub.operations.WebPubSubSharedPrivateLinkResourcesOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
-    :param subscription_id: Gets subscription Id which uniquely identify the Microsoft Azure
-     subscription. The subscription ID forms part of the URI for every service call. Required.
+    :param subscription_id: The ID of the target subscription. The value must be an UUID. Required.
     :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
-    :keyword api_version: Api Version. Default value is "2022-08-01-preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2023-06-01-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(
@@ -80,17 +82,17 @@
         subscription_id: str,
         base_url: str = "https://management.azure.com",
         **kwargs: Any
     ) -> None:
         self._config = WebPubSubManagementClientConfiguration(
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
         self.web_pub_sub = WebPubSubOperations(self._client, self._config, self._serialize, self._deserialize)
         self.usages = UsagesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.web_pub_sub_custom_certificates = WebPubSubCustomCertificatesOperations(
@@ -102,14 +104,17 @@
         self.web_pub_sub_hubs = WebPubSubHubsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.web_pub_sub_private_endpoint_connections = WebPubSubPrivateEndpointConnectionsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.web_pub_sub_private_link_resources = WebPubSubPrivateLinkResourcesOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
+        self.web_pub_sub_replicas = WebPubSubReplicasOperations(
+            self._client, self._config, self._serialize, self._deserialize
+        )
         self.web_pub_sub_shared_private_link_resources = WebPubSubSharedPrivateLinkResourcesOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
 
     def _send_request(self, request: HttpRequest, **kwargs: Any) -> HttpResponse:
         """Runs the network request through the client's chained policies.
 
@@ -128,19 +133,16 @@
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
-        # type: () -> WebPubSubManagementClient
+    def __enter__(self) -> "WebPubSubManagementClient":
         self._client.__enter__()
         return self
 
-    def __exit__(self, *exc_details):
-        # type: (Any) -> None
+    def __exit__(self, *exc_details: Any) -> None:
         self._client.__exit__(*exc_details)
```

## Comparing `azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/operations/__init__.py` & `azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/operations/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,26 +10,28 @@
 from ._web_pub_sub_operations import WebPubSubOperations
 from ._usages_operations import UsagesOperations
 from ._web_pub_sub_custom_certificates_operations import WebPubSubCustomCertificatesOperations
 from ._web_pub_sub_custom_domains_operations import WebPubSubCustomDomainsOperations
 from ._web_pub_sub_hubs_operations import WebPubSubHubsOperations
 from ._web_pub_sub_private_endpoint_connections_operations import WebPubSubPrivateEndpointConnectionsOperations
 from ._web_pub_sub_private_link_resources_operations import WebPubSubPrivateLinkResourcesOperations
+from ._web_pub_sub_replicas_operations import WebPubSubReplicasOperations
 from ._web_pub_sub_shared_private_link_resources_operations import WebPubSubSharedPrivateLinkResourcesOperations
 
 from ._patch import __all__ as _patch_all
-from ._patch import *  # type: ignore # pylint: disable=unused-wildcard-import
+from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "Operations",
     "WebPubSubOperations",
     "UsagesOperations",
     "WebPubSubCustomCertificatesOperations",
     "WebPubSubCustomDomainsOperations",
     "WebPubSubHubsOperations",
     "WebPubSubPrivateEndpointConnectionsOperations",
     "WebPubSubPrivateLinkResourcesOperations",
+    "WebPubSubReplicasOperations",
     "WebPubSubSharedPrivateLinkResourcesOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

## Comparing `azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_private_link_resources_operations.py` & `azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_private_link_resources_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, Iterable, Optional, TypeVar
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -26,48 +25,51 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(
     resource_group_name: str, resource_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-08-01-preview")
-    )  # type: Literal["2022-08-01-preview"]
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/privateLinkResources",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "resourceName": _SERIALIZER.url(
+            "resource_name",
+            resource_name,
+            "str",
+            max_length=63,
+            min_length=3,
+            pattern=r"^[a-zA-Z][a-zA-Z0-9-]{1,61}[a-zA-Z0-9]$",
+        ),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
@@ -95,31 +97,29 @@
 
     @distributed_trace
     def list(
         self, resource_group_name: str, resource_name: str, **kwargs: Any
     ) -> Iterable["_models.PrivateLinkResource"]:
         """Get the private link resources that need to be created for a resource.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either PrivateLinkResource or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.webpubsub.models.PrivateLinkResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.PrivateLinkResourceList]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.PrivateLinkResourceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -134,15 +134,15 @@
                     subscription_id=self._config.subscription_id,
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
@@ -150,36 +150,39 @@
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
             deserialized = self._deserialize("PrivateLinkResourceList", pipeline_response)
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
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/privateLinkResources"}  # type: ignore
+    list.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/privateLinkResources"
+    }
```

## Comparing `azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_custom_domains_operations.py` & `azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_custom_domains_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -28,48 +28,51 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(
     resource_group_name: str, resource_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-08-01-preview")
-    )  # type: Literal["2022-08-01-preview"]
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customDomains",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "resourceName": _SERIALIZER.url(
+            "resource_name",
+            resource_name,
+            "str",
+            max_length=63,
+            min_length=3,
+            pattern=r"^[a-zA-Z][a-zA-Z0-9-]{1,61}[a-zA-Z0-9]$",
+        ),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
@@ -78,32 +81,39 @@
 
 def build_get_request(
     resource_group_name: str, resource_name: str, name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-08-01-preview")
-    )  # type: Literal["2022-08-01-preview"]
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customDomains/{name}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "resourceName": _SERIALIZER.url(
+            "resource_name",
+            resource_name,
+            "str",
+            max_length=63,
+            min_length=3,
+            pattern=r"^[a-zA-Z][a-zA-Z0-9-]{1,61}[a-zA-Z0-9]$",
+        ),
         "name": _SERIALIZER.url("name", name, "str"),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
@@ -112,33 +122,40 @@
 
 def build_create_or_update_request(
     resource_group_name: str, resource_name: str, name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-08-01-preview")
-    )  # type: Literal["2022-08-01-preview"]
-    content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customDomains/{name}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "resourceName": _SERIALIZER.url(
+            "resource_name",
+            resource_name,
+            "str",
+            max_length=63,
+            min_length=3,
+            pattern=r"^[a-zA-Z][a-zA-Z0-9-]{1,61}[a-zA-Z0-9]$",
+        ),
         "name": _SERIALIZER.url("name", name, "str"),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
@@ -149,32 +166,39 @@
 
 def build_delete_request(
     resource_group_name: str, resource_name: str, name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-08-01-preview")
-    )  # type: Literal["2022-08-01-preview"]
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customDomains/{name}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "resourceName": _SERIALIZER.url(
+            "resource_name",
+            resource_name,
+            "str",
+            max_length=63,
+            min_length=3,
+            pattern=r"^[a-zA-Z][a-zA-Z0-9-]{1,61}[a-zA-Z0-9]$",
+        ),
         "name": _SERIALIZER.url("name", name, "str"),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
@@ -200,31 +224,29 @@
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
     def list(self, resource_group_name: str, resource_name: str, **kwargs: Any) -> Iterable["_models.CustomDomain"]:
         """List all custom domains.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either CustomDomain or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.webpubsub.models.CustomDomain]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.CustomDomainList]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.CustomDomainList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -239,15 +261,15 @@
                     subscription_id=self._config.subscription_id,
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
@@ -255,50 +277,53 @@
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
             deserialized = self._deserialize("CustomDomainList", pipeline_response)
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
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customDomains"}  # type: ignore
+    list.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customDomains"
+    }
 
     @distributed_trace
     def get(self, resource_group_name: str, resource_name: str, name: str, **kwargs: Any) -> _models.CustomDomain:
         """Get a custom domain.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :param name: Custom domain name. Required.
         :type name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: CustomDomain or the result of cls(response)
@@ -312,34 +337,33 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.CustomDomain]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.CustomDomain] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
             name=name,
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -348,15 +372,17 @@
         deserialized = self._deserialize("CustomDomain", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    get.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customDomains/{name}"}  # type: ignore
+    get.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customDomains/{name}"
+    }
 
     def _create_or_update_initial(
         self,
         resource_group_name: str,
         resource_name: str,
         name: str,
         parameters: Union[_models.CustomDomain, IO],
@@ -369,24 +395,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.CustomDomain]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.CustomDomain] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "CustomDomain")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
@@ -397,18 +421,19 @@
             json=_json,
             content=_content,
             template_url=self._create_or_update_initial.metadata["url"],
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
 
         if response.status_code not in [201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -417,31 +442,33 @@
         deserialized = self._deserialize("CustomDomain", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    _create_or_update_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customDomains/{name}"}  # type: ignore
+    _create_or_update_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customDomains/{name}"
+    }
 
     @overload
     def begin_create_or_update(
         self,
         resource_group_name: str,
         resource_name: str,
         name: str,
         parameters: _models.CustomDomain,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.CustomDomain]:
         """Create or update a custom domain.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :param name: Custom domain name. Required.
         :type name: str
         :param parameters: Required.
         :type parameters: ~azure.mgmt.webpubsub.models.CustomDomain
@@ -471,16 +498,16 @@
         parameters: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.CustomDomain]:
         """Create or update a custom domain.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :param name: Custom domain name. Required.
         :type name: str
         :param parameters: Required.
         :type parameters: IO
@@ -508,22 +535,22 @@
         resource_name: str,
         name: str,
         parameters: Union[_models.CustomDomain, IO],
         **kwargs: Any
     ) -> LROPoller[_models.CustomDomain]:
         """Create or update a custom domain.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :param name: Custom domain name. Required.
         :type name: str
-        :param parameters: Is either a model type or a IO type. Required.
+        :param parameters: Is either a CustomDomain type or a IO type. Required.
         :type parameters: ~azure.mgmt.webpubsub.models.CustomDomain or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json',
          'text/json'. Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -536,24 +563,22 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.webpubsub.models.CustomDomain]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.CustomDomain]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.CustomDomain] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = self._create_or_update_initial(  # type: ignore
+            raw_result = self._create_or_update_initial(
                 resource_group_name=resource_group_name,
                 resource_name=resource_name,
                 name=name,
                 parameters=parameters,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
@@ -566,29 +591,33 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("CustomDomain", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
         if polling is True:
-            polling_method = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))  # type: PollingMethod
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
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
 
-    begin_create_or_update.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customDomains/{name}"}  # type: ignore
+    begin_create_or_update.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customDomains/{name}"
+    }
 
     def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, resource_name: str, name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -596,54 +625,55 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
             name=name,
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
-    _delete_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customDomains/{name}"}  # type: ignore
+    _delete_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customDomains/{name}"
+    }
 
     @distributed_trace
     def begin_delete(self, resource_group_name: str, resource_name: str, name: str, **kwargs: Any) -> LROPoller[None]:
         """Delete a custom domain.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :param name: Custom domain name. Required.
         :type name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
@@ -656,21 +686,19 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
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
                 resource_name=resource_name,
                 name=name,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
@@ -681,24 +709,26 @@
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
                 return cls(pipeline_response, None, {})
 
         if polling is True:
-            polling_method = cast(
+            polling_method: PollingMethod = cast(
                 PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
-            )  # type: PollingMethod
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
 
-    begin_delete.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customDomains/{name}"}  # type: ignore
+    begin_delete.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customDomains/{name}"
+    }
```

## Comparing `azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/operations/_patch.py` & `azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_shared_private_link_resources_operations.py` & `azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_shared_private_link_resources_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -28,48 +28,51 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(
     resource_group_name: str, resource_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-08-01-preview")
-    )  # type: Literal["2022-08-01-preview"]
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/sharedPrivateLinkResources",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "resourceName": _SERIALIZER.url(
+            "resource_name",
+            resource_name,
+            "str",
+            max_length=63,
+            min_length=3,
+            pattern=r"^[a-zA-Z][a-zA-Z0-9-]{1,61}[a-zA-Z0-9]$",
+        ),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
@@ -82,34 +85,41 @@
     resource_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-08-01-preview")
-    )  # type: Literal["2022-08-01-preview"]
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/sharedPrivateLinkResources/{sharedPrivateLinkResourceName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "sharedPrivateLinkResourceName": _SERIALIZER.url(
             "shared_private_link_resource_name", shared_private_link_resource_name, "str"
         ),
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "resourceName": _SERIALIZER.url(
+            "resource_name",
+            resource_name,
+            "str",
+            max_length=63,
+            min_length=3,
+            pattern=r"^[a-zA-Z][a-zA-Z0-9-]{1,61}[a-zA-Z0-9]$",
+        ),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
@@ -122,35 +132,42 @@
     resource_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-08-01-preview")
-    )  # type: Literal["2022-08-01-preview"]
-    content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/sharedPrivateLinkResources/{sharedPrivateLinkResourceName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "sharedPrivateLinkResourceName": _SERIALIZER.url(
             "shared_private_link_resource_name", shared_private_link_resource_name, "str"
         ),
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "resourceName": _SERIALIZER.url(
+            "resource_name",
+            resource_name,
+            "str",
+            max_length=63,
+            min_length=3,
+            pattern=r"^[a-zA-Z][a-zA-Z0-9-]{1,61}[a-zA-Z0-9]$",
+        ),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
@@ -165,34 +182,41 @@
     resource_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-08-01-preview")
-    )  # type: Literal["2022-08-01-preview"]
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/sharedPrivateLinkResources/{sharedPrivateLinkResourceName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "sharedPrivateLinkResourceName": _SERIALIZER.url(
             "shared_private_link_resource_name", shared_private_link_resource_name, "str"
         ),
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "resourceName": _SERIALIZER.url(
+            "resource_name",
+            resource_name,
+            "str",
+            max_length=63,
+            min_length=3,
+            pattern=r"^[a-zA-Z][a-zA-Z0-9-]{1,61}[a-zA-Z0-9]$",
+        ),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
@@ -220,32 +244,30 @@
 
     @distributed_trace
     def list(
         self, resource_group_name: str, resource_name: str, **kwargs: Any
     ) -> Iterable["_models.SharedPrivateLinkResource"]:
         """List shared private link resources.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either SharedPrivateLinkResource or the result of
          cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.webpubsub.models.SharedPrivateLinkResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.SharedPrivateLinkResourceList]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.SharedPrivateLinkResourceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -260,15 +282,15 @@
                     subscription_id=self._config.subscription_id,
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
@@ -276,55 +298,58 @@
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
             deserialized = self._deserialize("SharedPrivateLinkResourceList", pipeline_response)
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
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/sharedPrivateLinkResources"}  # type: ignore
+    list.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/sharedPrivateLinkResources"
+    }
 
     @distributed_trace
     def get(
         self, shared_private_link_resource_name: str, resource_group_name: str, resource_name: str, **kwargs: Any
     ) -> _models.SharedPrivateLinkResource:
         """Get the specified shared private link resource.
 
         :param shared_private_link_resource_name: The name of the shared private link resource.
          Required.
         :type shared_private_link_resource_name: str
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: SharedPrivateLinkResource or the result of cls(response)
         :rtype: ~azure.mgmt.webpubsub.models.SharedPrivateLinkResource
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -336,34 +361,33 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.SharedPrivateLinkResource]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.SharedPrivateLinkResource] = kwargs.pop("cls", None)
 
         request = build_get_request(
             shared_private_link_resource_name=shared_private_link_resource_name,
             resource_group_name=resource_group_name,
             resource_name=resource_name,
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -372,15 +396,17 @@
         deserialized = self._deserialize("SharedPrivateLinkResource", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    get.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/sharedPrivateLinkResources/{sharedPrivateLinkResourceName}"}  # type: ignore
+    get.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/sharedPrivateLinkResources/{sharedPrivateLinkResourceName}"
+    }
 
     def _create_or_update_initial(
         self,
         shared_private_link_resource_name: str,
         resource_group_name: str,
         resource_name: str,
         parameters: Union[_models.SharedPrivateLinkResource, IO],
@@ -393,24 +419,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.SharedPrivateLinkResource]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.SharedPrivateLinkResource] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "SharedPrivateLinkResource")
 
         request = build_create_or_update_request(
             shared_private_link_resource_name=shared_private_link_resource_name,
             resource_group_name=resource_group_name,
@@ -421,18 +445,19 @@
             json=_json,
             content=_content,
             template_url=self._create_or_update_initial.metadata["url"],
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
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -441,19 +466,21 @@
         if response.status_code == 200:
             deserialized = self._deserialize("SharedPrivateLinkResource", pipeline_response)
 
         if response.status_code == 201:
             deserialized = self._deserialize("SharedPrivateLinkResource", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
+        return deserialized  # type: ignore
 
-    _create_or_update_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/sharedPrivateLinkResources/{sharedPrivateLinkResourceName}"}  # type: ignore
+    _create_or_update_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/sharedPrivateLinkResources/{sharedPrivateLinkResourceName}"
+    }
 
     @overload
     def begin_create_or_update(
         self,
         shared_private_link_resource_name: str,
         resource_group_name: str,
         resource_name: str,
@@ -463,16 +490,16 @@
         **kwargs: Any
     ) -> LROPoller[_models.SharedPrivateLinkResource]:
         """Create or update a shared private link resource.
 
         :param shared_private_link_resource_name: The name of the shared private link resource.
          Required.
         :type shared_private_link_resource_name: str
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :param parameters: The shared private link resource. Required.
         :type parameters: ~azure.mgmt.webpubsub.models.SharedPrivateLinkResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
@@ -503,16 +530,16 @@
         **kwargs: Any
     ) -> LROPoller[_models.SharedPrivateLinkResource]:
         """Create or update a shared private link resource.
 
         :param shared_private_link_resource_name: The name of the shared private link resource.
          Required.
         :type shared_private_link_resource_name: str
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :param parameters: The shared private link resource. Required.
         :type parameters: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
@@ -541,21 +568,21 @@
         **kwargs: Any
     ) -> LROPoller[_models.SharedPrivateLinkResource]:
         """Create or update a shared private link resource.
 
         :param shared_private_link_resource_name: The name of the shared private link resource.
          Required.
         :type shared_private_link_resource_name: str
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
-        :param parameters: The shared private link resource. Is either a model type or a IO type.
-         Required.
+        :param parameters: The shared private link resource. Is either a SharedPrivateLinkResource type
+         or a IO type. Required.
         :type parameters: ~azure.mgmt.webpubsub.models.SharedPrivateLinkResource or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -568,24 +595,22 @@
          of cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.webpubsub.models.SharedPrivateLinkResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.SharedPrivateLinkResource]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.SharedPrivateLinkResource] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = self._create_or_update_initial(  # type: ignore
+            raw_result = self._create_or_update_initial(
                 shared_private_link_resource_name=shared_private_link_resource_name,
                 resource_group_name=resource_group_name,
                 resource_name=resource_name,
                 parameters=parameters,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
@@ -598,29 +623,33 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("SharedPrivateLinkResource", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
         if polling is True:
-            polling_method = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))  # type: PollingMethod
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
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
 
-    begin_create_or_update.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/sharedPrivateLinkResources/{sharedPrivateLinkResourceName}"}  # type: ignore
+    begin_create_or_update.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/sharedPrivateLinkResources/{sharedPrivateLinkResourceName}"
+    }
 
     def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, shared_private_link_resource_name: str, resource_group_name: str, resource_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -628,59 +657,60 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             shared_private_link_resource_name=shared_private_link_resource_name,
             resource_group_name=resource_group_name,
             resource_name=resource_name,
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
-    _delete_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/sharedPrivateLinkResources/{sharedPrivateLinkResourceName}"}  # type: ignore
+    _delete_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/sharedPrivateLinkResources/{sharedPrivateLinkResourceName}"
+    }
 
     @distributed_trace
     def begin_delete(
         self, shared_private_link_resource_name: str, resource_group_name: str, resource_name: str, **kwargs: Any
     ) -> LROPoller[None]:
         """Delete the specified shared private link resource.
 
         :param shared_private_link_resource_name: The name of the shared private link resource.
          Required.
         :type shared_private_link_resource_name: str
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
@@ -691,21 +721,19 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
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
                 shared_private_link_resource_name=shared_private_link_resource_name,
                 resource_group_name=resource_group_name,
                 resource_name=resource_name,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
@@ -716,24 +744,26 @@
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
                 return cls(pipeline_response, None, {})
 
         if polling is True:
-            polling_method = cast(
+            polling_method: PollingMethod = cast(
                 PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
-            )  # type: PollingMethod
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
 
-    begin_delete.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/sharedPrivateLinkResources/{sharedPrivateLinkResourceName}"}  # type: ignore
+    begin_delete.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/sharedPrivateLinkResources/{sharedPrivateLinkResourceName}"
+    }
```

## Comparing `azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_custom_certificates_operations.py` & `azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_custom_certificates_operations.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -28,48 +28,51 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(
     resource_group_name: str, resource_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-08-01-preview")
-    )  # type: Literal["2022-08-01-preview"]
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customCertificates",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "resourceName": _SERIALIZER.url(
+            "resource_name",
+            resource_name,
+            "str",
+            max_length=63,
+            min_length=3,
+            pattern=r"^[a-zA-Z][a-zA-Z0-9-]{1,61}[a-zA-Z0-9]$",
+        ),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
@@ -78,32 +81,39 @@
 
 def build_get_request(
     resource_group_name: str, resource_name: str, certificate_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-08-01-preview")
-    )  # type: Literal["2022-08-01-preview"]
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customCertificates/{certificateName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "resourceName": _SERIALIZER.url(
+            "resource_name",
+            resource_name,
+            "str",
+            max_length=63,
+            min_length=3,
+            pattern=r"^[a-zA-Z][a-zA-Z0-9-]{1,61}[a-zA-Z0-9]$",
+        ),
         "certificateName": _SERIALIZER.url("certificate_name", certificate_name, "str"),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
@@ -112,33 +122,40 @@
 
 def build_create_or_update_request(
     resource_group_name: str, resource_name: str, certificate_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-08-01-preview")
-    )  # type: Literal["2022-08-01-preview"]
-    content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customCertificates/{certificateName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "resourceName": _SERIALIZER.url(
+            "resource_name",
+            resource_name,
+            "str",
+            max_length=63,
+            min_length=3,
+            pattern=r"^[a-zA-Z][a-zA-Z0-9-]{1,61}[a-zA-Z0-9]$",
+        ),
         "certificateName": _SERIALIZER.url("certificate_name", certificate_name, "str"),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
@@ -149,32 +166,39 @@
 
 def build_delete_request(
     resource_group_name: str, resource_name: str, certificate_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-08-01-preview")
-    )  # type: Literal["2022-08-01-preview"]
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customCertificates/{certificateName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "resourceName": _SERIALIZER.url(
+            "resource_name",
+            resource_name,
+            "str",
+            max_length=63,
+            min_length=3,
+            pattern=r"^[a-zA-Z][a-zA-Z0-9-]{1,61}[a-zA-Z0-9]$",
+        ),
         "certificateName": _SERIALIZER.url("certificate_name", certificate_name, "str"),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
@@ -202,31 +226,29 @@
 
     @distributed_trace
     def list(
         self, resource_group_name: str, resource_name: str, **kwargs: Any
     ) -> Iterable["_models.CustomCertificate"]:
         """List all custom certificates.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either CustomCertificate or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.webpubsub.models.CustomCertificate]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.CustomCertificateList]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.CustomCertificateList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -241,15 +263,15 @@
                     subscription_id=self._config.subscription_id,
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
@@ -257,52 +279,55 @@
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
             deserialized = self._deserialize("CustomCertificateList", pipeline_response)
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
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customCertificates"}  # type: ignore
+    list.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customCertificates"
+    }
 
     @distributed_trace
     def get(
         self, resource_group_name: str, resource_name: str, certificate_name: str, **kwargs: Any
     ) -> _models.CustomCertificate:
         """Get a custom certificate.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :param certificate_name: Custom certificate name. Required.
         :type certificate_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: CustomCertificate or the result of cls(response)
@@ -316,34 +341,33 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.CustomCertificate]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.CustomCertificate] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
             certificate_name=certificate_name,
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -352,15 +376,17 @@
         deserialized = self._deserialize("CustomCertificate", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    get.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customCertificates/{certificateName}"}  # type: ignore
+    get.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customCertificates/{certificateName}"
+    }
 
     def _create_or_update_initial(
         self,
         resource_group_name: str,
         resource_name: str,
         certificate_name: str,
         parameters: Union[_models.CustomCertificate, IO],
@@ -373,24 +399,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.CustomCertificate]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.CustomCertificate] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "CustomCertificate")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
@@ -401,18 +425,19 @@
             json=_json,
             content=_content,
             template_url=self._create_or_update_initial.metadata["url"],
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
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -421,35 +446,37 @@
         if response.status_code == 200:
             deserialized = self._deserialize("CustomCertificate", pipeline_response)
 
         if response.status_code == 201:
             deserialized = self._deserialize("CustomCertificate", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
+        return deserialized  # type: ignore
 
-    _create_or_update_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customCertificates/{certificateName}"}  # type: ignore
+    _create_or_update_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customCertificates/{certificateName}"
+    }
 
     @overload
     def begin_create_or_update(
         self,
         resource_group_name: str,
         resource_name: str,
         certificate_name: str,
         parameters: _models.CustomCertificate,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.CustomCertificate]:
         """Create or update a custom certificate.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :param certificate_name: Custom certificate name. Required.
         :type certificate_name: str
         :param parameters: Required.
         :type parameters: ~azure.mgmt.webpubsub.models.CustomCertificate
@@ -479,16 +506,16 @@
         parameters: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.CustomCertificate]:
         """Create or update a custom certificate.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :param certificate_name: Custom certificate name. Required.
         :type certificate_name: str
         :param parameters: Required.
         :type parameters: IO
@@ -516,22 +543,22 @@
         resource_name: str,
         certificate_name: str,
         parameters: Union[_models.CustomCertificate, IO],
         **kwargs: Any
     ) -> LROPoller[_models.CustomCertificate]:
         """Create or update a custom certificate.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :param certificate_name: Custom certificate name. Required.
         :type certificate_name: str
-        :param parameters: Is either a model type or a IO type. Required.
+        :param parameters: Is either a CustomCertificate type or a IO type. Required.
         :type parameters: ~azure.mgmt.webpubsub.models.CustomCertificate or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json',
          'text/json'. Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -544,24 +571,22 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.webpubsub.models.CustomCertificate]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.CustomCertificate]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.CustomCertificate] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = self._create_or_update_initial(  # type: ignore
+            raw_result = self._create_or_update_initial(
                 resource_group_name=resource_group_name,
                 resource_name=resource_name,
                 certificate_name=certificate_name,
                 parameters=parameters,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
@@ -574,38 +599,42 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("CustomCertificate", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
         if polling is True:
-            polling_method = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))  # type: PollingMethod
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
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
 
-    begin_create_or_update.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customCertificates/{certificateName}"}  # type: ignore
+    begin_create_or_update.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customCertificates/{certificateName}"
+    }
 
     @distributed_trace
     def delete(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, resource_name: str, certificate_name: str, **kwargs: Any
     ) -> None:
         """Delete a custom certificate.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :param certificate_name: Custom certificate name. Required.
         :type certificate_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
@@ -619,40 +648,41 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
             certificate_name=certificate_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.delete.metadata["url"],
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
 
         if response.status_code not in [200, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
-    delete.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customCertificates/{certificateName}"}  # type: ignore
+    delete.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customCertificates/{certificateName}"
+    }
```

## Comparing `azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/operations/_usages_operations.py` & `azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/operations/_usages_operations.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, Iterable, Optional, TypeVar
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -26,44 +25,38 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(location: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-08-01-preview")
-    )  # type: Literal["2022-08-01-preview"]
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.SignalRService/locations/{location}/usages"
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "location": _SERIALIZER.url("location", location, "str"),
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
@@ -99,18 +92,16 @@
         :return: An iterator like instance of either SignalRServiceUsage or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.webpubsub.models.SignalRServiceUsage]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.SignalRServiceUsageList]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.SignalRServiceUsageList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -124,15 +115,15 @@
                     subscription_id=self._config.subscription_id,
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
@@ -140,36 +131,39 @@
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
             deserialized = self._deserialize("SignalRServiceUsageList", pipeline_response)
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
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/providers/Microsoft.SignalRService/locations/{location}/usages"}  # type: ignore
+    list.metadata = {
+        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.SignalRService/locations/{location}/usages"
+    }
```

## Comparing `azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_hubs_operations.py` & `azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_hubs_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -28,48 +28,51 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(
     resource_group_name: str, resource_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-08-01-preview")
-    )  # type: Literal["2022-08-01-preview"]
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/hubs",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "resourceName": _SERIALIZER.url(
+            "resource_name",
+            resource_name,
+            "str",
+            max_length=63,
+            min_length=3,
+            pattern=r"^[a-zA-Z][a-zA-Z0-9-]{1,61}[a-zA-Z0-9]$",
+        ),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
@@ -78,32 +81,39 @@
 
 def build_get_request(
     hub_name: str, resource_group_name: str, resource_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-08-01-preview")
-    )  # type: Literal["2022-08-01-preview"]
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/hubs/{hubName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "hubName": _SERIALIZER.url("hub_name", hub_name, "str"),
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "resourceName": _SERIALIZER.url(
+            "resource_name",
+            resource_name,
+            "str",
+            max_length=63,
+            min_length=3,
+            pattern=r"^[a-zA-Z][a-zA-Z0-9-]{1,61}[a-zA-Z0-9]$",
+        ),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
@@ -112,33 +122,40 @@
 
 def build_create_or_update_request(
     hub_name: str, resource_group_name: str, resource_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-08-01-preview")
-    )  # type: Literal["2022-08-01-preview"]
-    content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/hubs/{hubName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "hubName": _SERIALIZER.url("hub_name", hub_name, "str"),
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "resourceName": _SERIALIZER.url(
+            "resource_name",
+            resource_name,
+            "str",
+            max_length=63,
+            min_length=3,
+            pattern=r"^[a-zA-Z][a-zA-Z0-9-]{1,61}[a-zA-Z0-9]$",
+        ),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
@@ -149,32 +166,39 @@
 
 def build_delete_request(
     hub_name: str, resource_group_name: str, resource_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-08-01-preview")
-    )  # type: Literal["2022-08-01-preview"]
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/hubs/{hubName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "hubName": _SERIALIZER.url("hub_name", hub_name, "str"),
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "resourceName": _SERIALIZER.url(
+            "resource_name",
+            resource_name,
+            "str",
+            max_length=63,
+            min_length=3,
+            pattern=r"^[a-zA-Z][a-zA-Z0-9-]{1,61}[a-zA-Z0-9]$",
+        ),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
@@ -200,31 +224,29 @@
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
     def list(self, resource_group_name: str, resource_name: str, **kwargs: Any) -> Iterable["_models.WebPubSubHub"]:
         """List hub settings.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either WebPubSubHub or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.webpubsub.models.WebPubSubHub]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.WebPubSubHubList]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.WebPubSubHubList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -239,15 +261,15 @@
                     subscription_id=self._config.subscription_id,
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
@@ -255,52 +277,55 @@
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
             deserialized = self._deserialize("WebPubSubHubList", pipeline_response)
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
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/hubs"}  # type: ignore
+    list.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/hubs"
+    }
 
     @distributed_trace
     def get(self, hub_name: str, resource_group_name: str, resource_name: str, **kwargs: Any) -> _models.WebPubSubHub:
         """Get a hub setting.
 
         :param hub_name: The hub name. Required.
         :type hub_name: str
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: WebPubSubHub or the result of cls(response)
         :rtype: ~azure.mgmt.webpubsub.models.WebPubSubHub
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -312,34 +337,33 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.WebPubSubHub]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.WebPubSubHub] = kwargs.pop("cls", None)
 
         request = build_get_request(
             hub_name=hub_name,
             resource_group_name=resource_group_name,
             resource_name=resource_name,
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -348,15 +372,17 @@
         deserialized = self._deserialize("WebPubSubHub", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    get.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/hubs/{hubName}"}  # type: ignore
+    get.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/hubs/{hubName}"
+    }
 
     def _create_or_update_initial(
         self,
         hub_name: str,
         resource_group_name: str,
         resource_name: str,
         parameters: Union[_models.WebPubSubHub, IO],
@@ -369,24 +395,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.WebPubSubHub]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.WebPubSubHub] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "WebPubSubHub")
 
         request = build_create_or_update_request(
             hub_name=hub_name,
             resource_group_name=resource_group_name,
@@ -397,18 +421,19 @@
             json=_json,
             content=_content,
             template_url=self._create_or_update_initial.metadata["url"],
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
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -417,19 +442,21 @@
         if response.status_code == 200:
             deserialized = self._deserialize("WebPubSubHub", pipeline_response)
 
         if response.status_code == 201:
             deserialized = self._deserialize("WebPubSubHub", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
+        return deserialized  # type: ignore
 
-    _create_or_update_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/hubs/{hubName}"}  # type: ignore
+    _create_or_update_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/hubs/{hubName}"
+    }
 
     @overload
     def begin_create_or_update(
         self,
         hub_name: str,
         resource_group_name: str,
         resource_name: str,
@@ -438,16 +465,16 @@
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.WebPubSubHub]:
         """Create or update a hub setting.
 
         :param hub_name: The hub name. Required.
         :type hub_name: str
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :param parameters: The resource of WebPubSubHub and its properties. Required.
         :type parameters: ~azure.mgmt.webpubsub.models.WebPubSubHub
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
@@ -477,16 +504,16 @@
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.WebPubSubHub]:
         """Create or update a hub setting.
 
         :param hub_name: The hub name. Required.
         :type hub_name: str
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :param parameters: The resource of WebPubSubHub and its properties. Required.
         :type parameters: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
@@ -514,21 +541,21 @@
         parameters: Union[_models.WebPubSubHub, IO],
         **kwargs: Any
     ) -> LROPoller[_models.WebPubSubHub]:
         """Create or update a hub setting.
 
         :param hub_name: The hub name. Required.
         :type hub_name: str
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
-        :param parameters: The resource of WebPubSubHub and its properties. Is either a model type or a
-         IO type. Required.
+        :param parameters: The resource of WebPubSubHub and its properties. Is either a WebPubSubHub
+         type or a IO type. Required.
         :type parameters: ~azure.mgmt.webpubsub.models.WebPubSubHub or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -541,24 +568,22 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.webpubsub.models.WebPubSubHub]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.WebPubSubHub]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.WebPubSubHub] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = self._create_or_update_initial(  # type: ignore
+            raw_result = self._create_or_update_initial(
                 hub_name=hub_name,
                 resource_group_name=resource_group_name,
                 resource_name=resource_name,
                 parameters=parameters,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
@@ -571,29 +596,33 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("WebPubSubHub", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
         if polling is True:
-            polling_method = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))  # type: PollingMethod
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
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
 
-    begin_create_or_update.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/hubs/{hubName}"}  # type: ignore
+    begin_create_or_update.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/hubs/{hubName}"
+    }
 
     def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, hub_name: str, resource_group_name: str, resource_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -601,58 +630,59 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             hub_name=hub_name,
             resource_group_name=resource_group_name,
             resource_name=resource_name,
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
-    _delete_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/hubs/{hubName}"}  # type: ignore
+    _delete_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/hubs/{hubName}"
+    }
 
     @distributed_trace
     def begin_delete(
         self, hub_name: str, resource_group_name: str, resource_name: str, **kwargs: Any
     ) -> LROPoller[None]:
         """Delete a hub setting.
 
         :param hub_name: The hub name. Required.
         :type hub_name: str
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
@@ -663,21 +693,19 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
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
                 hub_name=hub_name,
                 resource_group_name=resource_group_name,
                 resource_name=resource_name,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
@@ -688,24 +716,26 @@
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
                 return cls(pipeline_response, None, {})
 
         if polling is True:
-            polling_method = cast(
+            polling_method: PollingMethod = cast(
                 PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
-            )  # type: PollingMethod
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
 
-    begin_delete.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/hubs/{hubName}"}  # type: ignore
+    begin_delete.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/hubs/{hubName}"
+    }
```

## Comparing `azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/operations/_operations.py` & `azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/operations/_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, Iterable, Optional, TypeVar
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -26,32 +25,26 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(**kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-08-01-preview")
-    )  # type: Literal["2022-08-01-preview"]
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/providers/Microsoft.SignalRService/operations")
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -89,18 +82,16 @@
         :return: An iterator like instance of either Operation or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.webpubsub.models.Operation]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.OperationList]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.OperationList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -112,15 +103,15 @@
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
@@ -128,36 +119,37 @@
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
             deserialized = self._deserialize("OperationList", pipeline_response)
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
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
-    list.metadata = {"url": "/providers/Microsoft.SignalRService/operations"}  # type: ignore
+    list.metadata = {"url": "/providers/Microsoft.SignalRService/operations"}
```

## Comparing `azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_private_endpoint_connections_operations.py` & `azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_private_endpoint_connections_operations.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -28,48 +28,51 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(
     resource_group_name: str, resource_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-08-01-preview")
-    )  # type: Literal["2022-08-01-preview"]
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/privateEndpointConnections",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "resourceName": _SERIALIZER.url(
+            "resource_name",
+            resource_name,
+            "str",
+            max_length=63,
+            min_length=3,
+            pattern=r"^[a-zA-Z][a-zA-Z0-9-]{1,61}[a-zA-Z0-9]$",
+        ),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
@@ -82,34 +85,41 @@
     resource_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-08-01-preview")
-    )  # type: Literal["2022-08-01-preview"]
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "privateEndpointConnectionName": _SERIALIZER.url(
             "private_endpoint_connection_name", private_endpoint_connection_name, "str"
         ),
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "resourceName": _SERIALIZER.url(
+            "resource_name",
+            resource_name,
+            "str",
+            max_length=63,
+            min_length=3,
+            pattern=r"^[a-zA-Z][a-zA-Z0-9-]{1,61}[a-zA-Z0-9]$",
+        ),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
@@ -122,35 +132,42 @@
     resource_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-08-01-preview")
-    )  # type: Literal["2022-08-01-preview"]
-    content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "privateEndpointConnectionName": _SERIALIZER.url(
             "private_endpoint_connection_name", private_endpoint_connection_name, "str"
         ),
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "resourceName": _SERIALIZER.url(
+            "resource_name",
+            resource_name,
+            "str",
+            max_length=63,
+            min_length=3,
+            pattern=r"^[a-zA-Z][a-zA-Z0-9-]{1,61}[a-zA-Z0-9]$",
+        ),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
@@ -165,34 +182,41 @@
     resource_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-08-01-preview")
-    )  # type: Literal["2022-08-01-preview"]
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "privateEndpointConnectionName": _SERIALIZER.url(
             "private_endpoint_connection_name", private_endpoint_connection_name, "str"
         ),
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "resourceName": _SERIALIZER.url(
+            "resource_name",
+            resource_name,
+            "str",
+            max_length=63,
+            min_length=3,
+            pattern=r"^[a-zA-Z][a-zA-Z0-9-]{1,61}[a-zA-Z0-9]$",
+        ),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
@@ -220,32 +244,30 @@
 
     @distributed_trace
     def list(
         self, resource_group_name: str, resource_name: str, **kwargs: Any
     ) -> Iterable["_models.PrivateEndpointConnection"]:
         """List private endpoint connections.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either PrivateEndpointConnection or the result of
          cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.webpubsub.models.PrivateEndpointConnection]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.PrivateEndpointConnectionList]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.PrivateEndpointConnectionList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -260,15 +282,15 @@
                     subscription_id=self._config.subscription_id,
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
@@ -276,54 +298,58 @@
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
             deserialized = self._deserialize("PrivateEndpointConnectionList", pipeline_response)
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
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/privateEndpointConnections"}  # type: ignore
+    list.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/privateEndpointConnections"
+    }
 
     @distributed_trace
     def get(
         self, private_endpoint_connection_name: str, resource_group_name: str, resource_name: str, **kwargs: Any
     ) -> _models.PrivateEndpointConnection:
         """Get the specified private endpoint connection.
 
-        :param private_endpoint_connection_name: The name of the private endpoint connection. Required.
+        :param private_endpoint_connection_name: The name of the private endpoint connection associated
+         with the Azure resource. Required.
         :type private_endpoint_connection_name: str
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PrivateEndpointConnection or the result of cls(response)
         :rtype: ~azure.mgmt.webpubsub.models.PrivateEndpointConnection
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -335,34 +361,33 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.PrivateEndpointConnection]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.PrivateEndpointConnection] = kwargs.pop("cls", None)
 
         request = build_get_request(
             private_endpoint_connection_name=private_endpoint_connection_name,
             resource_group_name=resource_group_name,
             resource_name=resource_name,
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -371,33 +396,36 @@
         deserialized = self._deserialize("PrivateEndpointConnection", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    get.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}"}  # type: ignore
+    get.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}"
+    }
 
     @overload
     def update(
         self,
         private_endpoint_connection_name: str,
         resource_group_name: str,
         resource_name: str,
         parameters: _models.PrivateEndpointConnection,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.PrivateEndpointConnection:
         """Update the state of specified private endpoint connection.
 
-        :param private_endpoint_connection_name: The name of the private endpoint connection. Required.
+        :param private_endpoint_connection_name: The name of the private endpoint connection associated
+         with the Azure resource. Required.
         :type private_endpoint_connection_name: str
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :param parameters: The resource of private endpoint and its properties. Required.
         :type parameters: ~azure.mgmt.webpubsub.models.PrivateEndpointConnection
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
@@ -417,18 +445,19 @@
         parameters: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.PrivateEndpointConnection:
         """Update the state of specified private endpoint connection.
 
-        :param private_endpoint_connection_name: The name of the private endpoint connection. Required.
+        :param private_endpoint_connection_name: The name of the private endpoint connection associated
+         with the Azure resource. Required.
         :type private_endpoint_connection_name: str
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :param parameters: The resource of private endpoint and its properties. Required.
         :type parameters: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
@@ -446,23 +475,24 @@
         resource_group_name: str,
         resource_name: str,
         parameters: Union[_models.PrivateEndpointConnection, IO],
         **kwargs: Any
     ) -> _models.PrivateEndpointConnection:
         """Update the state of specified private endpoint connection.
 
-        :param private_endpoint_connection_name: The name of the private endpoint connection. Required.
+        :param private_endpoint_connection_name: The name of the private endpoint connection associated
+         with the Azure resource. Required.
         :type private_endpoint_connection_name: str
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
-        :param parameters: The resource of private endpoint and its properties. Is either a model type
-         or a IO type. Required.
+        :param parameters: The resource of private endpoint and its properties. Is either a
+         PrivateEndpointConnection type or a IO type. Required.
         :type parameters: ~azure.mgmt.webpubsub.models.PrivateEndpointConnection or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PrivateEndpointConnection or the result of cls(response)
         :rtype: ~azure.mgmt.webpubsub.models.PrivateEndpointConnection
@@ -475,24 +505,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.PrivateEndpointConnection]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.PrivateEndpointConnection] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "PrivateEndpointConnection")
 
         request = build_update_request(
             private_endpoint_connection_name=private_endpoint_connection_name,
             resource_group_name=resource_group_name,
@@ -503,18 +531,19 @@
             json=_json,
             content=_content,
             template_url=self.update.metadata["url"],
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -523,15 +552,17 @@
         deserialized = self._deserialize("PrivateEndpointConnection", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    update.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}"}  # type: ignore
+    update.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}"
+    }
 
     def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, private_endpoint_connection_name: str, resource_group_name: str, resource_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -539,58 +570,60 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             private_endpoint_connection_name=private_endpoint_connection_name,
             resource_group_name=resource_group_name,
             resource_name=resource_name,
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
-    _delete_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}"}  # type: ignore
+    _delete_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}"
+    }
 
     @distributed_trace
     def begin_delete(
         self, private_endpoint_connection_name: str, resource_group_name: str, resource_name: str, **kwargs: Any
     ) -> LROPoller[None]:
         """Delete the specified private endpoint connection.
 
-        :param private_endpoint_connection_name: The name of the private endpoint connection. Required.
+        :param private_endpoint_connection_name: The name of the private endpoint connection associated
+         with the Azure resource. Required.
         :type private_endpoint_connection_name: str
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
@@ -601,21 +634,19 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
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
                 private_endpoint_connection_name=private_endpoint_connection_name,
                 resource_group_name=resource_group_name,
                 resource_name=resource_name,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
@@ -626,24 +657,26 @@
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
                 return cls(pipeline_response, None, {})
 
         if polling is True:
-            polling_method = cast(
+            polling_method: PollingMethod = cast(
                 PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
-            )  # type: PollingMethod
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
 
-    begin_delete.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}"}  # type: ignore
+    begin_delete.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}"
+    }
```

## Comparing `azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_operations.py` & `azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/operations/_web_pub_sub_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -28,46 +28,40 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_check_name_availability_request(location: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-08-01-preview")
-    )  # type: Literal["2022-08-01-preview"]
-    content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/providers/Microsoft.SignalRService/locations/{location}/checkNameAvailability",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "location": _SERIALIZER.url("location", location, "str"),
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
@@ -76,87 +70,92 @@
     return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_list_by_subscription_request(subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-08-01-preview")
-    )  # type: Literal["2022-08-01-preview"]
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.SignalRService/webPubSub")
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
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
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-08-01-preview")
-    )  # type: Literal["2022-08-01-preview"]
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_get_request(resource_group_name: str, resource_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-08-01-preview")
-    )  # type: Literal["2022-08-01-preview"]
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "resourceName": _SERIALIZER.url(
+            "resource_name",
+            resource_name,
+            "str",
+            max_length=63,
+            min_length=3,
+            pattern=r"^[a-zA-Z][a-zA-Z0-9-]{1,61}[a-zA-Z0-9]$",
+        ),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
@@ -165,32 +164,39 @@
 
 def build_create_or_update_request(
     resource_group_name: str, resource_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-08-01-preview")
-    )  # type: Literal["2022-08-01-preview"]
-    content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "resourceName": _SERIALIZER.url(
+            "resource_name",
+            resource_name,
+            "str",
+            max_length=63,
+            min_length=3,
+            pattern=r"^[a-zA-Z][a-zA-Z0-9-]{1,61}[a-zA-Z0-9]$",
+        ),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
@@ -201,31 +207,38 @@
 
 def build_delete_request(
     resource_group_name: str, resource_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-08-01-preview")
-    )  # type: Literal["2022-08-01-preview"]
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "resourceName": _SERIALIZER.url(
+            "resource_name",
+            resource_name,
+            "str",
+            max_length=63,
+            min_length=3,
+            pattern=r"^[a-zA-Z][a-zA-Z0-9-]{1,61}[a-zA-Z0-9]$",
+        ),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
@@ -234,32 +247,39 @@
 
 def build_update_request(
     resource_group_name: str, resource_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-08-01-preview")
-    )  # type: Literal["2022-08-01-preview"]
-    content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "resourceName": _SERIALIZER.url(
+            "resource_name",
+            resource_name,
+            "str",
+            max_length=63,
+            min_length=3,
+            pattern=r"^[a-zA-Z][a-zA-Z0-9-]{1,61}[a-zA-Z0-9]$",
+        ),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
@@ -270,31 +290,38 @@
 
 def build_list_keys_request(
     resource_group_name: str, resource_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-08-01-preview")
-    )  # type: Literal["2022-08-01-preview"]
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/listKeys",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "resourceName": _SERIALIZER.url(
+            "resource_name",
+            resource_name,
+            "str",
+            max_length=63,
+            min_length=3,
+            pattern=r"^[a-zA-Z][a-zA-Z0-9-]{1,61}[a-zA-Z0-9]$",
+        ),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
@@ -303,67 +330,129 @@
 
 def build_regenerate_key_request(
     resource_group_name: str, resource_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-08-01-preview")
-    )  # type: Literal["2022-08-01-preview"]
-    content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/regenerateKey",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "resourceName": _SERIALIZER.url(
+            "resource_name",
+            resource_name,
+            "str",
+            max_length=63,
+            min_length=3,
+            pattern=r"^[a-zA-Z][a-zA-Z0-9-]{1,61}[a-zA-Z0-9]$",
+        ),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
+def build_list_replica_skus_request(
+    resource_group_name: str, resource_name: str, replica_name: str, subscription_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/replicas/{replicaName}/skus",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "resourceName": _SERIALIZER.url(
+            "resource_name",
+            resource_name,
+            "str",
+            max_length=63,
+            min_length=3,
+            pattern=r"^[a-zA-Z][a-zA-Z0-9-]{1,61}[a-zA-Z0-9]$",
+        ),
+        "replicaName": _SERIALIZER.url(
+            "replica_name",
+            replica_name,
+            "str",
+            max_length=63,
+            min_length=3,
+            pattern=r"^[a-zA-Z][a-zA-Z0-9-]{1,61}[a-zA-Z0-9]$",
+        ),
+    }
+
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
+
+
 def build_restart_request(
     resource_group_name: str, resource_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-08-01-preview")
-    )  # type: Literal["2022-08-01-preview"]
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/restart",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "resourceName": _SERIALIZER.url(
+            "resource_name",
+            resource_name,
+            "str",
+            max_length=63,
+            min_length=3,
+            pattern=r"^[a-zA-Z][a-zA-Z0-9-]{1,61}[a-zA-Z0-9]$",
+        ),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
@@ -372,31 +461,38 @@
 
 def build_list_skus_request(
     resource_group_name: str, resource_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-08-01-preview")
-    )  # type: Literal["2022-08-01-preview"]
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/skus",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "resourceName": _SERIALIZER.url(
+            "resource_name",
+            resource_name,
+            "str",
+            max_length=63,
+            min_length=3,
+            pattern=r"^[a-zA-Z][a-zA-Z0-9-]{1,61}[a-zA-Z0-9]$",
+        ),
     }
 
-    _url = _format_url_section(_url, **path_format_arguments)
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
@@ -469,16 +565,16 @@
     def check_name_availability(
         self, location: str, parameters: Union[_models.NameAvailabilityParameters, IO], **kwargs: Any
     ) -> _models.NameAvailability:
         """Checks that the resource name is valid and is not already in use.
 
         :param location: the region. Required.
         :type location: str
-        :param parameters: Parameters supplied to the operation. Is either a model type or a IO type.
-         Required.
+        :param parameters: Parameters supplied to the operation. Is either a NameAvailabilityParameters
+         type or a IO type. Required.
         :type parameters: ~azure.mgmt.webpubsub.models.NameAvailabilityParameters or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: NameAvailability or the result of cls(response)
         :rtype: ~azure.mgmt.webpubsub.models.NameAvailability
@@ -491,24 +587,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.NameAvailability]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.NameAvailability] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "NameAvailabilityParameters")
 
         request = build_check_name_availability_request(
             location=location,
             subscription_id=self._config.subscription_id,
@@ -517,18 +611,19 @@
             json=_json,
             content=_content,
             template_url=self.check_name_availability.metadata["url"],
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -537,32 +632,32 @@
         deserialized = self._deserialize("NameAvailability", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    check_name_availability.metadata = {"url": "/subscriptions/{subscriptionId}/providers/Microsoft.SignalRService/locations/{location}/checkNameAvailability"}  # type: ignore
+    check_name_availability.metadata = {
+        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.SignalRService/locations/{location}/checkNameAvailability"
+    }
 
     @distributed_trace
     def list_by_subscription(self, **kwargs: Any) -> Iterable["_models.WebPubSubResource"]:
         """Handles requests to list all resources in a subscription.
 
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either WebPubSubResource or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.webpubsub.models.WebPubSubResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.WebPubSubResourceList]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.WebPubSubResourceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -575,15 +670,15 @@
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
@@ -591,63 +686,64 @@
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
             deserialized = self._deserialize("WebPubSubResourceList", pipeline_response)
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
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
-    list_by_subscription.metadata = {"url": "/subscriptions/{subscriptionId}/providers/Microsoft.SignalRService/webPubSub"}  # type: ignore
+    list_by_subscription.metadata = {
+        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.SignalRService/webPubSub"
+    }
 
     @distributed_trace
     def list_by_resource_group(self, resource_group_name: str, **kwargs: Any) -> Iterable["_models.WebPubSubResource"]:
         """Handles requests to list all resources in a resource group.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either WebPubSubResource or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.webpubsub.models.WebPubSubResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.WebPubSubResourceList]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.WebPubSubResourceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -661,15 +757,15 @@
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
@@ -677,50 +773,53 @@
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
             deserialized = self._deserialize("WebPubSubResourceList", pipeline_response)
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
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
-    list_by_resource_group.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub"}  # type: ignore
+    list_by_resource_group.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub"
+    }
 
     @distributed_trace
     def get(self, resource_group_name: str, resource_name: str, **kwargs: Any) -> _models.WebPubSubResource:
         """Get the resource and its properties.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: WebPubSubResource or the result of cls(response)
         :rtype: ~azure.mgmt.webpubsub.models.WebPubSubResource
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -732,33 +831,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.WebPubSubResource]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.WebPubSubResource] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -767,15 +865,17 @@
         deserialized = self._deserialize("WebPubSubResource", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    get.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}"}  # type: ignore
+    get.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}"
+    }
 
     def _create_or_update_initial(
         self,
         resource_group_name: str,
         resource_name: str,
         parameters: Union[_models.WebPubSubResource, IO],
         **kwargs: Any
@@ -787,24 +887,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[Optional[_models.WebPubSubResource]]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[Optional[_models.WebPubSubResource]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "WebPubSubResource")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
@@ -814,18 +912,19 @@
             json=_json,
             content=_content,
             template_url=self._create_or_update_initial.metadata["url"],
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
 
         if response.status_code not in [200, 201, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -839,30 +938,32 @@
             deserialized = self._deserialize("WebPubSubResource", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    _create_or_update_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}"}  # type: ignore
+    _create_or_update_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}"
+    }
 
     @overload
     def begin_create_or_update(
         self,
         resource_group_name: str,
         resource_name: str,
         parameters: _models.WebPubSubResource,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.WebPubSubResource]:
         """Create or update a resource.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :param parameters: Parameters for the create or update operation. Required.
         :type parameters: ~azure.mgmt.webpubsub.models.WebPubSubResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
@@ -889,16 +990,16 @@
         parameters: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.WebPubSubResource]:
         """Create or update a resource.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :param parameters: Parameters for the create or update operation. Required.
         :type parameters: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
@@ -923,21 +1024,21 @@
         resource_group_name: str,
         resource_name: str,
         parameters: Union[_models.WebPubSubResource, IO],
         **kwargs: Any
     ) -> LROPoller[_models.WebPubSubResource]:
         """Create or update a resource.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
-        :param parameters: Parameters for the create or update operation. Is either a model type or a
-         IO type. Required.
+        :param parameters: Parameters for the create or update operation. Is either a WebPubSubResource
+         type or a IO type. Required.
         :type parameters: ~azure.mgmt.webpubsub.models.WebPubSubResource or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -950,24 +1051,22 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.webpubsub.models.WebPubSubResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.WebPubSubResource]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.WebPubSubResource] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = self._create_or_update_initial(  # type: ignore
+            raw_result = self._create_or_update_initial(
                 resource_group_name=resource_group_name,
                 resource_name=resource_name,
                 parameters=parameters,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
@@ -979,29 +1078,33 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("WebPubSubResource", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
         if polling is True:
-            polling_method = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))  # type: PollingMethod
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
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
 
-    begin_create_or_update.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}"}  # type: ignore
+    begin_create_or_update.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}"
+    }
 
     def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, resource_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -1009,53 +1112,54 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
-    _delete_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}"}  # type: ignore
+    _delete_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}"
+    }
 
     @distributed_trace
     def begin_delete(self, resource_group_name: str, resource_name: str, **kwargs: Any) -> LROPoller[None]:
         """Operation to delete a resource.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
@@ -1066,21 +1170,19 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
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
                 resource_name=resource_name,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
                 headers=_headers,
@@ -1090,31 +1192,33 @@
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
                 return cls(pipeline_response, None, {})
 
         if polling is True:
-            polling_method = cast(
+            polling_method: PollingMethod = cast(
                 PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
-            )  # type: PollingMethod
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
 
-    begin_delete.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}"}  # type: ignore
+    begin_delete.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}"
+    }
 
     def _update_initial(
         self,
         resource_group_name: str,
         resource_name: str,
         parameters: Union[_models.WebPubSubResource, IO],
         **kwargs: Any
@@ -1126,24 +1230,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[Optional[_models.WebPubSubResource]]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[Optional[_models.WebPubSubResource]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "WebPubSubResource")
 
         request = build_update_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
@@ -1153,52 +1255,59 @@
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = None
+        response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("WebPubSubResource", pipeline_response)
 
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, response_headers)
 
         return deserialized
 
-    _update_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}"}  # type: ignore
+    _update_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}"
+    }
 
     @overload
     def begin_update(
         self,
         resource_group_name: str,
         resource_name: str,
         parameters: _models.WebPubSubResource,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.WebPubSubResource]:
         """Operation to update an exiting resource.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :param parameters: Parameters for the update operation. Required.
         :type parameters: ~azure.mgmt.webpubsub.models.WebPubSubResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
@@ -1225,16 +1334,16 @@
         parameters: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.WebPubSubResource]:
         """Operation to update an exiting resource.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :param parameters: Parameters for the update operation. Required.
         :type parameters: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
@@ -1259,21 +1368,21 @@
         resource_group_name: str,
         resource_name: str,
         parameters: Union[_models.WebPubSubResource, IO],
         **kwargs: Any
     ) -> LROPoller[_models.WebPubSubResource]:
         """Operation to update an exiting resource.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
-        :param parameters: Parameters for the update operation. Is either a model type or a IO type.
-         Required.
+        :param parameters: Parameters for the update operation. Is either a WebPubSubResource type or a
+         IO type. Required.
         :type parameters: ~azure.mgmt.webpubsub.models.WebPubSubResource or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -1286,24 +1395,22 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.webpubsub.models.WebPubSubResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.WebPubSubResource]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.WebPubSubResource] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = self._update_initial(  # type: ignore
+            raw_result = self._update_initial(
                 resource_group_name=resource_group_name,
                 resource_name=resource_name,
                 parameters=parameters,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
@@ -1315,36 +1422,40 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("WebPubSubResource", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
         if polling is True:
-            polling_method = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))  # type: PollingMethod
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
 
-    begin_update.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}"}  # type: ignore
+    begin_update.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}"
+    }
 
     @distributed_trace
     def list_keys(self, resource_group_name: str, resource_name: str, **kwargs: Any) -> _models.WebPubSubKeys:
         """Get the access keys of the resource.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: WebPubSubKeys or the result of cls(response)
         :rtype: ~azure.mgmt.webpubsub.models.WebPubSubKeys
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -1356,33 +1467,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.WebPubSubKeys]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.WebPubSubKeys] = kwargs.pop("cls", None)
 
         request = build_list_keys_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.list_keys.metadata["url"],
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -1391,15 +1501,17 @@
         deserialized = self._deserialize("WebPubSubKeys", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    list_keys.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/listKeys"}  # type: ignore
+    list_keys.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/listKeys"
+    }
 
     def _regenerate_key_initial(
         self,
         resource_group_name: str,
         resource_name: str,
         parameters: Union[_models.RegenerateKeyParameters, IO],
         **kwargs: Any
@@ -1411,24 +1523,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.WebPubSubKeys]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.WebPubSubKeys] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "RegenerateKeyParameters")
 
         request = build_regenerate_key_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
@@ -1438,51 +1548,61 @@
             json=_json,
             content=_content,
             template_url=self._regenerate_key_initial.metadata["url"],
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
 
-        if response.status_code not in [202]:
+        if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize("WebPubSubKeys", pipeline_response)
+        response_headers = {}
+        if response.status_code == 200:
+            deserialized = self._deserialize("WebPubSubKeys", pipeline_response)
+
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+
+            deserialized = self._deserialize("WebPubSubKeys", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
-        return deserialized
+        return deserialized  # type: ignore
 
-    _regenerate_key_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/regenerateKey"}  # type: ignore
+    _regenerate_key_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/regenerateKey"
+    }
 
     @overload
     def begin_regenerate_key(
         self,
         resource_group_name: str,
         resource_name: str,
         parameters: _models.RegenerateKeyParameters,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.WebPubSubKeys]:
         """Regenerate the access key for the resource. PrimaryKey and SecondaryKey cannot be regenerated
         at the same time.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :param parameters: Parameter that describes the Regenerate Key Operation. Required.
         :type parameters: ~azure.mgmt.webpubsub.models.RegenerateKeyParameters
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
@@ -1510,16 +1630,16 @@
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.WebPubSubKeys]:
         """Regenerate the access key for the resource. PrimaryKey and SecondaryKey cannot be regenerated
         at the same time.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :param parameters: Parameter that describes the Regenerate Key Operation. Required.
         :type parameters: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
@@ -1545,21 +1665,21 @@
         resource_name: str,
         parameters: Union[_models.RegenerateKeyParameters, IO],
         **kwargs: Any
     ) -> LROPoller[_models.WebPubSubKeys]:
         """Regenerate the access key for the resource. PrimaryKey and SecondaryKey cannot be regenerated
         at the same time.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
-        :param parameters: Parameter that describes the Regenerate Key Operation. Is either a model
-         type or a IO type. Required.
+        :param parameters: Parameter that describes the Regenerate Key Operation. Is either a
+         RegenerateKeyParameters type or a IO type. Required.
         :type parameters: ~azure.mgmt.webpubsub.models.RegenerateKeyParameters or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -1572,24 +1692,22 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.webpubsub.models.WebPubSubKeys]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.WebPubSubKeys]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.WebPubSubKeys] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = self._regenerate_key_initial(  # type: ignore
+            raw_result = self._regenerate_key_initial(
                 resource_group_name=resource_group_name,
                 resource_name=resource_name,
                 parameters=parameters,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
@@ -1601,31 +1719,101 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("WebPubSubKeys", pipeline_response)
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
+
+    begin_regenerate_key.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/regenerateKey"
+    }
+
+    @distributed_trace
+    def list_replica_skus(
+        self, resource_group_name: str, resource_name: str, replica_name: str, **kwargs: Any
+    ) -> _models.SkuList:
+        """List all available skus of the replica resource.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param resource_name: The name of the resource. Required.
+        :type resource_name: str
+        :param replica_name: The name of the replica. Required.
+        :type replica_name: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :return: SkuList or the result of cls(response)
+        :rtype: ~azure.mgmt.webpubsub.models.SkuList
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.SkuList] = kwargs.pop("cls", None)
+
+        request = build_list_replica_skus_request(
+            resource_group_name=resource_group_name,
+            resource_name=resource_name,
+            replica_name=replica_name,
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            template_url=self.list_replica_skus.metadata["url"],
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
+        deserialized = self._deserialize("SkuList", pipeline_response)
 
-    begin_regenerate_key.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/regenerateKey"}  # type: ignore
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    list_replica_skus.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/replicas/{replicaName}/skus"
+    }
 
     def _restart_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, resource_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -1633,53 +1821,58 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_restart_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self._restart_initial.metadata["url"],
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
 
         if response.status_code not in [202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
+        response_headers = {}
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, None, response_headers)
 
-    _restart_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/restart"}  # type: ignore
+    _restart_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/restart"
+    }
 
     @distributed_trace
     def begin_restart(self, resource_group_name: str, resource_name: str, **kwargs: Any) -> LROPoller[None]:
         """Operation to restart a resource.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
@@ -1690,21 +1883,19 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._restart_initial(  # type: ignore
                 resource_group_name=resource_group_name,
                 resource_name=resource_name,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
                 headers=_headers,
@@ -1714,38 +1905,40 @@
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
 
-    begin_restart.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/restart"}  # type: ignore
+    begin_restart.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/restart"
+    }
 
     @distributed_trace
     def list_skus(self, resource_group_name: str, resource_name: str, **kwargs: Any) -> _models.SkuList:
         """List all available skus of the resource.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: SkuList or the result of cls(response)
         :rtype: ~azure.mgmt.webpubsub.models.SkuList
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -1757,33 +1950,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.SkuList]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.SkuList] = kwargs.pop("cls", None)
 
         request = build_list_skus_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.list_skus.metadata["url"],
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -1792,8 +1984,10 @@
         deserialized = self._deserialize("SkuList", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    list_skus.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/skus"}  # type: ignore
+    list_skus.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/skus"
+    }
```

## Comparing `azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/models/__init__.py` & `azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,16 @@
 from ._models_py3 import PrivateEndpointConnection
 from ._models_py3 import PrivateEndpointConnectionList
 from ._models_py3 import PrivateLinkResource
 from ._models_py3 import PrivateLinkResourceList
 from ._models_py3 import PrivateLinkServiceConnectionState
 from ._models_py3 import ProxyResource
 from ._models_py3 import RegenerateKeyParameters
+from ._models_py3 import Replica
+from ._models_py3 import ReplicaList
 from ._models_py3 import Resource
 from ._models_py3 import ResourceLogCategory
 from ._models_py3 import ResourceLogConfiguration
 from ._models_py3 import ResourceReference
 from ._models_py3 import ResourceSku
 from ._models_py3 import ServiceSpecification
 from ._models_py3 import ShareablePrivateLinkResourceProperties
@@ -76,20 +78,21 @@
 from ._web_pub_sub_management_client_enums import EventListenerEndpointDiscriminator
 from ._web_pub_sub_management_client_enums import EventListenerFilterDiscriminator
 from ._web_pub_sub_management_client_enums import KeyType
 from ._web_pub_sub_management_client_enums import ManagedIdentityType
 from ._web_pub_sub_management_client_enums import PrivateLinkServiceConnectionStatus
 from ._web_pub_sub_management_client_enums import ProvisioningState
 from ._web_pub_sub_management_client_enums import ScaleType
+from ._web_pub_sub_management_client_enums import ServiceKind
 from ._web_pub_sub_management_client_enums import SharedPrivateLinkResourceStatus
 from ._web_pub_sub_management_client_enums import UpstreamAuthType
 from ._web_pub_sub_management_client_enums import WebPubSubRequestType
 from ._web_pub_sub_management_client_enums import WebPubSubSkuTier
 from ._patch import __all__ as _patch_all
-from ._patch import *  # type: ignore # pylint: disable=unused-wildcard-import
+from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "CustomCertificate",
     "CustomCertificateList",
     "CustomDomain",
     "CustomDomainList",
@@ -121,14 +124,16 @@
     "PrivateEndpointConnection",
     "PrivateEndpointConnectionList",
     "PrivateLinkResource",
     "PrivateLinkResourceList",
     "PrivateLinkServiceConnectionState",
     "ProxyResource",
     "RegenerateKeyParameters",
+    "Replica",
+    "ReplicaList",
     "Resource",
     "ResourceLogCategory",
     "ResourceLogConfiguration",
     "ResourceReference",
     "ResourceSku",
     "ServiceSpecification",
     "ShareablePrivateLinkResourceProperties",
@@ -158,14 +163,15 @@
     "EventListenerEndpointDiscriminator",
     "EventListenerFilterDiscriminator",
     "KeyType",
     "ManagedIdentityType",
     "PrivateLinkServiceConnectionStatus",
     "ProvisioningState",
     "ScaleType",
+    "ServiceKind",
     "SharedPrivateLinkResourceStatus",
     "UpstreamAuthType",
     "WebPubSubRequestType",
     "WebPubSubSkuTier",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

## Comparing `azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/models/_patch.py` & `azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/models/_web_pub_sub_management_client_enums.py` & `azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/models/_web_pub_sub_management_client_enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,21 @@
     """The scale type applicable to the sku."""
 
     NONE = "None"
     MANUAL = "Manual"
     AUTOMATIC = "Automatic"
 
 
+class ServiceKind(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """The kind of the service."""
+
+    WEB_PUB_SUB = "WebPubSub"
+    SOCKET_IO = "SocketIO"
+
+
 class SharedPrivateLinkResourceStatus(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Status of the shared private link resource."""
 
     PENDING = "Pending"
     APPROVED = "Approved"
     REJECTED = "Rejected"
     DISCONNECTED = "Disconnected"
```

## Comparing `azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/models/_models_py3.py` & `azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/models/_models_py3.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,100 +4,119 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 import datetime
-from typing import Dict, List, Optional, TYPE_CHECKING, Union
+from typing import Any, Dict, List, Optional, TYPE_CHECKING, Union
 
 from .. import _serialization
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from .. import models as _models
 
 
 class Resource(_serialization.Model):
-    """The core properties of ARM resources.
+    """Common fields that are returned in the response for all Azure Resource Manager resources.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    :ivar id: Fully qualified resource Id for the resource.
+    :ivar id: Fully qualified resource ID for the resource. E.g.
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
-    :ivar type: The type of the resource - e.g. "Microsoft.SignalRService/SignalR".
+    :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
+     "Microsoft.Storage/storageAccounts".
     :vartype type: str
+    :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
+     information.
+    :vartype system_data: ~azure.mgmt.webpubsub.models.SystemData
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
         "type": {"readonly": True},
+        "system_data": {"readonly": True},
     }
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
+        "system_data": {"key": "systemData", "type": "SystemData"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.id = None
         self.name = None
         self.type = None
+        self.system_data = None
 
 
 class ProxyResource(Resource):
-    """The resource model definition for a ARM proxy resource. It will have everything other than required location and tags.
+    """The resource model definition for a Azure Resource Manager proxy resource. It will not have
+    tags and a location.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    :ivar id: Fully qualified resource Id for the resource.
+    :ivar id: Fully qualified resource ID for the resource. E.g.
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
-    :ivar type: The type of the resource - e.g. "Microsoft.SignalRService/SignalR".
+    :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
+     "Microsoft.Storage/storageAccounts".
     :vartype type: str
+    :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
+     information.
+    :vartype system_data: ~azure.mgmt.webpubsub.models.SystemData
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
         "type": {"readonly": True},
+        "system_data": {"readonly": True},
     }
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
+        "system_data": {"key": "systemData", "type": "SystemData"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
 
 
 class CustomCertificate(ProxyResource):
     """A custom certificate.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     All required parameters must be populated in order to send to Azure.
 
-    :ivar id: Fully qualified resource Id for the resource.
+    :ivar id: Fully qualified resource ID for the resource. E.g.
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
-    :ivar type: The type of the resource - e.g. "Microsoft.SignalRService/SignalR".
+    :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
+     "Microsoft.Storage/storageAccounts".
     :vartype type: str
-    :ivar system_data: Metadata pertaining to creation and last modification of the resource.
+    :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
+     information.
     :vartype system_data: ~azure.mgmt.webpubsub.models.SystemData
     :ivar provisioning_state: Provisioning state of the resource. Known values are: "Unknown",
      "Succeeded", "Failed", "Canceled", "Running", "Creating", "Updating", "Deleting", and "Moving".
     :vartype provisioning_state: str or ~azure.mgmt.webpubsub.models.ProvisioningState
     :ivar key_vault_base_uri: Base uri of the KeyVault that stores certificate. Required.
     :vartype key_vault_base_uri: str
     :ivar key_vault_secret_name: Certificate secret name. Required.
@@ -129,26 +148,25 @@
 
     def __init__(
         self,
         *,
         key_vault_base_uri: str,
         key_vault_secret_name: str,
         key_vault_secret_version: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword key_vault_base_uri: Base uri of the KeyVault that stores certificate. Required.
         :paramtype key_vault_base_uri: str
         :keyword key_vault_secret_name: Certificate secret name. Required.
         :paramtype key_vault_secret_name: str
         :keyword key_vault_secret_version: Certificate secret version.
         :paramtype key_vault_secret_version: str
         """
         super().__init__(**kwargs)
-        self.system_data = None
         self.provisioning_state = None
         self.key_vault_base_uri = key_vault_base_uri
         self.key_vault_secret_name = key_vault_secret_name
         self.key_vault_secret_version = key_vault_secret_version
 
 
 class CustomCertificateList(_serialization.Model):
@@ -163,16 +181,20 @@
 
     _attribute_map = {
         "value": {"key": "value", "type": "[CustomCertificate]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
     def __init__(
-        self, *, value: Optional[List["_models.CustomCertificate"]] = None, next_link: Optional[str] = None, **kwargs
-    ):
+        self,
+        *,
+        value: Optional[List["_models.CustomCertificate"]] = None,
+        next_link: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
         """
         :keyword value: List of custom certificates of this resource.
         :paramtype value: list[~azure.mgmt.webpubsub.models.CustomCertificate]
         :keyword next_link: The URL the client should use to fetch the next page (per server side
          paging).
          It's null for now, added for future use.
         :paramtype next_link: str
@@ -185,21 +207,24 @@
 class CustomDomain(ProxyResource):
     """A custom domain.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     All required parameters must be populated in order to send to Azure.
 
-    :ivar id: Fully qualified resource Id for the resource.
+    :ivar id: Fully qualified resource ID for the resource. E.g.
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
-    :ivar type: The type of the resource - e.g. "Microsoft.SignalRService/SignalR".
+    :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
+     "Microsoft.Storage/storageAccounts".
     :vartype type: str
-    :ivar system_data: Metadata pertaining to creation and last modification of the resource.
+    :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
+     information.
     :vartype system_data: ~azure.mgmt.webpubsub.models.SystemData
     :ivar provisioning_state: Provisioning state of the resource. Known values are: "Unknown",
      "Succeeded", "Failed", "Canceled", "Running", "Creating", "Updating", "Deleting", and "Moving".
     :vartype provisioning_state: str or ~azure.mgmt.webpubsub.models.ProvisioningState
     :ivar domain_name: The custom domain name. Required.
     :vartype domain_name: str
     :ivar custom_certificate: Reference to a resource. Required.
@@ -222,23 +247,22 @@
         "type": {"key": "type", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
         "provisioning_state": {"key": "properties.provisioningState", "type": "str"},
         "domain_name": {"key": "properties.domainName", "type": "str"},
         "custom_certificate": {"key": "properties.customCertificate", "type": "ResourceReference"},
     }
 
-    def __init__(self, *, domain_name: str, custom_certificate: "_models.ResourceReference", **kwargs):
+    def __init__(self, *, domain_name: str, custom_certificate: "_models.ResourceReference", **kwargs: Any) -> None:
         """
         :keyword domain_name: The custom domain name. Required.
         :paramtype domain_name: str
         :keyword custom_certificate: Reference to a resource. Required.
         :paramtype custom_certificate: ~azure.mgmt.webpubsub.models.ResourceReference
         """
         super().__init__(**kwargs)
-        self.system_data = None
         self.provisioning_state = None
         self.domain_name = domain_name
         self.custom_certificate = custom_certificate
 
 
 class CustomDomainList(_serialization.Model):
     """Custom domains list.
@@ -252,16 +276,16 @@
 
     _attribute_map = {
         "value": {"key": "value", "type": "[CustomDomain]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
     def __init__(
-        self, *, value: Optional[List["_models.CustomDomain"]] = None, next_link: Optional[str] = None, **kwargs
-    ):
+        self, *, value: Optional[List["_models.CustomDomain"]] = None, next_link: Optional[str] = None, **kwargs: Any
+    ) -> None:
         """
         :keyword value: List of custom domains that bind to this resource.
         :paramtype value: list[~azure.mgmt.webpubsub.models.CustomDomain]
         :keyword next_link: The URL the client should use to fetch the next page (per server side
          paging).
          It's null for now, added for future use.
         :paramtype next_link: str
@@ -295,16 +319,16 @@
     def __init__(
         self,
         *,
         name: Optional[str] = None,
         display_name: Optional[str] = None,
         internal_name: Optional[str] = None,
         to_be_exported_for_shoebox: Optional[bool] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword name: The public facing name of the dimension.
         :paramtype name: str
         :keyword display_name: Localized friendly display name of the dimension.
         :paramtype display_name: str
         :keyword internal_name: Name of the dimension as it appears in MDM.
         :paramtype internal_name: str
@@ -336,15 +360,15 @@
     }
 
     _attribute_map = {
         "type": {"key": "type", "type": "str"},
         "info": {"key": "info", "type": "object"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.type = None
         self.info = None
 
 
 class ErrorDetail(_serialization.Model):
@@ -376,36 +400,37 @@
         "code": {"key": "code", "type": "str"},
         "message": {"key": "message", "type": "str"},
         "target": {"key": "target", "type": "str"},
         "details": {"key": "details", "type": "[ErrorDetail]"},
         "additional_info": {"key": "additionalInfo", "type": "[ErrorAdditionalInfo]"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.code = None
         self.message = None
         self.target = None
         self.details = None
         self.additional_info = None
 
 
 class ErrorResponse(_serialization.Model):
-    """Common error response for all Azure Resource Manager APIs to return error details for failed operations. (This also follows the OData error response format.).
+    """Common error response for all Azure Resource Manager APIs to return error details for failed
+    operations. (This also follows the OData error response format.).
 
     :ivar error: The error object.
     :vartype error: ~azure.mgmt.webpubsub.models.ErrorDetail
     """
 
     _attribute_map = {
         "error": {"key": "error", "type": "ErrorDetail"},
     }
 
-    def __init__(self, *, error: Optional["_models.ErrorDetail"] = None, **kwargs):
+    def __init__(self, *, error: Optional["_models.ErrorDetail"] = None, **kwargs: Any) -> None:
         """
         :keyword error: The error object.
         :paramtype error: ~azure.mgmt.webpubsub.models.ErrorDetail
         """
         super().__init__(**kwargs)
         self.error = error
 
@@ -451,16 +476,16 @@
     def __init__(
         self,
         *,
         url_template: str,
         user_event_pattern: Optional[str] = None,
         system_events: Optional[List[str]] = None,
         auth: Optional["_models.UpstreamAuthSettings"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword url_template: Gets or sets the EventHandler URL template. You can use a predefined
          parameter {hub} and {event} inside the template, the value of the EventHandler URL is
          dynamically calculated when the client request comes in.
          For example, UrlTemplate can be ``http://example.com/api/{hub}/{event}``. The host part can't
          contains parameters. Required.
         :paramtype url_template: str
@@ -504,57 +529,58 @@
 
     _attribute_map = {
         "type": {"key": "type", "type": "str"},
     }
 
     _subtype_map = {"type": {"EventHub": "EventHubEndpoint"}}
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
-        self.type = None  # type: Optional[str]
+        self.type: Optional[str] = None
 
 
 class EventHubEndpoint(EventListenerEndpoint):
     """An Event Hub endpoint.
-    The managed identity of Web PubSub service must be enabled, and the identity should have the "Azure Event Hubs Data sender" role to access Event Hub.
+    The managed identity of Web PubSub service must be enabled, and the identity should have the
+    "Azure Event Hubs Data sender" role to access Event Hub.
 
-        All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to Azure.
 
-        :ivar type: Required. "EventHub"
-        :vartype type: str or ~azure.mgmt.webpubsub.models.EventListenerEndpointDiscriminator
-        :ivar fully_qualified_namespace: The fully qualified namespace name of the Event Hub resource.
-         For example, "example.servicebus.windows.net". Required.
-        :vartype fully_qualified_namespace: str
-        :ivar event_hub_name: The name of the Event Hub. Required.
-        :vartype event_hub_name: str
+    :ivar type: Required. "EventHub"
+    :vartype type: str or ~azure.mgmt.webpubsub.models.EventListenerEndpointDiscriminator
+    :ivar fully_qualified_namespace: The fully qualified namespace name of the Event Hub resource.
+     For example, "example.servicebus.windows.net". Required.
+    :vartype fully_qualified_namespace: str
+    :ivar event_hub_name: The name of the Event Hub. Required.
+    :vartype event_hub_name: str
     """
 
     _validation = {
         "type": {"required": True},
         "fully_qualified_namespace": {"required": True},
         "event_hub_name": {"required": True},
     }
 
     _attribute_map = {
         "type": {"key": "type", "type": "str"},
         "fully_qualified_namespace": {"key": "fullyQualifiedNamespace", "type": "str"},
         "event_hub_name": {"key": "eventHubName", "type": "str"},
     }
 
-    def __init__(self, *, fully_qualified_namespace: str, event_hub_name: str, **kwargs):
+    def __init__(self, *, fully_qualified_namespace: str, event_hub_name: str, **kwargs: Any) -> None:
         """
         :keyword fully_qualified_namespace: The fully qualified namespace name of the Event Hub
          resource. For example, "example.servicebus.windows.net". Required.
         :paramtype fully_qualified_namespace: str
         :keyword event_hub_name: The name of the Event Hub. Required.
         :paramtype event_hub_name: str
         """
         super().__init__(**kwargs)
-        self.type = "EventHub"  # type: str
+        self.type: str = "EventHub"
         self.fully_qualified_namespace = fully_qualified_namespace
         self.event_hub_name = event_hub_name
 
 
 class EventListener(_serialization.Model):
     """A setting defines which kinds of events should be sent to which endpoint.
 
@@ -578,30 +604,31 @@
     }
 
     def __init__(
         self,
         *,
         filter: "_models.EventListenerFilter",  # pylint: disable=redefined-builtin
         endpoint: "_models.EventListenerEndpoint",
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword filter: A base class for event filter which determines whether an event should be sent
          to an event listener. Required.
         :paramtype filter: ~azure.mgmt.webpubsub.models.EventListenerFilter
         :keyword endpoint: An endpoint specifying where Web PubSub should send events to. Required.
         :paramtype endpoint: ~azure.mgmt.webpubsub.models.EventListenerEndpoint
         """
         super().__init__(**kwargs)
         self.filter = filter
         self.endpoint = endpoint
 
 
 class EventListenerFilter(_serialization.Model):
-    """A base class for event filter which determines whether an event should be sent to an event listener.
+    """A base class for event filter which determines whether an event should be sent to an event
+    listener.
 
     You probably want to use the sub-classes and not this class directly. Known sub-classes are:
     EventNameFilter
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar type: Required. "EventName"
@@ -614,18 +641,18 @@
 
     _attribute_map = {
         "type": {"key": "type", "type": "str"},
     }
 
     _subtype_map = {"type": {"EventName": "EventNameFilter"}}
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
-        self.type = None  # type: Optional[str]
+        self.type: Optional[str] = None
 
 
 class EventNameFilter(EventListenerFilter):
     """Filter events by their name.
 
     All required parameters must be populated in order to send to Azure.
 
@@ -653,16 +680,16 @@
     _attribute_map = {
         "type": {"key": "type", "type": "str"},
         "system_events": {"key": "systemEvents", "type": "[str]"},
         "user_event_pattern": {"key": "userEventPattern", "type": "str"},
     }
 
     def __init__(
-        self, *, system_events: Optional[List[str]] = None, user_event_pattern: Optional[str] = None, **kwargs
-    ):
+        self, *, system_events: Optional[List[str]] = None, user_event_pattern: Optional[str] = None, **kwargs: Any
+    ) -> None:
         """
         :keyword system_events: Gets or sets a list of system events. Supported events: "connected" and
          "disconnected". Blocking event "connect" is not supported because it requires a response.
         :paramtype system_events: list[str]
         :keyword user_event_pattern: Gets or sets a matching pattern for event names.
          There are 3 kinds of patterns supported:
 
@@ -671,15 +698,15 @@
             1. "*", it matches any event name
             2. Combine multiple events with ",", for example "event1,event2", it matches events
          "event1" and "event2"
             3. A single event name, for example, "event1", it matches "event1".
         :paramtype user_event_pattern: str
         """
         super().__init__(**kwargs)
-        self.type = "EventName"  # type: str
+        self.type: str = "EventName"
         self.system_events = system_events
         self.user_event_pattern = user_event_pattern
 
 
 class LiveTraceCategory(_serialization.Model):
     """Live trace category configuration of a Microsoft.SignalRService resource.
 
@@ -694,15 +721,15 @@
     """
 
     _attribute_map = {
         "name": {"key": "name", "type": "str"},
         "enabled": {"key": "enabled", "type": "str"},
     }
 
-    def __init__(self, *, name: Optional[str] = None, enabled: Optional[str] = None, **kwargs):
+    def __init__(self, *, name: Optional[str] = None, enabled: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword name: Gets or sets the live trace category's name.
          Available values: ConnectivityLogs, MessagingLogs.
          Case insensitive.
         :paramtype name: str
         :keyword enabled: Indicates whether or the live trace category is enabled.
          Available values: true, false.
@@ -730,16 +757,16 @@
 
     _attribute_map = {
         "enabled": {"key": "enabled", "type": "str"},
         "categories": {"key": "categories", "type": "[LiveTraceCategory]"},
     }
 
     def __init__(
-        self, *, enabled: str = "false", categories: Optional[List["_models.LiveTraceCategory"]] = None, **kwargs
-    ):
+        self, *, enabled: str = "false", categories: Optional[List["_models.LiveTraceCategory"]] = None, **kwargs: Any
+    ) -> None:
         """
         :keyword enabled: Indicates whether or not enable live trace.
          When it's set to true, live trace client can connect to the service.
          Otherwise, live trace client can't connect to the service, so that you are unable to receive
          any log, no matter what you configure in "categories".
          Available values: true, false.
          Case insensitive.
@@ -762,15 +789,15 @@
     """
 
     _attribute_map = {
         "name": {"key": "name", "type": "str"},
         "display_name": {"key": "displayName", "type": "str"},
     }
 
-    def __init__(self, *, name: Optional[str] = None, display_name: Optional[str] = None, **kwargs):
+    def __init__(self, *, name: Optional[str] = None, display_name: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword name: Name of the log.
         :paramtype name: str
         :keyword display_name: Localized friendly display name of the log.
         :paramtype display_name: str
         """
         super().__init__(**kwargs)
@@ -810,16 +837,16 @@
     }
 
     def __init__(
         self,
         *,
         type: Optional[Union[str, "_models.ManagedIdentityType"]] = None,
         user_assigned_identities: Optional[Dict[str, "_models.UserAssignedIdentityProperty"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword type: Represents the identity type: systemAssigned, userAssigned, None. Known values
          are: "None", "SystemAssigned", and "UserAssigned".
         :paramtype type: str or ~azure.mgmt.webpubsub.models.ManagedIdentityType
         :keyword user_assigned_identities: Get or set the user assigned identities.
         :paramtype user_assigned_identities: dict[str,
          ~azure.mgmt.webpubsub.models.UserAssignedIdentityProperty]
@@ -839,15 +866,15 @@
     :vartype resource: str
     """
 
     _attribute_map = {
         "resource": {"key": "resource", "type": "str"},
     }
 
-    def __init__(self, *, resource: Optional[str] = None, **kwargs):
+    def __init__(self, *, resource: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword resource: The Resource indicating the App ID URI of the target resource.
          It also appears in the aud (audience) claim of the issued token.
         :paramtype resource: str
         """
         super().__init__(**kwargs)
         self.resource = resource
@@ -899,16 +926,16 @@
         display_name: Optional[str] = None,
         display_description: Optional[str] = None,
         unit: Optional[str] = None,
         aggregation_type: Optional[str] = None,
         fill_gap_with_zero: Optional[str] = None,
         category: Optional[str] = None,
         dimensions: Optional[List["_models.Dimension"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword name: Name of the metric.
         :paramtype name: str
         :keyword display_name: Localized friendly display name of the metric.
         :paramtype display_name: str
         :keyword display_description: Localized friendly description of the metric.
         :paramtype display_description: str
@@ -938,15 +965,16 @@
         self.aggregation_type = aggregation_type
         self.fill_gap_with_zero = fill_gap_with_zero
         self.category = category
         self.dimensions = dimensions
 
 
 class NameAvailability(_serialization.Model):
-    """Result of the request to check name availability. It contains a flag and possible reason of failure.
+    """Result of the request to check name availability. It contains a flag and possible reason of
+    failure.
 
     :ivar name_available: Indicates whether the name is available or not.
     :vartype name_available: bool
     :ivar reason: The reason of the availability. Required if name is not available.
     :vartype reason: str
     :ivar message: The message of the operation.
     :vartype message: str
@@ -960,16 +988,16 @@
 
     def __init__(
         self,
         *,
         name_available: Optional[bool] = None,
         reason: Optional[str] = None,
         message: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword name_available: Indicates whether the name is available or not.
         :paramtype name_available: bool
         :keyword reason: The reason of the availability. Required if name is not available.
         :paramtype reason: str
         :keyword message: The message of the operation.
         :paramtype message: str
@@ -981,16 +1009,17 @@
 
 
 class NameAvailabilityParameters(_serialization.Model):
     """Data POST-ed to the nameAvailability action.
 
     All required parameters must be populated in order to send to Azure.
 
-    :ivar type: The resource type. Can be "Microsoft.SignalRService/SignalR" or
-     "Microsoft.SignalRService/webPubSub". Required.
+    :ivar type: The resource type. Can be "Microsoft.SignalRService/SignalR",
+     "Microsoft.SignalRService/WebPubSub", "Microsoft.SignalRService/SignalR/replicas" or
+     "Microsoft.SignalRService/WebPubSub/replicas". Required.
     :vartype type: str
     :ivar name: The resource name to validate. e.g."my-resource-name". Required.
     :vartype name: str
     """
 
     _validation = {
         "type": {"required": True},
@@ -998,18 +1027,19 @@
     }
 
     _attribute_map = {
         "type": {"key": "type", "type": "str"},
         "name": {"key": "name", "type": "str"},
     }
 
-    def __init__(self, *, type: str, name: str, **kwargs):
+    def __init__(self, *, type: str, name: str, **kwargs: Any) -> None:
         """
-        :keyword type: The resource type. Can be "Microsoft.SignalRService/SignalR" or
-         "Microsoft.SignalRService/webPubSub". Required.
+        :keyword type: The resource type. Can be "Microsoft.SignalRService/SignalR",
+         "Microsoft.SignalRService/WebPubSub", "Microsoft.SignalRService/SignalR/replicas" or
+         "Microsoft.SignalRService/WebPubSub/replicas". Required.
         :paramtype type: str
         :keyword name: The resource name to validate. e.g."my-resource-name". Required.
         :paramtype name: str
         """
         super().__init__(**kwargs)
         self.type = type
         self.name = name
@@ -1032,16 +1062,16 @@
     }
 
     def __init__(
         self,
         *,
         allow: Optional[List[Union[str, "_models.WebPubSubRequestType"]]] = None,
         deny: Optional[List[Union[str, "_models.WebPubSubRequestType"]]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword allow: Allowed request types. The value can be one or more of: ClientConnection,
          ServerConnection, RESTAPI.
         :paramtype allow: list[str or ~azure.mgmt.webpubsub.models.WebPubSubRequestType]
         :keyword deny: Denied request types. The value can be one or more of: ClientConnection,
          ServerConnection, RESTAPI.
         :paramtype deny: list[str or ~azure.mgmt.webpubsub.models.WebPubSubRequestType]
@@ -1079,16 +1109,16 @@
         self,
         *,
         name: Optional[str] = None,
         is_data_action: Optional[bool] = None,
         display: Optional["_models.OperationDisplay"] = None,
         origin: Optional[str] = None,
         properties: Optional["_models.OperationProperties"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword name: Name of the operation with format: {provider}/{resource}/{operation}.
         :paramtype name: str
         :keyword is_data_action: If the operation is a data action. (for data plane rbac).
         :paramtype is_data_action: bool
         :keyword display: The object that describes a operation.
         :paramtype display: ~azure.mgmt.webpubsub.models.OperationDisplay
@@ -1129,16 +1159,16 @@
     def __init__(
         self,
         *,
         provider: Optional[str] = None,
         resource: Optional[str] = None,
         operation: Optional[str] = None,
         description: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword provider: Friendly name of the resource provider.
         :paramtype provider: str
         :keyword resource: Resource type on which the operation is performed.
         :paramtype resource: str
         :keyword operation: The localized friendly name for the operation.
         :paramtype operation: str
@@ -1163,15 +1193,17 @@
     """
 
     _attribute_map = {
         "value": {"key": "value", "type": "[Operation]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: Optional[List["_models.Operation"]] = None, next_link: Optional[str] = None, **kwargs):
+    def __init__(
+        self, *, value: Optional[List["_models.Operation"]] = None, next_link: Optional[str] = None, **kwargs: Any
+    ) -> None:
         """
         :keyword value: List of operations supported by the resource provider.
         :paramtype value: list[~azure.mgmt.webpubsub.models.Operation]
         :keyword next_link: The URL the client should use to fetch the next page (per server side
          paging).
          It's null for now, added for future use.
         :paramtype next_link: str
@@ -1188,15 +1220,17 @@
     :vartype service_specification: ~azure.mgmt.webpubsub.models.ServiceSpecification
     """
 
     _attribute_map = {
         "service_specification": {"key": "serviceSpecification", "type": "ServiceSpecification"},
     }
 
-    def __init__(self, *, service_specification: Optional["_models.ServiceSpecification"] = None, **kwargs):
+    def __init__(
+        self, *, service_specification: Optional["_models.ServiceSpecification"] = None, **kwargs: Any
+    ) -> None:
         """
         :keyword service_specification: An object that describes a specification.
         :paramtype service_specification: ~azure.mgmt.webpubsub.models.ServiceSpecification
         """
         super().__init__(**kwargs)
         self.service_specification = service_specification
 
@@ -1208,15 +1242,15 @@
     :vartype id: str
     """
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
     }
 
-    def __init__(self, *, id: Optional[str] = None, **kwargs):  # pylint: disable=redefined-builtin
+    def __init__(self, *, id: Optional[str] = None, **kwargs: Any) -> None:  # pylint: disable=redefined-builtin
         """
         :keyword id: Full qualified Id of the private endpoint.
         :paramtype id: str
         """
         super().__init__(**kwargs)
         self.id = id
 
@@ -1248,16 +1282,16 @@
 
     def __init__(
         self,
         *,
         name: str,
         allow: Optional[List[Union[str, "_models.WebPubSubRequestType"]]] = None,
         deny: Optional[List[Union[str, "_models.WebPubSubRequestType"]]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword allow: Allowed request types. The value can be one or more of: ClientConnection,
          ServerConnection, RESTAPI.
         :paramtype allow: list[str or ~azure.mgmt.webpubsub.models.WebPubSubRequestType]
         :keyword deny: Denied request types. The value can be one or more of: ClientConnection,
          ServerConnection, RESTAPI.
         :paramtype deny: list[str or ~azure.mgmt.webpubsub.models.WebPubSubRequestType]
@@ -1269,21 +1303,24 @@
 
 
 class PrivateEndpointConnection(ProxyResource):
     """A private endpoint connection to an azure resource.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    :ivar id: Fully qualified resource Id for the resource.
+    :ivar id: Fully qualified resource ID for the resource. E.g.
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
-    :ivar type: The type of the resource - e.g. "Microsoft.SignalRService/SignalR".
+    :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
+     "Microsoft.Storage/storageAccounts".
     :vartype type: str
-    :ivar system_data: Metadata pertaining to creation and last modification of the resource.
+    :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
+     information.
     :vartype system_data: ~azure.mgmt.webpubsub.models.SystemData
     :ivar provisioning_state: Provisioning state of the resource. Known values are: "Unknown",
      "Succeeded", "Failed", "Canceled", "Running", "Creating", "Updating", "Deleting", and "Moving".
     :vartype provisioning_state: str or ~azure.mgmt.webpubsub.models.ProvisioningState
     :ivar private_endpoint: Private endpoint.
     :vartype private_endpoint: ~azure.mgmt.webpubsub.models.PrivateEndpoint
     :ivar group_ids: Group IDs.
@@ -1318,26 +1355,25 @@
     }
 
     def __init__(
         self,
         *,
         private_endpoint: Optional["_models.PrivateEndpoint"] = None,
         private_link_service_connection_state: Optional["_models.PrivateLinkServiceConnectionState"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword private_endpoint: Private endpoint.
         :paramtype private_endpoint: ~azure.mgmt.webpubsub.models.PrivateEndpoint
         :keyword private_link_service_connection_state: Connection state of the private endpoint
          connection.
         :paramtype private_link_service_connection_state:
          ~azure.mgmt.webpubsub.models.PrivateLinkServiceConnectionState
         """
         super().__init__(**kwargs)
-        self.system_data = None
         self.provisioning_state = None
         self.private_endpoint = private_endpoint
         self.group_ids = None
         self.private_link_service_connection_state = private_link_service_connection_state
 
 
 class PrivateEndpointConnectionList(_serialization.Model):
@@ -1357,16 +1393,16 @@
     }
 
     def __init__(
         self,
         *,
         value: Optional[List["_models.PrivateEndpointConnection"]] = None,
         next_link: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword value: The list of the private endpoint connections.
         :paramtype value: list[~azure.mgmt.webpubsub.models.PrivateEndpointConnection]
         :keyword next_link: Request URL that can be used to query next page of private endpoint
          connections. Returned when the total number of requested private endpoint connections exceed
          maximum page size.
         :paramtype next_link: str
@@ -1377,20 +1413,25 @@
 
 
 class PrivateLinkResource(ProxyResource):
     """Private link resource.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    :ivar id: Fully qualified resource Id for the resource.
+    :ivar id: Fully qualified resource ID for the resource. E.g.
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
-    :ivar type: The type of the resource - e.g. "Microsoft.SignalRService/SignalR".
+    :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
+     "Microsoft.Storage/storageAccounts".
     :vartype type: str
+    :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
+     information.
+    :vartype system_data: ~azure.mgmt.webpubsub.models.SystemData
     :ivar group_id: Group Id of the private link resource.
     :vartype group_id: str
     :ivar required_members: Required members of the private link resource.
     :vartype required_members: list[str]
     :ivar required_zone_names: Required private DNS zone names.
     :vartype required_zone_names: list[str]
     :ivar shareable_private_link_resource_types: The list of resources that are onboarded to
@@ -1399,20 +1440,22 @@
      list[~azure.mgmt.webpubsub.models.ShareablePrivateLinkResourceType]
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
         "type": {"readonly": True},
+        "system_data": {"readonly": True},
     }
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
+        "system_data": {"key": "systemData", "type": "SystemData"},
         "group_id": {"key": "properties.groupId", "type": "str"},
         "required_members": {"key": "properties.requiredMembers", "type": "[str]"},
         "required_zone_names": {"key": "properties.requiredZoneNames", "type": "[str]"},
         "shareable_private_link_resource_types": {
             "key": "properties.shareablePrivateLinkResourceTypes",
             "type": "[ShareablePrivateLinkResourceType]",
         },
@@ -1421,16 +1464,16 @@
     def __init__(
         self,
         *,
         group_id: Optional[str] = None,
         required_members: Optional[List[str]] = None,
         required_zone_names: Optional[List[str]] = None,
         shareable_private_link_resource_types: Optional[List["_models.ShareablePrivateLinkResourceType"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword group_id: Group Id of the private link resource.
         :paramtype group_id: str
         :keyword required_members: Required members of the private link resource.
         :paramtype required_members: list[str]
         :keyword required_zone_names: Required private DNS zone names.
         :paramtype required_zone_names: list[str]
@@ -1458,16 +1501,20 @@
 
     _attribute_map = {
         "value": {"key": "value", "type": "[PrivateLinkResource]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
     def __init__(
-        self, *, value: Optional[List["_models.PrivateLinkResource"]] = None, next_link: Optional[str] = None, **kwargs
-    ):
+        self,
+        *,
+        value: Optional[List["_models.PrivateLinkResource"]] = None,
+        next_link: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
         """
         :keyword value: List of PrivateLinkResource.
         :paramtype value: list[~azure.mgmt.webpubsub.models.PrivateLinkResource]
         :keyword next_link: The URL the client should use to fetch the next page (per server side
          paging).
          It's null for now, added for future use.
         :paramtype next_link: str
@@ -1498,16 +1545,16 @@
 
     def __init__(
         self,
         *,
         status: Optional[Union[str, "_models.PrivateLinkServiceConnectionStatus"]] = None,
         description: Optional[str] = None,
         actions_required: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword status: Indicates whether the connection has been Approved/Rejected/Removed by the
          owner of the service. Known values are: "Pending", "Approved", "Rejected", and "Disconnected".
         :paramtype status: str or ~azure.mgmt.webpubsub.models.PrivateLinkServiceConnectionStatus
         :keyword description: The reason for approval/rejection of the connection.
         :paramtype description: str
         :keyword actions_required: A message indicating if changes on the service provider require any
@@ -1527,24 +1574,179 @@
     :vartype key_type: str or ~azure.mgmt.webpubsub.models.KeyType
     """
 
     _attribute_map = {
         "key_type": {"key": "keyType", "type": "str"},
     }
 
-    def __init__(self, *, key_type: Optional[Union[str, "_models.KeyType"]] = None, **kwargs):
+    def __init__(self, *, key_type: Optional[Union[str, "_models.KeyType"]] = None, **kwargs: Any) -> None:
         """
         :keyword key_type: The type of access key. Known values are: "Primary", "Secondary", and
          "Salt".
         :paramtype key_type: str or ~azure.mgmt.webpubsub.models.KeyType
         """
         super().__init__(**kwargs)
         self.key_type = key_type
 
 
+class TrackedResource(Resource):
+    """The resource model definition for an Azure Resource Manager tracked top level resource which
+    has 'tags' and a 'location'.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    All required parameters must be populated in order to send to Azure.
+
+    :ivar id: Fully qualified resource ID for the resource. E.g.
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
+    :vartype id: str
+    :ivar name: The name of the resource.
+    :vartype name: str
+    :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
+     "Microsoft.Storage/storageAccounts".
+    :vartype type: str
+    :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
+     information.
+    :vartype system_data: ~azure.mgmt.webpubsub.models.SystemData
+    :ivar tags: Resource tags.
+    :vartype tags: dict[str, str]
+    :ivar location: The geo-location where the resource lives. Required.
+    :vartype location: str
+    """
+
+    _validation = {
+        "id": {"readonly": True},
+        "name": {"readonly": True},
+        "type": {"readonly": True},
+        "system_data": {"readonly": True},
+        "location": {"required": True},
+    }
+
+    _attribute_map = {
+        "id": {"key": "id", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "type": {"key": "type", "type": "str"},
+        "system_data": {"key": "systemData", "type": "SystemData"},
+        "tags": {"key": "tags", "type": "{str}"},
+        "location": {"key": "location", "type": "str"},
+    }
+
+    def __init__(self, *, location: str, tags: Optional[Dict[str, str]] = None, **kwargs: Any) -> None:
+        """
+        :keyword tags: Resource tags.
+        :paramtype tags: dict[str, str]
+        :keyword location: The geo-location where the resource lives. Required.
+        :paramtype location: str
+        """
+        super().__init__(**kwargs)
+        self.tags = tags
+        self.location = location
+
+
+class Replica(TrackedResource):
+    """A class represent a replica resource.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    All required parameters must be populated in order to send to Azure.
+
+    :ivar id: Fully qualified resource ID for the resource. E.g.
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
+    :vartype id: str
+    :ivar name: The name of the resource.
+    :vartype name: str
+    :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
+     "Microsoft.Storage/storageAccounts".
+    :vartype type: str
+    :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
+     information.
+    :vartype system_data: ~azure.mgmt.webpubsub.models.SystemData
+    :ivar tags: Resource tags.
+    :vartype tags: dict[str, str]
+    :ivar location: The geo-location where the resource lives. Required.
+    :vartype location: str
+    :ivar sku: The billing information of the resource.
+    :vartype sku: ~azure.mgmt.webpubsub.models.ResourceSku
+    :ivar provisioning_state: Provisioning state of the resource. Known values are: "Unknown",
+     "Succeeded", "Failed", "Canceled", "Running", "Creating", "Updating", "Deleting", and "Moving".
+    :vartype provisioning_state: str or ~azure.mgmt.webpubsub.models.ProvisioningState
+    """
+
+    _validation = {
+        "id": {"readonly": True},
+        "name": {"readonly": True},
+        "type": {"readonly": True},
+        "system_data": {"readonly": True},
+        "location": {"required": True},
+        "provisioning_state": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "id": {"key": "id", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "type": {"key": "type", "type": "str"},
+        "system_data": {"key": "systemData", "type": "SystemData"},
+        "tags": {"key": "tags", "type": "{str}"},
+        "location": {"key": "location", "type": "str"},
+        "sku": {"key": "sku", "type": "ResourceSku"},
+        "provisioning_state": {"key": "properties.provisioningState", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        location: str,
+        tags: Optional[Dict[str, str]] = None,
+        sku: Optional["_models.ResourceSku"] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword tags: Resource tags.
+        :paramtype tags: dict[str, str]
+        :keyword location: The geo-location where the resource lives. Required.
+        :paramtype location: str
+        :keyword sku: The billing information of the resource.
+        :paramtype sku: ~azure.mgmt.webpubsub.models.ResourceSku
+        """
+        super().__init__(tags=tags, location=location, **kwargs)
+        self.sku = sku
+        self.provisioning_state = None
+
+
+class ReplicaList(_serialization.Model):
+    """ReplicaList.
+
+    :ivar value: List of the replica.
+    :vartype value: list[~azure.mgmt.webpubsub.models.Replica]
+    :ivar next_link: The URL the client should use to fetch the next page (per server side paging).
+     It's null for now, added for future use.
+    :vartype next_link: str
+    """
+
+    _attribute_map = {
+        "value": {"key": "value", "type": "[Replica]"},
+        "next_link": {"key": "nextLink", "type": "str"},
+    }
+
+    def __init__(
+        self, *, value: Optional[List["_models.Replica"]] = None, next_link: Optional[str] = None, **kwargs: Any
+    ) -> None:
+        """
+        :keyword value: List of the replica.
+        :paramtype value: list[~azure.mgmt.webpubsub.models.Replica]
+        :keyword next_link: The URL the client should use to fetch the next page (per server side
+         paging).
+         It's null for now, added for future use.
+        :paramtype next_link: str
+        """
+        super().__init__(**kwargs)
+        self.value = value
+        self.next_link = next_link
+
+
 class ResourceLogCategory(_serialization.Model):
     """Resource log category configuration of a Microsoft.SignalRService resource.
 
     :ivar name: Gets or sets the resource log category's name.
      Available values: ConnectivityLogs, MessagingLogs.
      Case insensitive.
     :vartype name: str
@@ -1555,15 +1757,15 @@
     """
 
     _attribute_map = {
         "name": {"key": "name", "type": "str"},
         "enabled": {"key": "enabled", "type": "str"},
     }
 
-    def __init__(self, *, name: Optional[str] = None, enabled: Optional[str] = None, **kwargs):
+    def __init__(self, *, name: Optional[str] = None, enabled: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword name: Gets or sets the resource log category's name.
          Available values: ConnectivityLogs, MessagingLogs.
          Case insensitive.
         :paramtype name: str
         :keyword enabled: Indicates whether or the resource log category is enabled.
          Available values: true, false.
@@ -1582,15 +1784,15 @@
     :vartype categories: list[~azure.mgmt.webpubsub.models.ResourceLogCategory]
     """
 
     _attribute_map = {
         "categories": {"key": "categories", "type": "[ResourceLogCategory]"},
     }
 
-    def __init__(self, *, categories: Optional[List["_models.ResourceLogCategory"]] = None, **kwargs):
+    def __init__(self, *, categories: Optional[List["_models.ResourceLogCategory"]] = None, **kwargs: Any) -> None:
         """
         :keyword categories: Gets or sets the list of category configurations.
         :paramtype categories: list[~azure.mgmt.webpubsub.models.ResourceLogCategory]
         """
         super().__init__(**kwargs)
         self.categories = categories
 
@@ -1602,15 +1804,15 @@
     :vartype id: str
     """
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
     }
 
-    def __init__(self, *, id: Optional[str] = None, **kwargs):  # pylint: disable=redefined-builtin
+    def __init__(self, *, id: Optional[str] = None, **kwargs: Any) -> None:  # pylint: disable=redefined-builtin
         """
         :keyword id: Resource ID.
         :paramtype id: str
         """
         super().__init__(**kwargs)
         self.id = id
 
@@ -1660,16 +1862,16 @@
 
     def __init__(
         self,
         *,
         name: str,
         tier: Optional[Union[str, "_models.WebPubSubSkuTier"]] = None,
         capacity: Optional[int] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword name: The name of the SKU. Required.
 
          Allowed values: Standard_S1, Free_F1, Premium_P1. Required.
         :paramtype name: str
         :keyword tier: Optional tier of this particular SKU. 'Standard' or 'Free'.
 
@@ -1707,16 +1909,16 @@
     }
 
     def __init__(
         self,
         *,
         metric_specifications: Optional[List["_models.MetricSpecification"]] = None,
         log_specifications: Optional[List["_models.LogSpecification"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword metric_specifications: Specifications of the Metrics for Azure Monitoring.
         :paramtype metric_specifications: list[~azure.mgmt.webpubsub.models.MetricSpecification]
         :keyword log_specifications: Specifications of the Logs for Azure Monitoring.
         :paramtype log_specifications: list[~azure.mgmt.webpubsub.models.LogSpecification]
         """
         super().__init__(**kwargs)
@@ -1741,16 +1943,21 @@
     _attribute_map = {
         "description": {"key": "description", "type": "str"},
         "group_id": {"key": "groupId", "type": "str"},
         "type": {"key": "type", "type": "str"},
     }
 
     def __init__(
-        self, *, description: Optional[str] = None, group_id: Optional[str] = None, type: Optional[str] = None, **kwargs
-    ):
+        self,
+        *,
+        description: Optional[str] = None,
+        group_id: Optional[str] = None,
+        type: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
         """
         :keyword description: The description of the resource type that has been onboarded to private
          link service.
         :paramtype description: str
         :keyword group_id: The resource provider group id for the resource that has been onboarded to
          private link service.
         :paramtype group_id: str
@@ -1780,16 +1987,16 @@
     }
 
     def __init__(
         self,
         *,
         name: Optional[str] = None,
         properties: Optional["_models.ShareablePrivateLinkResourceProperties"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword name: The name of the resource type that has been onboarded to private link service.
         :paramtype name: str
         :keyword properties: Describes the properties of a resource type that has been onboarded to
          private link service.
         :paramtype properties: ~azure.mgmt.webpubsub.models.ShareablePrivateLinkResourceProperties
         """
@@ -1799,21 +2006,24 @@
 
 
 class SharedPrivateLinkResource(ProxyResource):
     """Describes a Shared Private Link Resource.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    :ivar id: Fully qualified resource Id for the resource.
+    :ivar id: Fully qualified resource ID for the resource. E.g.
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
-    :ivar type: The type of the resource - e.g. "Microsoft.SignalRService/SignalR".
+    :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
+     "Microsoft.Storage/storageAccounts".
     :vartype type: str
-    :ivar system_data: Metadata pertaining to creation and last modification of the resource.
+    :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
+     information.
     :vartype system_data: ~azure.mgmt.webpubsub.models.SystemData
     :ivar group_id: The group id from the provider of resource the shared private link resource is
      for.
     :vartype group_id: str
     :ivar private_link_resource_id: The resource id of the resource the shared private link
      resource is for.
     :vartype private_link_resource_id: str
@@ -1851,29 +2061,28 @@
 
     def __init__(
         self,
         *,
         group_id: Optional[str] = None,
         private_link_resource_id: Optional[str] = None,
         request_message: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword group_id: The group id from the provider of resource the shared private link resource
          is for.
         :paramtype group_id: str
         :keyword private_link_resource_id: The resource id of the resource the shared private link
          resource is for.
         :paramtype private_link_resource_id: str
         :keyword request_message: The request message for requesting approval of the shared private
          link resource.
         :paramtype request_message: str
         """
         super().__init__(**kwargs)
-        self.system_data = None
         self.group_id = group_id
         self.private_link_resource_id = private_link_resource_id
         self.provisioning_state = None
         self.request_message = request_message
         self.status = None
 
 
@@ -1894,16 +2103,16 @@
     }
 
     def __init__(
         self,
         *,
         value: Optional[List["_models.SharedPrivateLinkResource"]] = None,
         next_link: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword value: The list of the shared private link resources.
         :paramtype value: list[~azure.mgmt.webpubsub.models.SharedPrivateLinkResource]
         :keyword next_link: Request URL that can be used to query next page of private endpoint
          connections. Returned when the total number of requested private endpoint connections exceed
          maximum page size.
         :paramtype next_link: str
@@ -1942,16 +2151,16 @@
         self,
         *,
         id: Optional[str] = None,  # pylint: disable=redefined-builtin
         current_value: Optional[int] = None,
         limit: Optional[int] = None,
         name: Optional["_models.SignalRServiceUsageName"] = None,
         unit: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword id: Fully qualified ARM resource id.
         :paramtype id: str
         :keyword current_value: Current value for the usage quota.
         :paramtype current_value: int
         :keyword limit: The maximum permitted value for the usage quota. If there is no limit, this
          value will be -1.
@@ -1982,16 +2191,20 @@
 
     _attribute_map = {
         "value": {"key": "value", "type": "[SignalRServiceUsage]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
     def __init__(
-        self, *, value: Optional[List["_models.SignalRServiceUsage"]] = None, next_link: Optional[str] = None, **kwargs
-    ):
+        self,
+        *,
+        value: Optional[List["_models.SignalRServiceUsage"]] = None,
+        next_link: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
         """
         :keyword value: List of the resource usages.
         :paramtype value: list[~azure.mgmt.webpubsub.models.SignalRServiceUsage]
         :keyword next_link: The URL the client should use to fetch the next page (per server side
          paging).
          It's null for now, added for future use.
         :paramtype next_link: str
@@ -2011,15 +2224,15 @@
     """
 
     _attribute_map = {
         "value": {"key": "value", "type": "str"},
         "localized_value": {"key": "localizedValue", "type": "str"},
     }
 
-    def __init__(self, *, value: Optional[str] = None, localized_value: Optional[str] = None, **kwargs):
+    def __init__(self, *, value: Optional[str] = None, localized_value: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword value: The identifier of the usage.
         :paramtype value: str
         :keyword localized_value: Localized name of the usage.
         :paramtype localized_value: str
         """
         super().__init__(**kwargs)
@@ -2048,15 +2261,15 @@
 
     _attribute_map = {
         "resource_type": {"key": "resourceType", "type": "str"},
         "sku": {"key": "sku", "type": "ResourceSku"},
         "capacity": {"key": "capacity", "type": "SkuCapacity"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.resource_type = None
         self.sku = None
         self.capacity = None
 
 
@@ -2090,15 +2303,15 @@
         "minimum": {"key": "minimum", "type": "int"},
         "maximum": {"key": "maximum", "type": "int"},
         "default": {"key": "default", "type": "int"},
         "allowed_values": {"key": "allowedValues", "type": "[int]"},
         "scale_type": {"key": "scaleType", "type": "str"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.minimum = None
         self.maximum = None
         self.default = None
         self.allowed_values = None
         self.scale_type = None
@@ -2122,15 +2335,15 @@
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[Sku]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.value = None
         self.next_link = None
 
 
 class SystemData(_serialization.Model):
@@ -2166,16 +2379,16 @@
         *,
         created_by: Optional[str] = None,
         created_by_type: Optional[Union[str, "_models.CreatedByType"]] = None,
         created_at: Optional[datetime.datetime] = None,
         last_modified_by: Optional[str] = None,
         last_modified_by_type: Optional[Union[str, "_models.CreatedByType"]] = None,
         last_modified_at: Optional[datetime.datetime] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword created_by: The identity that created the resource.
         :paramtype created_by: str
         :keyword created_by_type: The type of identity that created the resource. Known values are:
          "User", "Application", "ManagedIdentity", and "Key".
         :paramtype created_by_type: str or ~azure.mgmt.webpubsub.models.CreatedByType
         :keyword created_at: The timestamp of resource creation (UTC).
@@ -2193,60 +2406,14 @@
         self.created_by_type = created_by_type
         self.created_at = created_at
         self.last_modified_by = last_modified_by
         self.last_modified_by_type = last_modified_by_type
         self.last_modified_at = last_modified_at
 
 
-class TrackedResource(Resource):
-    """The resource model definition for a ARM tracked top level resource.
-
-    Variables are only populated by the server, and will be ignored when sending a request.
-
-    :ivar id: Fully qualified resource Id for the resource.
-    :vartype id: str
-    :ivar name: The name of the resource.
-    :vartype name: str
-    :ivar type: The type of the resource - e.g. "Microsoft.SignalRService/SignalR".
-    :vartype type: str
-    :ivar location: The GEO location of the resource. e.g. West US | East US | North Central US |
-     South Central US.
-    :vartype location: str
-    :ivar tags: Tags of the service which is a list of key value pairs that describe the resource.
-    :vartype tags: dict[str, str]
-    """
-
-    _validation = {
-        "id": {"readonly": True},
-        "name": {"readonly": True},
-        "type": {"readonly": True},
-    }
-
-    _attribute_map = {
-        "id": {"key": "id", "type": "str"},
-        "name": {"key": "name", "type": "str"},
-        "type": {"key": "type", "type": "str"},
-        "location": {"key": "location", "type": "str"},
-        "tags": {"key": "tags", "type": "{str}"},
-    }
-
-    def __init__(self, *, location: Optional[str] = None, tags: Optional[Dict[str, str]] = None, **kwargs):
-        """
-        :keyword location: The GEO location of the resource. e.g. West US | East US | North Central US
-         | South Central US.
-        :paramtype location: str
-        :keyword tags: Tags of the service which is a list of key value pairs that describe the
-         resource.
-        :paramtype tags: dict[str, str]
-        """
-        super().__init__(**kwargs)
-        self.location = location
-        self.tags = tags
-
-
 class UpstreamAuthSettings(_serialization.Model):
     """Upstream auth settings. If not set, no auth is used for upstream messages.
 
     :ivar type: Upstream auth type enum. Known values are: "None" and "ManagedIdentity".
     :vartype type: str or ~azure.mgmt.webpubsub.models.UpstreamAuthType
     :ivar managed_identity: Managed identity settings for upstream.
     :vartype managed_identity: ~azure.mgmt.webpubsub.models.ManagedIdentitySettings
@@ -2258,16 +2425,16 @@
     }
 
     def __init__(
         self,
         *,
         type: Optional[Union[str, "_models.UpstreamAuthType"]] = None,
         managed_identity: Optional["_models.ManagedIdentitySettings"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword type: Upstream auth type enum. Known values are: "None" and "ManagedIdentity".
         :paramtype type: str or ~azure.mgmt.webpubsub.models.UpstreamAuthType
         :keyword managed_identity: Managed identity settings for upstream.
         :paramtype managed_identity: ~azure.mgmt.webpubsub.models.ManagedIdentitySettings
         """
         super().__init__(**kwargs)
@@ -2292,35 +2459,38 @@
     }
 
     _attribute_map = {
         "principal_id": {"key": "principalId", "type": "str"},
         "client_id": {"key": "clientId", "type": "str"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.principal_id = None
         self.client_id = None
 
 
 class WebPubSubHub(ProxyResource):
     """A hub setting.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     All required parameters must be populated in order to send to Azure.
 
-    :ivar id: Fully qualified resource Id for the resource.
+    :ivar id: Fully qualified resource ID for the resource. E.g.
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
-    :ivar type: The type of the resource - e.g. "Microsoft.SignalRService/SignalR".
+    :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
+     "Microsoft.Storage/storageAccounts".
     :vartype type: str
-    :ivar system_data: Metadata pertaining to creation and last modification of the resource.
+    :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
+     information.
     :vartype system_data: ~azure.mgmt.webpubsub.models.SystemData
     :ivar properties: Properties of a hub. Required.
     :vartype properties: ~azure.mgmt.webpubsub.models.WebPubSubHubProperties
     """
 
     _validation = {
         "id": {"readonly": True},
@@ -2334,21 +2504,20 @@
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
         "properties": {"key": "properties", "type": "WebPubSubHubProperties"},
     }
 
-    def __init__(self, *, properties: "_models.WebPubSubHubProperties", **kwargs):
+    def __init__(self, *, properties: "_models.WebPubSubHubProperties", **kwargs: Any) -> None:
         """
         :keyword properties: Properties of a hub. Required.
         :paramtype properties: ~azure.mgmt.webpubsub.models.WebPubSubHubProperties
         """
         super().__init__(**kwargs)
-        self.system_data = None
         self.properties = properties
 
 
 class WebPubSubHubList(_serialization.Model):
     """Hub setting list.
 
     Variables are only populated by the server, and will be ignored when sending a request.
@@ -2365,15 +2534,15 @@
     }
 
     _attribute_map = {
         "value": {"key": "value", "type": "[WebPubSubHub]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, value: Optional[List["_models.WebPubSubHub"]] = None, **kwargs):
+    def __init__(self, *, value: Optional[List["_models.WebPubSubHub"]] = None, **kwargs: Any) -> None:
         """
         :keyword value: List of hub settings to this resource.
         :paramtype value: list[~azure.mgmt.webpubsub.models.WebPubSubHub]
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = None
@@ -2404,16 +2573,16 @@
 
     def __init__(
         self,
         *,
         event_handlers: Optional[List["_models.EventHandler"]] = None,
         event_listeners: Optional[List["_models.EventListener"]] = None,
         anonymous_connect_policy: str = "deny",
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword event_handlers: Event handler of a hub.
         :paramtype event_handlers: list[~azure.mgmt.webpubsub.models.EventHandler]
         :keyword event_listeners: Event listener settings for forwarding your client events to
          listeners.
          Event listener is transparent to Web PubSub clients, and it doesn't return any result to
          clients nor interrupt the lifetime of clients.
@@ -2454,16 +2623,16 @@
     def __init__(
         self,
         *,
         primary_key: Optional[str] = None,
         secondary_key: Optional[str] = None,
         primary_connection_string: Optional[str] = None,
         secondary_connection_string: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword primary_key: The primary access key.
         :paramtype primary_key: str
         :keyword secondary_key: The secondary access key.
         :paramtype secondary_key: str
         :keyword primary_connection_string: Connection string constructed via the primaryKey.
         :paramtype primary_connection_string: str
@@ -2496,16 +2665,16 @@
 
     def __init__(
         self,
         *,
         default_action: Optional[Union[str, "_models.ACLAction"]] = None,
         public_network: Optional["_models.NetworkACL"] = None,
         private_endpoints: Optional[List["_models.PrivateEndpointACL"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword default_action: Azure Networking ACL Action. Known values are: "Allow" and "Deny".
         :paramtype default_action: str or ~azure.mgmt.webpubsub.models.ACLAction
         :keyword public_network: Network ACL.
         :paramtype public_network: ~azure.mgmt.webpubsub.models.NetworkACL
         :keyword private_endpoints: ACLs for requests from private endpoints.
         :paramtype private_endpoints: list[~azure.mgmt.webpubsub.models.PrivateEndpointACL]
@@ -2517,31 +2686,37 @@
 
 
 class WebPubSubResource(TrackedResource):  # pylint: disable=too-many-instance-attributes
     """A class represent a resource.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    :ivar id: Fully qualified resource Id for the resource.
+    All required parameters must be populated in order to send to Azure.
+
+    :ivar id: Fully qualified resource ID for the resource. E.g.
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
-    :ivar type: The type of the resource - e.g. "Microsoft.SignalRService/SignalR".
+    :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
+     "Microsoft.Storage/storageAccounts".
     :vartype type: str
-    :ivar location: The GEO location of the resource. e.g. West US | East US | North Central US |
-     South Central US.
-    :vartype location: str
-    :ivar tags: Tags of the service which is a list of key value pairs that describe the resource.
+    :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
+     information.
+    :vartype system_data: ~azure.mgmt.webpubsub.models.SystemData
+    :ivar tags: Resource tags.
     :vartype tags: dict[str, str]
+    :ivar location: The geo-location where the resource lives. Required.
+    :vartype location: str
     :ivar sku: The billing information of the resource.
     :vartype sku: ~azure.mgmt.webpubsub.models.ResourceSku
+    :ivar kind: The kind of the service. Known values are: "WebPubSub" and "SocketIO".
+    :vartype kind: str or ~azure.mgmt.webpubsub.models.ServiceKind
     :ivar identity: A class represent managed identities used for request and response.
     :vartype identity: ~azure.mgmt.webpubsub.models.ManagedIdentity
-    :ivar system_data: Metadata pertaining to creation and last modification of the resource.
-    :vartype system_data: ~azure.mgmt.webpubsub.models.SystemData
     :ivar provisioning_state: Provisioning state of the resource. Known values are: "Unknown",
      "Succeeded", "Failed", "Canceled", "Running", "Creating", "Updating", "Deleting", and "Moving".
     :vartype provisioning_state: str or ~azure.mgmt.webpubsub.models.ProvisioningState
     :ivar external_ip: The publicly accessible IP of the resource.
     :vartype external_ip: str
     :ivar host_name: FQDN of the service instance.
     :vartype host_name: str
@@ -2588,14 +2763,15 @@
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
         "type": {"readonly": True},
         "system_data": {"readonly": True},
+        "location": {"required": True},
         "provisioning_state": {"readonly": True},
         "external_ip": {"readonly": True},
         "host_name": {"readonly": True},
         "public_port": {"readonly": True},
         "server_port": {"readonly": True},
         "version": {"readonly": True},
         "private_endpoint_connections": {"readonly": True},
@@ -2603,19 +2779,20 @@
         "host_name_prefix": {"readonly": True},
     }
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
-        "location": {"key": "location", "type": "str"},
+        "system_data": {"key": "systemData", "type": "SystemData"},
         "tags": {"key": "tags", "type": "{str}"},
+        "location": {"key": "location", "type": "str"},
         "sku": {"key": "sku", "type": "ResourceSku"},
+        "kind": {"key": "kind", "type": "str"},
         "identity": {"key": "identity", "type": "ManagedIdentity"},
-        "system_data": {"key": "systemData", "type": "SystemData"},
         "provisioning_state": {"key": "properties.provisioningState", "type": "str"},
         "external_ip": {"key": "properties.externalIP", "type": "str"},
         "host_name": {"key": "properties.hostName", "type": "str"},
         "public_port": {"key": "properties.publicPort", "type": "int"},
         "server_port": {"key": "properties.serverPort", "type": "int"},
         "version": {"key": "properties.version", "type": "str"},
         "private_endpoint_connections": {
@@ -2638,36 +2815,37 @@
         "disable_local_auth": {"key": "properties.disableLocalAuth", "type": "bool"},
         "disable_aad_auth": {"key": "properties.disableAadAuth", "type": "bool"},
     }
 
     def __init__(  # pylint: disable=too-many-locals
         self,
         *,
-        location: Optional[str] = None,
+        location: str,
         tags: Optional[Dict[str, str]] = None,
         sku: Optional["_models.ResourceSku"] = None,
+        kind: Optional[Union[str, "_models.ServiceKind"]] = None,
         identity: Optional["_models.ManagedIdentity"] = None,
         tls: Optional["_models.WebPubSubTlsSettings"] = None,
         live_trace_configuration: Optional["_models.LiveTraceConfiguration"] = None,
         resource_log_configuration: Optional["_models.ResourceLogConfiguration"] = None,
         network_ac_ls: Optional["_models.WebPubSubNetworkACLs"] = None,
         public_network_access: str = "Enabled",
         disable_local_auth: bool = False,
         disable_aad_auth: bool = False,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
-        :keyword location: The GEO location of the resource. e.g. West US | East US | North Central US
-         | South Central US.
-        :paramtype location: str
-        :keyword tags: Tags of the service which is a list of key value pairs that describe the
-         resource.
+        :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
+        :keyword location: The geo-location where the resource lives. Required.
+        :paramtype location: str
         :keyword sku: The billing information of the resource.
         :paramtype sku: ~azure.mgmt.webpubsub.models.ResourceSku
+        :keyword kind: The kind of the service. Known values are: "WebPubSub" and "SocketIO".
+        :paramtype kind: str or ~azure.mgmt.webpubsub.models.ServiceKind
         :keyword identity: A class represent managed identities used for request and response.
         :paramtype identity: ~azure.mgmt.webpubsub.models.ManagedIdentity
         :keyword tls: TLS settings for the resource.
         :paramtype tls: ~azure.mgmt.webpubsub.models.WebPubSubTlsSettings
         :keyword live_trace_configuration: Live trace configuration of a Microsoft.SignalRService
          resource.
         :paramtype live_trace_configuration: ~azure.mgmt.webpubsub.models.LiveTraceConfiguration
@@ -2686,18 +2864,18 @@
          When set as true, connection with AccessKey=xxx won't work.
         :paramtype disable_local_auth: bool
         :keyword disable_aad_auth: DisableLocalAuth
          Enable or disable aad auth
          When set as true, connection with AuthType=aad won't work.
         :paramtype disable_aad_auth: bool
         """
-        super().__init__(location=location, tags=tags, **kwargs)
+        super().__init__(tags=tags, location=location, **kwargs)
         self.sku = sku
+        self.kind = kind
         self.identity = identity
-        self.system_data = None
         self.provisioning_state = None
         self.external_ip = None
         self.host_name = None
         self.public_port = None
         self.server_port = None
         self.version = None
         self.private_endpoint_connections = None
@@ -2724,16 +2902,20 @@
 
     _attribute_map = {
         "value": {"key": "value", "type": "[WebPubSubResource]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
     def __init__(
-        self, *, value: Optional[List["_models.WebPubSubResource"]] = None, next_link: Optional[str] = None, **kwargs
-    ):
+        self,
+        *,
+        value: Optional[List["_models.WebPubSubResource"]] = None,
+        next_link: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
         """
         :keyword value: List of the resources.
         :paramtype value: list[~azure.mgmt.webpubsub.models.WebPubSubResource]
         :keyword next_link: The URL the client should use to fetch the next page (per server side
          paging).
          It's null for now, added for future use.
         :paramtype next_link: str
@@ -2742,22 +2924,24 @@
         self.value = value
         self.next_link = next_link
 
 
 class WebPubSubTlsSettings(_serialization.Model):
     """TLS settings for the resource.
 
-    :ivar client_cert_enabled: Request client certificate during TLS handshake if enabled.
+    :ivar client_cert_enabled: Request client certificate during TLS handshake if enabled. Not
+     supported for free tier. Any input will be ignored for free tier.
     :vartype client_cert_enabled: bool
     """
 
     _attribute_map = {
         "client_cert_enabled": {"key": "clientCertEnabled", "type": "bool"},
     }
 
-    def __init__(self, *, client_cert_enabled: bool = True, **kwargs):
+    def __init__(self, *, client_cert_enabled: bool = False, **kwargs: Any) -> None:
         """
-        :keyword client_cert_enabled: Request client certificate during TLS handshake if enabled.
+        :keyword client_cert_enabled: Request client certificate during TLS handshake if enabled. Not
+         supported for free tier. Any input will be ignored for free tier.
         :paramtype client_cert_enabled: bool
         """
         super().__init__(**kwargs)
         self.client_cert_enabled = client_cert_enabled
```

## Comparing `azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/__init__.py` & `azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,18 +3,21 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._web_pub_sub_management_client import WebPubSubManagementClient
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
 
 __all__ = [
     "WebPubSubManagementClient",
 ]
```

## Comparing `azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/_configuration.py` & `azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/_configuration.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,52 +2,45 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-import sys
 from typing import Any, TYPE_CHECKING
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
 from azure.mgmt.core.policies import ARMHttpLoggingPolicy, AsyncARMChallengeAuthenticationPolicy
 
 from .._version import VERSION
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
-
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials_async import AsyncTokenCredential
 
 
 class WebPubSubManagementClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
     """Configuration for WebPubSubManagementClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
-    :param subscription_id: Gets subscription Id which uniquely identify the Microsoft Azure
-     subscription. The subscription ID forms part of the URI for every service call. Required.
+    :param subscription_id: The ID of the target subscription. The value must be an UUID. Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2022-08-01-preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2023-06-01-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, credential: "AsyncTokenCredential", subscription_id: str, **kwargs: Any) -> None:
         super(WebPubSubManagementClientConfiguration, self).__init__(**kwargs)
-        api_version = kwargs.pop("api_version", "2022-08-01-preview")  # type: Literal["2022-08-01-preview"]
+        api_version: str = kwargs.pop("api_version", "2023-06-01-preview")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
```

## Comparing `azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/_patch.py` & `azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/_web_pub_sub_management_client.py` & `azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/_web_pub_sub_management_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,26 +8,27 @@
 
 from copy import deepcopy
 from typing import Any, Awaitable, TYPE_CHECKING
 
 from azure.core.rest import AsyncHttpResponse, HttpRequest
 from azure.mgmt.core import AsyncARMPipelineClient
 
-from .. import models
+from .. import models as _models
 from .._serialization import Deserializer, Serializer
 from ._configuration import WebPubSubManagementClientConfiguration
 from .operations import (
     Operations,
     UsagesOperations,
     WebPubSubCustomCertificatesOperations,
     WebPubSubCustomDomainsOperations,
     WebPubSubHubsOperations,
     WebPubSubOperations,
     WebPubSubPrivateEndpointConnectionsOperations,
     WebPubSubPrivateLinkResourcesOperations,
+    WebPubSubReplicasOperations,
     WebPubSubSharedPrivateLinkResourcesOperations,
 )
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials_async import AsyncTokenCredential
 
@@ -52,26 +53,27 @@
     :ivar web_pub_sub_private_endpoint_connections: WebPubSubPrivateEndpointConnectionsOperations
      operations
     :vartype web_pub_sub_private_endpoint_connections:
      azure.mgmt.webpubsub.aio.operations.WebPubSubPrivateEndpointConnectionsOperations
     :ivar web_pub_sub_private_link_resources: WebPubSubPrivateLinkResourcesOperations operations
     :vartype web_pub_sub_private_link_resources:
      azure.mgmt.webpubsub.aio.operations.WebPubSubPrivateLinkResourcesOperations
+    :ivar web_pub_sub_replicas: WebPubSubReplicasOperations operations
+    :vartype web_pub_sub_replicas: azure.mgmt.webpubsub.aio.operations.WebPubSubReplicasOperations
     :ivar web_pub_sub_shared_private_link_resources: WebPubSubSharedPrivateLinkResourcesOperations
      operations
     :vartype web_pub_sub_shared_private_link_resources:
      azure.mgmt.webpubsub.aio.operations.WebPubSubSharedPrivateLinkResourcesOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
-    :param subscription_id: Gets subscription Id which uniquely identify the Microsoft Azure
-     subscription. The subscription ID forms part of the URI for every service call. Required.
+    :param subscription_id: The ID of the target subscription. The value must be an UUID. Required.
     :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
-    :keyword api_version: Api Version. Default value is "2022-08-01-preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2023-06-01-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(
@@ -80,17 +82,17 @@
         subscription_id: str,
         base_url: str = "https://management.azure.com",
         **kwargs: Any
     ) -> None:
         self._config = WebPubSubManagementClientConfiguration(
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
         self.web_pub_sub = WebPubSubOperations(self._client, self._config, self._serialize, self._deserialize)
         self.usages = UsagesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.web_pub_sub_custom_certificates = WebPubSubCustomCertificatesOperations(
@@ -102,14 +104,17 @@
         self.web_pub_sub_hubs = WebPubSubHubsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.web_pub_sub_private_endpoint_connections = WebPubSubPrivateEndpointConnectionsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.web_pub_sub_private_link_resources = WebPubSubPrivateLinkResourcesOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
+        self.web_pub_sub_replicas = WebPubSubReplicasOperations(
+            self._client, self._config, self._serialize, self._deserialize
+        )
         self.web_pub_sub_shared_private_link_resources = WebPubSubSharedPrivateLinkResourcesOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
 
     def _send_request(self, request: HttpRequest, **kwargs: Any) -> Awaitable[AsyncHttpResponse]:
         """Runs the network request through the client's chained policies.
 
@@ -135,9 +140,9 @@
     async def close(self) -> None:
         await self._client.close()
 
     async def __aenter__(self) -> "WebPubSubManagementClient":
         await self._client.__aenter__()
         return self
 
-    async def __aexit__(self, *exc_details) -> None:
+    async def __aexit__(self, *exc_details: Any) -> None:
         await self._client.__aexit__(*exc_details)
```

## Comparing `azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/operations/__init__.py` & `azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/operations/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,26 +10,28 @@
 from ._web_pub_sub_operations import WebPubSubOperations
 from ._usages_operations import UsagesOperations
 from ._web_pub_sub_custom_certificates_operations import WebPubSubCustomCertificatesOperations
 from ._web_pub_sub_custom_domains_operations import WebPubSubCustomDomainsOperations
 from ._web_pub_sub_hubs_operations import WebPubSubHubsOperations
 from ._web_pub_sub_private_endpoint_connections_operations import WebPubSubPrivateEndpointConnectionsOperations
 from ._web_pub_sub_private_link_resources_operations import WebPubSubPrivateLinkResourcesOperations
+from ._web_pub_sub_replicas_operations import WebPubSubReplicasOperations
 from ._web_pub_sub_shared_private_link_resources_operations import WebPubSubSharedPrivateLinkResourcesOperations
 
 from ._patch import __all__ as _patch_all
-from ._patch import *  # type: ignore # pylint: disable=unused-wildcard-import
+from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "Operations",
     "WebPubSubOperations",
     "UsagesOperations",
     "WebPubSubCustomCertificatesOperations",
     "WebPubSubCustomDomainsOperations",
     "WebPubSubHubsOperations",
     "WebPubSubPrivateEndpointConnectionsOperations",
     "WebPubSubPrivateLinkResourcesOperations",
+    "WebPubSubReplicasOperations",
     "WebPubSubSharedPrivateLinkResourcesOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

## Comparing `azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_private_link_resources_operations.py` & `azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_private_link_resources_operations.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, AsyncIterable, Callable, Dict, Optional, TypeVar
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -26,18 +25,14 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._web_pub_sub_private_link_resources_operations import build_list_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class WebPubSubPrivateLinkResourcesOperations:
     """
     .. warning::
@@ -59,32 +54,30 @@
 
     @distributed_trace
     def list(
         self, resource_group_name: str, resource_name: str, **kwargs: Any
     ) -> AsyncIterable["_models.PrivateLinkResource"]:
         """Get the private link resources that need to be created for a resource.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either PrivateLinkResource or the result of cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.webpubsub.models.PrivateLinkResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.PrivateLinkResourceList]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.PrivateLinkResourceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -99,15 +92,15 @@
                     subscription_id=self._config.subscription_id,
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
@@ -115,36 +108,39 @@
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
             deserialized = self._deserialize("PrivateLinkResourceList", pipeline_response)
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
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/privateLinkResources"}  # type: ignore
+    list.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/privateLinkResources"
+    }
```

## Comparing `azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_custom_domains_operations.py` & `azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_hubs_operations.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -27,71 +27,65 @@
 from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.async_arm_polling import AsyncARMPolling
 
 from ... import models as _models
 from ..._vendor import _convert_request
-from ...operations._web_pub_sub_custom_domains_operations import (
+from ...operations._web_pub_sub_hubs_operations import (
     build_create_or_update_request,
     build_delete_request,
     build_get_request,
     build_list_request,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
-class WebPubSubCustomDomainsOperations:
+class WebPubSubHubsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.webpubsub.aio.WebPubSubManagementClient`'s
-        :attr:`web_pub_sub_custom_domains` attribute.
+        :attr:`web_pub_sub_hubs` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
     def list(
         self, resource_group_name: str, resource_name: str, **kwargs: Any
-    ) -> AsyncIterable["_models.CustomDomain"]:
-        """List all custom domains.
+    ) -> AsyncIterable["_models.WebPubSubHub"]:
+        """List hub settings.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either CustomDomain or the result of cls(response)
-        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.webpubsub.models.CustomDomain]
+        :return: An iterator like instance of either WebPubSubHub or the result of cls(response)
+        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.webpubsub.models.WebPubSubHub]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.CustomDomainList]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.WebPubSubHubList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -106,15 +100,15 @@
                     subscription_id=self._config.subscription_id,
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
@@ -122,402 +116,418 @@
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
-            deserialized = self._deserialize("CustomDomainList", pipeline_response)
+            deserialized = self._deserialize("WebPubSubHubList", pipeline_response)
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
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customDomains"}  # type: ignore
+    list.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/hubs"
+    }
 
     @distributed_trace_async
-    async def get(self, resource_group_name: str, resource_name: str, name: str, **kwargs: Any) -> _models.CustomDomain:
-        """Get a custom domain.
-
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+    async def get(
+        self, hub_name: str, resource_group_name: str, resource_name: str, **kwargs: Any
+    ) -> _models.WebPubSubHub:
+        """Get a hub setting.
+
+        :param hub_name: The hub name. Required.
+        :type hub_name: str
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
-        :param name: Custom domain name. Required.
-        :type name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: CustomDomain or the result of cls(response)
-        :rtype: ~azure.mgmt.webpubsub.models.CustomDomain
+        :return: WebPubSubHub or the result of cls(response)
+        :rtype: ~azure.mgmt.webpubsub.models.WebPubSubHub
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.CustomDomain]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.WebPubSubHub] = kwargs.pop("cls", None)
 
         request = build_get_request(
+            hub_name=hub_name,
             resource_group_name=resource_group_name,
             resource_name=resource_name,
-            name=name,
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize("CustomDomain", pipeline_response)
+        deserialized = self._deserialize("WebPubSubHub", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    get.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customDomains/{name}"}  # type: ignore
+    get.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/hubs/{hubName}"
+    }
 
     async def _create_or_update_initial(
         self,
+        hub_name: str,
         resource_group_name: str,
         resource_name: str,
-        name: str,
-        parameters: Union[_models.CustomDomain, IO],
+        parameters: Union[_models.WebPubSubHub, IO],
         **kwargs: Any
-    ) -> _models.CustomDomain:
+    ) -> _models.WebPubSubHub:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.CustomDomain]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.WebPubSubHub] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
-            _json = self._serialize.body(parameters, "CustomDomain")
+            _json = self._serialize.body(parameters, "WebPubSubHub")
 
         request = build_create_or_update_request(
+            hub_name=hub_name,
             resource_group_name=resource_group_name,
             resource_name=resource_name,
-            name=name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
             template_url=self._create_or_update_initial.metadata["url"],
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
 
-        if response.status_code not in [201]:
+        if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize("CustomDomain", pipeline_response)
+        if response.status_code == 200:
+            deserialized = self._deserialize("WebPubSubHub", pipeline_response)
+
+        if response.status_code == 201:
+            deserialized = self._deserialize("WebPubSubHub", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
+        return deserialized  # type: ignore
 
-    _create_or_update_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customDomains/{name}"}  # type: ignore
+    _create_or_update_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/hubs/{hubName}"
+    }
 
     @overload
     async def begin_create_or_update(
         self,
+        hub_name: str,
         resource_group_name: str,
         resource_name: str,
-        name: str,
-        parameters: _models.CustomDomain,
+        parameters: _models.WebPubSubHub,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.CustomDomain]:
-        """Create or update a custom domain.
+    ) -> AsyncLROPoller[_models.WebPubSubHub]:
+        """Create or update a hub setting.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param hub_name: The hub name. Required.
+        :type hub_name: str
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
-        :param name: Custom domain name. Required.
-        :type name: str
-        :param parameters: Required.
-        :type parameters: ~azure.mgmt.webpubsub.models.CustomDomain
+        :param parameters: The resource of WebPubSubHub and its properties. Required.
+        :type parameters: ~azure.mgmt.webpubsub.models.WebPubSubHub
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either CustomDomain or the result of
+        :return: An instance of AsyncLROPoller that returns either WebPubSubHub or the result of
          cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.webpubsub.models.CustomDomain]
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.webpubsub.models.WebPubSubHub]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_create_or_update(
         self,
+        hub_name: str,
         resource_group_name: str,
         resource_name: str,
-        name: str,
         parameters: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.CustomDomain]:
-        """Create or update a custom domain.
+    ) -> AsyncLROPoller[_models.WebPubSubHub]:
+        """Create or update a hub setting.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param hub_name: The hub name. Required.
+        :type hub_name: str
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
-        :param name: Custom domain name. Required.
-        :type name: str
-        :param parameters: Required.
+        :param parameters: The resource of WebPubSubHub and its properties. Required.
         :type parameters: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
-         Known values are: 'application/json', 'text/json'. Default value is "application/json".
+         Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either CustomDomain or the result of
+        :return: An instance of AsyncLROPoller that returns either WebPubSubHub or the result of
          cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.webpubsub.models.CustomDomain]
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.webpubsub.models.WebPubSubHub]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_create_or_update(
         self,
+        hub_name: str,
         resource_group_name: str,
         resource_name: str,
-        name: str,
-        parameters: Union[_models.CustomDomain, IO],
+        parameters: Union[_models.WebPubSubHub, IO],
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.CustomDomain]:
-        """Create or update a custom domain.
+    ) -> AsyncLROPoller[_models.WebPubSubHub]:
+        """Create or update a hub setting.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param hub_name: The hub name. Required.
+        :type hub_name: str
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
-        :param name: Custom domain name. Required.
-        :type name: str
-        :param parameters: Is either a model type or a IO type. Required.
-        :type parameters: ~azure.mgmt.webpubsub.models.CustomDomain or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json',
-         'text/json'. Default value is None.
+        :param parameters: The resource of WebPubSubHub and its properties. Is either a WebPubSubHub
+         type or a IO type. Required.
+        :type parameters: ~azure.mgmt.webpubsub.models.WebPubSubHub or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
+         Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either CustomDomain or the result of
+        :return: An instance of AsyncLROPoller that returns either WebPubSubHub or the result of
          cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.webpubsub.models.CustomDomain]
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.webpubsub.models.WebPubSubHub]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.CustomDomain]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.WebPubSubHub] = kwargs.pop("cls", None)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = await self._create_or_update_initial(  # type: ignore
+            raw_result = await self._create_or_update_initial(
+                hub_name=hub_name,
                 resource_group_name=resource_group_name,
                 resource_name=resource_name,
-                name=name,
                 parameters=parameters,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
-            deserialized = self._deserialize("CustomDomain", pipeline_response)
+            deserialized = self._deserialize("WebPubSubHub", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
         if polling is True:
-            polling_method = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))  # type: AsyncPollingMethod
+            polling_method: AsyncPollingMethod = cast(
+                AsyncPollingMethod,
+                AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
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
 
-    begin_create_or_update.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customDomains/{name}"}  # type: ignore
+    begin_create_or_update.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/hubs/{hubName}"
+    }
 
     async def _delete_initial(  # pylint: disable=inconsistent-return-statements
-        self, resource_group_name: str, resource_name: str, name: str, **kwargs: Any
+        self, hub_name: str, resource_group_name: str, resource_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
+            hub_name=hub_name,
             resource_group_name=resource_group_name,
             resource_name=resource_name,
-            name=name,
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
-    _delete_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customDomains/{name}"}  # type: ignore
+    _delete_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/hubs/{hubName}"
+    }
 
     @distributed_trace_async
     async def begin_delete(
-        self, resource_group_name: str, resource_name: str, name: str, **kwargs: Any
+        self, hub_name: str, resource_group_name: str, resource_name: str, **kwargs: Any
     ) -> AsyncLROPoller[None]:
-        """Delete a custom domain.
+        """Delete a hub setting.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param hub_name: The hub name. Required.
+        :type hub_name: str
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
-        :param name: Custom domain name. Required.
-        :type name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
@@ -525,49 +535,49 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
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
+                hub_name=hub_name,
                 resource_group_name=resource_group_name,
                 resource_name=resource_name,
-                name=name,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
                 return cls(pipeline_response, None, {})
 
         if polling is True:
-            polling_method = cast(
+            polling_method: AsyncPollingMethod = cast(
                 AsyncPollingMethod, AsyncARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
-            )  # type: AsyncPollingMethod
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
 
-    begin_delete.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customDomains/{name}"}  # type: ignore
+    begin_delete.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/hubs/{hubName}"
+    }
```

## Comparing `azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/operations/_patch.py` & `azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_shared_private_link_resources_operations.py` & `azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_shared_private_link_resources_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -34,18 +34,14 @@
 from ...operations._web_pub_sub_shared_private_link_resources_operations import (
     build_create_or_update_request,
     build_delete_request,
     build_get_request,
     build_list_request,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class WebPubSubSharedPrivateLinkResourcesOperations:
     """
     .. warning::
@@ -67,33 +63,31 @@
 
     @distributed_trace
     def list(
         self, resource_group_name: str, resource_name: str, **kwargs: Any
     ) -> AsyncIterable["_models.SharedPrivateLinkResource"]:
         """List shared private link resources.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either SharedPrivateLinkResource or the result of
          cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.webpubsub.models.SharedPrivateLinkResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.SharedPrivateLinkResourceList]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.SharedPrivateLinkResourceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -108,15 +102,15 @@
                     subscription_id=self._config.subscription_id,
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
@@ -124,55 +118,58 @@
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
             deserialized = self._deserialize("SharedPrivateLinkResourceList", pipeline_response)
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
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/sharedPrivateLinkResources"}  # type: ignore
+    list.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/sharedPrivateLinkResources"
+    }
 
     @distributed_trace_async
     async def get(
         self, shared_private_link_resource_name: str, resource_group_name: str, resource_name: str, **kwargs: Any
     ) -> _models.SharedPrivateLinkResource:
         """Get the specified shared private link resource.
 
         :param shared_private_link_resource_name: The name of the shared private link resource.
          Required.
         :type shared_private_link_resource_name: str
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: SharedPrivateLinkResource or the result of cls(response)
         :rtype: ~azure.mgmt.webpubsub.models.SharedPrivateLinkResource
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -184,34 +181,33 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.SharedPrivateLinkResource]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.SharedPrivateLinkResource] = kwargs.pop("cls", None)
 
         request = build_get_request(
             shared_private_link_resource_name=shared_private_link_resource_name,
             resource_group_name=resource_group_name,
             resource_name=resource_name,
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -220,15 +216,17 @@
         deserialized = self._deserialize("SharedPrivateLinkResource", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    get.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/sharedPrivateLinkResources/{sharedPrivateLinkResourceName}"}  # type: ignore
+    get.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/sharedPrivateLinkResources/{sharedPrivateLinkResourceName}"
+    }
 
     async def _create_or_update_initial(
         self,
         shared_private_link_resource_name: str,
         resource_group_name: str,
         resource_name: str,
         parameters: Union[_models.SharedPrivateLinkResource, IO],
@@ -241,24 +239,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.SharedPrivateLinkResource]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.SharedPrivateLinkResource] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "SharedPrivateLinkResource")
 
         request = build_create_or_update_request(
             shared_private_link_resource_name=shared_private_link_resource_name,
             resource_group_name=resource_group_name,
@@ -269,18 +265,19 @@
             json=_json,
             content=_content,
             template_url=self._create_or_update_initial.metadata["url"],
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
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -289,19 +286,21 @@
         if response.status_code == 200:
             deserialized = self._deserialize("SharedPrivateLinkResource", pipeline_response)
 
         if response.status_code == 201:
             deserialized = self._deserialize("SharedPrivateLinkResource", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
+        return deserialized  # type: ignore
 
-    _create_or_update_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/sharedPrivateLinkResources/{sharedPrivateLinkResourceName}"}  # type: ignore
+    _create_or_update_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/sharedPrivateLinkResources/{sharedPrivateLinkResourceName}"
+    }
 
     @overload
     async def begin_create_or_update(
         self,
         shared_private_link_resource_name: str,
         resource_group_name: str,
         resource_name: str,
@@ -311,16 +310,16 @@
         **kwargs: Any
     ) -> AsyncLROPoller[_models.SharedPrivateLinkResource]:
         """Create or update a shared private link resource.
 
         :param shared_private_link_resource_name: The name of the shared private link resource.
          Required.
         :type shared_private_link_resource_name: str
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :param parameters: The shared private link resource. Required.
         :type parameters: ~azure.mgmt.webpubsub.models.SharedPrivateLinkResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
@@ -352,16 +351,16 @@
         **kwargs: Any
     ) -> AsyncLROPoller[_models.SharedPrivateLinkResource]:
         """Create or update a shared private link resource.
 
         :param shared_private_link_resource_name: The name of the shared private link resource.
          Required.
         :type shared_private_link_resource_name: str
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :param parameters: The shared private link resource. Required.
         :type parameters: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
@@ -391,21 +390,21 @@
         **kwargs: Any
     ) -> AsyncLROPoller[_models.SharedPrivateLinkResource]:
         """Create or update a shared private link resource.
 
         :param shared_private_link_resource_name: The name of the shared private link resource.
          Required.
         :type shared_private_link_resource_name: str
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
-        :param parameters: The shared private link resource. Is either a model type or a IO type.
-         Required.
+        :param parameters: The shared private link resource. Is either a SharedPrivateLinkResource type
+         or a IO type. Required.
         :type parameters: ~azure.mgmt.webpubsub.models.SharedPrivateLinkResource or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -419,24 +418,22 @@
         :rtype:
          ~azure.core.polling.AsyncLROPoller[~azure.mgmt.webpubsub.models.SharedPrivateLinkResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.SharedPrivateLinkResource]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.SharedPrivateLinkResource] = kwargs.pop("cls", None)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = await self._create_or_update_initial(  # type: ignore
+            raw_result = await self._create_or_update_initial(
                 shared_private_link_resource_name=shared_private_link_resource_name,
                 resource_group_name=resource_group_name,
                 resource_name=resource_name,
                 parameters=parameters,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
@@ -449,29 +446,34 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("SharedPrivateLinkResource", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
         if polling is True:
-            polling_method = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))  # type: AsyncPollingMethod
+            polling_method: AsyncPollingMethod = cast(
+                AsyncPollingMethod,
+                AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
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
 
-    begin_create_or_update.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/sharedPrivateLinkResources/{sharedPrivateLinkResourceName}"}  # type: ignore
+    begin_create_or_update.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/sharedPrivateLinkResources/{sharedPrivateLinkResourceName}"
+    }
 
     async def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, shared_private_link_resource_name: str, resource_group_name: str, resource_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -479,59 +481,60 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             shared_private_link_resource_name=shared_private_link_resource_name,
             resource_group_name=resource_group_name,
             resource_name=resource_name,
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
-    _delete_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/sharedPrivateLinkResources/{sharedPrivateLinkResourceName}"}  # type: ignore
+    _delete_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/sharedPrivateLinkResources/{sharedPrivateLinkResourceName}"
+    }
 
     @distributed_trace_async
     async def begin_delete(
         self, shared_private_link_resource_name: str, resource_group_name: str, resource_name: str, **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Delete the specified shared private link resource.
 
         :param shared_private_link_resource_name: The name of the shared private link resource.
          Required.
         :type shared_private_link_resource_name: str
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
@@ -542,21 +545,19 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
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
                 shared_private_link_resource_name=shared_private_link_resource_name,
                 resource_group_name=resource_group_name,
                 resource_name=resource_name,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
@@ -567,24 +568,26 @@
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
                 return cls(pipeline_response, None, {})
 
         if polling is True:
-            polling_method = cast(
+            polling_method: AsyncPollingMethod = cast(
                 AsyncPollingMethod, AsyncARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
-            )  # type: AsyncPollingMethod
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
 
-    begin_delete.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/sharedPrivateLinkResources/{sharedPrivateLinkResourceName}"}  # type: ignore
+    begin_delete.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/sharedPrivateLinkResources/{sharedPrivateLinkResourceName}"
+    }
```

## Comparing `azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_custom_certificates_operations.py` & `azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_custom_certificates_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -34,18 +34,14 @@
 from ...operations._web_pub_sub_custom_certificates_operations import (
     build_create_or_update_request,
     build_delete_request,
     build_get_request,
     build_list_request,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class WebPubSubCustomCertificatesOperations:
     """
     .. warning::
@@ -67,31 +63,29 @@
 
     @distributed_trace
     def list(
         self, resource_group_name: str, resource_name: str, **kwargs: Any
     ) -> AsyncIterable["_models.CustomCertificate"]:
         """List all custom certificates.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either CustomCertificate or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.webpubsub.models.CustomCertificate]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.CustomCertificateList]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.CustomCertificateList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -106,15 +100,15 @@
                     subscription_id=self._config.subscription_id,
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
@@ -122,52 +116,55 @@
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
             deserialized = self._deserialize("CustomCertificateList", pipeline_response)
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
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customCertificates"}  # type: ignore
+    list.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customCertificates"
+    }
 
     @distributed_trace_async
     async def get(
         self, resource_group_name: str, resource_name: str, certificate_name: str, **kwargs: Any
     ) -> _models.CustomCertificate:
         """Get a custom certificate.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :param certificate_name: Custom certificate name. Required.
         :type certificate_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: CustomCertificate or the result of cls(response)
@@ -181,34 +178,33 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.CustomCertificate]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.CustomCertificate] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
             certificate_name=certificate_name,
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -217,15 +213,17 @@
         deserialized = self._deserialize("CustomCertificate", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    get.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customCertificates/{certificateName}"}  # type: ignore
+    get.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customCertificates/{certificateName}"
+    }
 
     async def _create_or_update_initial(
         self,
         resource_group_name: str,
         resource_name: str,
         certificate_name: str,
         parameters: Union[_models.CustomCertificate, IO],
@@ -238,24 +236,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.CustomCertificate]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.CustomCertificate] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "CustomCertificate")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
@@ -266,18 +262,19 @@
             json=_json,
             content=_content,
             template_url=self._create_or_update_initial.metadata["url"],
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
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -286,35 +283,37 @@
         if response.status_code == 200:
             deserialized = self._deserialize("CustomCertificate", pipeline_response)
 
         if response.status_code == 201:
             deserialized = self._deserialize("CustomCertificate", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
+        return deserialized  # type: ignore
 
-    _create_or_update_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customCertificates/{certificateName}"}  # type: ignore
+    _create_or_update_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customCertificates/{certificateName}"
+    }
 
     @overload
     async def begin_create_or_update(
         self,
         resource_group_name: str,
         resource_name: str,
         certificate_name: str,
         parameters: _models.CustomCertificate,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.CustomCertificate]:
         """Create or update a custom certificate.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :param certificate_name: Custom certificate name. Required.
         :type certificate_name: str
         :param parameters: Required.
         :type parameters: ~azure.mgmt.webpubsub.models.CustomCertificate
@@ -344,16 +343,16 @@
         parameters: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.CustomCertificate]:
         """Create or update a custom certificate.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :param certificate_name: Custom certificate name. Required.
         :type certificate_name: str
         :param parameters: Required.
         :type parameters: IO
@@ -381,22 +380,22 @@
         resource_name: str,
         certificate_name: str,
         parameters: Union[_models.CustomCertificate, IO],
         **kwargs: Any
     ) -> AsyncLROPoller[_models.CustomCertificate]:
         """Create or update a custom certificate.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :param certificate_name: Custom certificate name. Required.
         :type certificate_name: str
-        :param parameters: Is either a model type or a IO type. Required.
+        :param parameters: Is either a CustomCertificate type or a IO type. Required.
         :type parameters: ~azure.mgmt.webpubsub.models.CustomCertificate or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json',
          'text/json'. Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -409,24 +408,22 @@
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.webpubsub.models.CustomCertificate]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.CustomCertificate]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.CustomCertificate] = kwargs.pop("cls", None)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = await self._create_or_update_initial(  # type: ignore
+            raw_result = await self._create_or_update_initial(
                 resource_group_name=resource_group_name,
                 resource_name=resource_name,
                 certificate_name=certificate_name,
                 parameters=parameters,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
@@ -439,38 +436,43 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("CustomCertificate", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
         if polling is True:
-            polling_method = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))  # type: AsyncPollingMethod
+            polling_method: AsyncPollingMethod = cast(
+                AsyncPollingMethod,
+                AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
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
 
-    begin_create_or_update.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customCertificates/{certificateName}"}  # type: ignore
+    begin_create_or_update.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customCertificates/{certificateName}"
+    }
 
     @distributed_trace_async
     async def delete(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, resource_name: str, certificate_name: str, **kwargs: Any
     ) -> None:
         """Delete a custom certificate.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :param certificate_name: Custom certificate name. Required.
         :type certificate_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
@@ -484,40 +486,41 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
             certificate_name=certificate_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.delete.metadata["url"],
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
 
         if response.status_code not in [200, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
-    delete.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customCertificates/{certificateName}"}  # type: ignore
+    delete.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customCertificates/{certificateName}"
+    }
```

## Comparing `azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/operations/_usages_operations.py` & `azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/operations/_usages_operations.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, AsyncIterable, Callable, Dict, Optional, TypeVar
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -26,18 +25,14 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._usages_operations import build_list_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class UsagesOperations:
     """
     .. warning::
@@ -68,18 +63,16 @@
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.webpubsub.models.SignalRServiceUsage]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.SignalRServiceUsageList]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.SignalRServiceUsageList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -93,15 +86,15 @@
                     subscription_id=self._config.subscription_id,
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
@@ -109,36 +102,39 @@
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
             deserialized = self._deserialize("SignalRServiceUsageList", pipeline_response)
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
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/providers/Microsoft.SignalRService/locations/{location}/usages"}  # type: ignore
+    list.metadata = {
+        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.SignalRService/locations/{location}/usages"
+    }
```

## Comparing `azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_hubs_operations.py` & `azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_custom_domains_operations.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -27,71 +27,65 @@
 from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.async_arm_polling import AsyncARMPolling
 
 from ... import models as _models
 from ..._vendor import _convert_request
-from ...operations._web_pub_sub_hubs_operations import (
+from ...operations._web_pub_sub_custom_domains_operations import (
     build_create_or_update_request,
     build_delete_request,
     build_get_request,
     build_list_request,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
-class WebPubSubHubsOperations:
+class WebPubSubCustomDomainsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.webpubsub.aio.WebPubSubManagementClient`'s
-        :attr:`web_pub_sub_hubs` attribute.
+        :attr:`web_pub_sub_custom_domains` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
     def list(
         self, resource_group_name: str, resource_name: str, **kwargs: Any
-    ) -> AsyncIterable["_models.WebPubSubHub"]:
-        """List hub settings.
+    ) -> AsyncIterable["_models.CustomDomain"]:
+        """List all custom domains.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either WebPubSubHub or the result of cls(response)
-        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.webpubsub.models.WebPubSubHub]
+        :return: An iterator like instance of either CustomDomain or the result of cls(response)
+        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.webpubsub.models.CustomDomain]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.WebPubSubHubList]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.CustomDomainList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -106,15 +100,15 @@
                     subscription_id=self._config.subscription_id,
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
@@ -122,409 +116,411 @@
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
-            deserialized = self._deserialize("WebPubSubHubList", pipeline_response)
+            deserialized = self._deserialize("CustomDomainList", pipeline_response)
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
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/hubs"}  # type: ignore
+    list.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customDomains"
+    }
 
     @distributed_trace_async
-    async def get(
-        self, hub_name: str, resource_group_name: str, resource_name: str, **kwargs: Any
-    ) -> _models.WebPubSubHub:
-        """Get a hub setting.
-
-        :param hub_name: The hub name. Required.
-        :type hub_name: str
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+    async def get(self, resource_group_name: str, resource_name: str, name: str, **kwargs: Any) -> _models.CustomDomain:
+        """Get a custom domain.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
+        :param name: Custom domain name. Required.
+        :type name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: WebPubSubHub or the result of cls(response)
-        :rtype: ~azure.mgmt.webpubsub.models.WebPubSubHub
+        :return: CustomDomain or the result of cls(response)
+        :rtype: ~azure.mgmt.webpubsub.models.CustomDomain
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.WebPubSubHub]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.CustomDomain] = kwargs.pop("cls", None)
 
         request = build_get_request(
-            hub_name=hub_name,
             resource_group_name=resource_group_name,
             resource_name=resource_name,
+            name=name,
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize("WebPubSubHub", pipeline_response)
+        deserialized = self._deserialize("CustomDomain", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    get.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/hubs/{hubName}"}  # type: ignore
+    get.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customDomains/{name}"
+    }
 
     async def _create_or_update_initial(
         self,
-        hub_name: str,
         resource_group_name: str,
         resource_name: str,
-        parameters: Union[_models.WebPubSubHub, IO],
+        name: str,
+        parameters: Union[_models.CustomDomain, IO],
         **kwargs: Any
-    ) -> _models.WebPubSubHub:
+    ) -> _models.CustomDomain:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.WebPubSubHub]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.CustomDomain] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
-            _json = self._serialize.body(parameters, "WebPubSubHub")
+            _json = self._serialize.body(parameters, "CustomDomain")
 
         request = build_create_or_update_request(
-            hub_name=hub_name,
             resource_group_name=resource_group_name,
             resource_name=resource_name,
+            name=name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
             template_url=self._create_or_update_initial.metadata["url"],
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
 
-        if response.status_code not in [200, 201]:
+        if response.status_code not in [201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        if response.status_code == 200:
-            deserialized = self._deserialize("WebPubSubHub", pipeline_response)
-
-        if response.status_code == 201:
-            deserialized = self._deserialize("WebPubSubHub", pipeline_response)
+        deserialized = self._deserialize("CustomDomain", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    _create_or_update_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/hubs/{hubName}"}  # type: ignore
+    _create_or_update_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customDomains/{name}"
+    }
 
     @overload
     async def begin_create_or_update(
         self,
-        hub_name: str,
         resource_group_name: str,
         resource_name: str,
-        parameters: _models.WebPubSubHub,
+        name: str,
+        parameters: _models.CustomDomain,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.WebPubSubHub]:
-        """Create or update a hub setting.
+    ) -> AsyncLROPoller[_models.CustomDomain]:
+        """Create or update a custom domain.
 
-        :param hub_name: The hub name. Required.
-        :type hub_name: str
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
-        :param parameters: The resource of WebPubSubHub and its properties. Required.
-        :type parameters: ~azure.mgmt.webpubsub.models.WebPubSubHub
+        :param name: Custom domain name. Required.
+        :type name: str
+        :param parameters: Required.
+        :type parameters: ~azure.mgmt.webpubsub.models.CustomDomain
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either WebPubSubHub or the result of
+        :return: An instance of AsyncLROPoller that returns either CustomDomain or the result of
          cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.webpubsub.models.WebPubSubHub]
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.webpubsub.models.CustomDomain]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_create_or_update(
         self,
-        hub_name: str,
         resource_group_name: str,
         resource_name: str,
+        name: str,
         parameters: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.WebPubSubHub]:
-        """Create or update a hub setting.
+    ) -> AsyncLROPoller[_models.CustomDomain]:
+        """Create or update a custom domain.
 
-        :param hub_name: The hub name. Required.
-        :type hub_name: str
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
-        :param parameters: The resource of WebPubSubHub and its properties. Required.
+        :param name: Custom domain name. Required.
+        :type name: str
+        :param parameters: Required.
         :type parameters: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
-         Default value is "application/json".
+         Known values are: 'application/json', 'text/json'. Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either WebPubSubHub or the result of
+        :return: An instance of AsyncLROPoller that returns either CustomDomain or the result of
          cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.webpubsub.models.WebPubSubHub]
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.webpubsub.models.CustomDomain]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_create_or_update(
         self,
-        hub_name: str,
         resource_group_name: str,
         resource_name: str,
-        parameters: Union[_models.WebPubSubHub, IO],
+        name: str,
+        parameters: Union[_models.CustomDomain, IO],
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.WebPubSubHub]:
-        """Create or update a hub setting.
+    ) -> AsyncLROPoller[_models.CustomDomain]:
+        """Create or update a custom domain.
 
-        :param hub_name: The hub name. Required.
-        :type hub_name: str
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
-        :param parameters: The resource of WebPubSubHub and its properties. Is either a model type or a
-         IO type. Required.
-        :type parameters: ~azure.mgmt.webpubsub.models.WebPubSubHub or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
+        :param name: Custom domain name. Required.
+        :type name: str
+        :param parameters: Is either a CustomDomain type or a IO type. Required.
+        :type parameters: ~azure.mgmt.webpubsub.models.CustomDomain or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/json',
+         'text/json'. Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either WebPubSubHub or the result of
+        :return: An instance of AsyncLROPoller that returns either CustomDomain or the result of
          cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.webpubsub.models.WebPubSubHub]
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.webpubsub.models.CustomDomain]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.WebPubSubHub]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.CustomDomain] = kwargs.pop("cls", None)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = await self._create_or_update_initial(  # type: ignore
-                hub_name=hub_name,
+            raw_result = await self._create_or_update_initial(
                 resource_group_name=resource_group_name,
                 resource_name=resource_name,
+                name=name,
                 parameters=parameters,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
-            deserialized = self._deserialize("WebPubSubHub", pipeline_response)
+            deserialized = self._deserialize("CustomDomain", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
         if polling is True:
-            polling_method = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))  # type: AsyncPollingMethod
+            polling_method: AsyncPollingMethod = cast(
+                AsyncPollingMethod,
+                AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
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
 
-    begin_create_or_update.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/hubs/{hubName}"}  # type: ignore
+    begin_create_or_update.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customDomains/{name}"
+    }
 
     async def _delete_initial(  # pylint: disable=inconsistent-return-statements
-        self, hub_name: str, resource_group_name: str, resource_name: str, **kwargs: Any
+        self, resource_group_name: str, resource_name: str, name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
-            hub_name=hub_name,
             resource_group_name=resource_group_name,
             resource_name=resource_name,
+            name=name,
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
-    _delete_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/hubs/{hubName}"}  # type: ignore
+    _delete_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customDomains/{name}"
+    }
 
     @distributed_trace_async
     async def begin_delete(
-        self, hub_name: str, resource_group_name: str, resource_name: str, **kwargs: Any
+        self, resource_group_name: str, resource_name: str, name: str, **kwargs: Any
     ) -> AsyncLROPoller[None]:
-        """Delete a hub setting.
+        """Delete a custom domain.
 
-        :param hub_name: The hub name. Required.
-        :type hub_name: str
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
+        :param name: Custom domain name. Required.
+        :type name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
@@ -532,49 +528,49 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
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
-                hub_name=hub_name,
                 resource_group_name=resource_group_name,
                 resource_name=resource_name,
+                name=name,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
                 return cls(pipeline_response, None, {})
 
         if polling is True:
-            polling_method = cast(
+            polling_method: AsyncPollingMethod = cast(
                 AsyncPollingMethod, AsyncARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
-            )  # type: AsyncPollingMethod
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
 
-    begin_delete.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/hubs/{hubName}"}  # type: ignore
+    begin_delete.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/customDomains/{name}"
+    }
```

## Comparing `azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/operations/_operations.py` & `azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/operations/_operations.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, AsyncIterable, Callable, Dict, Optional, TypeVar
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -26,18 +25,14 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._operations import build_list_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class Operations:
     """
     .. warning::
@@ -65,18 +60,16 @@
         :return: An iterator like instance of either Operation or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.webpubsub.models.Operation]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.OperationList]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.OperationList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -88,15 +81,15 @@
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
@@ -104,36 +97,37 @@
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
             deserialized = self._deserialize("OperationList", pipeline_response)
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
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list.metadata = {"url": "/providers/Microsoft.SignalRService/operations"}  # type: ignore
+    list.metadata = {"url": "/providers/Microsoft.SignalRService/operations"}
```

## Comparing `azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_private_endpoint_connections_operations.py` & `azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_private_endpoint_connections_operations.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -34,18 +34,14 @@
 from ...operations._web_pub_sub_private_endpoint_connections_operations import (
     build_delete_request,
     build_get_request,
     build_list_request,
     build_update_request,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class WebPubSubPrivateEndpointConnectionsOperations:
     """
     .. warning::
@@ -67,33 +63,31 @@
 
     @distributed_trace
     def list(
         self, resource_group_name: str, resource_name: str, **kwargs: Any
     ) -> AsyncIterable["_models.PrivateEndpointConnection"]:
         """List private endpoint connections.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either PrivateEndpointConnection or the result of
          cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.webpubsub.models.PrivateEndpointConnection]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.PrivateEndpointConnectionList]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.PrivateEndpointConnectionList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -108,15 +102,15 @@
                     subscription_id=self._config.subscription_id,
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
@@ -124,54 +118,58 @@
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
             deserialized = self._deserialize("PrivateEndpointConnectionList", pipeline_response)
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
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/privateEndpointConnections"}  # type: ignore
+    list.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/privateEndpointConnections"
+    }
 
     @distributed_trace_async
     async def get(
         self, private_endpoint_connection_name: str, resource_group_name: str, resource_name: str, **kwargs: Any
     ) -> _models.PrivateEndpointConnection:
         """Get the specified private endpoint connection.
 
-        :param private_endpoint_connection_name: The name of the private endpoint connection. Required.
+        :param private_endpoint_connection_name: The name of the private endpoint connection associated
+         with the Azure resource. Required.
         :type private_endpoint_connection_name: str
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PrivateEndpointConnection or the result of cls(response)
         :rtype: ~azure.mgmt.webpubsub.models.PrivateEndpointConnection
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -183,34 +181,33 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.PrivateEndpointConnection]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.PrivateEndpointConnection] = kwargs.pop("cls", None)
 
         request = build_get_request(
             private_endpoint_connection_name=private_endpoint_connection_name,
             resource_group_name=resource_group_name,
             resource_name=resource_name,
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -219,33 +216,36 @@
         deserialized = self._deserialize("PrivateEndpointConnection", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    get.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}"}  # type: ignore
+    get.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}"
+    }
 
     @overload
     async def update(
         self,
         private_endpoint_connection_name: str,
         resource_group_name: str,
         resource_name: str,
         parameters: _models.PrivateEndpointConnection,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.PrivateEndpointConnection:
         """Update the state of specified private endpoint connection.
 
-        :param private_endpoint_connection_name: The name of the private endpoint connection. Required.
+        :param private_endpoint_connection_name: The name of the private endpoint connection associated
+         with the Azure resource. Required.
         :type private_endpoint_connection_name: str
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :param parameters: The resource of private endpoint and its properties. Required.
         :type parameters: ~azure.mgmt.webpubsub.models.PrivateEndpointConnection
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
@@ -265,18 +265,19 @@
         parameters: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.PrivateEndpointConnection:
         """Update the state of specified private endpoint connection.
 
-        :param private_endpoint_connection_name: The name of the private endpoint connection. Required.
+        :param private_endpoint_connection_name: The name of the private endpoint connection associated
+         with the Azure resource. Required.
         :type private_endpoint_connection_name: str
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :param parameters: The resource of private endpoint and its properties. Required.
         :type parameters: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
@@ -294,23 +295,24 @@
         resource_group_name: str,
         resource_name: str,
         parameters: Union[_models.PrivateEndpointConnection, IO],
         **kwargs: Any
     ) -> _models.PrivateEndpointConnection:
         """Update the state of specified private endpoint connection.
 
-        :param private_endpoint_connection_name: The name of the private endpoint connection. Required.
+        :param private_endpoint_connection_name: The name of the private endpoint connection associated
+         with the Azure resource. Required.
         :type private_endpoint_connection_name: str
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
-        :param parameters: The resource of private endpoint and its properties. Is either a model type
-         or a IO type. Required.
+        :param parameters: The resource of private endpoint and its properties. Is either a
+         PrivateEndpointConnection type or a IO type. Required.
         :type parameters: ~azure.mgmt.webpubsub.models.PrivateEndpointConnection or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PrivateEndpointConnection or the result of cls(response)
         :rtype: ~azure.mgmt.webpubsub.models.PrivateEndpointConnection
@@ -323,24 +325,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.PrivateEndpointConnection]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.PrivateEndpointConnection] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "PrivateEndpointConnection")
 
         request = build_update_request(
             private_endpoint_connection_name=private_endpoint_connection_name,
             resource_group_name=resource_group_name,
@@ -351,18 +351,19 @@
             json=_json,
             content=_content,
             template_url=self.update.metadata["url"],
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -371,15 +372,17 @@
         deserialized = self._deserialize("PrivateEndpointConnection", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    update.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}"}  # type: ignore
+    update.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}"
+    }
 
     async def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, private_endpoint_connection_name: str, resource_group_name: str, resource_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -387,58 +390,60 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             private_endpoint_connection_name=private_endpoint_connection_name,
             resource_group_name=resource_group_name,
             resource_name=resource_name,
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
-    _delete_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}"}  # type: ignore
+    _delete_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}"
+    }
 
     @distributed_trace_async
     async def begin_delete(
         self, private_endpoint_connection_name: str, resource_group_name: str, resource_name: str, **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Delete the specified private endpoint connection.
 
-        :param private_endpoint_connection_name: The name of the private endpoint connection. Required.
+        :param private_endpoint_connection_name: The name of the private endpoint connection associated
+         with the Azure resource. Required.
         :type private_endpoint_connection_name: str
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
@@ -449,21 +454,19 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
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
                 private_endpoint_connection_name=private_endpoint_connection_name,
                 resource_group_name=resource_group_name,
                 resource_name=resource_name,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
@@ -474,24 +477,26 @@
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
                 return cls(pipeline_response, None, {})
 
         if polling is True:
-            polling_method = cast(
+            polling_method: AsyncPollingMethod = cast(
                 AsyncPollingMethod, AsyncARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
-            )  # type: AsyncPollingMethod
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
 
-    begin_delete.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}"}  # type: ignore
+    begin_delete.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}"
+    }
```

## Comparing `azure-mgmt-webpubsub-1.1.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_operations.py` & `azure-mgmt-webpubsub-2.0.0b1/azure/mgmt/webpubsub/aio/operations/_web_pub_sub_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -35,24 +35,21 @@
     build_check_name_availability_request,
     build_create_or_update_request,
     build_delete_request,
     build_get_request,
     build_list_by_resource_group_request,
     build_list_by_subscription_request,
     build_list_keys_request,
+    build_list_replica_skus_request,
     build_list_skus_request,
     build_regenerate_key_request,
     build_restart_request,
     build_update_request,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class WebPubSubOperations:
     """
     .. warning::
@@ -119,16 +116,16 @@
     async def check_name_availability(
         self, location: str, parameters: Union[_models.NameAvailabilityParameters, IO], **kwargs: Any
     ) -> _models.NameAvailability:
         """Checks that the resource name is valid and is not already in use.
 
         :param location: the region. Required.
         :type location: str
-        :param parameters: Parameters supplied to the operation. Is either a model type or a IO type.
-         Required.
+        :param parameters: Parameters supplied to the operation. Is either a NameAvailabilityParameters
+         type or a IO type. Required.
         :type parameters: ~azure.mgmt.webpubsub.models.NameAvailabilityParameters or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: NameAvailability or the result of cls(response)
         :rtype: ~azure.mgmt.webpubsub.models.NameAvailability
@@ -141,24 +138,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.NameAvailability]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.NameAvailability] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "NameAvailabilityParameters")
 
         request = build_check_name_availability_request(
             location=location,
             subscription_id=self._config.subscription_id,
@@ -167,18 +162,19 @@
             json=_json,
             content=_content,
             template_url=self.check_name_availability.metadata["url"],
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -187,32 +183,32 @@
         deserialized = self._deserialize("NameAvailability", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    check_name_availability.metadata = {"url": "/subscriptions/{subscriptionId}/providers/Microsoft.SignalRService/locations/{location}/checkNameAvailability"}  # type: ignore
+    check_name_availability.metadata = {
+        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.SignalRService/locations/{location}/checkNameAvailability"
+    }
 
     @distributed_trace
     def list_by_subscription(self, **kwargs: Any) -> AsyncIterable["_models.WebPubSubResource"]:
         """Handles requests to list all resources in a subscription.
 
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either WebPubSubResource or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.webpubsub.models.WebPubSubResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.WebPubSubResourceList]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.WebPubSubResourceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -225,15 +221,15 @@
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
@@ -241,65 +237,66 @@
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
             deserialized = self._deserialize("WebPubSubResourceList", pipeline_response)
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
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list_by_subscription.metadata = {"url": "/subscriptions/{subscriptionId}/providers/Microsoft.SignalRService/webPubSub"}  # type: ignore
+    list_by_subscription.metadata = {
+        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.SignalRService/webPubSub"
+    }
 
     @distributed_trace
     def list_by_resource_group(
         self, resource_group_name: str, **kwargs: Any
     ) -> AsyncIterable["_models.WebPubSubResource"]:
         """Handles requests to list all resources in a resource group.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either WebPubSubResource or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.webpubsub.models.WebPubSubResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.WebPubSubResourceList]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.WebPubSubResourceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -313,15 +310,15 @@
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
@@ -329,50 +326,53 @@
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
             deserialized = self._deserialize("WebPubSubResourceList", pipeline_response)
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
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list_by_resource_group.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub"}  # type: ignore
+    list_by_resource_group.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub"
+    }
 
     @distributed_trace_async
     async def get(self, resource_group_name: str, resource_name: str, **kwargs: Any) -> _models.WebPubSubResource:
         """Get the resource and its properties.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: WebPubSubResource or the result of cls(response)
         :rtype: ~azure.mgmt.webpubsub.models.WebPubSubResource
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -384,33 +384,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.WebPubSubResource]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.WebPubSubResource] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -419,15 +418,17 @@
         deserialized = self._deserialize("WebPubSubResource", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    get.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}"}  # type: ignore
+    get.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}"
+    }
 
     async def _create_or_update_initial(
         self,
         resource_group_name: str,
         resource_name: str,
         parameters: Union[_models.WebPubSubResource, IO],
         **kwargs: Any
@@ -439,24 +440,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[Optional[_models.WebPubSubResource]]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[Optional[_models.WebPubSubResource]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "WebPubSubResource")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
@@ -466,18 +465,19 @@
             json=_json,
             content=_content,
             template_url=self._create_or_update_initial.metadata["url"],
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
 
         if response.status_code not in [200, 201, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -491,30 +491,32 @@
             deserialized = self._deserialize("WebPubSubResource", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    _create_or_update_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}"}  # type: ignore
+    _create_or_update_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}"
+    }
 
     @overload
     async def begin_create_or_update(
         self,
         resource_group_name: str,
         resource_name: str,
         parameters: _models.WebPubSubResource,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.WebPubSubResource]:
         """Create or update a resource.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :param parameters: Parameters for the create or update operation. Required.
         :type parameters: ~azure.mgmt.webpubsub.models.WebPubSubResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
@@ -541,16 +543,16 @@
         parameters: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.WebPubSubResource]:
         """Create or update a resource.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :param parameters: Parameters for the create or update operation. Required.
         :type parameters: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
@@ -575,21 +577,21 @@
         resource_group_name: str,
         resource_name: str,
         parameters: Union[_models.WebPubSubResource, IO],
         **kwargs: Any
     ) -> AsyncLROPoller[_models.WebPubSubResource]:
         """Create or update a resource.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
-        :param parameters: Parameters for the create or update operation. Is either a model type or a
-         IO type. Required.
+        :param parameters: Parameters for the create or update operation. Is either a WebPubSubResource
+         type or a IO type. Required.
         :type parameters: ~azure.mgmt.webpubsub.models.WebPubSubResource or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -602,24 +604,22 @@
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.webpubsub.models.WebPubSubResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.WebPubSubResource]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.WebPubSubResource] = kwargs.pop("cls", None)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = await self._create_or_update_initial(  # type: ignore
+            raw_result = await self._create_or_update_initial(
                 resource_group_name=resource_group_name,
                 resource_name=resource_name,
                 parameters=parameters,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
@@ -631,29 +631,34 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("WebPubSubResource", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
         if polling is True:
-            polling_method = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))  # type: AsyncPollingMethod
+            polling_method: AsyncPollingMethod = cast(
+                AsyncPollingMethod,
+                AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
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
 
-    begin_create_or_update.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}"}  # type: ignore
+    begin_create_or_update.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}"
+    }
 
     async def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, resource_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -661,53 +666,54 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
-    _delete_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}"}  # type: ignore
+    _delete_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}"
+    }
 
     @distributed_trace_async
     async def begin_delete(self, resource_group_name: str, resource_name: str, **kwargs: Any) -> AsyncLROPoller[None]:
         """Operation to delete a resource.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
@@ -718,21 +724,19 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
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
                 resource_name=resource_name,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
                 headers=_headers,
@@ -742,31 +746,33 @@
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
                 return cls(pipeline_response, None, {})
 
         if polling is True:
-            polling_method = cast(
+            polling_method: AsyncPollingMethod = cast(
                 AsyncPollingMethod, AsyncARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
-            )  # type: AsyncPollingMethod
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
 
-    begin_delete.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}"}  # type: ignore
+    begin_delete.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}"
+    }
 
     async def _update_initial(
         self,
         resource_group_name: str,
         resource_name: str,
         parameters: Union[_models.WebPubSubResource, IO],
         **kwargs: Any
@@ -778,24 +784,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[Optional[_models.WebPubSubResource]]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[Optional[_models.WebPubSubResource]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "WebPubSubResource")
 
         request = build_update_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
@@ -805,52 +809,59 @@
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = None
+        response_headers = {}
         if response.status_code == 200:
             deserialized = self._deserialize("WebPubSubResource", pipeline_response)
 
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, response_headers)
 
         return deserialized
 
-    _update_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}"}  # type: ignore
+    _update_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}"
+    }
 
     @overload
     async def begin_update(
         self,
         resource_group_name: str,
         resource_name: str,
         parameters: _models.WebPubSubResource,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.WebPubSubResource]:
         """Operation to update an exiting resource.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :param parameters: Parameters for the update operation. Required.
         :type parameters: ~azure.mgmt.webpubsub.models.WebPubSubResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
@@ -877,16 +888,16 @@
         parameters: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.WebPubSubResource]:
         """Operation to update an exiting resource.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :param parameters: Parameters for the update operation. Required.
         :type parameters: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
@@ -911,21 +922,21 @@
         resource_group_name: str,
         resource_name: str,
         parameters: Union[_models.WebPubSubResource, IO],
         **kwargs: Any
     ) -> AsyncLROPoller[_models.WebPubSubResource]:
         """Operation to update an exiting resource.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
-        :param parameters: Parameters for the update operation. Is either a model type or a IO type.
-         Required.
+        :param parameters: Parameters for the update operation. Is either a WebPubSubResource type or a
+         IO type. Required.
         :type parameters: ~azure.mgmt.webpubsub.models.WebPubSubResource or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -938,24 +949,22 @@
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.webpubsub.models.WebPubSubResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.WebPubSubResource]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.WebPubSubResource] = kwargs.pop("cls", None)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = await self._update_initial(  # type: ignore
+            raw_result = await self._update_initial(
                 resource_group_name=resource_group_name,
                 resource_name=resource_name,
                 parameters=parameters,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
@@ -967,36 +976,40 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("WebPubSubResource", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
         if polling is True:
-            polling_method = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))  # type: AsyncPollingMethod
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
 
-    begin_update.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}"}  # type: ignore
+    begin_update.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}"
+    }
 
     @distributed_trace_async
     async def list_keys(self, resource_group_name: str, resource_name: str, **kwargs: Any) -> _models.WebPubSubKeys:
         """Get the access keys of the resource.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: WebPubSubKeys or the result of cls(response)
         :rtype: ~azure.mgmt.webpubsub.models.WebPubSubKeys
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -1008,33 +1021,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.WebPubSubKeys]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.WebPubSubKeys] = kwargs.pop("cls", None)
 
         request = build_list_keys_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.list_keys.metadata["url"],
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -1043,15 +1055,17 @@
         deserialized = self._deserialize("WebPubSubKeys", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    list_keys.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/listKeys"}  # type: ignore
+    list_keys.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/listKeys"
+    }
 
     async def _regenerate_key_initial(
         self,
         resource_group_name: str,
         resource_name: str,
         parameters: Union[_models.RegenerateKeyParameters, IO],
         **kwargs: Any
@@ -1063,24 +1077,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.WebPubSubKeys]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.WebPubSubKeys] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "RegenerateKeyParameters")
 
         request = build_regenerate_key_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
@@ -1090,51 +1102,61 @@
             json=_json,
             content=_content,
             template_url=self._regenerate_key_initial.metadata["url"],
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
 
-        if response.status_code not in [202]:
+        if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize("WebPubSubKeys", pipeline_response)
+        response_headers = {}
+        if response.status_code == 200:
+            deserialized = self._deserialize("WebPubSubKeys", pipeline_response)
+
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+
+            deserialized = self._deserialize("WebPubSubKeys", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
-        return deserialized
+        return deserialized  # type: ignore
 
-    _regenerate_key_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/regenerateKey"}  # type: ignore
+    _regenerate_key_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/regenerateKey"
+    }
 
     @overload
     async def begin_regenerate_key(
         self,
         resource_group_name: str,
         resource_name: str,
         parameters: _models.RegenerateKeyParameters,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.WebPubSubKeys]:
         """Regenerate the access key for the resource. PrimaryKey and SecondaryKey cannot be regenerated
         at the same time.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :param parameters: Parameter that describes the Regenerate Key Operation. Required.
         :type parameters: ~azure.mgmt.webpubsub.models.RegenerateKeyParameters
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
@@ -1162,16 +1184,16 @@
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.WebPubSubKeys]:
         """Regenerate the access key for the resource. PrimaryKey and SecondaryKey cannot be regenerated
         at the same time.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :param parameters: Parameter that describes the Regenerate Key Operation. Required.
         :type parameters: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
@@ -1197,21 +1219,21 @@
         resource_name: str,
         parameters: Union[_models.RegenerateKeyParameters, IO],
         **kwargs: Any
     ) -> AsyncLROPoller[_models.WebPubSubKeys]:
         """Regenerate the access key for the resource. PrimaryKey and SecondaryKey cannot be regenerated
         at the same time.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
-        :param parameters: Parameter that describes the Regenerate Key Operation. Is either a model
-         type or a IO type. Required.
+        :param parameters: Parameter that describes the Regenerate Key Operation. Is either a
+         RegenerateKeyParameters type or a IO type. Required.
         :type parameters: ~azure.mgmt.webpubsub.models.RegenerateKeyParameters or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -1224,24 +1246,22 @@
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.webpubsub.models.WebPubSubKeys]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.WebPubSubKeys]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.WebPubSubKeys] = kwargs.pop("cls", None)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = await self._regenerate_key_initial(  # type: ignore
+            raw_result = await self._regenerate_key_initial(
                 resource_group_name=resource_group_name,
                 resource_name=resource_name,
                 parameters=parameters,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
@@ -1253,32 +1273,101 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("WebPubSubKeys", pipeline_response)
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
+
+    begin_regenerate_key.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/regenerateKey"
+    }
+
+    @distributed_trace_async
+    async def list_replica_skus(
+        self, resource_group_name: str, resource_name: str, replica_name: str, **kwargs: Any
+    ) -> _models.SkuList:
+        """List all available skus of the replica resource.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param resource_name: The name of the resource. Required.
+        :type resource_name: str
+        :param replica_name: The name of the replica. Required.
+        :type replica_name: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :return: SkuList or the result of cls(response)
+        :rtype: ~azure.mgmt.webpubsub.models.SkuList
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
 
-    begin_regenerate_key.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/regenerateKey"}  # type: ignore
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.SkuList] = kwargs.pop("cls", None)
+
+        request = build_list_replica_skus_request(
+            resource_group_name=resource_group_name,
+            resource_name=resource_name,
+            replica_name=replica_name,
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            template_url=self.list_replica_skus.metadata["url"],
+            headers=_headers,
+            params=_params,
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
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
+        deserialized = self._deserialize("SkuList", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    list_replica_skus.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/replicas/{replicaName}/skus"
+    }
 
     async def _restart_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, resource_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -1286,53 +1375,58 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_restart_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self._restart_initial.metadata["url"],
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
 
         if response.status_code not in [202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
+        response_headers = {}
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, None, response_headers)
 
-    _restart_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/restart"}  # type: ignore
+    _restart_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/restart"
+    }
 
     @distributed_trace_async
     async def begin_restart(self, resource_group_name: str, resource_name: str, **kwargs: Any) -> AsyncLROPoller[None]:
         """Operation to restart a resource.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
@@ -1343,21 +1437,19 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
-        polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._restart_initial(  # type: ignore
                 resource_group_name=resource_group_name,
                 resource_name=resource_name,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
                 headers=_headers,
@@ -1367,39 +1459,40 @@
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
 
-    begin_restart.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/restart"}  # type: ignore
+    begin_restart.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/restart"
+    }
 
     @distributed_trace_async
     async def list_skus(self, resource_group_name: str, resource_name: str, **kwargs: Any) -> _models.SkuList:
         """List all available skus of the resource.
 
-        :param resource_group_name: The name of the resource group that contains the resource. You can
-         obtain this value from the Azure Resource Manager API or the portal. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :param resource_name: The name of the resource. Required.
         :type resource_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: SkuList or the result of cls(response)
         :rtype: ~azure.mgmt.webpubsub.models.SkuList
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -1411,33 +1504,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )  # type: Literal["2022-08-01-preview"]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.SkuList]
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.SkuList] = kwargs.pop("cls", None)
 
         request = build_list_skus_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.list_skus.metadata["url"],
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
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -1446,8 +1538,10 @@
         deserialized = self._deserialize("SkuList", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    list_skus.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/skus"}  # type: ignore
+    list_skus.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.SignalRService/webPubSub/{resourceName}/skus"
+    }
```

