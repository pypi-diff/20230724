# Comparing `tmp/tencentcloud-sdk-python-tdid-3.0.940.tar.gz` & `tmp/tencentcloud-sdk-python-tdid-3.0.941.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tdid-3.0.940.tar", last modified: Fri Jul 21 00:50:43 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tdid-3.0.941.tar", last modified: Mon Jul 24 00:45:21 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tdid-3.0.940.tar` & `tencentcloud-sdk-python-tdid-3.0.941.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:50:43.000000 tencentcloud-sdk-python-tdid-3.0.940/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-21 00:50:43.000000 tencentcloud-sdk-python-tdid-3.0.940/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:50:43.000000 tencentcloud-sdk-python-tdid-3.0.940/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-21 00:50:43.000000 tencentcloud-sdk-python-tdid-3.0.940/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:50:43.000000 tencentcloud-sdk-python-tdid-3.0.940/tencentcloud/tdid/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:50:43.000000 tencentcloud-sdk-python-tdid-3.0.940/tencentcloud/tdid/v20210519/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:50:43.000000 tencentcloud-sdk-python-tdid-3.0.940/tencentcloud/tdid/v20210519/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14468 2023-07-21 00:50:43.000000 tencentcloud-sdk-python-tdid-3.0.940/tencentcloud/tdid/v20210519/tdid_client.py
--rw-r--r--   0 root         (0) root         (0)     1838 2023-07-21 00:50:43.000000 tencentcloud-sdk-python-tdid-3.0.940/tencentcloud/tdid/v20210519/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    49215 2023-07-21 00:50:43.000000 tencentcloud-sdk-python-tdid-3.0.940/tencentcloud/tdid/v20210519/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:50:43.000000 tencentcloud-sdk-python-tdid-3.0.940/tencentcloud/tdid/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-21 00:50:43.000000 tencentcloud-sdk-python-tdid-3.0.940/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:50:43.000000 tencentcloud-sdk-python-tdid-3.0.940/tencentcloud_sdk_python_tdid.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 00:50:43.000000 tencentcloud-sdk-python-tdid-3.0.940/tencentcloud_sdk_python_tdid.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-21 00:50:43.000000 tencentcloud-sdk-python-tdid-3.0.940/tencentcloud_sdk_python_tdid.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-21 00:50:43.000000 tencentcloud-sdk-python-tdid-3.0.940/tencentcloud_sdk_python_tdid.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-21 00:50:43.000000 tencentcloud-sdk-python-tdid-3.0.940/tencentcloud_sdk_python_tdid.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-21 00:50:43.000000 tencentcloud-sdk-python-tdid-3.0.940/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-21 00:50:43.000000 tencentcloud-sdk-python-tdid-3.0.940/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:45:21.000000 tencentcloud-sdk-python-tdid-3.0.941/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-24 00:45:21.000000 tencentcloud-sdk-python-tdid-3.0.941/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:45:21.000000 tencentcloud-sdk-python-tdid-3.0.941/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-24 00:45:21.000000 tencentcloud-sdk-python-tdid-3.0.941/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:45:21.000000 tencentcloud-sdk-python-tdid-3.0.941/tencentcloud/tdid/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:45:21.000000 tencentcloud-sdk-python-tdid-3.0.941/tencentcloud/tdid/v20210519/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:45:21.000000 tencentcloud-sdk-python-tdid-3.0.941/tencentcloud/tdid/v20210519/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12712 2023-07-24 00:45:21.000000 tencentcloud-sdk-python-tdid-3.0.941/tencentcloud/tdid/v20210519/tdid_client.py
+-rw-r--r--   0 root         (0) root         (0)     1775 2023-07-24 00:45:21.000000 tencentcloud-sdk-python-tdid-3.0.941/tencentcloud/tdid/v20210519/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    43358 2023-07-24 00:45:21.000000 tencentcloud-sdk-python-tdid-3.0.941/tencentcloud/tdid/v20210519/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:45:21.000000 tencentcloud-sdk-python-tdid-3.0.941/tencentcloud/tdid/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-24 00:45:21.000000 tencentcloud-sdk-python-tdid-3.0.941/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:45:21.000000 tencentcloud-sdk-python-tdid-3.0.941/tencentcloud_sdk_python_tdid.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 00:45:21.000000 tencentcloud-sdk-python-tdid-3.0.941/tencentcloud_sdk_python_tdid.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-24 00:45:21.000000 tencentcloud-sdk-python-tdid-3.0.941/tencentcloud_sdk_python_tdid.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-24 00:45:21.000000 tencentcloud-sdk-python-tdid-3.0.941/tencentcloud_sdk_python_tdid.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-24 00:45:21.000000 tencentcloud-sdk-python-tdid-3.0.941/tencentcloud_sdk_python_tdid.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-24 00:45:21.000000 tencentcloud-sdk-python-tdid-3.0.941/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-24 00:45:21.000000 tencentcloud-sdk-python-tdid-3.0.941/README.rst
```

### Comparing `tencentcloud-sdk-python-tdid-3.0.940/setup.py` & `tencentcloud-sdk-python-tdid-3.0.941/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdid-3.0.940/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tdid-3.0.941/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tdid-3.0.940/tencentcloud/tdid/v20210519/tdid_client.py` & `tencentcloud-sdk-python-tdid-3.0.941/tencentcloud/tdid/v20210519/tdid_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,39 +22,14 @@
 
 class TdidClient(AbstractClient):
     _apiVersion = '2021-05-19'
     _endpoint = 'tdid.tencentcloudapi.com'
     _service = 'tdid'
 
 
