# Comparing `tmp/bizlogic-0.2.6.tar.gz` & `tmp/bizlogic-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bizlogic-0.2.6.tar", max compression
+gzip compressed data, was "bizlogic-0.2.7.tar", max compression
```

## Comparing `bizlogic-0.2.6.tar` & `bizlogic-0.2.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1211 2023-04-20 00:41:45.427991 bizlogic-0.2.6/LICENSE
--rw-r--r--   0        0        0     2182 2023-05-15 17:30:35.537449 bizlogic-0.2.6/README.md
--rw-r--r--   0        0        0      341 2023-07-22 13:43:19.828316 bizlogic-0.2.6/bizlogic/__init__.py
--rw-r--r--   0        0        0     5923 2023-05-15 17:30:35.537815 bizlogic-0.2.6/bizlogic/application.py
--rw-r--r--   0        0        0       61 2023-04-23 15:36:06.068712 bizlogic-0.2.6/bizlogic/loan/__init__.py
--rw-r--r--   0        0        0     7709 2023-07-22 13:43:02.033455 bizlogic-0.2.6/bizlogic/loan/reader.py
--rw-r--r--   0        0        0     2742 2023-07-22 13:03:29.399551 bizlogic-0.2.6/bizlogic/loan/repayment.py
--rw-r--r--   0        0        0     1136 2023-07-22 13:03:29.400196 bizlogic-0.2.6/bizlogic/loan/status.py
--rw-r--r--   0        0        0     4269 2023-05-15 17:30:35.538679 bizlogic-0.2.6/bizlogic/loan/writer.py
--rw-r--r--   0        0        0       48 2023-04-23 15:35:52.968443 bizlogic-0.2.6/bizlogic/protoc/__init__.py
--rw-r--r--   0        0        0     1053 2023-05-15 17:30:35.538935 bizlogic-0.2.6/bizlogic/protoc/loan_application_pb2.py
--rw-r--r--   0        0        0     1709 2023-05-14 16:41:31.172854 bizlogic-0.2.6/bizlogic/protoc/loan_pb2.py
--rw-r--r--   0        0        0      952 2023-05-15 17:30:35.539315 bizlogic-0.2.6/bizlogic/protoc/vouch_pb2.py
--rw-r--r--   0        0        0     3462 2023-07-22 13:03:29.401263 bizlogic-0.2.6/bizlogic/utils.py
--rw-r--r--   0        0        0     4165 2023-05-15 17:30:35.539612 bizlogic-0.2.6/bizlogic/vouch.py
--rw-r--r--   0        0        0      451 2023-07-22 13:43:23.860164 bizlogic-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     2715 1970-01-01 00:00:00.000000 bizlogic-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-20 00:41:45.427991 bizlogic-0.2.7/LICENSE
+-rw-r--r--   0        0        0     2182 2023-05-15 17:30:35.537449 bizlogic-0.2.7/README.md
+-rw-r--r--   0        0        0      341 2023-07-24 16:26:12.085176 bizlogic-0.2.7/bizlogic/__init__.py
+-rw-r--r--   0        0        0     5923 2023-05-15 17:30:35.537815 bizlogic-0.2.7/bizlogic/application.py
+-rw-r--r--   0        0        0       61 2023-04-23 15:36:06.068712 bizlogic-0.2.7/bizlogic/loan/__init__.py
+-rw-r--r--   0        0        0     7709 2023-07-22 13:43:02.033455 bizlogic-0.2.7/bizlogic/loan/reader.py
+-rw-r--r--   0        0        0     2742 2023-07-22 13:03:29.399551 bizlogic-0.2.7/bizlogic/loan/repayment.py
+-rw-r--r--   0        0        0     1094 2023-07-24 16:25:36.776214 bizlogic-0.2.7/bizlogic/loan/status.py
+-rw-r--r--   0        0        0     4269 2023-05-15 17:30:35.538679 bizlogic-0.2.7/bizlogic/loan/writer.py
+-rw-r--r--   0        0        0       48 2023-04-23 15:35:52.968443 bizlogic-0.2.7/bizlogic/protoc/__init__.py
+-rw-r--r--   0        0        0     1053 2023-05-15 17:30:35.538935 bizlogic-0.2.7/bizlogic/protoc/loan_application_pb2.py
+-rw-r--r--   0        0        0     1709 2023-05-14 16:41:31.172854 bizlogic-0.2.7/bizlogic/protoc/loan_pb2.py
+-rw-r--r--   0        0        0      952 2023-05-15 17:30:35.539315 bizlogic-0.2.7/bizlogic/protoc/vouch_pb2.py
+-rw-r--r--   0        0        0     3462 2023-07-22 13:03:29.401263 bizlogic-0.2.7/bizlogic/utils.py
+-rw-r--r--   0        0        0     4165 2023-05-15 17:30:35.539612 bizlogic-0.2.7/bizlogic/vouch.py
+-rw-r--r--   0        0        0      451 2023-07-24 16:26:04.501091 bizlogic-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     2715 1970-01-01 00:00:00.000000 bizlogic-0.2.7/PKG-INFO
```

### Comparing `bizlogic-0.2.6/LICENSE` & `bizlogic-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.6/README.md` & `bizlogic-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.6/bizlogic/application.py` & `bizlogic-0.2.7/bizlogic/application.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.6/bizlogic/loan/reader.py` & `bizlogic-0.2.7/bizlogic/loan/reader.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.6/bizlogic/loan/repayment.py` & `bizlogic-0.2.7/bizlogic/loan/repayment.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.6/bizlogic/loan/status.py` & `bizlogic-0.2.7/bizlogic/loan/status.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-from datetime import datetime, timedelta
+from datetime import datetime, timezone
 from enum import Enum
 
 from bizlogic.protoc.loan_pb2 import Loan
 
-from google.protobuf.timestamp_pb2 import Timestamp
-
 
 class LoanStatusType(Enum):
     """Loan Status Type."""
 
     PENDING_ACCEPTANCE = 1
     EXPIRED_UNACCEPTED = 2
     ACCEPTED = 3
@@ -23,15 +21,15 @@
 
         Args:
             loan: the loan
 
         Returns:
             LoanStatusType: the status of the loan
         """
-        now = datetime.now()
+        now = datetime.now(timezone.utc)
 
         # if the loan has not expired and is not accepted
         if loan['offer_expiry'] > now and not loan['accepted']:
             return LoanStatusType.PENDING_ACCEPTANCE
 
         # if the loan has expired and is not accepted
         elif loan['offer_expiry'] <= now and not loan['accepted']:
```

### Comparing `bizlogic-0.2.6/bizlogic/loan/writer.py` & `bizlogic-0.2.7/bizlogic/loan/writer.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.6/bizlogic/protoc/loan_application_pb2.py` & `bizlogic-0.2.7/bizlogic/protoc/loan_application_pb2.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.6/bizlogic/protoc/loan_pb2.py` & `bizlogic-0.2.7/bizlogic/protoc/loan_pb2.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.6/bizlogic/protoc/vouch_pb2.py` & `bizlogic-0.2.7/bizlogic/protoc/vouch_pb2.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.6/bizlogic/utils.py` & `bizlogic-0.2.7/bizlogic/utils.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.6/bizlogic/vouch.py` & `bizlogic-0.2.7/bizlogic/vouch.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.6/PKG-INFO` & `bizlogic-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bizlogic
-Version: 0.2.6
+Version: 0.2.7
 Summary: web3 lending platform business logic
 Author: Nate Schultz
 Author-email: nate.schultz@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ipfsclient (==0.0.7)
```

