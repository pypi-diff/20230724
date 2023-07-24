# Comparing `tmp/aliyun-python-sdk-eipanycast-1.0.4.tar.gz` & `tmp/aliyun-python-sdk-eipanycast-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-eipanycast-1.0.4.tar", last modified: Fri Jun  9 04:50:47 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-eipanycast-1.0.5.tar", last modified: Mon Jul 24 07:28:28 2023, max compression
```

## Comparing `aliyun-python-sdk-eipanycast-1.0.4.tar` & `aliyun-python-sdk-eipanycast-1.0.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:50:47.000000 aliyun-python-sdk-eipanycast-1.0.4/
--rw-r--r--   0 root         (0) root         (0)      575 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1572 2023-06-09 04:50:47.000000 aliyun-python-sdk-eipanycast-1.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      541 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:50:47.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyun_python_sdk_eipanycast.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1572 2023-06-09 04:50:47.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyun_python_sdk_eipanycast.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1490 2023-06-09 04:50:47.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyun_python_sdk_eipanycast.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 04:50:47.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyun_python_sdk_eipanycast.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-06-09 04:50:47.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyun_python_sdk_eipanycast.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-06-09 04:50:47.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyun_python_sdk_eipanycast.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:50:47.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1088 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:50:47.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:50:47.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/
--rw-r--r--   0 root         (0) root         (0)     2733 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/AllocateAnycastEipAddressRequest.py
--rw-r--r--   0 root         (0) root         (0)     3342 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/AssociateAnycastEipAddressRequest.py
--rw-r--r--   0 root         (0) root         (0)     1843 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/DescribeAnycastEipAddressRequest.py
--rw-r--r--   0 root         (0) root         (0)     1525 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/DescribeAnycastPopLocationsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1527 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/DescribeAnycastServerRegionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     4333 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/ListAnycastEipAddressesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2550 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/ListTagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1851 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/ModifyAnycastEipAddressAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/ModifyAnycastEipAddressSpecRequest.py
--rw-r--r--   0 root         (0) root         (0)     1680 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/ReleaseAnycastEipAddressRequest.py
--rw-r--r--   0 root         (0) root         (0)     2166 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/TagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2775 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/UnassociateAnycastEipAddressRequest.py
--rw-r--r--   0 root         (0) root         (0)     1993 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/UntagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3093 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/UpdateAnycastEipAddressAssociationsRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-06-09 04:50:47.000000 aliyun-python-sdk-eipanycast-1.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2487 2023-06-09 04:50:46.000000 aliyun-python-sdk-eipanycast-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:28:28.000000 aliyun-python-sdk-eipanycast-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-07-24 07:28:28.000000 aliyun-python-sdk-eipanycast-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-07-24 07:28:28.000000 aliyun-python-sdk-eipanycast-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1572 2023-07-24 07:28:28.000000 aliyun-python-sdk-eipanycast-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      541 2023-07-24 07:28:28.000000 aliyun-python-sdk-eipanycast-1.0.5/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:28:28.000000 aliyun-python-sdk-eipanycast-1.0.5/aliyun_python_sdk_eipanycast.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1572 2023-07-24 07:28:28.000000 aliyun-python-sdk-eipanycast-1.0.5/aliyun_python_sdk_eipanycast.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-07-24 07:28:28.000000 aliyun-python-sdk-eipanycast-1.0.5/aliyun_python_sdk_eipanycast.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 07:28:28.000000 aliyun-python-sdk-eipanycast-1.0.5/aliyun_python_sdk_eipanycast.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-07-24 07:28:28.000000 aliyun-python-sdk-eipanycast-1.0.5/aliyun_python_sdk_eipanycast.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-24 07:28:28.000000 aliyun-python-sdk-eipanycast-1.0.5/aliyun_python_sdk_eipanycast.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:28:28.000000 aliyun-python-sdk-eipanycast-1.0.5/aliyunsdkeipanycast/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-24 07:28:28.000000 aliyun-python-sdk-eipanycast-1.0.5/aliyunsdkeipanycast/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-07-24 07:28:28.000000 aliyun-python-sdk-eipanycast-1.0.5/aliyunsdkeipanycast/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:28:28.000000 aliyun-python-sdk-eipanycast-1.0.5/aliyunsdkeipanycast/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 07:28:28.000000 aliyun-python-sdk-eipanycast-1.0.5/aliyunsdkeipanycast/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:28:28.000000 aliyun-python-sdk-eipanycast-1.0.5/aliyunsdkeipanycast/request/v20200309/
+-rw-r--r--   0 root         (0) root         (0)     2967 2023-07-24 07:28:28.000000 aliyun-python-sdk-eipanycast-1.0.5/aliyunsdkeipanycast/request/v20200309/AllocateAnycastEipAddressRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3355 2023-07-24 07:28:28.000000 aliyun-python-sdk-eipanycast-1.0.5/aliyunsdkeipanycast/request/v20200309/AssociateAnycastEipAddressRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1856 2023-07-24 07:28:28.000000 aliyun-python-sdk-eipanycast-1.0.5/aliyunsdkeipanycast/request/v20200309/DescribeAnycastEipAddressRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1538 2023-07-24 07:28:28.000000 aliyun-python-sdk-eipanycast-1.0.5/aliyunsdkeipanycast/request/v20200309/DescribeAnycastPopLocationsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1540 2023-07-24 07:28:28.000000 aliyun-python-sdk-eipanycast-1.0.5/aliyunsdkeipanycast/request/v20200309/DescribeAnycastServerRegionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4567 2023-07-24 07:28:28.000000 aliyun-python-sdk-eipanycast-1.0.5/aliyunsdkeipanycast/request/v20200309/ListAnycastEipAddressesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2563 2023-07-24 07:28:28.000000 aliyun-python-sdk-eipanycast-1.0.5/aliyunsdkeipanycast/request/v20200309/ListTagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2023-07-24 07:28:28.000000 aliyun-python-sdk-eipanycast-1.0.5/aliyunsdkeipanycast/request/v20200309/ModifyAnycastEipAddressAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1687 2023-07-24 07:28:28.000000 aliyun-python-sdk-eipanycast-1.0.5/aliyunsdkeipanycast/request/v20200309/ModifyAnycastEipAddressSpecRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1693 2023-07-24 07:28:28.000000 aliyun-python-sdk-eipanycast-1.0.5/aliyunsdkeipanycast/request/v20200309/ReleaseAnycastEipAddressRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2179 2023-07-24 07:28:28.000000 aliyun-python-sdk-eipanycast-1.0.5/aliyunsdkeipanycast/request/v20200309/TagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2788 2023-07-24 07:28:28.000000 aliyun-python-sdk-eipanycast-1.0.5/aliyunsdkeipanycast/request/v20200309/UnassociateAnycastEipAddressRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2006 2023-07-24 07:28:28.000000 aliyun-python-sdk-eipanycast-1.0.5/aliyunsdkeipanycast/request/v20200309/UntagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3106 2023-07-24 07:28:28.000000 aliyun-python-sdk-eipanycast-1.0.5/aliyunsdkeipanycast/request/v20200309/UpdateAnycastEipAddressAssociationsRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 07:28:28.000000 aliyun-python-sdk-eipanycast-1.0.5/aliyunsdkeipanycast/request/v20200309/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-07-24 07:28:28.000000 aliyun-python-sdk-eipanycast-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2487 2023-07-24 07:28:28.000000 aliyun-python-sdk-eipanycast-1.0.5/setup.py
```

### Comparing `aliyun-python-sdk-eipanycast-1.0.4/LICENSE` & `aliyun-python-sdk-eipanycast-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eipanycast-1.0.4/PKG-INFO` & `aliyun-python-sdk-eipanycast-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-eipanycast
-Version: 1.0.4
+Version: 1.0.5
 Summary: The eipanycast module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-eipanycast
