# Comparing `tmp/HawaData-0.8.4.tar.gz` & `tmp/HawaData-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HawaData-0.8.4.tar", last modified: Mon Jul 24 07:05:21 2023, max compression
+gzip compressed data, was "HawaData-0.8.5.tar", last modified: Mon Jul 24 08:00:36 2023, max compression
```

## Comparing `HawaData-0.8.4.tar` & `HawaData-0.8.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 07:05:21.358096 HawaData-0.8.4/
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 07:05:21.346704 HawaData-0.8.4/HawaData.egg-info/
--rw-r--r--   0 wangzhou   (501) staff       (20)     3436 2023-07-24 07:05:21.000000 HawaData-0.8.4/HawaData.egg-info/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      584 2023-07-24 07:05:21.000000 HawaData-0.8.4/HawaData.egg-info/SOURCES.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-07-24 07:05:21.000000 HawaData-0.8.4/HawaData.egg-info/dependency_links.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-07-24 07:05:21.000000 HawaData-0.8.4/HawaData.egg-info/top_level.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)     3436 2023-07-24 07:05:21.357851 HawaData-0.8.4/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.8.4/README.md
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 07:05:21.347180 HawaData-0.8.4/hawa/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.8.4/hawa/__init__.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 07:05:21.349512 HawaData-0.8.4/hawa/base/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.8.4/hawa/base/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2627 2023-06-19 08:54:42.000000 HawaData-0.8.4/hawa/base/db.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.8.4/hawa/base/decos.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.8.4/hawa/base/errors.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.8.4/hawa/base/init.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 07:05:21.351189 HawaData-0.8.4/hawa/common/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.8.4/hawa/common/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    16490 2023-07-24 07:05:02.000000 HawaData-0.8.4/hawa/common/data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     6457 2023-07-21 07:00:47.000000 HawaData-0.8.4/hawa/common/query.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     3236 2023-07-24 04:28:13.000000 HawaData-0.8.4/hawa/common/utils.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2714 2023-07-24 04:07:20.000000 HawaData-0.8.4/hawa/config.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 07:05:21.354745 HawaData-0.8.4/hawa/data/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.8.4/hawa/data/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.8.4/hawa/data/city.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.8.4/hawa/data/district.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.8.4/hawa/data/klass.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      711 2023-06-26 06:27:54.000000 HawaData-0.8.4/hawa/data/province.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1129 2023-07-24 04:28:13.000000 HawaData-0.8.4/hawa/data/school.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1015 2023-07-19 03:28:20.000000 HawaData-0.8.4/hawa/data/student.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 07:05:21.356948 HawaData-0.8.4/hawa/paper/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.8.4/hawa/paper/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    28951 2023-07-24 04:31:22.000000 HawaData-0.8.4/hawa/paper/health.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5470 2023-07-24 04:31:22.000000 HawaData-0.8.4/hawa/paper/mht.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-07-24 07:05:21.358168 HawaData-0.8.4/setup.cfg
--rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.8.4/setup.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 07:05:21.357335 HawaData-0.8.4/test/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.8.4/test/test_query.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 08:00:36.741340 HawaData-0.8.5/
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 08:00:36.726947 HawaData-0.8.5/HawaData.egg-info/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3459 2023-07-24 08:00:36.000000 HawaData-0.8.5/HawaData.egg-info/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      584 2023-07-24 08:00:36.000000 HawaData-0.8.5/HawaData.egg-info/SOURCES.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-07-24 08:00:36.000000 HawaData-0.8.5/HawaData.egg-info/dependency_links.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-07-24 08:00:36.000000 HawaData-0.8.5/HawaData.egg-info/top_level.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3459 2023-07-24 08:00:36.740963 HawaData-0.8.5/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.8.5/README.md
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 08:00:36.727569 HawaData-0.8.5/hawa/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.8.5/hawa/__init__.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 08:00:36.730402 HawaData-0.8.5/hawa/base/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.8.5/hawa/base/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2627 2023-06-19 08:54:42.000000 HawaData-0.8.5/hawa/base/db.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.8.5/hawa/base/decos.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.8.5/hawa/base/errors.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.8.5/hawa/base/init.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 08:00:36.732231 HawaData-0.8.5/hawa/common/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.8.5/hawa/common/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    16980 2023-07-24 08:00:29.000000 HawaData-0.8.5/hawa/common/data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     6457 2023-07-21 07:00:47.000000 HawaData-0.8.5/hawa/common/query.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3236 2023-07-24 04:28:13.000000 HawaData-0.8.5/hawa/common/utils.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2714 2023-07-24 04:07:20.000000 HawaData-0.8.5/hawa/config.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 08:00:36.736694 HawaData-0.8.5/hawa/data/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.8.5/hawa/data/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.8.5/hawa/data/city.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.8.5/hawa/data/district.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.8.5/hawa/data/klass.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      711 2023-06-26 06:27:54.000000 HawaData-0.8.5/hawa/data/province.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1129 2023-07-24 04:28:13.000000 HawaData-0.8.5/hawa/data/school.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1015 2023-07-19 03:28:20.000000 HawaData-0.8.5/hawa/data/student.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 08:00:36.739377 HawaData-0.8.5/hawa/paper/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.8.5/hawa/paper/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    28951 2023-07-24 04:31:22.000000 HawaData-0.8.5/hawa/paper/health.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5470 2023-07-24 04:31:22.000000 HawaData-0.8.5/hawa/paper/mht.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-07-24 08:00:36.741448 HawaData-0.8.5/setup.cfg
+-rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.8.5/setup.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 08:00:36.740111 HawaData-0.8.5/test/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.8.5/test/test_query.py
```

### Comparing `HawaData-0.8.4/HawaData.egg-info/PKG-INFO` & `HawaData-0.8.5/HawaData.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.8.4
+Version: 0.8.5
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -116,7 +116,8 @@
 - 0.7.8 optimization student data
 - 0.7.9 sort dim field
 - 0.8.0 sort dim field
 - 0.8.1 sort dim field
 - 0.8.2 add global precision
 - 0.8.3 add global precision in func
 - 0.8.4 fix extra dim/field
