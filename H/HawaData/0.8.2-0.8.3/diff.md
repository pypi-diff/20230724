# Comparing `tmp/HawaData-0.8.2.tar.gz` & `tmp/HawaData-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HawaData-0.8.2.tar", last modified: Mon Jul 24 04:17:50 2023, max compression
+gzip compressed data, was "HawaData-0.8.3.tar", last modified: Mon Jul 24 04:31:52 2023, max compression
```

## Comparing `HawaData-0.8.2.tar` & `HawaData-0.8.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 04:17:50.419211 HawaData-0.8.2/
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 04:17:50.409480 HawaData-0.8.2/HawaData.egg-info/
--rw-r--r--   0 wangzhou   (501) staff       (20)     3371 2023-07-24 04:17:50.000000 HawaData-0.8.2/HawaData.egg-info/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      584 2023-07-24 04:17:50.000000 HawaData-0.8.2/HawaData.egg-info/SOURCES.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-07-24 04:17:50.000000 HawaData-0.8.2/HawaData.egg-info/dependency_links.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-07-24 04:17:50.000000 HawaData-0.8.2/HawaData.egg-info/top_level.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)     3371 2023-07-24 04:17:50.418902 HawaData-0.8.2/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.8.2/README.md
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 04:17:50.410005 HawaData-0.8.2/hawa/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.8.2/hawa/__init__.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 04:17:50.411928 HawaData-0.8.2/hawa/base/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.8.2/hawa/base/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2627 2023-06-19 08:54:42.000000 HawaData-0.8.2/hawa/base/db.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.8.2/hawa/base/decos.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.8.2/hawa/base/errors.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.8.2/hawa/base/init.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 04:17:50.413713 HawaData-0.8.2/hawa/common/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.8.2/hawa/common/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    16387 2023-07-24 04:17:40.000000 HawaData-0.8.2/hawa/common/data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     6457 2023-07-21 07:00:47.000000 HawaData-0.8.2/hawa/common/query.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     3098 2023-06-19 08:54:42.000000 HawaData-0.8.2/hawa/common/utils.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2714 2023-07-24 04:07:20.000000 HawaData-0.8.2/hawa/config.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 04:17:50.416896 HawaData-0.8.2/hawa/data/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.8.2/hawa/data/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.8.2/hawa/data/city.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.8.2/hawa/data/district.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.8.2/hawa/data/klass.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      711 2023-06-26 06:27:54.000000 HawaData-0.8.2/hawa/data/province.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1103 2023-07-24 04:17:40.000000 HawaData-0.8.2/hawa/data/school.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1015 2023-07-19 03:28:20.000000 HawaData-0.8.2/hawa/data/student.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 04:17:50.417977 HawaData-0.8.2/hawa/paper/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.8.2/hawa/paper/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    28835 2023-07-24 04:17:40.000000 HawaData-0.8.2/hawa/paper/health.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5421 2023-07-24 04:17:40.000000 HawaData-0.8.2/hawa/paper/mht.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-07-24 04:17:50.419303 HawaData-0.8.2/setup.cfg
--rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.8.2/setup.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 04:17:50.418291 HawaData-0.8.2/test/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.8.2/test/test_query.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 04:31:52.142791 HawaData-0.8.3/
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 04:31:52.135347 HawaData-0.8.3/HawaData.egg-info/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3408 2023-07-24 04:31:52.000000 HawaData-0.8.3/HawaData.egg-info/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      584 2023-07-24 04:31:52.000000 HawaData-0.8.3/HawaData.egg-info/SOURCES.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-07-24 04:31:52.000000 HawaData-0.8.3/HawaData.egg-info/dependency_links.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-07-24 04:31:52.000000 HawaData-0.8.3/HawaData.egg-info/top_level.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3408 2023-07-24 04:31:52.142507 HawaData-0.8.3/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.8.3/README.md
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 04:31:52.136052 HawaData-0.8.3/hawa/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.8.3/hawa/__init__.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 04:31:52.137699 HawaData-0.8.3/hawa/base/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.8.3/hawa/base/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2627 2023-06-19 08:54:42.000000 HawaData-0.8.3/hawa/base/db.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.8.3/hawa/base/decos.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.8.3/hawa/base/errors.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.8.3/hawa/base/init.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 04:31:52.138820 HawaData-0.8.3/hawa/common/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.8.3/hawa/common/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    16413 2023-07-24 04:31:22.000000 HawaData-0.8.3/hawa/common/data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     6457 2023-07-21 07:00:47.000000 HawaData-0.8.3/hawa/common/query.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3236 2023-07-24 04:28:13.000000 HawaData-0.8.3/hawa/common/utils.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2714 2023-07-24 04:07:20.000000 HawaData-0.8.3/hawa/config.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 04:31:52.140746 HawaData-0.8.3/hawa/data/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.8.3/hawa/data/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.8.3/hawa/data/city.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.8.3/hawa/data/district.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.8.3/hawa/data/klass.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      711 2023-06-26 06:27:54.000000 HawaData-0.8.3/hawa/data/province.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1129 2023-07-24 04:28:13.000000 HawaData-0.8.3/hawa/data/school.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1015 2023-07-19 03:28:20.000000 HawaData-0.8.3/hawa/data/student.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 04:31:52.141574 HawaData-0.8.3/hawa/paper/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.8.3/hawa/paper/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    28951 2023-07-24 04:31:22.000000 HawaData-0.8.3/hawa/paper/health.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5470 2023-07-24 04:31:22.000000 HawaData-0.8.3/hawa/paper/mht.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-07-24 04:31:52.142876 HawaData-0.8.3/setup.cfg
+-rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.8.3/setup.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 04:31:52.141849 HawaData-0.8.3/test/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.8.3/test/test_query.py
```

### Comparing `HawaData-0.8.2/HawaData.egg-info/PKG-INFO` & `HawaData-0.8.3/HawaData.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.8.2
+Version: 0.8.3
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -114,7 +114,8 @@
 - 0.7.6 add ProvinceHealthApiDataLess for cascade schools
 - 0.7.7 add school mht api data
 - 0.7.8 optimization student data
 - 0.7.9 sort dim field
 - 0.8.0 sort dim field
 - 0.8.1 sort dim field
 - 0.8.2 add global precision
