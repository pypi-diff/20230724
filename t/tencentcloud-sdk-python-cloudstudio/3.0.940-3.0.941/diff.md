# Comparing `tmp/tencentcloud-sdk-python-cloudstudio-3.0.940.tar.gz` & `tmp/tencentcloud-sdk-python-cloudstudio-3.0.941.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cloudstudio-3.0.940.tar", last modified: Fri Jul 21 00:25:56 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cloudstudio-3.0.941.tar", last modified: Mon Jul 24 00:33:56 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cloudstudio-3.0.940.tar` & `tencentcloud-sdk-python-cloudstudio-3.0.941.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:25:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.940/
--rw-r--r--   0 root         (0) root         (0)     1022 2023-07-21 00:25:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.940/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:25:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.940/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:25:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.940/tencentcloud/cloudstudio/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:25:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.940/tencentcloud/cloudstudio/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:25:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.940/tencentcloud/cloudstudio/v20210524/
--rw-r--r--   0 root         (0) root         (0)    21897 2023-07-21 00:25:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.940/tencentcloud/cloudstudio/v20210524/cloudstudio_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:25:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.940/tencentcloud/cloudstudio/v20210524/__init__.py
--rw-r--r--   0 root         (0) root         (0)      828 2023-07-21 00:25:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.940/tencentcloud/cloudstudio/v20210524/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   112109 2023-07-21 00:25:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.940/tencentcloud/cloudstudio/v20210524/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:25:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.940/tencentcloud/cloudstudio/v20230508/
--rw-r--r--   0 root         (0) root         (0)     8992 2023-07-21 00:25:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.940/tencentcloud/cloudstudio/v20230508/cloudstudio_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:25:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.940/tencentcloud/cloudstudio/v20230508/__init__.py
--rw-r--r--   0 root         (0) root         (0)      979 2023-07-21 00:25:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.940/tencentcloud/cloudstudio/v20230508/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    33456 2023-07-21 00:25:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.940/tencentcloud/cloudstudio/v20230508/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-21 00:25:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.940/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-21 00:25:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.940/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1699 2023-07-21 00:25:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.940/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      761 2023-07-21 00:25:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.940/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:25:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.940/tencentcloud_sdk_python_cloudstudio.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 00:25:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.940/tencentcloud_sdk_python_cloudstudio.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      723 2023-07-21 00:25:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.940/tencentcloud_sdk_python_cloudstudio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1699 2023-07-21 00:25:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.940/tencentcloud_sdk_python_cloudstudio.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-21 00:25:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.940/tencentcloud_sdk_python_cloudstudio.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:33:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.941/
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-07-24 00:33:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.941/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:33:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.941/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:33:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.941/tencentcloud/cloudstudio/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:33:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.941/tencentcloud/cloudstudio/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:33:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.941/tencentcloud/cloudstudio/v20210524/
+-rw-r--r--   0 root         (0) root         (0)    21897 2023-07-24 00:33:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.941/tencentcloud/cloudstudio/v20210524/cloudstudio_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:33:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.941/tencentcloud/cloudstudio/v20210524/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      828 2023-07-24 00:33:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.941/tencentcloud/cloudstudio/v20210524/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   112109 2023-07-24 00:33:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.941/tencentcloud/cloudstudio/v20210524/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:33:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.941/tencentcloud/cloudstudio/v20230508/
+-rw-r--r--   0 root         (0) root         (0)     8992 2023-07-24 00:33:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.941/tencentcloud/cloudstudio/v20230508/cloudstudio_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:33:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.941/tencentcloud/cloudstudio/v20230508/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      979 2023-07-24 00:33:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.941/tencentcloud/cloudstudio/v20230508/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    33829 2023-07-24 00:33:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.941/tencentcloud/cloudstudio/v20230508/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-24 00:33:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.941/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-24 00:33:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.941/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1699 2023-07-24 00:33:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.941/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      761 2023-07-24 00:33:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.941/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:33:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.941/tencentcloud_sdk_python_cloudstudio.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 00:33:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.941/tencentcloud_sdk_python_cloudstudio.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      723 2023-07-24 00:33:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.941/tencentcloud_sdk_python_cloudstudio.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1699 2023-07-24 00:33:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.941/tencentcloud_sdk_python_cloudstudio.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-24 00:33:56.000000 tencentcloud-sdk-python-cloudstudio-3.0.941/tencentcloud_sdk_python_cloudstudio.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-cloudstudio-3.0.940/setup.py` & `tencentcloud-sdk-python-cloudstudio-3.0.941/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cloudstudio-3.0.940/tencentcloud/cloudstudio/v20210524/cloudstudio_client.py` & `tencentcloud-sdk-python-cloudstudio-3.0.941/tencentcloud/cloudstudio/v20210524/cloudstudio_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cloudstudio-3.0.940/tencentcloud/cloudstudio/v20210524/errorcodes.py` & `tencentcloud-sdk-python-cloudstudio-3.0.941/tencentcloud/cloudstudio/v20210524/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cloudstudio-3.0.940/tencentcloud/cloudstudio/v20210524/models.py` & `tencentcloud-sdk-python-cloudstudio-3.0.941/tencentcloud/cloudstudio/v20210524/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cloudstudio-3.0.940/tencentcloud/cloudstudio/v20230508/cloudstudio_client.py` & `tencentcloud-sdk-python-cloudstudio-3.0.941/tencentcloud/cloudstudio/v20230508/cloudstudio_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cloudstudio-3.0.940/tencentcloud/cloudstudio/v20230508/errorcodes.py` & `tencentcloud-sdk-python-cloudstudio-3.0.941/tencentcloud/cloudstudio/v20230508/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cloudstudio-3.0.940/tencentcloud/cloudstudio/v20230508/models.py` & `tencentcloud-sdk-python-cloudstudio-3.0.941/tencentcloud/cloudstudio/v20230508/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,17 +200,20 @@
 
     def __init__(self):
         r"""
         :param _SpaceKey: 工作空间 SpaceKey
         :type SpaceKey: str
         :param _TokenExpiredLimitSec: token过期时间，单位是秒，默认 3600
         :type TokenExpiredLimitSec: int
+        :param _Policies: token 授权策略，可选值为 workspace-run-only, all。默认为 all
+        :type Policies: list of str
         """
         self._SpaceKey = None
         self._TokenExpiredLimitSec = None
