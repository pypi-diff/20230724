# Comparing `tmp/phap-3.0.0.tar.gz` & `tmp/phap-3.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phap-3.0.0.tar", last modified: Sun Jul 23 04:50:57 2023, max compression
+gzip compressed data, was "phap-3.1.0a1.tar", last modified: Mon Jul 24 11:44:11 2023, max compression
```

## Comparing `phap-3.0.0.tar` & `phap-3.1.0a1.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-23 04:50:57.772704 phap-3.0.0/
--rw-rw-rw-   0        0        0     1069 2023-05-25 04:31:47.000000 phap-3.0.0/LICENSE
--rw-rw-rw-   0        0        0     2495 2023-07-23 04:50:57.770704 phap-3.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1698 2023-07-23 04:49:48.000000 phap-3.0.0/README.md
--rw-rw-rw-   0        0        0       86 2022-03-12 07:02:40.000000 phap-3.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-23 04:50:57.772704 phap-3.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1683 2023-07-23 04:49:19.000000 phap-3.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-23 04:50:57.683406 phap-3.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-23 04:50:57.738000 phap-3.0.0/src/algo/
--rw-rw-rw-   0        0        0      210 2023-07-23 04:14:03.000000 phap-3.0.0/src/algo/__init__.py
--rw-rw-rw-   0        0        0      601 2023-07-23 04:13:41.000000 phap-3.0.0/src/algo/arraylib.py
--rw-rw-rw-   0        0        0     2357 2023-07-23 04:09:49.000000 phap-3.0.0/src/algo/treelib.py
-drwxrwxrwx   0        0        0        0 2023-07-23 04:50:57.740980 phap-3.0.0/src/phap/
--rw-rw-rw-   0        0        0      940 2023-07-23 04:16:00.000000 phap-3.0.0/src/phap/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-23 04:50:57.751110 phap-3.0.0/src/phap.egg-info/
--rw-rw-rw-   0        0        0     2495 2023-07-23 04:50:57.000000 phap-3.0.0/src/phap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      432 2023-07-23 04:50:57.000000 phap-3.0.0/src/phap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-23 04:50:57.000000 phap-3.0.0/src/phap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-07-23 04:50:57.000000 phap-3.0.0/src/phap.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-23 04:50:57.759109 phap-3.0.0/src/stralgo/
--rw-rw-rw-   0        0        0      718 2023-07-23 04:26:02.000000 phap-3.0.0/src/stralgo/__init__.py
--rw-rw-rw-   0        0        0     1021 2023-07-23 04:21:42.000000 phap-3.0.0/src/stralgo/base.py
-drwxrwxrwx   0        0        0        0 2023-07-23 04:50:57.764702 phap-3.0.0/src/stralgo/hash/
--rw-rw-rw-   0        0        0      354 2023-07-23 04:20:12.000000 phap-3.0.0/src/stralgo/hash/__init__.py
--rw-rw-rw-   0        0        0      508 2023-07-23 04:20:41.000000 phap-3.0.0/src/stralgo/hash/sha.py
-drwxrwxrwx   0        0        0        0 2023-07-23 04:50:57.767703 phap-3.0.0/src/stralgo/hash/sm/
--rw-rw-rw-   0        0        0      148 2023-07-23 04:17:13.000000 phap-3.0.0/src/stralgo/hash/sm/__init__.py
--rw-rw-rw-   0        0        0     7024 2023-07-23 04:18:55.000000 phap-3.0.0/src/stralgo/hash/sm/sm3libs.py
--rw-rw-rw-   0        0        0      233 2023-07-23 04:22:18.000000 phap-3.0.0/src/stralgo/json.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:44:11.340023 phap-3.1.0a1/
+-rw-rw-rw-   0        0        0     1069 2023-05-25 04:31:47.000000 phap-3.1.0a1/LICENSE
+-rw-rw-rw-   0        0        0     2504 2023-07-24 11:44:11.332014 phap-3.1.0a1/PKG-INFO
+-rw-rw-rw-   0        0        0     1705 2023-07-24 11:38:22.000000 phap-3.1.0a1/README.md
+-rw-rw-rw-   0        0        0       86 2022-03-12 07:02:40.000000 phap-3.1.0a1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-24 11:44:11.340023 phap-3.1.0a1/setup.cfg
+-rw-rw-rw-   0        0        0     1685 2023-07-24 11:38:28.000000 phap-3.1.0a1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:44:11.212351 phap-3.1.0a1/src/
+drwxrwxrwx   0        0        0        0 2023-07-24 11:44:11.268380 phap-3.1.0a1/src/algo/
+-rw-rw-rw-   0        0        0      210 2023-07-23 04:55:40.000000 phap-3.1.0a1/src/algo/__init__.py
+-rw-rw-rw-   0        0        0      600 2023-07-24 11:42:41.000000 phap-3.1.0a1/src/algo/arraylib.py
+-rw-rw-rw-   0        0        0     2356 2023-07-24 11:41:55.000000 phap-3.1.0a1/src/algo/treelib.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:44:11.276394 phap-3.1.0a1/src/pba/
+-rw-rw-rw-   0        0        0     1013 2023-07-24 11:41:34.000000 phap-3.1.0a1/src/pba/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:44:11.276394 phap-3.1.0a1/src/phap/
+-rw-rw-rw-   0        0        0       72 2023-07-24 11:39:49.000000 phap-3.1.0a1/src/phap/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:44:11.291984 phap-3.1.0a1/src/phap.egg-info/
+-rw-rw-rw-   0        0        0     2504 2023-07-24 11:44:11.000000 phap-3.1.0a1/src/phap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      452 2023-07-24 11:44:11.000000 phap-3.1.0a1/src/phap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 11:44:11.000000 phap-3.1.0a1/src/phap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-07-24 11:44:11.000000 phap-3.1.0a1/src/phap.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 11:44:11.324013 phap-3.1.0a1/src/stralgo/
+-rw-rw-rw-   0        0        0      718 2023-07-23 04:55:41.000000 phap-3.1.0a1/src/stralgo/__init__.py
+-rw-rw-rw-   0        0        0     1021 2023-07-23 04:55:41.000000 phap-3.1.0a1/src/stralgo/base.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:44:11.324013 phap-3.1.0a1/src/stralgo/hash/
+-rw-rw-rw-   0        0        0      354 2023-07-23 04:55:41.000000 phap-3.1.0a1/src/stralgo/hash/__init__.py
+-rw-rw-rw-   0        0        0      508 2023-07-23 04:55:41.000000 phap-3.1.0a1/src/stralgo/hash/sha.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:44:11.332014 phap-3.1.0a1/src/stralgo/hash/sm/
+-rw-rw-rw-   0        0        0      148 2023-07-23 04:55:41.000000 phap-3.1.0a1/src/stralgo/hash/sm/__init__.py
+-rw-rw-rw-   0        0        0     6943 2023-07-24 11:35:14.000000 phap-3.1.0a1/src/stralgo/hash/sm/sm3libs.py
+-rw-rw-rw-   0        0        0      233 2023-07-23 04:55:41.000000 phap-3.1.0a1/src/stralgo/json.py
```

### Comparing `phap-3.0.0/LICENSE` & `phap-3.1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `phap-3.0.0/PKG-INFO` & `phap-3.1.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phap
-Version: 3.0.0
+Version: 3.1.0a1
 Summary: Programing Helpful Algorithm Package
 Home-page: https://github.com/DashBing/phap/
 Author: DashBing
 Author-email: mcbbkf@outlook.com
 Project-URL: Github, https://github.com/DashBing/phap/
 Project-URL: Old Project Version(stralgo), https://pypi.org/project/stralgo/
 Classifier: Development Status :: 5 - Production/Stable
@@ -38,15 +38,15 @@
 + v2.2.1
 
 ## Latest Available Version
 + v3.0.0
 
 ## Latest Version
 ### *(The data under the master branch is inaccurate. Please refer to the dev branch for details)*
-+ v3.0.0
++ v3.1.0-alpha1
 
 # To Use
 ## Read our development document
 ### *(Click the [Github](https://github.com/DashBing/phap/ "Github") link to read this document，or you may can not to open the link)*
 + [Development Document](doc/README.md)
 
 # Build
```

