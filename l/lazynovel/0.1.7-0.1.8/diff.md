# Comparing `tmp/lazynovel-0.1.7.tar.gz` & `tmp/lazynovel-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazynovel-0.1.7.tar", last modified: Mon Jul 24 04:11:07 2023, max compression
+gzip compressed data, was "lazynovel-0.1.8.tar", last modified: Mon Jul 24 04:30:03 2023, max compression
```

## Comparing `lazynovel-0.1.7.tar` & `lazynovel-0.1.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-24 04:11:07.082623 lazynovel-0.1.7/
--rw-r--r--   0 zeroseeker   (501) staff       (20)    35181 2023-02-28 06:27:15.000000 lazynovel-0.1.7/LICENSE
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1305 2023-07-24 04:11:07.082497 lazynovel-0.1.7/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      954 2023-02-28 06:27:15.000000 lazynovel-0.1.7/README.md
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-24 04:11:07.081415 lazynovel-0.1.7/lazynovel/
--rw-r--r--   0 zeroseeker   (501) staff       (20)      415 2023-05-25 10:17:10.000000 lazynovel-0.1.7/lazynovel/__init__.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    11345 2023-07-24 04:10:03.000000 lazynovel-0.1.7/lazynovel/crawler_changdu.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    10870 2023-06-28 07:17:21.000000 lazynovel-0.1.7/lazynovel/crawler_mbookcn.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     5914 2023-07-05 07:09:26.000000 lazynovel-0.1.7/lazynovel/crawler_reading163.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    10568 2023-02-28 06:27:15.000000 lazynovel-0.1.7/lazynovel/open_changdu.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     9853 2023-02-28 06:27:15.000000 lazynovel-0.1.7/lazynovel/open_dianzhong.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     9680 2023-02-28 06:27:15.000000 lazynovel-0.1.7/lazynovel/open_mbookcn.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    21587 2023-05-29 10:32:37.000000 lazynovel-0.1.7/lazynovel/open_reading163.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      830 2023-02-28 06:27:15.000000 lazynovel-0.1.7/lazynovel/open_yangguang.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     2694 2023-02-28 06:27:15.000000 lazynovel-0.1.7/lazynovel/open_yiqbook.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    57844 2023-02-28 06:27:15.000000 lazynovel-0.1.7/lazynovel/open_yuewen.py
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-24 04:11:07.082280 lazynovel-0.1.7/lazynovel.egg-info/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1305 2023-07-24 04:11:07.000000 lazynovel-0.1.7/lazynovel.egg-info/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      490 2023-07-24 04:11:07.000000 lazynovel-0.1.7/lazynovel.egg-info/SOURCES.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2023-07-24 04:11:07.000000 lazynovel-0.1.7/lazynovel.egg-info/dependency_links.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       15 2023-07-24 04:11:07.000000 lazynovel-0.1.7/lazynovel.egg-info/requires.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       10 2023-07-24 04:11:07.000000 lazynovel-0.1.7/lazynovel.egg-info/top_level.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2023-07-24 04:11:07.082670 lazynovel-0.1.7/setup.cfg
--rw-r--r--   0 zeroseeker   (501) staff       (20)      869 2023-07-24 04:10:30.000000 lazynovel-0.1.7/setup.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-24 04:30:03.844418 lazynovel-0.1.8/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    35181 2023-02-28 06:27:15.000000 lazynovel-0.1.8/LICENSE
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1305 2023-07-24 04:30:03.844320 lazynovel-0.1.8/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      954 2023-02-28 06:27:15.000000 lazynovel-0.1.8/README.md
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-24 04:30:03.843428 lazynovel-0.1.8/lazynovel/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      415 2023-05-25 10:17:10.000000 lazynovel-0.1.8/lazynovel/__init__.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    12391 2023-07-24 04:29:37.000000 lazynovel-0.1.8/lazynovel/crawler_changdu.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    10870 2023-06-28 07:17:21.000000 lazynovel-0.1.8/lazynovel/crawler_mbookcn.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     5914 2023-07-05 07:09:26.000000 lazynovel-0.1.8/lazynovel/crawler_reading163.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    10568 2023-02-28 06:27:15.000000 lazynovel-0.1.8/lazynovel/open_changdu.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     9853 2023-02-28 06:27:15.000000 lazynovel-0.1.8/lazynovel/open_dianzhong.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     9680 2023-02-28 06:27:15.000000 lazynovel-0.1.8/lazynovel/open_mbookcn.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    21587 2023-05-29 10:32:37.000000 lazynovel-0.1.8/lazynovel/open_reading163.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      830 2023-02-28 06:27:15.000000 lazynovel-0.1.8/lazynovel/open_yangguang.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     2694 2023-02-28 06:27:15.000000 lazynovel-0.1.8/lazynovel/open_yiqbook.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    57844 2023-02-28 06:27:15.000000 lazynovel-0.1.8/lazynovel/open_yuewen.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-24 04:30:03.844169 lazynovel-0.1.8/lazynovel.egg-info/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1305 2023-07-24 04:30:03.000000 lazynovel-0.1.8/lazynovel.egg-info/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      490 2023-07-24 04:30:03.000000 lazynovel-0.1.8/lazynovel.egg-info/SOURCES.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2023-07-24 04:30:03.000000 lazynovel-0.1.8/lazynovel.egg-info/dependency_links.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       15 2023-07-24 04:30:03.000000 lazynovel-0.1.8/lazynovel.egg-info/requires.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       10 2023-07-24 04:30:03.000000 lazynovel-0.1.8/lazynovel.egg-info/top_level.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2023-07-24 04:30:03.844456 lazynovel-0.1.8/setup.cfg
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      869 2023-07-24 04:29:37.000000 lazynovel-0.1.8/setup.py
```

### Comparing `lazynovel-0.1.7/LICENSE` & `lazynovel-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.7/PKG-INFO` & `lazynovel-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazynovel
-Version: 0.1.7
+Version: 0.1.8
 Summary: 小说平台接口封包
 Home-page: https://gitee.com/ZeroSeeker/lazynovel
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `lazynovel-0.1.7/README.md` & `lazynovel-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.7/lazynovel/crawler_changdu.py` & `lazynovel-0.1.8/lazynovel/crawler_changdu.py`

 * *Files 2% similar despite different names*

