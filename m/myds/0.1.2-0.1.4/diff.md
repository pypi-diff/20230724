# Comparing `tmp/myds-0.1.2.tar.gz` & `tmp/myds-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myds-0.1.2.tar", last modified: Mon Jul 24 09:13:00 2023, max compression
+gzip compressed data, was "myds-0.1.4.tar", last modified: Mon Jul 24 11:50:41 2023, max compression
```

## Comparing `myds-0.1.2.tar` & `myds-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 09:13:00.996857 myds-0.1.2/
--rw-rw-rw-   0        0        0     1082 2022-07-09 03:01:52.000000 myds-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      278 2023-07-24 09:13:00.996857 myds-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-24 09:13:00.989020 myds-0.1.2/myds/
--rw-rw-rw-   0        0        0       44 2023-07-23 08:18:54.000000 myds-0.1.2/myds/__init__.py
--rw-rw-rw-   0        0        0     1723 2023-07-24 08:51:57.000000 myds-0.1.2/myds/database.py
--rw-rw-rw-   0        0        0      223 2023-07-24 09:12:02.000000 myds-0.1.2/myds/test.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:13:00.994886 myds-0.1.2/myds.egg-info/
--rw-rw-rw-   0        0        0      278 2023-07-24 09:13:00.000000 myds-0.1.2/myds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-07-24 09:13:00.000000 myds-0.1.2/myds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 09:13:00.000000 myds-0.1.2/myds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-24 09:13:00.000000 myds-0.1.2/myds.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-24 09:13:00.000000 myds-0.1.2/myds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 09:13:00.996857 myds-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      739 2023-07-24 09:12:53.000000 myds-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:50:41.526068 myds-0.1.4/
+-rw-rw-rw-   0        0        0     1082 2022-07-09 03:01:52.000000 myds-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      278 2023-07-24 11:50:41.526068 myds-0.1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-24 11:50:41.517090 myds-0.1.4/myds/
+-rw-rw-rw-   0        0        0       52 2023-07-24 11:48:48.000000 myds-0.1.4/myds/__init__.py
+-rw-rw-rw-   0        0        0     1625 2023-07-24 11:48:35.000000 myds-0.1.4/myds/database.py
+-rw-rw-rw-   0        0        0      194 2023-07-24 11:49:48.000000 myds-0.1.4/myds/test.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:50:41.524073 myds-0.1.4/myds.egg-info/
+-rw-rw-rw-   0        0        0      278 2023-07-24 11:50:41.000000 myds-0.1.4/myds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-07-24 11:50:41.000000 myds-0.1.4/myds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 11:50:41.000000 myds-0.1.4/myds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-24 11:50:41.000000 myds-0.1.4/myds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-24 11:50:41.000000 myds-0.1.4/myds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 11:50:41.526068 myds-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      739 2023-07-24 11:50:09.000000 myds-0.1.4/setup.py
```

### Comparing `myds-0.1.2/LICENSE` & `myds-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `myds-0.1.2/myds/database.py` & `myds-0.1.4/myds/database.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,52 +2,49 @@
 from requests.exceptions import (
     InvalidSchema,
 )
 import requests
 from urllib.parse import urlparse
 from urllib.parse import urlencode
 
-def getDb(dbName,port=5149,charset='UTF-8'):
-    params = {"dbName": dbName, "charset": charset};
-    url = f'http://localhost:{port}/query?'+urlencode(params)
-    res = requests.get(url).text
-    return res
-
 class HttpQuerier:
-    def __init__(self, host="localhost",isSSL=False):
-        self.host=host
-        self.isSSL=isSSL
+    def __init__(self, host="localhost", isSSL=False):
+        self.host = host
+        self.isSSL = isSSL
 
     def getQueryUrl(self, mydsUrl):
         parsed_url = urlparse(mydsUrl)
         scheme = parsed_url.scheme  # 获取协议
-        if scheme!="myds":
+        if scheme != "myds":
             raise InvalidSchema(f"Requires 'myds' protocol for {mydsUrl!r}")
-        prot="http"
+        prot = "http"
         if self.isSSL:
-            prot+="s"
+            prot += "s"
         port = parsed_url.port
         if port is None:
-            port=5149
+            port = 5149
         hostname = parsed_url.hostname  # 获取域名和端口
         params = {"dbName": hostname};
-        urlStr = f'{prot}://{self.host}:{port}/query?'+urlencode(params)
+        urlStr = f'{prot}://{self.host}:{port}/query?' + urlencode(params)
         args = parsed_url.query  # 获取查询字符串
-        if args!="":
-            urlStr+="&"+args
+        if args != "":
+            urlStr += "&" + args
         return urlStr
 
     def query(self, mydsUrl):
-        urlStr=self.getQueryUrl(mydsUrl);
+        urlStr = self.getQueryUrl(mydsUrl);
         res = requests.get(urlStr).text
         if res.startswith("[error]"):
             raise ConnectionError(res)
         parsed_url = urlparse(mydsUrl)
         path = parsed_url.path
-        if path!="":
+        if path != "":
             if res.startswith("/"):
-                res=res[0:-1]
-            while len(path)>=3 and path[0:3]=="/..":
-                res=os.path.dirname(res)
-                path=path[3:]
-            res+=path
-        return res
+                res = res[0:-1]
+            while len(path) >= 3 and path[0:3] == "/..":
+                res = os.path.dirname(res)
+                path = path[3:]
+            res += path
+        return res
+
+def simpleQuery(dsName):
+    return HttpQuerier().query(f'myds://{dsName}')
```

### Comparing `myds-0.1.2/setup.py` & `myds-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #############################################
 
 
 from setuptools import setup, find_packages
 
 setup(
     name = "myds",
-    version = "0.1.2",
+    version = "0.1.4",
     keywords = ("database","localServer"),
     description = "A database name Getter",
     long_description = "A database name Getter",
     license = "MIT Licence",
     author = "Cai Jianping",
     author_email = "jpingcai@163.com",
```

