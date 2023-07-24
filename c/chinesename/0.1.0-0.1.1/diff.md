# Comparing `tmp/chinesename-0.1.0.tar.gz` & `tmp/chinesename-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/chinesename-0.1.0.tar", last modified: Fri Nov 23 08:47:13 2018, max compression
+gzip compressed data, was "dist/chinesename-0.1.1.tar", last modified: Mon Jul 24 14:03:58 2023, max compression
```

## Comparing `chinesename-0.1.0.tar` & `chinesename-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 QMP        (501) admin       (80)        0 2018-11-23 08:47:13.000000 chinesename-0.1.0/
-drwxr-xr-x   0 QMP        (501) admin       (80)        0 2018-11-23 08:47:13.000000 chinesename-0.1.0/chinesename/
--rw-r--r--   0 QMP        (501) admin       (80)      162 2018-06-20 13:12:54.000000 chinesename-0.1.0/chinesename/__init__.py
--rw-r--r--   0 QMP        (501) admin       (80)     6496 2018-07-23 01:38:48.000000 chinesename-0.1.0/chinesename/chinesename.py
-drwxr-xr-x   0 QMP        (501) admin       (80)        0 2018-11-23 08:47:13.000000 chinesename-0.1.0/chinesename/source/
--rw-r--r--   0 QMP        (501) admin       (80)    50795 2018-06-20 09:58:13.000000 chinesename-0.1.0/chinesename/source/boy.json
--rw-r--r--   0 QMP        (501) admin       (80)    11334 2018-06-20 11:37:04.000000 chinesename-0.1.0/chinesename/source/firstnames.txt
--rw-r--r--   0 QMP        (501) admin       (80)    43406 2018-06-20 09:58:13.000000 chinesename-0.1.0/chinesename/source/girl.json
--rw-r--r--   0 QMP        (501) admin       (80)   250926 2018-06-20 07:52:12.000000 chinesename-0.1.0/chinesename/source/gushiwen.json
--rw-r--r--   0 QMP        (501) admin       (80)     2195 2018-06-20 08:49:00.000000 chinesename-0.1.0/chinesename/source/lastnames.txt
-drwxr-xr-x   0 QMP        (501) admin       (80)        0 2018-11-23 08:47:13.000000 chinesename-0.1.0/chinesename.egg-info/
--rw-r--r--   0 QMP        (501) admin       (80)        1 2018-11-23 08:47:13.000000 chinesename-0.1.0/chinesename.egg-info/dependency_links.txt
--rw-r--r--   0 QMP        (501) admin       (80)     3004 2018-11-23 08:47:13.000000 chinesename-0.1.0/chinesename.egg-info/PKG-INFO
--rw-r--r--   0 QMP        (501) admin       (80)      367 2018-11-23 08:47:13.000000 chinesename-0.1.0/chinesename.egg-info/SOURCES.txt
--rw-r--r--   0 QMP        (501) admin       (80)       12 2018-11-23 08:47:13.000000 chinesename-0.1.0/chinesename.egg-info/top_level.txt
--rw-r--r--   0 QMP        (501) admin       (80)     3004 2018-11-23 08:47:13.000000 chinesename-0.1.0/PKG-INFO
--rw-r--r--   0 QMP        (501) admin       (80)     2037 2018-11-23 08:47:13.000000 chinesename-0.1.0/README.rst
--rw-r--r--   0 QMP        (501) admin       (80)       59 2018-11-23 08:47:13.000000 chinesename-0.1.0/setup.cfg
--rw-r--r--   0 QMP        (501) admin       (80)     1395 2018-11-23 08:46:35.000000 chinesename-0.1.0/setup.py
+drwxr-xr-x   0 hina       (501) staff       (20)        0 2023-07-24 14:03:58.000000 chinesename-0.1.1/
+-rwxr-xr-x   0 hina       (501) staff       (20)       55 2023-07-24 14:02:23.000000 chinesename-0.1.1/MANIFEST.in
+-rw-r--r--   0 hina       (501) staff       (20)     3093 2023-07-24 14:03:58.000000 chinesename-0.1.1/PKG-INFO
+-rw-r--r--   0 hina       (501) staff       (20)     2015 2023-07-24 13:56:57.000000 chinesename-0.1.1/README.md
+drwxr-xr-x   0 hina       (501) staff       (20)        0 2023-07-24 14:03:58.000000 chinesename-0.1.1/chinesename/
+-rw-r--r--   0 hina       (501) staff       (20)      162 2023-07-24 13:47:56.000000 chinesename-0.1.1/chinesename/__init__.py
+-rw-r--r--   0 hina       (501) staff       (20)     6039 2023-07-24 13:56:07.000000 chinesename-0.1.1/chinesename/chinesename.py
+drwxr-xr-x   0 hina       (501) staff       (20)        0 2023-07-24 14:03:58.000000 chinesename-0.1.1/chinesename/source/
+-rw-r--r--   0 hina       (501) staff       (20)    50795 2023-07-24 13:47:56.000000 chinesename-0.1.1/chinesename/source/boy.json
+-rw-r--r--   0 hina       (501) staff       (20)    11334 2023-07-24 13:47:56.000000 chinesename-0.1.1/chinesename/source/firstnames.txt
+-rw-r--r--   0 hina       (501) staff       (20)    43406 2023-07-24 13:47:56.000000 chinesename-0.1.1/chinesename/source/girl.json
+-rw-r--r--   0 hina       (501) staff       (20)   250926 2023-07-24 13:47:56.000000 chinesename-0.1.1/chinesename/source/gushiwen.json
+-rw-r--r--   0 hina       (501) staff       (20)     2195 2023-07-24 13:47:56.000000 chinesename-0.1.1/chinesename/source/lastnames.txt
+drwxr-xr-x   0 hina       (501) staff       (20)        0 2023-07-24 14:03:58.000000 chinesename-0.1.1/chinesename.egg-info/
+-rw-r--r--   0 hina       (501) staff       (20)     3093 2023-07-24 14:03:58.000000 chinesename-0.1.1/chinesename.egg-info/PKG-INFO
+-rw-r--r--   0 hina       (501) staff       (20)      408 2023-07-24 14:03:58.000000 chinesename-0.1.1/chinesename.egg-info/SOURCES.txt
+-rw-r--r--   0 hina       (501) staff       (20)        1 2023-07-24 14:03:58.000000 chinesename-0.1.1/chinesename.egg-info/dependency_links.txt
+-rw-r--r--   0 hina       (501) staff       (20)       18 2023-07-24 14:03:58.000000 chinesename-0.1.1/chinesename.egg-info/top_level.txt
+-rw-r--r--   0 hina       (501) staff       (20)        1 2023-07-24 14:00:01.000000 chinesename-0.1.1/chinesename.egg-info/zip-safe
+-rw-r--r--   0 hina       (501) staff       (20)       38 2023-07-24 14:03:58.000000 chinesename-0.1.1/setup.cfg
+-rw-r--r--   0 hina       (501) staff       (20)     2416 2023-07-24 14:01:02.000000 chinesename-0.1.1/setup.py
```

### Comparing `chinesename-0.1.0/chinesename/chinesename.py` & `chinesename-0.1.1/chinesename/chinesename.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,22 +195,7 @@
             lastname： 姓氏，默认随机 - String
             sex: {str} 性别(boy | girl)
         Returns:
             Yield：姓名生成器
         """
         for i in range(count):
             yield self.getName(char_count, lastname, sex)
-        
-
-def main():
-    chinesename = ChineseName()     # 初始化，可以指定姓氏文件
-    name = chinesename.getName(lastname="白", sex="boy")  # 获取一个姓名
-    print(name)
-    names=chinesename.getNames(100,char_count=2,lastname="彭")   # 获取一个姓名列表
-    print(names)
-
-    # 获取一个姓名生成器
-    name_generator = chinesename.getNameGenerator(10)
-    print(name_generator)
-
-if __name__ == '__main__':
-    main()
```

### Comparing `chinesename-0.1.0/chinesename/source/boy.json` & `chinesename-0.1.1/chinesename/source/boy.json`

 * *Files identical despite different names*

### Comparing `chinesename-0.1.0/chinesename/source/firstnames.txt` & `chinesename-0.1.1/chinesename/source/firstnames.txt`

 * *Files identical despite different names*

### Comparing `chinesename-0.1.0/chinesename/source/girl.json` & `chinesename-0.1.1/chinesename/source/girl.json`

 * *Files identical despite different names*

### Comparing `chinesename-0.1.0/chinesename/source/gushiwen.json` & `chinesename-0.1.1/chinesename/source/gushiwen.json`

 * *Files identical despite different names*

### Comparing `chinesename-0.1.0/chinesename/source/lastnames.txt` & `chinesename-0.1.1/chinesename/source/lastnames.txt`

 * *Files identical despite different names*

