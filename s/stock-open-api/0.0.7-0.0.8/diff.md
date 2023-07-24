# Comparing `tmp/stock-open-api-0.0.7.tar.gz` & `tmp/stock-open-api-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/stock-open-api-0.0.7.tar", last modified: Mon Jul 24 06:39:58 2023, max compression
+gzip compressed data, was "dist/stock-open-api-0.0.8.tar", last modified: Mon Jul 24 06:54:37 2023, max compression
```

## Comparing `stock-open-api-0.0.7.tar` & `stock-open-api-0.0.8.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:39:58.000000 stock-open-api-0.0.7/
--rwxr-xr-x   0 runner    (1001) docker     (123)      414 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-24 06:39:58.000000 stock-open-api-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:39:58.000000 stock-open-api-0.0.7/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/requirements/production.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 06:39:58.000000 stock-open-api-0.0.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3181 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:39:58.000000 stock-open-api-0.0.7/stock_open_api/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:39:58.000000 stock-open-api-0.0.7/stock_open_api/api/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:39:58.000000 stock-open-api-0.0.7/stock_open_api/api/bse/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/api/bse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:39:58.000000 stock-open-api-0.0.7/stock_open_api/api/eastmoney/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/api/eastmoney/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/api/eastmoney/company.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/api/eastmoney/company_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/api/eastmoney/hk_stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/api/eastmoney/hk_stock_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/api/eastmoney/kcb_stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/api/eastmoney/kcb_stock_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/api/eastmoney/neeq_stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/api/eastmoney/neeq_stock_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/api/eastmoney/sh_stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/api/eastmoney/sz_stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/api/eastmoney/us_chinese_stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/api/eastmoney/us_chinese_stock_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:39:58.000000 stock-open-api-0.0.7/stock_open_api/api/sse/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/api/sse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/api/sse/sh_stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/api/sse/sh_stock_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:39:58.000000 stock-open-api-0.0.7/stock_open_api/items/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/items/list_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:39:58.000000 stock-open-api-0.0.7/stock_open_api/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/utils/iterator_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/utils/json_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/utils/request_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/utils/time_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/utils/ua_util.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-24 06:39:41.000000 stock-open-api-0.0.7/stock_open_api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:39:58.000000 stock-open-api-0.0.7/stock_open_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-24 06:39:57.000000 stock-open-api-0.0.7/stock_open_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-24 06:39:58.000000 stock-open-api-0.0.7/stock_open_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 06:39:57.000000 stock-open-api-0.0.7/stock_open_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 06:39:57.000000 stock-open-api-0.0.7/stock_open_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-24 06:39:57.000000 stock-open-api-0.0.7/stock_open_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 06:39:57.000000 stock-open-api-0.0.7/stock_open_api.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:54:37.000000 stock-open-api-0.0.8/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      414 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-07-24 06:54:37.000000 stock-open-api-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:54:37.000000 stock-open-api-0.0.8/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/requirements/production.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 06:54:37.000000 stock-open-api-0.0.8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3181 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:54:37.000000 stock-open-api-0.0.8/stock_open_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:54:37.000000 stock-open-api-0.0.8/stock_open_api/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:54:37.000000 stock-open-api-0.0.8/stock_open_api/api/bse/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/api/bse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:54:37.000000 stock-open-api-0.0.8/stock_open_api/api/eastmoney/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/api/eastmoney/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/api/eastmoney/company.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/api/eastmoney/company_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/api/eastmoney/hk_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/api/eastmoney/hk_stock_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/api/eastmoney/kcb_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/api/eastmoney/kcb_stock_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/api/eastmoney/neeq_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/api/eastmoney/neeq_stock_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/api/eastmoney/sh_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/api/eastmoney/sz_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/api/eastmoney/us_chinese_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/api/eastmoney/us_chinese_stock_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:54:37.000000 stock-open-api-0.0.8/stock_open_api/api/sse/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/api/sse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/api/sse/sh_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/api/sse/sh_stock_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:54:37.000000 stock-open-api-0.0.8/stock_open_api/items/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/items/list_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:54:37.000000 stock-open-api-0.0.8/stock_open_api/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/utils/iterator_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/utils/json_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/utils/request_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/utils/time_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/utils/ua_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-24 06:54:25.000000 stock-open-api-0.0.8/stock_open_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:54:37.000000 stock-open-api-0.0.8/stock_open_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-07-24 06:54:37.000000 stock-open-api-0.0.8/stock_open_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-24 06:54:37.000000 stock-open-api-0.0.8/stock_open_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 06:54:37.000000 stock-open-api-0.0.8/stock_open_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 06:54:37.000000 stock-open-api-0.0.8/stock_open_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-24 06:54:37.000000 stock-open-api-0.0.8/stock_open_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 06:54:37.000000 stock-open-api-0.0.8/stock_open_api.egg-info/zip-safe
```

### Comparing `stock-open-api-0.0.7/PKG-INFO` & `stock-open-api-0.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stock-open-api
-Version: 0.0.7
+Version: 0.0.8
 Summary: a api collection for stock
 Home-page: https://github.com/mouday/stock-open-api
 Author: Peng Shiyu
 Author-email: pengshiyuyx@gmail.com
 License: MIT
 Description: # Stock Open Api
         
