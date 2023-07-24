# Comparing `tmp/pygbop-0.2.0.5.tar.gz` & `tmp/pygbop-0.2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pygbop-0.2.0.5.tar", last modified: Wed Jul 19 05:56:19 2023, max compression
+gzip compressed data, was "dist\pygbop-0.2.0.6.tar", last modified: Mon Jul 24 05:17:05 2023, max compression
```

## Comparing `pygbop-0.2.0.5.tar` & `pygbop-0.2.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 05:56:19.000000 pygbop-0.2.0.5/
--rw-rw-rw-   0        0        0      207 2023-07-05 07:13:48.000000 pygbop-0.2.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     3245 2023-07-19 05:56:19.000000 pygbop-0.2.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-19 05:56:19.000000 pygbop-0.2.0.5/pygbop/
--rw-rw-rw-   0        0        0      480 2023-07-19 05:43:19.000000 pygbop-0.2.0.5/pygbop/common.py
--rw-rw-rw-   0        0        0     3950 2023-07-19 05:43:41.000000 pygbop-0.2.0.5/pygbop/event_push.py
--rw-rw-rw-   0        0        0     4199 2023-07-05 06:47:47.000000 pygbop-0.2.0.5/pygbop/gbop.py
--rw-rw-rw-   0        0        0      601 2023-07-05 07:08:15.000000 pygbop-0.2.0.5/pygbop/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-19 05:56:19.000000 pygbop-0.2.0.5/pygbop.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-19 05:56:19.000000 pygbop-0.2.0.5/pygbop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     3245 2023-07-19 05:56:19.000000 pygbop-0.2.0.5/pygbop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0        9 2023-07-19 05:56:19.000000 pygbop-0.2.0.5/pygbop.egg-info/requires.txt
--rw-rw-rw-   0        0        0      278 2023-07-19 05:56:19.000000 pygbop-0.2.0.5/pygbop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-07-19 05:56:19.000000 pygbop-0.2.0.5/pygbop.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2287 2023-07-19 05:53:06.000000 pygbop-0.2.0.5/readme.md
--rw-rw-rw-   0        0        0       16 2022-07-08 06:38:50.000000 pygbop-0.2.0.5/requirements.txt
--rw-rw-rw-   0        0        0       64 2023-07-19 05:56:19.000000 pygbop-0.2.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1274 2023-07-19 05:56:15.000000 pygbop-0.2.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 05:17:05.000000 pygbop-0.2.0.6/
+-rw-rw-rw-   0        0        0      207 2023-07-05 07:13:48.000000 pygbop-0.2.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     3320 2023-07-24 05:17:05.000000 pygbop-0.2.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-24 05:17:05.000000 pygbop-0.2.0.6/pygbop/
+-rw-rw-rw-   0        0        0      480 2023-07-19 05:43:19.000000 pygbop-0.2.0.6/pygbop/common.py
+-rw-rw-rw-   0        0        0     4274 2023-07-24 05:11:25.000000 pygbop-0.2.0.6/pygbop/event_push.py
+-rw-rw-rw-   0        0        0     4321 2023-07-24 05:08:43.000000 pygbop-0.2.0.6/pygbop/gbop.py
+-rw-rw-rw-   0        0        0      601 2023-07-05 07:08:15.000000 pygbop-0.2.0.6/pygbop/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 05:17:05.000000 pygbop-0.2.0.6/pygbop.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-24 05:17:05.000000 pygbop-0.2.0.6/pygbop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     3320 2023-07-24 05:17:05.000000 pygbop-0.2.0.6/pygbop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0        9 2023-07-24 05:17:05.000000 pygbop-0.2.0.6/pygbop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      278 2023-07-24 05:17:05.000000 pygbop-0.2.0.6/pygbop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-24 05:17:05.000000 pygbop-0.2.0.6/pygbop.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2362 2023-07-24 05:16:49.000000 pygbop-0.2.0.6/readme.md
+-rw-rw-rw-   0        0        0       16 2022-07-08 06:38:50.000000 pygbop-0.2.0.6/requirements.txt
+-rw-rw-rw-   0        0        0       64 2023-07-24 05:17:05.000000 pygbop-0.2.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1274 2023-07-24 05:12:18.000000 pygbop-0.2.0.6/setup.py
```

### Comparing `pygbop-0.2.0.5/PKG-INFO` & `pygbop-0.2.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygbop
-Version: 0.2.0.5
+Version: 0.2.0.6
 Summary: Geely GBOP Client
 Home-page: https://pypi.python.org/pypi/GbopApiClient
 Author: huang.xiaogang
 Author-email: huang.xiaogang@geely.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -45,15 +45,16 @@
 print('=============POST=============')
 data = {'params3': 'testA', 'params4': 'testB'}
 res = client.execute(Method.POST, '/api/v1/demo', data=data)
 print(res.decode('utf-8'))
 
 print('=============POST2=============')
 params = {'params3': 'testA', 'params4': 'testB'}
