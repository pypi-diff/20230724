# Comparing `tmp/bizlogic-0.2.7.tar.gz` & `tmp/bizlogic-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bizlogic-0.2.7.tar", max compression
+gzip compressed data, was "bizlogic-0.2.8.tar", max compression
```

## Comparing `bizlogic-0.2.7.tar` & `bizlogic-0.2.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1211 2023-04-20 00:41:45.427991 bizlogic-0.2.7/LICENSE
--rw-r--r--   0        0        0     2182 2023-05-15 17:30:35.537449 bizlogic-0.2.7/README.md
--rw-r--r--   0        0        0      341 2023-07-24 16:26:12.085176 bizlogic-0.2.7/bizlogic/__init__.py
--rw-r--r--   0        0        0     5923 2023-05-15 17:30:35.537815 bizlogic-0.2.7/bizlogic/application.py
--rw-r--r--   0        0        0       61 2023-04-23 15:36:06.068712 bizlogic-0.2.7/bizlogic/loan/__init__.py
--rw-r--r--   0        0        0     7709 2023-07-22 13:43:02.033455 bizlogic-0.2.7/bizlogic/loan/reader.py
--rw-r--r--   0        0        0     2742 2023-07-22 13:03:29.399551 bizlogic-0.2.7/bizlogic/loan/repayment.py
--rw-r--r--   0        0        0     1094 2023-07-24 16:25:36.776214 bizlogic-0.2.7/bizlogic/loan/status.py
--rw-r--r--   0        0        0     4269 2023-05-15 17:30:35.538679 bizlogic-0.2.7/bizlogic/loan/writer.py
--rw-r--r--   0        0        0       48 2023-04-23 15:35:52.968443 bizlogic-0.2.7/bizlogic/protoc/__init__.py
--rw-r--r--   0        0        0     1053 2023-05-15 17:30:35.538935 bizlogic-0.2.7/bizlogic/protoc/loan_application_pb2.py
--rw-r--r--   0        0        0     1709 2023-05-14 16:41:31.172854 bizlogic-0.2.7/bizlogic/protoc/loan_pb2.py
--rw-r--r--   0        0        0      952 2023-05-15 17:30:35.539315 bizlogic-0.2.7/bizlogic/protoc/vouch_pb2.py
--rw-r--r--   0        0        0     3462 2023-07-22 13:03:29.401263 bizlogic-0.2.7/bizlogic/utils.py
--rw-r--r--   0        0        0     4165 2023-05-15 17:30:35.539612 bizlogic-0.2.7/bizlogic/vouch.py
--rw-r--r--   0        0        0      451 2023-07-24 16:26:04.501091 bizlogic-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     2715 1970-01-01 00:00:00.000000 bizlogic-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-20 00:41:45.427991 bizlogic-0.2.8/LICENSE
+-rw-r--r--   0        0        0     2182 2023-05-15 17:30:35.537449 bizlogic-0.2.8/README.md
+-rw-r--r--   0        0        0      341 2023-07-24 17:35:42.596923 bizlogic-0.2.8/bizlogic/__init__.py
+-rw-r--r--   0        0        0     5923 2023-05-15 17:30:35.537815 bizlogic-0.2.8/bizlogic/application.py
+-rw-r--r--   0        0        0       61 2023-04-23 15:36:06.068712 bizlogic-0.2.8/bizlogic/loan/__init__.py
+-rw-r--r--   0        0        0     7709 2023-07-24 16:57:55.056690 bizlogic-0.2.8/bizlogic/loan/reader.py
+-rw-r--r--   0        0        0     2742 2023-07-22 13:03:29.399551 bizlogic-0.2.8/bizlogic/loan/repayment.py
+-rw-r--r--   0        0        0     1094 2023-07-24 16:57:55.056841 bizlogic-0.2.8/bizlogic/loan/status.py
+-rw-r--r--   0        0        0     4269 2023-05-15 17:30:35.538679 bizlogic-0.2.8/bizlogic/loan/writer.py
+-rw-r--r--   0        0        0       48 2023-04-23 15:35:52.968443 bizlogic-0.2.8/bizlogic/protoc/__init__.py
+-rw-r--r--   0        0        0     1053 2023-05-15 17:30:35.538935 bizlogic-0.2.8/bizlogic/protoc/loan_application_pb2.py
+-rw-r--r--   0        0        0     1709 2023-05-14 16:41:31.172854 bizlogic-0.2.8/bizlogic/protoc/loan_pb2.py
+-rw-r--r--   0        0        0      952 2023-05-15 17:30:35.539315 bizlogic-0.2.8/bizlogic/protoc/vouch_pb2.py
+-rw-r--r--   0        0        0     3514 2023-07-24 17:36:44.053400 bizlogic-0.2.8/bizlogic/utils.py
+-rw-r--r--   0        0        0     4165 2023-05-15 17:30:35.539612 bizlogic-0.2.8/bizlogic/vouch.py
+-rw-r--r--   0        0        0      451 2023-07-24 17:35:30.592732 bizlogic-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     2715 1970-01-01 00:00:00.000000 bizlogic-0.2.8/PKG-INFO
```

### Comparing `bizlogic-0.2.7/LICENSE` & `bizlogic-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.7/README.md` & `bizlogic-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.7/bizlogic/application.py` & `bizlogic-0.2.8/bizlogic/application.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.7/bizlogic/loan/reader.py` & `bizlogic-0.2.8/bizlogic/loan/reader.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.7/bizlogic/loan/repayment.py` & `bizlogic-0.2.8/bizlogic/loan/repayment.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.7/bizlogic/loan/status.py` & `bizlogic-0.2.8/bizlogic/loan/status.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.7/bizlogic/loan/writer.py` & `bizlogic-0.2.8/bizlogic/loan/writer.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.7/bizlogic/protoc/loan_application_pb2.py` & `bizlogic-0.2.8/bizlogic/protoc/loan_application_pb2.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.7/bizlogic/protoc/loan_pb2.py` & `bizlogic-0.2.8/bizlogic/protoc/loan_pb2.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.7/bizlogic/protoc/vouch_pb2.py` & `bizlogic-0.2.8/bizlogic/protoc/vouch_pb2.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.7/bizlogic/utils.py` & `bizlogic-0.2.8/bizlogic/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import datetime
+import pytz
 
 from ipfskvs.store import Store
 
 import pandas as pd
 
 import logging
 
