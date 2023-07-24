# Comparing `tmp/tencentcloud-sdk-python-cbs-3.0.940.tar.gz` & `tmp/tencentcloud-sdk-python-cbs-3.0.941.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cbs-3.0.940.tar", last modified: Fri Jul 21 00:24:21 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cbs-3.0.941.tar", last modified: Mon Jul 24 00:32:19 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cbs-3.0.940.tar` & `tencentcloud-sdk-python-cbs-3.0.941.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:24:21.000000 tencentcloud-sdk-python-cbs-3.0.940/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:24:21.000000 tencentcloud-sdk-python-cbs-3.0.940/tencentcloud_sdk_python_cbs.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 00:24:21.000000 tencentcloud-sdk-python-cbs-3.0.940/tencentcloud_sdk_python_cbs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-21 00:24:21.000000 tencentcloud-sdk-python-cbs-3.0.940/tencentcloud_sdk_python_cbs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-21 00:24:21.000000 tencentcloud-sdk-python-cbs-3.0.940/tencentcloud_sdk_python_cbs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-21 00:24:21.000000 tencentcloud-sdk-python-cbs-3.0.940/tencentcloud_sdk_python_cbs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-21 00:24:21.000000 tencentcloud-sdk-python-cbs-3.0.940/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:24:21.000000 tencentcloud-sdk-python-cbs-3.0.940/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-21 00:24:21.000000 tencentcloud-sdk-python-cbs-3.0.940/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:24:21.000000 tencentcloud-sdk-python-cbs-3.0.940/tencentcloud/cbs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:24:21.000000 tencentcloud-sdk-python-cbs-3.0.940/tencentcloud/cbs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:24:21.000000 tencentcloud-sdk-python-cbs-3.0.940/tencentcloud/cbs/v20170312/
--rw-r--r--   0 root         (0) root         (0)    53500 2023-07-21 00:24:21.000000 tencentcloud-sdk-python-cbs-3.0.940/tencentcloud/cbs/v20170312/cbs_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:24:21.000000 tencentcloud-sdk-python-cbs-3.0.940/tencentcloud/cbs/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7755 2023-07-21 00:24:21.000000 tencentcloud-sdk-python-cbs-3.0.940/tencentcloud/cbs/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   239960 2023-07-21 00:24:21.000000 tencentcloud-sdk-python-cbs-3.0.940/tencentcloud/cbs/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-21 00:24:21.000000 tencentcloud-sdk-python-cbs-3.0.940/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-21 00:24:21.000000 tencentcloud-sdk-python-cbs-3.0.940/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-21 00:24:21.000000 tencentcloud-sdk-python-cbs-3.0.940/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:32:19.000000 tencentcloud-sdk-python-cbs-3.0.941/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:32:19.000000 tencentcloud-sdk-python-cbs-3.0.941/tencentcloud_sdk_python_cbs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 00:32:19.000000 tencentcloud-sdk-python-cbs-3.0.941/tencentcloud_sdk_python_cbs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-24 00:32:19.000000 tencentcloud-sdk-python-cbs-3.0.941/tencentcloud_sdk_python_cbs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-24 00:32:19.000000 tencentcloud-sdk-python-cbs-3.0.941/tencentcloud_sdk_python_cbs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-24 00:32:19.000000 tencentcloud-sdk-python-cbs-3.0.941/tencentcloud_sdk_python_cbs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-24 00:32:19.000000 tencentcloud-sdk-python-cbs-3.0.941/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:32:19.000000 tencentcloud-sdk-python-cbs-3.0.941/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-24 00:32:19.000000 tencentcloud-sdk-python-cbs-3.0.941/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:32:19.000000 tencentcloud-sdk-python-cbs-3.0.941/tencentcloud/cbs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:32:19.000000 tencentcloud-sdk-python-cbs-3.0.941/tencentcloud/cbs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:32:19.000000 tencentcloud-sdk-python-cbs-3.0.941/tencentcloud/cbs/v20170312/
+-rw-r--r--   0 root         (0) root         (0)    51002 2023-07-24 00:32:19.000000 tencentcloud-sdk-python-cbs-3.0.941/tencentcloud/cbs/v20170312/cbs_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:32:19.000000 tencentcloud-sdk-python-cbs-3.0.941/tencentcloud/cbs/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7755 2023-07-24 00:32:19.000000 tencentcloud-sdk-python-cbs-3.0.941/tencentcloud/cbs/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   227562 2023-07-24 00:32:19.000000 tencentcloud-sdk-python-cbs-3.0.941/tencentcloud/cbs/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-24 00:32:19.000000 tencentcloud-sdk-python-cbs-3.0.941/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-24 00:32:19.000000 tencentcloud-sdk-python-cbs-3.0.941/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-24 00:32:19.000000 tencentcloud-sdk-python-cbs-3.0.941/README.rst
```

### Comparing `tencentcloud-sdk-python-cbs-3.0.940/tencentcloud_sdk_python_cbs.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cbs-3.0.941/tencentcloud_sdk_python_cbs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cbs
-Version: 3.0.940
+Version: 3.0.941
 Summary: Tencent Cloud Cbs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cbs-3.0.940/setup.py` & `tencentcloud-sdk-python-cbs-3.0.941/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cbs-3.0.940/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cbs-3.0.941/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cbs-3.0.940/tencentcloud/cbs/v20170312/cbs_client.py` & `tencentcloud-sdk-python-cbs-3.0.941/tencentcloud/cbs/v20170312/cbs_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -429,39 +429,14 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeDiskOperationLogs(self, request):
