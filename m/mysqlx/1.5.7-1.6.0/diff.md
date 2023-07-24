# Comparing `tmp/mysqlx-1.5.7.tar.gz` & `tmp/mysqlx-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mysqlx-1.5.7.tar", last modified: Fri Jul 21 10:08:35 2023, max compression
+gzip compressed data, was "dist\mysqlx-1.6.0.tar", last modified: Mon Jul 24 01:51:52 2023, max compression
```

## Comparing `mysqlx-1.5.7.tar` & `mysqlx-1.6.0.tar`

### file list

```diff
@@ -1,24 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 10:08:35.000000 mysqlx-1.5.7/
-drwxrwxrwx   0        0        0        0 2023-07-21 10:08:35.000000 mysqlx-1.5.7/mysqlx/
--rw-rw-rw-   0        0        0      567 2023-07-19 13:27:51.000000 mysqlx-1.5.7/mysqlx/constant.py
--rw-rw-rw-   0        0        0    17591 2023-07-19 14:03:44.000000 mysqlx-1.5.7/mysqlx/db.py
--rw-rw-rw-   0        0        0     7255 2023-07-19 13:52:43.000000 mysqlx-1.5.7/mysqlx/dbx.py
--rw-rw-rw-   0        0        0     3984 2023-07-13 13:31:18.000000 mysqlx-1.5.7/mysqlx/log_support.py
--rw-rw-rw-   0        0        0    38034 2023-07-19 13:47:01.000000 mysqlx-1.5.7/mysqlx/orm.py
--rw-rw-rw-   0        0        0     2392 2023-06-26 14:23:12.000000 mysqlx-1.5.7/mysqlx/snowflake.py
--rw-rw-rw-   0        0        0     6307 2023-07-19 13:44:39.000000 mysqlx-1.5.7/mysqlx/sql_holder.py
--rw-rw-rw-   0        0        0     4096 2023-07-19 13:45:03.000000 mysqlx-1.5.7/mysqlx/sql_mapper.py
--rw-rw-rw-   0        0        0     3408 2023-07-21 08:20:17.000000 mysqlx-1.5.7/mysqlx/sql_support.py
--rw-rw-rw-   0        0        0     4969 2023-07-19 13:40:26.000000 mysqlx-1.5.7/mysqlx/support.py
--rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.5.7/mysqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 10:08:35.000000 mysqlx-1.5.7/mysqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-21 10:08:35.000000 mysqlx-1.5.7/mysqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-21 10:08:35.000000 mysqlx-1.5.7/mysqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     4409 2023-07-21 10:08:35.000000 mysqlx-1.5.7/mysqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-07-21 10:08:35.000000 mysqlx-1.5.7/mysqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      400 2023-07-21 10:08:35.000000 mysqlx-1.5.7/mysqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-07-21 10:08:35.000000 mysqlx-1.5.7/mysqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4409 2023-07-21 10:08:35.000000 mysqlx-1.5.7/PKG-INFO
--rw-rw-rw-   0        0        0     3905 2023-07-21 10:06:40.000000 mysqlx-1.5.7/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-21 10:08:35.000000 mysqlx-1.5.7/setup.cfg
--rw-rw-rw-   0        0        0     1211 2023-07-21 10:08:06.000000 mysqlx-1.5.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 01:51:52.000000 mysqlx-1.6.0/
+drwxrwxrwx   0        0        0        0 2023-07-24 01:51:52.000000 mysqlx-1.6.0/mysqlx/
+-rw-rw-rw-   0        0        0     1083 2023-07-24 01:21:11.000000 mysqlx-1.6.0/mysqlx/db.py
+-rw-rw-rw-   0        0        0      668 2023-07-24 01:21:11.000000 mysqlx-1.6.0/mysqlx/dbx.py
+-rw-rw-rw-   0        0        0      344 2023-07-24 01:32:22.000000 mysqlx-1.6.0/mysqlx/log_support.py
+-rw-rw-rw-   0        0        0     1783 2023-07-24 01:16:32.000000 mysqlx-1.6.0/mysqlx/orm.py
+-rw-rw-rw-   0        0        0       57 2023-07-24 00:49:57.000000 mysqlx-1.6.0/mysqlx/snowflake.py
+-rw-rw-rw-   0        0        0      103 2023-07-24 00:31:03.000000 mysqlx-1.6.0/mysqlx/sql_mapper.py
+-rw-rw-rw-   0        0        0      125 2023-07-24 01:06:19.000000 mysqlx-1.6.0/mysqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 01:51:52.000000 mysqlx-1.6.0/mysqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-24 01:51:52.000000 mysqlx-1.6.0/mysqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-24 01:51:52.000000 mysqlx-1.6.0/mysqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     4410 2023-07-24 01:51:52.000000 mysqlx-1.6.0/mysqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       32 2023-07-24 01:51:52.000000 mysqlx-1.6.0/mysqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      320 2023-07-24 01:51:52.000000 mysqlx-1.6.0/mysqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-24 01:51:52.000000 mysqlx-1.6.0/mysqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4410 2023-07-24 01:51:52.000000 mysqlx-1.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3906 2023-07-24 01:17:21.000000 mysqlx-1.6.0/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-24 01:51:52.000000 mysqlx-1.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1241 2023-07-24 01:51:43.000000 mysqlx-1.6.0/setup.py
```

### Comparing `mysqlx-1.5.7/mysqlx.egg-info/PKG-INFO` & `mysqlx-1.6.0/mysqlx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlx
-Version: 1.5.7
+Version: 1.6.0
 Summary: MySqlx is a simple python sql executor for MySQL like MyBatis.
 Home-page: https://gitee.com/summry/mysqlx
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,MyBatis,python
 Platform: UNKNOWN
