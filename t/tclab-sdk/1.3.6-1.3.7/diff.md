# Comparing `tmp/tclab-sdk-1.3.6.tar.gz` & `tmp/tclab-sdk-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tclab-sdk-1.3.6.tar", last modified: Mon Jul 24 14:24:45 2023, max compression
+gzip compressed data, was "tclab-sdk-1.3.7.tar", last modified: Mon Jul 24 14:27:35 2023, max compression
```

## Comparing `tclab-sdk-1.3.6.tar` & `tclab-sdk-1.3.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 14:24:45.699838 tclab-sdk-1.3.6/
--rw-rw-rw-   0        0        0      888 2023-07-24 14:24:45.698838 tclab-sdk-1.3.6/PKG-INFO
--rw-rw-rw-   0        0        0      434 2023-07-07 03:03:35.000000 tclab-sdk-1.3.6/README.md
--rw-rw-rw-   0        0        0       42 2023-07-24 14:24:45.699838 tclab-sdk-1.3.6/setup.cfg
--rw-rw-rw-   0        0        0      946 2023-07-24 14:24:41.000000 tclab-sdk-1.3.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-24 14:24:45.667867 tclab-sdk-1.3.6/tclab/
--rw-rw-rw-   0        0        0    17060 2023-07-24 14:24:31.000000 tclab-sdk-1.3.6/tclab/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 14:24:45.695876 tclab-sdk-1.3.6/tclab_sdk.egg-info/
--rw-rw-rw-   0        0        0      888 2023-07-24 14:24:45.000000 tclab-sdk-1.3.6/tclab_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2023-07-24 14:24:45.000000 tclab-sdk-1.3.6/tclab_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 14:24:45.000000 tclab-sdk-1.3.6/tclab_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-07-24 14:24:45.000000 tclab-sdk-1.3.6/tclab_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-24 14:24:45.000000 tclab-sdk-1.3.6/tclab_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 14:27:35.506420 tclab-sdk-1.3.7/
+-rw-rw-rw-   0        0        0      888 2023-07-24 14:27:35.505416 tclab-sdk-1.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2023-07-07 03:03:35.000000 tclab-sdk-1.3.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-24 14:27:35.507416 tclab-sdk-1.3.7/setup.cfg
+-rw-rw-rw-   0        0        0      946 2023-07-24 14:27:33.000000 tclab-sdk-1.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 14:27:35.473417 tclab-sdk-1.3.7/tclab/
+-rw-rw-rw-   0        0        0    17055 2023-07-24 14:26:54.000000 tclab-sdk-1.3.7/tclab/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 14:27:35.502413 tclab-sdk-1.3.7/tclab_sdk.egg-info/
+-rw-rw-rw-   0        0        0      888 2023-07-24 14:27:35.000000 tclab-sdk-1.3.7/tclab_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2023-07-24 14:27:35.000000 tclab-sdk-1.3.7/tclab_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 14:27:35.000000 tclab-sdk-1.3.7/tclab_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-07-24 14:27:35.000000 tclab-sdk-1.3.7/tclab_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-24 14:27:35.000000 tclab-sdk-1.3.7/tclab_sdk.egg-info/top_level.txt
```

### Comparing `tclab-sdk-1.3.6/PKG-INFO` & `tclab-sdk-1.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tclab-sdk
-Version: 1.3.6
+Version: 1.3.7
 Summary: TC Laboratory Central_Management_System Client Module
 Home-page: UNKNOWN
 Author: Haotian Yang
 Author-email: yht1592754117@126.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tclab-sdk-1.3.6/setup.py` & `tclab-sdk-1.3.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 with open("README.md", "r",encoding='utf-8') as fh:
     long_description = fh.read()
 setuptools.setup(
     name="tclab-sdk",  # 模块名称
-    version="1.3.6",  # 当前版本
+    version="1.3.7",  # 当前版本
     author="Haotian Yang",  # 作者
     author_email="yht1592754117@126.com",  # 作者邮箱
     description="TC Laboratory Central_Management_System Client Module",  # 模块简介
     long_description=long_description,  # 模块详细介绍
     long_description_content_type="text/markdown",  # 模块详细介绍格式
     packages=setuptools.find_packages(),  # 自动找到项目中导入的模块
     # 模块相关的元数据
```

### Comparing `tclab-sdk-1.3.6/tclab/__init__.py` & `tclab-sdk-1.3.7/tclab/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         self.keys._request=self.request
         # 检查是否能连接
         try:
             res = _requests.post(f'{self.lab_server}/',timeout=10).text
         except Exception as e:
             raise Exception('failed to connect')
         if 'TC Laboratory Central Management System' not in res:
-            raise Exception('isn\'t tclab server')
+            raise Exception('server invalid')
 
     def encrypt_data(self,data: str, key: str):
         """加密函数
 
         Args:
             data (str): 待加密的数据
             key (str): 加密密钥
```

### Comparing `tclab-sdk-1.3.6/tclab_sdk.egg-info/PKG-INFO` & `tclab-sdk-1.3.7/tclab_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tclab-sdk
-Version: 1.3.6
+Version: 1.3.7
 Summary: TC Laboratory Central_Management_System Client Module
 Home-page: UNKNOWN
 Author: Haotian Yang
 Author-email: yht1592754117@126.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