-        """接口已废弃，切换至云审计接口。见https://tapd.woa.com/pro/prong/stories/view/1010114221880719007
-
-        查询云盘操作日志功能已迁移至LookUpEvents接口（https://cloud.tencent.com/document/product/629/12359），本接口（DescribeDiskOperationLogs）即将下线，后续不再提供调用，请知悉。
-
-        :param request: Request instance for DescribeDiskOperationLogs.
-        :type request: :class:`tencentcloud.cbs.v20170312.models.DescribeDiskOperationLogsRequest`
-        :rtype: :class:`tencentcloud.cbs.v20170312.models.DescribeDiskOperationLogsResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DescribeDiskOperationLogs", params, headers=headers)
-            response = json.loads(body)
-            model = models.DescribeDiskOperationLogsResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(type(e).__name__, str(e))
-
-
     def DescribeDiskStoragePool(self, request):
         """本接口（DescribeDiskStoragePool）查询用户的云硬盘独享集群列表。
 
         * 可以根据独享集群ID(CdcId)、可用区(zone)等信息来查询和过滤云硬盘独享集群详细信息，不同的过滤条件之间为与(AND)的关系，过滤信息详细请见过滤器`Filter`。
         * 如果参数为空，返回当前用户一定数量（`Limit`所指定的数量，默认为20）的云硬盘独享集群列表。
 
         :param request: Request instance for DescribeDiskStoragePool.
@@ -529,39 +504,14 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
-
-
-    def DescribeSnapshotOperationLogs(self, request):
-        """接口已废弃，切换至云审计接口。见https://tapd.woa.com/pro/prong/stories/view/1010114221880719007
-
-        查询快照操作日志功能已迁移至LookUpEvents接口（https://cloud.tencent.com/document/product/629/12359），本接口（DescribeSnapshotOperationLogs）即将下线，后续不再提供调用，请知悉。
-
-        :param request: Request instance for DescribeSnapshotOperationLogs.
-        :type request: :class:`tencentcloud.cbs.v20170312.models.DescribeSnapshotOperationLogsRequest`
-        :rtype: :class:`tencentcloud.cbs.v20170312.models.DescribeSnapshotOperationLogsResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DescribeSnapshotOperationLogs", params, headers=headers)
-            response = json.loads(body)
-            model = models.DescribeSnapshotOperationLogsResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSnapshotSharePermission(self, request):
         """本接口（DescribeSnapshotSharePermission）用于查询快照的分享信息。
 
         :param request: Request instance for DescribeSnapshotSharePermission.
         :type request: :class:`tencentcloud.cbs.v20170312.models.DescribeSnapshotSharePermissionRequest`
