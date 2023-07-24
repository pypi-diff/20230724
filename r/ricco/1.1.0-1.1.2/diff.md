# Comparing `tmp/ricco-1.1.0.tar.gz` & `tmp/ricco-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ricco-1.1.0.tar", last modified: Fri May  5 10:31:41 2023, max compression
+gzip compressed data, was "ricco-1.1.2.tar", last modified: Mon Jul 24 07:56:07 2023, max compression
```

## Comparing `ricco-1.1.0.tar` & `ricco-1.1.2.tar`

### file list

```diff
@@ -1,48 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:31:41.215655 ricco-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-05 10:31:41.215655 ricco-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-05 10:31:28.000000 ricco-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 10:31:41.215655 ricco-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-05 10:31:28.000000 ricco-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:31:41.211655 ricco-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:31:41.215655 ricco-1.1.0/src/ricco/
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:31:41.215655 ricco-1.1.0/src/ricco/etl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/etl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/etl/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/etl/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/etl/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/etl/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:31:41.215655 ricco-1.1.0/src/ricco/geocode/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/geocode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/geocode/amap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/geocode/baidu.py
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/geocode/geocode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/geocode/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:31:41.215655 ricco-1.1.0/src/ricco/resource/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   161544 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/resource/area_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    15551 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/resource/city_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/resource/crs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23330 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/resource/epsg_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/resource/names.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/resource/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/resource/phone_number.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:31:41.215655 ricco-1.1.0/src/ricco/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/util/address_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/util/building_address.py
--rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/util/coord_trans.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/util/dt.py
--rw-r--r--   0 runner    (1001) docker     (123)    15686 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/util/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/util/id_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/util/os.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/util/phone_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/util/strings.py
--rw-r--r--   0 runner    (1001) docker     (123)    11322 2023-05-05 10:31:28.000000 ricco-1.1.0/src/ricco/util/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:31:41.215655 ricco-1.1.0/src/ricco.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-05 10:31:41.000000 ricco-1.1.0/src/ricco.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-05 10:31:41.000000 ricco-1.1.0/src/ricco.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 10:31:41.000000 ricco-1.1.0/src/ricco.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-05 10:31:41.000000 ricco-1.1.0/src/ricco.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-05 10:31:41.000000 ricco-1.1.0/src/ricco.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:56:07.241949 ricco-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-24 07:56:07.241949 ricco-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-24 07:55:57.000000 ricco-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 07:56:07.245949 ricco-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-24 07:55:57.000000 ricco-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:56:07.237949 ricco-1.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:56:07.241949 ricco-1.1.2/src/ricco/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:56:07.241949 ricco-1.1.2/src/ricco/etl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/etl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/etl/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/etl/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/etl/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/etl/stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/etl/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:56:07.241949 ricco-1.1.2/src/ricco/geocode/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/geocode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/geocode/amap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/geocode/baidu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/geocode/geocode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/geocode/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:56:07.241949 ricco-1.1.2/src/ricco/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   161544 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/resource/area_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15551 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/resource/city_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/resource/crs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23330 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/resource/epsg_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/resource/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/resource/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/resource/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/resource/phone_number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:56:07.241949 ricco-1.1.2/src/ricco/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/util/address_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/util/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/util/building_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/util/coord_trans.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/util/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/util/docx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/util/dt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22210 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/util/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/util/id_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/util/os.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/util/phone_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/util/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/util/topology_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13557 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/util/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:56:07.241949 ricco-1.1.2/src/ricco.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-24 07:56:07.000000 ricco-1.1.2/src/ricco.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-24 07:56:07.000000 ricco-1.1.2/src/ricco.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 07:56:07.000000 ricco-1.1.2/src/ricco.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-24 07:56:07.000000 ricco-1.1.2/src/ricco.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 07:56:07.000000 ricco-1.1.2/src/ricco.egg-info/top_level.txt
```

### Comparing `ricco-1.1.0/PKG-INFO` & `ricco-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ricco
-Version: 1.1.0
+Version: 1.1.2
 Summary: A handy ETL&GEOM kit
 Home-page: https://github.com/Ricco1010/ricco
 Author: Ricco Wang
 Author-email: wyk_0610@163.com
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ricco-1.1.0/setup.py` & `ricco-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `ricco-1.1.0/src/ricco/__init__.py` & `ricco-1.1.2/src/ricco/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-__version__ = '1.1.0'
+__version__ = '1.1.2'
 
 from .etl import file
 from .etl import load
 from .etl import transformer
 from .etl.extract import rdf
 from .etl.transformer import expand_dict
+from .etl.transformer import table2dict
 from .geocode.geocode import geocode
 from .geocode.geocode import geocode_df
+from .local import Rc
+from .local import Ricco
 from .util import coord_trans
 from .util import dt
 from .util import geom
 from .util import id_number
 from .util import os
 from .util import phone_number
 from .util import strings
@@ -24,8 +27,11 @@
 from .util.os import mkdir_2
 from .util.strings import drop_repeat_string
 from .util.util import extract_num
 from .util.util import is_empty
 from .util.util import list2dict
 from .util.util import not_empty
 from .util.util import pinyin
+from .util.util import re_fast
 from .util.util import segment
+from .util.util import union_list
+from .util.util import union_str
```

### Comparing `ricco-1.1.0/src/ricco/etl/extract.py` & `ricco-1.1.2/src/ricco/etl/extract.py`

 * *Files identical despite different names*

### Comparing `ricco-1.1.0/src/ricco/etl/file.py` & `ricco-1.1.2/src/ricco/etl/file.py`

 * *Files identical despite different names*

### Comparing `ricco-1.1.0/src/ricco/etl/load.py` & `ricco-1.1.2/src/ricco/etl/load.py`

 * *Files identical despite different names*

### Comparing `ricco-1.1.0/src/ricco/etl/transformer.py` & `ricco-1.1.2/src/ricco/etl/transformer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,58 +1,51 @@
+import warnings
 from datetime import datetime
 
 import pandas as pd
 
-from ..util.geom import wkb_loads
+from ..util.assertion import assert_series_unique
+from ..util.decorator import timer
+from ..util.decorator import progress
+from ..util.util import and_
 from ..util.util import ensure_list
 from ..util.util import fuzz_match
 from ..util.util import list2dict
 from ..util.util import to_float
 
 
-def filter_valid_geom(df: pd.DataFrame,
-                      c_geometry='geometry',
-                      ignore_index=True):
-  """仅保留有效的geometry，剔除空白和错误的geometry行"""
-  if 'temp_xxx' in df.columns:
-    raise KeyError('数据集中不能存在【temp_xxx】列')
-  df['temp_xxx'] = df[c_geometry].apply(wkb_loads)
-  df = df[df['temp_xxx'].notna()]
-  if ignore_index:
-    df = df.reset_index(drop=True)
-  del df['temp_xxx']
-  return df
-
-
 def best_unique(df: pd.DataFrame,
                 key_cols: (list, str),
                 value_cols: (str, list) = None,
                 filter=False,
-                drop_if_null='all'):
+                drop_if_null=None) -> pd.DataFrame:
   """
   优化的去重函数：
     为保证数据的完整性，去重时优先去除指定列中的空值
 
   :param df:
   :param key_cols: 按照哪些列去重
   :param value_cols: 优先去除那些列的空值，该列表是有顺序的
   :param filter:
   :param drop_if_null: 如何处理value_cols内值为空的列；'all'：都为空时删除该列，'any'：任意一列为空时就删除，None：保留空白
   :return:
   """
   key_cols = ensure_list(key_cols)
-  if value_cols is None:
+  if not value_cols:
     value_cols = [i for i in df.columns if i not in key_cols]
