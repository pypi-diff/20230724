# Comparing `tmp/stock-open-api-0.0.6.tar.gz` & `tmp/stock-open-api-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/stock-open-api-0.0.6.tar", last modified: Wed Jul 19 09:50:44 2023, max compression
+gzip compressed data, was "dist/stock-open-api-0.0.7.tar", last modified: Mon Jul 24 06:39:58 2023, max compression
```

## Comparing `stock-open-api-0.0.6.tar` & `stock-open-api-0.0.7.tar`

### file list

```diff
@@ -1,49 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:50:44.000000 stock-open-api-0.0.6/
--rwxr-xr-x   0 runner    (1001) docker     (123)      414 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-19 09:50:44.000000 stock-open-api-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:50:44.000000 stock-open-api-0.0.6/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/requirements/production.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 09:50:44.000000 stock-open-api-0.0.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3181 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:50:44.000000 stock-open-api-0.0.6/stock_open_api/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:50:44.000000 stock-open-api-0.0.6/stock_open_api/api/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:50:44.000000 stock-open-api-0.0.6/stock_open_api/api/eastmoney/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/api/eastmoney/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/api/eastmoney/company.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/api/eastmoney/company_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/api/eastmoney/hk_stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/api/eastmoney/hk_stock_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/api/eastmoney/kcb_stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/api/eastmoney/kcb_stock_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/api/eastmoney/neeq_stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/api/eastmoney/neeq_stock_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/api/eastmoney/sz_stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/api/eastmoney/us_chinese_stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/api/eastmoney/us_chinese_stock_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:50:44.000000 stock-open-api-0.0.6/stock_open_api/api/sse/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/api/sse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/api/sse/sh_stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/api/sse/sh_stock_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:50:44.000000 stock-open-api-0.0.6/stock_open_api/items/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/items/list_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:50:44.000000 stock-open-api-0.0.6/stock_open_api/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/utils/iterator_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/utils/json_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/utils/request_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/utils/time_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/utils/ua_util.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-19 09:50:33.000000 stock-open-api-0.0.6/stock_open_api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:50:44.000000 stock-open-api-0.0.6/stock_open_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-19 09:50:43.000000 stock-open-api-0.0.6/stock_open_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-19 09:50:43.000000 stock-open-api-0.0.6/stock_open_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 09:50:43.000000 stock-open-api-0.0.6/stock_open_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-19 09:50:43.000000 stock-open-api-0.0.6/stock_open_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-19 09:50:43.000000 stock-open-api-0.0.6/stock_open_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 09:50:43.000000 stock-open-api-0.0.6/stock_open_api.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:39:58.000000 stock-open-api-0.0.7/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      414 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-24 06:39:58.000000 stock-open-api-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:39:58.000000 stock-open-api-0.0.7/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/requirements/production.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 06:39:58.000000 stock-open-api-0.0.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3181 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:39:58.000000 stock-open-api-0.0.7/stock_open_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:39:58.000000 stock-open-api-0.0.7/stock_open_api/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:39:58.000000 stock-open-api-0.0.7/stock_open_api/api/bse/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/api/bse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:39:58.000000 stock-open-api-0.0.7/stock_open_api/api/eastmoney/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/api/eastmoney/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/api/eastmoney/company.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/api/eastmoney/company_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/api/eastmoney/hk_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/api/eastmoney/hk_stock_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/api/eastmoney/kcb_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/api/eastmoney/kcb_stock_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/api/eastmoney/neeq_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/api/eastmoney/neeq_stock_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/api/eastmoney/sh_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/api/eastmoney/sz_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/api/eastmoney/us_chinese_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/api/eastmoney/us_chinese_stock_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:39:58.000000 stock-open-api-0.0.7/stock_open_api/api/sse/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/api/sse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/api/sse/sh_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/api/sse/sh_stock_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:39:58.000000 stock-open-api-0.0.7/stock_open_api/items/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/items/list_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:39:58.000000 stock-open-api-0.0.7/stock_open_api/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/utils/iterator_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/utils/json_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/utils/request_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/utils/time_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/utils/ua_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:39:58.000000 stock-open-api-0.0.7/stock_open_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-24 06:39:57.000000 stock-open-api-0.0.7/stock_open_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-24 06:39:58.000000 stock-open-api-0.0.7/stock_open_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 06:39:57.000000 stock-open-api-0.0.7/stock_open_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 06:39:57.000000 stock-open-api-0.0.7/stock_open_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-24 06:39:57.000000 stock-open-api-0.0.7/stock_open_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 06:39:57.000000 stock-open-api-0.0.7/stock_open_api.egg-info/zip-safe
```

### Comparing `stock-open-api-0.0.6/PKG-INFO` & `stock-open-api-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stock-open-api
-Version: 0.0.6
+Version: 0.0.7
 Summary: a api collection for stock
 Home-page: https://github.com/mouday/stock-open-api
 Author: Peng Shiyu
 Author-email: pengshiyuyx@gmail.com
 License: MIT
 Description: # Stock Open Api