-res = client.execute(Method.POST, '/api/v1/demo', params=params, data=data)
+header = {'content-type':'application/json;charset=utf-8'}
+res = client.execute(Method.POST, '/api/v1/demo', params=params, data=data, header=header)
 print(res.decode('utf-8'))
 ```
 
 cloud event push demo:
 
 ```python
 from pygbop import CloudEventBasicAuth, EventPushClient
```

### Comparing `pygbop-0.2.0.5/pygbop/event_push.py` & `pygbop-0.2.0.6/pygbop/event_push.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,54 +50,63 @@
             "token": self.auth.secret_token,
             "content-type": self.auth.CONTENT_TYPE,
             "language": self.auth.LANGUAGE,
             "time": datetime.datetime.now(datetime.timezone.utc).isoformat().replace('+00:00', '+08:00'),
         }
         return headers
 
-    def push_message(self, data: dict, source: str, type_: str, id_: str = '', timeout: int = 30) -> str:
+    def push_message(self, data: dict, source: str, type_: str, id_: str = '', timeout: int = 30,
+                     header: dict = {}) -> str:
         """
         消息推送
         :param timeout: 超时时间
         :param data: 数据体
+        :param header: header
         :param source: 数据来源
         :param type_: 数据类型
         :param id_: 自定义数据编号(不传使用uuid)
         :return: response content
         """
         _data = {
             "id": id_ if id_ else str(uuid.uuid1()),
             "source": source,
             "type": type_,
             "specversion": "1.0",
             "subject": self.auth.subject,
             "data": data
         }
-        response = requests.post(self.base_url, json=_data, headers=self._get_headers(), timeout=timeout).content
+        headers = self._get_headers()
+        if isinstance(header, dict):
+            headers.update(header)
+        response = requests.post(self.base_url, json=_data, headers=headers, timeout=timeout).content
         return response
 
-    def push(self, data: dict, source: str, type_: str, id_: str = '', timeout: int = 30) -> str:
+    def push(self, data: dict, source: str, type_: str, id_: str = '', timeout: int = 30, header: dict = {}) -> str:
         """
         消息推送
         :param timeout: 超时时间
         :param data: 数据体
         :param source: 数据来源
         :param type_: 数据类型
+        :param header: header
         :param id_: 自定义数据编号(不传使用uuid)
         :return: response content
         """
         _data = {
             "id": id_ if id_ else str(uuid.uuid1()),
             "source": source,
             "type": type_,
             "specversion": "1.0",
             "subject": self.auth.subject,
             "data": data
         }
-        response = requests.post(self.base_url, json=_data, headers=self._get_headers(), timeout=timeout).content
+        headers = self._get_headers()
+        if isinstance(header, dict):
+            headers.update(header)
+        response = requests.post(self.base_url, json=_data, headers=headers, timeout=timeout).content
         res_json = json.loads(response.decode('utf-8'))
         code = res_json['retCode']
         msg = res_json['retMsg']
         if code == 0:
             result = True
             data = msg[msg.find('messageId=') + 10:-1]
             msg = ''
