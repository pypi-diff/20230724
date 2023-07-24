# Comparing `tmp/tencentcloud-sdk-python-cdb-3.0.940.tar.gz` & `tmp/tencentcloud-sdk-python-cdb-3.0.941.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cdb-3.0.940.tar", last modified: Fri Jul 21 00:24:30 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cdb-3.0.941.tar", last modified: Mon Jul 24 00:32:31 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cdb-3.0.940.tar` & `tencentcloud-sdk-python-cdb-3.0.941.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:24:30.000000 tencentcloud-sdk-python-cdb-3.0.940/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-21 00:24:30.000000 tencentcloud-sdk-python-cdb-3.0.940/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:24:30.000000 tencentcloud-sdk-python-cdb-3.0.940/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-21 00:24:30.000000 tencentcloud-sdk-python-cdb-3.0.940/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:24:30.000000 tencentcloud-sdk-python-cdb-3.0.940/tencentcloud/cdb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:24:30.000000 tencentcloud-sdk-python-cdb-3.0.940/tencentcloud/cdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:24:30.000000 tencentcloud-sdk-python-cdb-3.0.940/tencentcloud/cdb/v20170320/
--rw-r--r--   0 root         (0) root         (0)   152053 2023-07-21 00:24:30.000000 tencentcloud-sdk-python-cdb-3.0.940/tencentcloud/cdb/v20170320/cdb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:24:30.000000 tencentcloud-sdk-python-cdb-3.0.940/tencentcloud/cdb/v20170320/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19678 2023-07-21 00:24:30.000000 tencentcloud-sdk-python-cdb-3.0.940/tencentcloud/cdb/v20170320/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   844268 2023-07-21 00:24:30.000000 tencentcloud-sdk-python-cdb-3.0.940/tencentcloud/cdb/v20170320/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-21 00:24:30.000000 tencentcloud-sdk-python-cdb-3.0.940/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:24:30.000000 tencentcloud-sdk-python-cdb-3.0.940/tencentcloud_sdk_python_cdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 00:24:30.000000 tencentcloud-sdk-python-cdb-3.0.940/tencentcloud_sdk_python_cdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-21 00:24:30.000000 tencentcloud-sdk-python-cdb-3.0.940/tencentcloud_sdk_python_cdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-21 00:24:30.000000 tencentcloud-sdk-python-cdb-3.0.940/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-21 00:24:30.000000 tencentcloud-sdk-python-cdb-3.0.940/tencentcloud_sdk_python_cdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-21 00:24:30.000000 tencentcloud-sdk-python-cdb-3.0.940/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-21 00:24:30.000000 tencentcloud-sdk-python-cdb-3.0.940/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:32:31.000000 tencentcloud-sdk-python-cdb-3.0.941/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-24 00:32:30.000000 tencentcloud-sdk-python-cdb-3.0.941/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:32:31.000000 tencentcloud-sdk-python-cdb-3.0.941/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-24 00:32:30.000000 tencentcloud-sdk-python-cdb-3.0.941/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:32:31.000000 tencentcloud-sdk-python-cdb-3.0.941/tencentcloud/cdb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:32:30.000000 tencentcloud-sdk-python-cdb-3.0.941/tencentcloud/cdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:32:31.000000 tencentcloud-sdk-python-cdb-3.0.941/tencentcloud/cdb/v20170320/
+-rw-r--r--   0 root         (0) root         (0)   146951 2023-07-24 00:32:30.000000 tencentcloud-sdk-python-cdb-3.0.941/tencentcloud/cdb/v20170320/cdb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:32:30.000000 tencentcloud-sdk-python-cdb-3.0.941/tencentcloud/cdb/v20170320/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19678 2023-07-24 00:32:30.000000 tencentcloud-sdk-python-cdb-3.0.941/tencentcloud/cdb/v20170320/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   798517 2023-07-24 00:32:30.000000 tencentcloud-sdk-python-cdb-3.0.941/tencentcloud/cdb/v20170320/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-24 00:32:31.000000 tencentcloud-sdk-python-cdb-3.0.941/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:32:31.000000 tencentcloud-sdk-python-cdb-3.0.941/tencentcloud_sdk_python_cdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 00:32:31.000000 tencentcloud-sdk-python-cdb-3.0.941/tencentcloud_sdk_python_cdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-24 00:32:31.000000 tencentcloud-sdk-python-cdb-3.0.941/tencentcloud_sdk_python_cdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-24 00:32:31.000000 tencentcloud-sdk-python-cdb-3.0.941/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-24 00:32:31.000000 tencentcloud-sdk-python-cdb-3.0.941/tencentcloud_sdk_python_cdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-24 00:32:31.000000 tencentcloud-sdk-python-cdb-3.0.941/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-24 00:32:30.000000 tencentcloud-sdk-python-cdb-3.0.941/README.rst
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.940/setup.py` & `tencentcloud-sdk-python-cdb-3.0.941/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.940/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cdb-3.0.941/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cdb-3.0.940/tencentcloud/cdb/v20170320/cdb_client.py` & `tencentcloud-sdk-python-cdb-3.0.941/tencentcloud/cdb/v20170320/cdb_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1195,39 +1195,14 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeCDBProxy(self, request):
-        """接口已经废弃，请使用+DescribeCdbProxyInfo+进行替换。
-
-        查询数据库代理（待下线，替换接口QueryCDBProxy）
-
-        :param request: Request instance for DescribeCDBProxy.
-        :type request: :class:`tencentcloud.cdb.v20170320.models.DescribeCDBProxyRequest`
-        :rtype: :class:`tencentcloud.cdb.v20170320.models.DescribeCDBProxyResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DescribeCDBProxy", params, headers=headers)
-            response = json.loads(body)
-            model = models.DescribeCDBProxyResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(type(e).__name__, str(e))
-
-
     def DescribeCdbProxyInfo(self, request):
         """查询数据库代理详情信息
 
         :param request: Request instance for DescribeCdbProxyInfo.
         :type request: :class:`tencentcloud.cdb.v20170320.models.DescribeCdbProxyInfoRequest`
         :rtype: :class:`tencentcloud.cdb.v20170320.models.DescribeCdbProxyInfoResponse`
 
@@ -1821,39 +1796,14 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeProxyConnectionPoolConf(self, request):
-        """当前接口已经废弃，请使用+DescribeCdbProxyInfo+替代。
-
-        获取数据库代理连接池相关规格配置
-
-        :param request: Request instance for DescribeProxyConnectionPoolConf.
-        :type request: :class:`tencentcloud.cdb.v20170320.models.DescribeProxyConnectionPoolConfRequest`
-        :rtype: :class:`tencentcloud.cdb.v20170320.models.DescribeProxyConnectionPoolConfResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DescribeProxyConnectionPoolConf", params, headers=headers)
-            response = json.loads(body)
-            model = models.DescribeProxyConnectionPoolConfResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(type(e).__name__, str(e))
-
-
     def DescribeProxyCustomConf(self, request):
         """查询代理规格配置
 
         :param request: Request instance for DescribeProxyCustomConf.
         :type request: :class:`tencentcloud.cdb.v20170320.models.DescribeProxyCustomConfRequest`
         :rtype: :class:`tencentcloud.cdb.v20170320.models.DescribeProxyCustomConfResponse`
 