```

### Comparing `stock-open-api-0.0.6/README.md` & `stock-open-api-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.6/setup.py` & `stock-open-api-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.6/stock_open_api/api/eastmoney/company.py` & `stock-open-api-0.0.7/stock_open_api/api/eastmoney/company.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
       "B股代码": null,
       "B股简称": null,
       "H股代码": null,
       "H股简称": null,
       "证券类别": "上交所主板A股",
       "上市交易所": "上海证券交易所",
       "所属东财行业": "轻工制造-家具-家具制造",
-      "所属证监会行业": "鲁昌华,张京跃,王文兵",
+      "所属证监会行业": "制造业-家具制造业",
       "总经理": "许帮顺",
       "法人代表": "孙志勇",
       "董秘": "孙娟",
       "董事长": "孙志勇",
       "证券事务代表": "臧晶晶",
       "独立董事": "鲁昌华,张京跃,王文兵",
       "联系电话": "0551-67186564",
```

### Comparing `stock-open-api-0.0.6/stock_open_api/api/eastmoney/company_config.py` & `stock-open-api-0.0.7/stock_open_api/api/eastmoney/company_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     },
     {
         "title": "所属东财行业",
         "key": "EM2016",
     },
     {
         "title": "所属证监会行业",
-        "key": "INDEDIRECTORS",
+        "key": "INDUSTRYCSRC1",
     },
     {
         "title": "总经理",
         "key": "PRESIDENT",
     },
     {
         "title": "法人代表",
```

### Comparing `stock-open-api-0.0.6/stock_open_api/api/eastmoney/hk_stock.py` & `stock-open-api-0.0.7/stock_open_api/api/eastmoney/hk_stock.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.6/stock_open_api/api/eastmoney/hk_stock_config.py` & `stock-open-api-0.0.7/stock_open_api/api/eastmoney/hk_stock_config.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.6/stock_open_api/api/eastmoney/kcb_stock.py` & `stock-open-api-0.0.7/stock_open_api/api/eastmoney/kcb_stock.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 @File    : kcb_stock.py
 @Date    : 2023-07-17
 科创板相关接口
 """
 
-from stock_open_api.api.eastmoney import kcb_stock_config, sz_stock
+from stock_open_api.api.eastmoney import kcb_stock_config, sh_stock
 from stock_open_api.items.list_item import ListItem
 from stock_open_api.utils import time_util, request_util, json_util
 
 
 def get_list(page=1, size=20):
     """
     科创板列表
@@ -93,17 +93,17 @@
     list_item.items = items
     return list_item
 
 
 def get_company_info(code):
     """
     科创板 公司 基本资料 | 发行相关
-    http://emweb.securities.eastmoney.com/PC_HSF10/CompanySurvey/Index?type=web&code=sh603801
+    https://emweb.securities.eastmoney.com/PC_HSF10/CompanySurvey/Index?type=web&code=sh688092
 
-    :param code: str eg: 688627
+    :param code: str eg: 688092
 
     :return:
 
     >>> get_company_info('688627')
     {
       "公司名称": "志邦家居股份有限公司",
       "英文名称": "Zbom Home Collection Co.,Ltd",
@@ -114,15 +114,15 @@
       "B股代码": null,
       "B股简称": null,
       "H股代码": null,
       "H股简称": null,
       "证券类别": "上交所主板A股",
       "上市交易所": "上海证券交易所",
       "所属东财行业": "轻工制造-家具-家具制造",
-      "所属证监会行业": "鲁昌华,张京跃,王文兵",
+      "所属证监会行业": "制造业-家具制造业",
       "总经理": "许帮顺",
       "法人代表": "孙志勇",
       "董秘": "孙娟",
       "董事长": "孙志勇",
       "证券事务代表": "臧晶晶",
       "独立董事": "鲁昌华,张京跃,王文兵",
       "联系电话": "0551-67186564",
@@ -157,12 +157,13 @@
       "首日换手率": 0.0914,
       "首日最高价(元)": 33.8,
       "网下配售中签率": 0.02743221,
       "定价中签率": 0.03205759
     }
 
     """
-    return sz_stock.get_company_info(code)
+    return sh_stock.get_company_info(code)
 
 
 if __name__ == '__main__':
-    print(json_util.format_json(get_list().to_dict()))
+    # print(json_util.format_json(get_list().to_dict()))
+    print(json_util.format_json(get_company_info('688092')))
```

### Comparing `stock-open-api-0.0.6/stock_open_api/api/eastmoney/kcb_stock_config.py` & `stock-open-api-0.0.7/stock_open_api/api/eastmoney/kcb_stock_config.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.6/stock_open_api/api/eastmoney/neeq_stock.py` & `stock-open-api-0.0.7/stock_open_api/api/eastmoney/neeq_stock.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.6/stock_open_api/api/eastmoney/neeq_stock_config.py` & `stock-open-api-0.0.7/stock_open_api/api/eastmoney/neeq_stock_config.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.6/stock_open_api/api/eastmoney/sz_stock.py` & `stock-open-api-0.0.7/stock_open_api/api/eastmoney/sz_stock.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
           "B股代码": null,
           "B股简称": null,
           "H股代码": null,
           "H股简称": null,
           "证券类别": "上交所主板A股",
           "上市交易所": "上海证券交易所",
           "所属东财行业": "轻工制造-家具-家具制造",
-          "所属证监会行业": "鲁昌华,张京跃,王文兵",
+          "所属证监会行业": "制造业-家具制造业",
           "总经理": "许帮顺",
           "法人代表": "孙志勇",
           "董秘": "孙娟",
           "董事长": "孙志勇",
           "证券事务代表": "臧晶晶",
           "独立董事": "鲁昌华,张京跃,王文兵",
           "联系电话": "0551-67186564",
```

### Comparing `stock-open-api-0.0.6/stock_open_api/api/eastmoney/us_chinese_stock.py` & `stock-open-api-0.0.7/stock_open_api/api/eastmoney/us_chinese_stock.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,9 +212,9 @@
         item[row['title']] = value
 
     return item
 
 
 if __name__ == '__main__':
     # print(json.dumps(get_list().to_dict(), indent=2, ensure_ascii=False))
-    # print(json.dumps(get_org_profile('YBZN'), indent=2, ensure_ascii=False))
-    print(json.dumps(get_security_info('YBZN.O'), indent=2, ensure_ascii=False))
+    # print(json.dumps(get_org_profile('WXT'), indent=2, ensure_ascii=False))
+    print(json.dumps(get_security_info('WXT.O'), indent=2, ensure_ascii=False))
```

### Comparing `stock-open-api-0.0.6/stock_open_api/api/eastmoney/us_chinese_stock_config.py` & `stock-open-api-0.0.7/stock_open_api/api/eastmoney/us_chinese_stock_config.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.6/stock_open_api/api/sse/sh_stock.py` & `stock-open-api-0.0.7/stock_open_api/api/sse/sh_stock.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.6/stock_open_api/api/sse/sh_stock_config.py` & `stock-open-api-0.0.7/stock_open_api/api/sse/sh_stock_config.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.6/stock_open_api/log.py` & `stock-open-api-0.0.7/stock_open_api/log.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.6/stock_open_api/utils/iterator_util.py` & `stock-open-api-0.0.7/stock_open_api/utils/iterator_util.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.6/stock_open_api/utils/request_util.py` & `stock-open-api-0.0.7/stock_open_api/utils/request_util.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.6/stock_open_api.egg-info/PKG-INFO` & `stock-open-api-0.0.7/stock_open_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stock-open-api
-Version: 0.0.6
+Version: 0.0.7
 Summary: a api collection for stock
 Home-page: https://github.com/mouday/stock-open-api
 Author: Peng Shiyu
 Author-email: pengshiyuyx@gmail.com
 License: MIT
 Description: # Stock Open Api
```

### Comparing `stock-open-api-0.0.6/stock_open_api.egg-info/SOURCES.txt` & `stock-open-api-0.0.7/stock_open_api.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,23 +9,25 @@
 stock_open_api.egg-info/PKG-INFO
 stock_open_api.egg-info/SOURCES.txt
 stock_open_api.egg-info/dependency_links.txt
 stock_open_api.egg-info/requires.txt
 stock_open_api.egg-info/top_level.txt
 stock_open_api.egg-info/zip-safe
 stock_open_api/api/__init__.py
+stock_open_api/api/bse/__init__.py
 stock_open_api/api/eastmoney/__init__.py
 stock_open_api/api/eastmoney/company.py
 stock_open_api/api/eastmoney/company_config.py
 stock_open_api/api/eastmoney/hk_stock.py
 stock_open_api/api/eastmoney/hk_stock_config.py
 stock_open_api/api/eastmoney/kcb_stock.py
 stock_open_api/api/eastmoney/kcb_stock_config.py
 stock_open_api/api/eastmoney/neeq_stock.py
 stock_open_api/api/eastmoney/neeq_stock_config.py
+stock_open_api/api/eastmoney/sh_stock.py
 stock_open_api/api/eastmoney/sz_stock.py
 stock_open_api/api/eastmoney/us_chinese_stock.py
 stock_open_api/api/eastmoney/us_chinese_stock_config.py
 stock_open_api/api/sse/__init__.py
 stock_open_api/api/sse/sh_stock.py
 stock_open_api/api/sse/sh_stock_config.py
 stock_open_api/items/__init__.py
```

