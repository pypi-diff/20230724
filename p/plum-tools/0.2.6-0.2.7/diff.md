# Comparing `tmp/plum_tools-0.2.6.tar.gz` & `tmp/plum_tools-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/plum_tools-0.2.6.tar", last modified: Wed Feb 23 04:04:21 2022, max compression
+gzip compressed data, was "plum_tools-0.2.7.tar", last modified: Mon Jul 24 10:50:08 2023, max compression
```

## Comparing `plum_tools-0.2.6.tar` & `plum_tools-0.2.7.tar`

### file list

```diff
@@ -1,43 +1,51 @@
-drwxr-xr-x   0 seekplum   (501) staff       (20)        0 2022-02-23 04:04:21.000000 plum_tools-0.2.6/
--rw-r--r--   0 seekplum   (501) staff       (20)    11357 2020-10-21 14:56:05.000000 plum_tools-0.2.6/LICENSE
--rw-r--r--   0 seekplum   (501) staff       (20)      163 2020-10-21 14:56:18.000000 plum_tools-0.2.6/MANIFEST.in
--rw-r--r--   0 seekplum   (501) staff       (20)      516 2022-02-23 04:04:21.000000 plum_tools-0.2.6/PKG-INFO
--rw-r--r--   0 seekplum   (501) staff       (20)     6143 2020-10-21 14:56:18.000000 plum_tools-0.2.6/README.md
--rw-r--r--   0 seekplum   (501) staff       (20)        6 2022-02-23 04:02:52.000000 plum_tools-0.2.6/VERSION
-drwxr-xr-x   0 seekplum   (501) staff       (20)        0 2022-02-23 04:04:21.000000 plum_tools-0.2.6/bin/
--rw-r--r--   0 seekplum   (501) staff       (20)        0 2020-10-21 14:56:05.000000 plum_tools-0.2.6/bin/.gitkeep
-drwxr-xr-x   0 seekplum   (501) staff       (20)        0 2022-02-23 04:04:21.000000 plum_tools-0.2.6/plum_tools/
--rw-r--r--   0 seekplum   (501) staff       (20)      378 2020-10-21 14:34:23.000000 plum_tools-0.2.6/plum_tools/.plum_tools.yaml
--rw-r--r--   0 seekplum   (501) staff       (20)      406 2022-02-10 08:47:39.000000 plum_tools-0.2.6/plum_tools/__init__.py
--rw-r--r--   0 seekplum   (501) staff       (20)      866 2020-10-24 07:43:31.000000 plum_tools-0.2.6/plum_tools/compat.py
--rw-r--r--   0 seekplum   (501) staff       (20)     3703 2022-02-23 04:02:52.000000 plum_tools-0.2.6/plum_tools/conf.py
--rw-r--r--   0 seekplum   (501) staff       (20)     1028 2020-10-21 14:34:23.000000 plum_tools-0.2.6/plum_tools/exceptions.py
--rw-r--r--   0 seekplum   (501) staff       (20)     3766 2021-01-27 14:54:26.000000 plum_tools-0.2.6/plum_tools/gitrepo.py
--rw-r--r--   0 seekplum   (501) staff       (20)     3806 2020-10-21 14:34:23.000000 plum_tools-0.2.6/plum_tools/gitstash.py
--rw-r--r--   0 seekplum   (501) staff       (20)    11818 2022-02-10 07:47:52.000000 plum_tools-0.2.6/plum_tools/pipmi.py
--rw-r--r--   0 seekplum   (501) staff       (20)     2159 2021-04-27 02:37:03.000000 plum_tools-0.2.6/plum_tools/pping.py
--rw-r--r--   0 seekplum   (501) staff       (20)    13161 2022-02-23 04:01:20.000000 plum_tools-0.2.6/plum_tools/prn.py
--rw-r--r--   0 seekplum   (501) staff       (20)     3470 2021-01-27 14:53:33.000000 plum_tools-0.2.6/plum_tools/pssh.py
-drwxr-xr-x   0 seekplum   (501) staff       (20)        0 2022-02-23 04:04:21.000000 plum_tools-0.2.6/plum_tools/utils/
--rw-r--r--   0 seekplum   (501) staff       (20)      410 2020-06-12 09:42:18.000000 plum_tools-0.2.6/plum_tools/utils/__init__.py
--rw-r--r--   0 seekplum   (501) staff       (20)     2658 2020-10-21 04:37:31.000000 plum_tools-0.2.6/plum_tools/utils/git.py
--rw-r--r--   0 seekplum   (501) staff       (20)     2252 2020-06-12 09:42:18.000000 plum_tools-0.2.6/plum_tools/utils/printer.py
--rw-r--r--   0 seekplum   (501) staff       (20)     6848 2020-10-21 14:34:23.000000 plum_tools-0.2.6/plum_tools/utils/sshconf.py
--rw-r--r--   0 seekplum   (501) staff       (20)     6226 2022-02-23 03:59:13.000000 plum_tools-0.2.6/plum_tools/utils/utils.py
-drwxr-xr-x   0 seekplum   (501) staff       (20)        0 2022-02-23 04:04:21.000000 plum_tools-0.2.6/plum_tools.egg-info/
--rw-r--r--   0 seekplum   (501) staff       (20)      516 2022-02-23 04:04:21.000000 plum_tools-0.2.6/plum_tools.egg-info/PKG-INFO
--rw-r--r--   0 seekplum   (501) staff       (20)      821 2022-02-23 04:04:21.000000 plum_tools-0.2.6/plum_tools.egg-info/SOURCES.txt
--rw-r--r--   0 seekplum   (501) staff       (20)        1 2022-02-23 04:04:21.000000 plum_tools-0.2.6/plum_tools.egg-info/dependency_links.txt
--rw-r--r--   0 seekplum   (501) staff       (20)      203 2022-02-23 04:04:21.000000 plum_tools-0.2.6/plum_tools.egg-info/entry_points.txt
--rw-r--r--   0 seekplum   (501) staff       (20)       11 2022-02-23 04:04:21.000000 plum_tools-0.2.6/plum_tools.egg-info/namespace_packages.txt
--rw-r--r--   0 seekplum   (501) staff       (20)       36 2022-02-23 04:04:21.000000 plum_tools-0.2.6/plum_tools.egg-info/requires.txt
--rw-r--r--   0 seekplum   (501) staff       (20)       17 2022-02-23 04:04:21.000000 plum_tools-0.2.6/plum_tools.egg-info/top_level.txt
--rw-r--r--   0 seekplum   (501) staff       (20)      424 2022-02-23 04:04:21.000000 plum_tools-0.2.6/setup.cfg
--rw-r--r--   0 seekplum   (501) staff       (20)     1668 2022-02-23 04:02:52.000000 plum_tools-0.2.6/setup.py
-drwxr-xr-x   0 seekplum   (501) staff       (20)        0 2022-02-23 04:04:21.000000 plum_tools-0.2.6/tests/
-drwxr-xr-x   0 seekplum   (501) staff       (20)        0 2022-02-23 04:04:21.000000 plum_tools-0.2.6/tests/utils/
--rw-r--r--   0 seekplum   (501) staff       (20)      375 2020-06-12 09:42:18.000000 plum_tools-0.2.6/tests/utils/__init__.py
--rw-r--r--   0 seekplum   (501) staff       (20)     3378 2021-01-05 04:56:20.000000 plum_tools-0.2.6/tests/utils/test_git.py
--rw-r--r--   0 seekplum   (501) staff       (20)     3174 2021-01-05 04:56:20.000000 plum_tools-0.2.6/tests/utils/test_printer.py
--rw-r--r--   0 seekplum   (501) staff       (20)     7356 2021-01-05 04:56:20.000000 plum_tools-0.2.6/tests/utils/test_sshconf.py
--rw-r--r--   0 seekplum   (501) staff       (20)      415 2020-06-12 09:42:18.000000 plum_tools-0.2.6/tests/utils/test_utils.py
+drwxr-xr-x   0 seekplum  (1000) seekplum  (1000)        0 2023-07-24 10:50:08.644510 plum_tools-0.2.7/
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)    11357 2020-10-21 14:56:05.000000 plum_tools-0.2.7/LICENSE
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)      163 2020-10-21 14:56:18.000000 plum_tools-0.2.7/MANIFEST.in
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)      452 2023-07-24 10:50:08.644510 plum_tools-0.2.7/PKG-INFO
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)     6143 2020-10-21 14:56:18.000000 plum_tools-0.2.7/README.md
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)        6 2023-07-24 10:47:21.000000 plum_tools-0.2.7/VERSION
+drwxr-xr-x   0 seekplum  (1000) seekplum  (1000)        0 2023-07-24 10:50:08.644510 plum_tools-0.2.7/bin/
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)        0 2020-10-21 14:56:05.000000 plum_tools-0.2.7/bin/.gitkeep
+drwxr-xr-x   0 seekplum  (1000) seekplum  (1000)        0 2023-07-24 10:50:08.644510 plum_tools-0.2.7/plum_tools/
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)      378 2020-10-21 14:34:23.000000 plum_tools-0.2.7/plum_tools/.plum_tools.yaml
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)      406 2022-02-10 08:47:39.000000 plum_tools-0.2.7/plum_tools/__init__.py
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)      866 2020-10-24 07:43:31.000000 plum_tools-0.2.7/plum_tools/compat.py
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)     3703 2023-07-24 10:47:21.000000 plum_tools-0.2.7/plum_tools/conf.py
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)     1028 2020-10-21 14:34:23.000000 plum_tools-0.2.7/plum_tools/exceptions.py
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)     3766 2021-01-27 14:54:26.000000 plum_tools-0.2.7/plum_tools/gitrepo.py
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)     3806 2020-10-21 14:34:23.000000 plum_tools-0.2.7/plum_tools/gitstash.py
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)    11818 2022-02-10 07:47:52.000000 plum_tools-0.2.7/plum_tools/pipmi.py
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)     2159 2021-04-27 02:37:03.000000 plum_tools-0.2.7/plum_tools/pping.py
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)    13161 2023-07-24 10:45:28.000000 plum_tools-0.2.7/plum_tools/prn.py
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)     3470 2021-01-27 14:53:33.000000 plum_tools-0.2.7/plum_tools/pssh.py
+drwxr-xr-x   0 seekplum  (1000) seekplum  (1000)        0 2023-07-24 10:50:08.644510 plum_tools-0.2.7/plum_tools/utils/
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)      410 2020-06-12 09:42:18.000000 plum_tools-0.2.7/plum_tools/utils/__init__.py
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)     2658 2020-10-21 04:37:31.000000 plum_tools-0.2.7/plum_tools/utils/git.py
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)     2252 2020-06-12 09:42:18.000000 plum_tools-0.2.7/plum_tools/utils/printer.py
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)     6848 2020-10-21 14:34:23.000000 plum_tools-0.2.7/plum_tools/utils/sshconf.py
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)     6224 2023-07-24 09:34:24.000000 plum_tools-0.2.7/plum_tools/utils/utils.py
+drwxr-xr-x   0 seekplum  (1000) seekplum  (1000)        0 2023-07-24 10:50:08.644510 plum_tools-0.2.7/plum_tools.egg-info/
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)      452 2023-07-24 10:50:08.000000 plum_tools-0.2.7/plum_tools.egg-info/PKG-INFO
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)      981 2023-07-24 10:50:08.000000 plum_tools-0.2.7/plum_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)        1 2023-07-24 10:50:08.000000 plum_tools-0.2.7/plum_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)      202 2023-07-24 10:50:08.000000 plum_tools-0.2.7/plum_tools.egg-info/entry_points.txt
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)       11 2023-07-24 10:50:08.000000 plum_tools-0.2.7/plum_tools.egg-info/namespace_packages.txt
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)       36 2023-07-24 10:50:08.000000 plum_tools-0.2.7/plum_tools.egg-info/requires.txt
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)       17 2023-07-24 10:50:08.000000 plum_tools-0.2.7/plum_tools.egg-info/top_level.txt
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)      424 2023-07-24 10:50:08.644510 plum_tools-0.2.7/setup.cfg
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)     1668 2023-07-24 10:47:21.000000 plum_tools-0.2.7/setup.py
+drwxr-xr-x   0 seekplum  (1000) seekplum  (1000)        0 2023-07-24 10:50:08.644510 plum_tools-0.2.7/tests/
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)     5824 2021-01-05 04:56:20.000000 plum_tools-0.2.7/tests/test_conf.py
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)     7855 2021-04-27 02:37:31.000000 plum_tools-0.2.7/tests/test_gitrepo.py
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)     1442 2021-04-27 02:36:15.000000 plum_tools-0.2.7/tests/test_gitstash.py
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)      403 2021-01-05 04:56:20.000000 plum_tools-0.2.7/tests/test_main.py
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)      408 2020-06-12 09:42:18.000000 plum_tools-0.2.7/tests/test_pipmi.py
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)     2742 2021-04-27 02:35:44.000000 plum_tools-0.2.7/tests/test_pping.py
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)     7797 2023-07-24 10:47:17.000000 plum_tools-0.2.7/tests/test_prn.py
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)     2375 2021-01-27 14:52:08.000000 plum_tools-0.2.7/tests/test_pssh.py
+drwxr-xr-x   0 seekplum  (1000) seekplum  (1000)        0 2023-07-24 10:50:08.644510 plum_tools-0.2.7/tests/utils/
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)      375 2020-06-12 09:42:18.000000 plum_tools-0.2.7/tests/utils/__init__.py
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)     3378 2021-01-05 04:56:20.000000 plum_tools-0.2.7/tests/utils/test_git.py
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)     3174 2021-01-05 04:56:20.000000 plum_tools-0.2.7/tests/utils/test_printer.py
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)     7356 2021-01-05 04:56:20.000000 plum_tools-0.2.7/tests/utils/test_sshconf.py
+-rw-r--r--   0 seekplum  (1000) seekplum  (1000)      415 2020-06-12 09:42:18.000000 plum_tools-0.2.7/tests/utils/test_utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `plum_tools-0.2.6/LICENSE` & `plum_tools-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `plum_tools-0.2.6/README.md` & `plum_tools-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `plum_tools-0.2.6/plum_tools/compat.py` & `plum_tools-0.2.7/plum_tools/compat.py`

 * *Files identical despite different names*

