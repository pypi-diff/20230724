# Comparing `tmp/tclab-sdk-1.3.4.tar.gz` & `tmp/tclab-sdk-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tclab-sdk-1.3.4.tar", last modified: Sun Jul  9 02:42:45 2023, max compression
+gzip compressed data, was "tclab-sdk-1.3.5.tar", last modified: Mon Jul 24 14:13:20 2023, max compression
```

## Comparing `tclab-sdk-1.3.4.tar` & `tclab-sdk-1.3.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 02:42:45.906373 tclab-sdk-1.3.4/
--rw-rw-rw-   0        0        0      888 2023-07-09 02:42:45.904361 tclab-sdk-1.3.4/PKG-INFO
--rw-rw-rw-   0        0        0      434 2023-07-07 03:03:35.000000 tclab-sdk-1.3.4/README.md
--rw-rw-rw-   0        0        0       42 2023-07-09 02:42:45.906373 tclab-sdk-1.3.4/setup.cfg
--rw-rw-rw-   0        0        0      946 2023-07-09 02:42:35.000000 tclab-sdk-1.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-09 02:42:45.865360 tclab-sdk-1.3.4/tclab/
--rw-rw-rw-   0        0        0    16809 2023-07-09 02:41:41.000000 tclab-sdk-1.3.4/tclab/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 02:42:45.901358 tclab-sdk-1.3.4/tclab_sdk.egg-info/
--rw-rw-rw-   0        0        0      888 2023-07-09 02:42:45.000000 tclab-sdk-1.3.4/tclab_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2023-07-09 02:42:45.000000 tclab-sdk-1.3.4/tclab_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 02:42:45.000000 tclab-sdk-1.3.4/tclab_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-07-09 02:42:45.000000 tclab-sdk-1.3.4/tclab_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-09 02:42:45.000000 tclab-sdk-1.3.4/tclab_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 14:13:20.512902 tclab-sdk-1.3.5/
+-rw-rw-rw-   0        0        0      888 2023-07-24 14:13:20.511900 tclab-sdk-1.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2023-07-07 03:03:35.000000 tclab-sdk-1.3.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-24 14:13:20.513900 tclab-sdk-1.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      946 2023-07-24 14:12:46.000000 tclab-sdk-1.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 14:13:20.459900 tclab-sdk-1.3.5/tclab/
+-rw-rw-rw-   0        0        0    16954 2023-07-24 14:10:02.000000 tclab-sdk-1.3.5/tclab/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 14:13:20.506898 tclab-sdk-1.3.5/tclab_sdk.egg-info/
+-rw-rw-rw-   0        0        0      888 2023-07-24 14:13:20.000000 tclab-sdk-1.3.5/tclab_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2023-07-24 14:13:20.000000 tclab-sdk-1.3.5/tclab_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 14:13:20.000000 tclab-sdk-1.3.5/tclab_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-07-24 14:13:20.000000 tclab-sdk-1.3.5/tclab_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-24 14:13:20.000000 tclab-sdk-1.3.5/tclab_sdk.egg-info/top_level.txt
```

### Comparing `tclab-sdk-1.3.4/PKG-INFO` & `tclab-sdk-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tclab-sdk
-Version: 1.3.4
+Version: 1.3.5
 Summary: TC Laboratory Central_Management_System Client Module
 Home-page: UNKNOWN
 Author: Haotian Yang
 Author-email: yht1592754117@126.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tclab-sdk-1.3.4/setup.py` & `tclab-sdk-1.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 with open("README.md", "r",encoding='utf-8') as fh:
     long_description = fh.read()
 setuptools.setup(
     name="tclab-sdk",  # 模块名称
-    version="1.3.4",  # 当前版本
+    version="1.3.5",  # 当前版本
     author="Haotian Yang",  # 作者
     author_email="yht1592754117@126.com",  # 作者邮箱
     description="TC Laboratory Central_Management_System Client Module",  # 模块简介
     long_description=long_description,  # 模块详细介绍
     long_description_content_type="text/markdown",  # 模块详细介绍格式
     packages=setuptools.find_packages(),  # 自动找到项目中导入的模块
     # 模块相关的元数据
```

### Comparing `tclab-sdk-1.3.4/tclab/__init__.py` & `tclab-sdk-1.3.5/tclab/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,15 +254,19 @@
                     'function': self.name,
                     'args': args
                 }
                 action_id = self._request('/device/command/submit', data)['id']
                 if '_async' in kwargs and kwargs['_async']:
                     return action_id
                 while True:
-                    res = self._action_status(action_id)
+                    try:
+                        res = self._action_status(action_id)
+                    except:
+                        res={'status':'_'}
+                        _time.sleep(0.1)
                     if res['status'] in ['done', 'ok', 'finished']:
                         return True,res['return']
                     elif res['status'] in ['error']:
                         raise Exception(res['return'])
 
         def _register(self, description: str, functions: dict, default_access: int):
             """注册设备
```

### Comparing `tclab-sdk-1.3.4/tclab_sdk.egg-info/PKG-INFO` & `tclab-sdk-1.3.5/tclab_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tclab-sdk
-Version: 1.3.4
+Version: 1.3.5
 Summary: TC Laboratory Central_Management_System Client Module
 Home-page: UNKNOWN
 Author: Haotian Yang
 Author-email: yht1592754117@126.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