+- 0.8.3 add global precision in func
```

### Comparing `HawaData-0.8.2/HawaData.egg-info/SOURCES.txt` & `HawaData-0.8.3/HawaData.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.2/PKG-INFO` & `HawaData-0.8.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.8.2
+Version: 0.8.3
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -114,7 +114,8 @@
 - 0.7.6 add ProvinceHealthApiDataLess for cascade schools
 - 0.7.7 add school mht api data
 - 0.7.8 optimization student data
 - 0.7.9 sort dim field
 - 0.8.0 sort dim field
 - 0.8.1 sort dim field
 - 0.8.2 add global precision
+- 0.8.3 add global precision in func
```

### Comparing `HawaData-0.8.2/README.md` & `HawaData-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.2/hawa/base/db.py` & `HawaData-0.8.3/hawa/base/db.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.2/hawa/base/init.py` & `HawaData-0.8.3/hawa/base/init.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.2/hawa/common/data.py` & `HawaData-0.8.3/hawa/common/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import pandas as pd
 import pendulum
 from munch import Munch
 
 from hawa.base.db import DbUtil, RedisUtil
 from hawa.base.errors import NoCasesError
 from hawa.common.query import DataQuery
-from hawa.common.utils import GradeData, CaseData, Measurement
+from hawa.common.utils import GradeData, CaseData, Measurement, Util
 from hawa.config import project
 
 
 class MetaCommomData(type):
     def __new__(cls, name, bases, attrs):
         attrs['db'] = DbUtil()
         attrs['redis'] = RedisUtil()
@@ -258,29 +258,29 @@
         """
         计算维度、领域的 ranks 分级比例
         :param item_code:dimision or field
         """
         r = defaultdict(list)
         codes = set()
         for (s, c), student_code_group in self.final_answers.groupby(['student_id', item_code]):