-  else:
-    value_cols = ensure_list(value_cols)
-  if drop_if_null is not None:
-    df = df.dropna(subset=value_cols, how=drop_if_null).dropna(subset=key_cols,
-                                                               how='all')
+  value_cols = ensure_list(value_cols)
+  if drop_if_null:
+    df = df.dropna(
+        subset=value_cols,
+        how=drop_if_null
+    ).dropna(
+        subset=key_cols,
+        how='all')
   df = df.sort_values(value_cols, na_position='first')
-  df = df.drop_duplicates(key_cols, keep='last').reset_index(drop=True)
+  df = df.drop_duplicates(key_cols, keep='last', ignore_index=True)
   if filter:
     df = df[key_cols + value_cols]
   return df
 
 
 def table2dict(df: pd.DataFrame,
                key_col: str = None,
@@ -64,21 +57,18 @@
   :param df:
   :param key_col: 生成key的列
   :param value_col: 生成value的列
   :param orient: 生成dict的方式，默认'dict',还有 ‘list’, ‘series’, ‘split’, ‘records’, ‘index’
   :return:
   """
   if (key_col is None) or (value_col is None):
-    cols = list(df.columns).copy()
+    cols = df.columns.tolist()
     key_col = cols[0]
     value_col = cols[1]
-
-  df = df[~df[key_col].isna()]
-  df.set_index(key_col, inplace=True)
-
+  df = df[df[key_col].notna()].set_index(key_col)
   if isinstance(value_col, list):
     df = df[value_col]
     return df.to_dict(orient=orient)
   else:
     df = df[[value_col]]
     return df.to_dict(orient=orient)[value_col]
 
@@ -112,51 +102,46 @@
   series[series <= min_score] = min_score
   return series
 
 
 def update_df(df: pd.DataFrame,
               new_df: pd.DataFrame,
               on: (str, list) = None,
-              mode='update'):
+              overwrite: bool = True,
+              errors: str = 'ignore') -> pd.DataFrame:
   """
   根据某一列更新dataframe里的数据
-
-  :param df: 待升级的
-  :param new_df: 新表
-  :param on: 根据哪一列升级,默认为None，使用index
-  :param mode：处理方式，update：直接更新对应位置的数值，insert：只有对应位置为空时才更新
-  :return:
-  """
-  v1 = len(df)
-  if on is not None:
-    on = ensure_list(on)
-    new_df = new_df.drop_duplicates()
-    if any(new_df[on].duplicated()):
-      raise ValueError('new_df中有重复的索引列对应不同的值，请检查')
-    new_df = df[on].drop_duplicates().merge(new_df, how='inner', on=on)
-    df = df.set_index(on, drop=False)
-    new_df = new_df.set_index(on, drop=False)
-  if mode == 'update':
-    df.update(new_df)
-  elif mode == 'insert':
-    df = df.combine_first(new_df)
+  Args:
+    df: 待升级的数据集
+    new_df: 用于更新的DataFrame
+    on: （可选参数）用于判断更新哪些行的列
+    overwrite : （可选参数）控制如何处理原DataFrame在重叠位置上 **非空** 的值，默认为True
+
+      * True: 默认值；使用 `other` DataFrame中的值覆盖原DataFrame中相应位置的值.
+      * False: 只更新原DataFrame中重叠位置数据为 *空* 的值.
+    errors: （可选参数）控制如何处理两个DataFrame同一位置都有值的行为，默认为'ignore'
+
+      * 'ignore': 默认值；DataFrame类型 df和other在同一个cell位置都是非NA值，
+        使用other中的值替换df中的值。
+      * 'raise': target和other都在同一位置包含非NA数据将抛出ValueError异常（'Data overlaps'）。
+  """
+  if on:
+    df.set_index(on, inplace=True)
+    df.update(new_df.set_index(on), overwrite=overwrite, errors=errors)
+    df.reset_index(inplace=True)
   else:
-    raise ValueError(f'参数{mode}错误,可选参数为 update or insert')
-  df = df.reset_index(drop=True)
-  if on is not None:
-    if v1 != len(df):
-      raise ValueError('update后Dataframe结构发生变化，请检查')
+    df.update(new_df, overwrite=overwrite, errors=errors)
   return df
 
 
 def date_to(series: pd.Series, mode: str = 'first') -> pd.Series:
   """
   将日期转为当月的第一天或最后一天
 
-  :param series: pd.Serise
+  :param series: pd.Series
   :param mode: 'first' or 'last'
   :return:
   """
   from pandas.tseries.offsets import MonthEnd
 
   def trans(x):
     if x is not pd.NaT:
@@ -175,27 +160,29 @@
   else:
     raise ValueError(f"{mode}不是正确的参数，请使用 'first' or 'last'")
   return series.apply(trans)
 
 
 def fuzz_df(df: pd.DataFrame,
             col: str,
-            target_serise: (list, pd.Series)) -> pd.DataFrame:
+            target_series: (list, pd.Series)) -> pd.DataFrame:
   """
   为DataFrame中的某一列，从某个集合中匹配相似度最高的元素
 
   :param df: 输入的dataframe
   :param col: 要匹配的列
-  :param target_serise: 从何处匹配， list/pd.Serise
+  :param target_series: 从何处匹配， list/pd.Series
   :return:
   """
