# Comparing `tmp/mwsqlite-1.2.3.tar.gz` & `tmp/mwsqlite-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mwsqlite-1.2.3.tar", last modified: Tue Jul 11 11:00:06 2023, max compression
+gzip compressed data, was "dist\mwsqlite-1.3.0.tar", last modified: Mon Jul 24 08:45:01 2023, max compression
```

## Comparing `mwsqlite-1.2.3.tar` & `mwsqlite-1.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 11:00:06.830474 mwsqlite-1.2.3/
--rw-rw-rw-   0        0        0     1088 2022-10-20 18:54:22.000000 mwsqlite-1.2.3/LICENSE
--rw-rw-rw-   0        0        0     3172 2023-07-11 11:00:06.831475 mwsqlite-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     2075 2022-12-19 15:39:05.000000 mwsqlite-1.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 11:00:06.805468 mwsqlite-1.2.3/mwsqlite/
--rw-rw-rw-   0        0        0      186 2022-12-19 10:39:07.000000 mwsqlite-1.2.3/mwsqlite/__init__.py
--rw-rw-rw-   0        0        0     1979 2023-07-11 10:59:01.000000 mwsqlite-1.2.3/mwsqlite/_types.py
--rw-rw-rw-   0        0        0    14773 2023-06-26 20:56:30.000000 mwsqlite-1.2.3/mwsqlite/mw_sql.py
--rw-rw-rw-   0        0        0     3388 2022-12-23 15:06:08.000000 mwsqlite-1.2.3/mwsqlite/sql_compile.py
--rw-rw-rw-   0        0        0      551 2022-12-23 17:48:26.000000 mwsqlite-1.2.3/mwsqlite/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-11 11:00:06.829473 mwsqlite-1.2.3/mwsqlite.egg-info/
--rw-rw-rw-   0        0        0     3172 2023-07-11 11:00:06.000000 mwsqlite-1.2.3/mwsqlite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-07-11 11:00:06.000000 mwsqlite-1.2.3/mwsqlite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 11:00:06.000000 mwsqlite-1.2.3/mwsqlite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-11 11:00:06.000000 mwsqlite-1.2.3/mwsqlite.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-07-11 11:00:06.000000 mwsqlite-1.2.3/mwsqlite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 11:00:06.832717 mwsqlite-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1666 2023-07-11 10:56:50.000000 mwsqlite-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 08:45:01.933732 mwsqlite-1.3.0/
+-rw-rw-rw-   0        0        0     1088 2022-10-20 18:54:22.000000 mwsqlite-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0     3172 2023-07-24 08:45:01.934733 mwsqlite-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2075 2022-12-19 15:39:05.000000 mwsqlite-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 08:45:01.911728 mwsqlite-1.3.0/mwsqlite/
+-rw-rw-rw-   0        0        0      209 2023-07-24 07:45:57.000000 mwsqlite-1.3.0/mwsqlite/__init__.py
+-rw-rw-rw-   0        0        0     2405 2023-07-24 07:30:17.000000 mwsqlite-1.3.0/mwsqlite/_types.py
+-rw-rw-rw-   0        0        0    14212 2023-07-24 07:45:25.000000 mwsqlite-1.3.0/mwsqlite/mw_sql.py
+-rw-rw-rw-   0        0        0     3388 2022-12-23 15:06:08.000000 mwsqlite-1.3.0/mwsqlite/sql_compile.py
+-rw-rw-rw-   0        0        0      551 2022-12-23 17:48:26.000000 mwsqlite-1.3.0/mwsqlite/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-24 08:45:01.932732 mwsqlite-1.3.0/mwsqlite.egg-info/
+-rw-rw-rw-   0        0        0     3172 2023-07-24 08:45:01.000000 mwsqlite-1.3.0/mwsqlite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-07-24 08:45:01.000000 mwsqlite-1.3.0/mwsqlite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 08:45:01.000000 mwsqlite-1.3.0/mwsqlite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-24 08:45:01.000000 mwsqlite-1.3.0/mwsqlite.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-07-24 08:45:01.000000 mwsqlite-1.3.0/mwsqlite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 08:45:01.939734 mwsqlite-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1666 2023-07-24 07:46:27.000000 mwsqlite-1.3.0/setup.py
```

### Comparing `mwsqlite-1.2.3/LICENSE` & `mwsqlite-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mwsqlite-1.2.3/PKG-INFO` & `mwsqlite-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mwsqlite
-Version: 1.2.3
+Version: 1.3.0
 Summary: Simply python library for interact with (EOSIO) WAX blockchain
 Home-page: https://github.com/makarworld/mwsqlite.git