### Comparing `plum_tools-0.2.6/plum_tools/conf.py` & `plum_tools-0.2.7/plum_tools/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import print_function
 
 import os
 
 import six
 
 
-VERSION = "0.2.6"
+VERSION = "0.2.7"
 
 
 class ClsReadOnlyClass(type):
     """类属性只读"""
 
     def __setattr__(cls, key, value):
         """修改属性式抛出异常"""
```

### Comparing `plum_tools-0.2.6/plum_tools/exceptions.py` & `plum_tools-0.2.7/plum_tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `plum_tools-0.2.6/plum_tools/gitrepo.py` & `plum_tools-0.2.7/plum_tools/gitrepo.py`

 * *Files identical despite different names*

### Comparing `plum_tools-0.2.6/plum_tools/gitstash.py` & `plum_tools-0.2.7/plum_tools/gitstash.py`

 * *Files identical despite different names*

### Comparing `plum_tools-0.2.6/plum_tools/pipmi.py` & `plum_tools-0.2.7/plum_tools/pipmi.py`

 * *Files identical despite different names*

### Comparing `plum_tools-0.2.6/plum_tools/pping.py` & `plum_tools-0.2.7/plum_tools/pping.py`

 * *Files identical despite different names*

### Comparing `plum_tools-0.2.6/plum_tools/prn.py` & `plum_tools-0.2.7/plum_tools/prn.py`

 * *Files identical despite different names*

