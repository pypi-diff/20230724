# Comparing `tmp/openi-beta-2.0.1.tar.gz` & `tmp/openi-beta-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openi-beta-2.0.1.tar", last modified: Mon Jul 24 09:19:00 2023, max compression
+gzip compressed data, was "openi-beta-2.0.2.tar", last modified: Mon Jul 24 09:36:03 2023, max compression
```

## Comparing `openi-beta-2.0.1.tar` & `openi-beta-2.0.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 09:19:00.972297 openi-beta-2.0.1/
--rw-rw-rw-   0        0        0     5381 2023-07-24 09:19:00.972297 openi-beta-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4735 2023-07-24 07:49:31.000000 openi-beta-2.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-24 09:19:00.972297 openi-beta-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1290 2023-07-24 09:18:38.000000 openi-beta-2.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:19:00.924788 openi-beta-2.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-24 09:19:00.930785 openi-beta-2.0.1/src/openi/
--rw-rw-rw-   0        0        0      194 2023-07-24 07:15:17.000000 openi-beta-2.0.1/src/openi/__init__.py
--rw-rw-rw-   0        0        0     6459 2023-07-24 07:13:05.000000 openi-beta-2.0.1/src/openi/apis.py
--rw-rw-rw-   0        0        0     5238 2023-07-24 07:13:04.000000 openi-beta-2.0.1/src/openi/cli.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:19:00.934785 openi-beta-2.0.1/src/openi/cloudbrain/
--rw-rw-rw-   0        0        0       84 2023-07-24 07:06:23.000000 openi-beta-2.0.1/src/openi/cloudbrain/__init__.py
--rw-rw-rw-   0        0        0     1609 2023-07-24 07:06:26.000000 openi-beta-2.0.1/src/openi/cloudbrain/env_check.py
--rw-rw-rw-   0        0        0     5313 2023-07-24 07:06:29.000000 openi-beta-2.0.1/src/openi/cloudbrain/helper.py
--rw-rw-rw-   0        0        0     1559 2023-07-24 07:06:31.000000 openi-beta-2.0.1/src/openi/cloudbrain/minio_operate.py
--rw-rw-rw-   0        0        0     2886 2023-07-24 07:06:32.000000 openi-beta-2.0.1/src/openi/cloudbrain/obs_operate.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:19:00.944790 openi-beta-2.0.1/src/openi/dataset/
--rw-rw-rw-   0        0        0      109 2023-07-24 07:06:34.000000 openi-beta-2.0.1/src/openi/dataset/__init__.py
--rw-rw-rw-   0        0        0     2855 2023-07-24 07:06:35.000000 openi-beta-2.0.1/src/openi/dataset/dataset_file.py
--rw-rw-rw-   0        0        0     2685 2023-07-24 07:20:32.000000 openi-beta-2.0.1/src/openi/dataset/download.py
--rw-rw-rw-   0        0        0     4669 2023-07-24 09:18:26.000000 openi-beta-2.0.1/src/openi/dataset/upload.py
--rw-rw-rw-   0        0        0     3356 2023-07-24 07:13:03.000000 openi-beta-2.0.1/src/openi/login.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:19:00.946792 openi-beta-2.0.1/src/openi/path/
--rw-rw-rw-   0        0        0       21 2023-07-24 07:06:52.000000 openi-beta-2.0.1/src/openi/path/__init__.py
--rw-rw-rw-   0        0        0     2405 2023-07-24 07:07:00.000000 openi-beta-2.0.1/src/openi/path/path.py
--rw-rw-rw-   0        0        0     4081 2023-07-24 07:13:02.000000 openi-beta-2.0.1/src/openi/settings.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:19:00.956305 openi-beta-2.0.1/src/openi/utils/
--rw-rw-rw-   0        0        0       50 2023-07-24 07:07:03.000000 openi-beta-2.0.1/src/openi/utils/__init__.py
--rw-rw-rw-   0        0        0     2197 2023-07-24 07:07:05.000000 openi-beta-2.0.1/src/openi/utils/file_utils.py
--rw-rw-rw-   0        0        0      723 2023-07-24 07:07:16.000000 openi-beta-2.0.1/src/openi/utils/logger.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:19:00.970297 openi-beta-2.0.1/src/openi_beta.egg-info/
--rw-rw-rw-   0        0        0     5381 2023-07-24 09:19:00.000000 openi-beta-2.0.1/src/openi_beta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      787 2023-07-24 09:19:00.000000 openi-beta-2.0.1/src/openi_beta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 09:19:00.000000 openi-beta-2.0.1/src/openi_beta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-07-24 09:19:00.000000 openi-beta-2.0.1/src/openi_beta.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2023-07-24 09:19:00.000000 openi-beta-2.0.1/src/openi_beta.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-24 09:19:00.000000 openi-beta-2.0.1/src/openi_beta.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-24 09:19:00.971297 openi-beta-2.0.1/test/
--rw-rw-rw-   0        0        0       87 2023-07-24 07:35:25.000000 openi-beta-2.0.1/test/test.py
+drwxrwxrwx   0        0        0        0 2023-07-24 09:36:03.871833 openi-beta-2.0.2/
+-rw-rw-rw-   0        0        0     5381 2023-07-24 09:36:03.871833 openi-beta-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4735 2023-07-24 07:49:31.000000 openi-beta-2.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-24 09:36:03.872833 openi-beta-2.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1290 2023-07-24 09:35:46.000000 openi-beta-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 09:36:03.840204 openi-beta-2.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-24 09:36:03.846206 openi-beta-2.0.2/src/openi/
+-rw-rw-rw-   0        0        0      194 2023-07-24 07:15:17.000000 openi-beta-2.0.2/src/openi/__init__.py
+-rw-rw-rw-   0        0        0     6459 2023-07-24 07:13:05.000000 openi-beta-2.0.2/src/openi/apis.py
+-rw-rw-rw-   0        0        0     5238 2023-07-24 07:13:04.000000 openi-beta-2.0.2/src/openi/cli.py
+drwxrwxrwx   0        0        0        0 2023-07-24 09:36:03.850204 openi-beta-2.0.2/src/openi/cloudbrain/
+-rw-rw-rw-   0        0        0       84 2023-07-24 07:06:23.000000 openi-beta-2.0.2/src/openi/cloudbrain/__init__.py
+-rw-rw-rw-   0        0        0     1609 2023-07-24 07:06:26.000000 openi-beta-2.0.2/src/openi/cloudbrain/env_check.py
+-rw-rw-rw-   0        0        0     5313 2023-07-24 07:06:29.000000 openi-beta-2.0.2/src/openi/cloudbrain/helper.py
+-rw-rw-rw-   0        0        0     1559 2023-07-24 07:06:31.000000 openi-beta-2.0.2/src/openi/cloudbrain/minio_operate.py
+-rw-rw-rw-   0        0        0     2886 2023-07-24 07:06:32.000000 openi-beta-2.0.2/src/openi/cloudbrain/obs_operate.py
+drwxrwxrwx   0        0        0        0 2023-07-24 09:36:03.853204 openi-beta-2.0.2/src/openi/dataset/
+-rw-rw-rw-   0        0        0      109 2023-07-24 07:06:34.000000 openi-beta-2.0.2/src/openi/dataset/__init__.py
+-rw-rw-rw-   0        0        0     2855 2023-07-24 07:06:35.000000 openi-beta-2.0.2/src/openi/dataset/dataset_file.py
+-rw-rw-rw-   0        0        0     2685 2023-07-24 07:20:32.000000 openi-beta-2.0.2/src/openi/dataset/download.py
+-rw-rw-rw-   0        0        0     4669 2023-07-24 09:18:26.000000 openi-beta-2.0.2/src/openi/dataset/upload.py
+-rw-rw-rw-   0        0        0     3356 2023-07-24 07:13:03.000000 openi-beta-2.0.2/src/openi/login.py
+drwxrwxrwx   0        0        0        0 2023-07-24 09:36:03.855203 openi-beta-2.0.2/src/openi/path/
+-rw-rw-rw-   0        0        0       21 2023-07-24 07:06:52.000000 openi-beta-2.0.2/src/openi/path/__init__.py
+-rw-rw-rw-   0        0        0     2405 2023-07-24 07:07:00.000000 openi-beta-2.0.2/src/openi/path/path.py
+-rw-rw-rw-   0        0        0     4081 2023-07-24 09:33:32.000000 openi-beta-2.0.2/src/openi/settings.py
+drwxrwxrwx   0        0        0        0 2023-07-24 09:36:03.857203 openi-beta-2.0.2/src/openi/utils/
+-rw-rw-rw-   0        0        0       50 2023-07-24 07:07:03.000000 openi-beta-2.0.2/src/openi/utils/__init__.py
+-rw-rw-rw-   0        0        0     2197 2023-07-24 07:07:05.000000 openi-beta-2.0.2/src/openi/utils/file_utils.py
+-rw-rw-rw-   0        0        0      723 2023-07-24 07:07:16.000000 openi-beta-2.0.2/src/openi/utils/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-24 09:36:03.869833 openi-beta-2.0.2/src/openi_beta.egg-info/
+-rw-rw-rw-   0        0        0     5381 2023-07-24 09:36:03.000000 openi-beta-2.0.2/src/openi_beta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      787 2023-07-24 09:36:03.000000 openi-beta-2.0.2/src/openi_beta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 09:36:03.000000 openi-beta-2.0.2/src/openi_beta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-07-24 09:36:03.000000 openi-beta-2.0.2/src/openi_beta.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-07-24 09:36:03.000000 openi-beta-2.0.2/src/openi_beta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-24 09:36:03.000000 openi-beta-2.0.2/src/openi_beta.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 09:36:03.870832 openi-beta-2.0.2/test/
+-rw-rw-rw-   0        0        0       87 2023-07-24 07:35:25.000000 openi-beta-2.0.2/test/test.py
```

### Comparing `openi-beta-2.0.1/PKG-INFO` & `openi-beta-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-beta
-Version: 2.0.1
+Version: 2.0.2
 Summary: Beta package for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `openi-beta-2.0.1/README.md` & `openi-beta-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.1/setup.py` & `openi-beta-2.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="openi-beta",
-    version="2.0.1",
+    version="2.0.2",
     description="Beta package for openi pypi",
     package_dir={"": "src"},
     packages=find_packages("src"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi",
     author="chenzh05",
```

