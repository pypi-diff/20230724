# Comparing `tmp/fastmysql-0.1.0.tar.gz` & `tmp/fastmysql-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastmysql-0.1.0.tar", last modified: Fri Jul 14 08:50:17 2023, max compression
+gzip compressed data, was "fastmysql-0.1.1.tar", last modified: Mon Jul 24 10:15:49 2023, max compression
```

## Comparing `fastmysql-0.1.0.tar` & `fastmysql-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-14 08:50:17.427523 fastmysql-0.1.0/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1775 2023-07-14 08:50:17.427429 fastmysql-0.1.0/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1442 2023-02-22 07:55:41.000000 fastmysql-0.1.0/README.md
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-14 08:50:17.426395 fastmysql-0.1.0/fastmysql/
--rw-r--r--   0 zeroseeker   (501) staff       (20)      208 2023-02-22 07:55:41.000000 fastmysql-0.1.0/fastmysql/__init__.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    47513 2023-07-14 08:48:57.000000 fastmysql-0.1.0/fastmysql/fastmysql.py
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-14 08:50:17.427277 fastmysql-0.1.0/fastmysql.egg-info/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1775 2023-07-14 08:50:17.000000 fastmysql-0.1.0/fastmysql.egg-info/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      227 2023-07-14 08:50:17.000000 fastmysql-0.1.0/fastmysql.egg-info/SOURCES.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2023-07-14 08:50:17.000000 fastmysql-0.1.0/fastmysql.egg-info/dependency_links.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)      131 2023-07-14 08:50:17.000000 fastmysql-0.1.0/fastmysql.egg-info/requires.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       10 2023-07-14 08:50:17.000000 fastmysql-0.1.0/fastmysql.egg-info/top_level.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2023-07-14 08:50:17.427557 fastmysql-0.1.0/setup.cfg
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1076 2023-07-14 08:49:36.000000 fastmysql-0.1.0/setup.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-24 10:15:49.469204 fastmysql-0.1.1/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1775 2023-07-24 10:15:49.469074 fastmysql-0.1.1/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1442 2023-02-22 07:55:41.000000 fastmysql-0.1.1/README.md
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-24 10:15:49.467171 fastmysql-0.1.1/fastmysql/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      208 2023-02-22 07:55:41.000000 fastmysql-0.1.1/fastmysql/__init__.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    47561 2023-07-24 10:15:15.000000 fastmysql-0.1.1/fastmysql/fastmysql.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-24 10:15:49.468894 fastmysql-0.1.1/fastmysql.egg-info/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1775 2023-07-24 10:15:49.000000 fastmysql-0.1.1/fastmysql.egg-info/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      227 2023-07-24 10:15:49.000000 fastmysql-0.1.1/fastmysql.egg-info/SOURCES.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2023-07-24 10:15:49.000000 fastmysql-0.1.1/fastmysql.egg-info/dependency_links.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      131 2023-07-24 10:15:49.000000 fastmysql-0.1.1/fastmysql.egg-info/requires.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       10 2023-07-24 10:15:49.000000 fastmysql-0.1.1/fastmysql.egg-info/top_level.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2023-07-24 10:15:49.469246 fastmysql-0.1.1/setup.cfg
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1076 2023-07-24 10:15:15.000000 fastmysql-0.1.1/setup.py
```

### Comparing `fastmysql-0.1.0/PKG-INFO` & `fastmysql-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastmysql
-Version: 0.1.0
+Version: 0.1.1
 Summary: make it easy to use pymysql
 Home-page: https://gitee.com/ZeroSeeker/fastmysql
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `fastmysql-0.1.0/README.md` & `fastmysql-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `fastmysql-0.1.0/fastmysql/fastmysql.py` & `fastmysql-0.1.1/fastmysql/fastmysql.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,16 @@
                 showlog.info(f'User [{username}] are trying to connect to the database [{db_name}] ...')
             con = pymysql.connect(
                 host=host,
                 db=db_name,
                 user=username,
                 passwd=password,
                 port=port,
-                charset=charset
+                charset=charset,
+                connect_timeout=reconnect_wait
             )
             if ssc is False:
                 cur = con.cursor()
             else:
                 cur = pymysql.cursors.SSCursor(con)  # 使用流式游标
             cur.execute(query='SET NAMES utf8mb4')
             cur.execute(query='SET CHARACTER SET utf8mb4')
```

### Comparing `fastmysql-0.1.0/fastmysql.egg-info/PKG-INFO` & `fastmysql-0.1.1/fastmysql.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastmysql
-Version: 0.1.0
+Version: 0.1.1
 Summary: make it easy to use pymysql
 Home-page: https://gitee.com/ZeroSeeker/fastmysql
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `fastmysql-0.1.0/setup.py` & `fastmysql-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fastmysql",
-    version="0.1.0",
+    version="0.1.1",
     author="ZeroSeeker",
     author_email="zeroseeker@foxmail.com",
     description="make it easy to use pymysql",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/ZeroSeeker/fastmysql",
     packages=setuptools.find_packages(),
```

