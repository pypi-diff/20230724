# Comparing `tmp/openi-beta-2.0.0.tar.gz` & `tmp/openi-beta-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openi-beta-2.0.0.tar", last modified: Mon Jul 24 07:23:28 2023, max compression
+gzip compressed data, was "openi-beta-2.0.1.tar", last modified: Mon Jul 24 09:19:00 2023, max compression
```

## Comparing `openi-beta-2.0.0.tar` & `openi-beta-2.0.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 07:23:28.340349 openi-beta-2.0.0/
--rw-rw-rw-   0        0        0     5377 2023-07-24 07:23:28.339331 openi-beta-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4731 2023-07-24 07:01:34.000000 openi-beta-2.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-24 07:23:28.340349 openi-beta-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1290 2023-07-24 07:23:14.000000 openi-beta-2.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-24 07:23:28.288322 openi-beta-2.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-24 07:23:28.295768 openi-beta-2.0.0/src/openi/
--rw-rw-rw-   0        0        0      194 2023-07-24 07:15:17.000000 openi-beta-2.0.0/src/openi/__init__.py
--rw-rw-rw-   0        0        0     6459 2023-07-24 07:13:05.000000 openi-beta-2.0.0/src/openi/apis.py
--rw-rw-rw-   0        0        0     5238 2023-07-24 07:13:04.000000 openi-beta-2.0.0/src/openi/cli.py
-drwxrwxrwx   0        0        0        0 2023-07-24 07:23:28.300292 openi-beta-2.0.0/src/openi/cloudbrain/
--rw-rw-rw-   0        0        0       84 2023-07-24 07:06:23.000000 openi-beta-2.0.0/src/openi/cloudbrain/__init__.py
--rw-rw-rw-   0        0        0     1609 2023-07-24 07:06:26.000000 openi-beta-2.0.0/src/openi/cloudbrain/env_check.py
--rw-rw-rw-   0        0        0     5313 2023-07-24 07:06:29.000000 openi-beta-2.0.0/src/openi/cloudbrain/helper.py
--rw-rw-rw-   0        0        0     1559 2023-07-24 07:06:31.000000 openi-beta-2.0.0/src/openi/cloudbrain/minio_operate.py
--rw-rw-rw-   0        0        0     2886 2023-07-24 07:06:32.000000 openi-beta-2.0.0/src/openi/cloudbrain/obs_operate.py
-drwxrwxrwx   0        0        0        0 2023-07-24 07:23:28.303086 openi-beta-2.0.0/src/openi/dataset/
--rw-rw-rw-   0        0        0      109 2023-07-24 07:06:34.000000 openi-beta-2.0.0/src/openi/dataset/__init__.py
--rw-rw-rw-   0        0        0     2855 2023-07-24 07:06:35.000000 openi-beta-2.0.0/src/openi/dataset/dataset_file.py
--rw-rw-rw-   0        0        0     2685 2023-07-24 07:20:32.000000 openi-beta-2.0.0/src/openi/dataset/download.py
--rw-rw-rw-   0        0        0     4592 2023-07-24 07:08:01.000000 openi-beta-2.0.0/src/openi/dataset/upload.py
--rw-rw-rw-   0        0        0     3356 2023-07-24 07:13:03.000000 openi-beta-2.0.0/src/openi/login.py
-drwxrwxrwx   0        0        0        0 2023-07-24 07:23:28.304085 openi-beta-2.0.0/src/openi/path/
--rw-rw-rw-   0        0        0       21 2023-07-24 07:06:52.000000 openi-beta-2.0.0/src/openi/path/__init__.py
--rw-rw-rw-   0        0        0     2405 2023-07-24 07:07:00.000000 openi-beta-2.0.0/src/openi/path/path.py
--rw-rw-rw-   0        0        0     4081 2023-07-24 07:13:02.000000 openi-beta-2.0.0/src/openi/settings.py
-drwxrwxrwx   0        0        0        0 2023-07-24 07:23:28.325091 openi-beta-2.0.0/src/openi/utils/
--rw-rw-rw-   0        0        0       50 2023-07-24 07:07:03.000000 openi-beta-2.0.0/src/openi/utils/__init__.py
--rw-rw-rw-   0        0        0     2197 2023-07-24 07:07:05.000000 openi-beta-2.0.0/src/openi/utils/file_utils.py
--rw-rw-rw-   0        0        0      723 2023-07-24 07:07:16.000000 openi-beta-2.0.0/src/openi/utils/logger.py
-drwxrwxrwx   0        0        0        0 2023-07-24 07:23:28.338332 openi-beta-2.0.0/src/openi_beta.egg-info/
--rw-rw-rw-   0        0        0     5377 2023-07-24 07:23:28.000000 openi-beta-2.0.0/src/openi_beta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      787 2023-07-24 07:23:28.000000 openi-beta-2.0.0/src/openi_beta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 07:23:28.000000 openi-beta-2.0.0/src/openi_beta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-07-24 07:23:28.000000 openi-beta-2.0.0/src/openi_beta.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2023-07-24 07:23:28.000000 openi-beta-2.0.0/src/openi_beta.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-24 07:23:28.000000 openi-beta-2.0.0/src/openi_beta.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-24 07:23:28.339331 openi-beta-2.0.0/test/
--rw-rw-rw-   0        0        0      199 2023-07-24 04:14:29.000000 openi-beta-2.0.0/test/test.py
+drwxrwxrwx   0        0        0        0 2023-07-24 09:19:00.972297 openi-beta-2.0.1/
+-rw-rw-rw-   0        0        0     5381 2023-07-24 09:19:00.972297 openi-beta-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4735 2023-07-24 07:49:31.000000 openi-beta-2.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-24 09:19:00.972297 openi-beta-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1290 2023-07-24 09:18:38.000000 openi-beta-2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 09:19:00.924788 openi-beta-2.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-24 09:19:00.930785 openi-beta-2.0.1/src/openi/
+-rw-rw-rw-   0        0        0      194 2023-07-24 07:15:17.000000 openi-beta-2.0.1/src/openi/__init__.py
+-rw-rw-rw-   0        0        0     6459 2023-07-24 07:13:05.000000 openi-beta-2.0.1/src/openi/apis.py
+-rw-rw-rw-   0        0        0     5238 2023-07-24 07:13:04.000000 openi-beta-2.0.1/src/openi/cli.py
+drwxrwxrwx   0        0        0        0 2023-07-24 09:19:00.934785 openi-beta-2.0.1/src/openi/cloudbrain/
+-rw-rw-rw-   0        0        0       84 2023-07-24 07:06:23.000000 openi-beta-2.0.1/src/openi/cloudbrain/__init__.py
+-rw-rw-rw-   0        0        0     1609 2023-07-24 07:06:26.000000 openi-beta-2.0.1/src/openi/cloudbrain/env_check.py
+-rw-rw-rw-   0        0        0     5313 2023-07-24 07:06:29.000000 openi-beta-2.0.1/src/openi/cloudbrain/helper.py
+-rw-rw-rw-   0        0        0     1559 2023-07-24 07:06:31.000000 openi-beta-2.0.1/src/openi/cloudbrain/minio_operate.py
+-rw-rw-rw-   0        0        0     2886 2023-07-24 07:06:32.000000 openi-beta-2.0.1/src/openi/cloudbrain/obs_operate.py
+drwxrwxrwx   0        0        0        0 2023-07-24 09:19:00.944790 openi-beta-2.0.1/src/openi/dataset/
+-rw-rw-rw-   0        0        0      109 2023-07-24 07:06:34.000000 openi-beta-2.0.1/src/openi/dataset/__init__.py
+-rw-rw-rw-   0        0        0     2855 2023-07-24 07:06:35.000000 openi-beta-2.0.1/src/openi/dataset/dataset_file.py
+-rw-rw-rw-   0        0        0     2685 2023-07-24 07:20:32.000000 openi-beta-2.0.1/src/openi/dataset/download.py
+-rw-rw-rw-   0        0        0     4669 2023-07-24 09:18:26.000000 openi-beta-2.0.1/src/openi/dataset/upload.py
+-rw-rw-rw-   0        0        0     3356 2023-07-24 07:13:03.000000 openi-beta-2.0.1/src/openi/login.py
+drwxrwxrwx   0        0        0        0 2023-07-24 09:19:00.946792 openi-beta-2.0.1/src/openi/path/
+-rw-rw-rw-   0        0        0       21 2023-07-24 07:06:52.000000 openi-beta-2.0.1/src/openi/path/__init__.py
+-rw-rw-rw-   0        0        0     2405 2023-07-24 07:07:00.000000 openi-beta-2.0.1/src/openi/path/path.py
+-rw-rw-rw-   0        0        0     4081 2023-07-24 07:13:02.000000 openi-beta-2.0.1/src/openi/settings.py
+drwxrwxrwx   0        0        0        0 2023-07-24 09:19:00.956305 openi-beta-2.0.1/src/openi/utils/
+-rw-rw-rw-   0        0        0       50 2023-07-24 07:07:03.000000 openi-beta-2.0.1/src/openi/utils/__init__.py
+-rw-rw-rw-   0        0        0     2197 2023-07-24 07:07:05.000000 openi-beta-2.0.1/src/openi/utils/file_utils.py
+-rw-rw-rw-   0        0        0      723 2023-07-24 07:07:16.000000 openi-beta-2.0.1/src/openi/utils/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-24 09:19:00.970297 openi-beta-2.0.1/src/openi_beta.egg-info/
+-rw-rw-rw-   0        0        0     5381 2023-07-24 09:19:00.000000 openi-beta-2.0.1/src/openi_beta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      787 2023-07-24 09:19:00.000000 openi-beta-2.0.1/src/openi_beta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 09:19:00.000000 openi-beta-2.0.1/src/openi_beta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-07-24 09:19:00.000000 openi-beta-2.0.1/src/openi_beta.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-07-24 09:19:00.000000 openi-beta-2.0.1/src/openi_beta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-24 09:19:00.000000 openi-beta-2.0.1/src/openi_beta.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 09:19:00.971297 openi-beta-2.0.1/test/
+-rw-rw-rw-   0        0        0       87 2023-07-24 07:35:25.000000 openi-beta-2.0.1/test/test.py
```

### Comparing `openi-beta-2.0.0/PKG-INFO` & `openi-beta-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-beta
-Version: 2.0.0
+Version: 2.0.1
 Summary: Beta package for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -80,20 +80,22 @@
     login               使用令牌登录启智并保存到本机
     logout              登出当前用户并删除本地令牌文件
     whoami              查询当前登录用户
     dataset (d)         {upload,download} 上传/下载启智AI协作平台的数据集
 ```
 
 #### 数据集上传/下载
+
 ```bash
 > openi dataset upload -f local_dir/my_data.zip -r user1/repo1 -c gpu
 14:35:07 - `my_data.zip`(GPU) calculating md5...
 14:35:07 - Uploading: 100%|███████████████████████████████████| 154M/154M [01:28<00:00, 1.73MB/s]
 14:36:37 - 🎉 Successfully uploaded, view on link: https://openi.pcl.ac.cn/user1/repo1/datasets
 ```
+
 ```bash
 > openi dataset download -f my_data.zip -r user1/repo -c gpu -p local_dir/
 14:51:59 - `my_data.zip`(GPU) preprocessing...
 14:52:00 - Downloading: 100%|█████████████████████████████████| 154M/154M [00:02<00:00, 59.5MB/s]
 14:52:02 - 🎉 Download complete! file was saved to `local_dir/my_data.zip`
 ```
```

