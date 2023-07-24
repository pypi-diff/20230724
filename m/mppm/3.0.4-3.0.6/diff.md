# Comparing `tmp/mppm-3.0.4.tar.gz` & `tmp/mppm-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mppm-3.0.4.tar", last modified: Mon Jul 24 09:47:25 2023, max compression
+gzip compressed data, was "dist/mppm-3.0.6.tar", last modified: Mon Jul 24 09:56:46 2023, max compression
```

## Comparing `mppm-3.0.4.tar` & `mppm-3.0.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 09:47:25.000000 mppm-3.0.4/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 09:47:25.000000 mppm-3.0.4/mppm/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 09:47:25.000000 mppm-3.0.4/mppm/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 09:47:25.000000 mppm-3.0.4/mppm/src/command/
--rw-r--r--   0 root         (0) root         (0)     3057 2023-07-24 09:36:55.000000 mppm-3.0.4/mppm/src/command/argpass.py
--rw-r--r--   0 root         (0) root         (0)      527 2023-07-24 09:36:55.000000 mppm-3.0.4/mppm/src/command/cmd_dispatch.py
--rw-r--r--   0 root         (0) root         (0)     1159 2023-07-24 09:36:55.000000 mppm-3.0.4/mppm/src/command/download.py
--rw-r--r--   0 root         (0) root         (0)      681 2023-07-24 09:36:55.000000 mppm-3.0.4/mppm/src/command/rewrite.py
--rw-r--r--   0 root         (0) root         (0)     1077 2023-07-24 09:36:55.000000 mppm-3.0.4/mppm/src/command/uninstall.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 09:47:25.000000 mppm-3.0.4/mppm/src/common/
--rw-r--r--   0 root         (0) root         (0)     1579 2023-07-24 09:46:26.000000 mppm-3.0.4/mppm/src/common/const.py
--rw-r--r--   0 root         (0) root         (0)     2784 2023-07-24 09:36:55.000000 mppm-3.0.4/mppm/src/common/utility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 09:47:25.000000 mppm-3.0.4/mppm/src/config/
--rw-r--r--   0 root         (0) root         (0)     1383 2023-07-24 09:36:55.000000 mppm-3.0.4/mppm/src/config/pip_conf.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 09:36:55.000000 mppm-3.0.4/mppm/src/__init__.py
--rw-r--r--   0 root         (0) root         (0)      322 2023-07-24 09:36:55.000000 mppm-3.0.4/mppm/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 09:47:25.000000 mppm-3.0.4/mppm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3162 2023-07-24 09:47:25.000000 mppm-3.0.4/mppm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      457 2023-07-24 09:47:25.000000 mppm-3.0.4/mppm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 09:47:25.000000 mppm-3.0.4/mppm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       40 2023-07-24 09:47:25.000000 mppm-3.0.4/mppm.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       92 2023-07-24 09:47:25.000000 mppm-3.0.4/mppm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-07-24 09:47:25.000000 mppm-3.0.4/mppm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1073 2023-07-24 09:36:55.000000 mppm-3.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2458 2023-07-24 09:36:55.000000 mppm-3.0.4/README.md
--rw-r--r--   0 root         (0) root         (0)     1345 2023-07-24 09:46:26.000000 mppm-3.0.4/setup.py
--rw-r--r--   0 root         (0) root         (0)     3162 2023-07-24 09:47:25.000000 mppm-3.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 09:47:25.000000 mppm-3.0.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 09:56:46.000000 mppm-3.0.6/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 09:56:46.000000 mppm-3.0.6/mppm/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 09:56:46.000000 mppm-3.0.6/mppm/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 09:56:46.000000 mppm-3.0.6/mppm/src/command/
+-rw-r--r--   0 root         (0) root         (0)     3057 2023-07-24 09:56:14.000000 mppm-3.0.6/mppm/src/command/argpass.py
+-rw-r--r--   0 root         (0) root         (0)      527 2023-07-24 09:56:14.000000 mppm-3.0.6/mppm/src/command/cmd_dispatch.py
+-rw-r--r--   0 root         (0) root         (0)     1159 2023-07-24 09:56:14.000000 mppm-3.0.6/mppm/src/command/download.py
+-rw-r--r--   0 root         (0) root         (0)      681 2023-07-24 09:56:14.000000 mppm-3.0.6/mppm/src/command/rewrite.py
+-rw-r--r--   0 root         (0) root         (0)     1077 2023-07-24 09:56:14.000000 mppm-3.0.6/mppm/src/command/uninstall.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 09:56:46.000000 mppm-3.0.6/mppm/src/common/
+-rw-r--r--   0 root         (0) root         (0)     1579 2023-07-24 09:56:14.000000 mppm-3.0.6/mppm/src/common/const.py
+-rw-r--r--   0 root         (0) root         (0)     2784 2023-07-24 09:56:14.000000 mppm-3.0.6/mppm/src/common/utility.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 09:56:46.000000 mppm-3.0.6/mppm/src/config/
+-rw-r--r--   0 root         (0) root         (0)     1383 2023-07-24 09:56:14.000000 mppm-3.0.6/mppm/src/config/pip_conf.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 09:56:14.000000 mppm-3.0.6/mppm/src/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      322 2023-07-24 09:56:14.000000 mppm-3.0.6/mppm/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 09:56:46.000000 mppm-3.0.6/mppm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3162 2023-07-24 09:56:46.000000 mppm-3.0.6/mppm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      457 2023-07-24 09:56:46.000000 mppm-3.0.6/mppm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 09:56:46.000000 mppm-3.0.6/mppm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2023-07-24 09:56:46.000000 mppm-3.0.6/mppm.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       78 2023-07-24 09:56:46.000000 mppm-3.0.6/mppm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-07-24 09:56:46.000000 mppm-3.0.6/mppm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-07-24 09:56:14.000000 mppm-3.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2458 2023-07-24 09:56:14.000000 mppm-3.0.6/README.md
+-rw-r--r--   0 root         (0) root         (0)     1338 2023-07-24 09:56:14.000000 mppm-3.0.6/setup.py
+-rw-r--r--   0 root         (0) root         (0)     3162 2023-07-24 09:56:46.000000 mppm-3.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 09:56:46.000000 mppm-3.0.6/setup.cfg
```

### Comparing `mppm-3.0.4/mppm/src/command/argpass.py` & `mppm-3.0.6/mppm/src/command/argpass.py`

 * *Files identical despite different names*

### Comparing `mppm-3.0.4/mppm/src/command/cmd_dispatch.py` & `mppm-3.0.6/mppm/src/command/cmd_dispatch.py`

 * *Files identical despite different names*

### Comparing `mppm-3.0.4/mppm/src/command/download.py` & `mppm-3.0.6/mppm/src/command/download.py`

 * *Files identical despite different names*

### Comparing `mppm-3.0.4/mppm/src/command/rewrite.py` & `mppm-3.0.6/mppm/src/command/rewrite.py`

 * *Files identical despite different names*

### Comparing `mppm-3.0.4/mppm/src/command/uninstall.py` & `mppm-3.0.6/mppm/src/command/uninstall.py`

 * *Files identical despite different names*

### Comparing `mppm-3.0.4/mppm/src/common/const.py` & `mppm-3.0.6/mppm/src/common/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 APP_NAME = 'mppm'  # 程序名称
 APP_VERSION_MAJOR = "3.0"