```

### Comparing `aliyun-python-sdk-eipanycast-1.0.4/README.rst` & `aliyun-python-sdk-eipanycast-1.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eipanycast-1.0.4/aliyun_python_sdk_eipanycast.egg-info/PKG-INFO` & `aliyun-python-sdk-eipanycast-1.0.5/aliyun_python_sdk_eipanycast.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-eipanycast
-Version: 1.0.4
+Version: 1.0.5
 Summary: The eipanycast module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-eipanycast
```

### Comparing `aliyun-python-sdk-eipanycast-1.0.4/aliyun_python_sdk_eipanycast.egg-info/SOURCES.txt` & `aliyun-python-sdk-eipanycast-1.0.5/aliyun_python_sdk_eipanycast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/endpoint.py` & `aliyun-python-sdk-eipanycast-1.0.5/aliyunsdkeipanycast/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/AllocateAnycastEipAddressRequest.py` & `aliyun-python-sdk-eipanycast-1.0.5/aliyunsdkeipanycast/request/v20200309/AllocateAnycastEipAddressRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkeipanycast.endpoint import endpoint_data
 
 class AllocateAnycastEipAddressRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'AllocateAnycastEipAddress')
+		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'AllocateAnycastEipAddress','eipanycast')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
@@ -47,14 +47,19 @@
 	def set_ClientToken(self, ClientToken):  # String
 		self.add_query_param('ClientToken', ClientToken)
 	def get_Description(self): # String
 		return self.get_query_params().get('Description')
 
 	def set_Description(self, Description):  # String
 		self.add_query_param('Description', Description)