-  df[[f'{col}_target',
-      'normal_score',
-      'partial_score']] = df.apply(lambda x: fuzz_match(x[col], target_serise),
-                                   result_type='expand', axis=1)
+  df[[
+    f'{col}_target', 'normal_score', 'partial_score'
+  ]] = df.apply(
+      lambda x: fuzz_match(x[col], target_series),
+      result_type='expand',
+      axis=1)
   return df
 
 
 def series_to_float(series: pd.Series, rex_method: str = 'mean') -> pd.Series:
   """
   pandas.Series: str --> float
 
@@ -217,30 +204,34 @@
         _cond = _cond & df[c].isna()
       else:
         _cond = _cond & (df[c] == value)
     cond = cond | _cond
   return df[cond]
 
 
+@timer
+@progress
 def expand_dict(df, c_src):
   """展开字典为多列"""
   return pd.concat(
       [
         df.drop(c_src, axis=1),
-        df[c_src].apply(
+        df[c_src].progress_apply(
             lambda x: pd.Series(x, dtype='object')
         ).set_index(df.index)
       ],
       axis=1
   )
 
 
+@progress
+@timer
 def split_list_to_row(df, column):
   """将列表列中列表的元素拆成多行"""
-  df[column] = df[column].apply(list2dict)
+  df[column] = df[column].progress_apply(list2dict)
   return df.drop(columns=column).join(
       expand_dict(
           df[[column]], column
       ).stack(
       ).reset_index(
           level=1, drop=True
       ).rename(column)
@@ -251,7 +242,64 @@
   """将字典转为dataframe"""
   df = pd.DataFrame()
   df[c_key] = data.keys()
   df[c_value] = data.values()
   if as_index:
     df.set_index(c_key, inplace=True)
   return df
+
+
+def is_unique(df: pd.DataFrame, key_cols: (str, list) = None):
+  """判断是否唯一"""
+  warnings.warn(
+      '方法即将停用，请使用"ricco.util.util.is_unique_series"方法替代',
+      DeprecationWarning
+  )
+  if not key_cols:
+    key_cols = df.columns.to_list()
+  key_cols = ensure_list(key_cols)
+  return not df.duplicated(subset=key_cols, keep=False).any()
+
+
+def one_line(df, key_cols, key_value, value_cols):
+  """获取一行重置索引后的数据"""
+  cond = and_(*[df[c] == key_value[c] for c in key_cols])
+  df = df[cond][[*key_cols, *value_cols]]
+  return df.reset_index(drop=True)
+
+
+@timer
+def is_changed(df_old: pd.DataFrame,
+               df_new: pd.DataFrame,
+               key_cols: (str, list) = None,
+               value_cols: (str, list) = None,
+               c_res: str = 'is_changed') -> pd.DataFrame:
+  """判断新旧数据集中的每一条数据是否变化"""
+  # 数据集及参数检验
+  key_cols = ensure_list(key_cols)
+  assert_series_unique(df_new, key_cols)
+  if not value_cols:
+    error_msg = 'Each datasets must have same columns.'
+    assert set(df_new.columns) == set(df_old.columns), error_msg
+    value_cols = [c for c in df_old if c not in key_cols]
+  # 对比
+  # 默认所有的都是更改的
+  df_new = df_new.copy()
+  df_new[c_res] = 'Changed'
+  df_temp = df_old[[*key_cols, *value_cols]].merge(
+      df_new[[*key_cols, *value_cols, c_res]],
+      how='left',
+      on=key_cols)
+  # 合并后为空的为 NotFound
+  df_temp[c_res] = df_temp[c_res].fillna('NotFound')
+
+  # 对比每一个值，如果每一列的每一个值都相同，则认为是没有变化
+  cond = and_(
+      *[
+        (df_temp[f'{c}_x'] == df_temp[f'{c}_y']) |
+        (df_temp[f'{c}_x'].isna() & df_temp[f'{c}_y'].isna())
+        for c in value_cols
+      ]
+  )
+  df_temp.loc[cond, c_res] = 'NotChange'
+  df_temp = df_temp[[*key_cols, c_res]]
+  return df_old.merge(df_temp, how='left', on=key_cols)
```

### Comparing `ricco-1.1.0/src/ricco/geocode/amap.py` & `ricco-1.1.2/src/ricco/geocode/amap.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+import logging
+
 import requests
-from fuzzywuzzy import fuzz
 
 from ..util.util import is_empty
 from .util import MapKeys
 from .util import MapUrls
 from .util import error_amap
 from .util import fix_address
 from .util import gcj2xx
+from .util import rv_score
 
 KEY = MapKeys.amap
 
 
 def address_json(city: str, address: str, key=None):
   """高德地理编码接口"""
   if is_empty(address):
@@ -48,15 +50,19 @@
              key=None):
   """脉策geocode服务"""
   if is_empty(address):
     return None
   url = f'{MapUrls.mdt}?address={address}&city={city}&disable_cache={disable_cache}&with_detail={with_detail}&source={source}'
   req = requests.get(url)
   if req.status_code == 200:
-    return req.json()['result'][0]['extra']
+    try:
+      return req.json()['result'][0]['extra']
+    except Exception as e:
+      logging.warning(f'{e}，{req}')
+      return None
   elif req.status_code in (400, 403):
     if source == 'amap':
       return address_json(city=city, address=address, key=key)
     elif source == 'amap_poi':
       return place_json(city=city, keywords=address, key=key)
     else:
       raise ValueError('source参数错误')
@@ -104,16 +110,15 @@
   res = get_amap(city=city, address=keywords, source='amap_poi', key=key)
   if res:
     rv = res['name']
     lnglat = res['location'].split(',')
     latlng = gcj2xx(lnglat, srs=srs)
     lng = latlng[1]
     lat = latlng[0]
-    score = max(fuzz.ratio(rv, keywords.lstrip(city)),
-                fuzz.partial_ratio(rv, keywords.lstrip(city)))
+    score = rv_score(city, keywords, rv)
   else:
     rv, lng, lat, score = None, None, None, 0
   return {
     'rv': rv,
     'score': score,
     'lng': lng,
     'lat': lat,
```

### Comparing `ricco-1.1.0/src/ricco/geocode/baidu.py` & `ricco-1.1.2/src/ricco/geocode/baidu.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import requests
-from fuzzywuzzy import fuzz
 
 from ..util.util import is_empty
 from .util import MapKeys
 from .util import MapUrls
 from .util import error_baidu
 from .util import fix_address
 from .util import gcj2xx
+from .util import rv_score
 
 KEY = MapKeys.baidu
 
 
 def address_json(city: str, address: str, key=None):
   """百度地理编码接口"""
   if is_empty(address):
@@ -108,16 +108,15 @@
   res = get_baidu(city=city, address=keywords, source='baidu_poi', key=key)
   if res:
     rv = res['name']
     lnglat = [res['location']['lng'], res['location']['lat']]
     latlng = gcj2xx(lnglat, srs=srs)
     lng = latlng[1]
     lat = latlng[0]
-    score = max(fuzz.ratio(rv, keywords.lstrip(city)),
-                fuzz.partial_ratio(rv, keywords.lstrip(city)))
+    score = rv_score(city, keywords, rv)
   else:
     rv, lng, lat, score = None, None, None, 0
   return {
     'rv': rv,
     'score': score,
     'lng': lng,
     'lat': lat,
```

### Comparing `ricco-1.1.0/src/ricco/geocode/geocode.py` & `ricco-1.1.2/src/ricco/geocode/geocode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import uuid
 import warnings
 
 import pandas as pd
 from requests.exceptions import ConnectionError
 from requests.exceptions import ConnectTimeout
 from tqdm import tqdm
@@ -144,31 +145,34 @@
   else:
     raise TypeError(f'city类型错误，请传入list或str类型')
 
   on = [temp_city_col, by]
   df_temp = df[on].drop_duplicates().reset_index(drop=True)
 
   for i in tqdm(df_temp.index):
-    kw = df_temp[by][i]
-    ct = df_temp[temp_city_col][i]
-    if address_type == 'poi':
-      rv = geocode_best_poi(
-          ct, kw,
-          sig=sig,
-          address_geocode=address_geocode,
-          srs=srs,
-          key_baidu=key_baidu,
-          key_amap=key_amap)
-    elif address_type == 'address':
-      rv = geocode_best_address(ct, kw, srs=srs,
-                                key_baidu=key_baidu, key_amap=key_amap)
-    else:
-      raise ValueError('参数address_type错误，可选参数为"poi"或"address"')
-    df_temp.loc[
-      (df_temp[temp_city_col] == ct) & (df_temp[by] == kw),
-      ['lng', 'lat', 'rv', 'geocode_score', 'geocode_type']] = rv
+    try:
+      kw = df_temp[by][i]
+      ct = df_temp[temp_city_col][i]
+      if address_type == 'poi':
+        rv = geocode_best_poi(
+            ct, kw,
+            sig=sig,
+            address_geocode=address_geocode,
+            srs=srs,
+            key_baidu=key_baidu,
+            key_amap=key_amap)
+      elif address_type == 'address':
+        rv = geocode_best_address(ct, kw, srs=srs,
+                                  key_baidu=key_baidu, key_amap=key_amap)
+      else:
+        raise ValueError('参数address_type错误，可选参数为"poi"或"address"')
+      df_temp.loc[
+        (df_temp[temp_city_col] == ct) & (df_temp[by] == kw),
+        ['lng', 'lat', 'rv', 'geocode_score', 'geocode_type']] = rv
+    except Exception as e:
+      logging.warning(f'{e},{kw}')
 
   df = df.merge(df_temp, on=on, how='left')
   if not with_detail:
     del df['rv'], df['geocode_score'], df['geocode_type']
   del df[temp_city_col]
   return df
```

### Comparing `ricco-1.1.0/src/ricco/geocode/util.py` & `ricco-1.1.2/src/ricco/geocode/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -51,7 +51,15 @@
     )
 
 
 def fix_address(string):
   if is_empty(string):
     return ''
   return str(string)
+
+
+def rv_score(city, keywords, rv):
+  from fuzzywuzzy import fuzz
+  return max(
+      fuzz.ratio(rv, keywords.lstrip(city)),
+      fuzz.partial_ratio(rv, keywords.lstrip(city))
+  )
```

### Comparing `ricco-1.1.0/src/ricco/local.py` & `ricco-1.1.2/src/ricco/local.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
   p_huamu_fangwu = '/Users/ricco/Project/collector_api_sdk/huamu/花木市民-房屋基本信息表.csv'
 
   def p_street(self, city):
     return f'/Users/ricco/common_data/bd_region/{city}边界_街镇最新.csv'
 
   def p_region(self, city):
-    return f'/Users/ricco/common_data/bd_region/{city}边界_街镇最新.csv'
+    return f'/Users/ricco/common_data/bd_region/{city}边界_区县最新.csv'
 
 
 class Datas(Dirs):
   def street(self, city='上海'):
     return rdf(self.p_street(city))
 
   def region(self, city='上海'):
```

### Comparing `ricco-1.1.0/src/ricco/resource/area_code.py` & `ricco-1.1.2/src/ricco/resource/area_code.py`

 * *Files identical despite different names*

### Comparing `ricco-1.1.0/src/ricco/resource/city_id.py` & `ricco-1.1.2/src/ricco/resource/city_id.py`

 * *Files identical despite different names*

### Comparing `ricco-1.1.0/src/ricco/resource/epsg_code.py` & `ricco-1.1.2/src/ricco/resource/epsg_code.py`

 * *Files identical despite different names*

### Comparing `ricco-1.1.0/src/ricco/resource/names.py` & `ricco-1.1.2/src/ricco/resource/names.py`

 * *Files identical despite different names*

### Comparing `ricco-1.1.0/src/ricco/resource/phone_number.py` & `ricco-1.1.2/src/ricco/resource/phone_number.py`

 * *Files identical despite different names*

### Comparing `ricco-1.1.0/src/ricco/util/address_tools.py` & `ricco-1.1.2/src/ricco/util/address_tools.py`

 * *Files identical despite different names*

### Comparing `ricco-1.1.0/src/ricco/util/building_address.py` & `ricco-1.1.2/src/ricco/util/building_address.py`

 * *Files identical despite different names*

### Comparing `ricco-1.1.0/src/ricco/util/coord_trans.py` & `ricco-1.1.2/src/ricco/util/coord_trans.py`

 * *Files identical despite different names*

### Comparing `ricco-1.1.0/src/ricco/util/geom.py` & `ricco-1.1.2/src/ricco/util/geom.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,39 @@
 import json
 import logging
 import warnings
+from typing import List
+from typing import Union
 
 import geojson
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 from shapely import wkb
 from shapely import wkt
 from shapely.errors import GeometryTypeError
 from shapely.errors import ShapelyDeprecationWarning
 from shapely.errors import WKBReadingError
-from shapely.geometry import LinearRing
-from shapely.geometry import LineString
 from shapely.geometry import MultiLineString
-from shapely.geometry import MultiPoint
 from shapely.geometry import MultiPolygon
 from shapely.geometry import Point
 from shapely.geometry import Polygon
 from shapely.geometry import shape
 from shapely.geos import WKTReadingError
 from simplejson.errors import JSONDecodeError
+from tqdm import tqdm
 
 from ..util.util import ensure_list
 from ..util.util import first_notnull_value
+from ..util.util import is_empty
+from ..util.util import not_empty
+from .decorator import geom_progress
 
 warnings.filterwarnings('ignore', category=ShapelyDeprecationWarning)
 
-GeomTypeSet = (
-  Point, MultiPoint,
-  Polygon, MultiPolygon,
-  LineString, MultiLineString,
-  LinearRing
-)
-
 
 class GeomFormat:
   wkb = 'wkb'
   wkt = 'wkt'
   shapely = 'shapely'
   geojson = 'geojson'
   unknown = 'unknown'
@@ -103,109 +99,122 @@
 
 
 def wkb_loads(x, hex=True):
   warnings.filterwarnings('ignore',
                           'Geometry column does not contain geometry.',
                           UserWarning)
 
-  if pd.isna(x):
-    return None
+  if is_empty(x):
+    return
 
   try:
     return wkb.loads(x, hex=hex)
-  except (AttributeError, WKBReadingError):
-    return None
+  except (AttributeError, WKBReadingError) as e:
+    warnings.warn(f'{e}, 【{x}】')
+    return
 
 
 def wkb_dumps(x, hex=True, srid=4326) -> (str, None):
-  if pd.isna(x):
-    return None
+  if is_empty(x):
+    return
 
   try:
     return wkb.dumps(x, hex=hex, srid=srid)
-  except AttributeError:
-    return None
+  except AttributeError as e:
+    warnings.warn(f'{e}, 【{x}】')
+    return
 
 
 def wkt_loads(x):
-  if pd.isna(x):
-    return None
+  if is_empty(x):
+    return
   try:
     return wkt.loads(x)
-  except (AttributeError, WKTReadingError):
-    return None
+  except (AttributeError, WKTReadingError, TypeError) as e:
+    warnings.warn(f'{e}, 【{x}】')
+    return
 
 
 def wkt_dumps(x) -> (str, None):
-  if pd.isna(x):
-    return None
+  if is_empty(x):
+    return
   try:
     return wkt.dumps(x)
-  except AttributeError:
-    return None
+  except AttributeError as e:
+    warnings.warn(f'{e}, 【{x}】')
+    return
 
 
 def geojson_loads(x):
   """geojson文本形式转为shapely格式"""
-  if pd.isna(x):
-    return None
+  if is_empty(x):
+    return
   try:
     geom = shape(geojson.loads(x))
     if geom.is_empty:
-      return None
+      return
     return geom
-  except (JSONDecodeError, AttributeError, GeometryTypeError, TypeError):
-    return None
+  except (JSONDecodeError, AttributeError, GeometryTypeError, TypeError) as e:
+    warnings.warn(f'{e}, 【{x}】')
+    return
 
 
 def geojson_dumps(x) -> (str, None):
   """shapely转为geojson文本格式"""
-  if pd.isna(x):
-    return None
+  if is_empty(x):
+    return
   try:
     geom = geojson.Feature(geometry=x)
     return json.dumps(geom.geometry)
-  except TypeError:
-    return None
+  except TypeError as e:
+    warnings.warn(f'{e}, 【{x}】')
+    return
 
 
 def is_shapely(x, na=False) -> bool:
   """判断是否为shapely格式"""
+  from ..resource.geometry import GeomTypeSet
   if pd.isna(x):
     return na
   if type(x) in GeomTypeSet:
     return True
   else:
     return False
 
 
 def is_wkb(x, na=False) -> bool:
   """判断是否为wkb格式"""
+  if not isinstance(x, str):
+    return False
   if pd.isna(x):
     return na
   try:
     wkb.loads(x, hex=True)
     return True
   except WKBReadingError:
     return False
 
 
 def is_wkt(x, na=False) -> bool:
   """判断是否为wkt格式"""
+  if not isinstance(x, str):
+    return False
   if pd.isna(x):
     return na
   try:
     wkt.loads(x)
     return True
   except WKTReadingError:
     return False
 
 
 def is_geojson(x, na=False) -> bool:
   """判断是否为geojson格式"""
+  if not isinstance(x, (str, dict)):
+    return False
   if pd.isna(x):
     return na
   try:
     if shape(geojson.loads(x)).is_empty:
       return False
     return True
   except (JSONDecodeError, AttributeError, GeometryTypeError, TypeError):
@@ -244,102 +253,166 @@
       lng, lat = lngs[i], lats[i]
       point = Point((lng, lat))
       if len(coords) >= 1:
         if point != coords[-1]:
           coords.append(point)
       else:
         coords.append(point)
-  return MultiPolygon([Polygon(coords)])
-
-
-def geom_wkt2shapely(df, geometry='geometry',
-                     epsg_code: int = 4326) -> gpd.GeoDataFrame:
-  """wkt转gpd"""
-  df[geometry] = df[geometry].apply(wkt_loads)
-  return gpd.GeoDataFrame(df, geometry=geometry, crs=epsg_code)
-
-
-def geom_wkb2lnglat(df, geometry='geometry', delete=False, within=False):
-  """geometry转经纬度，求中心点经纬度"""
-  df = geom_wkb2shapely(df, geometry=geometry)
-  df = geom_shapely2lnglat(df, geometry=geometry, within=within, delete=delete)
-  if not delete:
-    df[geometry] = df[geometry].apply(wkb_dumps)
-  return df
+  try:
+    return MultiPolygon([Polygon(coords)])
+  except ValueError as e:
+    warnings.warn(f'{e}，{multiline_shapely}')
+    return
 
 
 def get_inner_point(polygon: Polygon, within=True):
   """返回面内的一个点，默认返回中心点，当中心点不在面内则返回面内一个点"""
-  if pd.isna(polygon):
-    return None
+  if is_empty(polygon):
+    return
   point = polygon.centroid
-  if polygon.contains(point):
+  if not polygon.is_valid:
+    polygon = polygon.buffer(0.000001)
+  if polygon.contains(point) or not within:
     return point
-  else:
-    if within:
-      return polygon.representative_point()
-    else:
-      return point
+  return polygon.representative_point()
 
 
-def geom_wkt2wkb(df, geometry='geometry', epsg_code: int = 4326):
-  """wkb转wkt"""
-  df = geom_wkt2shapely(df, geometry=geometry, epsg_code=epsg_code)
-  df[geometry] = df[geometry].apply(wkb_dumps)
+@geom_progress
+def geom_wkb2shapely(df, geometry='geometry',
+                     epsg_code: int = 4326) -> gpd.GeoDataFrame:
+  df = df.copy()
+  df[geometry] = df[geometry].progress_apply(wkb_loads)
+  return gpd.GeoDataFrame(df, geometry=geometry, crs=epsg_code)
+
+
+@geom_progress
+def geom_shapely2wkb(df, geometry='geometry'):
+  df[geometry] = df[geometry].progress_apply(wkb_dumps)
   return df
 
 
-def geom_wkb2shapely(df, geometry='geometry',
+@geom_progress
+def geom_wkt2shapely(df, geometry='geometry',
                      epsg_code: int = 4326) -> gpd.GeoDataFrame:
-  """wkb直接转Dataframe"""
-  df = df.copy()
-  df[geometry] = df[geometry].apply(wkb_loads)
+  df[geometry] = df[geometry].progress_apply(wkt_loads)
   return gpd.GeoDataFrame(df, geometry=geometry, crs=epsg_code)
 
 
-def geom_lnglat2shapely(df, lng='lng', lat='lat', delete=True,
+@geom_progress
+def geom_shapely2wkt(df, geometry='geometry'):
+  df[geometry] = df[geometry].progress_apply(wkt_dumps)
+  return df
+
+
+@geom_progress
+def geom_lnglat2shapely(df,
+                        lng='lng',
+                        lat='lat',
+                        geometry='geometry',
+                        delete=True,
                         epsg_code: int = 4326) -> gpd.GeoDataFrame:
-  """包含经纬度的DataFrame转GeoDataFrame"""
   from pandas.errors import SettingWithCopyWarning
   warnings.filterwarnings('ignore', category=SettingWithCopyWarning)
-  df['geometry'] = df.apply(
-      lambda d: Point((d[lng], d[lat])) if all([d[lng], d[lat]]) else None,
+
+  df[geometry] = df.progress_apply(
+      lambda d: Point((d[lng], d[lat]))
+      if not_empty(d[lng]) and not_empty(d[lat])
+      else None,
       axis=1
   )
   df = gpd.GeoDataFrame(df, crs=epsg_code)
   if delete:
     del df[lng], df[lat]
   return df
 
 
-def geom_shapely2lnglat(df, geometry='geometry', within=False, delete=False):
+@geom_progress
+def geom_shapely2lnglat(df, geometry='geometry',
+                        lng='lng', lat='lat',
+                        within=False, delete=False):
   """
   shapely格式提取中心点转为经纬度。
   within: 范围的点是否再面内，默认False，直接返回中心点；
   当为True时，不在面内的中心点将用一个在面内的点代替
   """
-  df['geometry_temp'] = df[geometry].apply(
-      lambda x: get_inner_point(x, within=within) if x else None)
-  df['lng'] = df['geometry_temp'].centroid.x
-  df['lat'] = df['geometry_temp'].centroid.y
-  del df['geometry_temp']
+
+  def get_xy(x):
+    p = get_inner_point(x, within=within)
+    return p.centroid.x, p.centroid.y
+
+  df[[lng, lat]] = df[[geometry]].progress_apply(
+      lambda r: get_xy(r[geometry]) if r[geometry] else (None, None),
+      result_type='expand',
+      axis=1
+  )
   if delete:
     del df[geometry]
   return df
 
 
-def geom_lnglat2wkb(df, lng='lng', lat='lat', delete=False, code=4326):
+def geom_wkb2lnglat(df, geometry='geometry', delete=False, within=False):
+  """geometry转经纬度，求中心点经纬度"""
+  df = geom_wkb2shapely(df, geometry=geometry)
+  df = geom_shapely2lnglat(df, geometry=geometry, within=within, delete=delete)
+  if not delete:
+    df = geom_shapely2wkb(df, geometry=geometry)
+  return df
+
+
+def geom_lnglat2wkb(df,
+                    lng='lng',
+                    lat='lat',
+                    geometry='geometry',
+                    delete=False, code=4326):
   """经纬度转wkb格式的geometry"""
-  df = geom_lnglat2shapely(df, 'lng', 'lat', delete=delete, epsg_code=code)
-  df['geometry'] = df['geometry'].apply(wkb_dumps)
+  df = geom_lnglat2shapely(
+      df, 'lng', 'lat', geometry=geometry, delete=delete, epsg_code=code
+  )
+  df = geom_shapely2wkb(df, geometry=geometry)
   if not delete:
     df = df.rename(columns={'lng': lng, 'lat': lat})
   return df
 
 
+def geom_wkt2lnglat(df, geometry='geometry', delete=False, within=False):
+  """geometry转经纬度，求中心点经纬度"""
+  df = geom_wkt2shapely(df, geometry=geometry)
+  df = geom_shapely2lnglat(df, geometry=geometry, within=within, delete=delete)
+  if not delete:
+    df = geom_shapely2wkt(df, geometry=geometry)
+  return df
+
+
+def geom_lnglat2wkt(df,
+                    lng='lng',
+                    lat='lat',
+                    geometry='geometry',
+                    delete=False, code=4326):
+  """经纬度转wkb格式的geometry"""
+  df = geom_lnglat2shapely(
+      df, 'lng', 'lat', geometry=geometry, delete=delete, epsg_code=code
+  )
+  df = geom_shapely2wkt(df, geometry=geometry)
+  if not delete:
+    df = df.rename(columns={'lng': lng, 'lat': lat})
+  return df
+
+
+def geom_wkb2wkt(df, geometry='geometry', epsg_code: int = 4326):
+  """wkb转wkt"""
+  df = geom_wkb2shapely(df, geometry=geometry, epsg_code=epsg_code)
+  return geom_shapely2wkt(df, geometry=geometry)
+
+
+def geom_wkt2wkb(df, geometry='geometry', epsg_code: int = 4326):
+  """wkb转wkt"""
+  df = geom_wkt2shapely(df, geometry=geometry, epsg_code=epsg_code)
+  return geom_shapely2wkb(df, geometry=geometry)
+
+
 def geom_split_grids(df: gpd.GeoDataFrame, step: int, city: str = None):
   """
   根据所给边界划分固定边长的栅格
 
   Args:
       df: 边界文件，GeoDataFrame格式
       step: 栅格边长，单位：米
