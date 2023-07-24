# Comparing `tmp/mapped_pb-0.42.8.tar.gz` & `tmp/mapped_pb-0.47.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapped_pb-0.42.8.tar", max compression
+gzip compressed data, was "mapped_pb-0.47.0.tar", max compression
```

## Comparing `mapped_pb-0.42.8.tar` & `mapped_pb-0.47.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       41 2023-06-10 05:47:28.673032 mapped_pb-0.42.8/README.md
--rw-r--r--   0        0        0        0 2023-06-10 05:47:41.665054 mapped_pb-0.42.8/mapped_pb/__init__.py
--rw-r--r--   0        0        0        0 2023-06-10 05:47:41.665054 mapped_pb-0.42.8/mapped_pb/cloud/__init__.py
--rw-r--r--   0        0        0    21055 2023-06-10 05:47:41.665054 mapped_pb-0.42.8/mapped_pb/cloud/types/__init__.py
--rw-r--r--   0        0        0     1540 2023-06-10 05:47:41.665054 mapped_pb-0.42.8/mapped_pb/cloud/types/calendar_period_pb2.py
--rw-r--r--   0        0        0     1377 2023-06-10 05:47:41.665054 mapped_pb-0.42.8/mapped_pb/cloud/types/date_pb2.py
--rw-r--r--   0        0        0     1554 2023-06-10 05:47:41.665054 mapped_pb-0.42.8/mapped_pb/cloud/types/dayofweek_pb2.py
--rw-r--r--   0        0        0     1347 2023-06-10 05:47:41.665054 mapped_pb-0.42.8/mapped_pb/cloud/types/geojson_pb2.py
--rw-r--r--   0        0        0     1546 2023-06-10 05:47:41.665054 mapped_pb-0.42.8/mapped_pb/cloud/types/interval_pb2.py
--rw-r--r--   0        0        0     2209 2023-06-10 05:47:41.665054 mapped_pb-0.42.8/mapped_pb/cloud/types/metadata_pb2.py
--rw-r--r--   0        0        0     1382 2023-06-10 05:47:41.665054 mapped_pb-0.42.8/mapped_pb/cloud/types/money_pb2.py
--rw-r--r--   0        0        0     1629 2023-06-10 05:47:41.665054 mapped_pb-0.42.8/mapped_pb/cloud/types/month_pb2.py
--rw-r--r--   0        0        0     1719 2023-06-10 05:47:41.665054 mapped_pb-0.42.8/mapped_pb/cloud/types/phone_number_pb2.py
--rw-r--r--   0        0        0     1909 2023-06-10 05:47:41.665054 mapped_pb-0.42.8/mapped_pb/cloud/types/postal_address_pb2.py
--rw-r--r--   0        0        0     1484 2023-06-10 05:47:41.665054 mapped_pb-0.42.8/mapped_pb/cloud/types/timeofday_pb2.py
--rw-r--r--   0        0        0     7205 2023-06-10 05:47:41.665054 mapped_pb-0.42.8/mapped_pb/cloud/types/typed_value_pb2.py
--rw-r--r--   0        0        0     6175 2023-06-10 05:47:41.665054 mapped_pb-0.42.8/mapped_pb/gateway/__init__.py
--rw-r--r--   0        0        0     3579 2023-06-10 05:47:41.665054 mapped_pb-0.42.8/mapped_pb/gateway/edgecontrol_pb2.py
--rw-r--r--   0        0        0     1914 2023-06-10 05:47:41.665054 mapped_pb-0.42.8/mapped_pb/gateway/redispoint_pb2.py
--rw-r--r--   0        0        0      616 2023-06-10 05:47:51.729015 mapped_pb-0.42.8/pyproject.toml
--rw-r--r--   0        0        0      799 1970-01-01 00:00:00.000000 mapped_pb-0.42.8/PKG-INFO
+-rw-r--r--   0        0        0       41 2023-07-24 15:59:16.739542 mapped_pb-0.47.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-24 15:59:31.363762 mapped_pb-0.47.0/mapped_pb/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-24 15:59:31.363762 mapped_pb-0.47.0/mapped_pb/cloud/__init__.py
+-rw-r--r--   0        0        0    21055 2023-07-24 15:59:31.363762 mapped_pb-0.47.0/mapped_pb/cloud/types/__init__.py
+-rw-r--r--   0        0        0     1540 2023-07-24 15:59:31.363762 mapped_pb-0.47.0/mapped_pb/cloud/types/calendar_period_pb2.py
+-rw-r--r--   0        0        0     1377 2023-07-24 15:59:31.363762 mapped_pb-0.47.0/mapped_pb/cloud/types/date_pb2.py
+-rw-r--r--   0        0        0     1554 2023-07-24 15:59:31.363762 mapped_pb-0.47.0/mapped_pb/cloud/types/dayofweek_pb2.py
+-rw-r--r--   0        0        0     1347 2023-07-24 15:59:31.363762 mapped_pb-0.47.0/mapped_pb/cloud/types/geojson_pb2.py
+-rw-r--r--   0        0        0     1546 2023-07-24 15:59:31.363762 mapped_pb-0.47.0/mapped_pb/cloud/types/interval_pb2.py
+-rw-r--r--   0        0        0     2209 2023-07-24 15:59:31.363762 mapped_pb-0.47.0/mapped_pb/cloud/types/metadata_pb2.py
+-rw-r--r--   0        0        0     1382 2023-07-24 15:59:31.363762 mapped_pb-0.47.0/mapped_pb/cloud/types/money_pb2.py
+-rw-r--r--   0        0        0     1629 2023-07-24 15:59:31.363762 mapped_pb-0.47.0/mapped_pb/cloud/types/month_pb2.py
+-rw-r--r--   0        0        0     1719 2023-07-24 15:59:31.363762 mapped_pb-0.47.0/mapped_pb/cloud/types/phone_number_pb2.py
+-rw-r--r--   0        0        0     1909 2023-07-24 15:59:31.363762 mapped_pb-0.47.0/mapped_pb/cloud/types/postal_address_pb2.py
+-rw-r--r--   0        0        0     1484 2023-07-24 15:59:31.363762 mapped_pb-0.47.0/mapped_pb/cloud/types/timeofday_pb2.py
+-rw-r--r--   0        0        0     7205 2023-07-24 15:59:31.363762 mapped_pb-0.47.0/mapped_pb/cloud/types/typed_value_pb2.py
+-rw-r--r--   0        0        0     6175 2023-07-24 15:59:31.363762 mapped_pb-0.47.0/mapped_pb/gateway/__init__.py
+-rw-r--r--   0        0        0     3579 2023-07-24 15:59:31.363762 mapped_pb-0.47.0/mapped_pb/gateway/edgecontrol_pb2.py
+-rw-r--r--   0        0        0     1914 2023-07-24 15:59:31.363762 mapped_pb-0.47.0/mapped_pb/gateway/redispoint_pb2.py
+-rw-r--r--   0        0        0      616 2023-07-24 15:59:43.211941 mapped_pb-0.47.0/pyproject.toml
+-rw-r--r--   0        0        0      799 1970-01-01 00:00:00.000000 mapped_pb-0.47.0/PKG-INFO
```

### Comparing `mapped_pb-0.42.8/mapped_pb/cloud/types/__init__.py` & `mapped_pb-0.47.0/mapped_pb/cloud/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mapped_pb-0.42.8/mapped_pb/cloud/types/calendar_period_pb2.py` & `mapped_pb-0.47.0/mapped_pb/cloud/types/calendar_period_pb2.py`

 * *Files identical despite different names*

### Comparing `mapped_pb-0.42.8/mapped_pb/cloud/types/date_pb2.py` & `mapped_pb-0.47.0/mapped_pb/cloud/types/date_pb2.py`

 * *Files identical despite different names*

### Comparing `mapped_pb-0.42.8/mapped_pb/cloud/types/dayofweek_pb2.py` & `mapped_pb-0.47.0/mapped_pb/cloud/types/dayofweek_pb2.py`

 * *Files identical despite different names*

### Comparing `mapped_pb-0.42.8/mapped_pb/cloud/types/geojson_pb2.py` & `mapped_pb-0.47.0/mapped_pb/cloud/types/geojson_pb2.py`

 * *Files identical despite different names*

### Comparing `mapped_pb-0.42.8/mapped_pb/cloud/types/interval_pb2.py` & `mapped_pb-0.47.0/mapped_pb/cloud/types/interval_pb2.py`

 * *Files identical despite different names*

### Comparing `mapped_pb-0.42.8/mapped_pb/cloud/types/metadata_pb2.py` & `mapped_pb-0.47.0/mapped_pb/cloud/types/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `mapped_pb-0.42.8/mapped_pb/cloud/types/money_pb2.py` & `mapped_pb-0.47.0/mapped_pb/cloud/types/money_pb2.py`

 * *Files identical despite different names*