@@ -2542,64 +2492,14 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def ModifyCDBProxyConnectionPool(self, request):
-        """当前接口已经废弃，请使用+AdjustCdbProxyAddress+进行替代。
-
-        请求该接口配置数据库连接池；支持的连接池配置请求DescribeProxyConnectionPoolConf接口获取。
-
-        :param request: Request instance for ModifyCDBProxyConnectionPool.
-        :type request: :class:`tencentcloud.cdb.v20170320.models.ModifyCDBProxyConnectionPoolRequest`
-        :rtype: :class:`tencentcloud.cdb.v20170320.models.ModifyCDBProxyConnectionPoolResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("ModifyCDBProxyConnectionPool", params, headers=headers)
-            response = json.loads(body)
-            model = models.ModifyCDBProxyConnectionPoolResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(type(e).__name__, str(e))
-
-
-    def ModifyCDBProxyVipVPort(self, request):
-        """当前接口已经废弃，请使用+ModifyCdbProxyAddressVipAndVPort+进行替代。
-
-        修改数据库代理VIP或端口
-
-        :param request: Request instance for ModifyCDBProxyVipVPort.
-        :type request: :class:`tencentcloud.cdb.v20170320.models.ModifyCDBProxyVipVPortRequest`
-        :rtype: :class:`tencentcloud.cdb.v20170320.models.ModifyCDBProxyVipVPortResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("ModifyCDBProxyVipVPort", params, headers=headers)
-            response = json.loads(body)
-            model = models.ModifyCDBProxyVipVPortResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(type(e).__name__, str(e))
-
-
     def ModifyCdbProxyAddressDesc(self, request):
         """修改代理地址描述信息
 
         :param request: Request instance for ModifyCdbProxyAddressDesc.
         :type request: :class:`tencentcloud.cdb.v20170320.models.ModifyCdbProxyAddressDescRequest`
         :rtype: :class:`tencentcloud.cdb.v20170320.models.ModifyCdbProxyAddressDescResponse`
 
@@ -3089,39 +2989,14 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
-
-
-    def QueryCDBProxy(self, request):
-        """当前接口已经废弃，请使用+DescribeCdbProxyInfo+进行替代。
-
-        查询代理详情
-
-        :param request: Request instance for QueryCDBProxy.
-        :type request: :class:`tencentcloud.cdb.v20170320.models.QueryCDBProxyRequest`
-        :rtype: :class:`tencentcloud.cdb.v20170320.models.QueryCDBProxyResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("QueryCDBProxy", params, headers=headers)
-            response = json.loads(body)
-            model = models.QueryCDBProxyResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReleaseIsolatedDBInstances(self, request):
         """本接口（ReleaseIsolatedDBInstances）用于恢复已隔离云数据库实例。
 
         :param request: Request instance for ReleaseIsolatedDBInstances.
         :type request: :class:`tencentcloud.cdb.v20170320.models.ReleaseIsolatedDBInstancesRequest`
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.940/tencentcloud/cdb/v20170320/errorcodes.py` & `tencentcloud-sdk-python-cdb-3.0.941/tencentcloud/cdb/v20170320/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.940/tencentcloud/cdb/v20170320/models.py` & `tencentcloud-sdk-python-cdb-3.0.941/tencentcloud/cdb/v20170320/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -318,100 +318,14 @@
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         self._RequestId = params.get("RequestId")
 
 
-class Address(AbstractModel):
-    """地址
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _Vip: 地址
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Vip: str
-        :param _VPort: 端口
-注意：此字段可能返回 null，表示取不到有效值。
-        :type VPort: int
-        :param _UniqVpcId: 私有网络ID
-注意：此字段可能返回 null，表示取不到有效值。
-        :type UniqVpcId: str
-        :param _UniqSubnet: 私有网络子网ID
-注意：此字段可能返回 null，表示取不到有效值。
-        :type UniqSubnet: str
-        :param _Desc: 描述
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Desc: str
-        """
-        self._Vip = None
-        self._VPort = None
-        self._UniqVpcId = None
-        self._UniqSubnet = None
-        self._Desc = None
-
-    @property
-    def Vip(self):
-        return self._Vip
-
-    @Vip.setter
-    def Vip(self, Vip):
-        self._Vip = Vip
-
-    @property
-    def VPort(self):
-        return self._VPort
-
-    @VPort.setter
-    def VPort(self, VPort):
-        self._VPort = VPort
-
-    @property
-    def UniqVpcId(self):
-        return self._UniqVpcId
-
-    @UniqVpcId.setter
-    def UniqVpcId(self, UniqVpcId):
-        self._UniqVpcId = UniqVpcId
-
-    @property
-    def UniqSubnet(self):
-        return self._UniqSubnet
-
-    @UniqSubnet.setter
-    def UniqSubnet(self, UniqSubnet):
-        self._UniqSubnet = UniqSubnet
-
-    @property
-    def Desc(self):
-        return self._Desc
-
-    @Desc.setter
-    def Desc(self, Desc):
-        self._Desc = Desc
-
-
-    def _deserialize(self, params):
-        self._Vip = params.get("Vip")
-        self._VPort = params.get("VPort")
-        self._UniqVpcId = params.get("UniqVpcId")
-        self._UniqSubnet = params.get("UniqSubnet")
-        self._Desc = params.get("Desc")
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
 class AdjustCdbProxyAddressRequest(AbstractModel):
     """AdjustCdbProxyAddress请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -2668,139 +2582,14 @@
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         self._RequestId = params.get("RequestId")
 
 
-class BaseGroupInfo(AbstractModel):
-    """proxy代理组信息
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _ProxyGroupId: 代理组ID
-注意：此字段可能返回 null，表示取不到有效值。
-        :type ProxyGroupId: str
-        :param _NodeCount: 代理节点数
-注意：此字段可能返回 null，表示取不到有效值。
-        :type NodeCount: int
-        :param _Status: 状态：发货中（init）运行中（online）下线中（offline）销毁中（destroy）
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Status: str
-        :param _Region: 地域
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Region: str
-        :param _Zone: 可用区
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Zone: str
-        :param _OpenRW: 是否开启读写分离
-注意：此字段可能返回 null，表示取不到有效值。
-        :type OpenRW: bool
-        :param _CurrentProxyVersion: 当前代理版本
-注意：此字段可能返回 null，表示取不到有效值。
-        :type CurrentProxyVersion: str
-        :param _SupportUpgradeProxyVersion: 支持升级版本
-注意：此字段可能返回 null，表示取不到有效值。
-        :type SupportUpgradeProxyVersion: str
-        """
-        self._ProxyGroupId = None
-        self._NodeCount = None
-        self._Status = None
-        self._Region = None
-        self._Zone = None
-        self._OpenRW = None
-        self._CurrentProxyVersion = None
-        self._SupportUpgradeProxyVersion = None
-
-    @property
-    def ProxyGroupId(self):
-        return self._ProxyGroupId
-
-    @ProxyGroupId.setter
-    def ProxyGroupId(self, ProxyGroupId):
-        self._ProxyGroupId = ProxyGroupId
-
-    @property
-    def NodeCount(self):
-        return self._NodeCount
-
-    @NodeCount.setter
-    def NodeCount(self, NodeCount):
-        self._NodeCount = NodeCount
-
-    @property
-    def Status(self):
-        return self._Status
-
-    @Status.setter
-    def Status(self, Status):
-        self._Status = Status
-
-    @property
-    def Region(self):
-        return self._Region
-
-    @Region.setter
-    def Region(self, Region):
-        self._Region = Region
-
-    @property
-    def Zone(self):
-        return self._Zone
-
-    @Zone.setter
-    def Zone(self, Zone):
-        self._Zone = Zone
-
-    @property
-    def OpenRW(self):
-        return self._OpenRW
-
-    @OpenRW.setter
-    def OpenRW(self, OpenRW):
-        self._OpenRW = OpenRW
-
-    @property
-    def CurrentProxyVersion(self):
-        return self._CurrentProxyVersion
-
-    @CurrentProxyVersion.setter
-    def CurrentProxyVersion(self, CurrentProxyVersion):
-        self._CurrentProxyVersion = CurrentProxyVersion
-
-    @property
-    def SupportUpgradeProxyVersion(self):
-        return self._SupportUpgradeProxyVersion
-
-    @SupportUpgradeProxyVersion.setter
-    def SupportUpgradeProxyVersion(self, SupportUpgradeProxyVersion):
-        self._SupportUpgradeProxyVersion = SupportUpgradeProxyVersion
-
-
-    def _deserialize(self, params):
-        self._ProxyGroupId = params.get("ProxyGroupId")
-        self._NodeCount = params.get("NodeCount")
-        self._Status = params.get("Status")
-        self._Region = params.get("Region")
-        self._Zone = params.get("Zone")
-        self._OpenRW = params.get("OpenRW")
-        self._CurrentProxyVersion = params.get("CurrentProxyVersion")
-        self._SupportUpgradeProxyVersion = params.get("SupportUpgradeProxyVersion")
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
 class BinlogInfo(AbstractModel):
     """二进制日志信息
 
     """
 
     def __init__(self):
         r"""
@@ -4240,74 +4029,14 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class ConnectionPoolInfo(AbstractModel):
-    """连接池信息
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _ConnectionPool: 是否开启了连接池
-注意：此字段可能返回 null，表示取不到有效值。
-        :type ConnectionPool: bool
-        :param _ConnectionPoolType: 连接池类型：SessionConnectionPool（会话级别连接池）
-注意：此字段可能返回 null，表示取不到有效值。
-        :type ConnectionPoolType: str
-        :param _PoolConnectionTimeOut: 连接池保持阈值：单位（秒）
-注意：此字段可能返回 null，表示取不到有效值。
-        :type PoolConnectionTimeOut: int
-        """
-        self._ConnectionPool = None
-        self._ConnectionPoolType = None
-        self._PoolConnectionTimeOut = None
-
-    @property
-    def ConnectionPool(self):
-        return self._ConnectionPool
-
-    @ConnectionPool.setter
-    def ConnectionPool(self, ConnectionPool):
-        self._ConnectionPool = ConnectionPool
-
-    @property
-    def ConnectionPoolType(self):
-        return self._ConnectionPoolType
-
-    @ConnectionPoolType.setter
-    def ConnectionPoolType(self, ConnectionPoolType):
-        self._ConnectionPoolType = ConnectionPoolType
-
-    @property
-    def PoolConnectionTimeOut(self):
-        return self._PoolConnectionTimeOut
-
-    @PoolConnectionTimeOut.setter
-    def PoolConnectionTimeOut(self, PoolConnectionTimeOut):
-        self._PoolConnectionTimeOut = PoolConnectionTimeOut
-
-
-    def _deserialize(self, params):
-        self._ConnectionPool = params.get("ConnectionPool")
-        self._ConnectionPoolType = params.get("ConnectionPoolType")
-        self._PoolConnectionTimeOut = params.get("PoolConnectionTimeOut")
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
 class CreateAccountsRequest(AbstractModel):
     """CreateAccounts请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -10640,190 +10369,14 @@
             for item in params.get("Items"):
                 obj = BinlogInfo()
                 obj._deserialize(item)
                 self._Items.append(obj)
         self._RequestId = params.get("RequestId")
 
 