@@ -97,29 +97,26 @@
         | [公司概况](http://www.sse.com.cn/assortment/stock/list/info/company/index.shtml?COMPANY_CODE=688001) | api/sse/sh_stock.get_company_info |
         
         数据源：东方财富 [www.eastmoney.com](https://www.eastmoney.com/)
         
         | 数据 | 方法名 |
         | - | - | 
         | [港股-列表](http://www.sse.com.cn/assortment/stock/list/info/company/index.shtml?COMPANY_CODE=688001) | api/eastmoney/hk_stock.get_list |
-        | [港股-列表迭代器](http://www.sse.com.cn/assortment/stock/list/info/company/index.shtml?COMPANY_CODE=688001) | api/eastmoney/hk_stock.get_list_iter |
         | [港股-公司资料](http://emweb.securities.eastmoney.com/PC_HKF10/pages/home/index.html?code=00491&type=web&color=w#/CompanyProfile) | api/eastmoney/hk_stock.get_org_profile |
         | [港股-证券资料](http://emweb.securities.eastmoney.com/PC_HKF10/pages/home/index.html?code=00491&type=web&color=w#/CompanyProfile) | api/eastmoney/hk_stock.get_security_info |
         | [中国概念股-列表](http://quote.eastmoney.com/center/gridlist.html#us_chinese) | api/eastmoney/us_chinese_stock.get_list |
-        | [中国概念股-列表迭代器](http://quote.eastmoney.com/center/gridlist.html#us_chinese) | api/eastmoney/us_chinese_stock.get_list_iter |
         | [中国概念股-公司资料](http://emweb.eastmoney.com/PC_USF10/pages/index.html?code=PWM&type=web&color=w#/gsgk/gszl) | api/eastmoney/us_chinese_stock.get_org_profile |
         | [中国概念股-证券资料](http://emweb.eastmoney.com/PC_USF10/pages/index.html?code=PWM&type=web&color=w#/gsgk/zqzl) | api/eastmoney/us_chinese_stock.get_security_info |
         | [科创板-列表](http://quote.eastmoney.com/center/gridlist.html#kcb_board) | api/eastmoney/kcb_stock.get_list |
-        | [科创板-列表迭代器](http://quote.eastmoney.com/center/gridlist.html#kcb_board) | api/eastmoney/kcb_stock.get_list_iter |
         | [科创板-基本资料+发行相关](http://emweb.securities.eastmoney.com/PC_HSF10/CompanySurvey/Index?type=web&code=sh603801) | api/eastmoney/kcb_stock.get_company_info |
         | [新三板-列表](http://quote.eastmoney.com/center/gridlist.html#neeq_stocks) | api/eastmoney/neeq_stock.get_list |
-        | [新三板-列表迭代器](http://quote.eastmoney.com/center/gridlist.html#neeq_stocks) | api/eastmoney/neeq_stock.get_list_iter |
         | [新三板-公司资料+证券资料](http://xinsanban.eastmoney.com/F10/CompanyInfo/Introduction/839499.html) | api/eastmoney/neeq_stock.get_company_info |
         | [A股-基本资料+发行相关](http://emweb.securities.eastmoney.com/PC_HSF10/CompanySurvey/Index?type=web&code=sh603801) | api/eastmoney/company.get_company_info |
         | [深圳A股-基本资料+发行相关](http://emweb.securities.eastmoney.com/PC_HSF10/CompanySurvey/Index?type=web&code=sh603801) | api/eastmoney/sz_stock.get_company_info |
+        | [上证A股-基本资料+发行相关](http://emweb.securities.eastmoney.com/PC_HSF10/CompanySurvey/Index?type=web&code=sh603801) | api/eastmoney/sh_stock.get_company_info |
         
         ## 升级记录 
          
         [CHANGELOG.md](https://github.com/mouday/stock-open-api/blob/master/CHANGELOG.md)
         
         ## 其他相关库
```

### Comparing `stock-open-api-0.0.7/README.md` & `stock-open-api-0.0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -89,29 +89,26 @@
 | [公司概况](http://www.sse.com.cn/assortment/stock/list/info/company/index.shtml?COMPANY_CODE=688001) | api/sse/sh_stock.get_company_info |
 
 数据源：东方财富 [www.eastmoney.com](https://www.eastmoney.com/)
 
 | 数据 | 方法名 |
 | - | - | 
 | [港股-列表](http://www.sse.com.cn/assortment/stock/list/info/company/index.shtml?COMPANY_CODE=688001) | api/eastmoney/hk_stock.get_list |
-| [港股-列表迭代器](http://www.sse.com.cn/assortment/stock/list/info/company/index.shtml?COMPANY_CODE=688001) | api/eastmoney/hk_stock.get_list_iter |
 | [港股-公司资料](http://emweb.securities.eastmoney.com/PC_HKF10/pages/home/index.html?code=00491&type=web&color=w#/CompanyProfile) | api/eastmoney/hk_stock.get_org_profile |
 | [港股-证券资料](http://emweb.securities.eastmoney.com/PC_HKF10/pages/home/index.html?code=00491&type=web&color=w#/CompanyProfile) | api/eastmoney/hk_stock.get_security_info |
 | [中国概念股-列表](http://quote.eastmoney.com/center/gridlist.html#us_chinese) | api/eastmoney/us_chinese_stock.get_list |
-| [中国概念股-列表迭代器](http://quote.eastmoney.com/center/gridlist.html#us_chinese) | api/eastmoney/us_chinese_stock.get_list_iter |
 | [中国概念股-公司资料](http://emweb.eastmoney.com/PC_USF10/pages/index.html?code=PWM&type=web&color=w#/gsgk/gszl) | api/eastmoney/us_chinese_stock.get_org_profile |
 | [中国概念股-证券资料](http://emweb.eastmoney.com/PC_USF10/pages/index.html?code=PWM&type=web&color=w#/gsgk/zqzl) | api/eastmoney/us_chinese_stock.get_security_info |
 | [科创板-列表](http://quote.eastmoney.com/center/gridlist.html#kcb_board) | api/eastmoney/kcb_stock.get_list |
-| [科创板-列表迭代器](http://quote.eastmoney.com/center/gridlist.html#kcb_board) | api/eastmoney/kcb_stock.get_list_iter |
 | [科创板-基本资料+发行相关](http://emweb.securities.eastmoney.com/PC_HSF10/CompanySurvey/Index?type=web&code=sh603801) | api/eastmoney/kcb_stock.get_company_info |
 | [新三板-列表](http://quote.eastmoney.com/center/gridlist.html#neeq_stocks) | api/eastmoney/neeq_stock.get_list |
-| [新三板-列表迭代器](http://quote.eastmoney.com/center/gridlist.html#neeq_stocks) | api/eastmoney/neeq_stock.get_list_iter |
 | [新三板-公司资料+证券资料](http://xinsanban.eastmoney.com/F10/CompanyInfo/Introduction/839499.html) | api/eastmoney/neeq_stock.get_company_info |
 | [A股-基本资料+发行相关](http://emweb.securities.eastmoney.com/PC_HSF10/CompanySurvey/Index?type=web&code=sh603801) | api/eastmoney/company.get_company_info |
 | [深圳A股-基本资料+发行相关](http://emweb.securities.eastmoney.com/PC_HSF10/CompanySurvey/Index?type=web&code=sh603801) | api/eastmoney/sz_stock.get_company_info |
+| [上证A股-基本资料+发行相关](http://emweb.securities.eastmoney.com/PC_HSF10/CompanySurvey/Index?type=web&code=sh603801) | api/eastmoney/sh_stock.get_company_info |
 
 ## 升级记录 
  
 [CHANGELOG.md](https://github.com/mouday/stock-open-api/blob/master/CHANGELOG.md)
 
 ## 其他相关库
```

### Comparing `stock-open-api-0.0.7/setup.py` & `stock-open-api-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.7/stock_open_api/api/eastmoney/company.py` & `stock-open-api-0.0.8/stock_open_api/api/eastmoney/company.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,15 +99,16 @@
     item = {}
     for row in company_config.company_key_map:
         value = company_info.get(row['key'])
         if isinstance(value, str):
             value = value.strip()
 
         # 上市日期 成立日期 网上发行日期
-        if row['key'] in ['LISTING_DATE', 'FOUND_DATE', 'ONLINE_ISSUE_DATE']:
+        # fix: AttributeError: 'NoneType' object has no attribute 'split'
+        if row['key'] in ['LISTING_DATE', 'FOUND_DATE', 'ONLINE_ISSUE_DATE'] and value:
             value = value.split(' ')[0]
 
         item[row['title']] = value
 
     return item
```

### Comparing `stock-open-api-0.0.7/stock_open_api/api/eastmoney/company_config.py` & `stock-open-api-0.0.8/stock_open_api/api/eastmoney/company_config.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.7/stock_open_api/api/eastmoney/hk_stock.py` & `stock-open-api-0.0.8/stock_open_api/api/eastmoney/hk_stock.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.7/stock_open_api/api/eastmoney/hk_stock_config.py` & `stock-open-api-0.0.8/stock_open_api/api/eastmoney/hk_stock_config.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.7/stock_open_api/api/eastmoney/kcb_stock.py` & `stock-open-api-0.0.8/stock_open_api/api/eastmoney/kcb_stock.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.7/stock_open_api/api/eastmoney/kcb_stock_config.py` & `stock-open-api-0.0.8/stock_open_api/api/eastmoney/kcb_stock_config.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.7/stock_open_api/api/eastmoney/neeq_stock.py` & `stock-open-api-0.0.8/stock_open_api/api/eastmoney/neeq_stock.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.7/stock_open_api/api/eastmoney/neeq_stock_config.py` & `stock-open-api-0.0.8/stock_open_api/api/eastmoney/neeq_stock_config.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.7/stock_open_api/api/eastmoney/sh_stock.py` & `stock-open-api-0.0.8/stock_open_api/api/eastmoney/sh_stock.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.7/stock_open_api/api/eastmoney/sz_stock.py` & `stock-open-api-0.0.8/stock_open_api/api/eastmoney/sz_stock.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.7/stock_open_api/api/eastmoney/us_chinese_stock.py` & `stock-open-api-0.0.8/stock_open_api/api/eastmoney/us_chinese_stock.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.7/stock_open_api/api/eastmoney/us_chinese_stock_config.py` & `stock-open-api-0.0.8/stock_open_api/api/eastmoney/us_chinese_stock_config.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.7/stock_open_api/api/sse/sh_stock.py` & `stock-open-api-0.0.8/stock_open_api/api/sse/sh_stock.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.7/stock_open_api/api/sse/sh_stock_config.py` & `stock-open-api-0.0.8/stock_open_api/api/sse/sh_stock_config.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.7/stock_open_api/log.py` & `stock-open-api-0.0.8/stock_open_api/log.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.7/stock_open_api/utils/request_util.py` & `stock-open-api-0.0.8/stock_open_api/utils/request_util.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.7/stock_open_api.egg-info/PKG-INFO` & `stock-open-api-0.0.8/stock_open_api.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stock-open-api
-Version: 0.0.7
+Version: 0.0.8
 Summary: a api collection for stock
 Home-page: https://github.com/mouday/stock-open-api
 Author: Peng Shiyu
 Author-email: pengshiyuyx@gmail.com
 License: MIT
 Description: # Stock Open Api
         
@@ -97,29 +97,26 @@
         | [公司概况](http://www.sse.com.cn/assortment/stock/list/info/company/index.shtml?COMPANY_CODE=688001) | api/sse/sh_stock.get_company_info |
         
         数据源：东方财富 [www.eastmoney.com](https://www.eastmoney.com/)
         
         | 数据 | 方法名 |
         | - | - | 
         | [港股-列表](http://www.sse.com.cn/assortment/stock/list/info/company/index.shtml?COMPANY_CODE=688001) | api/eastmoney/hk_stock.get_list |
-        | [港股-列表迭代器](http://www.sse.com.cn/assortment/stock/list/info/company/index.shtml?COMPANY_CODE=688001) | api/eastmoney/hk_stock.get_list_iter |
         | [港股-公司资料](http://emweb.securities.eastmoney.com/PC_HKF10/pages/home/index.html?code=00491&type=web&color=w#/CompanyProfile) | api/eastmoney/hk_stock.get_org_profile |
         | [港股-证券资料](http://emweb.securities.eastmoney.com/PC_HKF10/pages/home/index.html?code=00491&type=web&color=w#/CompanyProfile) | api/eastmoney/hk_stock.get_security_info |
         | [中国概念股-列表](http://quote.eastmoney.com/center/gridlist.html#us_chinese) | api/eastmoney/us_chinese_stock.get_list |
-        | [中国概念股-列表迭代器](http://quote.eastmoney.com/center/gridlist.html#us_chinese) | api/eastmoney/us_chinese_stock.get_list_iter |
         | [中国概念股-公司资料](http://emweb.eastmoney.com/PC_USF10/pages/index.html?code=PWM&type=web&color=w#/gsgk/gszl) | api/eastmoney/us_chinese_stock.get_org_profile |
         | [中国概念股-证券资料](http://emweb.eastmoney.com/PC_USF10/pages/index.html?code=PWM&type=web&color=w#/gsgk/zqzl) | api/eastmoney/us_chinese_stock.get_security_info |
         | [科创板-列表](http://quote.eastmoney.com/center/gridlist.html#kcb_board) | api/eastmoney/kcb_stock.get_list |
-        | [科创板-列表迭代器](http://quote.eastmoney.com/center/gridlist.html#kcb_board) | api/eastmoney/kcb_stock.get_list_iter |
         | [科创板-基本资料+发行相关](http://emweb.securities.eastmoney.com/PC_HSF10/CompanySurvey/Index?type=web&code=sh603801) | api/eastmoney/kcb_stock.get_company_info |
         | [新三板-列表](http://quote.eastmoney.com/center/gridlist.html#neeq_stocks) | api/eastmoney/neeq_stock.get_list |
-        | [新三板-列表迭代器](http://quote.eastmoney.com/center/gridlist.html#neeq_stocks) | api/eastmoney/neeq_stock.get_list_iter |
         | [新三板-公司资料+证券资料](http://xinsanban.eastmoney.com/F10/CompanyInfo/Introduction/839499.html) | api/eastmoney/neeq_stock.get_company_info |
         | [A股-基本资料+发行相关](http://emweb.securities.eastmoney.com/PC_HSF10/CompanySurvey/Index?type=web&code=sh603801) | api/eastmoney/company.get_company_info |
         | [深圳A股-基本资料+发行相关](http://emweb.securities.eastmoney.com/PC_HSF10/CompanySurvey/Index?type=web&code=sh603801) | api/eastmoney/sz_stock.get_company_info |
+        | [上证A股-基本资料+发行相关](http://emweb.securities.eastmoney.com/PC_HSF10/CompanySurvey/Index?type=web&code=sh603801) | api/eastmoney/sh_stock.get_company_info |
         
         ## 升级记录 
          
         [CHANGELOG.md](https://github.com/mouday/stock-open-api/blob/master/CHANGELOG.md)
         
         ## 其他相关库
```

### Comparing `stock-open-api-0.0.7/stock_open_api.egg-info/SOURCES.txt` & `stock-open-api-0.0.8/stock_open_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