### Comparing `plum_tools-0.2.6/plum_tools/pssh.py` & `plum_tools-0.2.7/plum_tools/pssh.py`

 * *Files identical despite different names*

### Comparing `plum_tools-0.2.6/plum_tools/utils/git.py` & `plum_tools-0.2.7/plum_tools/utils/git.py`

 * *Files identical despite different names*

### Comparing `plum_tools-0.2.6/plum_tools/utils/printer.py` & `plum_tools-0.2.7/plum_tools/utils/printer.py`

 * *Files identical despite different names*

### Comparing `plum_tools-0.2.6/plum_tools/utils/sshconf.py` & `plum_tools-0.2.7/plum_tools/utils/sshconf.py`

 * *Files identical despite different names*

### Comparing `plum_tools-0.2.6/plum_tools/utils/utils.py` & `plum_tools-0.2.7/plum_tools/utils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,15 +211,15 @@
     path = replace_path(path)
     cmd = OsCommand.stat_command % path
     output = run_cmd(cmd)
 
     # 获取操作系统类型
     system_type = platform.system()
     if system_type == "Linux":
-        pattern = re.compile(r'File: "(.*)"')
+        pattern = re.compile(r'File: (.*)')
     # mac系统
     elif system_type == "Darwin":
         pattern = re.compile(r'"\s+\d+\s+\d+\s+\d+(.*)$')
     else:
         raise SystemTypeError("此项功能仅支持 Linux / Darwin(mac)")
     match = pattern.search(output)
     abs_path = replace_path(match.group(1).strip())
