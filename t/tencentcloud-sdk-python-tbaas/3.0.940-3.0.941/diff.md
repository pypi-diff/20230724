# Comparing `tmp/tencentcloud-sdk-python-tbaas-3.0.940.tar.gz` & `tmp/tencentcloud-sdk-python-tbaas-3.0.941.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tbaas-3.0.940.tar", last modified: Fri Jul 21 00:49:43 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tbaas-3.0.941.tar", last modified: Mon Jul 24 00:44:00 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tbaas-3.0.940.tar` & `tencentcloud-sdk-python-tbaas-3.0.941.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:49:43.000000 tencentcloud-sdk-python-tbaas-3.0.940/
--rw-r--r--   0 root         (0) root         (0)     1010 2023-07-21 00:49:43.000000 tencentcloud-sdk-python-tbaas-3.0.940/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:49:43.000000 tencentcloud-sdk-python-tbaas-3.0.940/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:49:43.000000 tencentcloud-sdk-python-tbaas-3.0.940/tencentcloud/tbaas/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:49:43.000000 tencentcloud-sdk-python-tbaas-3.0.940/tencentcloud/tbaas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:49:43.000000 tencentcloud-sdk-python-tbaas-3.0.940/tencentcloud/tbaas/v20180416/
--rw-r--r--   0 root         (0) root         (0)    20172 2023-07-21 00:49:43.000000 tencentcloud-sdk-python-tbaas-3.0.940/tencentcloud/tbaas/v20180416/tbaas_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:49:43.000000 tencentcloud-sdk-python-tbaas-3.0.940/tencentcloud/tbaas/v20180416/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10641 2023-07-21 00:49:43.000000 tencentcloud-sdk-python-tbaas-3.0.940/tencentcloud/tbaas/v20180416/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   112703 2023-07-21 00:49:43.000000 tencentcloud-sdk-python-tbaas-3.0.940/tencentcloud/tbaas/v20180416/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-21 00:49:43.000000 tencentcloud-sdk-python-tbaas-3.0.940/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:49:43.000000 tencentcloud-sdk-python-tbaas-3.0.940/tencentcloud_sdk_python_tbaas.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 00:49:43.000000 tencentcloud-sdk-python-tbaas-3.0.940/tencentcloud_sdk_python_tbaas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-07-21 00:49:43.000000 tencentcloud-sdk-python-tbaas-3.0.940/tencentcloud_sdk_python_tbaas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-21 00:49:43.000000 tencentcloud-sdk-python-tbaas-3.0.940/tencentcloud_sdk_python_tbaas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-21 00:49:43.000000 tencentcloud-sdk-python-tbaas-3.0.940/tencentcloud_sdk_python_tbaas.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-21 00:49:43.000000 tencentcloud-sdk-python-tbaas-3.0.940/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-21 00:49:43.000000 tencentcloud-sdk-python-tbaas-3.0.940/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      743 2023-07-21 00:49:43.000000 tencentcloud-sdk-python-tbaas-3.0.940/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:44:00.000000 tencentcloud-sdk-python-tbaas-3.0.941/
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-07-24 00:44:00.000000 tencentcloud-sdk-python-tbaas-3.0.941/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:44:00.000000 tencentcloud-sdk-python-tbaas-3.0.941/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:44:00.000000 tencentcloud-sdk-python-tbaas-3.0.941/tencentcloud/tbaas/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:44:00.000000 tencentcloud-sdk-python-tbaas-3.0.941/tencentcloud/tbaas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:44:00.000000 tencentcloud-sdk-python-tbaas-3.0.941/tencentcloud/tbaas/v20180416/
+-rw-r--r--   0 root         (0) root         (0)    20172 2023-07-24 00:44:00.000000 tencentcloud-sdk-python-tbaas-3.0.941/tencentcloud/tbaas/v20180416/tbaas_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:44:00.000000 tencentcloud-sdk-python-tbaas-3.0.941/tencentcloud/tbaas/v20180416/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10664 2023-07-24 00:44:00.000000 tencentcloud-sdk-python-tbaas-3.0.941/tencentcloud/tbaas/v20180416/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   112703 2023-07-24 00:44:00.000000 tencentcloud-sdk-python-tbaas-3.0.941/tencentcloud/tbaas/v20180416/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-24 00:44:00.000000 tencentcloud-sdk-python-tbaas-3.0.941/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:44:00.000000 tencentcloud-sdk-python-tbaas-3.0.941/tencentcloud_sdk_python_tbaas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 00:44:00.000000 tencentcloud-sdk-python-tbaas-3.0.941/tencentcloud_sdk_python_tbaas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-07-24 00:44:00.000000 tencentcloud-sdk-python-tbaas-3.0.941/tencentcloud_sdk_python_tbaas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-24 00:44:00.000000 tencentcloud-sdk-python-tbaas-3.0.941/tencentcloud_sdk_python_tbaas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-24 00:44:00.000000 tencentcloud-sdk-python-tbaas-3.0.941/tencentcloud_sdk_python_tbaas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-24 00:44:00.000000 tencentcloud-sdk-python-tbaas-3.0.941/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-24 00:44:00.000000 tencentcloud-sdk-python-tbaas-3.0.941/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      743 2023-07-24 00:44:00.000000 tencentcloud-sdk-python-tbaas-3.0.941/README.rst
```

### Comparing `tencentcloud-sdk-python-tbaas-3.0.940/setup.py` & `tencentcloud-sdk-python-tbaas-3.0.941/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tbaas-3.0.940/tencentcloud/tbaas/v20180416/tbaas_client.py` & `tencentcloud-sdk-python-tbaas-3.0.941/tencentcloud/tbaas/v20180416/tbaas_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tbaas-3.0.940/tencentcloud/tbaas/v20180416/errorcodes.py` & `tencentcloud-sdk-python-tbaas-3.0.941/tencentcloud/tbaas/v20180416/errorcodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 
 # Bcos无效的群组编号。
 FAILEDOPERATION_INVALIDGROUPPK = 'FailedOperation.InvalidGroupPk'
 
 # Bcos无效的私钥用户信息。
 FAILEDOPERATION_INVALIDKEYUSER = 'FailedOperation.InvalidKeyUser'
 
