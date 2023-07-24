# Comparing `tmp/stix_shifter_modules_aws_athena-6.0.0.dev80-py2.py3-none-any.whl.zip` & `tmp/stix_shifter_modules_aws_athena-6.0.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,40 +1,40 @@
-Zip file size: 81136 bytes, number of entries: 38
--rw-rw-r--  2.0 unx        0 b- defN 23-Jul-24 15:13 stix_shifter_modules/aws_athena/__init__.py
--rw-rw-r--  2.0 unx     1374 b- defN 23-Jul-24 15:13 stix_shifter_modules/aws_athena/entry_point.py
--rw-rw-r--  2.0 unx   239955 b- defN 23-Jul-24 15:16 stix_shifter_modules/aws_athena/configuration/config.json
--rw-rw-r--  2.0 unx      229 b- defN 23-Jul-24 15:16 stix_shifter_modules/aws_athena/configuration/dialects.json
--rw-rw-r--  2.0 unx     4766 b- defN 23-Jul-24 15:16 stix_shifter_modules/aws_athena/configuration/lang_en.json
--rw-rw-r--  2.0 unx        0 b- defN 23-Jul-24 15:13 stix_shifter_modules/aws_athena/stix_translation/__init__.py
--rw-rw-r--  2.0 unx    27024 b- defN 23-Jul-24 15:16 stix_shifter_modules/aws_athena/stix_translation/json_to_stix_translator.py
--rw-rw-r--  2.0 unx    24044 b- defN 23-Jul-24 15:13 stix_shifter_modules/aws_athena/stix_translation/query_constructor.py
--rw-rw-r--  2.0 unx     1024 b- defN 23-Jul-24 15:13 stix_shifter_modules/aws_athena/stix_translation/query_translator.py
--rw-rw-r--  2.0 unx     1075 b- defN 23-Jul-24 15:13 stix_shifter_modules/aws_athena/stix_translation/transformers.py
--rw-rw-r--  2.0 unx     4765 b- defN 23-Jul-24 15:13 stix_shifter_modules/aws_athena/stix_translation/json/guardduty_config.json
--rw-rw-r--  2.0 unx     1894 b- defN 23-Jul-24 15:13 stix_shifter_modules/aws_athena/stix_translation/json/guardduty_from_stix_map.json
--rw-rw-r--  2.0 unx    10146 b- defN 23-Jul-24 15:13 stix_shifter_modules/aws_athena/stix_translation/json/guardduty_to_stix_map.json
--rw-rw-r--  2.0 unx      139 b- defN 23-Jul-24 15:13 stix_shifter_modules/aws_athena/stix_translation/json/hash_algorithm_map.json
--rw-rw-r--  2.0 unx     2439 b- defN 23-Jul-24 15:13 stix_shifter_modules/aws_athena/stix_translation/json/network_protocol_map.json
--rw-rw-r--  2.0 unx    18300 b- defN 23-Jul-24 15:13 stix_shifter_modules/aws_athena/stix_translation/json/ocsf_from_stix_map.json
--rw-rw-r--  2.0 unx    75601 b- defN 23-Jul-24 15:13 stix_shifter_modules/aws_athena/stix_translation/json/ocsf_to_stix_map.json
--rw-rw-r--  2.0 unx      591 b- defN 23-Jul-24 15:13 stix_shifter_modules/aws_athena/stix_translation/json/operators.json
--rw-rw-r--  2.0 unx      814 b- defN 23-Jul-24 15:13 stix_shifter_modules/aws_athena/stix_translation/json/vpcflow_from_stix_map.json
--rw-rw-r--  2.0 unx     2350 b- defN 23-Jul-24 15:13 stix_shifter_modules/aws_athena/stix_translation/json/vpcflow_to_stix_map.json
--rw-rw-r--  2.0 unx     1894 b- defN 23-Jul-24 15:13 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/guardduty_from_stix_map.json
--rw-rw-r--  2.0 unx    18297 b- defN 23-Jul-24 15:13 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/ocsf_from_stix_map.json
--rw-rw-r--  2.0 unx    93792 b- defN 23-Jul-24 15:13 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/to_stix_map.json
--rw-rw-r--  2.0 unx      891 b- defN 23-Jul-24 15:13 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/vpcflow_from_stix_map.json
--rw-rw-r--  2.0 unx        0 b- defN 23-Jul-24 15:13 stix_shifter_modules/aws_athena/stix_transmission/__init__.py
--rw-rw-r--  2.0 unx     4173 b- defN 23-Jul-24 15:13 stix_shifter_modules/aws_athena/stix_transmission/boto3_client.py
--rw-rw-r--  2.0 unx     1207 b- defN 23-Jul-24 15:13 stix_shifter_modules/aws_athena/stix_transmission/delete_connector.py
--rw-rw-r--  2.0 unx     1959 b- defN 23-Jul-24 15:13 stix_shifter_modules/aws_athena/stix_transmission/error_mapper.py
--rw-rw-r--  2.0 unx     1370 b- defN 23-Jul-24 15:13 stix_shifter_modules/aws_athena/stix_transmission/ping_connector.py
--rw-rw-r--  2.0 unx     7443 b- defN 23-Jul-24 15:13 stix_shifter_modules/aws_athena/stix_transmission/query_connector.py
--rw-rw-r--  2.0 unx    15539 b- defN 23-Jul-24 15:13 stix_shifter_modules/aws_athena/stix_transmission/results_connector.py
--rw-rw-r--  2.0 unx     3175 b- defN 23-Jul-24 15:13 stix_shifter_modules/aws_athena/stix_transmission/status_connector.py
--rw-rw-r--  2.0 unx    12786 b- defN 23-Jul-24 15:16 stix_shifter_modules_aws_athena-6.0.0.dev80.dist-info/LICENSE.md
--rw-rw-r--  2.0 unx     8046 b- defN 23-Jul-24 15:16 stix_shifter_modules_aws_athena-6.0.0.dev80.dist-info/METADATA
--rw-rw-r--  2.0 unx     1418 b- defN 23-Jul-24 15:16 stix_shifter_modules_aws_athena-6.0.0.dev80.dist-info/NOTICE
--rw-rw-r--  2.0 unx      110 b- defN 23-Jul-24 15:16 stix_shifter_modules_aws_athena-6.0.0.dev80.dist-info/WHEEL
--rw-rw-r--  2.0 unx       21 b- defN 23-Jul-24 15:16 stix_shifter_modules_aws_athena-6.0.0.dev80.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     4727 b- defN 23-Jul-24 15:16 stix_shifter_modules_aws_athena-6.0.0.dev80.dist-info/RECORD
-38 files, 593378 bytes uncompressed, 72984 bytes compressed:  87.7%
+Zip file size: 81052 bytes, number of entries: 38
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jul-24 17:41 stix_shifter_modules/aws_athena/__init__.py
+-rw-rw-r--  2.0 unx     1374 b- defN 23-Jul-24 17:41 stix_shifter_modules/aws_athena/entry_point.py
+-rw-rw-r--  2.0 unx   239955 b- defN 23-Jul-24 17:44 stix_shifter_modules/aws_athena/configuration/config.json
+-rw-rw-r--  2.0 unx      229 b- defN 23-Jul-24 17:44 stix_shifter_modules/aws_athena/configuration/dialects.json
+-rw-rw-r--  2.0 unx     4766 b- defN 23-Jul-24 17:44 stix_shifter_modules/aws_athena/configuration/lang_en.json
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jul-24 17:41 stix_shifter_modules/aws_athena/stix_translation/__init__.py
+-rw-rw-r--  2.0 unx    27024 b- defN 23-Jul-24 17:44 stix_shifter_modules/aws_athena/stix_translation/json_to_stix_translator.py
+-rw-rw-r--  2.0 unx    24044 b- defN 23-Jul-24 17:41 stix_shifter_modules/aws_athena/stix_translation/query_constructor.py
+-rw-rw-r--  2.0 unx     1024 b- defN 23-Jul-24 17:41 stix_shifter_modules/aws_athena/stix_translation/query_translator.py
+-rw-rw-r--  2.0 unx     1075 b- defN 23-Jul-24 17:41 stix_shifter_modules/aws_athena/stix_translation/transformers.py
+-rw-rw-r--  2.0 unx     4765 b- defN 23-Jul-24 17:41 stix_shifter_modules/aws_athena/stix_translation/json/guardduty_config.json
+-rw-rw-r--  2.0 unx     1894 b- defN 23-Jul-24 17:41 stix_shifter_modules/aws_athena/stix_translation/json/guardduty_from_stix_map.json
+-rw-rw-r--  2.0 unx    10146 b- defN 23-Jul-24 17:41 stix_shifter_modules/aws_athena/stix_translation/json/guardduty_to_stix_map.json
+-rw-rw-r--  2.0 unx      139 b- defN 23-Jul-24 17:41 stix_shifter_modules/aws_athena/stix_translation/json/hash_algorithm_map.json
+-rw-rw-r--  2.0 unx     2439 b- defN 23-Jul-24 17:41 stix_shifter_modules/aws_athena/stix_translation/json/network_protocol_map.json
+-rw-rw-r--  2.0 unx    18300 b- defN 23-Jul-24 17:41 stix_shifter_modules/aws_athena/stix_translation/json/ocsf_from_stix_map.json
+-rw-rw-r--  2.0 unx    75601 b- defN 23-Jul-24 17:41 stix_shifter_modules/aws_athena/stix_translation/json/ocsf_to_stix_map.json
+-rw-rw-r--  2.0 unx      591 b- defN 23-Jul-24 17:41 stix_shifter_modules/aws_athena/stix_translation/json/operators.json
+-rw-rw-r--  2.0 unx      814 b- defN 23-Jul-24 17:41 stix_shifter_modules/aws_athena/stix_translation/json/vpcflow_from_stix_map.json
+-rw-rw-r--  2.0 unx     2350 b- defN 23-Jul-24 17:41 stix_shifter_modules/aws_athena/stix_translation/json/vpcflow_to_stix_map.json
+-rw-rw-r--  2.0 unx     1894 b- defN 23-Jul-24 17:41 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/guardduty_from_stix_map.json
+-rw-rw-r--  2.0 unx    18297 b- defN 23-Jul-24 17:41 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/ocsf_from_stix_map.json
+-rw-rw-r--  2.0 unx    93792 b- defN 23-Jul-24 17:41 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/to_stix_map.json
+-rw-rw-r--  2.0 unx      891 b- defN 23-Jul-24 17:41 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/vpcflow_from_stix_map.json
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jul-24 17:41 stix_shifter_modules/aws_athena/stix_transmission/__init__.py
+-rw-rw-r--  2.0 unx     4173 b- defN 23-Jul-24 17:41 stix_shifter_modules/aws_athena/stix_transmission/boto3_client.py
+-rw-rw-r--  2.0 unx     1207 b- defN 23-Jul-24 17:41 stix_shifter_modules/aws_athena/stix_transmission/delete_connector.py
+-rw-rw-r--  2.0 unx     1959 b- defN 23-Jul-24 17:41 stix_shifter_modules/aws_athena/stix_transmission/error_mapper.py
+-rw-rw-r--  2.0 unx     1370 b- defN 23-Jul-24 17:41 stix_shifter_modules/aws_athena/stix_transmission/ping_connector.py
+-rw-rw-r--  2.0 unx     7443 b- defN 23-Jul-24 17:41 stix_shifter_modules/aws_athena/stix_transmission/query_connector.py
+-rw-rw-r--  2.0 unx    15539 b- defN 23-Jul-24 17:41 stix_shifter_modules/aws_athena/stix_transmission/results_connector.py
+-rw-rw-r--  2.0 unx     3175 b- defN 23-Jul-24 17:41 stix_shifter_modules/aws_athena/stix_transmission/status_connector.py
+-rw-rw-r--  2.0 unx    12786 b- defN 23-Jul-24 17:44 stix_shifter_modules_aws_athena-6.0.1.dist-info/LICENSE.md
+-rw-rw-r--  2.0 unx     7954 b- defN 23-Jul-24 17:44 stix_shifter_modules_aws_athena-6.0.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx     1418 b- defN 23-Jul-24 17:44 stix_shifter_modules_aws_athena-6.0.1.dist-info/NOTICE
+-rw-rw-r--  2.0 unx      110 b- defN 23-Jul-24 17:44 stix_shifter_modules_aws_athena-6.0.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       21 b- defN 23-Jul-24 17:44 stix_shifter_modules_aws_athena-6.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     4691 b- defN 23-Jul-24 17:44 stix_shifter_modules_aws_athena-6.0.1.dist-info/RECORD
+38 files, 593250 bytes uncompressed, 72972 bytes compressed:  87.7%
```

## zipnote {}

```diff
@@ -90,26 +90,26 @@
 
 Filename: stix_shifter_modules/aws_athena/stix_transmission/results_connector.py
 Comment: 
 
 Filename: stix_shifter_modules/aws_athena/stix_transmission/status_connector.py
 Comment: 
 