+- 0.8.5 load less data
```

### Comparing `HawaData-0.8.4/HawaData.egg-info/SOURCES.txt` & `HawaData-0.8.5/HawaData.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.4/PKG-INFO` & `HawaData-0.8.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.8.4
+Version: 0.8.5
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -116,7 +116,8 @@
 - 0.7.8 optimization student data
 - 0.7.9 sort dim field
 - 0.8.0 sort dim field
 - 0.8.1 sort dim field
 - 0.8.2 add global precision
 - 0.8.3 add global precision in func
 - 0.8.4 fix extra dim/field
+- 0.8.5 load less data
```

### Comparing `HawaData-0.8.4/README.md` & `HawaData-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.4/hawa/base/db.py` & `HawaData-0.8.5/hawa/base/db.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.4/hawa/base/init.py` & `HawaData-0.8.5/hawa/base/init.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.4/hawa/common/data.py` & `HawaData-0.8.5/hawa/common/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,16 @@
     meta_unit: Optional[Any] = None
 
     # 时间目标
     target_year: Optional[int] = None
     last_year_num: Optional[int] = None
     is_load_last: bool = True  # 仅计算往年数据时 为 False
 
+    is_load_all: bool = True  # 加载全部数据
+
     # 卷子
     test_type: str = ''
     test_types: list = field(default_factory=list)
     code_word_list: Set[str] = field(default=set)  # 卷子使用指标的词表，详见继承
 
     # meta class tool
     db: ClassVar[DbUtil] = None
@@ -77,25 +79,27 @@
 
     # 去年全国数据
     last_year = None
     last_year_code_scores: Optional[pd.DataFrame] = field(default_factory=pd.DataFrame)
 
     def __post_init__(self):
         # 初始化数据
-        init_functions = [i for i in dir(self) if i.startswith('_to_init_')]
-        for func in init_functions:
-            getattr(self, func)()
+        if self.is_load_all:
+            self.load_all_data()
 
-        # 构建辅助工具
-        self._to_build_helper()
+            # 构建辅助工具
+            self._to_build_helper()
 
-        # 计算数据
-        count_functions = [i for i in dir(self) if i.startswith('_to_count_')]
-        for func in count_functions:
-            getattr(self, func)()
+            # 计算数据
+            count_functions = [i for i in dir(self) if i.startswith('_to_count_')]
+            for func in count_functions:
+                getattr(self, func)()
+        else:
+            self.load_less_data()
+            self._to_build_helper()
 
     def _to_init_a_meta_unit(self):
         self.meta_unit = self.query.query_unit(self.meta_unit_type, str(self.meta_unit_id))
 
     def _to_init_b_time(self):
         if not self.target_year:
             self.target_year = pendulum.now().year
@@ -393,7 +397,19 @@
         :param key: dimension/field
         """
         data = self.codebook.loc[self.codebook['category'] == key, :]
         order_map = {i['name']: i['order'] for _, i in data.iterrows()}
         if '其他' in order_map.keys():
             del order_map['其他']
         return order_map
+
+    def load_less_data(self):
+        init_functions = [i for i in dir(self) if i.startswith('_to_init_')]
+        for func in init_functions:
+            if '_to_init_e_' in func:
+                break
+            getattr(self, func)()
+
+    def load_all_data(self):
+        init_functions = [i for i in dir(self) if i.startswith('_to_init_')]
+        for func in init_functions:
+            getattr(self, func)()
```

### Comparing `HawaData-0.8.4/hawa/common/query.py` & `HawaData-0.8.5/hawa/common/query.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.4/hawa/common/utils.py` & `HawaData-0.8.5/hawa/common/utils.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.4/hawa/config.py` & `HawaData-0.8.5/hawa/config.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.4/hawa/data/klass.py` & `HawaData-0.8.5/hawa/data/klass.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.4/hawa/data/province.py` & `HawaData-0.8.5/hawa/data/province.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.4/hawa/data/school.py` & `HawaData-0.8.5/hawa/data/school.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.4/hawa/data/student.py` & `HawaData-0.8.5/hawa/data/student.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.4/hawa/paper/health.py` & `HawaData-0.8.5/hawa/paper/health.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.4/hawa/paper/mht.py` & `HawaData-0.8.5/hawa/paper/mht.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.4/setup.py` & `HawaData-0.8.5/setup.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.4/test/test_query.py` & `HawaData-0.8.5/test/test_query.py`

 * *Files identical despite different names*