```

### Comparing `pygbop-0.2.0.5/pygbop/gbop.py` & `pygbop-0.2.0.6/pygbop/gbop.py`

 * *Files 8% similar despite different names*

```diff
@@ -88,27 +88,30 @@
 
     def _get_url_str(self, path, params):
         query_str = self._get_query_str(params)
         format_string = f"{self.base_url}{path}?{query_str}" if query_str else f"{self.base_url}{path}"
         url = self.protocol + format_string
         return url
 
-    def execute(self, method=Method.GET, path='', params={}, data={}, is_beta_api=False, is_has_status=False,
+    def execute(self, method=Method.GET, path='', params={}, data={}, header={}, is_beta_api=False, is_has_status=False,
                 timeout=30):
         """
         接口调用
         :param method: 调用方法
         :param path: 调用路径
         :param params: GET参数
         :param data: POST参数
+        :param header: header参数
         :param is_beta_api: 是否测试API
         :param is_has_status: 是否返回http code
         :param timeout: 超时时间
         :return:
         """
         url = self._get_url_str(path, params)
         headers = self._get_header(path, method.value, params, is_beta_api)
+        if isinstance(header, dict):
+            headers.update(header)
         res = requests.request(method.value, url, headers=headers, data=data, timeout=timeout)
         if is_has_status:
             return res.status_code, res.content
         else:
             return res.content
```

### Comparing `pygbop-0.2.0.5/pygbop/__init__.py` & `pygbop-0.2.0.6/pygbop/__init__.py`

 * *Files identical despite different names*

### Comparing `pygbop-0.2.0.5/pygbop.egg-info/PKG-INFO` & `pygbop-0.2.0.6/pygbop.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygbop
-Version: 0.2.0.5
+Version: 0.2.0.6
 Summary: Geely GBOP Client
 Home-page: https://pypi.python.org/pypi/GbopApiClient
 Author: huang.xiaogang
 Author-email: huang.xiaogang@geely.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -45,15 +45,16 @@
 print('=============POST=============')
 data = {'params3': 'testA', 'params4': 'testB'}
 res = client.execute(Method.POST, '/api/v1/demo', data=data)
 print(res.decode('utf-8'))
 
 print('=============POST2=============')
 params = {'params3': 'testA', 'params4': 'testB'}
-res = client.execute(Method.POST, '/api/v1/demo', params=params, data=data)
+header = {'content-type':'application/json;charset=utf-8'}
+res = client.execute(Method.POST, '/api/v1/demo', params=params, data=data, header=header)
 print(res.decode('utf-8'))
 ```
 
 cloud event push demo:
 
 ```python
 from pygbop import CloudEventBasicAuth, EventPushClient
```

### Comparing `pygbop-0.2.0.5/readme.md` & `pygbop-0.2.0.6/readme.md`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,16 @@
 print('=============POST=============')
 data = {'params3': 'testA', 'params4': 'testB'}
 res = client.execute(Method.POST, '/api/v1/demo', data=data)
 print(res.decode('utf-8'))
 
 print('=============POST2=============')
 params = {'params3': 'testA', 'params4': 'testB'}
-res = client.execute(Method.POST, '/api/v1/demo', params=params, data=data)
+header = {'content-type':'application/json;charset=utf-8'}
+res = client.execute(Method.POST, '/api/v1/demo', params=params, data=data, header=header)
 print(res.decode('utf-8'))
 ```
 
 cloud event push demo:
 
 ```python
 from pygbop import CloudEventBasicAuth, EventPushClient
```

### Comparing `pygbop-0.2.0.5/setup.py` & `pygbop-0.2.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 from __future__ import print_function
 from setuptools import setup, find_packages
 
 setup(
     name="pygbop",
-    version="0.2.0.5",
+    version="0.2.0.6",
     author="huang.xiaogang",
     author_email="huang.xiaogang@geely.com",
     description="Geely GBOP Client",
     long_description=open("readme.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://pypi.python.org/pypi/GbopApiClient",
```

