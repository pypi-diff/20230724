# Comparing `tmp/myds-0.1.1.tar.gz` & `tmp/myds-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myds-0.1.1.tar", last modified: Sun Jul 23 08:22:30 2023, max compression
+gzip compressed data, was "myds-0.1.2.tar", last modified: Mon Jul 24 09:13:00 2023, max compression
```

## Comparing `myds-0.1.1.tar` & `myds-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-23 08:22:30.133167 myds-0.1.1/
--rw-rw-rw-   0        0        0     1082 2022-07-09 03:01:52.000000 myds-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      278 2023-07-23 08:22:30.132168 myds-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-23 08:22:30.105689 myds-0.1.1/myds/
--rw-rw-rw-   0        0        0       44 2023-07-23 08:18:54.000000 myds-0.1.1/myds/__init__.py
--rw-rw-rw-   0        0        0     1717 2023-07-23 07:56:36.000000 myds-0.1.1/myds/database.py
--rw-rw-rw-   0        0        0      222 2023-07-23 08:00:50.000000 myds-0.1.1/myds/test.py
-drwxrwxrwx   0        0        0        0 2023-07-23 08:22:30.131169 myds-0.1.1/myds.egg-info/
--rw-rw-rw-   0        0        0      278 2023-07-23 08:22:30.000000 myds-0.1.1/myds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-07-23 08:22:30.000000 myds-0.1.1/myds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-23 08:22:30.000000 myds-0.1.1/myds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-23 08:22:30.000000 myds-0.1.1/myds.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-23 08:22:30.000000 myds-0.1.1/myds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-23 08:22:30.133167 myds-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      739 2023-07-23 08:22:11.000000 myds-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 09:13:00.996857 myds-0.1.2/
+-rw-rw-rw-   0        0        0     1082 2022-07-09 03:01:52.000000 myds-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      278 2023-07-24 09:13:00.996857 myds-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-24 09:13:00.989020 myds-0.1.2/myds/
+-rw-rw-rw-   0        0        0       44 2023-07-23 08:18:54.000000 myds-0.1.2/myds/__init__.py
+-rw-rw-rw-   0        0        0     1723 2023-07-24 08:51:57.000000 myds-0.1.2/myds/database.py
+-rw-rw-rw-   0        0        0      223 2023-07-24 09:12:02.000000 myds-0.1.2/myds/test.py
+drwxrwxrwx   0        0        0        0 2023-07-24 09:13:00.994886 myds-0.1.2/myds.egg-info/
+-rw-rw-rw-   0        0        0      278 2023-07-24 09:13:00.000000 myds-0.1.2/myds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-07-24 09:13:00.000000 myds-0.1.2/myds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 09:13:00.000000 myds-0.1.2/myds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-24 09:13:00.000000 myds-0.1.2/myds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-24 09:13:00.000000 myds-0.1.2/myds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 09:13:00.996857 myds-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      739 2023-07-24 09:12:53.000000 myds-0.1.2/setup.py
```

### Comparing `myds-0.1.1/LICENSE` & `myds-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `myds-0.1.1/myds/database.py` & `myds-0.1.2/myds/database.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,16 +24,16 @@
             raise InvalidSchema(f"Requires 'myds' protocol for {mydsUrl!r}")
         prot="http"
         if self.isSSL:
             prot+="s"
         port = parsed_url.port
         if port is None:
             port=5149
-        netloc = parsed_url.netloc  # 获取域名和端口
-        params = {"dbName": netloc};
+        hostname = parsed_url.hostname  # 获取域名和端口
+        params = {"dbName": hostname};
         urlStr = f'{prot}://{self.host}:{port}/query?'+urlencode(params)
         args = parsed_url.query  # 获取查询字符串
         if args!="":
             urlStr+="&"+args
         return urlStr
 
     def query(self, mydsUrl):
```

### Comparing `myds-0.1.1/setup.py` & `myds-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #############################################
 
 
 from setuptools import setup, find_packages
 
 setup(
     name = "myds",
-    version = "0.1.1",
+    version = "0.1.2",
     keywords = ("database","localServer"),
     description = "A database name Getter",
     long_description = "A database name Getter",
     license = "MIT Licence",
     author = "Cai Jianping",
     author_email = "jpingcai@163.com",
```

