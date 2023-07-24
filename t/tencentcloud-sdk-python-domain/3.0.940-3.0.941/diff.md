# Comparing `tmp/tencentcloud-sdk-python-domain-3.0.940.tar.gz` & `tmp/tencentcloud-sdk-python-domain-3.0.941.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-domain-3.0.940.tar", last modified: Fri Jul 21 00:27:57 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-domain-3.0.941.tar", last modified: Mon Jul 24 00:35:53 2023, max compression
```

## Comparing `tencentcloud-sdk-python-domain-3.0.940.tar` & `tencentcloud-sdk-python-domain-3.0.941.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:27:57.000000 tencentcloud-sdk-python-domain-3.0.940/
--rw-r--r--   0 root         (0) root         (0)     1012 2023-07-21 00:27:57.000000 tencentcloud-sdk-python-domain-3.0.940/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:27:57.000000 tencentcloud-sdk-python-domain-3.0.940/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-21 00:27:57.000000 tencentcloud-sdk-python-domain-3.0.940/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:27:57.000000 tencentcloud-sdk-python-domain-3.0.940/tencentcloud/domain/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:27:57.000000 tencentcloud-sdk-python-domain-3.0.940/tencentcloud/domain/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:27:57.000000 tencentcloud-sdk-python-domain-3.0.940/tencentcloud/domain/v20180808/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:27:57.000000 tencentcloud-sdk-python-domain-3.0.940/tencentcloud/domain/v20180808/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8787 2023-07-21 00:27:57.000000 tencentcloud-sdk-python-domain-3.0.940/tencentcloud/domain/v20180808/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    25207 2023-07-21 00:27:57.000000 tencentcloud-sdk-python-domain-3.0.940/tencentcloud/domain/v20180808/domain_client.py
--rw-r--r--   0 root         (0) root         (0)   121377 2023-07-21 00:27:57.000000 tencentcloud-sdk-python-domain-3.0.940/tencentcloud/domain/v20180808/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-21 00:27:57.000000 tencentcloud-sdk-python-domain-3.0.940/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:27:57.000000 tencentcloud-sdk-python-domain-3.0.940/tencentcloud_sdk_python_domain.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 00:27:57.000000 tencentcloud-sdk-python-domain-3.0.940/tencentcloud_sdk_python_domain.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-07-21 00:27:57.000000 tencentcloud-sdk-python-domain-3.0.940/tencentcloud_sdk_python_domain.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-21 00:27:57.000000 tencentcloud-sdk-python-domain-3.0.940/tencentcloud_sdk_python_domain.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-21 00:27:57.000000 tencentcloud-sdk-python-domain-3.0.940/tencentcloud_sdk_python_domain.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-21 00:27:57.000000 tencentcloud-sdk-python-domain-3.0.940/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      746 2023-07-21 00:27:57.000000 tencentcloud-sdk-python-domain-3.0.940/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:35:53.000000 tencentcloud-sdk-python-domain-3.0.941/
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-07-24 00:35:53.000000 tencentcloud-sdk-python-domain-3.0.941/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:35:53.000000 tencentcloud-sdk-python-domain-3.0.941/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-24 00:35:53.000000 tencentcloud-sdk-python-domain-3.0.941/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:35:53.000000 tencentcloud-sdk-python-domain-3.0.941/tencentcloud/domain/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:35:53.000000 tencentcloud-sdk-python-domain-3.0.941/tencentcloud/domain/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:35:53.000000 tencentcloud-sdk-python-domain-3.0.941/tencentcloud/domain/v20180808/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:35:53.000000 tencentcloud-sdk-python-domain-3.0.941/tencentcloud/domain/v20180808/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8876 2023-07-24 00:35:53.000000 tencentcloud-sdk-python-domain-3.0.941/tencentcloud/domain/v20180808/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    26115 2023-07-24 00:35:53.000000 tencentcloud-sdk-python-domain-3.0.941/tencentcloud/domain/v20180808/domain_client.py
+-rw-r--r--   0 root         (0) root         (0)   122825 2023-07-24 00:35:53.000000 tencentcloud-sdk-python-domain-3.0.941/tencentcloud/domain/v20180808/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-24 00:35:53.000000 tencentcloud-sdk-python-domain-3.0.941/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:35:53.000000 tencentcloud-sdk-python-domain-3.0.941/tencentcloud_sdk_python_domain.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 00:35:53.000000 tencentcloud-sdk-python-domain-3.0.941/tencentcloud_sdk_python_domain.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-07-24 00:35:53.000000 tencentcloud-sdk-python-domain-3.0.941/tencentcloud_sdk_python_domain.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-24 00:35:53.000000 tencentcloud-sdk-python-domain-3.0.941/tencentcloud_sdk_python_domain.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-24 00:35:53.000000 tencentcloud-sdk-python-domain-3.0.941/tencentcloud_sdk_python_domain.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-24 00:35:53.000000 tencentcloud-sdk-python-domain-3.0.941/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-07-24 00:35:53.000000 tencentcloud-sdk-python-domain-3.0.941/README.rst
```

### Comparing `tencentcloud-sdk-python-domain-3.0.940/setup.py` & `tencentcloud-sdk-python-domain-3.0.941/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-domain-3.0.940/tencentcloud/__init__.py` & `tencentcloud-sdk-python-domain-3.0.941/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-domain-3.0.940/tencentcloud/domain/v20180808/errorcodes.py` & `tencentcloud-sdk-python-domain-3.0.941/tencentcloud/domain/v20180808/errorcodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,17 @@
 
 # 获取域名价格失败。
 FAILEDOPERATION_GETDOMAINPRICEFAILED = 'FailedOperation.GetDomainPriceFailed'
 
 # 域名过户失败。
 FAILEDOPERATION_MODIFYDOMAINOWNERFAILED = 'FailedOperation.ModifyDomainOwnerFailed'
 