@@ -408,15 +481,16 @@
   df_temp = pd.DataFrame({'i': i_l, 'j': j_l, 'lng': lng_l, 'lat': lat_l})
   # 删除末尾的格子，避免后面出现out of range
   df_res = df_temp.loc[
     (df_temp['i'] != x_num - 1) & (df_temp['j'] != y_num - 1),
     ['i', 'j']].reset_index(drop=True)
 
   # 组合坐标集并转为Polygon
-  df_res['geometry'] = df_res.apply(
+  tqdm.pandas(desc='lnglat2shapely')
+  df_res['geometry'] = df_res.progress_apply(
       lambda df: get_lnglat_sets(df_temp, df['i'], df['j']), axis=1)
 
   # 生成grid_id列
   df_res['grid_id'] = df_res['i'].astype(str) + '-' + df_res['j'].astype(str)
   del df_res['i'], df_res['j']
 
   # 通过边界裁剪栅格
@@ -424,15 +498,16 @@
   df.crs = 'epsg:4326'
   df_res = gpd.sjoin(df_res,
                      df,
                      how='inner',
                      predicate='intersects').drop('index_right', axis=1)
 
   # 将geometry转为wkb格式
-  df_res['geometry'] = df_res['geometry'].apply(wkb_dumps)
+  tqdm.pandas(desc='shapely2wkb')
+  df_res['geometry'] = df_res['geometry'].progress_apply(wkb_dumps)
   return df_res
 
 
 def ensure_gdf(df, geometry='geometry'):
   geom = first_notnull_value(df[geometry])
   geom_format = infer_geom_format(geom)
   if geom_format == 'wkb':
@@ -447,45 +522,48 @@
 
 def mark_tags_v2(
     point_df: pd.DataFrame,
     polygon_df: pd.DataFrame,
     col_list: list = None,
     predicate='intersects',
     drop_geometry=False,
-    geometry_format='wkb'):
+    geometry_format='wkb',
+    warning_message=True):
   """
   使用面数据通过空间关联（sjoin）给点数据打标签
 
   Args:
       point_df: 点数据
       polygon_df: 面数据
       col_list: 面数据中要关联到结果中的列，若为空则全部关联
       predicate: 关联方法，默认'intersects'
       drop_geometry: 结果是否删除geometry，默认删除
       geometry_format: 输出的geometry格式，支持wkb,、wkt、shapely，默认wkb
   """
   if not col_list:
     col_list = polygon_df.columns.to_list()
   else:
-    polygon_df = polygon_df[col_list + ['geometry']]
+    col_list = ensure_list(col_list)
+    polygon_df = polygon_df[[*col_list, 'geometry']]
 
-  col_list = ensure_list(col_list)
   for c in col_list:
     if c in point_df and c not in ['lng', 'lat', 'geometry']:
       c_n = f'{c}_origin'
-      warnings.warn(f'点数据中存在面文件中待关联的列，已重命名：{c} --> {c_n}')
+      if warning_message:
+        warnings.warn(f'点数据中存在面文件中待关联的列，已重命名：{c} --> {c_n}')
       point_df.rename(columns={c: c_n}, inplace=True)
 
   if 'geometry' in point_df:
     point_df = ensure_gdf(point_df)
     geom = first_notnull_value(point_df['geometry'])
     if geom.geom_type not in ['point', 'Point']:
-      warnings.warn('左侧数据实际非点数据，将自动提取中心点进行关联')
+      if warning_message:
+        warnings.warn('左侧数据实际非点数据，将自动提取中心点进行关联')
       point_df['geometry_backup'] = point_df['geometry']
-      point_df = geom_shapely2lnglat(point_df)
+      point_df = geom_shapely2lnglat(point_df, within=True)
       point_df = geom_lnglat2shapely(point_df, delete=False)
   elif 'lng' in point_df and 'lat' in point_df:
     point_df = geom_lnglat2shapely(point_df, delete=False)
   else:
     raise KeyError('点文件中必须有经纬度或geometry')
 
   polygon_df = ensure_gdf(polygon_df)