-class DescribeCDBProxyRequest(AbstractModel):
-    """DescribeCDBProxy请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _InstanceId: 实例ID
-        :type InstanceId: str
-        :param _ProxyGroupId: 代理组ID
-        :type ProxyGroupId: str
-        """
-        self._InstanceId = None
-        self._ProxyGroupId = None
-
-    @property
-    def InstanceId(self):
-        return self._InstanceId
-
-    @InstanceId.setter
-    def InstanceId(self, InstanceId):
-        self._InstanceId = InstanceId
-
-    @property
-    def ProxyGroupId(self):
-        return self._ProxyGroupId
-
-    @ProxyGroupId.setter
-    def ProxyGroupId(self, ProxyGroupId):
-        self._ProxyGroupId = ProxyGroupId
-
-
-    def _deserialize(self, params):
-        self._InstanceId = params.get("InstanceId")
-        self._ProxyGroupId = params.get("ProxyGroupId")
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
-class DescribeCDBProxyResponse(AbstractModel):
-    """DescribeCDBProxy返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _BaseGroup: 代理组基本信息
-注意：此字段可能返回 null，表示取不到有效值。
-        :type BaseGroup: :class:`tencentcloud.cdb.v20170320.models.BaseGroupInfo`
-        :param _Address: 代理组地址信息
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Address: :class:`tencentcloud.cdb.v20170320.models.Address`
-        :param _ProxyNode: 代理组节点信息
-注意：此字段可能返回 null，表示取不到有效值。
-        :type ProxyNode: :class:`tencentcloud.cdb.v20170320.models.ProxyNodeInfo`
-        :param _RWInstInfo: 读写分析信息
-注意：此字段可能返回 null，表示取不到有效值。
-        :type RWInstInfo: :class:`tencentcloud.cdb.v20170320.models.RWInfo`
-        :param _ConnectionPoolInfo: 连接池信息
-注意：此字段可能返回 null，表示取不到有效值。
-        :type ConnectionPoolInfo: :class:`tencentcloud.cdb.v20170320.models.ConnectionPoolInfo`
-        :param _Count: 代理数量
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Count: int
-        :param _ProxyGroup: 代理信息
-注意：此字段可能返回 null，表示取不到有效值。
-        :type ProxyGroup: list of ProxyGroup
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._BaseGroup = None
-        self._Address = None
-        self._ProxyNode = None
-        self._RWInstInfo = None
-        self._ConnectionPoolInfo = None
-        self._Count = None
-        self._ProxyGroup = None
-        self._RequestId = None
-
-    @property
-    def BaseGroup(self):
-        return self._BaseGroup
-
-    @BaseGroup.setter
-    def BaseGroup(self, BaseGroup):
-        self._BaseGroup = BaseGroup
-
-    @property
-    def Address(self):
-        return self._Address
-
-    @Address.setter
-    def Address(self, Address):
-        self._Address = Address
-
-    @property
-    def ProxyNode(self):
-        return self._ProxyNode
-
-    @ProxyNode.setter
-    def ProxyNode(self, ProxyNode):
-        self._ProxyNode = ProxyNode
-
-    @property
-    def RWInstInfo(self):
-        return self._RWInstInfo
-
-    @RWInstInfo.setter
-    def RWInstInfo(self, RWInstInfo):
-        self._RWInstInfo = RWInstInfo
-
-    @property
-    def ConnectionPoolInfo(self):
-        return self._ConnectionPoolInfo
-
-    @ConnectionPoolInfo.setter
-    def ConnectionPoolInfo(self, ConnectionPoolInfo):
-        self._ConnectionPoolInfo = ConnectionPoolInfo
-
-    @property
-    def Count(self):
-        return self._Count
-
-    @Count.setter
-    def Count(self, Count):
-        self._Count = Count
-
-    @property
-    def ProxyGroup(self):
-        return self._ProxyGroup
-
-    @ProxyGroup.setter
-    def ProxyGroup(self, ProxyGroup):
-        self._ProxyGroup = ProxyGroup
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
-        if params.get("BaseGroup") is not None:
-            self._BaseGroup = BaseGroupInfo()
-            self._BaseGroup._deserialize(params.get("BaseGroup"))
-        if params.get("Address") is not None:
-            self._Address = Address()
-            self._Address._deserialize(params.get("Address"))
-        if params.get("ProxyNode") is not None:
-            self._ProxyNode = ProxyNodeInfo()
-            self._ProxyNode._deserialize(params.get("ProxyNode"))
-        if params.get("RWInstInfo") is not None:
-            self._RWInstInfo = RWInfo()
-            self._RWInstInfo._deserialize(params.get("RWInstInfo"))
-        if params.get("ConnectionPoolInfo") is not None:
-            self._ConnectionPoolInfo = ConnectionPoolInfo()
-            self._ConnectionPoolInfo._deserialize(params.get("ConnectionPoolInfo"))
-        self._Count = params.get("Count")
-        if params.get("ProxyGroup") is not None:
-            self._ProxyGroup = []
-            for item in params.get("ProxyGroup"):
-                obj = ProxyGroup()
-                obj._deserialize(item)
-                self._ProxyGroup.append(obj)
-        self._RequestId = params.get("RequestId")
-
-
 class DescribeCdbProxyInfoRequest(AbstractModel):
     """DescribeCdbProxyInfo请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -14318,124 +13871,14 @@
                 obj = SecurityGroup()
                 obj._deserialize(item)
                 self._Groups.append(obj)
         self._TotalCount = params.get("TotalCount")
         self._RequestId = params.get("RequestId")
 
 