+        self._Policies = None
 
     @property
     def SpaceKey(self):
         return self._SpaceKey
 
     @SpaceKey.setter
     def SpaceKey(self, SpaceKey):
@@ -220,18 +223,27 @@
     def TokenExpiredLimitSec(self):
         return self._TokenExpiredLimitSec
 
     @TokenExpiredLimitSec.setter
     def TokenExpiredLimitSec(self, TokenExpiredLimitSec):
         self._TokenExpiredLimitSec = TokenExpiredLimitSec
 
+    @property
+    def Policies(self):
+        return self._Policies
+
+    @Policies.setter
+    def Policies(self, Policies):
+        self._Policies = Policies
+
 
     def _deserialize(self, params):
         self._SpaceKey = params.get("SpaceKey")
         self._TokenExpiredLimitSec = params.get("TokenExpiredLimitSec")
+        self._Policies = params.get("Policies")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-cloudstudio-3.0.940/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cloudstudio-3.0.941/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cloudstudio-3.0.940/PKG-INFO` & `tencentcloud-sdk-python-cloudstudio-3.0.941/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cloudstudio
-Version: 3.0.940
+Version: 3.0.941
 Summary: Tencent Cloud Cloudstudio SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cloudstudio-3.0.940/README.rst` & `tencentcloud-sdk-python-cloudstudio-3.0.941/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cloudstudio-3.0.940/tencentcloud_sdk_python_cloudstudio.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-cloudstudio-3.0.941/tencentcloud_sdk_python_cloudstudio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cloudstudio-3.0.940/tencentcloud_sdk_python_cloudstudio.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cloudstudio-3.0.941/tencentcloud_sdk_python_cloudstudio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cloudstudio
-Version: 3.0.940
+Version: 3.0.941
 Summary: Tencent Cloud Cloudstudio SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

