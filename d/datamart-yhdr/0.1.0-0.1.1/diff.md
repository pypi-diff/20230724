# Comparing `tmp/datamart_yhdr-0.1.0.tar.gz` & `tmp/datamart_yhdr-0.1.1.tar.gz`

## Comparing `datamart_yhdr-0.1.0.tar` & `datamart_yhdr-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,21 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.0/src/datamart_yhdr/__init__.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.0/src/datamart_yhdr/const.py
--rw-r--r--   0        0        0     4604 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.0/src/datamart_yhdr/interface.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.0/src/datamart_yhdr/settings.py
--rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.0/tests/datamart_yhdr-0.0.1-py3-none-any.whl
--rw-r--r--   0        0        0    12909 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.0/tests/datamart_yhdr-0.0.1.tar.gz
--rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.0/tests/datamart_yhdr-0.0.2-py3-none-any.whl
--rw-r--r--   0        0        0    13273 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.0/tests/datamart_yhdr-0.0.2.tar.gz
--rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.0/tests/datamart_yhdr-0.0.3-py3-none-any.whl
--rw-r--r--   0        0        0    40616 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.0/tests/datamart_yhdr-0.0.3.tar.gz
--rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.0/tests/datamart_yhdr-0.0.4-py3-none-any.whl
--rw-r--r--   0        0        0    79181 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.0/tests/datamart_yhdr-0.0.4.tar.gz
--rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.0/tests/datamart_yhdr-0.0.5-py3-none-any.whl
--rw-r--r--   0        0        0   162244 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.0/tests/datamart_yhdr-0.0.5.tar.gz
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.0/LICENSE
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.0/README.md
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.1/uploadpackage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.1/src/datamart_yhdr/__init__.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.1/src/datamart_yhdr/const.py
+-rw-r--r--   0        0        0     4829 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.1/src/datamart_yhdr/interface.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.1/src/datamart_yhdr/settings.py
+-rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.1/tests/datamart_yhdr-0.0.1-py3-none-any.whl
+-rw-r--r--   0        0        0    12909 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.1/tests/datamart_yhdr-0.0.1.tar.gz
+-rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.1/tests/datamart_yhdr-0.0.2-py3-none-any.whl
+-rw-r--r--   0        0        0    13273 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.1/tests/datamart_yhdr-0.0.2.tar.gz
+-rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.1/tests/datamart_yhdr-0.0.3-py3-none-any.whl
+-rw-r--r--   0        0        0    40616 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.1/tests/datamart_yhdr-0.0.3.tar.gz
+-rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.1/tests/datamart_yhdr-0.0.4-py3-none-any.whl
+-rw-r--r--   0        0        0    79181 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.1/tests/datamart_yhdr-0.0.4.tar.gz
+-rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.1/tests/datamart_yhdr-0.0.5-py3-none-any.whl
+-rw-r--r--   0        0        0   162244 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.1/tests/datamart_yhdr-0.0.5.tar.gz
+-rw-r--r--   0        0        0     4563 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.1/tests/datamart_yhdr-0.1.0-py3-none-any.whl
+-rw-r--r--   0        0        0   328596 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.1/tests/datamart_yhdr-0.1.0.tar.gz
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.1/LICENSE
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.1/README.md
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 datamart_yhdr-0.1.1/PKG-INFO
```

### Comparing `datamart_yhdr-0.1.0/src/datamart_yhdr/interface.py` & `datamart_yhdr-0.1.1/src/datamart_yhdr/interface.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,24 +8,31 @@
         """
         初始化银河德睿数据平台接口对象
         :param username: 用户名
         :param password: 密码
         """
         self.username = username
         self.password = password
+
+        self.token_url = const.HALO_URL
+        self.query_url = const.QUERY_URL
+        self.command_url = const.COMMAND_URL
+        self.batch_url = const.BATCH_URL
+
         if env == "UAT":
             self.token_url = const.HALO_URL_UAT
             self.query_url = const.QUERY_URL_UAT
             self.command_url = const.COMMAND_URL_UAT
             self.batch_url = const.BATCH_URL_UAT
-        else:
-            self.token_url = const.HALO_URL
-            self.query_url = const.QUERY_URL
-            self.command_url = const.COMMAND_URL
-            self.batch_url = const.BATCH_URL
+        elif env == "DEV":
+            self.token_url = const.HALO_URL_DEV
+            self.query_url = const.QUERY_URL_DEV
+            self.command_url = const.COMMAND_URL_DEV
+            self.batch_url = const.BATCH_URL_DEV
+
         self.token = self.get_token()
 
     def get_token(self):
         """
         用于获取数据平台接口授权
         :return: 接口授权
         """
@@ -104,15 +111,15 @@
         sub = requests.post(self.batch_url, headers={'Authorization': self.token}, json=command_params).json()
 
         if "success" in sub:
             if not sub["success"]:
                 raise ConnectionAbortedError(f"请求失败，请检查操作入参。\n备注：{sub.get('remarks')} \n问题数据：{sub.get('failItems')}")
             else:
                 if not silent_mode:
-                    return True
+                    print("请求成功。")
         else:
             raise ConnectionError("请求失败，未知原因。")
         return True
 
 
 if __name__ == '__main__':
-    print("Hello!")
+    print("Hello world.")
```

### Comparing `datamart_yhdr-0.1.0/src/datamart_yhdr/settings.py` & `datamart_yhdr-0.1.1/src/datamart_yhdr/settings.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,7 +5,11 @@
 const.QUERY_URL = "http://192.168.10.111:82/query/query"
 const.COMMAND_URL = "http://192.168.10.111:82/message/message/submit"
 const.BATCH_URL = "http://192.168.10.111:82/message/message/submit/batch"
 const.HALO_URL_UAT = "http://192.168.10.175:82/base/token/create"
 const.QUERY_URL_UAT = "http://192.168.10.175:82/query/query"
 const.COMMAND_URL_UAT = "http://192.168.10.175:82/message/message/submit"
 const.BATCH_URL_UAT = "http://192.168.10.175:82/message/message/submit/batch"
+const.HALO_URL_DEV = "http://192.168.100.73:83/base/token/create"
+const.QUERY_URL_DEV = "http://192.168.100.73:83/query/query"
+const.COMMAND_URL_DEV = "http://192.168.100.73:83/message/message/submit"
+const.BATCH_URL_DEV = "http://192.168.100.73:83/message/message/submit/batch"
```

### Comparing `datamart_yhdr-0.1.0/tests/datamart_yhdr-0.0.1-py3-none-any.whl` & `datamart_yhdr-0.1.1/tests/datamart_yhdr-0.0.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `datamart_yhdr-0.1.0/tests/datamart_yhdr-0.0.1.tar.gz` & `datamart_yhdr-0.1.1/tests/datamart_yhdr-0.0.1.tar.gz`

 * *Files identical despite different names*

### Comparing `datamart_yhdr-0.1.0/tests/datamart_yhdr-0.0.2-py3-none-any.whl` & `datamart_yhdr-0.1.1/tests/datamart_yhdr-0.0.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `datamart_yhdr-0.1.0/tests/datamart_yhdr-0.0.2.tar.gz` & `datamart_yhdr-0.1.1/tests/datamart_yhdr-0.0.2.tar.gz`

 * *Files identical despite different names*

### Comparing `datamart_yhdr-0.1.0/tests/datamart_yhdr-0.0.3-py3-none-any.whl` & `datamart_yhdr-0.1.1/tests/datamart_yhdr-0.0.3-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `datamart_yhdr-0.1.0/tests/datamart_yhdr-0.0.3.tar.gz` & `datamart_yhdr-0.1.1/tests/datamart_yhdr-0.0.3.tar.gz`

 * *Files identical despite different names*

### Comparing `datamart_yhdr-0.1.0/tests/datamart_yhdr-0.0.4-py3-none-any.whl` & `datamart_yhdr-0.1.1/tests/datamart_yhdr-0.0.4-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `datamart_yhdr-0.1.0/tests/datamart_yhdr-0.0.4.tar.gz` & `datamart_yhdr-0.1.1/tests/datamart_yhdr-0.0.4.tar.gz`

 * *Files identical despite different names*

### Comparing `datamart_yhdr-0.1.0/tests/datamart_yhdr-0.0.5-py3-none-any.whl` & `datamart_yhdr-0.1.1/tests/datamart_yhdr-0.0.5-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `datamart_yhdr-0.1.0/tests/datamart_yhdr-0.0.5.tar.gz` & `datamart_yhdr-0.1.1/tests/datamart_yhdr-0.0.5.tar.gz`

 * *Files identical despite different names*

### Comparing `datamart_yhdr-0.1.0/LICENSE` & `datamart_yhdr-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datamart_yhdr-0.1.0/pyproject.toml` & `datamart_yhdr-0.1.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "requests"]
 build-backend = "hatchling.build"
 
 [project]
 name = "datamart_yhdr"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Shihua Huang", email="huangshihua@galaxyderivatives.com" },
 ]
 description = "A data interface package developed for Galaxy Derivatives Data Mart"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `datamart_yhdr-0.1.0/PKG-INFO` & `datamart_yhdr-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamart_yhdr
-Version: 0.1.0
+Version: 0.1.1
 Summary: A data interface package developed for Galaxy Derivatives Data Mart
 Project-URL: Homepage, https://galaxyderivatives.feishu.cn/wiki/wikcn6BhNvlpE8yOCmkjmJHTWHe
 Project-URL: Documentation, https://galaxyderivatives.feishu.cn/wiki/wikcnjOa3s7OQ06v82CzXHBDqUd
 Author-email: Shihua Huang <huangshihua@galaxyderivatives.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