-Filename: stix_shifter_modules_aws_athena-6.0.0.dev80.dist-info/LICENSE.md
+Filename: stix_shifter_modules_aws_athena-6.0.1.dist-info/LICENSE.md
 Comment: 
 
-Filename: stix_shifter_modules_aws_athena-6.0.0.dev80.dist-info/METADATA
+Filename: stix_shifter_modules_aws_athena-6.0.1.dist-info/METADATA
 Comment: 
 
-Filename: stix_shifter_modules_aws_athena-6.0.0.dev80.dist-info/NOTICE
+Filename: stix_shifter_modules_aws_athena-6.0.1.dist-info/NOTICE
 Comment: 
 
-Filename: stix_shifter_modules_aws_athena-6.0.0.dev80.dist-info/WHEEL
+Filename: stix_shifter_modules_aws_athena-6.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: stix_shifter_modules_aws_athena-6.0.0.dev80.dist-info/top_level.txt
+Filename: stix_shifter_modules_aws_athena-6.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: stix_shifter_modules_aws_athena-6.0.0.dev80.dist-info/RECORD
+Filename: stix_shifter_modules_aws_athena-6.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `stix_shifter_modules_aws_athena-6.0.0.dev80.dist-info/LICENSE.md` & `stix_shifter_modules_aws_athena-6.0.1.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `stix_shifter_modules_aws_athena-6.0.0.dev80.dist-info/METADATA` & `stix_shifter_modules_aws_athena-6.0.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stix-shifter-modules-aws-athena
-Version: 6.0.0.dev80
+Version: 6.0.1
 Summary: Tools and interface to translate STIX formatted results and queries to different data source formats and to set up appropriate connection strings for invoking and triggering actions in openwhisk
 Home-page: https://github.com/opencybersecurityalliance/stix-shifter
 Author: ibm
 Author-email: 
 Project-URL: Source, https://github.com/opencybersecurityalliance/stix-shifter
 Keywords: datasource stix translate transform transmit
 Classifier: License :: OSI Approved :: Apache Software License