```

### Comparing `tencentcloud-sdk-python-cbs-3.0.940/tencentcloud/cbs/v20170312/errorcodes.py` & `tencentcloud-sdk-python-cbs-3.0.941/tencentcloud/cbs/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cbs-3.0.940/tencentcloud/cbs/v20170312/models.py` & `tencentcloud-sdk-python-cbs-3.0.941/tencentcloud/cbs/v20170312/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -2441,119 +2441,14 @@
             for item in params.get("DiskConfigSet"):
                 obj = DiskConfig()
                 obj._deserialize(item)
                 self._DiskConfigSet.append(obj)
         self._RequestId = params.get("RequestId")
 
 
-class DescribeDiskOperationLogsRequest(AbstractModel):
-    """DescribeDiskOperationLogs请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _Filters: 过滤条件。支持以下条件：
-<li>disk-id - Array of String - 是否必填：是 - 按云盘ID过滤，每个请求最多可指定10个云盘ID。
-        :type Filters: list of Filter
-        :param _EndTime: 要查询的操作日志的截止时间，例如：“2019-11-22 23:59:59"
-        :type EndTime: str
-        :param _BeginTime: 要查询的操作日志的起始时间，例如：“2019-11-22 00:00:00"
-        :type BeginTime: str
-        """
-        self._Filters = None
-        self._EndTime = None
-        self._BeginTime = None
-
-    @property
-    def Filters(self):
-        return self._Filters
-
-    @Filters.setter
-    def Filters(self, Filters):
-        self._Filters = Filters
-
-    @property
-    def EndTime(self):
-        return self._EndTime
-
-    @EndTime.setter
-    def EndTime(self, EndTime):
-        self._EndTime = EndTime
-
-    @property
-    def BeginTime(self):
-        return self._BeginTime
-
-    @BeginTime.setter
-    def BeginTime(self, BeginTime):
-        self._BeginTime = BeginTime
-
-
-    def _deserialize(self, params):
-        if params.get("Filters") is not None:
-            self._Filters = []
-            for item in params.get("Filters"):
-                obj = Filter()
-                obj._deserialize(item)
-                self._Filters.append(obj)
-        self._EndTime = params.get("EndTime")
-        self._BeginTime = params.get("BeginTime")
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
-class DescribeDiskOperationLogsResponse(AbstractModel):
-    """DescribeDiskOperationLogs返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _DiskOperationLogSet: 云盘的操作日志列表。
-        :type DiskOperationLogSet: list of DiskOperationLog
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._DiskOperationLogSet = None
-        self._RequestId = None
-
-    @property
-    def DiskOperationLogSet(self):
-        return self._DiskOperationLogSet
-
-    @DiskOperationLogSet.setter
-    def DiskOperationLogSet(self, DiskOperationLogSet):
-        self._DiskOperationLogSet = DiskOperationLogSet
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
-        if params.get("DiskOperationLogSet") is not None:
-            self._DiskOperationLogSet = []
-            for item in params.get("DiskOperationLogSet"):
-                obj = DiskOperationLog()
-                obj._deserialize(item)
-                self._DiskOperationLogSet.append(obj)
-        self._RequestId = params.get("RequestId")
-
-
 class DescribeDiskStoragePoolRequest(AbstractModel):
     """DescribeDiskStoragePool请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -2930,119 +2825,14 @@
             for item in params.get("AttachDetail"):
                 obj = AttachDetail()
                 obj._deserialize(item)
                 self._AttachDetail.append(obj)
         self._RequestId = params.get("RequestId")
 
 