+# 权限不足。
+FAILEDOPERATION_PERMISSIONDENIED = 'FailedOperation.PermissionDenied'
+
 # 禁止的手机或邮箱。
 FAILEDOPERATION_PROHIBITPHONEEMAIL = 'FailedOperation.ProhibitPhoneEmail'
 
 # 域名注册操作失败，请稍后重试。
 FAILEDOPERATION_REGISTERDOMAIN = 'FailedOperation.RegisterDomain'
 
 # 域名注册操作失败，请稍后重试。
```

### Comparing `tencentcloud-sdk-python-domain-3.0.940/tencentcloud/domain/v20180808/domain_client.py` & `tencentcloud-sdk-python-domain-3.0.941/tencentcloud/domain/v20180808/domain_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def CreateDomainRedemption(self, request):
+        """创建赎回订单。
+
+        :param request: Request instance for CreateDomainRedemption.
+        :type request: :class:`tencentcloud.domain.v20180808.models.CreateDomainRedemptionRequest`
+        :rtype: :class:`tencentcloud.domain.v20180808.models.CreateDomainRedemptionResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateDomainRedemption", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateDomainRedemptionResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def CreatePhoneEmail(self, request):
         """此接口用于创建有效的手机、邮箱
 
         :param request: Request instance for CreatePhoneEmail.
         :type request: :class:`tencentcloud.domain.v20180808.models.CreatePhoneEmailRequest`
         :rtype: :class:`tencentcloud.domain.v20180808.models.CreatePhoneEmailResponse`
```

### Comparing `tencentcloud-sdk-python-domain-3.0.940/tencentcloud/domain/v20180808/models.py` & `tencentcloud-sdk-python-domain-3.0.941/tencentcloud/domain/v20180808/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1043,14 +1043,72 @@
 
 
     def _deserialize(self, params):
         self._LogId = params.get("LogId")
         self._RequestId = params.get("RequestId")
 
 
+class CreateDomainRedemptionRequest(AbstractModel):
+    """CreateDomainRedemption请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _DomainId: 域名 ID
+        :type DomainId: str
+        """
+        self._DomainId = None
+
+    @property
+    def DomainId(self):
+        return self._DomainId
+
+    @DomainId.setter
+    def DomainId(self, DomainId):
+        self._DomainId = DomainId
+
+
+    def _deserialize(self, params):
+        self._DomainId = params.get("DomainId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateDomainRedemptionResponse(AbstractModel):
+    """CreateDomainRedemption返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._RequestId = None
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._RequestId = params.get("RequestId")
+
+
 class CreatePhoneEmailRequest(AbstractModel):
     """CreatePhoneEmail请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-domain-3.0.940/tencentcloud_sdk_python_domain.egg-info/PKG-INFO` & `tencentcloud-sdk-python-domain-3.0.941/tencentcloud_sdk_python_domain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-domain
-Version: 3.0.940
+Version: 3.0.941
 Summary: Tencent Cloud Domain SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-domain-3.0.940/PKG-INFO` & `tencentcloud-sdk-python-domain-3.0.941/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-domain
-Version: 3.0.940
+Version: 3.0.941
 Summary: Tencent Cloud Domain SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-domain-3.0.940/README.rst` & `tencentcloud-sdk-python-domain-3.0.941/README.rst`

 * *Files identical despite different names*

