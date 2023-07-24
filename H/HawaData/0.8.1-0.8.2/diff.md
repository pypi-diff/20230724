# Comparing `tmp/HawaData-0.8.1.tar.gz` & `tmp/HawaData-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HawaData-0.8.1.tar", last modified: Sun Jul 23 08:55:10 2023, max compression
+gzip compressed data, was "HawaData-0.8.2.tar", last modified: Mon Jul 24 04:17:50 2023, max compression
```

## Comparing `HawaData-0.8.1.tar` & `HawaData-0.8.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-23 08:55:10.500066 HawaData-0.8.1/
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-23 08:55:10.488413 HawaData-0.8.1/HawaData.egg-info/
--rw-r--r--   0 wangzhou   (501) staff       (20)     3342 2023-07-23 08:55:10.000000 HawaData-0.8.1/HawaData.egg-info/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      584 2023-07-23 08:55:10.000000 HawaData-0.8.1/HawaData.egg-info/SOURCES.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-07-23 08:55:10.000000 HawaData-0.8.1/HawaData.egg-info/dependency_links.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-07-23 08:55:10.000000 HawaData-0.8.1/HawaData.egg-info/top_level.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)     3342 2023-07-23 08:55:10.499785 HawaData-0.8.1/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.8.1/README.md
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-23 08:55:10.488937 HawaData-0.8.1/hawa/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.8.1/hawa/__init__.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-23 08:55:10.491437 HawaData-0.8.1/hawa/base/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.8.1/hawa/base/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2627 2023-06-19 08:54:42.000000 HawaData-0.8.1/hawa/base/db.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.8.1/hawa/base/decos.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.8.1/hawa/base/errors.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.8.1/hawa/base/init.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-23 08:55:10.493299 HawaData-0.8.1/hawa/common/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.8.1/hawa/common/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    16330 2023-07-23 08:53:40.000000 HawaData-0.8.1/hawa/common/data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     6457 2023-07-21 07:00:47.000000 HawaData-0.8.1/hawa/common/query.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     3098 2023-06-19 08:54:42.000000 HawaData-0.8.1/hawa/common/utils.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2696 2023-06-26 02:08:50.000000 HawaData-0.8.1/hawa/config.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-23 08:55:10.497212 HawaData-0.8.1/hawa/data/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.8.1/hawa/data/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.8.1/hawa/data/city.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.8.1/hawa/data/district.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.8.1/hawa/data/klass.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      711 2023-06-26 06:27:54.000000 HawaData-0.8.1/hawa/data/province.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1055 2023-07-17 06:57:10.000000 HawaData-0.8.1/hawa/data/school.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1015 2023-07-19 03:28:20.000000 HawaData-0.8.1/hawa/data/student.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-23 08:55:10.498484 HawaData-0.8.1/hawa/paper/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.8.1/hawa/paper/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    28707 2023-07-23 08:45:55.000000 HawaData-0.8.1/hawa/paper/health.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5373 2023-07-17 07:05:31.000000 HawaData-0.8.1/hawa/paper/mht.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-07-23 08:55:10.500149 HawaData-0.8.1/setup.cfg
--rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.8.1/setup.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-23 08:55:10.499136 HawaData-0.8.1/test/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.8.1/test/test_query.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 04:17:50.419211 HawaData-0.8.2/
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 04:17:50.409480 HawaData-0.8.2/HawaData.egg-info/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3371 2023-07-24 04:17:50.000000 HawaData-0.8.2/HawaData.egg-info/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      584 2023-07-24 04:17:50.000000 HawaData-0.8.2/HawaData.egg-info/SOURCES.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-07-24 04:17:50.000000 HawaData-0.8.2/HawaData.egg-info/dependency_links.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-07-24 04:17:50.000000 HawaData-0.8.2/HawaData.egg-info/top_level.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3371 2023-07-24 04:17:50.418902 HawaData-0.8.2/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.8.2/README.md
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 04:17:50.410005 HawaData-0.8.2/hawa/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.8.2/hawa/__init__.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 04:17:50.411928 HawaData-0.8.2/hawa/base/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.8.2/hawa/base/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2627 2023-06-19 08:54:42.000000 HawaData-0.8.2/hawa/base/db.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.8.2/hawa/base/decos.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.8.2/hawa/base/errors.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.8.2/hawa/base/init.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 04:17:50.413713 HawaData-0.8.2/hawa/common/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.8.2/hawa/common/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    16387 2023-07-24 04:17:40.000000 HawaData-0.8.2/hawa/common/data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     6457 2023-07-21 07:00:47.000000 HawaData-0.8.2/hawa/common/query.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3098 2023-06-19 08:54:42.000000 HawaData-0.8.2/hawa/common/utils.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2714 2023-07-24 04:07:20.000000 HawaData-0.8.2/hawa/config.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 04:17:50.416896 HawaData-0.8.2/hawa/data/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.8.2/hawa/data/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.8.2/hawa/data/city.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.8.2/hawa/data/district.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.8.2/hawa/data/klass.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      711 2023-06-26 06:27:54.000000 HawaData-0.8.2/hawa/data/province.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1103 2023-07-24 04:17:40.000000 HawaData-0.8.2/hawa/data/school.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1015 2023-07-19 03:28:20.000000 HawaData-0.8.2/hawa/data/student.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 04:17:50.417977 HawaData-0.8.2/hawa/paper/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.8.2/hawa/paper/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    28835 2023-07-24 04:17:40.000000 HawaData-0.8.2/hawa/paper/health.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5421 2023-07-24 04:17:40.000000 HawaData-0.8.2/hawa/paper/mht.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-07-24 04:17:50.419303 HawaData-0.8.2/setup.cfg
+-rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.8.2/setup.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 04:17:50.418291 HawaData-0.8.2/test/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.8.2/test/test_query.py
```

### Comparing `HawaData-0.8.1/HawaData.egg-info/PKG-INFO` & `HawaData-0.8.2/HawaData.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.8.1
+Version: 0.8.2
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -113,7 +113,8 @@
 - 0.7.5 add ch key for dim_field data
 - 0.7.6 add ProvinceHealthApiDataLess for cascade schools
 - 0.7.7 add school mht api data
 - 0.7.8 optimization student data
 - 0.7.9 sort dim field
 - 0.8.0 sort dim field
 - 0.8.1 sort dim field
