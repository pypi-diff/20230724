# Comparing `tmp/tencentcloud-sdk-python-tiw-3.0.940.tar.gz` & `tmp/tencentcloud-sdk-python-tiw-3.0.941.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tiw-3.0.940.tar", last modified: Fri Jul 21 00:51:51 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tiw-3.0.941.tar", last modified: Mon Jul 24 00:46:24 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tiw-3.0.940.tar` & `tencentcloud-sdk-python-tiw-3.0.941.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:51:51.000000 tencentcloud-sdk-python-tiw-3.0.940/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:51:51.000000 tencentcloud-sdk-python-tiw-3.0.940/tencentcloud_sdk_python_tiw.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 00:51:51.000000 tencentcloud-sdk-python-tiw-3.0.940/tencentcloud_sdk_python_tiw.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-21 00:51:51.000000 tencentcloud-sdk-python-tiw-3.0.940/tencentcloud_sdk_python_tiw.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-21 00:51:51.000000 tencentcloud-sdk-python-tiw-3.0.940/tencentcloud_sdk_python_tiw.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-21 00:51:51.000000 tencentcloud-sdk-python-tiw-3.0.940/tencentcloud_sdk_python_tiw.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-21 00:51:51.000000 tencentcloud-sdk-python-tiw-3.0.940/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:51:51.000000 tencentcloud-sdk-python-tiw-3.0.940/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:51:51.000000 tencentcloud-sdk-python-tiw-3.0.940/tencentcloud/tiw/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:51:51.000000 tencentcloud-sdk-python-tiw-3.0.940/tencentcloud/tiw/v20190919/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:51:51.000000 tencentcloud-sdk-python-tiw-3.0.940/tencentcloud/tiw/v20190919/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6089 2023-07-21 00:51:51.000000 tencentcloud-sdk-python-tiw-3.0.940/tencentcloud/tiw/v20190919/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    60499 2023-07-21 00:51:51.000000 tencentcloud-sdk-python-tiw-3.0.940/tencentcloud/tiw/v20190919/tiw_client.py
--rw-r--r--   0 root         (0) root         (0)   281650 2023-07-21 00:51:51.000000 tencentcloud-sdk-python-tiw-3.0.940/tencentcloud/tiw/v20190919/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:51:51.000000 tencentcloud-sdk-python-tiw-3.0.940/tencentcloud/tiw/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-21 00:51:51.000000 tencentcloud-sdk-python-tiw-3.0.940/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-21 00:51:51.000000 tencentcloud-sdk-python-tiw-3.0.940/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-21 00:51:51.000000 tencentcloud-sdk-python-tiw-3.0.940/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-21 00:51:51.000000 tencentcloud-sdk-python-tiw-3.0.940/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:46:24.000000 tencentcloud-sdk-python-tiw-3.0.941/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:46:24.000000 tencentcloud-sdk-python-tiw-3.0.941/tencentcloud_sdk_python_tiw.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 00:46:24.000000 tencentcloud-sdk-python-tiw-3.0.941/tencentcloud_sdk_python_tiw.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-24 00:46:24.000000 tencentcloud-sdk-python-tiw-3.0.941/tencentcloud_sdk_python_tiw.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-24 00:46:24.000000 tencentcloud-sdk-python-tiw-3.0.941/tencentcloud_sdk_python_tiw.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-24 00:46:24.000000 tencentcloud-sdk-python-tiw-3.0.941/tencentcloud_sdk_python_tiw.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-24 00:46:24.000000 tencentcloud-sdk-python-tiw-3.0.941/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:46:24.000000 tencentcloud-sdk-python-tiw-3.0.941/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:46:24.000000 tencentcloud-sdk-python-tiw-3.0.941/tencentcloud/tiw/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:46:24.000000 tencentcloud-sdk-python-tiw-3.0.941/tencentcloud/tiw/v20190919/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:46:24.000000 tencentcloud-sdk-python-tiw-3.0.941/tencentcloud/tiw/v20190919/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6089 2023-07-24 00:46:24.000000 tencentcloud-sdk-python-tiw-3.0.941/tencentcloud/tiw/v20190919/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    61449 2023-07-24 00:46:24.000000 tencentcloud-sdk-python-tiw-3.0.941/tencentcloud/tiw/v20190919/tiw_client.py
+-rw-r--r--   0 root         (0) root         (0)   284659 2023-07-24 00:46:24.000000 tencentcloud-sdk-python-tiw-3.0.941/tencentcloud/tiw/v20190919/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:46:24.000000 tencentcloud-sdk-python-tiw-3.0.941/tencentcloud/tiw/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-24 00:46:24.000000 tencentcloud-sdk-python-tiw-3.0.941/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-24 00:46:24.000000 tencentcloud-sdk-python-tiw-3.0.941/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-24 00:46:24.000000 tencentcloud-sdk-python-tiw-3.0.941/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-24 00:46:24.000000 tencentcloud-sdk-python-tiw-3.0.941/README.rst
```

### Comparing `tencentcloud-sdk-python-tiw-3.0.940/tencentcloud_sdk_python_tiw.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tiw-3.0.941/tencentcloud_sdk_python_tiw.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tiw
-Version: 3.0.940
+Version: 3.0.941
 Summary: Tencent Cloud Tiw SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tiw-3.0.940/setup.py` & `tencentcloud-sdk-python-tiw-3.0.941/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tiw-3.0.940/tencentcloud/tiw/v20190919/errorcodes.py` & `tencentcloud-sdk-python-tiw-3.0.941/tencentcloud/tiw/v20190919/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tiw-3.0.940/tencentcloud/tiw/v20190919/tiw_client.py` & `tencentcloud-sdk-python-tiw-3.0.941/tencentcloud/tiw/v20190919/tiw_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -647,14 +647,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def DescribeTranscodeByUrl(self, request):