@@ -501,17 +579,17 @@
     del point_df['geometry']
     point_df.rename(columns={'geometry_backup': 'geometry'}, inplace=True)
 
   if drop_geometry:
     del point_df['geometry']
   else:
     if geometry_format == 'wkb':
-      point_df['geometry'] = point_df['geometry'].apply(wkb_dumps)
+      point_df = geom_shapely2wkb(point_df)
     elif geometry_format == 'wkt':
-      point_df['geometry'] = point_df['geometry'].apply(wkt_dumps)
+      point_df = geom_shapely2wkt(point_df)
     elif geometry_format == 'shapely':
       pass
     else:
       raise ValueError('不支持的geometry格式')
 
   return pd.DataFrame(point_df)
 
@@ -552,7 +630,117 @@
   """
   p1, p2 = ensure_lnglat(p1), ensure_lnglat(p2)
   if not epsg_to:
     epsg_to = get_epsg(city) if city else get_epsg_by_lng([p1[0], p2[0]])
   p1 = projection_lnglat(p1, epsg_from, epsg_to)
   p2 = projection_lnglat(p2, epsg_from, epsg_to)
   return Point(p1).distance(Point(p2))
+
+
+def buffer(df: pd.DataFrame, radius: Union[int, float],
+           city: str = None,
+           geo_type: str = 'point',
+           geometry: str = 'geometry',
+           buffer_geometry: str = 'buffer_geometry',
+           geo_format='wkb') -> pd.DataFrame:
+  """
+  获得一定半径的缓冲区
+
+  Args:
+    df: pd.DataFrame, 包含地理信息的DataFrame
+    radius: numeric, 缓冲区半径（单位米）
+    city: str, 可选, 投影城市，可提高数据精度
+    geo_type: str, 地理数据类型，可选point, line或polygon(包括multipolygon)，默认point
+    geometry: str, geometry字段名，默认"geometry"
+    buffer_geometry: 输出的缓冲区geometry字段名，默认"buffer_geometry"
+    geo_format: str, 输出的缓冲区geometry格式，支持"wkb","wkt","shapely"，默认"wkb"
+
+  Returns: 包含缓冲区geometry的DataFrame
+
+  Examples:
+    >>> df = pd.DataFrame({'id': [1, 2, 3],
+    >>>                    'lng': [116.18601, 116.18366, 116.18529],
+    >>>                    'lat': [40.02894, 40.03550, 40.03565]})
+
+    >>> df
+        id        lng       lat
+    0   1  116.18601  40.02894
+    1   2  116.18366  40.03550
+    2   3  116.18529  40.03565
+
+    >>> buffer(df=df, radius=1500, city='北京', geo_type='point')
+        id        lng       lat                                    buffer_geometry
+    0   1  116.18601  40.02894  0103000020E6100000010000004100000092A0207A070D...
+    1   2  116.18366  40.03550  0103000020E6100000010000004100000071178800E10C...
+    2   3  116.18529  40.03565  0103000020E610000001000000410000008A2570B5FB0C...
+
+  """
+  df = df.reset_index(drop=True)
+  cols = []
+  if geometry in df:
+    cols.append(geometry)
+  if 'lng' in df and 'lat' in df:
+    cols.extend(['lng', 'lat'])
+  df_tmp = df[cols]
+  df_tmp.rename(columns={geometry: 'geometry'}, inplace=True)
+
+  if geo_type == 'point':
+    if 'geometry' in df_tmp:
+      df_tmp = ensure_gdf(df_tmp)
+      geom = first_notnull_value(df_tmp['geometry'])
+      if geom.geom_type not in ['point', 'Point']:
+        warnings.warn('数据实际非点数据，将自动提取中心点进行关联')
+        df_tmp = geom_shapely2lnglat(df_tmp)
+        df_tmp = geom_lnglat2shapely(df_tmp, delete=False)
+    elif 'lng' in df_tmp and 'lat' in df_tmp:
+      df_tmp = geom_lnglat2shapely(df_tmp, delete=False)
+
+    else:
+      raise KeyError('点文件中必须有经纬度或geometry')
+  elif geo_type == 'line' or geo_type == 'polygon':
+    df_tmp = ensure_gdf(df_tmp, geometry=geometry)
+  else:
+    raise ValueError('geo_type必须为point，line或polygon')
+  df_buffer = df_tmp[['geometry']]
+
+  df_buffer = projection(df_buffer, city=city)
+  df_buffer['geometry'] = df_buffer.geometry.buffer(radius)
+  df_buffer = projection(df_buffer, epsg=4326)
+  if geo_format == 'wkb':
+    tqdm.pandas(desc='shapely2wkb')
+    df_buffer['geometry'] = df_buffer['geometry'].progress_apply(wkb_dumps)
+  elif geo_format == 'wkt':
+    tqdm.pandas(desc='shapely2wkt')
+    df_buffer['geometry'] = df_buffer['geometry'].progress_apply(wkt_dumps)
+  elif geo_format == 'shapely':
+    pass
+  else:
+    raise ValueError('不支持的geometry格式')
+  df_buffer.rename(columns={'geometry': buffer_geometry}, inplace=True)
+  df = df.join(df_buffer, how='left')
+
+  return df
+
+
+def spatial_agg(point_df: pd.DataFrame, polygon_df: pd.DataFrame,
+                by: Union[str, List[str]],
+                agg: dict,
+                polygon_geometry: str = 'geometry') -> pd.DataFrame:
+  """
+  对面数据覆盖范围内的点数据进行空间统计
+  Args:
+    point_df: pd.DataFrame, 点数据dataframe;
+    polygon_df: pd.DataFrame, 面数据dataframe;
+    by: Union[str, List[str]], 空间统计单位字段；
+    agg: dict, 空间统计操作。格式为{'被统计字段名': '操作名', ...}的字典。如{'poi':'sum'};
+    polygon_geometry: str, 面数据geometry字段名，默认"geometry";
+
+  Returns: pd.DataFrame, 包含空间统计单位字段和被统计字段和面数据geometry的DataFrame
+  """
+
+  polygon_df.rename({polygon_geometry: 'geometry'}, inplace=True)
+  polygon_df = polygon_df[[by, 'geometry']]
+  point_df = mark_tags_v2(polygon_df=polygon_df, point_df=point_df,
+                          drop_geometry=True)
+  df_grouped = point_df.groupby(by=by, as_index=False).agg(agg)
+
+  return df_grouped
```

### Comparing `ricco-1.1.0/src/ricco/util/id_number.py` & `ricco-1.1.2/src/ricco/util/id_number.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,27 +5,18 @@
 import pandas as pd
 
 from ..resource.patterns import Pattern
 from .util import all_year_old
 from .util import random_date
 
 
-def get_check_code(id_number):
+def get_check_code(id_number) -> str:
   mapping = {
-    0: '1',
-    1: '0',
-    2: 'X',
-    3: '9',
-    4: '8',
-    5: '7',
-    6: '6',
-    7: '5',
-    8: '4',
-    9: '3',
-    10: '2',
+    0: '1', 1: '0', 2: 'X', 3: '9', 4: '8',
+    5: '7', 6: '6', 7: '5', 8: '4', 9: '3', 10: '2',
   }
   weight = [7, 9, 10, 5, 8, 4, 2, 1, 6, 3, 7, 9, 10, 5, 8, 4, 2]
   ils = [int(i) for i in id_number[:17]]
   return mapping.get(sum(np.multiply(weight, ils)) % 11)
 
 
 class IDNumber:
@@ -35,37 +26,40 @@
     self.__gender = self.id_number[-2]
 
   @property
   def value(self):
     return self.id_number
 
   @staticmethod
-  def is_valid(id_number) -> bool:
+  def is_valid(id_number, check_code=False) -> bool:
     """判断身份证号是否有效"""
     string = str(id_number)
     if re.match(Pattern.ID_number, string):
+      if check_code:
+        if get_check_code(string) != string[-1]:
+          return False
       return True
     return False
 
   @staticmethod
-  def not_valid(id_number) -> bool:
+  def not_valid(id_number, check_code=False) -> bool:
     """判断身份证号是否无效"""
-    string = str(id_number)
-    if not re.match(Pattern.ID_number, string):
-      return True
-    return False
+    return not IDNumber.is_valid(id_number, check_code == check_code)
 
   def format_id_number(self, id_number) -> str:
     """对身份证号进行校验并转为字符串格式"""
     if isinstance(id_number, (float, int)):
       id_number = str(int(id_number))
     if self.is_valid(id_number):
       return id_number
-    else:
-      raise ValueError('身份证号格式错误')
+    raise ValueError('身份证号格式错误')
+
+  @property
+  def check_code(self):
+    return get_check_code(self.id_number)
 
   @property
   def birthdate(self):
     """出生日期"""
     return pd.to_datetime(self.__birthday, format='%Y%m%d')
 
   def birthday(self, format: str = '%Y-%m-%d') -> str:
```

### Comparing `ricco-1.1.0/src/ricco/util/os.py` & `ricco-1.1.2/src/ricco/util/os.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import datetime
 import logging
 import os
 import zipfile
+from .util import ensure_list
 
 
 def ext(filepath):
   """扩展名"""
   return os.path.splitext(filepath)[1]
 
 
@@ -92,7 +93,30 @@
   for dirpath, dirnames, filenames in os.walk(dir_path):
     for dirname in dirnames:
       dir_full_path = os.path.join(dirpath, dirname)
       num = get_file_counts(dir_full_path)
       if num == 0:
         remove_dir(dir_full_path)
         logging.warning(f'已删除空文件夹：{dir_full_path}')
+
+
+def dir_iter(root, exts: (list, str) = None, abspath=False):
+  """
+  文件夹中的文件路径生成器，用于遍历文件夹中的文件
+  Args:
+    root: 文件目录
+    exts: 文件扩展名，不指定则返回所有文件
+
+  Returns:
+
+  """
+
+  for filename in os.listdir(root):
+    filepath = os.path.join(root, filename)
+    if abspath:
+      filepath = os.path.abspath(filepath)
+    if exts:
+      exts = ensure_list(exts)
+      if ext(filepath) in exts:
+        yield filepath
+    else:
+      yield filepath
```

### Comparing `ricco-1.1.0/src/ricco/util/phone_number.py` & `ricco-1.1.2/src/ricco/util/phone_number.py`

 * *Files identical despite different names*

### Comparing `ricco-1.1.0/src/ricco/util/strings.py` & `ricco-1.1.2/src/ricco/util/strings.py`

 * *Files identical despite different names*

### Comparing `ricco-1.1.0/src/ricco/util/util.py` & `ricco-1.1.2/src/ricco/util/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import uuid
 import warnings
 from ast import literal_eval
 
 import numpy as np
 import pandas as pd
 
+from ..resource.geometry import GeomTypeSet
 from ..resource.names import FirstName
 from ..resource.names import LastName
 from ..resource.patterns import Pattern
 
 
 def ensure_list(val):
   """将标量值和Collection类型都统一转换为LIST类型"""
@@ -48,15 +49,15 @@
   """
   校验一个字符串是否为正确的身份证号
 
   :param string: 要传入的字符串
   :param na: 空值返回True还是False，默认为False
   :return:
   """
-  if pd.isna(string):
+  if is_empty(string):
     return na
 
   if not isinstance(string, str):
     string = str(string)
   if len(string) != 18:
     return False
   if re.match(Pattern.ID_number, string):
@@ -73,15 +74,15 @@
   return re.sub(f'{kwd}$', '', string)
 
 
 def get_shortest_element(elements: list):
   """获取列表中长度最短的元素"""
 
   def condition(string):
-    if pd.isna(string):
+    if is_empty(string):
       return np.inf
     string = str(string)
     return len(string)
 
   return min(elements, key=condition)
 
 
@@ -118,15 +119,15 @@
     return now.year - birthday.year
   else:
     return now.year - birthday.year - 1
 
 
 def first_notnull_value(series):
   for v in series:
-    if pd.notna(v):
+    if pd.notna(v) or not v.is_empty:
       return v
   warnings.warn('所有值均为空值')
   return None
 
 
 def pinyin(word: str) -> str:
   """将中文转换为汉语拼音"""
@@ -147,15 +148,15 @@
   except ValueError:
     return False
   return str(uuid_obj) == uuid_to_test
 
 
 def get_uuid(s):
   """针对格式错误的uuid和空白值生成新的uuid"""
-  if pd.isna(s):
+  if is_empty(s):
     return uuid.uuid4()
   elif not is_valid_uuid(s):
     return uuid.uuid4()
   else:
     return s
 
 
@@ -350,19 +351,26 @@
     k: v
     for k, v in dic.items()
     if not_empty(v)
   }
 
 
 def is_empty(x) -> bool:
-  """判断是否为空值"""
+  """
+  判断是否为空值，以下值认为是空白
+    - 空白列表、字典, 如：[], {}，
+    - 空白Dataframe、series, 如：pd.DataFrame()
+    - 空白shapely格式的geometry，如：Point(np.nan, np.nan)
+  """
   if isinstance(x, (list, dict, tuple)):
     return False if x else True
   if isinstance(x, (pd.DataFrame, pd.Series)):
     return x.empty
+  if isinstance(x, GeomTypeSet):
+    return x.is_empty
   return pd.isna(x)
 
 
 def not_empty(x) -> bool:
   """判断是否非空"""
   return not is_empty(x)
 
@@ -398,18 +406,19 @@
   if is_empty(x):
     return {}
   return {i: j for i, j in enumerate(x)}
 
 
 def re_fast(pattern, string, warning=True):
   """根据正则表达式快速提取匹配到的第一个"""
-  if ls := re.findall(pattern, string):
-    if warning and len(ls) >= 2:
-      warnings.warn('匹配到多个值，默认返回第一个')
-    return ls[0]
+  if isinstance(string, str):
+    if ls := re.findall(pattern, string):
+      if warning and len(ls) >= 2:
+        warnings.warn('匹配到多个值，默认返回第一个')
+      return ls[0]
 
 
 def random_name():
   """随机生成中文名字，仅生成2或3字名字"""
   c = [random.choice(FirstName)]
   l = random.randint(1, 2)
   for i in range(l):
@@ -444,12 +453,87 @@
       p=np.array(list(mapping.values())).ravel()
   )
 
 
 def to_int_str(x):
   if is_empty(x):
     return
-  else:
-    try:
-      return str(int(float(x)))
-    except ValueError:
-      return str(x)
+  try:
+    return str(int(float(x)))
+  except ValueError:
+    return str(x)
+
+
+def fix_empty_str(x: str) -> (str, None):
+  """将字符串两端的空格及换行符删除，如果为空白字符串则返回空值"""
+  if isinstance(x, str):
+    x = x.strip()
+    if x == '':
+      return None
+  return x
+
+
+def fix_str(x: str) -> (str, None):
+  """将字符串两端的空格及换行符删除，如果为空白字符串则返回空值"""
+  return fix_empty_str(x)
+
+
+def interchange_dict(dic: dict) -> dict:
+  """将字典的key和value互换"""
+  return dict((v, k) for k, v in dic.items())
+
+
+def to_bool(x,
+            na: bool = False,
+            other: (bool, str) = False,
+            t_list: list = None,
+            f_list: list = None):
+  """
+  将常见的布尔类型的代替值转为布尔类型
+  Args:
+    x: 输入值
+    na: 空值返回真还是假
+    other: 无法判断的值如何处理
+      - 'raise'：抛出异常
+      - 'coerce'：返回传入的值
+      - 除'raise'和'coerce'之外的其他值：直接返回该值
+    t_list:指定为True的类别
+    f_list:指定为False的类别
+  """
+  if not t_list:
+    t_list = ['是', 1, 1.0, '1', '1.0', 't', 'true']
+  if not f_list:
+    f_list = ['否', 0, '0', 'f', 'false']
+
+  if is_empty(x):
+    return na
+  if isinstance(x, bool):
+    return x
+
+  x2 = x.lower() if isinstance(x, str) else x
+  if x2 in t_list:
+    return True
+  if x2 in f_list:
+    return False
+  if other == 'raise':
+    raise ValueError(f'无法转换的值：{x}')
+  if other == 'coerce':
+    return x
+  return other
+
+
+def is_unique_series(df: pd.DataFrame, key_cols: (str, list) = None):
+  """判断是否唯一"""
+  if not key_cols:
+    key_cols = df.columns.tolist()
+  key_cols = ensure_list(key_cols)
+  return not df.duplicated(subset=key_cols, keep=False).any()
+
+
+def is_digit(x):
+  if isinstance(x, bool):
+    return False
+  try:
+    int(float(x))
+    return True
+  except (ValueError, TypeError):
+    return False
```

### Comparing `ricco-1.1.0/src/ricco.egg-info/PKG-INFO` & `ricco-1.1.2/src/ricco.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ricco
-Version: 1.1.0
+Version: 1.1.2
 Summary: A handy ETL&GEOM kit
 Home-page: https://github.com/Ricco1010/ricco
 Author: Ricco Wang
 Author-email: wyk_0610@163.com
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ricco-1.1.0/src/ricco.egg-info/SOURCES.txt` & `ricco-1.1.2/src/ricco.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -7,32 +7,38 @@
 src/ricco.egg-info/dependency_links.txt
 src/ricco.egg-info/requires.txt
 src/ricco.egg-info/top_level.txt
 src/ricco/etl/__init__.py
 src/ricco/etl/extract.py
 src/ricco/etl/file.py
 src/ricco/etl/load.py
+src/ricco/etl/stat.py
 src/ricco/etl/transformer.py
 src/ricco/geocode/__init__.py
 src/ricco/geocode/amap.py
 src/ricco/geocode/baidu.py
 src/ricco/geocode/geocode.py
 src/ricco/geocode/util.py
 src/ricco/resource/__init__.py
 src/ricco/resource/area_code.py
 src/ricco/resource/city_id.py
 src/ricco/resource/crs.py
 src/ricco/resource/epsg_code.py
+src/ricco/resource/geometry.py
 src/ricco/resource/names.py
 src/ricco/resource/patterns.py
 src/ricco/resource/phone_number.py
 src/ricco/util/__init__.py
 src/ricco/util/address_tools.py
+src/ricco/util/assertion.py
 src/ricco/util/building_address.py
 src/ricco/util/coord_trans.py
+src/ricco/util/decorator.py
+src/ricco/util/docx.py
 src/ricco/util/dt.py
 src/ricco/util/geom.py
 src/ricco/util/id_number.py
 src/ricco/util/os.py
 src/ricco/util/phone_number.py
 src/ricco/util/strings.py
+src/ricco/util/topology_check.py
 src/ricco/util/util.py
```