+- 0.8.2 add global precision
```

### Comparing `HawaData-0.8.1/HawaData.egg-info/SOURCES.txt` & `HawaData-0.8.2/HawaData.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.1/PKG-INFO` & `HawaData-0.8.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.8.1
+Version: 0.8.2
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -113,7 +113,8 @@
 - 0.7.5 add ch key for dim_field data
 - 0.7.6 add ProvinceHealthApiDataLess for cascade schools
 - 0.7.7 add school mht api data
 - 0.7.8 optimization student data
 - 0.7.9 sort dim field
 - 0.8.0 sort dim field
 - 0.8.1 sort dim field
+- 0.8.2 add global precision
```

### Comparing `HawaData-0.8.1/README.md` & `HawaData-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.1/hawa/base/db.py` & `HawaData-0.8.2/hawa/base/db.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.1/hawa/base/init.py` & `HawaData-0.8.2/hawa/base/init.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.1/hawa/common/data.py` & `HawaData-0.8.2/hawa/common/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,29 +258,30 @@
         """
         计算维度、领域的 ranks 分级比例
         :param item_code:dimision or field
         """
         r = defaultdict(list)
         codes = set()
         for (s, c), student_code_group in self.final_answers.groupby(['student_id', item_code]):
-            s_c_score = round(student_code_group.score.mean() * 100, 2)
+            s_c_score = round(student_code_group.score.mean() * 100, project.precision)
             codes.add(c)
             r[c].append(s_c_score)
         codes = list(codes)
         df = pd.DataFrame.from_records(r)
         res = {}
         for c in codes:
             row = df[c]
             base_row_ranks = {k: 0 for k in self.rank_names}
             count_row_ranks = pd.cut(
                 row, bins=[0, 60, 80, 90, 100], labels=self.rank_names,
                 right=False, include_lowest=True,
             ).value_counts().to_dict()
             sum_value = sum(count_row_ranks.values())