+	def get_ResourceGroupId(self): # String
+		return self.get_query_params().get('ResourceGroupId')
+
+	def set_ResourceGroupId(self, ResourceGroupId):  # String
+		self.add_query_param('ResourceGroupId', ResourceGroupId)
 	def get_InternetChargeType(self): # String
 		return self.get_query_params().get('InternetChargeType')
 
 	def set_InternetChargeType(self, InternetChargeType):  # String
 		self.add_query_param('InternetChargeType', InternetChargeType)
 	def get_Name(self): # String
 		return self.get_query_params().get('Name')
```

### Comparing `aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/AssociateAnycastEipAddressRequest.py` & `aliyun-python-sdk-eipanycast-1.0.5/aliyunsdkeipanycast/request/v20200309/AssociateAnycastEipAddressRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkeipanycast.endpoint import endpoint_data
 
 class AssociateAnycastEipAddressRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'AssociateAnycastEipAddress')
+		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'AssociateAnycastEipAddress','eipanycast')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/DescribeAnycastEipAddressRequest.py` & `aliyun-python-sdk-eipanycast-1.0.5/aliyunsdkeipanycast/request/v20200309/DescribeAnycastEipAddressRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkeipanycast.endpoint import endpoint_data
 
 class DescribeAnycastEipAddressRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'DescribeAnycastEipAddress')
+		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'DescribeAnycastEipAddress','eipanycast')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/DescribeAnycastPopLocationsRequest.py` & `aliyun-python-sdk-eipanycast-1.0.5/aliyunsdkeipanycast/request/v20200309/DescribeAnycastPopLocationsRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkeipanycast.endpoint import endpoint_data
 
 class DescribeAnycastPopLocationsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'DescribeAnycastPopLocations')
+		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'DescribeAnycastPopLocations','eipanycast')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/DescribeAnycastServerRegionsRequest.py` & `aliyun-python-sdk-eipanycast-1.0.5/aliyunsdkeipanycast/request/v20200309/DescribeAnycastServerRegionsRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkeipanycast.endpoint import endpoint_data
 
 class DescribeAnycastServerRegionsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'DescribeAnycastServerRegions')
+		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'DescribeAnycastServerRegions','eipanycast')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/ListAnycastEipAddressesRequest.py` & `aliyun-python-sdk-eipanycast-1.0.5/aliyunsdkeipanycast/request/v20200309/ListAnycastEipAddressesRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,22 +19,27 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkeipanycast.endpoint import endpoint_data
 
 class ListAnycastEipAddressesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'ListAnycastEipAddresses')