@@ -104,15 +104,15 @@
        
        users = db.select('select id, name, age from user where name=?', 'zhangsan')
        # result:
        # (3, 'zhangsan', 15)
        
        # you can use orm to operate a single table
        class User(Model):
-           __pk__ = 'id'
+           __key__ = 'id'
            __table__ = 'user'
 
            def __init__(self, id: int = None, name: str = None, age: int = None):
                self.id = id
                self.name = name
                self.age = age
```

### Comparing `mysqlx-1.5.7/PKG-INFO` & `mysqlx-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlx
-Version: 1.5.7
+Version: 1.6.0
 Summary: MySqlx is a simple python sql executor for MySQL like MyBatis.
 Home-page: https://gitee.com/summry/mysqlx
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,MyBatis,python
 Platform: UNKNOWN
@@ -104,15 +104,15 @@
        
        users = db.select('select id, name, age from user where name=?', 'zhangsan')
        # result:
        # (3, 'zhangsan', 15)
        
        # you can use orm to operate a single table
        class User(Model):
-           __pk__ = 'id'
+           __key__ = 'id'
            __table__ = 'user'
 
            def __init__(self, id: int = None, name: str = None, age: int = None):
                self.id = id
                self.name = name
                self.age = age
```

### Comparing `mysqlx-1.5.7/README.rst` & `mysqlx-1.6.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -91,15 +91,15 @@
        
        users = db.select('select id, name, age from user where name=?', 'zhangsan')
        # result:
        # (3, 'zhangsan', 15)
        
        # you can use orm to operate a single table
        class User(Model):
-           __pk__ = 'id'
+           __key__ = 'id'
            __table__ = 'user'
 
            def __init__(self, id: int = None, name: str = None, age: int = None):
                self.id = id
                self.name = name
                self.age = age
```

### Comparing `mysqlx-1.5.7/setup.py` & `mysqlx-1.6.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,17 +15,18 @@
     name='mysqlx',
     packages=['mysqlx'],
     description="MySqlx is a simple python sql executor for MySQL like MyBatis.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=2.7.0',
+        'sqlx-batis>=0.0.7',
         # 'mysql-connector-python>=8.0.13',
     ],
-    version='1.5.7',
+    version='1.6.0',
     url='https://gitee.com/summry/mysqlx',
     author='summry',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