-class DescribeSnapshotOperationLogsRequest(AbstractModel):
-    """DescribeSnapshotOperationLogs请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _Filters: 过滤条件。支持以下条件：
-<li>snapshot-id - Array of String - 是否必填：是 - 按快照ID过滤，每个请求最多可指定10个快照ID。
-        :type Filters: list of Filter
-        :param _EndTime: 要查询的操作日志的截止时间，例如：“2019-11-22 23:59:59"
-        :type EndTime: str
-        :param _BeginTime: 要查询的操作日志的起始时间，例如：“2019-11-22 00:00:00"
-        :type BeginTime: str
-        """
-        self._Filters = None
-        self._EndTime = None
-        self._BeginTime = None
-
-    @property
-    def Filters(self):
-        return self._Filters
-
-    @Filters.setter
-    def Filters(self, Filters):
-        self._Filters = Filters
-
-    @property
-    def EndTime(self):
-        return self._EndTime
-
-    @EndTime.setter
-    def EndTime(self, EndTime):
-        self._EndTime = EndTime
-
-    @property
-    def BeginTime(self):
-        return self._BeginTime
-
-    @BeginTime.setter
-    def BeginTime(self, BeginTime):
-        self._BeginTime = BeginTime
-
-
-    def _deserialize(self, params):
-        if params.get("Filters") is not None:
-            self._Filters = []
-            for item in params.get("Filters"):
-                obj = Filter()
-                obj._deserialize(item)
-                self._Filters.append(obj)
-        self._EndTime = params.get("EndTime")
-        self._BeginTime = params.get("BeginTime")
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
-class DescribeSnapshotOperationLogsResponse(AbstractModel):
-    """DescribeSnapshotOperationLogs返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _SnapshotOperationLogSet: 快照操作日志列表。
-        :type SnapshotOperationLogSet: list of SnapshotOperationLog
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._SnapshotOperationLogSet = None
-        self._RequestId = None
-
-    @property
-    def SnapshotOperationLogSet(self):
-        return self._SnapshotOperationLogSet
-
-    @SnapshotOperationLogSet.setter
-    def SnapshotOperationLogSet(self, SnapshotOperationLogSet):
-        self._SnapshotOperationLogSet = SnapshotOperationLogSet
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
-        if params.get("SnapshotOperationLogSet") is not None:
-            self._SnapshotOperationLogSet = []
-            for item in params.get("SnapshotOperationLogSet"):
-                obj = SnapshotOperationLog()
-                obj._deserialize(item)
-                self._SnapshotOperationLogSet.append(obj)
-        self._RequestId = params.get("RequestId")
-
-
 class DescribeSnapshotSharePermissionRequest(AbstractModel):
     """DescribeSnapshotSharePermission请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -4403,119 +4193,14 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class DiskOperationLog(AbstractModel):
