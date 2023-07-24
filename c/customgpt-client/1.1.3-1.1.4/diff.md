# Comparing `tmp/customgpt_client-1.1.3-py3-none-any.whl.zip` & `tmp/customgpt_client-1.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 404484 bytes, number of entries: 505
+Zip file size: 404494 bytes, number of entries: 505
 -rw-r--r--  2.0 unx      105 b- defN 80-Jan-01 00:00 customgpt_client/__init__.py
 -rw-r--r--  2.0 unx       47 b- defN 80-Jan-01 00:00 customgpt_client/api/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 customgpt_client/api/citations/__init__.py
 -rw-r--r--  2.0 unx     5868 b- defN 80-Jan-01 00:00 customgpt_client/api/citations/get_open_graph_data_for_citation.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 customgpt_client/api/conversations/__init__.py
 -rw-r--r--  2.0 unx     6697 b- defN 80-Jan-01 00:00 customgpt_client/api/conversations/create_project_conversation.py
 -rw-r--r--  2.0 unx     6332 b- defN 80-Jan-01 00:00 customgpt_client/api/conversations/delete_project_conversation.py
@@ -497,11 +497,11 @@
 -rw-r--r--  2.0 unx     3168 b- defN 80-Jan-01 00:00 customgpt_client/models/update_user_profile_response_500.py
 -rw-r--r--  2.0 unx     2330 b- defN 80-Jan-01 00:00 customgpt_client/models/update_user_profile_response_500_data.py
 -rw-r--r--  2.0 unx      262 b- defN 80-Jan-01 00:00 customgpt_client/models/update_user_profile_response_500_data_code.py
 -rw-r--r--  2.0 unx      183 b- defN 80-Jan-01 00:00 customgpt_client/models/update_user_profile_response_500_status.py
 -rw-r--r--  2.0 unx     3770 b- defN 80-Jan-01 00:00 customgpt_client/models/user.py
 -rw-r--r--  2.0 unx       25 b- defN 80-Jan-01 00:00 customgpt_client/py.typed
 -rw-r--r--  2.0 unx      993 b- defN 80-Jan-01 00:00 customgpt_client/types.py
--rw-r--r--  2.0 unx     1224 b- defN 80-Jan-01 00:00 customgpt_client-1.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 customgpt_client-1.1.3.dist-info/WHEEL
-?rw-r--r--  2.0 unx    60483 b- defN 16-Jan-01 00:00 customgpt_client-1.1.3.dist-info/RECORD
-505 files, 1144978 bytes uncompressed, 302066 bytes compressed:  73.6%
+-rw-r--r--  2.0 unx     1259 b- defN 80-Jan-01 00:00 customgpt_client-1.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 customgpt_client-1.1.4.dist-info/WHEEL
+?rw-r--r--  2.0 unx    60483 b- defN 16-Jan-01 00:00 customgpt_client-1.1.4.dist-info/RECORD
+505 files, 1145013 bytes uncompressed, 302076 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -1500,17 +1500,17 @@
 
 Filename: customgpt_client/py.typed
 Comment: 
 
 Filename: customgpt_client/types.py
 Comment: 
 
-Filename: customgpt_client-1.1.3.dist-info/METADATA
+Filename: customgpt_client-1.1.4.dist-info/METADATA
 Comment: 
 
-Filename: customgpt_client-1.1.3.dist-info/WHEEL
+Filename: customgpt_client-1.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: customgpt_client-1.1.3.dist-info/RECORD
+Filename: customgpt_client-1.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `customgpt_client-1.1.3.dist-info/METADATA` & `customgpt_client-1.1.4.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: customgpt-client
-Version: 1.1.3
+Version: 1.1.4
 Summary: A client library for accessing customgpt
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: attrs (>=21.3.0)
 Requires-Dist: python-dateutil (>=2.8.0,<3.0.0)
+Requires-Dist: requests (==2.31.0)
 Requires-Dist: sseclient-py (==1.7.2)
 Description-Content-Type: text/markdown
 
 # CustomGPT SDK
 
 ## Usage
 First, create a client:
```

## Comparing `customgpt_client-1.1.3.dist-info/RECORD` & `customgpt_client-1.1.4.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -496,10 +496,10 @@
 customgpt_client/models/update_user_profile_response_500.py,sha256=DFB1mxDP5sTW90072fG8quTkEIv2VwreJEvDMqwZSJI,3168
 customgpt_client/models/update_user_profile_response_500_data.py,sha256=qQ42Uw6yxVZu6a5X7AdlL2nIH-yIMbIZfFo7FPNmFQ0,2330
 customgpt_client/models/update_user_profile_response_500_data_code.py,sha256=o-GDpigGzvI3qFGG1HstdR5Lx5p508fuGNvkauwP9s8,262
 customgpt_client/models/update_user_profile_response_500_status.py,sha256=sX5mpQWL7wNrEpdCiSpvQgsm1f6kaNvLlPmfSkzW-I8,183
 customgpt_client/models/user.py,sha256=mgFRGG_RaO2qScwDVy9Lw-LzKPtkvfyIbrumqE42T74,3770
 customgpt_client/py.typed,sha256=8ZJUsxZiuOy1oJeVhsTWQhTG_6pTVHVXk5hJL79ebTk,25
 customgpt_client/types.py,sha256=4xaUIOliefW-5jz_p-JT2LO7-V0wKWaniHGtjPBQfvQ,993
-customgpt_client-1.1.3.dist-info/METADATA,sha256=-CrUglvh4ybAvOMveIiwHvYHZbOW418ZmfTA4LDyAmk,1224
-customgpt_client-1.1.3.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-customgpt_client-1.1.3.dist-info/RECORD,,
+customgpt_client-1.1.4.dist-info/METADATA,sha256=Karodwq0oG7lX6yD2hPUof37durLUZqclMvat5UXabw,1259
+customgpt_client-1.1.4.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+customgpt_client-1.1.4.dist-info/RECORD,,
```

