# Comparing `tmp/wcommon-1.5.6.tar.gz` & `tmp/wcommon-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wcommon-1.5.6.tar", last modified: Fri May 12 07:52:50 2023, max compression
+gzip compressed data, was "wcommon-1.5.8.tar", last modified: Mon Jul 24 08:02:01 2023, max compression
```

## Comparing `wcommon-1.5.6.tar` & `wcommon-1.5.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 wangjunbo   (502) staff       (20)        0 2023-05-12 07:52:50.389356 wcommon-1.5.6/
--rw-r--r--   0 wangjunbo   (502) staff       (20)     1725 2023-05-12 07:52:50.388942 wcommon-1.5.6/PKG-INFO
--rw-r--r--   0 wangjunbo   (502) staff       (20)     1331 2023-02-27 09:51:48.000000 wcommon-1.5.6/README.md
--rw-r--r--   0 wangjunbo   (502) staff       (20)       38 2023-05-12 07:52:50.389530 wcommon-1.5.6/setup.cfg
--rw-r--r--   0 wangjunbo   (502) staff       (20)     1400 2023-05-12 07:51:53.000000 wcommon-1.5.6/setup.py
-drwxr-xr-x   0 wangjunbo   (502) staff       (20)        0 2023-05-12 07:52:50.384383 wcommon-1.5.6/wcommon/
--rw-r--r--   0 wangjunbo   (502) staff       (20)    25863 2023-05-12 07:24:30.000000 wcommon-1.5.6/wcommon/__init__.py
-drwxr-xr-x   0 wangjunbo   (502) staff       (20)        0 2023-05-12 07:52:50.388380 wcommon-1.5.6/wcommon.egg-info/
--rw-r--r--   0 wangjunbo   (502) staff       (20)     1725 2023-05-12 07:52:50.000000 wcommon-1.5.6/wcommon.egg-info/PKG-INFO
--rw-r--r--   0 wangjunbo   (502) staff       (20)      192 2023-05-12 07:52:50.000000 wcommon-1.5.6/wcommon.egg-info/SOURCES.txt
--rw-r--r--   0 wangjunbo   (502) staff       (20)        1 2023-05-12 07:52:50.000000 wcommon-1.5.6/wcommon.egg-info/dependency_links.txt
--rw-r--r--   0 wangjunbo   (502) staff       (20)       37 2023-05-12 07:52:50.000000 wcommon-1.5.6/wcommon.egg-info/requires.txt
--rw-r--r--   0 wangjunbo   (502) staff       (20)        8 2023-05-12 07:52:50.000000 wcommon-1.5.6/wcommon.egg-info/top_level.txt
+drwxr-xr-x   0 wangjunbo   (502) staff       (20)        0 2023-07-24 08:02:01.549283 wcommon-1.5.8/
+-rw-r--r--   0 wangjunbo   (502) staff       (20)     1725 2023-07-24 08:02:01.548952 wcommon-1.5.8/PKG-INFO
+-rw-r--r--   0 wangjunbo   (502) staff       (20)     1331 2023-02-27 09:51:48.000000 wcommon-1.5.8/README.md
+-rw-r--r--   0 wangjunbo   (502) staff       (20)       38 2023-07-24 08:02:01.549411 wcommon-1.5.8/setup.cfg
+-rw-r--r--   0 wangjunbo   (502) staff       (20)     1400 2023-07-24 08:01:55.000000 wcommon-1.5.8/setup.py
+drwxr-xr-x   0 wangjunbo   (502) staff       (20)        0 2023-07-24 08:02:01.544700 wcommon-1.5.8/wcommon/
+-rw-r--r--   0 wangjunbo   (502) staff       (20)    27329 2023-07-24 07:29:23.000000 wcommon-1.5.8/wcommon/__init__.py
+drwxr-xr-x   0 wangjunbo   (502) staff       (20)        0 2023-07-24 08:02:01.548436 wcommon-1.5.8/wcommon.egg-info/
+-rw-r--r--   0 wangjunbo   (502) staff       (20)     1725 2023-07-24 08:02:01.000000 wcommon-1.5.8/wcommon.egg-info/PKG-INFO
+-rw-r--r--   0 wangjunbo   (502) staff       (20)      192 2023-07-24 08:02:01.000000 wcommon-1.5.8/wcommon.egg-info/SOURCES.txt
+-rw-r--r--   0 wangjunbo   (502) staff       (20)        1 2023-07-24 08:02:01.000000 wcommon-1.5.8/wcommon.egg-info/dependency_links.txt
+-rw-r--r--   0 wangjunbo   (502) staff       (20)       37 2023-07-24 08:02:01.000000 wcommon-1.5.8/wcommon.egg-info/requires.txt
+-rw-r--r--   0 wangjunbo   (502) staff       (20)        8 2023-07-24 08:02:01.000000 wcommon-1.5.8/wcommon.egg-info/top_level.txt
```

### Comparing `wcommon-1.5.6/PKG-INFO` & `wcommon-1.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcommon
-Version: 1.5.6
+Version: 1.5.8
 Summary: 常用工具类方法集合
 Home-page: http://www.hohode.com
 Author: WangJunbo
 Author-email: wjbhnu@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wcommon-1.5.6/README.md` & `wcommon-1.5.8/README.md`

 * *Files identical despite different names*

### Comparing `wcommon-1.5.6/setup.py` & `wcommon-1.5.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     # 项目的名称 一般在同级目录中有个同名的文件夹
     name="wcommon",
     # 项目的版本
