# Comparing `tmp/picimagesearch-3.9.4.tar.gz` & `tmp/picimagesearch-3.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picimagesearch-3.9.4.tar", max compression
+gzip compressed data, was "picimagesearch-3.9.5.tar", max compression
```

## Comparing `picimagesearch-3.9.4.tar` & `picimagesearch-3.9.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1063 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/LICENSE
--rw-r--r--   0        0        0      251 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/PicImageSearch/__init__.py
--rw-r--r--   0        0        0     2061 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/PicImageSearch/ascii2d.py
--rw-r--r--   0        0        0     1257 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/PicImageSearch/baidu.py
--rw-r--r--   0        0        0     1415 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/PicImageSearch/ehentai.py
--rw-r--r--   0        0        0     2381 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/PicImageSearch/google.py
--rw-r--r--   0        0        0     1193 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/PicImageSearch/iqdb.py
--rw-r--r--   0        0        0      397 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/PicImageSearch/model/__init__.py
--rw-r--r--   0        0        0     3375 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/PicImageSearch/model/ascii2d.py
--rw-r--r--   0        0        0      778 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/PicImageSearch/model/baidu.py
--rw-r--r--   0        0        0     1895 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/PicImageSearch/model/ehentai.py
--rw-r--r--   0        0        0     2234 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/PicImageSearch/model/google.py
--rw-r--r--   0        0        0     3711 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/PicImageSearch/model/iqdb.py
--rw-r--r--   0        0        0     5170 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/PicImageSearch/model/saucenao.py
--rw-r--r--   0        0        0     2755 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/PicImageSearch/model/tracemoe.py
--rw-r--r--   0        0        0     1312 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/PicImageSearch/model/yandex.py
--rw-r--r--   0        0        0     4576 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/PicImageSearch/network.py
--rw-r--r--   0        0        0     4639 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/PicImageSearch/saucenao.py
--rw-r--r--   0        0        0     1518 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/PicImageSearch/sync.py
--rw-r--r--   0        0        0     4770 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/PicImageSearch/tracemoe.py
--rw-r--r--   0        0        0     1909 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/PicImageSearch/yandex.py
--rw-r--r--   0        0        0     1999 2023-07-13 00:29:39.806856 picimagesearch-3.9.4/README.md
--rw-r--r--   0        0        0     1179 2023-07-13 00:29:39.810856 picimagesearch-3.9.4/pyproject.toml
--rw-r--r--   0        0        0     3064 1970-01-01 00:00:00.000000 picimagesearch-3.9.4/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-24 11:32:25.016061 picimagesearch-3.9.5/LICENSE
+-rw-r--r--   0        0        0      251 2023-07-24 11:32:25.016061 picimagesearch-3.9.5/PicImageSearch/__init__.py
+-rw-r--r--   0        0        0     2061 2023-07-24 11:32:25.016061 picimagesearch-3.9.5/PicImageSearch/ascii2d.py
+-rw-r--r--   0        0        0     1257 2023-07-24 11:32:25.016061 picimagesearch-3.9.5/PicImageSearch/baidu.py
+-rw-r--r--   0        0        0     1415 2023-07-24 11:32:25.016061 picimagesearch-3.9.5/PicImageSearch/ehentai.py
+-rw-r--r--   0        0        0     2381 2023-07-24 11:32:25.016061 picimagesearch-3.9.5/PicImageSearch/google.py
+-rw-r--r--   0        0        0     1193 2023-07-24 11:32:25.016061 picimagesearch-3.9.5/PicImageSearch/iqdb.py
+-rw-r--r--   0        0        0      397 2023-07-24 11:32:25.016061 picimagesearch-3.9.5/PicImageSearch/model/__init__.py
+-rw-r--r--   0        0        0     3375 2023-07-24 11:32:25.020062 picimagesearch-3.9.5/PicImageSearch/model/ascii2d.py
+-rw-r--r--   0        0        0      778 2023-07-24 11:32:25.020062 picimagesearch-3.9.5/PicImageSearch/model/baidu.py
+-rw-r--r--   0        0        0     1895 2023-07-24 11:32:25.020062 picimagesearch-3.9.5/PicImageSearch/model/ehentai.py
+-rw-r--r--   0        0        0     2247 2023-07-24 11:32:25.020062 picimagesearch-3.9.5/PicImageSearch/model/google.py
+-rw-r--r--   0        0        0     3711 2023-07-24 11:32:25.020062 picimagesearch-3.9.5/PicImageSearch/model/iqdb.py
+-rw-r--r--   0        0        0     5170 2023-07-24 11:32:25.020062 picimagesearch-3.9.5/PicImageSearch/model/saucenao.py
+-rw-r--r--   0        0        0     2755 2023-07-24 11:32:25.020062 picimagesearch-3.9.5/PicImageSearch/model/tracemoe.py
+-rw-r--r--   0        0        0     1312 2023-07-24 11:32:25.020062 picimagesearch-3.9.5/PicImageSearch/model/yandex.py
+-rw-r--r--   0        0        0     4576 2023-07-24 11:32:25.020062 picimagesearch-3.9.5/PicImageSearch/network.py
+-rw-r--r--   0        0        0     4639 2023-07-24 11:32:25.020062 picimagesearch-3.9.5/PicImageSearch/saucenao.py
+-rw-r--r--   0        0        0     1518 2023-07-24 11:32:25.020062 picimagesearch-3.9.5/PicImageSearch/sync.py
+-rw-r--r--   0        0        0     4770 2023-07-24 11:32:25.020062 picimagesearch-3.9.5/PicImageSearch/tracemoe.py
+-rw-r--r--   0        0        0     1909 2023-07-24 11:32:25.020062 picimagesearch-3.9.5/PicImageSearch/yandex.py
+-rw-r--r--   0        0        0     1999 2023-07-24 11:32:25.020062 picimagesearch-3.9.5/README.md
+-rw-r--r--   0        0        0     1179 2023-07-24 11:32:25.020062 picimagesearch-3.9.5/pyproject.toml
+-rw-r--r--   0        0        0     3064 1970-01-01 00:00:00.000000 picimagesearch-3.9.5/PKG-INFO
```

### Comparing `picimagesearch-3.9.4/LICENSE` & `picimagesearch-3.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.4/PicImageSearch/ascii2d.py` & `picimagesearch-3.9.5/PicImageSearch/ascii2d.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.4/PicImageSearch/baidu.py` & `picimagesearch-3.9.5/PicImageSearch/baidu.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.4/PicImageSearch/ehentai.py` & `picimagesearch-3.9.5/PicImageSearch/ehentai.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.4/PicImageSearch/google.py` & `picimagesearch-3.9.5/PicImageSearch/google.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.4/PicImageSearch/iqdb.py` & `picimagesearch-3.9.5/PicImageSearch/iqdb.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.4/PicImageSearch/model/ascii2d.py` & `picimagesearch-3.9.5/PicImageSearch/model/ascii2d.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.4/PicImageSearch/model/baidu.py` & `picimagesearch-3.9.5/PicImageSearch/model/baidu.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.4/PicImageSearch/model/ehentai.py` & `picimagesearch-3.9.5/PicImageSearch/model/ehentai.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.4/PicImageSearch/model/google.py` & `picimagesearch-3.9.5/PicImageSearch/model/google.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             for i in data.find('a[aria-label~="Page"]').items()
         ]
         self.pages.insert(index - 1, resp_url)
         script_list = list(data.find("script").items())
         # 结果返回值
         thumbnail_dict: Dict[str, str] = self.create_thumbnail_dict(script_list)
         self.raw: List[GoogleItem] = [
-            GoogleItem(i, thumbnail_dict.get(i("img").attr("id"), None))
+            GoogleItem(i, thumbnail_dict.get(i('img[id^="dimg_"]').attr("id"), None))
             for i in data.find("#search .g").items()
         ]
 
     @staticmethod
     def create_thumbnail_dict(script_list: List[PyQuery]) -> Dict[str, str]:
         thumbnail_dict = {}
         base_64_regex = compile(r"data:image/(?:jpeg|jpg|png|gif);base64,[^'\"]+")