### Comparing `phap-3.0.0/README.md` & `phap-3.1.0a1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 + v2.2.1
 
 ## Latest Available Version
 + v3.0.0
 
 ## Latest Version
 ### *(The data under the master branch is inaccurate. Please refer to the dev branch for details)*
-+ v3.0.0
++ v3.1.0-alpha1
 
 # To Use
 ## Read our development document
 ### *(Click the [Github](https://github.com/DashBing/phap/ "Github") link to read this document，or you may can not to open the link)*
 + [Development Document](doc/README.md)
 
 # Build
```

### Comparing `phap-3.0.0/setup.py` & `phap-3.1.0a1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="phap",
-    version="3.0.0",  #版本
+    version="3.1.0a1",  #版本
     author="DashBing",
     author_email="mcbbkf@outlook.com",
     description="Programing Helpful Algorithm Package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     #scripts=[],
     url="https://github.com/DashBing/phap/",
```

### Comparing `phap-3.0.0/src/algo/arraylib.py` & `phap-3.1.0a1/src/algo/arraylib.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from phap import ErrorTemplate
+from pba import ErrorTemplate
 
 class phap_numalgo_deskcheck_DataNotTrueError(ErrorTemplate):  # 从phap包导入错误类模板，具体可见phap/__init__.py
     message = "The value is not true."
     info_list = ["Try to change a new value."]
 
 def deskcheck(
         array : list = None,
```

### Comparing `phap-3.0.0/src/algo/treelib.py` & `phap-3.1.0a1/src/algo/treelib.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from phap import ErrorTemplate
+from pba import ErrorTemplate
 
 class ValueTypeError(ErrorTemplate):  # 从phap包继承错误类模板，具体可见phap/__init__.py
     message = "The value's type must not be treenode."
     info_list = ['Try to change the type to "str" or "int".']
 
 class treenode:  # 二叉树类
     def __init__(self, val = 0, left = 0, right = 0):  # 参数分别是，初始节点参数，初始节点左边和右边的值
```

### Comparing `phap-3.0.0/src/phap/__init__.py` & `phap-3.1.0a1/src/pba/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import algo
-import stralgo
+# 本包是为了将一些所有包需要用到的共用算法独立出来方便统一集中调用
+
 from random import randint
 
 class ErrorTemplate(Exception):  # 错误模板
     message = ""  # 错误信息
     info_list = []  # 错误提示，若没有则从参数获取
     info_tips = "Detailed information: "
     def __init__(self, info:str = None):
```

### Comparing `phap-3.0.0/src/phap.egg-info/PKG-INFO` & `phap-3.1.0a1/src/phap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phap
-Version: 3.0.0
+Version: 3.1.0a1
 Summary: Programing Helpful Algorithm Package
 Home-page: https://github.com/DashBing/phap/
 Author: DashBing
 Author-email: mcbbkf@outlook.com
 Project-URL: Github, https://github.com/DashBing/phap/
 Project-URL: Old Project Version(stralgo), https://pypi.org/project/stralgo/
 Classifier: Development Status :: 5 - Production/Stable
@@ -38,15 +38,15 @@
 + v2.2.1
 
 ## Latest Available Version
 + v3.0.0
 
 ## Latest Version
 ### *(The data under the master branch is inaccurate. Please refer to the dev branch for details)*
-+ v3.0.0
++ v3.1.0-alpha1
 
 # To Use
 ## Read our development document
 ### *(Click the [Github](https://github.com/DashBing/phap/ "Github") link to read this document，or you may can not to open the link)*
 + [Development Document](doc/README.md)
 
 # Build
```

### Comparing `phap-3.0.0/src/stralgo/__init__.py` & `phap-3.1.0a1/src/stralgo/__init__.py`

 * *Files identical despite different names*

### Comparing `phap-3.0.0/src/stralgo/base.py` & `phap-3.1.0a1/src/stralgo/base.py`

 * *Files identical despite different names*

### Comparing `phap-3.0.0/src/stralgo/hash/sm/sm3libs.py` & `phap-3.1.0a1/src/stralgo/hash/sm/sm3libs.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,11 +266,7 @@
     #print(s)
     return(s)
 
 def sm3(text:str, IV:str='7380166f4914b2b9172442d7da8a0600a96f30bc163138aae38dee4db0fb0e4e') -> str:  # 商密算法的主函数
     s = str_to_int(text)
     s = sm3_int_hex(m=s, IV=IV)
     return(s)
-
-if __name__ == "__main__":
-    while True:
-        print(sm3(text=input()))
```