@@ -21,15 +21,15 @@
 
 STIX-shifter is an open source python library allowing software to connect to products that house data repositories by using STIX Patterning, and return results as STIX Observations.
 
 This library takes in STIX 2 Patterns as input, and "finds" data that matches the patterns inside various products that house repositories of cybersecurity data. Examples of such products include SIEM systems, endpoint management systems, threat intelligence platforms, orchestration platforms, network control points, data lakes, and more.
 
 In addition to "finding" the data by using these patterns, STIX-Shifter also _transforms the output_ into STIX 2 Observations. Why would we do that you ask? To put it simply - so that all of the security data, regardless of the source, mostly looks and behaves the same.
 
-[## Project Overview and CLI Commands](https://github.com/opencybersecurityalliance/stix-shifter/blob/develop/OVERVIEW.md)
+## Project Overview and CLI Commands
 
 For general information about STIX, this project, and the command line utilities, see the [STIX-shifter Overview](https://github.com/opencybersecurityalliance/stix-shifter/blob/develop/OVERVIEW.md)
 
 
 # Installation
 
 The recommended method for installing stix-shifter is via pip. Two prerequisite packages needs to be installed inlcuding the package of stix-shifter connector module to complete a stix-shifter connector installation. Run the below commands to install all the packages:
```

## Comparing `stix_shifter_modules_aws_athena-6.0.0.dev80.dist-info/NOTICE` & `stix_shifter_modules_aws_athena-6.0.1.dist-info/NOTICE`

 * *Files identical despite different names*

## Comparing `stix_shifter_modules_aws_athena-6.0.0.dev80.dist-info/RECORD` & `stix_shifter_modules_aws_athena-6.0.1.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -26,13 +26,13 @@
 stix_shifter_modules/aws_athena/stix_transmission/boto3_client.py,sha256=4hVUN_O77rghatKexuLOPsTGvzi2fHInpFfgYBuTPkM,4173
 stix_shifter_modules/aws_athena/stix_transmission/delete_connector.py,sha256=D2A5li6TWgZvqpnDGLXVveLqYHlWI1evVWKYKeXT60M,1207
 stix_shifter_modules/aws_athena/stix_transmission/error_mapper.py,sha256=u2IkHTEccByBayyajth6iudtzWy3tIxRDnbpPIX_610,1959
 stix_shifter_modules/aws_athena/stix_transmission/ping_connector.py,sha256=HkcSFvDlW71v6tBtMTcvAd_jQqit6Uh3YknjBu7YKmw,1370
 stix_shifter_modules/aws_athena/stix_transmission/query_connector.py,sha256=eOK6mHRwtASq4gZxOyqmSUvDDThxkDhhbdYQ8jOTweY,7443
 stix_shifter_modules/aws_athena/stix_transmission/results_connector.py,sha256=3J_nfleKOrrSbOGyxDYVxs4qWG1dFWY-qnJBR8jwhZY,15539
 stix_shifter_modules/aws_athena/stix_transmission/status_connector.py,sha256=G-JPjia6t91hGEtvAgImHpoGdO2DNI9ERZB4AAzqf7s,3175
-stix_shifter_modules_aws_athena-6.0.0.dev80.dist-info/LICENSE.md,sha256=ssGEKMVW69oFTBblVhD1YPolqCOyOCJi4wRDRI7xCnU,12786
-stix_shifter_modules_aws_athena-6.0.0.dev80.dist-info/METADATA,sha256=Gn6bJwa_ioQmvWQM8kDlWGwnjYMG4ODvRx4wiY6oZeU,8046
-stix_shifter_modules_aws_athena-6.0.0.dev80.dist-info/NOTICE,sha256=wx-gWE9vSnLJ7YQkrGlMp9VNXOXG57TTxDDRd9CEdYg,1418
-stix_shifter_modules_aws_athena-6.0.0.dev80.dist-info/WHEEL,sha256=k3vXr0c0OitO0k9eCWBlI2yTYnpb_n_I2SGzrrfY7HY,110
-stix_shifter_modules_aws_athena-6.0.0.dev80.dist-info/top_level.txt,sha256=NX-VgUOr8fI-lMXHt3gtjfsEn1UPaGAVszt6Z_CTp2s,21
-stix_shifter_modules_aws_athena-6.0.0.dev80.dist-info/RECORD,,
+stix_shifter_modules_aws_athena-6.0.1.dist-info/LICENSE.md,sha256=ssGEKMVW69oFTBblVhD1YPolqCOyOCJi4wRDRI7xCnU,12786
+stix_shifter_modules_aws_athena-6.0.1.dist-info/METADATA,sha256=k1OxwFWILKxEwn-aQgF3xUB_6eHWhvmirU1x4xHPthM,7954
+stix_shifter_modules_aws_athena-6.0.1.dist-info/NOTICE,sha256=wx-gWE9vSnLJ7YQkrGlMp9VNXOXG57TTxDDRd9CEdYg,1418
+stix_shifter_modules_aws_athena-6.0.1.dist-info/WHEEL,sha256=k3vXr0c0OitO0k9eCWBlI2yTYnpb_n_I2SGzrrfY7HY,110
+stix_shifter_modules_aws_athena-6.0.1.dist-info/top_level.txt,sha256=NX-VgUOr8fI-lMXHt3gtjfsEn1UPaGAVszt6Z_CTp2s,21
+stix_shifter_modules_aws_athena-6.0.1.dist-info/RECORD,,
```

