# Comparing `tmp/tencentcloud-sdk-python-ic-3.0.940.tar.gz` & `tmp/tencentcloud-sdk-python-ic-3.0.941.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ic-3.0.940.tar", last modified: Fri Jul 21 00:32:29 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ic-3.0.941.tar", last modified: Mon Jul 24 00:38:09 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ic-3.0.940.tar` & `tencentcloud-sdk-python-ic-3.0.941.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:32:29.000000 tencentcloud-sdk-python-ic-3.0.940/
--rw-r--r--   0 root         (0) root         (0)     1004 2023-07-21 00:32:29.000000 tencentcloud-sdk-python-ic-3.0.940/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:32:29.000000 tencentcloud-sdk-python-ic-3.0.940/tencentcloud_sdk_python_ic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 00:32:29.000000 tencentcloud-sdk-python-ic-3.0.940/tencentcloud_sdk_python_ic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      435 2023-07-21 00:32:29.000000 tencentcloud-sdk-python-ic-3.0.940/tencentcloud_sdk_python_ic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-21 00:32:29.000000 tencentcloud-sdk-python-ic-3.0.940/tencentcloud_sdk_python_ic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-21 00:32:29.000000 tencentcloud-sdk-python-ic-3.0.940/tencentcloud_sdk_python_ic.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:32:29.000000 tencentcloud-sdk-python-ic-3.0.940/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:32:29.000000 tencentcloud-sdk-python-ic-3.0.940/tencentcloud/ic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:32:29.000000 tencentcloud-sdk-python-ic-3.0.940/tencentcloud/ic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:32:29.000000 tencentcloud-sdk-python-ic-3.0.940/tencentcloud/ic/v20190307/
--rw-r--r--   0 root         (0) root         (0)     8987 2023-07-21 00:32:29.000000 tencentcloud-sdk-python-ic-3.0.940/tencentcloud/ic/v20190307/ic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:32:29.000000 tencentcloud-sdk-python-ic-3.0.940/tencentcloud/ic/v20190307/__init__.py
--rw-r--r--   0 root         (0) root         (0)      983 2023-07-21 00:32:29.000000 tencentcloud-sdk-python-ic-3.0.940/tencentcloud/ic/v20190307/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    46716 2023-07-21 00:32:29.000000 tencentcloud-sdk-python-ic-3.0.940/tencentcloud/ic/v20190307/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-21 00:32:29.000000 tencentcloud-sdk-python-ic-3.0.940/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-21 00:32:29.000000 tencentcloud-sdk-python-ic-3.0.940/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-21 00:32:29.000000 tencentcloud-sdk-python-ic-3.0.940/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      734 2023-07-21 00:32:29.000000 tencentcloud-sdk-python-ic-3.0.940/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:38:09.000000 tencentcloud-sdk-python-ic-3.0.941/
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-07-24 00:38:09.000000 tencentcloud-sdk-python-ic-3.0.941/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:38:09.000000 tencentcloud-sdk-python-ic-3.0.941/tencentcloud_sdk_python_ic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 00:38:09.000000 tencentcloud-sdk-python-ic-3.0.941/tencentcloud_sdk_python_ic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      435 2023-07-24 00:38:09.000000 tencentcloud-sdk-python-ic-3.0.941/tencentcloud_sdk_python_ic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-24 00:38:09.000000 tencentcloud-sdk-python-ic-3.0.941/tencentcloud_sdk_python_ic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-24 00:38:09.000000 tencentcloud-sdk-python-ic-3.0.941/tencentcloud_sdk_python_ic.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:38:09.000000 tencentcloud-sdk-python-ic-3.0.941/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:38:09.000000 tencentcloud-sdk-python-ic-3.0.941/tencentcloud/ic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:38:09.000000 tencentcloud-sdk-python-ic-3.0.941/tencentcloud/ic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:38:09.000000 tencentcloud-sdk-python-ic-3.0.941/tencentcloud/ic/v20190307/
+-rw-r--r--   0 root         (0) root         (0)     8987 2023-07-24 00:38:09.000000 tencentcloud-sdk-python-ic-3.0.941/tencentcloud/ic/v20190307/ic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:38:09.000000 tencentcloud-sdk-python-ic-3.0.941/tencentcloud/ic/v20190307/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      983 2023-07-24 00:38:09.000000 tencentcloud-sdk-python-ic-3.0.941/tencentcloud/ic/v20190307/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    46716 2023-07-24 00:38:09.000000 tencentcloud-sdk-python-ic-3.0.941/tencentcloud/ic/v20190307/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-24 00:38:09.000000 tencentcloud-sdk-python-ic-3.0.941/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-24 00:38:09.000000 tencentcloud-sdk-python-ic-3.0.941/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-24 00:38:09.000000 tencentcloud-sdk-python-ic-3.0.941/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      734 2023-07-24 00:38:09.000000 tencentcloud-sdk-python-ic-3.0.941/README.rst
```

### Comparing `tencentcloud-sdk-python-ic-3.0.940/setup.py` & `tencentcloud-sdk-python-ic-3.0.941/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ic-3.0.940/tencentcloud_sdk_python_ic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ic-3.0.941/tencentcloud_sdk_python_ic.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ic
-Version: 3.0.940
+Version: 3.0.941
 Summary: Tencent Cloud Ic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ic-3.0.940/tencentcloud/ic/v20190307/ic_client.py` & `tencentcloud-sdk-python-ic-3.0.941/tencentcloud/ic/v20190307/ic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ic-3.0.940/tencentcloud/ic/v20190307/errorcodes.py` & `tencentcloud-sdk-python-ic-3.0.941/tencentcloud/ic/v20190307/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ic-3.0.940/tencentcloud/ic/v20190307/models.py` & `tencentcloud-sdk-python-ic-3.0.941/tencentcloud/ic/v20190307/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ic-3.0.940/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ic-3.0.941/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ic-3.0.940/PKG-INFO` & `tencentcloud-sdk-python-ic-3.0.941/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ic
-Version: 3.0.940
+Version: 3.0.941
 Summary: Tencent Cloud Ic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ic-3.0.940/README.rst` & `tencentcloud-sdk-python-ic-3.0.941/README.rst`

 * *Files identical despite different names*