### Comparing `openi-beta-2.0.0/README.md` & `openi-beta-2.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -62,20 +62,22 @@
     login               使用令牌登录启智并保存到本机
     logout              登出当前用户并删除本地令牌文件
     whoami              查询当前登录用户
     dataset (d)         {upload,download} 上传/下载启智AI协作平台的数据集
 ```
 
 #### 数据集上传/下载
+
 ```bash
 > openi dataset upload -f local_dir/my_data.zip -r user1/repo1 -c gpu
 14:35:07 - `my_data.zip`(GPU) calculating md5...
 14:35:07 - Uploading: 100%|███████████████████████████████████| 154M/154M [01:28<00:00, 1.73MB/s]
 14:36:37 - 🎉 Successfully uploaded, view on link: https://openi.pcl.ac.cn/user1/repo1/datasets
 ```
+
 ```bash
 > openi dataset download -f my_data.zip -r user1/repo -c gpu -p local_dir/
 14:51:59 - `my_data.zip`(GPU) preprocessing...
 14:52:00 - Downloading: 100%|█████████████████████████████████| 154M/154M [00:02<00:00, 59.5MB/s]
 14:52:02 - 🎉 Download complete! file was saved to `local_dir/my_data.zip`
 ```
```

### Comparing `openi-beta-2.0.0/setup.py` & `openi-beta-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="openi-beta",
-    version="2.0.0",
+    version="2.0.1",
     description="Beta package for openi pypi",
     package_dir={"": "src"},
     packages=find_packages("src"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi",
     author="chenzh05",
```

### Comparing `openi-beta-2.0.0/src/openi/apis.py` & `openi-beta-2.0.1/src/openi/apis.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.0/src/openi/cli.py` & `openi-beta-2.0.1/src/openi/cli.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.0/src/openi/cloudbrain/env_check.py` & `openi-beta-2.0.1/src/openi/cloudbrain/env_check.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.0/src/openi/cloudbrain/helper.py` & `openi-beta-2.0.1/src/openi/cloudbrain/helper.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.0/src/openi/cloudbrain/minio_operate.py` & `openi-beta-2.0.1/src/openi/cloudbrain/minio_operate.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.0/src/openi/cloudbrain/obs_operate.py` & `openi-beta-2.0.1/src/openi/cloudbrain/obs_operate.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.0/src/openi/dataset/dataset_file.py` & `openi-beta-2.0.1/src/openi/dataset/dataset_file.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.0/src/openi/dataset/download.py` & `openi-beta-2.0.1/src/openi/dataset/download.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.0/src/openi/dataset/upload.py` & `openi-beta-2.0.1/src/openi/dataset/upload.py`

 * *Files 6% similar despite different names*

```diff
@@ -97,15 +97,16 @@
     if _get_chunks["uploaded"] == "1":
         # if _get_chunks.attachID == "0": # 删除数据集记录，未删除文件
         #     api.add_attachments(_file) # current not implemented in swagger api
         if _get_chunks["datasetID"] != "" and _get_chunks["datasetName"] != "":
             # ?on web js: and file.realName != ""
             msg = (
                 f"❌ Upload failed: `{_file.filename}` ({cluster})"
-                " already exists, cannot be uploaded again. "
+                " already exists in "
+                f"{api.endpoint.split('/api')[0]}/{_file.owner}/{_get_chunks['repoName']}/datasets"
             )
             logging.error(msg)
             raise ValueError(msg)
 
     # upload continue
     if _get_chunks["uuid"] != "" or _get_chunks["uploadID"] != "":
         _file.uuid, _file.upload_id = _get_chunks["uuid"], _get_chunks["uploadID"]
```

### Comparing `openi-beta-2.0.0/src/openi/login.py` & `openi-beta-2.0.1/src/openi/login.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.0/src/openi/path/path.py` & `openi-beta-2.0.1/src/openi/path/path.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.0/src/openi/settings.py` & `openi-beta-2.0.1/src/openi/settings.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.0/src/openi/utils/file_utils.py` & `openi-beta-2.0.1/src/openi/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.0/src/openi/utils/logger.py` & `openi-beta-2.0.1/src/openi/utils/logger.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.0/src/openi_beta.egg-info/PKG-INFO` & `openi-beta-2.0.1/src/openi_beta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-beta
-Version: 2.0.0
+Version: 2.0.1
 Summary: Beta package for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -80,20 +80,22 @@
     login               使用令牌登录启智并保存到本机
     logout              登出当前用户并删除本地令牌文件
     whoami              查询当前登录用户
     dataset (d)         {upload,download} 上传/下载启智AI协作平台的数据集
 ```
 
 #### 数据集上传/下载
+
 ```bash
 > openi dataset upload -f local_dir/my_data.zip -r user1/repo1 -c gpu
 14:35:07 - `my_data.zip`(GPU) calculating md5...
 14:35:07 - Uploading: 100%|███████████████████████████████████| 154M/154M [01:28<00:00, 1.73MB/s]
 14:36:37 - 🎉 Successfully uploaded, view on link: https://openi.pcl.ac.cn/user1/repo1/datasets
 ```
+
 ```bash
 > openi dataset download -f my_data.zip -r user1/repo -c gpu -p local_dir/
 14:51:59 - `my_data.zip`(GPU) preprocessing...
 14:52:00 - Downloading: 100%|█████████████████████████████████| 154M/154M [00:02<00:00, 59.5MB/s]
 14:52:02 - 🎉 Download complete! file was saved to `local_dir/my_data.zip`
 ```
```

### Comparing `openi-beta-2.0.0/src/openi_beta.egg-info/SOURCES.txt` & `openi-beta-2.0.1/src/openi_beta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

