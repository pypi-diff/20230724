# Comparing `tmp/tencentcloud-sdk-python-lighthouse-3.0.940.tar.gz` & `tmp/tencentcloud-sdk-python-lighthouse-3.0.941.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-lighthouse-3.0.940.tar", last modified: Fri Jul 21 00:45:04 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-lighthouse-3.0.941.tar", last modified: Mon Jul 24 00:39:29 2023, max compression
```

## Comparing `tencentcloud-sdk-python-lighthouse-3.0.940.tar` & `tencentcloud-sdk-python-lighthouse-3.0.941.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:45:04.000000 tencentcloud-sdk-python-lighthouse-3.0.940/
--rw-r--r--   0 root         (0) root         (0)     1020 2023-07-21 00:45:04.000000 tencentcloud-sdk-python-lighthouse-3.0.940/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:45:04.000000 tencentcloud-sdk-python-lighthouse-3.0.940/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-21 00:45:04.000000 tencentcloud-sdk-python-lighthouse-3.0.940/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:45:04.000000 tencentcloud-sdk-python-lighthouse-3.0.940/tencentcloud/lighthouse/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:45:04.000000 tencentcloud-sdk-python-lighthouse-3.0.940/tencentcloud/lighthouse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:45:04.000000 tencentcloud-sdk-python-lighthouse-3.0.940/tencentcloud/lighthouse/v20200324/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:45:04.000000 tencentcloud-sdk-python-lighthouse-3.0.940/tencentcloud/lighthouse/v20200324/__init__.py
--rw-r--r--   0 root         (0) root         (0)    92864 2023-07-21 00:45:04.000000 tencentcloud-sdk-python-lighthouse-3.0.940/tencentcloud/lighthouse/v20200324/lighthouse_client.py
--rw-r--r--   0 root         (0) root         (0)    26127 2023-07-21 00:45:04.000000 tencentcloud-sdk-python-lighthouse-3.0.940/tencentcloud/lighthouse/v20200324/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   360767 2023-07-21 00:45:04.000000 tencentcloud-sdk-python-lighthouse-3.0.940/tencentcloud/lighthouse/v20200324/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-21 00:45:04.000000 tencentcloud-sdk-python-lighthouse-3.0.940/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1694 2023-07-21 00:45:04.000000 tencentcloud-sdk-python-lighthouse-3.0.940/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      758 2023-07-21 00:45:04.000000 tencentcloud-sdk-python-lighthouse-3.0.940/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:45:04.000000 tencentcloud-sdk-python-lighthouse-3.0.940/tencentcloud_sdk_python_lighthouse.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 00:45:04.000000 tencentcloud-sdk-python-lighthouse-3.0.940/tencentcloud_sdk_python_lighthouse.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      515 2023-07-21 00:45:04.000000 tencentcloud-sdk-python-lighthouse-3.0.940/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-07-21 00:45:04.000000 tencentcloud-sdk-python-lighthouse-3.0.940/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-21 00:45:04.000000 tencentcloud-sdk-python-lighthouse-3.0.940/tencentcloud_sdk_python_lighthouse.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:39:29.000000 tencentcloud-sdk-python-lighthouse-3.0.941/
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-07-24 00:39:29.000000 tencentcloud-sdk-python-lighthouse-3.0.941/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:39:29.000000 tencentcloud-sdk-python-lighthouse-3.0.941/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-24 00:39:29.000000 tencentcloud-sdk-python-lighthouse-3.0.941/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:39:29.000000 tencentcloud-sdk-python-lighthouse-3.0.941/tencentcloud/lighthouse/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:39:29.000000 tencentcloud-sdk-python-lighthouse-3.0.941/tencentcloud/lighthouse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:39:29.000000 tencentcloud-sdk-python-lighthouse-3.0.941/tencentcloud/lighthouse/v20200324/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 00:39:29.000000 tencentcloud-sdk-python-lighthouse-3.0.941/tencentcloud/lighthouse/v20200324/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    92864 2023-07-24 00:39:29.000000 tencentcloud-sdk-python-lighthouse-3.0.941/tencentcloud/lighthouse/v20200324/lighthouse_client.py
+-rw-r--r--   0 root         (0) root         (0)    26127 2023-07-24 00:39:29.000000 tencentcloud-sdk-python-lighthouse-3.0.941/tencentcloud/lighthouse/v20200324/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   360767 2023-07-24 00:39:29.000000 tencentcloud-sdk-python-lighthouse-3.0.941/tencentcloud/lighthouse/v20200324/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-24 00:39:29.000000 tencentcloud-sdk-python-lighthouse-3.0.941/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-07-24 00:39:29.000000 tencentcloud-sdk-python-lighthouse-3.0.941/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      758 2023-07-24 00:39:29.000000 tencentcloud-sdk-python-lighthouse-3.0.941/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:39:29.000000 tencentcloud-sdk-python-lighthouse-3.0.941/tencentcloud_sdk_python_lighthouse.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 00:39:29.000000 tencentcloud-sdk-python-lighthouse-3.0.941/tencentcloud_sdk_python_lighthouse.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      515 2023-07-24 00:39:29.000000 tencentcloud-sdk-python-lighthouse-3.0.941/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-07-24 00:39:29.000000 tencentcloud-sdk-python-lighthouse-3.0.941/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-24 00:39:29.000000 tencentcloud-sdk-python-lighthouse-3.0.941/tencentcloud_sdk_python_lighthouse.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.940/setup.py` & `tencentcloud-sdk-python-lighthouse-3.0.941/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.940/tencentcloud/__init__.py` & `tencentcloud-sdk-python-lighthouse-3.0.941/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.940/tencentcloud/lighthouse/v20200324/lighthouse_client.py` & `tencentcloud-sdk-python-lighthouse-3.0.941/tencentcloud/lighthouse/v20200324/lighthouse_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.940/tencentcloud/lighthouse/v20200324/errorcodes.py` & `tencentcloud-sdk-python-lighthouse-3.0.941/tencentcloud/lighthouse/v20200324/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.940/tencentcloud/lighthouse/v20200324/models.py` & `tencentcloud-sdk-python-lighthouse-3.0.941/tencentcloud/lighthouse/v20200324/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.940/PKG-INFO` & `tencentcloud-sdk-python-lighthouse-3.0.941/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lighthouse
-Version: 3.0.940
+Version: 3.0.941
 Summary: Tencent Cloud Lighthouse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.940/README.rst` & `tencentcloud-sdk-python-lighthouse-3.0.941/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.940/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-lighthouse-3.0.941/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.940/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO` & `tencentcloud-sdk-python-lighthouse-3.0.941/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lighthouse
-Version: 3.0.940
+Version: 3.0.941
 Summary: Tencent Cloud Lighthouse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