-Download-URL: https://github.com/makarworld/mwsqlite/archive/refs/tags/v1.2.3.zip
+Download-URL: https://github.com/makarworld/mwsqlite/archive/refs/tags/v1.3.0.zip
 Author: abuztrade
 Author-email: abuztrade.work@gmail.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Communications :: Email
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mwsqlite-1.2.3/README.md` & `mwsqlite-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `mwsqlite-1.2.3/mwsqlite/_types.py` & `mwsqlite-1.3.0/mwsqlite/_types.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 class Order(dict):
     pass
 
 class Limit(int):
     pass
 
 
-class Struct:
+class __Struct:
     def __init__(self, _list=[], **entries):
         if _list:
             self.new_list = []
             for x in _list:
                 if isinstance(x, dict):
                     self.new_list.append(Struct(**x))
 
@@ -73,9 +73,23 @@
 
     def items(self):
         return self.__dict__.items()
     
     def get(self, key):
         return self.__dict__.get(key)
 
+class Struct(dict):
+    __setattr__ = dict.__setitem__
+    __delattr__ = dict.__delitem__
+
+    def __getattr__(cls, key):
+        item = cls.get(key)
+        if isinstance(item, dict):
+            item = Struct(**item)
+        elif isinstance(item, list):
+            for i in range(len(item)):
+                if isinstance(item[i], dict):
+                    item[i] = Struct(**item[i])
+        return item
+
 class InvalidColumnNameError(Exception):
     pass
```

### Comparing `mwsqlite-1.2.3/mwsqlite/mw_sql.py` & `mwsqlite-1.3.0/mwsqlite/mw_sql.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,34 +29,15 @@
             cursor = connection.cursor()
             res = func(cursor=cursor, *args, **kwargs)
             connection.commit()
         return res
            
     return inner
     
-    
-def check_list(lst: list):
-    for i in range(len(lst)):
-        if isinstance(lst[i], Row) or isinstance(lst[i], Struct):
-            lst[i] = check_dict(lst[i].dict())
-        elif isinstance(lst[i], list):
-            lst[i] = check_list(lst[i])
-    return lst
-
-def check_dict(dct: dict):
-    for k, v in dct.items():
-        if isinstance(v, Row) or isinstance(v, Struct):
-            dct[k] = check_dict(v.dict())
-        elif isinstance(v, list):
-            dct[k] = check_list(v)
-    return dct
-
 def check_kwargs(kwargs: dict):
-    kwargs = check_dict(kwargs)
-
     for k, v in kwargs.items():
         if isinstance(v, list) or isinstance(v, dict):
             kwargs[k] = json.dumps(v, separators = (',', ':'))
     
     return kwargs
```

### Comparing `mwsqlite-1.2.3/mwsqlite/sql_compile.py` & `mwsqlite-1.3.0/mwsqlite/sql_compile.py`

 * *Files identical despite different names*

### Comparing `mwsqlite-1.2.3/mwsqlite/utils.py` & `mwsqlite-1.3.0/mwsqlite/utils.py`

 * *Files identical despite different names*

### Comparing `mwsqlite-1.2.3/mwsqlite.egg-info/PKG-INFO` & `mwsqlite-1.3.0/mwsqlite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mwsqlite
-Version: 1.2.3
+Version: 1.3.0
 Summary: Simply python library for interact with (EOSIO) WAX blockchain
 Home-page: https://github.com/makarworld/mwsqlite.git
-Download-URL: https://github.com/makarworld/mwsqlite/archive/refs/tags/v1.2.3.zip
+Download-URL: https://github.com/makarworld/mwsqlite/archive/refs/tags/v1.3.0.zip
 Author: abuztrade
 Author-email: abuztrade.work@gmail.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Communications :: Email
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mwsqlite-1.2.3/setup.py` & `mwsqlite-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 :author: abuztrade
 :license: MIT License, see LICENSE file.
 :copyright: (c) 2022 by abuztrade.
 """
 
 
-version = '1.2.3'
+version = '1.3.0'
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="mwsqlite",
     version=version,
```