```

### Comparing `picimagesearch-3.9.4/PicImageSearch/model/iqdb.py` & `picimagesearch-3.9.5/PicImageSearch/model/iqdb.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.4/PicImageSearch/model/saucenao.py` & `picimagesearch-3.9.5/PicImageSearch/model/saucenao.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.4/PicImageSearch/model/tracemoe.py` & `picimagesearch-3.9.5/PicImageSearch/model/tracemoe.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.4/PicImageSearch/model/yandex.py` & `picimagesearch-3.9.5/PicImageSearch/model/yandex.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.4/PicImageSearch/network.py` & `picimagesearch-3.9.5/PicImageSearch/network.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.4/PicImageSearch/saucenao.py` & `picimagesearch-3.9.5/PicImageSearch/saucenao.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.4/PicImageSearch/sync.py` & `picimagesearch-3.9.5/PicImageSearch/sync.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.4/PicImageSearch/tracemoe.py` & `picimagesearch-3.9.5/PicImageSearch/tracemoe.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.4/PicImageSearch/yandex.py` & `picimagesearch-3.9.5/PicImageSearch/yandex.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.4/README.md` & `picimagesearch-3.9.5/README.md`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.4/pyproject.toml` & `picimagesearch-3.9.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PicImageSearch"
-version = "3.9.4"
+version = "3.9.5"
 description = "PicImageSearch APIs for Python 3.x 适用于 Python 3 以图搜源整合API"
 authors = ["kitUIN <kulujun@gmail.com>"]
 maintainers = ["kitUIN <kulujun@gmail.com>", "lleans", "chinoll", "NekoAria"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "PicImageSearch" }
```

### Comparing `picimagesearch-3.9.4/PKG-INFO` & `picimagesearch-3.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picimagesearch
-Version: 3.9.4
+Version: 3.9.5
 Summary: PicImageSearch APIs for Python 3.x 适用于 Python 3 以图搜源整合API
 Home-page: https://github.com/kitUIN/PicImageSearch
 License: MIT
 Keywords: ascii2d,baidu,e-hentai,google,iqdb,saucenao,tracemoe,yandex
 Author: kitUIN
 Author-email: kulujun@gmail.com
 Maintainer: kitUIN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: picimagesearch Version: 3.9.4 Summary:
+Metadata-Version: 2.1 Name: picimagesearch Version: 3.9.5 Summary:
 PicImageSearch APIs for Python 3.x éç¨äº Python 3 ä»¥å¾ææºæ´åAPI
 Home-page: https://github.com/kitUIN/PicImageSearch License: MIT Keywords:
 ascii2d,baidu,e-hentai,google,iqdb,saucenao,tracemoe,yandex Author: kitUIN
 Author-email: kulujun@gmail.com Maintainer: kitUIN Maintainer-email:
 kulujun@gmail.com Requires-Python: >=3.7,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
```