@@ -76,26 +77,27 @@
         df = df.sort_values('created').groupby(
             group_by, as_index=False
         ).last()
 
         return df
 
     @staticmethod
-    def parse_offer_expiry(store: Store) -> datetime.date:
+    def parse_offer_expiry(store: Store) -> datetime.datetime:
         """Get the offer expiry timestamp as a datetime.
 
         Args:
             store (Store): The store object to parse
 
         Returns:
-            datetime.date: The offer expiry
+            datetime: The offer expiry in UTC timezone
         """
         LOG.debug(f"Parsing: {store.reader}")
         return datetime.datetime.fromtimestamp(
-            store.reader.offer_expiry.seconds + store.reader.offer_expiry.nanos / 1e9  # noqa: E501
+            store.reader.offer_expiry.seconds + store.reader.offer_expiry.nanos / 1e9,  # noqa: E501
+            tz=pytz.UTC
         )
 
 
 PARSERS = {
     ParserType.LOAN_APPLICATION: {
         "amount_asking": lambda store: store.reader.amount_asking,
         "closed": lambda store: store.reader.closed,
```

### Comparing `bizlogic-0.2.7/bizlogic/vouch.py` & `bizlogic-0.2.8/bizlogic/vouch.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.7/PKG-INFO` & `bizlogic-0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bizlogic
-Version: 0.2.7
+Version: 0.2.8
 Summary: web3 lending platform business logic
 Author: Nate Schultz
 Author-email: nate.schultz@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ipfsclient (==0.0.7)
```

