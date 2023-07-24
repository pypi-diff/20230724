# Comparing `tmp/sonic-uia2-client-0.0.5.tar.gz` & `tmp/sonic-uia2-client-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sonic-uia2-client-0.0.5.tar", last modified: Fri Jun  9 12:23:06 2023, max compression
+gzip compressed data, was "sonic-uia2-client-0.0.6.tar", last modified: Mon Jul 24 03:02:12 2023, max compression
```

## Comparing `sonic-uia2-client-0.0.5.tar` & `sonic-uia2-client-0.0.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:23:06.588880 sonic-uia2-client-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-09 12:22:54.000000 sonic-uia2-client-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-06-09 12:23:06.588880 sonic-uia2-client-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-09 12:22:54.000000 sonic-uia2-client-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:23:06.588880 sonic-uia2-client-0.0.5/client/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-09 12:22:54.000000 sonic-uia2-client-0.0.5/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-06-09 12:22:54.000000 sonic-uia2-client-0.0.5/client/android_element.py
--rw-r--r--   0 runner    (1001) docker     (123)    10580 2023-06-09 12:22:54.000000 sonic-uia2-client-0.0.5/client/uia_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:23:06.588880 sonic-uia2-client-0.0.5/common/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-09 12:22:54.000000 sonic-uia2-client-0.0.5/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-09 12:22:54.000000 sonic-uia2-client-0.0.5/common/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-09 12:22:54.000000 sonic-uia2-client-0.0.5/common/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-09 12:22:54.000000 sonic-uia2-client-0.0.5/common/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-09 12:22:54.000000 sonic-uia2-client-0.0.5/common/resp_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-09 12:22:54.000000 sonic-uia2-client-0.0.5/common/sonic_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 12:23:06.588880 sonic-uia2-client-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-09 12:22:54.000000 sonic-uia2-client-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:23:06.588880 sonic-uia2-client-0.0.5/sonic_uia2_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-06-09 12:23:06.000000 sonic-uia2-client-0.0.5/sonic_uia2_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-09 12:23:06.000000 sonic-uia2-client-0.0.5/sonic_uia2_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 12:23:06.000000 sonic-uia2-client-0.0.5/sonic_uia2_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-09 12:23:06.000000 sonic-uia2-client-0.0.5/sonic_uia2_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:23:06.588880 sonic-uia2-client-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-09 12:22:54.000000 sonic-uia2-client-0.0.5/tests/test_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:23:06.588880 sonic-uia2-client-0.0.5/uia2/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-09 12:22:54.000000 sonic-uia2-client-0.0.5/uia2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-09 12:22:54.000000 sonic-uia2-client-0.0.5/uia2/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:02:12.030600 sonic-uia2-client-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-24 03:01:56.000000 sonic-uia2-client-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-07-24 03:02:12.030600 sonic-uia2-client-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-24 03:01:56.000000 sonic-uia2-client-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:02:12.026600 sonic-uia2-client-0.0.6/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-24 03:01:56.000000 sonic-uia2-client-0.0.6/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-07-24 03:01:56.000000 sonic-uia2-client-0.0.6/client/android_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-07-24 03:01:56.000000 sonic-uia2-client-0.0.6/client/uia_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:02:12.026600 sonic-uia2-client-0.0.6/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-24 03:01:56.000000 sonic-uia2-client-0.0.6/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-24 03:01:56.000000 sonic-uia2-client-0.0.6/common/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-24 03:01:56.000000 sonic-uia2-client-0.0.6/common/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-24 03:01:56.000000 sonic-uia2-client-0.0.6/common/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-24 03:01:56.000000 sonic-uia2-client-0.0.6/common/resp_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-24 03:01:56.000000 sonic-uia2-client-0.0.6/common/sonic_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 03:02:12.030600 sonic-uia2-client-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-24 03:01:56.000000 sonic-uia2-client-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:02:12.026600 sonic-uia2-client-0.0.6/sonic_uia2_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-07-24 03:02:12.000000 sonic-uia2-client-0.0.6/sonic_uia2_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-24 03:02:12.000000 sonic-uia2-client-0.0.6/sonic_uia2_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 03:02:12.000000 sonic-uia2-client-0.0.6/sonic_uia2_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-24 03:02:12.000000 sonic-uia2-client-0.0.6/sonic_uia2_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:02:12.026600 sonic-uia2-client-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-24 03:01:56.000000 sonic-uia2-client-0.0.6/tests/test_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:02:12.030600 sonic-uia2-client-0.0.6/uia2/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-24 03:01:56.000000 sonic-uia2-client-0.0.6/uia2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-24 03:01:56.000000 sonic-uia2-client-0.0.6/uia2/driver.py
```

### Comparing `sonic-uia2-client-0.0.5/LICENSE` & `sonic-uia2-client-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sonic-uia2-client-0.0.5/PKG-INFO` & `sonic-uia2-client-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sonic-uia2-client
-Version: 0.0.5
+Version: 0.0.6
 Home-page: https://github.com/SonicCloudOrg/sonic-uiautomator2-python-client
 Author: SonicCloudOrg
 Author-email: soniccloudorg@163.com
 License: MIT
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `sonic-uia2-client-0.0.5/README.md` & `sonic-uia2-client-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `sonic-uia2-client-0.0.5/client/android_element.py` & `sonic-uia2-client-0.0.6/client/android_element.py`

 * *Files identical despite different names*

### Comparing `sonic-uia2-client-0.0.5/client/uia_client.py` & `sonic-uia2-client-0.0.6/client/uia_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,16 +233,15 @@
             data = {"strategy": selector, "selector": value}
             b = self.resp_handler.get_resp(
                 HttpUtil.create_post(
                     self._remote_url + "/session/" + self.session_id + "/elements"
                 ).body(json.dumps(data))
             )
             if b.err is None:
-                self.logger.info("find elements successful.")
-                ids = json.loads(b.value)
+                ids = b.value
                 for ele in ids:
                     id = self.parse_element_id(ele)
                     if len(id) > 0:
                         android_element_list.append(AndroidElement(id, self))
                     else:
                         self.logger.error("parse element id %s failed.", ele)
                         continue
@@ -253,15 +252,17 @@
                     wait,
                     interval_init,
                 )
                 err_msg = b.err.message
             if wait < retry_init:
                 time.sleep(interval_init / 1000)
         if len(android_element_list) == 0:
-            raise SonicRespException(err_msg)
+            self.logger.info("No elements found.")
+        elif len(android_element_list) > 0:
+            self.logger.info("find elements successful.")
         return android_element_list
 
     def screenshot(self) -> bytes:
         self.check_session_id()
         b = self.resp_handler.get_resp(
             HttpUtil.create_get(
                 self._remote_url + "/session/" + self.session_id + "/screenshot"
```

### Comparing `sonic-uia2-client-0.0.5/common/http_client.py` & `sonic-uia2-client-0.0.6/common/http_client.py`

 * *Files identical despite different names*

### Comparing `sonic-uia2-client-0.0.5/common/logger.py` & `sonic-uia2-client-0.0.6/common/logger.py`

 * *Files identical despite different names*

### Comparing `sonic-uia2-client-0.0.5/common/models.py` & `sonic-uia2-client-0.0.6/common/models.py`

 * *Files identical despite different names*

### Comparing `sonic-uia2-client-0.0.5/common/resp_handler.py` & `sonic-uia2-client-0.0.6/common/resp_handler.py`

 * *Files identical despite different names*

### Comparing `sonic-uia2-client-0.0.5/setup.py` & `sonic-uia2-client-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 import os
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 0
-PATCH = 5
+PATCH = 6
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 
 setup(
     name="sonic-uia2-client",
     version=VERSION,
     author="SonicCloudOrg",
     author_email="soniccloudorg@163.com",
```

### Comparing `sonic-uia2-client-0.0.5/sonic_uia2_client.egg-info/PKG-INFO` & `sonic-uia2-client-0.0.6/sonic_uia2_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sonic-uia2-client
-Version: 0.0.5
+Version: 0.0.6
 Home-page: https://github.com/SonicCloudOrg/sonic-uiautomator2-python-client
 Author: SonicCloudOrg
 Author-email: soniccloudorg@163.com
 License: MIT
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `sonic-uia2-client-0.0.5/tests/test_driver.py` & `sonic-uia2-client-0.0.6/tests/test_driver.py`

 * *Files identical despite different names*

### Comparing `sonic-uia2-client-0.0.5/uia2/driver.py` & `sonic-uia2-client-0.0.6/uia2/driver.py`

 * *Files identical despite different names*