-class DescribeProxyConnectionPoolConfRequest(AbstractModel):
-    """DescribeProxyConnectionPoolConf请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _InstanceId: 实例ID
-        :type InstanceId: str
-        :param _Offset: 分页查询偏移量
-        :type Offset: int
-        :param _Limit: 分页查询限制
-        :type Limit: int
-        """
-        self._InstanceId = None
-        self._Offset = None
-        self._Limit = None
-
-    @property
-    def InstanceId(self):
-        return self._InstanceId
-
-    @InstanceId.setter
-    def InstanceId(self, InstanceId):
-        self._InstanceId = InstanceId
-
-    @property
-    def Offset(self):
-        return self._Offset
-
-    @Offset.setter
-    def Offset(self, Offset):
-        self._Offset = Offset
-
-    @property
-    def Limit(self):
-        return self._Limit
-
-    @Limit.setter
-    def Limit(self, Limit):
-        self._Limit = Limit
-
-
-    def _deserialize(self, params):
-        self._InstanceId = params.get("InstanceId")
-        self._Offset = params.get("Offset")
-        self._Limit = params.get("Limit")
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
-class DescribeProxyConnectionPoolConfResponse(AbstractModel):
-    """DescribeProxyConnectionPoolConf返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _Count: 配置规格数量
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Count: int
-        :param _PoolConf: 连接池配置规格
-注意：此字段可能返回 null，表示取不到有效值。
-        :type PoolConf: :class:`tencentcloud.cdb.v20170320.models.PoolConf`
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._Count = None
-        self._PoolConf = None
-        self._RequestId = None
-
-    @property
-    def Count(self):
-        return self._Count
-
-    @Count.setter
-    def Count(self, Count):
-        self._Count = Count
-
-    @property
-    def PoolConf(self):
-        return self._PoolConf
-
-    @PoolConf.setter
-    def PoolConf(self, PoolConf):
-        self._PoolConf = PoolConf
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
-        self._Count = params.get("Count")
-        if params.get("PoolConf") is not None:
-            self._PoolConf = PoolConf()
-            self._PoolConf._deserialize(params.get("PoolConf"))
-        self._RequestId = params.get("RequestId")
-
-
 class DescribeProxyCustomConfRequest(AbstractModel):
     """DescribeProxyCustomConf请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -19990,241 +19433,14 @@
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         self._RequestId = params.get("RequestId")
 
 
-class ModifyCDBProxyConnectionPoolRequest(AbstractModel):
-    """ModifyCDBProxyConnectionPool请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _ProxyGroupId: 数据库代理ID
-        :type ProxyGroupId: str
-        :param _OpenConnectionPool: 是否开启连接池，true：开启连接池；
-                             false：关闭连接池。
-        :type OpenConnectionPool: bool
-        :param _ConnectionPoolType: 连接池类型，
-通过DescribeProxyConnectionPoolConf获取连接池类型值
-        :type ConnectionPoolType: str
-        :param _PoolConnectionTimeOut: 连接保留阈值：单位（秒）
-        :type PoolConnectionTimeOut: int
-        """
-        self._ProxyGroupId = None
-        self._OpenConnectionPool = None
-        self._ConnectionPoolType = None
-        self._PoolConnectionTimeOut = None
-
-    @property
-    def ProxyGroupId(self):
-        return self._ProxyGroupId
-
-    @ProxyGroupId.setter
-    def ProxyGroupId(self, ProxyGroupId):
-        self._ProxyGroupId = ProxyGroupId
-
-    @property
-    def OpenConnectionPool(self):
-        return self._OpenConnectionPool
-
-    @OpenConnectionPool.setter
-    def OpenConnectionPool(self, OpenConnectionPool):
-        self._OpenConnectionPool = OpenConnectionPool
-
-    @property
-    def ConnectionPoolType(self):
-        return self._ConnectionPoolType
-
-    @ConnectionPoolType.setter
-    def ConnectionPoolType(self, ConnectionPoolType):
-        self._ConnectionPoolType = ConnectionPoolType
-
-    @property
-    def PoolConnectionTimeOut(self):
-        return self._PoolConnectionTimeOut
-
-    @PoolConnectionTimeOut.setter
-    def PoolConnectionTimeOut(self, PoolConnectionTimeOut):
-        self._PoolConnectionTimeOut = PoolConnectionTimeOut
-
-
-    def _deserialize(self, params):
-        self._ProxyGroupId = params.get("ProxyGroupId")
-        self._OpenConnectionPool = params.get("OpenConnectionPool")
-        self._ConnectionPoolType = params.get("ConnectionPoolType")
-        self._PoolConnectionTimeOut = params.get("PoolConnectionTimeOut")
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
-class ModifyCDBProxyConnectionPoolResponse(AbstractModel):
-    """ModifyCDBProxyConnectionPool返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _AsyncRequestId: 异步处理ID
-注意：此字段可能返回 null，表示取不到有效值。
-        :type AsyncRequestId: str
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._AsyncRequestId = None
-        self._RequestId = None
-
-    @property
-    def AsyncRequestId(self):
-        return self._AsyncRequestId
-
-    @AsyncRequestId.setter
-    def AsyncRequestId(self, AsyncRequestId):
-        self._AsyncRequestId = AsyncRequestId
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
-        self._AsyncRequestId = params.get("AsyncRequestId")
-        self._RequestId = params.get("RequestId")
-
-
-class ModifyCDBProxyVipVPortRequest(AbstractModel):
-    """ModifyCDBProxyVipVPort请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _ProxyGroupId: 代理组ID
-        :type ProxyGroupId: str
-        :param _UniqVpcId: 私有网络ID
-        :type UniqVpcId: str
-        :param _UniqSubnetId: 私有网络子网ID
-        :type UniqSubnetId: str
-        :param _DstIp: 目标IP
-        :type DstIp: str
-        :param _DstPort: 目标端口
-        :type DstPort: int
-        :param _ReleaseDuration: 旧IP回收时间 单位小时
-        :type ReleaseDuration: int
-        """
-        self._ProxyGroupId = None
-        self._UniqVpcId = None
-        self._UniqSubnetId = None
-        self._DstIp = None
-        self._DstPort = None
-        self._ReleaseDuration = None
-
-    @property
-    def ProxyGroupId(self):
-        return self._ProxyGroupId
-
-    @ProxyGroupId.setter
-    def ProxyGroupId(self, ProxyGroupId):
-        self._ProxyGroupId = ProxyGroupId
-
-    @property
-    def UniqVpcId(self):
-        return self._UniqVpcId
-
-    @UniqVpcId.setter
-    def UniqVpcId(self, UniqVpcId):
-        self._UniqVpcId = UniqVpcId
-
-    @property
-    def UniqSubnetId(self):
-        return self._UniqSubnetId
-
-    @UniqSubnetId.setter
-    def UniqSubnetId(self, UniqSubnetId):
-        self._UniqSubnetId = UniqSubnetId
-
-    @property
-    def DstIp(self):
-        return self._DstIp
-
-    @DstIp.setter
-    def DstIp(self, DstIp):
-        self._DstIp = DstIp
-
-    @property
-    def DstPort(self):
-        return self._DstPort
-
-    @DstPort.setter
-    def DstPort(self, DstPort):
-        self._DstPort = DstPort
-
-    @property
-    def ReleaseDuration(self):
-        return self._ReleaseDuration
-
-    @ReleaseDuration.setter
-    def ReleaseDuration(self, ReleaseDuration):
-        self._ReleaseDuration = ReleaseDuration
-
-
-    def _deserialize(self, params):
-        self._ProxyGroupId = params.get("ProxyGroupId")
-        self._UniqVpcId = params.get("UniqVpcId")
-        self._UniqSubnetId = params.get("UniqSubnetId")
-        self._DstIp = params.get("DstIp")
-        self._DstPort = params.get("DstPort")
-        self._ReleaseDuration = params.get("ReleaseDuration")
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
-class ModifyCDBProxyVipVPortResponse(AbstractModel):
-    """ModifyCDBProxyVipVPort返回参数结构体
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
 class ModifyCdbProxyAddressDescRequest(AbstractModel):
     """ModifyCdbProxyAddressDesc请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -22715,74 +21931,14 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class PoolConf(AbstractModel):
-    """数据库代理连接池规格配置
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _ConnectionPoolType: 连接池类型：SessionConnectionPool（会话级别连接池
-注意：此字段可能返回 null，表示取不到有效值。
-        :type ConnectionPoolType: str
-        :param _MaxPoolConnectionTimeOut: 最大可保持连接阈值：单位（秒）
-注意：此字段可能返回 null，表示取不到有效值。
-        :type MaxPoolConnectionTimeOut: int
-        :param _MinPoolConnectionTimeOut: 最小可保持连接阈值：单位（秒）
-注意：此字段可能返回 null，表示取不到有效值。
-        :type MinPoolConnectionTimeOut: int
-        """
-        self._ConnectionPoolType = None
-        self._MaxPoolConnectionTimeOut = None
-        self._MinPoolConnectionTimeOut = None
-
-    @property
-    def ConnectionPoolType(self):
-        return self._ConnectionPoolType
-
-    @ConnectionPoolType.setter
-    def ConnectionPoolType(self, ConnectionPoolType):
-        self._ConnectionPoolType = ConnectionPoolType
-
-    @property
-    def MaxPoolConnectionTimeOut(self):
-        return self._MaxPoolConnectionTimeOut
-
-    @MaxPoolConnectionTimeOut.setter
-    def MaxPoolConnectionTimeOut(self, MaxPoolConnectionTimeOut):
-        self._MaxPoolConnectionTimeOut = MaxPoolConnectionTimeOut
-
-    @property
-    def MinPoolConnectionTimeOut(self):
-        return self._MinPoolConnectionTimeOut
-
-    @MinPoolConnectionTimeOut.setter
-    def MinPoolConnectionTimeOut(self, MinPoolConnectionTimeOut):
-        self._MinPoolConnectionTimeOut = MinPoolConnectionTimeOut
-
-
-    def _deserialize(self, params):
-        self._ConnectionPoolType = params.get("ConnectionPoolType")
-        self._MaxPoolConnectionTimeOut = params.get("MaxPoolConnectionTimeOut")
-        self._MinPoolConnectionTimeOut = params.get("MinPoolConnectionTimeOut")
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
 class ProxyAddress(AbstractModel):
     """数据库代理地址信息
 
     """
 
     def __init__(self):
         r"""