### Comparing `mapped_pb-0.42.8/mapped_pb/cloud/types/month_pb2.py` & `mapped_pb-0.47.0/mapped_pb/cloud/types/month_pb2.py`

 * *Files identical despite different names*

### Comparing `mapped_pb-0.42.8/mapped_pb/cloud/types/phone_number_pb2.py` & `mapped_pb-0.47.0/mapped_pb/cloud/types/phone_number_pb2.py`

 * *Files identical despite different names*

### Comparing `mapped_pb-0.42.8/mapped_pb/cloud/types/postal_address_pb2.py` & `mapped_pb-0.47.0/mapped_pb/cloud/types/postal_address_pb2.py`

 * *Files identical despite different names*

### Comparing `mapped_pb-0.42.8/mapped_pb/cloud/types/timeofday_pb2.py` & `mapped_pb-0.47.0/mapped_pb/cloud/types/timeofday_pb2.py`

 * *Files identical despite different names*

### Comparing `mapped_pb-0.42.8/mapped_pb/cloud/types/typed_value_pb2.py` & `mapped_pb-0.47.0/mapped_pb/cloud/types/typed_value_pb2.py`

 * *Files identical despite different names*

### Comparing `mapped_pb-0.42.8/mapped_pb/gateway/__init__.py` & `mapped_pb-0.47.0/mapped_pb/gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `mapped_pb-0.42.8/mapped_pb/gateway/edgecontrol_pb2.py` & `mapped_pb-0.47.0/mapped_pb/gateway/edgecontrol_pb2.py`

 * *Files identical despite different names*

### Comparing `mapped_pb-0.42.8/mapped_pb/gateway/redispoint_pb2.py` & `mapped_pb-0.47.0/mapped_pb/gateway/redispoint_pb2.py`

 * *Files identical despite different names*

### Comparing `mapped_pb-0.42.8/pyproject.toml` & `mapped_pb-0.47.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mapped.pb"
-version = "0.42.8"
+version = "0.47.0"
 description = "public Mapped Platform Service Definitions using protobuf"
 authors = ["Mapped <support@mapped.com>"]
 license = "Apache-2.0"
 homepage = "https://www.mapped.com"
 repository = "https://github.com/mapped/pb"
 keywords = ["mapped", "protobuf"]
 readme = "README.md"
```

### Comparing `mapped_pb-0.42.8/PKG-INFO` & `mapped_pb-0.47.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapped-pb
-Version: 0.42.8
+Version: 0.47.0
 Summary: public Mapped Platform Service Definitions using protobuf
 Home-page: https://www.mapped.com
 License: Apache-2.0
 Keywords: mapped,protobuf
 Author: Mapped
 Author-email: support@mapped.com
 Requires-Python: >=3.8,<4.0
```