-            row_ranks = {k: round(v / sum_value * 100, 2) for k, v in (base_row_ranks | count_row_ranks).items()}
+            row_ranks = {k: round(v / sum_value * 100, project.precision) for k, v in
+                         (base_row_ranks | count_row_ranks).items()}
             res[c] = row_ranks
         code_map = self.get_dim_field_order(key=item_code)
         return {
             "data": res, "codes": sorted(codes, key=lambda x: code_map[x]),
             "legend": self.rank_names,
         }
```

### Comparing `HawaData-0.8.1/hawa/common/query.py` & `HawaData-0.8.2/hawa/common/query.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.1/hawa/common/utils.py` & `HawaData-0.8.2/hawa/common/utils.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.1/hawa/config.py` & `HawaData-0.8.2/hawa/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,15 @@
         12: '高中三'
     }
 
     grade_simple = {**dict(zip(range(1, 11), '一二三四五六七八九十')), **{11: '十一', 12: '十二'}}
 
     # number
     number_map = dict(zip(range(1, 11), '一二三四五六七八九十'))
+    precision = 1
 
     category_map = {
         'total': "学生", 'M': '男生', "F": "女生"
     }
 
     # other
     municipality = {11, 12, 31, 50}
```

### Comparing `HawaData-0.8.1/hawa/data/klass.py` & `HawaData-0.8.2/hawa/data/klass.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.1/hawa/data/province.py` & `HawaData-0.8.2/hawa/data/province.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.1/hawa/data/school.py` & `HawaData-0.8.2/hawa/data/school.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from dataclasses import dataclass
 
+from hawa.config import project
 from hawa.paper.health import HealthReportData, HealthApiData
 from hawa.paper.mht import MhtWebData, MhtApiData
 
 
 @dataclass
 class SchoolMixin:
     """为了在 __mro__ 中有更高的优先级， mixin 在继承时，应该放在最前"""
@@ -13,15 +14,15 @@
 @dataclass
 class SchoolHealthApiData(SchoolMixin, HealthApiData):
     def get_class_scores(self):
         """获取年级各班级的分数"""
         scores = self.final_scores
         scores['cls'] = scores['student_id'].apply(lambda x: f"{int(str(x)[13:15])}班")
         res = scores.groupby('cls').score.mean().to_dict()
-        keys, values = res.keys(), [round(i, 2) for i in res.values()]
+        keys, values = res.keys(), [round(i, project.precision) for i in res.values()]
         return {'keys': list(keys), 'values': list(values)}
 
 
 @dataclass
 class SchoolHealthReportData(SchoolMixin, HealthReportData):
     pass
```

### Comparing `HawaData-0.8.1/hawa/data/student.py` & `HawaData-0.8.2/hawa/data/student.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.1/hawa/paper/health.py` & `HawaData-0.8.2/hawa/paper/health.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,27 +55,27 @@
         if gender:
             final_scores = fs.loc[fs.gender == gender, :]
         raw = final_scores.level.value_counts().to_dict()
         data = base | raw
         sum_data = sum(data.values())
         if not sum_data:
             raise ValueError(f'grade {grade} score rank is empty')