@@ -23067,116 +22223,14 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class ProxyGroup(AbstractModel):
-    """数据代理组信息
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _BaseGroup: 代理基本信息
-注意：此字段可能返回 null，表示取不到有效值。
-        :type BaseGroup: :class:`tencentcloud.cdb.v20170320.models.BaseGroupInfo`
-        :param _Address: 代理地址信息
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Address: list of Address
-        :param _ConnectionPoolInfo: 代理连接池信息
-注意：此字段可能返回 null，表示取不到有效值。
-        :type ConnectionPoolInfo: :class:`tencentcloud.cdb.v20170320.models.ConnectionPoolInfo`
-        :param _ProxyNode: 代理节点信息
-注意：此字段可能返回 null，表示取不到有效值。
-        :type ProxyNode: list of ProxyNodeInfo
-        :param _RWInstInfo: 代理路由信息
-注意：此字段可能返回 null，表示取不到有效值。
-        :type RWInstInfo: :class:`tencentcloud.cdb.v20170320.models.RWInfo`
-        """
-        self._BaseGroup = None
-        self._Address = None
-        self._ConnectionPoolInfo = None
-        self._ProxyNode = None
-        self._RWInstInfo = None
-
-    @property
-    def BaseGroup(self):
-        return self._BaseGroup
-
-    @BaseGroup.setter
-    def BaseGroup(self, BaseGroup):
-        self._BaseGroup = BaseGroup
-
-    @property
-    def Address(self):
-        return self._Address
-
-    @Address.setter
-    def Address(self, Address):
-        self._Address = Address
-
-    @property
-    def ConnectionPoolInfo(self):
-        return self._ConnectionPoolInfo
-
-    @ConnectionPoolInfo.setter
-    def ConnectionPoolInfo(self, ConnectionPoolInfo):
-        self._ConnectionPoolInfo = ConnectionPoolInfo
-
-    @property
-    def ProxyNode(self):
-        return self._ProxyNode
-
-    @ProxyNode.setter
-    def ProxyNode(self, ProxyNode):
-        self._ProxyNode = ProxyNode
-
-    @property
-    def RWInstInfo(self):
-        return self._RWInstInfo
-
-    @RWInstInfo.setter
-    def RWInstInfo(self, RWInstInfo):
-        self._RWInstInfo = RWInstInfo
-
-
-    def _deserialize(self, params):
-        if params.get("BaseGroup") is not None:
-            self._BaseGroup = BaseGroupInfo()
-            self._BaseGroup._deserialize(params.get("BaseGroup"))
-        if params.get("Address") is not None:
-            self._Address = []
-            for item in params.get("Address"):
-                obj = Address()
-                obj._deserialize(item)
-                self._Address.append(obj)
-        if params.get("ConnectionPoolInfo") is not None:
-            self._ConnectionPoolInfo = ConnectionPoolInfo()
-            self._ConnectionPoolInfo._deserialize(params.get("ConnectionPoolInfo"))
-        if params.get("ProxyNode") is not None:
-            self._ProxyNode = []
-            for item in params.get("ProxyNode"):
-                obj = ProxyNodeInfo()
-                obj._deserialize(item)
-                self._ProxyNode.append(obj)
-        if params.get("RWInstInfo") is not None:
-            self._RWInstInfo = RWInfo()
-            self._RWInstInfo._deserialize(params.get("RWInstInfo"))
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
 class ProxyGroupInfo(AbstractModel):
     """代理组详情
 
     """
 
     def __init__(self):
         r"""
@@ -23329,116 +22383,14 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class ProxyGroups(AbstractModel):
-    """数据代理组信息
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _BaseGroup: 代理基本信息
-注意：此字段可能返回 null，表示取不到有效值。
-        :type BaseGroup: :class:`tencentcloud.cdb.v20170320.models.BaseGroupInfo`
-        :param _Address: 代理地址信息
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Address: list of Address
-        :param _ConnectionPoolInfo: 代理连接池信息
-注意：此字段可能返回 null，表示取不到有效值。
-        :type ConnectionPoolInfo: :class:`tencentcloud.cdb.v20170320.models.ConnectionPoolInfo`
-        :param _ProxyNode: 代理节点信息
-注意：此字段可能返回 null，表示取不到有效值。
-        :type ProxyNode: list of ProxyNodeInfo
-        :param _RWInstInfo: 代理路由信息
-注意：此字段可能返回 null，表示取不到有效值。
-        :type RWInstInfo: :class:`tencentcloud.cdb.v20170320.models.RWInfos`
-        """
-        self._BaseGroup = None
-        self._Address = None
-        self._ConnectionPoolInfo = None
-        self._ProxyNode = None
-        self._RWInstInfo = None
-
-    @property
-    def BaseGroup(self):
-        return self._BaseGroup
-
-    @BaseGroup.setter
-    def BaseGroup(self, BaseGroup):
-        self._BaseGroup = BaseGroup
-
-    @property
-    def Address(self):
-        return self._Address
-
-    @Address.setter
-    def Address(self, Address):
-        self._Address = Address
-
-    @property
-    def ConnectionPoolInfo(self):
-        return self._ConnectionPoolInfo
-
-    @ConnectionPoolInfo.setter
-    def ConnectionPoolInfo(self, ConnectionPoolInfo):
-        self._ConnectionPoolInfo = ConnectionPoolInfo
-
-    @property
-    def ProxyNode(self):
-        return self._ProxyNode
-
-    @ProxyNode.setter
-    def ProxyNode(self, ProxyNode):
-        self._ProxyNode = ProxyNode
-
-    @property
-    def RWInstInfo(self):
-        return self._RWInstInfo
-
-    @RWInstInfo.setter
-    def RWInstInfo(self, RWInstInfo):
-        self._RWInstInfo = RWInstInfo
-
-
-    def _deserialize(self, params):
-        if params.get("BaseGroup") is not None:
-            self._BaseGroup = BaseGroupInfo()
-            self._BaseGroup._deserialize(params.get("BaseGroup"))
-        if params.get("Address") is not None:
-            self._Address = []
-            for item in params.get("Address"):
-                obj = Address()
-                obj._deserialize(item)
-                self._Address.append(obj)
-        if params.get("ConnectionPoolInfo") is not None:
-            self._ConnectionPoolInfo = ConnectionPoolInfo()
-            self._ConnectionPoolInfo._deserialize(params.get("ConnectionPoolInfo"))
-        if params.get("ProxyNode") is not None:
-            self._ProxyNode = []
-            for item in params.get("ProxyNode"):
-                obj = ProxyNodeInfo()
-                obj._deserialize(item)
-                self._ProxyNode.append(obj)
-        if params.get("RWInstInfo") is not None:
-            self._RWInstInfo = RWInfos()
-            self._RWInstInfo._deserialize(params.get("RWInstInfo"))
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
 class ProxyInst(AbstractModel):
     """代理实例
 
     """
 
     def __init__(self):
         r"""