-APP_VERSION_MINOR = "4"
+APP_VERSION_MINOR = "6"
 EXIT_WITH_ERROR = 9999  # 错误退出码12 为用户自定义信号
 
 pypi_configuration_sources = [
     {"name": "pypi", "url": "https://pypi.org/simple/", "timeout": "120"},
     {"name": "tuna", "url": "https://pypi.tuna.tsinghua.edu.cn/simple/", "timeout": "60"},
     {"name": "aliyun", "url": "https://mirrors.aliyun.com/pypi/simple/", "timeout": "60"},
     {"name": "douban", "url": "http://pypi.douban.com/simple/", "timeout": "60"},
```

### Comparing `mppm-3.0.4/mppm/src/common/utility.py` & `mppm-3.0.6/mppm/src/common/utility.py`

 * *Files identical despite different names*

### Comparing `mppm-3.0.4/mppm/src/config/pip_conf.py` & `mppm-3.0.6/mppm/src/config/pip_conf.py`

 * *Files identical despite different names*

### Comparing `mppm-3.0.4/mppm.egg-info/PKG-INFO` & `mppm-3.0.6/mppm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mppm
-Version: 3.0.4
+Version: 3.0.6
 Summary: Manager Pypi Package & Mirror
 Home-page: https://gitee.com/TianCiwang/mppm.git
 Author: TianCiwang
 Author-email: 13623650548@163.com
 License: MIT
 Keywords: pypi,mirror,package
 Platform: UNKNOWN
```

### Comparing `mppm-3.0.4/LICENSE` & `mppm-3.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mppm-3.0.4/README.md` & `mppm-3.0.6/README.md`

 * *Files identical despite different names*

### Comparing `mppm-3.0.4/setup.py` & `mppm-3.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,25 +9,26 @@
     filepath = os.path.join(os.path.dirname(__file__), fname)
     with open(filepath, 'r') as fp:
         return fp.read()
 
 
 required = [
     'pip',
-    'crayons==0.4.0',
-    'blindspin==2.0.1',
+    'crayons',
+    'blindspin',
     'requests',
     'pick==1.3.1',
-    'configparser==6.0.0',
+    'configparser',
     'pip-autoremove',
+    'dir2pi',
 ]
 
 setup(
     name='mppm',
-    version='3.0.4',
+    version='3.0.6',
     description='Manager Pypi Package & Mirror',
     keywords='pypi,mirror,package',
     url='https://gitee.com/TianCiwang/mppm.git',
     long_description=fread('README.md'),
     long_description_content_type='text/markdown',
     author='TianCiwang',
     author_email='13623650548@163.com',
```

### Comparing `mppm-3.0.4/PKG-INFO` & `mppm-3.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mppm
-Version: 3.0.4
+Version: 3.0.6
 Summary: Manager Pypi Package & Mirror
 Home-page: https://gitee.com/TianCiwang/mppm.git
 Author: TianCiwang
 Author-email: 13623650548@163.com
 License: MIT
 Keywords: pypi,mirror,package
 Platform: UNKNOWN
```