### Comparing `openi-beta-2.0.1/src/openi/apis.py` & `openi-beta-2.0.2/src/openi/apis.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.1/src/openi/cli.py` & `openi-beta-2.0.2/src/openi/cli.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.1/src/openi/cloudbrain/env_check.py` & `openi-beta-2.0.2/src/openi/cloudbrain/env_check.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.1/src/openi/cloudbrain/helper.py` & `openi-beta-2.0.2/src/openi/cloudbrain/helper.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.1/src/openi/cloudbrain/minio_operate.py` & `openi-beta-2.0.2/src/openi/cloudbrain/minio_operate.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.1/src/openi/cloudbrain/obs_operate.py` & `openi-beta-2.0.2/src/openi/cloudbrain/obs_operate.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.1/src/openi/dataset/dataset_file.py` & `openi-beta-2.0.2/src/openi/dataset/dataset_file.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.1/src/openi/dataset/download.py` & `openi-beta-2.0.2/src/openi/dataset/download.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.1/src/openi/dataset/upload.py` & `openi-beta-2.0.2/src/openi/dataset/upload.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.1/src/openi/login.py` & `openi-beta-2.0.2/src/openi/login.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.1/src/openi/path/path.py` & `openi-beta-2.0.2/src/openi/path/path.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.1/src/openi/settings.py` & `openi-beta-2.0.2/src/openi/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 """
 CLI help 
 """
 
 
 class CLI(object):
     # main help page
-    banner = "OpenI command line tool 启智AI协作社区命令行工具"
+    banner = "OpenI command line tool 启智AI协作平台命令行工具"
 
     usage = "openi {login, whoami, dataset, ...} [<args>] [-h]"
     command_login = "使用令牌登录启智并保存到本机"
     command_logout = "登出当前用户并删除本地令牌文件"
     command_whoami = "查询当前登录用户"
     command_dataset = "{upload,download} 上传/下载启智AI协作平台的数据集 "
 
@@ -66,15 +66,15 @@
     param_endpoint = "选填: 仅内部使用"
 
     # Dataset
     dataset_choices = ["upload", "download"]
     dataset_usage = "openi dataset {upload,download} [<args>] [-h]"
 
     command_dataset_upload = "上传数据集文件，需指定文件名,仓库路径及存储类型"
-    dataset_upload_help = "下载数据集文件, openi dataset upload -h 查看更多说明"
+    dataset_upload_help = "上传数据集文件, openi dataset upload -h 查看更多说明"
     dataset_upload_usage = (
         "openi dataset upload [-f file] [-r repo_id] [-c cluster] [-h]"
     )
     dataset_upload_param_file = "本地文件名称，包含文件路径"
     dataset_upload_param_repo_id = "所在仓库路径，格式为`拥有者/仓库名`，登录用户需要拥有此仓库权限"
     dataset_upload_param_cluster = "选填: 文件的存储集群，不区分大小写，默认为`NPU`"
     # dataset_upload_epilog = textwrap.dedent(
```

### Comparing `openi-beta-2.0.1/src/openi/utils/file_utils.py` & `openi-beta-2.0.2/src/openi/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.1/src/openi/utils/logger.py` & `openi-beta-2.0.2/src/openi/utils/logger.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.1/src/openi_beta.egg-info/PKG-INFO` & `openi-beta-2.0.2/src/openi_beta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-beta
-Version: 2.0.1
+Version: 2.0.2
 Summary: Beta package for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `openi-beta-2.0.1/src/openi_beta.egg-info/SOURCES.txt` & `openi-beta-2.0.2/src/openi_beta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