-    version="1.5.6",
+    version="1.5.8",
     # 项目的作者
     author="WangJunbo",
     # 作者的邮箱
     author_email="wjbhnu@gmail.com",
     # 项目描述
     description="常用工具类方法集合",
     # 项目的长描述
```

### Comparing `wcommon-1.5.6/wcommon/__init__.py` & `wcommon-1.5.8/wcommon/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 import pymysql
 import re
 import configparser
 from loguru import logger
 import hashlib
 import platform
 import warnings
+import random
+import string
 
 # from Crypto.Cipher import AES
 # from binascii import b2a_hex
 
 # reload(sys)
 # sys.setdefaultencoding('utf8')
 # logger.info("WARN:please configuration the configuraion_file variable")
@@ -383,14 +385,27 @@
         s.close()
     except Exception as e:
         logger.debug(e)
         traceback.print_exc()
     return ip
 
 
+def generate_random_str(length):
+    chars = string.ascii_letters + string.digits
+    return ''.join(random.choice(chars) for _ in range(length))
+
+
+def generate_digit_str(length):
+    return ''.join(random.choice(string.digits) for _ in range(length))
+
+
+def generate_lower_str(length):
+    return ''.join(random.choice(string.ascii_lowercase) for _ in range(length))
+
+
 def get_external_ip():
     # 这里的-s参数目的是在进行网络请求的时候禁止在控制台输出进度
     proc = subprocess.Popen(["curl -s https://api.hohode.com/ip"], stdout=subprocess.PIPE, shell=True)
     (outer_ip, err) = proc.communicate()
     if isinstance(outer_ip, bytes):
         outer_ip = outer_ip.decode("utf8")
     return outer_ip
@@ -609,14 +624,33 @@
                         row[field] = tmp_value
                 rows.append(row)
         else:
             for row in cursor:
                 rows.append(row)
         return rows
 
+
+    @pingmysql
+    def get(self, sql, argumentTuple=(), timestamp2str=True):
+        """
+        获取单条数据，要么返回一条数据，要么返回None
+        :param sql:
+        :param argumentTuple:
+        :param timestamp2str:
+        :return:
+        """
+        if sql and sql.lower().find("limit") == -1:
+            sql = "{} limit 1".format(sql)
+
+        rows = self.query(sql,argumentTuple,timestamp2str)
+        if rows and len(rows) > 0:
+            return rows[0]
+        else:
+            return None
+
     @pingmysql
     def insert(self, tableName, dic, commit=True):
         cursor = self.database.cursor()
         cols = []
         vals = []
         placeholders = []
         id = ""
@@ -751,24 +785,39 @@
         self.password = password
         self.urlPrefix = "http://{}:{}".format(host, port)
 
     headers = {
         'content-type': 'application/json'
     }
 
-    def _transfer_data(self, data=None):
+    def _transfer_data(self, data=None,size=None,sort_field=None,sort_type=None):
+        query_dict = {}
         if data is not None:
             if type(data) == str:
-                return data
+                # return data
+                query_dict = json.loads(data)
             elif type(data) == dict:
-                return json.dumps(data)
-        return None
+                query_dict = data
+
+        if size is not None:
+            query_dict["size"] = size
+        if sort_field is not None:
+            if sort_type is None:
+                sort_type = "asc"
+            query_dict["sort"] = [
+                {
+                  sort_field: {
+                    "order": sort_type
+                  }
+                }
+              ]
+        return json.dumps(query_dict)
 
-    def search(self, action, data=None):
-        data1 = self._transfer_data(data)
+    def search(self, action, data=None,size=None,sort_field=None,sort_type=None):
+        data1 = self._transfer_data(data,size,sort_field,sort_type)
         return requests.get(url="{}{}".format(self.urlPrefix, action), auth=(self.username, self.password),
                             headers=self.headers, data=data1).json()
 
     def delete_by_query(self, index, data):
         """
         :param action: /sym/_delete_by_query
         :return:
```

### Comparing `wcommon-1.5.6/wcommon.egg-info/PKG-INFO` & `wcommon-1.5.8/wcommon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcommon
-Version: 1.5.6
+Version: 1.5.8
 Summary: 常用工具类方法集合
 Home-page: http://www.hohode.com
 Author: WangJunbo
 Author-email: wjbhnu@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

