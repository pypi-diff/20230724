# Comparing `tmp/alibabacloud_tea_util_py2-0.0.8.tar.gz` & `tmp/alibabacloud_tea_util_py2-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_tea_util_py2-0.0.8.tar", last modified: Mon Jun 26 10:16:14 2023, max compression
+gzip compressed data, was "dist/alibabacloud_tea_util_py2-0.0.9.tar", last modified: Mon Jul 24 02:51:10 2023, max compression
```

## Comparing `alibabacloud_tea_util_py2-0.0.8.tar` & `alibabacloud_tea_util_py2-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 10:16:14.000000 alibabacloud_tea_util_py2-0.0.8/
--rw-r--r--   0 root         (0) root         (0)     1826 2023-06-26 10:16:14.000000 alibabacloud_tea_util_py2-0.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      943 2023-06-26 10:16:14.000000 alibabacloud_tea_util_py2-0.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 10:16:14.000000 alibabacloud_tea_util_py2-0.0.8/alibabacloud_tea_util/
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-26 10:16:14.000000 alibabacloud_tea_util_py2-0.0.8/alibabacloud_tea_util/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10629 2023-06-26 10:16:14.000000 alibabacloud_tea_util_py2-0.0.8/alibabacloud_tea_util/client.py
--rw-r--r--   0 root         (0) root         (0)     5526 2023-06-26 10:16:14.000000 alibabacloud_tea_util_py2-0.0.8/alibabacloud_tea_util/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 10:16:14.000000 alibabacloud_tea_util_py2-0.0.8/alibabacloud_tea_util_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1826 2023-06-26 10:16:14.000000 alibabacloud_tea_util_py2-0.0.8/alibabacloud_tea_util_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      360 2023-06-26 10:16:14.000000 alibabacloud_tea_util_py2-0.0.8/alibabacloud_tea_util_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 10:16:14.000000 alibabacloud_tea_util_py2-0.0.8/alibabacloud_tea_util_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-26 10:16:14.000000 alibabacloud_tea_util_py2-0.0.8/alibabacloud_tea_util_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-26 10:16:14.000000 alibabacloud_tea_util_py2-0.0.8/alibabacloud_tea_util_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 10:16:14.000000 alibabacloud_tea_util_py2-0.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2197 2023-06-26 10:16:14.000000 alibabacloud_tea_util_py2-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 02:51:10.000000 alibabacloud_tea_util_py2-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)     1826 2023-07-24 02:51:10.000000 alibabacloud_tea_util_py2-0.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      943 2023-07-24 02:51:10.000000 alibabacloud_tea_util_py2-0.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 02:51:10.000000 alibabacloud_tea_util_py2-0.0.9/alibabacloud_tea_util/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-24 02:51:10.000000 alibabacloud_tea_util_py2-0.0.9/alibabacloud_tea_util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10981 2023-07-24 02:51:10.000000 alibabacloud_tea_util_py2-0.0.9/alibabacloud_tea_util/client.py
+-rw-r--r--   0 root         (0) root         (0)     5526 2023-07-24 02:51:10.000000 alibabacloud_tea_util_py2-0.0.9/alibabacloud_tea_util/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 02:51:10.000000 alibabacloud_tea_util_py2-0.0.9/alibabacloud_tea_util_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1826 2023-07-24 02:51:10.000000 alibabacloud_tea_util_py2-0.0.9/alibabacloud_tea_util_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      360 2023-07-24 02:51:10.000000 alibabacloud_tea_util_py2-0.0.9/alibabacloud_tea_util_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 02:51:10.000000 alibabacloud_tea_util_py2-0.0.9/alibabacloud_tea_util_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-24 02:51:10.000000 alibabacloud_tea_util_py2-0.0.9/alibabacloud_tea_util_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-24 02:51:10.000000 alibabacloud_tea_util_py2-0.0.9/alibabacloud_tea_util_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 02:51:10.000000 alibabacloud_tea_util_py2-0.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2197 2023-07-24 02:51:10.000000 alibabacloud_tea_util_py2-0.0.9/setup.py
```

### Comparing `alibabacloud_tea_util_py2-0.0.8/PKG-INFO` & `alibabacloud_tea_util_py2-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: alibabacloud_tea_util_py2
-Version: 0.0.8
+Version: 0.0.9
 Summary: The tea-util module of alibabaCloud Python2 SDK.
 Home-page: https://github.com/aliyun/tea-util/tree/master/python2
 Author: Alibaba Cloud
 Author-email: alibaba-cloud-sdk-dev-team@list.alibaba-inc.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_tea_util_py2-0.0.8/README.md` & `alibabacloud_tea_util_py2-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_tea_util_py2-0.0.8/alibabacloud_tea_util/client.py` & `alibabacloud_tea_util_py2-0.0.9/alibabacloud_tea_util/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 # -*- coding: utf-8 -*-
 import Tea
 import json
-import uuid
 import platform
-import socket
 import time
+import threading
+import random
+import hashlib
 
 from io import BytesIO
 from datetime import datetime
 try:
     from urllib import urlencode
 except ImportError:
     from urllib.parse import urlencode
 
 from Tea.converter import TeaConverter
 from Tea.model import TeaModel
 from Tea.stream import READABLE
 
+_process_start_time = int(time.time() * 1000)
+_seqId = 0
 
 class Client(object):
     """
     This is a utility module
     """
     class _ModelEncoder(json.JSONEncoder):
         def default(self, o):
@@ -108,17 +111,25 @@
 
     @staticmethod
     def get_nonce():
         """
         Generate a nonce string
         @return: the nonce string
         """
-        name = socket.gethostname() + str(uuid.uuid1())
-        namespace = uuid.NAMESPACE_URL
-        return str(uuid.uuid5(namespace, name))
+        global _seqId
+        thread_id = threading.current_thread().ident
+        current_time = int(time.time() * 1000)
+        seq = _seqId
+        _seqId += 1
+        randNum = random.getrandbits(64)
+        msg = '%d-%d-%d-%d-%d' % (_process_start_time, thread_id, current_time, seq, randNum)
+        # print(msg)
+        md5 = hashlib.md5()
+        md5.update(msg.encode('utf-8'))
+        return md5.hexdigest()
 
     @staticmethod
     def get_date_utcstring():
         """
         Get an UTC format string by current date, e.g. 'Thu, 06 Feb 2020 07:32:54 GMT'
         @return: the UTC format string
         """
```

### Comparing `alibabacloud_tea_util_py2-0.0.8/alibabacloud_tea_util/models.py` & `alibabacloud_tea_util_py2-0.0.9/alibabacloud_tea_util/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_tea_util_py2-0.0.8/alibabacloud_tea_util_py2.egg-info/PKG-INFO` & `alibabacloud_tea_util_py2-0.0.9/alibabacloud_tea_util_py2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: alibabacloud-tea-util-py2
-Version: 0.0.8
+Version: 0.0.9
 Summary: The tea-util module of alibabaCloud Python2 SDK.
 Home-page: https://github.com/aliyun/tea-util/tree/master/python2
 Author: Alibaba Cloud
 Author-email: alibaba-cloud-sdk-dev-team@list.alibaba-inc.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_tea_util_py2-0.0.8/setup.py` & `alibabacloud_tea_util_py2-0.0.9/setup.py`

 * *Files identical despite different names*