+        """通过文档URL查询转码任务，返回最近的一次转码结果
+
+        :param request: Request instance for DescribeTranscodeByUrl.
+        :type request: :class:`tencentcloud.tiw.v20190919.models.DescribeTranscodeByUrlRequest`
+        :rtype: :class:`tencentcloud.tiw.v20190919.models.DescribeTranscodeByUrlResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeTranscodeByUrl", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeTranscodeByUrlResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def DescribeTranscodeCallback(self, request):
         """查询文档转码回调地址
 
         :param request: Request instance for DescribeTranscodeCallback.
         :type request: :class:`tencentcloud.tiw.v20190919.models.DescribeTranscodeCallbackRequest`
         :rtype: :class:`tencentcloud.tiw.v20190919.models.DescribeTranscodeCallbackResponse`
```

### Comparing `tencentcloud-sdk-python-tiw-3.0.940/tencentcloud/tiw/v20190919/models.py` & `tencentcloud-sdk-python-tiw-3.0.941/tencentcloud/tiw/v20190919/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -3379,14 +3379,124 @@
                 obj = RoomUsageDataItem()
                 obj._deserialize(item)
                 self._Usages.append(obj)
         self._Total = params.get("Total")
         self._RequestId = params.get("RequestId")
 
 
+class DescribeTranscodeByUrlRequest(AbstractModel):
+    """DescribeTranscodeByUrl请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _SdkAppId: 客户的SdkAppId
+        :type SdkAppId: int
+        :param _Url: 经过URL编码后的转码文件地址。URL 编码会将字符转换为可通过因特网传输的格式，比如文档地址为http://example.com/测试.pdf，经过URL编码之后为http://example.com/%E6%B5%8B%E8%AF%95.pdf。为了提高URL解析的成功率，请对URL进行编码。	
+        :type Url: str
+        """
+        self._SdkAppId = None
+        self._Url = None
+
+    @property
+    def SdkAppId(self):
+        return self._SdkAppId
+
+    @SdkAppId.setter
+    def SdkAppId(self, SdkAppId):
+        self._SdkAppId = SdkAppId
+
+    @property
+    def Url(self):
+        return self._Url
+
+    @Url.setter
+    def Url(self, Url):
+        self._Url = Url
+
+
+    def _deserialize(self, params):
+        self._SdkAppId = params.get("SdkAppId")
+        self._Url = params.get("Url")
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
+class DescribeTranscodeByUrlResponse(AbstractModel):
+    """DescribeTranscodeByUrl返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Progress: 转码的当前进度,取值范围为0~100
+        :type Progress: int
+        :param _Status: 任务的当前状态
+- QUEUED: 正在排队等待转换
+- PROCESSING: 转换中
+- FINISHED: 转换完成
+- EXCEPTION: 转换异常
+        :type Status: str
+        :param _TaskId: 转码任务的唯一标识Id
+        :type TaskId: str
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Progress = None
+        self._Status = None
+        self._TaskId = None
+        self._RequestId = None
+
+    @property
+    def Progress(self):
+        return self._Progress
+
+    @Progress.setter
+    def Progress(self, Progress):
+        self._Progress = Progress
+
+    @property
+    def Status(self):
+        return self._Status
+
+    @Status.setter
+    def Status(self, Status):
+        self._Status = Status
+
+    @property
+    def TaskId(self):
+        return self._TaskId
+
+    @TaskId.setter
+    def TaskId(self, TaskId):
+        self._TaskId = TaskId
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
+        self._Progress = params.get("Progress")
+        self._Status = params.get("Status")
+        self._TaskId = params.get("TaskId")
+        self._RequestId = params.get("RequestId")
+
+
 class DescribeTranscodeCallbackRequest(AbstractModel):
     """DescribeTranscodeCallback请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-tiw-3.0.940/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tiw-3.0.941/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tiw-3.0.940/PKG-INFO` & `tencentcloud-sdk-python-tiw-3.0.941/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tiw
-Version: 3.0.940
+Version: 3.0.941
 Summary: Tencent Cloud Tiw SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tiw-3.0.940/README.rst` & `tencentcloud-sdk-python-tiw-3.0.941/README.rst`

 * *Files identical despite different names*