```diff
@@ -353,7 +353,40 @@
     return lazyrequests.lazy_requests(
         method='GET',
         url=url,
         headers=headers,
         params=params,
         return_json=True
     )
+
+
+def apps_from_login_v1(
+        cookie: str
+):
+    """
+    获取apps列表，所有的
+    """
+    url = 'https://www.changdunovel.com/novelsale/distributor/login/v1/'
+    headers = {
+        "Accept": "application/json, text/plain, */*",
+        "Accept-Encoding": "gzip, deflate",
+        "Accept-Language": "zh-CN,zh;q=0.8,zh-TW;q=0.7,zh-HK;q=0.5,en-US;q=0.3,en;q=0.2",
+        "Connection": "keep-alive",
+        "Cookie": cookie,
+        "Host": "www.changdunovel.com",
+        "Referer": "https://www.changdunovel.com/sale/monitor/center",
+        "Sec-Fetch-Dest": "empty",
+        "Sec-Fetch-Mode": "cors",
+        "Sec-Fetch-Site": "same-origin",
+        "TE": "trailers",
+        "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10.15; rv:108.0) Gecko/20100101 Firefox/108.0",
+        "agw-js-conv": "str",
+        # "appid": "0",
+        # "apptype": "1",
+        # "distributorid": "0"
+    }
+    return lazyrequests.lazy_requests(
+        method='GET',
+        url=url,
+        headers=headers,
+        return_json=True
+    )
```

### Comparing `lazynovel-0.1.7/lazynovel/crawler_mbookcn.py` & `lazynovel-0.1.8/lazynovel/crawler_mbookcn.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.7/lazynovel/crawler_reading163.py` & `lazynovel-0.1.8/lazynovel/crawler_reading163.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.7/lazynovel/open_changdu.py` & `lazynovel-0.1.8/lazynovel/open_changdu.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.7/lazynovel/open_dianzhong.py` & `lazynovel-0.1.8/lazynovel/open_dianzhong.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.7/lazynovel/open_mbookcn.py` & `lazynovel-0.1.8/lazynovel/open_mbookcn.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.7/lazynovel/open_reading163.py` & `lazynovel-0.1.8/lazynovel/open_reading163.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.7/lazynovel/open_yangguang.py` & `lazynovel-0.1.8/lazynovel/open_yangguang.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.7/lazynovel/open_yiqbook.py` & `lazynovel-0.1.8/lazynovel/open_yiqbook.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.7/lazynovel/open_yuewen.py` & `lazynovel-0.1.8/lazynovel/open_yuewen.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.7/lazynovel.egg-info/PKG-INFO` & `lazynovel-0.1.8/lazynovel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazynovel
-Version: 0.1.7
+Version: 0.1.8
 Summary: 小说平台接口封包
 Home-page: https://gitee.com/ZeroSeeker/lazynovel
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `lazynovel-0.1.7/setup.py` & `lazynovel-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lazynovel",
-    version="0.1.7",
+    version="0.1.8",
     description="小说平台接口封包",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ZeroSeeker",
     author_email="zeroseeker@foxmail.com",
     url="https://gitee.com/ZeroSeeker/lazynovel",
     packages=setuptools.find_packages(),
```