-    """云盘操作日志。
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _OperationState: 操作的状态。取值范围：
-SUCCESS :表示操作成功 
-FAILED :表示操作失败 
-PROCESSING :表示操作中。
-        :type OperationState: str
-        :param _StartTime: 开始时间。
-        :type StartTime: str
-        :param _Operator: 操作者的UIN。
-        :type Operator: str
-        :param _Operation: 操作类型。取值范围：
-CBS_OPERATION_ATTACH：挂载云硬盘
-CBS_OPERATION_DETACH：解挂云硬盘
-CBS_OPERATION_RENEW：续费
-CBS_OPERATION_EXPAND：扩容
-CBS_OPERATION_CREATE：创建
-CBS_OPERATION_ISOLATE：隔离
-CBS_OPERATION_MODIFY：修改云硬盘属性
-ASP_OPERATION_BIND：关联定期快照策略
-ASP_OPERATION_UNBIND：取消关联定期快照策略
-        :type Operation: str
-        :param _EndTime: 结束时间。
-        :type EndTime: str
-        :param _DiskId: 操作的云盘ID。
-        :type DiskId: str
-        """
-        self._OperationState = None
-        self._StartTime = None
-        self._Operator = None
-        self._Operation = None
-        self._EndTime = None
-        self._DiskId = None
-
-    @property
-    def OperationState(self):
-        return self._OperationState
-
-    @OperationState.setter
-    def OperationState(self, OperationState):
-        self._OperationState = OperationState
-
-    @property
-    def StartTime(self):
-        return self._StartTime
-
-    @StartTime.setter
-    def StartTime(self, StartTime):
-        self._StartTime = StartTime
-
-    @property
-    def Operator(self):
-        return self._Operator
-
-    @Operator.setter
-    def Operator(self, Operator):
-        self._Operator = Operator
-
-    @property
-    def Operation(self):
-        return self._Operation
-
-    @Operation.setter
-    def Operation(self, Operation):
-        self._Operation = Operation
-
-    @property
-    def EndTime(self):
-        return self._EndTime
-
-    @EndTime.setter
-    def EndTime(self, EndTime):
-        self._EndTime = EndTime
-
-    @property
-    def DiskId(self):
-        return self._DiskId
-
-    @DiskId.setter
-    def DiskId(self, DiskId):
-        self._DiskId = DiskId
-
-
-    def _deserialize(self, params):
-        self._OperationState = params.get("OperationState")
-        self._StartTime = params.get("StartTime")
-        self._Operator = params.get("Operator")
-        self._Operation = params.get("Operation")
-        self._EndTime = params.get("EndTime")
-        self._DiskId = params.get("DiskId")
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
 class Filter(AbstractModel):
     """描述键值对过滤器，用于条件过滤查询。
 
     """
 
     def __init__(self):
         r"""
@@ -6991,118 +6676,14 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class SnapshotOperationLog(AbstractModel):
-    """快照操作日志，已废弃。
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _OperationState: 操作的状态。取值范围：
-SUCCESS :表示操作成功 
-FAILED :表示操作失败 
-PROCESSING :表示操作中。
-        :type OperationState: str
-        :param _StartTime: 开始时间。
-        :type StartTime: str
-        :param _Operator: 操作者的UIN。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Operator: str
-        :param _SnapshotId: 操作的快照ID。
-        :type SnapshotId: str
-        :param _Operation: 操作类型。取值范围：
-SNAP_OPERATION_DELETE：删除快照
-SNAP_OPERATION_ROLLBACK：回滚快照
-SNAP_OPERATION_MODIFY：修改快照属性
-SNAP_OPERATION_CREATE：创建快照
-SNAP_OPERATION_COPY：跨地域复制快照
-ASP_OPERATION_CREATE_SNAP：由定期快照策略创建快照
-ASP_OPERATION_DELETE_SNAP：由定期快照策略删除快照
-        :type Operation: str
-        :param _EndTime: 结束时间。
-        :type EndTime: str
-        """
-        self._OperationState = None
-        self._StartTime = None
-        self._Operator = None
-        self._SnapshotId = None
-        self._Operation = None
-        self._EndTime = None
-
-    @property
-    def OperationState(self):
-        return self._OperationState
-
-    @OperationState.setter
-    def OperationState(self, OperationState):
-        self._OperationState = OperationState
-
-    @property
-    def StartTime(self):
-        return self._StartTime
-
-    @StartTime.setter
-    def StartTime(self, StartTime):
-        self._StartTime = StartTime
-
-    @property
-    def Operator(self):
-        return self._Operator
-
-    @Operator.setter
-    def Operator(self, Operator):
-        self._Operator = Operator
-
-    @property
-    def SnapshotId(self):
-        return self._SnapshotId
-
-    @SnapshotId.setter
-    def SnapshotId(self, SnapshotId):
-        self._SnapshotId = SnapshotId
-
-    @property
-    def Operation(self):
-        return self._Operation
-
-    @Operation.setter
-    def Operation(self, Operation):
-        self._Operation = Operation
-
-    @property
-    def EndTime(self):
-        return self._EndTime
-
-    @EndTime.setter
-    def EndTime(self, EndTime):
-        self._EndTime = EndTime
-
-
-    def _deserialize(self, params):
-        self._OperationState = params.get("OperationState")
-        self._StartTime = params.get("StartTime")
-        self._Operator = params.get("Operator")
-        self._SnapshotId = params.get("SnapshotId")
-        self._Operation = params.get("Operation")
-        self._EndTime = params.get("EndTime")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class Tag(AbstractModel):
     """标签。
 
     """
```

### Comparing `tencentcloud-sdk-python-cbs-3.0.940/PKG-INFO` & `tencentcloud-sdk-python-cbs-3.0.941/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cbs
-Version: 3.0.940
+Version: 3.0.941
 Summary: Tencent Cloud Cbs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cbs-3.0.940/README.rst` & `tencentcloud-sdk-python-cbs-3.0.941/README.rst`

 * *Files identical despite different names*