-    def AddLabel(self, request):
-        """下线已有内测接口，待上线正式版本的接口
-
-        DID添加标签
-
-        :param request: Request instance for AddLabel.
-        :type request: :class:`tencentcloud.tdid.v20210519.models.AddLabelRequest`
-        :rtype: :class:`tencentcloud.tdid.v20210519.models.AddLabelResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("AddLabel", params, headers=headers)
-            response = json.loads(body)
-            model = models.AddLabelResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(type(e).__name__, str(e))
-
-
     def CheckChain(self, request):
         """该接口不再使用
 
         检查区块链信息
 
         :param request: Request instance for CheckChain.
         :type request: :class:`tencentcloud.tdid.v20210519.models.CheckChainRequest`
@@ -195,39 +170,14 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
-
-
-    def GetAgencyTDid(self, request):
-        """该接口已废弃
-
-        本机构DID详情
-
-        :param request: Request instance for GetAgencyTDid.
-        :type request: :class:`tencentcloud.tdid.v20210519.models.GetAgencyTDidRequest`
-        :rtype: :class:`tencentcloud.tdid.v20210519.models.GetAgencyTDidResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("GetAgencyTDid", params, headers=headers)
-            response = json.loads(body)
-            model = models.GetAgencyTDidResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetAuthorityIssuer(self, request):
         """该接口不再使用
 
         获取权威机构信息
```

### Comparing `tencentcloud-sdk-python-tdid-3.0.940/tencentcloud/tdid/v20210519/errorcodes.py` & `tencentcloud-sdk-python-tdid-3.0.941/tencentcloud/tdid/v20210519/errorcodes.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,15 +46,12 @@
 
 # 参数取值错误。
 INVALIDPARAMETERVALUE = 'InvalidParameterValue'
 
 # 请求参数格式错误，请按照格式要求重新填写
 INVALIDPARAMETERVALUE_ILLEGALVALUE = 'InvalidParameterValue.IllegalValue'
 
-# 缺少参数错误。
-MISSINGPARAMETER = 'MissingParameter'
-
 # 资源不存在。
 RESOURCENOTFOUND = 'ResourceNotFound'
 
 # 操作不支持。
 UNSUPPORTEDOPERATION = 'UnsupportedOperation'
```

### Comparing `tencentcloud-sdk-python-tdid-3.0.940/tencentcloud/tdid/v20210519/models.py` & `tencentcloud-sdk-python-tdid-3.0.941/tencentcloud/tdid/v20210519/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,84 +14,14 @@
 # limitations under the License.
 
 import warnings
 
 from tencentcloud.common.abstract_model import AbstractModel
 
 
-class AddLabelRequest(AbstractModel):
-    """AddLabel请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _LabelId: 标签ID
-        :type LabelId: int
-        :param _Did: tdid
-        :type Did: str
-        """
-        self._LabelId = None
-        self._Did = None
-
-    @property
-    def LabelId(self):
-        return self._LabelId
-
-    @LabelId.setter
-    def LabelId(self, LabelId):
-        self._LabelId = LabelId
-
-    @property
-    def Did(self):
-        return self._Did
-
-    @Did.setter
-    def Did(self, Did):
-        self._Did = Did
-
-
-    def _deserialize(self, params):
-        self._LabelId = params.get("LabelId")
-        self._Did = params.get("Did")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class AddLabelResponse(AbstractModel):
-    """AddLabel返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._RequestId = None
-
-    @property
-    def RequestId(self):
-        return self._RequestId
-
-    @RequestId.setter
-    def RequestId(self, RequestId):
-        self._RequestId = RequestId
-
-
-    def _deserialize(self, params):
-        self._RequestId = params.get("RequestId")
-
-
 class CheckChainRequest(AbstractModel):
     """CheckChain请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -855,101 +785,14 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class GetAgencyTDidRequest(AbstractModel):