-        percent = {k: round(v * 100 / sum_data, 2) for k, v in data.items()}
+        percent = {k: round(v * 100 / sum_data, project.precision) for k, v in data.items()}
         return percent
 
     def gender_compare(self, grade: int):
         """某年级学生健康素养水平及性别比较图"""
         final_scores = self.__get_grade_final_scores(grade=grade)
         total_score = final_scores.score.mean()
         m_score = final_scores.loc[final_scores.gender == 'M'].score.mean()
         f_score = final_scores.loc[final_scores.gender == 'F'].score.mean()
         return {
-            "total": round(total_score, 2),
-            "M": round(m_score, 2),
-            "F": round(f_score, 2)
+            "total": round(total_score, project.precision),
+            "M": round(m_score, project.precision),
+            "F": round(f_score, project.precision)
         }
 
     def dim_field_gender_compare(self, grade: int, item_code: str, key_format: str = 'en'):
         """某年级六大领域/四大维度测评得分及性别比较图"""
         final_answers = self.__get_grade_final_answers(grade=grade)
         answers = final_answers.loc[~final_answers[item_code].isnull(), :]
         raw_data = {
@@ -135,15 +135,15 @@
         计算维度或领域得分
         :param answers: 由 final answers 中取出的部分数据，属于某一主体
         :param item_code: dimension/field
         :return:
         """
         keys, values, mapping = [], [], {}
         for code, code_group in answers.groupby(item_code):
-            score = round(code_group.score.mean() * 100, 2)
+            score = round(code_group.score.mean() * 100, project.precision)
             keys.append(code)
             values.append(score)
             mapping[code] = score
         match res_format:
             case 'dict':
                 return mapping
             case 'list':
@@ -196,15 +196,15 @@
                 records.append(record)
         self.code_scores = pd.DataFrame.from_records(records)
 
     def _to_count_d_summary_scores(self):
         records = defaultdict(dict)
         for grade, group in self.code_scores.groupby('grade'):
             for gender in project.gender_map.keys():
-                records[grade][gender] = round(self._count_school_score(group, key=gender), 1)
+                records[grade][gender] = round(self._count_school_score(group, key=gender), project.precision)
         self.summary_scores = records
 
     def _to_count_e_grade_good_bad(self):
         records = defaultdict(dict)
         for g, group in self.code_scores.groupby('grade'):
             for gender in project.gender_map.keys():
                 records[g][gender] = {
@@ -520,16 +520,16 @@
         data = data.loc[:, use_cols].sort_values(['category_sch', 'code'])
         del data['category_sch']
         return data
 
     def compare_gender_text(self, grade: int):
         grade_rank_dis_m = self.grade_rank_dis[grade].M
         grade_rank_dis_f = self.grade_rank_dis[grade].F
-        level_m = round(sum([grade_rank_dis_m['优秀'], grade_rank_dis_m['良好']]), 1)
-        level_f = round(sum([grade_rank_dis_f['优秀'], grade_rank_dis_f['良好']]), 1)
+        level_m = round(sum([grade_rank_dis_m['优秀'], grade_rank_dis_m['良好']]), project.precision)
+        level_f = round(sum([grade_rank_dis_f['优秀'], grade_rank_dis_f['良好']]), project.precision)
         if level_m - level_f >= 5:
             return '男生明显高于女生'
         elif level_m - level_f <= -5:
             return '男生明显低于女生'
         else:
             return '男生与女生不存在明显差异'
```

### Comparing `HawaData-0.8.1/hawa/paper/mht.py` & `HawaData-0.8.2/hawa/paper/mht.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,26 +77,26 @@
 
     def _to_count_h_grade_special_students(self):
         """计算各年级 某量表超过8分的学生"""
         res = defaultdict(list)
         for grade, grade_ans_group in self.final_answers.groupby('grade'):
             for student_id, student_group in grade_ans_group.groupby('student_id'):
                 student_name = student_group['username'].tolist()[0]
-                student_score = round(student_group['score'].sum(), 0)
+                student_score = round(student_group['score'].sum(), project.precision)
                 if student_score > 65:
                     res[grade].append(
                         self._tool_count_sub_code_score(answers=student_group, unit_name=student_name)
                     )
         self.grade_special_students = res
 
     # 计算工具
     def _tool_count_student_score(self, score: pd.DataFrame):
         data = []
         handred = set(range(0, 101))
-        score['score'] = score.score.apply(lambda x: int(round(x, 0)))
+        score['score'] = score.score.apply(lambda x: int(round(x, project.precision)))
 
         for s, row in score.groupby('score'):
             handred.discard(s)
             data.append((s, int(row.score.count())))
         for h in handred:
             data.append((h, 0))
         data.sort(key=lambda x: x[0])
@@ -116,15 +116,15 @@
         x_axis, y_axis = [], []
         for (student_id, mht), group in answers.groupby(by=['student_id', 'mht']):
             if mht == '效度':
                 continue
             mht_scores[mht].append(group.score.sum())
         for mht, score_list in mht_scores.items():
             x_axis.append(mht)
-            y_axis.append(round(float(sum(score_list) / len(score_list)), 1))
+            y_axis.append(round(float(sum(score_list) / len(score_list)), project.precision))
 
         return {
             "name": unit_name if unit_name else self.meta_unit.name,
             "x_axis": x_axis,
             "y_axis": y_axis,
         }
```

### Comparing `HawaData-0.8.1/setup.py` & `HawaData-0.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.1/test/test_query.py` & `HawaData-0.8.2/test/test_query.py`

 * *Files identical despite different names*

