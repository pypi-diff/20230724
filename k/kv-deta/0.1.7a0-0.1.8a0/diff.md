# Comparing `tmp/kv_deta-0.1.7a0-py3-none-any.whl.zip` & `tmp/kv_deta-0.1.8a0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 15398 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat     3895 b- defN 23-Jul-23 19:13 kv_model.py
--rw-rw-rw-  2.0 fat    34523 b- defN 23-Jul-23 19:34 kv_deta-0.1.7a0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2338 b- defN 23-Jul-23 19:34 kv_deta-0.1.7a0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-23 19:34 kv_deta-0.1.7a0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-23 19:34 kv_deta-0.1.7a0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      464 b- defN 23-Jul-23 19:34 kv_deta-0.1.7a0.dist-info/RECORD
-6 files, 41321 bytes uncompressed, 14560 bytes compressed:  64.8%
+Zip file size: 15417 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat     3889 b- defN 23-Jul-24 17:25 kv_model.py
+-rw-rw-rw-  2.0 fat    34523 b- defN 23-Jul-24 17:36 kv_deta-0.1.8a0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2395 b- defN 23-Jul-24 17:36 kv_deta-0.1.8a0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-24 17:36 kv_deta-0.1.8a0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-24 17:36 kv_deta-0.1.8a0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      464 b- defN 23-Jul-24 17:36 kv_deta-0.1.8a0.dist-info/RECORD
+6 files, 41372 bytes uncompressed, 14579 bytes compressed:  64.8%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: kv_model.py
 Comment: 
 
-Filename: kv_deta-0.1.7a0.dist-info/LICENSE
+Filename: kv_deta-0.1.8a0.dist-info/LICENSE
 Comment: 
 
-Filename: kv_deta-0.1.7a0.dist-info/METADATA
+Filename: kv_deta-0.1.8a0.dist-info/METADATA
 Comment: 
 
-Filename: kv_deta-0.1.7a0.dist-info/WHEEL
+Filename: kv_deta-0.1.8a0.dist-info/WHEEL
 Comment: 
 
-Filename: kv_deta-0.1.7a0.dist-info/top_level.txt
+Filename: kv_deta-0.1.8a0.dist-info/top_level.txt
 Comment: 
 
-Filename: kv_deta-0.1.7a0.dist-info/RECORD
+Filename: kv_deta-0.1.8a0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kv_model.py

```diff
@@ -1,14 +1,14 @@
 ####
 ##
 #
 #
 
 
-__version__ = "0.1.7-alpha"
+__version__ = "0.1.8-alpha"
 
 import re
 
 import more_itertools as mit
 from deta import Base as DetaBase
 from deta import Deta
 
@@ -104,16 +104,16 @@
 
     def __delattr__(self, name: str):
         print("__delattr__", name)
         pass
 
     def get(self, key: str, default=None):
         key = str(key)
-        if self.setdefault(key, self._db.get(key)) is None and default is not None:
-            self[key] = default
+        item = self._db.get(key)
+        self.setdefault(key, item["value"] if item is not None else default)
 
         return self[key]
 
     def inc(self, key):
         pass
 
     def dec(self, key):
```

## Comparing `kv_deta-0.1.7a0.dist-info/LICENSE` & `kv_deta-0.1.8a0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kv_deta-0.1.7a0.dist-info/METADATA` & `kv_deta-0.1.8a0.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: kv-deta
-Version: 0.1.7a0
-Summary: Key-Value Model by Detabase powered
+Version: 0.1.8a0
+Summary: Key-Value Model for Detabase
 Home-page: https://github.com/ablaternae/kv-deta
 Author: d;)
 License: GLWTPL
 Keywords: deta,detabase,kv,key value
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -23,70 +23,68 @@
 
 <!-- ![Lines of code](https://img.shields.io/tokei/lines/github/ablaternae/py-kv-deta) -->
 [![PyPI version](https://badge.fury.io/py/kv-deta.svg)](https://badge.fury.io/py/kv-deta)
 ![Downloads](https://img.shields.io/pypi/dm/kv-deta)
 [![Statistic](https://pepy.tech/badge/kv-deta/week)](https://pepy.tech/project/kv-deta)
 <!-- [![GitHub](https://img.shields.io/github/license/ablaternae/kv-deta)](https://github.com/ablaternae/kv-deta/blob/trunk/LICENSE.md) -->
 
-# Key-Value Model by Detabase powered
+# Key-Value Model for Detabase
 
 ## API
 ### constructor
 `class KVModel(dict)`
-
 example:
 ```
 from kv_deta import KVModel 
 
 class Example(KVModel):
-	class Config:
-		deta_key = DETA_BASE_KEY
-		# or
-		deta = Deta(DETA_BASE_KEY)
-		#
-		table_name = "my_kv_table"	# optional
-```
+  class Config:
+    deta_key = DETA_BASE_KEY
+    # or
+    deta = Deta(DETA_BASE_KEY)
 
+    table_name = "my_kv_table"	# optional
+```
 ```
 kv = Example({"key":"value"})
 ```
 
 ### update
 like for dictionary
 ```
 kv.update({"k2":42})
 ```
 
 ### save
-commit _all_ data to detabase
+commit __all__ data to detabase
 ```
 kv.save()
 ```
 
 ### get
-mixed dict.get(key) and deta.get(key)
+mixed dict.get(key), deta.get(key), dict.setdefault(key, default)
 ```
 kv.get(key:str="some key", default="newer data")
 ```
-return value from `deta.get(key)` or update it by `default` if defined 
+return value from `deta.get(key)` or update it by `default` if value is None 
 
 
 
 ### 
 
 ## Updates
-
-* implemented `get(key,default)`
+* `get` fixed
+* implemented `get(key, default)`
 * implemented `save()`
 
-
 ## License
 * It's opensource and free software, see the [LICENSE](LICENSE) for more details
 
 ## similar projects
-* [csv-deta](https://pypi.org/project/csv-deta/)  
-* [sql-deta](https://pypi.org/project/sql-deta/) WIP
+* [csv-deta](https://pypi.org/project/csv-deta/) 
+* [sql-deta](https://pypi.org/project/sql-deta/)
 
 ## TODO
-[ ] `dec()`
-[ ] `inc()`
-[x] `get()`
+* [ ] `query()`
+* [ ] `dec()`
+* [ ] `inc()`
+* [x] `get(key)`
```