-            s_c_score = round(student_code_group.score.mean() * 100, project.precision)
+            s_c_score = Util.format_num(student_code_group.score.mean() * 100, project.precision)
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
-            row_ranks = {k: round(v / sum_value * 100, project.precision) for k, v in
+            row_ranks = {k: Util.format_num(v / sum_value * 100, project.precision) for k, v in
                          (base_row_ranks | count_row_ranks).items()}
             res[c] = row_ranks
         code_map = self.get_dim_field_order(key=item_code)
         return {
             "data": res, "codes": sorted(codes, key=lambda x: code_map[x]),
             "legend": self.rank_names,
         }
```

### Comparing `HawaData-0.8.2/hawa/common/query.py` & `HawaData-0.8.3/hawa/common/query.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.2/hawa/common/utils.py` & `HawaData-0.8.3/hawa/common/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,7 +104,13 @@
             else:
                 res.add('高中')
         return res
 
     @property
     def grade_name_list(self) -> list[str]:
         return [f"{project.grade_simple[i]}年级" for i in self.grades]
+
+
+class Util:
+    @classmethod
+    def format_num(cls, num: float | int, precision: int = 1):
+        return round(float(num), precision)
```

### Comparing `HawaData-0.8.2/hawa/config.py` & `HawaData-0.8.3/hawa/config.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.2/hawa/data/klass.py` & `HawaData-0.8.3/hawa/data/klass.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.2/hawa/data/province.py` & `HawaData-0.8.3/hawa/data/province.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.2/hawa/data/school.py` & `HawaData-0.8.3/hawa/data/school.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from dataclasses import dataclass
 
+from hawa.common.utils import Util
 from hawa.config import project
 from hawa.paper.health import HealthReportData, HealthApiData
 from hawa.paper.mht import MhtWebData, MhtApiData
 
 
 @dataclass
 class SchoolMixin:
@@ -14,15 +15,15 @@
 @dataclass
 class SchoolHealthApiData(SchoolMixin, HealthApiData):
     def get_class_scores(self):
         """获取年级各班级的分数"""
         scores = self.final_scores
         scores['cls'] = scores['student_id'].apply(lambda x: f"{int(str(x)[13:15])}班")
         res = scores.groupby('cls').score.mean().to_dict()
-        keys, values = res.keys(), [round(i, project.precision) for i in res.values()]
+        keys, values = res.keys(), [Util.format_num(i) for i in res.values()]
         return {'keys': list(keys), 'values': list(values)}
 
 
 @dataclass
 class SchoolHealthReportData(SchoolMixin, HealthReportData):
     pass
```

### Comparing `HawaData-0.8.2/hawa/data/student.py` & `HawaData-0.8.3/hawa/data/student.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.2/hawa/paper/health.py` & `HawaData-0.8.3/hawa/paper/health.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 import pandas as pd
 from munch import Munch
 from pingouin import cronbach_alpha
 
 from hawa.base.errors import NoCasesError
 from hawa.common.data import CommonData
+from hawa.common.utils import Util
 from hawa.config import project
 
 
 @dataclass
 class HealthData(CommonData):
     """健康测评数据，不应直接使用，应向下继承 city/district/school 等"""
     test_types: list[str] = field(default_factory=lambda: ['publicWelfare', 'ZjpublicWelfare'])
@@ -55,27 +56,27 @@
         if gender:
             final_scores = fs.loc[fs.gender == gender, :]
         raw = final_scores.level.value_counts().to_dict()
         data = base | raw
         sum_data = sum(data.values())
         if not sum_data:
             raise ValueError(f'grade {grade} score rank is empty')
-        percent = {k: round(v * 100 / sum_data, project.precision) for k, v in data.items()}
+        percent = {k: Util.format_num(v * 100 / sum_data, project.precision) for k, v in data.items()}
         return percent
 
     def gender_compare(self, grade: int):
         """某年级学生健康素养水平及性别比较图"""
         final_scores = self.__get_grade_final_scores(grade=grade)
         total_score = final_scores.score.mean()
         m_score = final_scores.loc[final_scores.gender == 'M'].score.mean()
         f_score = final_scores.loc[final_scores.gender == 'F'].score.mean()
         return {
-            "total": round(total_score, project.precision),
-            "M": round(m_score, project.precision),
-            "F": round(f_score, project.precision)
+            "total": Util.format_num(total_score, project.precision),
+            "M": Util.format_num(m_score, project.precision),
+            "F": Util.format_num(f_score, project.precision),
         }
 
     def dim_field_gender_compare(self, grade: int, item_code: str, key_format: str = 'en'):
         """某年级六大领域/四大维度测评得分及性别比较图"""
         final_answers = self.__get_grade_final_answers(grade=grade)
         answers = final_answers.loc[~final_answers[item_code].isnull(), :]
         raw_data = {
@@ -135,15 +136,15 @@
         计算维度或领域得分
         :param answers: 由 final answers 中取出的部分数据，属于某一主体
         :param item_code: dimension/field
         :return:
         """
         keys, values, mapping = [], [], {}
         for code, code_group in answers.groupby(item_code):
-            score = round(code_group.score.mean() * 100, project.precision)
+            score = Util.format_num(code_group.score.mean() * 100, project.precision)
             keys.append(code)
             values.append(score)
             mapping[code] = score
         match res_format:
             case 'dict':
                 return mapping
             case 'list':
@@ -196,15 +197,15 @@
                 records.append(record)
         self.code_scores = pd.DataFrame.from_records(records)
 
     def _to_count_d_summary_scores(self):
         records = defaultdict(dict)
         for grade, group in self.code_scores.groupby('grade'):
             for gender in project.gender_map.keys():
-                records[grade][gender] = round(self._count_school_score(group, key=gender), project.precision)
+                records[grade][gender] = Util.format_num(self._count_school_score(group, key=gender), project.precision)
         self.summary_scores = records
 
     def _to_count_e_grade_good_bad(self):
         records = defaultdict(dict)
         for g, group in self.code_scores.groupby('grade'):
             for gender in project.gender_map.keys():
                 records[g][gender] = {
@@ -520,16 +521,16 @@
         data = data.loc[:, use_cols].sort_values(['category_sch', 'code'])
         del data['category_sch']
         return data
 
     def compare_gender_text(self, grade: int):
         grade_rank_dis_m = self.grade_rank_dis[grade].M
         grade_rank_dis_f = self.grade_rank_dis[grade].F
-        level_m = round(sum([grade_rank_dis_m['优秀'], grade_rank_dis_m['良好']]), project.precision)
-        level_f = round(sum([grade_rank_dis_f['优秀'], grade_rank_dis_f['良好']]), project.precision)
+        level_m = Util.format_num(sum([grade_rank_dis_m['优秀'], grade_rank_dis_m['良好']]), project.precision)
+        level_f = Util.format_num(sum([grade_rank_dis_f['优秀'], grade_rank_dis_f['良好']]), project.precision)
         if level_m - level_f >= 5:
             return '男生明显高于女生'
         elif level_m - level_f <= -5:
             return '男生明显低于女生'
         else:
             return '男生与女生不存在明显差异'
```

### Comparing `HawaData-0.8.2/hawa/paper/mht.py` & `HawaData-0.8.3/hawa/paper/mht.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from collections import defaultdict
 from dataclasses import dataclass, field
 from typing import Set
 
 import pandas as pd
 
 from hawa.common.data import CommonData
+from hawa.common.utils import Util
 from hawa.config import project
 
 
 @dataclass
 class MhtData(CommonData):
     test_types: list[str] = field(default_factory=lambda: ['mht', 'mhtPlus'])
     code_word_list: Set[str] = field(default_factory=lambda: {'mht'})
@@ -77,26 +78,26 @@
 
     def _to_count_h_grade_special_students(self):
         """计算各年级 某量表超过8分的学生"""
         res = defaultdict(list)
         for grade, grade_ans_group in self.final_answers.groupby('grade'):
             for student_id, student_group in grade_ans_group.groupby('student_id'):
                 student_name = student_group['username'].tolist()[0]
-                student_score = round(student_group['score'].sum(), project.precision)
+                student_score = Util.format_num(student_group['score'].sum(), precision=project.precision)
                 if student_score > 65:
                     res[grade].append(
                         self._tool_count_sub_code_score(answers=student_group, unit_name=student_name)
                     )
         self.grade_special_students = res
 
     # 计算工具
     def _tool_count_student_score(self, score: pd.DataFrame):
         data = []
         handred = set(range(0, 101))
-        score['score'] = score.score.apply(lambda x: int(round(x, project.precision)))
+        score['score'] = score.score.apply(lambda x: int(x))
 
         for s, row in score.groupby('score'):
             handred.discard(s)
             data.append((s, int(row.score.count())))
         for h in handred:
             data.append((h, 0))
         data.sort(key=lambda x: x[0])
@@ -116,15 +117,15 @@
         x_axis, y_axis = [], []
         for (student_id, mht), group in answers.groupby(by=['student_id', 'mht']):
             if mht == '效度':
                 continue
             mht_scores[mht].append(group.score.sum())
         for mht, score_list in mht_scores.items():
             x_axis.append(mht)
-            y_axis.append(round(float(sum(score_list) / len(score_list)), project.precision))
+            y_axis.append(Util.format_num(float(sum(score_list) / len(score_list)), precision=project.precision))
 
         return {
             "name": unit_name if unit_name else self.meta_unit.name,
             "x_axis": x_axis,
             "y_axis": y_axis,
         }
```

### Comparing `HawaData-0.8.2/setup.py` & `HawaData-0.8.3/setup.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.2/test/test_query.py` & `HawaData-0.8.3/test/test_query.py`

 * *Files identical despite different names*