```

### Comparing `plum_tools-0.2.6/plum_tools.egg-info/SOURCES.txt` & `plum_tools-0.2.7/plum_tools.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -24,12 +24,20 @@
 plum_tools.egg-info/requires.txt
 plum_tools.egg-info/top_level.txt
 plum_tools/utils/__init__.py
 plum_tools/utils/git.py
 plum_tools/utils/printer.py
 plum_tools/utils/sshconf.py
 plum_tools/utils/utils.py
+tests/test_conf.py
+tests/test_gitrepo.py
+tests/test_gitstash.py
+tests/test_main.py
+tests/test_pipmi.py
+tests/test_pping.py
+tests/test_prn.py
+tests/test_pssh.py
 tests/utils/__init__.py
 tests/utils/test_git.py
 tests/utils/test_printer.py
 tests/utils/test_sshconf.py
 tests/utils/test_utils.py
```

### Comparing `plum_tools-0.2.6/setup.py` & `plum_tools-0.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import shutil
 
 from setuptools import setup, find_packages
 
 from plum_tools.conf import PathConfig
 
-version = '0.2.6'
+version = '0.2.7'
 
 
 def install():
     setup(
         author="seekplum",
         author_email='1131909224m@sina.cn',
         classifiers=[
```

### Comparing `plum_tools-0.2.6/tests/utils/test_git.py` & `plum_tools-0.2.7/tests/utils/test_git.py`

 * *Files identical despite different names*

### Comparing `plum_tools-0.2.6/tests/utils/test_printer.py` & `plum_tools-0.2.7/tests/utils/test_printer.py`

 * *Files identical despite different names*

### Comparing `plum_tools-0.2.6/tests/utils/test_sshconf.py` & `plum_tools-0.2.7/tests/utils/test_sshconf.py`

 * *Files identical despite different names*