-    """GetAgencyTDid请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _ClusterId: 网络ID
-        :type ClusterId: str
-        """
-        self._ClusterId = None
-
-    @property
-    def ClusterId(self):
-        return self._ClusterId
-
-    @ClusterId.setter
-    def ClusterId(self, ClusterId):
-        self._ClusterId = ClusterId
-
-
-    def _deserialize(self, params):
-        self._ClusterId = params.get("ClusterId")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class GetAgencyTDidResponse(AbstractModel):
-    """GetAgencyTDid返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _Prefix: 固定前缀
-        :type Prefix: str
-        :param _Identity: did详情
-        :type Identity: list of Identity
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._Prefix = None
-        self._Identity = None
-        self._RequestId = None
-
-    @property
-    def Prefix(self):
-        return self._Prefix
-
-    @Prefix.setter
-    def Prefix(self, Prefix):
-        self._Prefix = Prefix
-
-    @property
-    def Identity(self):
-        return self._Identity
-
-    @Identity.setter
-    def Identity(self, Identity):
-        self._Identity = Identity
-
-    @property
-    def RequestId(self):
-        return self._RequestId
-
-    @RequestId.setter
-    def RequestId(self, RequestId):
-        self._RequestId = RequestId
-
-
-    def _deserialize(self, params):
-        self._Prefix = params.get("Prefix")
-        if params.get("Identity") is not None:
-            self._Identity = []
-            for item in params.get("Identity"):
-                obj = Identity()
-                obj._deserialize(item)
-                self._Identity.append(obj)
-        self._RequestId = params.get("RequestId")
-
-
 class GetAuthorityIssuerRequest(AbstractModel):
     """GetAuthorityIssuer请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -1308,95 +1151,14 @@
 
     def _deserialize(self, params):
         self._Name = params.get("Name")
         self._Document = params.get("Document")
         self._RequestId = params.get("RequestId")
 
 
-class Identity(AbstractModel):
-    """did详情
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _AccountIdentifier: 账户标识符
-        :type AccountIdentifier: str
-        :param _ChainID: 链ID
-        :type ChainID: str
-        :param _Did: 完整tdid
-        :type Did: str
-        :param _GroupId: 群组ID
-        :type GroupId: int
-        :param _GroupName: 群组名称
-        :type GroupName: str
-        """
-        self._AccountIdentifier = None
-        self._ChainID = None
-        self._Did = None
-        self._GroupId = None
-        self._GroupName = None
-
-    @property
-    def AccountIdentifier(self):
-        return self._AccountIdentifier
-
-    @AccountIdentifier.setter
-    def AccountIdentifier(self, AccountIdentifier):
-        self._AccountIdentifier = AccountIdentifier
-
-    @property
-    def ChainID(self):
-        return self._ChainID
-
-    @ChainID.setter
-    def ChainID(self, ChainID):
-        self._ChainID = ChainID
-
-    @property
-    def Did(self):
-        return self._Did
-
-    @Did.setter
-    def Did(self, Did):
-        self._Did = Did
-
-    @property
-    def GroupId(self):
-        return self._GroupId
-
-    @GroupId.setter
-    def GroupId(self, GroupId):
-        self._GroupId = GroupId
-
-    @property
-    def GroupName(self):
-        return self._GroupName
-
-    @GroupName.setter
-    def GroupName(self, GroupName):
-        self._GroupName = GroupName
-
-
-    def _deserialize(self, params):
-        self._AccountIdentifier = params.get("AccountIdentifier")
-        self._ChainID = params.get("ChainID")
-        self._Did = params.get("Did")
-        self._GroupId = params.get("GroupId")
-        self._GroupName = params.get("GroupName")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
 class Proof(AbstractModel):
     """验证凭证签名
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-tdid-3.0.940/tencentcloud_sdk_python_tdid.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tdid-3.0.941/tencentcloud_sdk_python_tdid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdid
-Version: 3.0.940
+Version: 3.0.941
 Summary: Tencent Cloud Tdid SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdid-3.0.940/PKG-INFO` & `tencentcloud-sdk-python-tdid-3.0.941/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdid
-Version: 3.0.940
+Version: 3.0.941
 Summary: Tencent Cloud Tdid SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdid-3.0.940/README.rst` & `tencentcloud-sdk-python-tdid-3.0.941/README.rst`

 * *Files identical despite different names*