-# 无效操作。
+# 用户非法操作。
 FAILEDOPERATION_INVALIDOPERATION = 'FailedOperation.InvalidOperation'
 
 # 交易请求异常。
 FAILEDOPERATION_MANAGESERVICE = 'FailedOperation.ManageService'
 
 # Bcos新建合约失败。
 FAILEDOPERATION_NEWCONTRACT = 'FailedOperation.NewContract'
@@ -205,15 +205,15 @@
 
 # Bcos不支持的请求类型。
 INTERNALERROR_METHODTYPENOTSUPPORT = 'InternalError.MethodTypeNotSupport'
 
 # 错误码未定义。
 INTERNALERROR_NODEFINEERROR = 'InternalError.NoDefineError'
 
-# Bcos服务器异常，请重试。
+# 内部错误，请稍后重试或者联系技术人员
 INTERNALERROR_SERVERERROR = 'InternalError.ServerError'
 
 # 服务器异常。
 INTERNALERROR_SERVEREXCEPTION = 'InternalError.ServerException'
 
 # 服务异常，请重试。
 INTERNALERROR_SERVICEERROR = 'InternalError.ServiceError'
@@ -295,15 +295,15 @@
 
 # 参数取值错误。
 INVALIDPARAMETERVALUE = 'InvalidParameterValue'
 
 # 参数格式不正确。
 INVALIDPARAMETERVALUE_ILLEGALFORMAT = 'InvalidParameterValue.IllegalFormat'
 
-# 参数取值不合法。
+# 请求参数错误。
 INVALIDPARAMETERVALUE_ILLEGALVALUE = 'InvalidParameterValue.IllegalValue'
 
 # 参数值为空。
 INVALIDPARAMETERVALUE_PARAMETEREMPTY = 'InvalidParameterValue.ParameterEmpty'
 
 # Bcos缺少参数。
 MISSINGPARAMETER_EMPTYPARAM = 'MissingParameter.EmptyParam'
```

### Comparing `tencentcloud-sdk-python-tbaas-3.0.940/tencentcloud/tbaas/v20180416/models.py` & `tencentcloud-sdk-python-tbaas-3.0.941/tencentcloud/tbaas/v20180416/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tbaas-3.0.940/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tbaas-3.0.941/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.940'
+__version__ = '3.0.941'
```

### Comparing `tencentcloud-sdk-python-tbaas-3.0.940/tencentcloud_sdk_python_tbaas.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tbaas-3.0.941/tencentcloud_sdk_python_tbaas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tbaas
-Version: 3.0.940
+Version: 3.0.941
 Summary: Tencent Cloud Tbaas SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tbaas-3.0.940/PKG-INFO` & `tencentcloud-sdk-python-tbaas-3.0.941/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tbaas
-Version: 3.0.940
+Version: 3.0.941
 Summary: Tencent Cloud Tbaas SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tbaas-3.0.940/README.rst` & `tencentcloud-sdk-python-tbaas-3.0.941/README.rst`

 * *Files identical despite different names*