+		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'ListAnycastEipAddresses','eipanycast')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_ResourceGroupId(self): # String
+		return self.get_query_params().get('ResourceGroupId')
+
+	def set_ResourceGroupId(self, ResourceGroupId):  # String
+		self.add_query_param('ResourceGroupId', ResourceGroupId)
 	def get_NextToken(self): # String
 		return self.get_query_params().get('NextToken')
 
 	def set_NextToken(self, NextToken):  # String
 		self.add_query_param('NextToken', NextToken)
 	def get_InstanceChargeType(self): # String
 		return self.get_query_params().get('InstanceChargeType')
```

### Comparing `aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/ListTagResourcesRequest.py` & `aliyun-python-sdk-eipanycast-1.0.5/aliyunsdkeipanycast/request/v20200309/ListTagResourcesRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkeipanycast.endpoint import endpoint_data
 
 class ListTagResourcesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'ListTagResources')
+		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'ListTagResources','eipanycast')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/ModifyAnycastEipAddressAttributeRequest.py` & `aliyun-python-sdk-eipanycast-1.0.5/aliyunsdkeipanycast/request/v20200309/ModifyAnycastEipAddressAttributeRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkeipanycast.endpoint import endpoint_data
 
 class ModifyAnycastEipAddressAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'ModifyAnycastEipAddressAttribute')
+		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'ModifyAnycastEipAddressAttribute','eipanycast')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/ModifyAnycastEipAddressSpecRequest.py` & `aliyun-python-sdk-eipanycast-1.0.5/aliyunsdkeipanycast/request/v20200309/ModifyAnycastEipAddressSpecRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkeipanycast.endpoint import endpoint_data
 
 class ModifyAnycastEipAddressSpecRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'ModifyAnycastEipAddressSpec')
+		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'ModifyAnycastEipAddressSpec','eipanycast')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/ReleaseAnycastEipAddressRequest.py` & `aliyun-python-sdk-eipanycast-1.0.5/aliyunsdkeipanycast/request/v20200309/ReleaseAnycastEipAddressRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkeipanycast.endpoint import endpoint_data
 
 class ReleaseAnycastEipAddressRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'ReleaseAnycastEipAddress')
+		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'ReleaseAnycastEipAddress','eipanycast')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/TagResourcesRequest.py` & `aliyun-python-sdk-eipanycast-1.0.5/aliyunsdkeipanycast/request/v20200309/TagResourcesRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkeipanycast.endpoint import endpoint_data
 
 class TagResourcesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'TagResources')
+		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'TagResources','eipanycast')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/UnassociateAnycastEipAddressRequest.py` & `aliyun-python-sdk-eipanycast-1.0.5/aliyunsdkeipanycast/request/v20200309/UnassociateAnycastEipAddressRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkeipanycast.endpoint import endpoint_data
 
 class UnassociateAnycastEipAddressRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'UnassociateAnycastEipAddress')
+		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'UnassociateAnycastEipAddress','eipanycast')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/UntagResourcesRequest.py` & `aliyun-python-sdk-eipanycast-1.0.5/aliyunsdkeipanycast/request/v20200309/UntagResourcesRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkeipanycast.endpoint import endpoint_data
 
 class UntagResourcesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'UntagResources')
+		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'UntagResources','eipanycast')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-eipanycast-1.0.4/aliyunsdkeipanycast/request/v20200309/UpdateAnycastEipAddressAssociationsRequest.py` & `aliyun-python-sdk-eipanycast-1.0.5/aliyunsdkeipanycast/request/v20200309/UpdateAnycastEipAddressAssociationsRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkeipanycast.endpoint import endpoint_data
 
 class UpdateAnycastEipAddressAssociationsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'UpdateAnycastEipAddressAssociations')
+		RpcRequest.__init__(self, 'Eipanycast', '2020-03-09', 'UpdateAnycastEipAddressAssociations','eipanycast')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-eipanycast-1.0.4/setup.py` & `aliyun-python-sdk-eipanycast-1.0.5/setup.py`

 * *Files identical despite different names*

