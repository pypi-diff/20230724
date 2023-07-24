# Comparing `tmp/ops_channel-0.5.7.tar.gz` & `tmp/ops_channel-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ops_channel-0.5.7.tar", last modified: Tue May  9 06:42:02 2023, max compression
+gzip compressed data, was "ops_channel-0.5.8.tar", last modified: Mon Jul 24 05:57:36 2023, max compression
```

## Comparing `ops_channel-0.5.7.tar` & `ops_channel-0.5.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 junqiang.zhang   (510) staff       (20)        0 2023-05-09 06:42:02.167414 ops_channel-0.5.7/
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)      259 2023-05-09 06:42:02.166849 ops_channel-0.5.7/PKG-INFO
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)     2910 2021-11-29 01:44:53.000000 ops_channel-0.5.7/README.md
-drwxr-xr-x   0 junqiang.zhang   (510) staff       (20)        0 2023-05-09 06:42:02.160720 ops_channel-0.5.7/ops_channel/
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)       97 2023-04-17 02:21:10.000000 ops_channel-0.5.7/ops_channel/__init__.py
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)    99265 2023-05-09 06:40:14.000000 ops_channel-0.5.7/ops_channel/base.py
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)     5284 2023-04-20 08:22:19.000000 ops_channel-0.5.7/ops_channel/test.py
-drwxr-xr-x   0 junqiang.zhang   (510) staff       (20)        0 2023-05-09 06:42:02.165926 ops_channel-0.5.7/ops_channel.egg-info/
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)      259 2023-05-09 06:42:02.000000 ops_channel-0.5.7/ops_channel.egg-info/PKG-INFO
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)      222 2023-05-09 06:42:02.000000 ops_channel-0.5.7/ops_channel.egg-info/SOURCES.txt
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)        1 2023-05-09 06:42:02.000000 ops_channel-0.5.7/ops_channel.egg-info/dependency_links.txt
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)       12 2023-05-09 06:42:02.000000 ops_channel-0.5.7/ops_channel.egg-info/top_level.txt
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)       38 2023-05-09 06:42:02.167596 ops_channel-0.5.7/setup.cfg
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)      675 2023-05-09 06:41:23.000000 ops_channel-0.5.7/setup.py
+drwxr-xr-x   0 junqiang.zhang   (510) staff       (20)        0 2023-07-24 05:57:36.701018 ops_channel-0.5.8/
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)      259 2023-07-24 05:57:36.700486 ops_channel-0.5.8/PKG-INFO
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)     2910 2021-11-29 01:44:53.000000 ops_channel-0.5.8/README.md
+drwxr-xr-x   0 junqiang.zhang   (510) staff       (20)        0 2023-07-24 05:57:36.695164 ops_channel-0.5.8/ops_channel/
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)       97 2023-04-17 02:21:10.000000 ops_channel-0.5.8/ops_channel/__init__.py
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)    99421 2023-07-24 05:56:29.000000 ops_channel-0.5.8/ops_channel/base.py
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)     5284 2023-04-20 08:22:19.000000 ops_channel-0.5.8/ops_channel/test.py
+drwxr-xr-x   0 junqiang.zhang   (510) staff       (20)        0 2023-07-24 05:57:36.699665 ops_channel-0.5.8/ops_channel.egg-info/
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)      259 2023-07-24 05:57:36.000000 ops_channel-0.5.8/ops_channel.egg-info/PKG-INFO
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)      222 2023-07-24 05:57:36.000000 ops_channel-0.5.8/ops_channel.egg-info/SOURCES.txt
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)        1 2023-07-24 05:57:36.000000 ops_channel-0.5.8/ops_channel.egg-info/dependency_links.txt
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)       12 2023-07-24 05:57:36.000000 ops_channel-0.5.8/ops_channel.egg-info/top_level.txt
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)       38 2023-07-24 05:57:36.701217 ops_channel-0.5.8/setup.cfg
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)      675 2023-07-24 05:56:40.000000 ops_channel-0.5.8/setup.py
```

### Comparing `ops_channel-0.5.7/README.md` & `ops_channel-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `ops_channel-0.5.7/ops_channel/base.py` & `ops_channel-0.5.8/ops_channel/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1099,18 +1099,22 @@
                                      database=dsn.database,
                                      charset=charset,
                                      cursorclass=OrderedDictCursor,
                                      # local_infile=True,
                                      client_flag=CLIENT.MULTI_STATEMENTS,
                                      max_allowed_packet=1024 * 1024 * 1024)
         connection.autocommit(True)
-        # try:
-        #     self.mysql_query(connection, 'set  global max_allowed_packet=1073741824;')
-        # except Exception as er:
-        #     pass
+        try:
+            self.mysql_query(connection, 'set  global max_allowed_packet=1073741824;')
+        except Exception as er:
+            try:
+                self.mysql_query(connection, 'set  global max_allowed_packet=536870912;')
+            except Exception as er:
+                pass
+            pass
 
 
         return connection
 
     def mysql_query(self, connection, sql, *args):
         '''
         :param connection=cli.get_mysql_connection('mysql://root:root@localhost:3306/ferry'):
```

### Comparing `ops_channel-0.5.7/ops_channel/test.py` & `ops_channel-0.5.8/ops_channel/test.py`

 * *Files identical despite different names*

### Comparing `ops_channel-0.5.7/setup.py` & `ops_channel-0.5.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Created Time:  2018-11-27 19:17:34
 #############################################
 
 from setuptools import setup, find_packages
 
 setup(
     name="ops_channel",
-    version="0.5.7",
+    version="0.5.8",
     keywords=("pip", "ops_channel"),
     description="ops_channel util",
     long_description="ops_channel util",
     license="MIT Licence",
     packages=find_packages(),
     url="https://github.com/sjqzhang/ops_channel",
     author="jqzhang",
```