@@ -23736,472 +22688,14 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class ProxyNodeInfo(AbstractModel):
-    """代理节点信息
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _ProxyNodeId: 代理节点ID
-注意：此字段可能返回 null，表示取不到有效值。
-        :type ProxyNodeId: str
-        :param _ProxyNodeConnections: 节点当前连接数
-注意：此字段可能返回 null，表示取不到有效值。
-        :type ProxyNodeConnections: int
-        :param _ProxyNodeCpu: cup
-注意：此字段可能返回 null，表示取不到有效值。
-        :type ProxyNodeCpu: int
-        :param _ProxyNodeMem: 内存
-注意：此字段可能返回 null，表示取不到有效值。
-        :type ProxyNodeMem: int
-        :param _ProxyStatus: 节点状态：
-init（申请中）
-online（运行中）
-offline（离线中）
-destroy（已销毁）
-recovering（故障恢复中）
-error（节点故障）
-注意：此字段可能返回 null，表示取不到有效值。
-        :type ProxyStatus: str
-        """
-        self._ProxyNodeId = None
-        self._ProxyNodeConnections = None
-        self._ProxyNodeCpu = None
-        self._ProxyNodeMem = None
-        self._ProxyStatus = None
-
-    @property
-    def ProxyNodeId(self):
-        return self._ProxyNodeId
-
-    @ProxyNodeId.setter
-    def ProxyNodeId(self, ProxyNodeId):
-        self._ProxyNodeId = ProxyNodeId
-
-    @property
-    def ProxyNodeConnections(self):
-        return self._ProxyNodeConnections
-
-    @ProxyNodeConnections.setter
-    def ProxyNodeConnections(self, ProxyNodeConnections):
-        self._ProxyNodeConnections = ProxyNodeConnections
-
-    @property
-    def ProxyNodeCpu(self):
-        return self._ProxyNodeCpu
-
-    @ProxyNodeCpu.setter
-    def ProxyNodeCpu(self, ProxyNodeCpu):
-        self._ProxyNodeCpu = ProxyNodeCpu
-
-    @property
-    def ProxyNodeMem(self):
-        return self._ProxyNodeMem
-
-    @ProxyNodeMem.setter
-    def ProxyNodeMem(self, ProxyNodeMem):
-        self._ProxyNodeMem = ProxyNodeMem
-
-    @property
-    def ProxyStatus(self):
-        return self._ProxyStatus
-
-    @ProxyStatus.setter
-    def ProxyStatus(self, ProxyStatus):
-        self._ProxyStatus = ProxyStatus
-
-
-    def _deserialize(self, params):
-        self._ProxyNodeId = params.get("ProxyNodeId")
-        self._ProxyNodeConnections = params.get("ProxyNodeConnections")
-        self._ProxyNodeCpu = params.get("ProxyNodeCpu")
-        self._ProxyNodeMem = params.get("ProxyNodeMem")
-        self._ProxyStatus = params.get("ProxyStatus")
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
-class QueryCDBProxyRequest(AbstractModel):
-    """QueryCDBProxy请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _InstanceId: 实例ID
-        :type InstanceId: str
-        :param _ProxyGroupId: 代理ID
-        :type ProxyGroupId: str
-        """
-        self._InstanceId = None
-        self._ProxyGroupId = None
-
-    @property
-    def InstanceId(self):
-        return self._InstanceId
-
-    @InstanceId.setter
-    def InstanceId(self, InstanceId):
-        self._InstanceId = InstanceId
-
-    @property
-    def ProxyGroupId(self):
-        return self._ProxyGroupId
-
-    @ProxyGroupId.setter
-    def ProxyGroupId(self, ProxyGroupId):
-        self._ProxyGroupId = ProxyGroupId
-
-
-    def _deserialize(self, params):
-        self._InstanceId = params.get("InstanceId")
-        self._ProxyGroupId = params.get("ProxyGroupId")
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
-class QueryCDBProxyResponse(AbstractModel):
-    """QueryCDBProxy返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _Count: 代理数量
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Count: int
-        :param _ProxyGroup: 代理信息
-注意：此字段可能返回 null，表示取不到有效值。
-        :type ProxyGroup: list of ProxyGroups
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._Count = None
-        self._ProxyGroup = None
-        self._RequestId = None
-
-    @property
-    def Count(self):
-        return self._Count
-
-    @Count.setter
-    def Count(self, Count):
-        self._Count = Count
-
-    @property
-    def ProxyGroup(self):
-        return self._ProxyGroup
-
-    @ProxyGroup.setter
-    def ProxyGroup(self, ProxyGroup):
-        self._ProxyGroup = ProxyGroup
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
-        self._Count = params.get("Count")
-        if params.get("ProxyGroup") is not None:
-            self._ProxyGroup = []
-            for item in params.get("ProxyGroup"):
-                obj = ProxyGroups()
-                obj._deserialize(item)
-                self._ProxyGroup.append(obj)
-        self._RequestId = params.get("RequestId")
-
-
-class RWInfo(AbstractModel):
-    """proxy读写分离信息
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _InstCount: 代理实例数量
-注意：此字段可能返回 null，表示取不到有效值。
-        :type InstCount: int
-        :param _WeightMode: 权重分配模式；
-系统自动分配："system"， 自定义："custom"
-注意：此字段可能返回 null，表示取不到有效值。
-        :type WeightMode: str
-        :param _IsKickOut: 是否开启延迟剔除
-注意：此字段可能返回 null，表示取不到有效值。
-        :type IsKickOut: bool
-        :param _MinCount: 最小保留数
-注意：此字段可能返回 null，表示取不到有效值。
-        :type MinCount: int
-        :param _MaxDelay: 延迟剔除阈值
-注意：此字段可能返回 null，表示取不到有效值。
-        :type MaxDelay: int
-        :param _FailOver: 是否开启故障转移
-注意：此字段可能返回 null，表示取不到有效值。
-        :type FailOver: bool
-        :param _AutoAddRo: 是否自动添加RO
-注意：此字段可能返回 null，表示取不到有效值。
-        :type AutoAddRo: bool
-        :param _RWInstInfo: 代理实例信息
-注意：此字段可能返回 null，表示取不到有效值。
-        :type RWInstInfo: :class:`tencentcloud.cdb.v20170320.models.RWInstanceInfo`
-        """
-        self._InstCount = None
-        self._WeightMode = None
-        self._IsKickOut = None
-        self._MinCount = None
-        self._MaxDelay = None
-        self._FailOver = None
-        self._AutoAddRo = None
-        self._RWInstInfo = None
-
-    @property
-    def InstCount(self):
-        return self._InstCount
-
-    @InstCount.setter
-    def InstCount(self, InstCount):
-        self._InstCount = InstCount
-
-    @property
-    def WeightMode(self):
-        return self._WeightMode
-
-    @WeightMode.setter
-    def WeightMode(self, WeightMode):
-        self._WeightMode = WeightMode
-
-    @property
-    def IsKickOut(self):
-        return self._IsKickOut
-
-    @IsKickOut.setter
-    def IsKickOut(self, IsKickOut):
-        self._IsKickOut = IsKickOut
-
-    @property
-    def MinCount(self):
-        return self._MinCount
-
-    @MinCount.setter
-    def MinCount(self, MinCount):
-        self._MinCount = MinCount
-
-    @property
-    def MaxDelay(self):
-        return self._MaxDelay
-
-    @MaxDelay.setter
-    def MaxDelay(self, MaxDelay):
-        self._MaxDelay = MaxDelay
-
-    @property
-    def FailOver(self):
-        return self._FailOver
-
-    @FailOver.setter
-    def FailOver(self, FailOver):
-        self._FailOver = FailOver
-
-    @property
-    def AutoAddRo(self):
-        return self._AutoAddRo
-
-    @AutoAddRo.setter
-    def AutoAddRo(self, AutoAddRo):
-        self._AutoAddRo = AutoAddRo
-
-    @property
-    def RWInstInfo(self):
-        return self._RWInstInfo
-
-    @RWInstInfo.setter
-    def RWInstInfo(self, RWInstInfo):
-        self._RWInstInfo = RWInstInfo
-
-
-    def _deserialize(self, params):
-        self._InstCount = params.get("InstCount")
-        self._WeightMode = params.get("WeightMode")
-        self._IsKickOut = params.get("IsKickOut")
-        self._MinCount = params.get("MinCount")
-        self._MaxDelay = params.get("MaxDelay")
-        self._FailOver = params.get("FailOver")
-        self._AutoAddRo = params.get("AutoAddRo")
-        if params.get("RWInstInfo") is not None:
-            self._RWInstInfo = RWInstanceInfo()
-            self._RWInstInfo._deserialize(params.get("RWInstInfo"))
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
-class RWInfos(AbstractModel):
-    """proxy读写分离信息
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _InstCount: 代理实例数量
-注意：此字段可能返回 null，表示取不到有效值。
-        :type InstCount: int
-        :param _WeightMode: 权重分配模式；
-系统自动分配："system"， 自定义："custom"
-注意：此字段可能返回 null，表示取不到有效值。
-        :type WeightMode: str
-        :param _IsKickOut: 是否开启延迟剔除
-注意：此字段可能返回 null，表示取不到有效值。
-        :type IsKickOut: bool
-        :param _MinCount: 最小保留数
-注意：此字段可能返回 null，表示取不到有效值。
-        :type MinCount: int
-        :param _MaxDelay: 延迟剔除阈值
-注意：此字段可能返回 null，表示取不到有效值。
-        :type MaxDelay: int
-        :param _FailOver: 是否开启故障转移
-注意：此字段可能返回 null，表示取不到有效值。
-        :type FailOver: bool
-        :param _AutoAddRo: 是否自动添加RO
-注意：此字段可能返回 null，表示取不到有效值。
-        :type AutoAddRo: bool
-        :param _RWInstInfo: 代理实例信息
-注意：此字段可能返回 null，表示取不到有效值。
-        :type RWInstInfo: list of RWInstanceInfo
-        """
-        self._InstCount = None
-        self._WeightMode = None
-        self._IsKickOut = None
-        self._MinCount = None
-        self._MaxDelay = None
-        self._FailOver = None
-        self._AutoAddRo = None
-        self._RWInstInfo = None
-
-    @property
-    def InstCount(self):
-        return self._InstCount
-
-    @InstCount.setter
-    def InstCount(self, InstCount):
-        self._InstCount = InstCount
-
-    @property
-    def WeightMode(self):
-        return self._WeightMode
-
-    @WeightMode.setter
-    def WeightMode(self, WeightMode):
-        self._WeightMode = WeightMode
-
-    @property
-    def IsKickOut(self):
-        return self._IsKickOut
-
-    @IsKickOut.setter
-    def IsKickOut(self, IsKickOut):
-        self._IsKickOut = IsKickOut
-
-    @property
-    def MinCount(self):
-        return self._MinCount
-
-    @MinCount.setter
-    def MinCount(self, MinCount):
-        self._MinCount = MinCount
-
-    @property
-    def MaxDelay(self):
-        return self._MaxDelay
-
-    @MaxDelay.setter
-    def MaxDelay(self, MaxDelay):
-        self._MaxDelay = MaxDelay
-
-    @property
-    def FailOver(self):
-        return self._FailOver
-
-    @FailOver.setter
-    def FailOver(self, FailOver):
-        self._FailOver = FailOver
-
-    @property
-    def AutoAddRo(self):
-        return self._AutoAddRo
-
-    @AutoAddRo.setter
-    def AutoAddRo(self, AutoAddRo):
-        self._AutoAddRo = AutoAddRo
-
-    @property
-    def RWInstInfo(self):
-        return self._RWInstInfo
-
-    @RWInstInfo.setter
-    def RWInstInfo(self, RWInstInfo):
-        self._RWInstInfo = RWInstInfo
-
-
-    def _deserialize(self, params):
-        self._InstCount = params.get("InstCount")
-        self._WeightMode = params.get("WeightMode")
-        self._IsKickOut = params.get("IsKickOut")
-        self._MinCount = params.get("MinCount")
-        self._MaxDelay = params.get("MaxDelay")
-        self._FailOver = params.get("FailOver")
-        self._AutoAddRo = params.get("AutoAddRo")
-        if params.get("RWInstInfo") is not None:
-            self._RWInstInfo = []
-            for item in params.get("RWInstInfo"):
-                obj = RWInstanceInfo()
-                obj._deserialize(item)
-                self._RWInstInfo.append(obj)
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
-class RWInstanceInfo(AbstractModel):
-    """代理实例信息
-
-    """
-
-
 class ReleaseIsolatedDBInstancesRequest(AbstractModel):
     """ReleaseIsolatedDBInstances请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.940/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cdb-3.0.941/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdb
-Version: 3.0.940
+Version: 3.0.941
 Summary: Tencent Cloud Cdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.940/PKG-INFO` & `tencentcloud-sdk-python-cdb-3.0.941/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdb
-Version: 3.0.940
+Version: 3.0.941
 Summary: Tencent Cloud Cdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.940/README.rst` & `tencentcloud-sdk-python-cdb-3.0.941/README.rst`

 * *Files identical despite different names*

