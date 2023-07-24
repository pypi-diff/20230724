# Comparing `tmp/mppm-3.0.1.tar.gz` & `tmp/mppm-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mppm-3.0.1.tar", last modified: Fri Jul 21 07:51:11 2023, max compression
+gzip compressed data, was "dist/mppm-3.0.4.tar", last modified: Mon Jul 24 09:47:25 2023, max compression
```

## Comparing `mppm-3.0.1.tar` & `mppm-3.0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 07:51:11.828369 mppm-3.0.1/
--rw-r--r--   0 root         (0) root         (0)     1073 2023-07-19 13:19:06.000000 mppm-3.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3142 2023-07-21 07:51:11.828369 mppm-3.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2458 2023-07-21 07:49:27.000000 mppm-3.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 07:51:11.826369 mppm-3.0.1/mppm/
--rw-r--r--   0 root         (0) root         (0)      322 2023-07-19 13:19:06.000000 mppm-3.0.1/mppm/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 07:51:11.827370 mppm-3.0.1/mppm/src/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 13:19:06.000000 mppm-3.0.1/mppm/src/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 07:51:11.827370 mppm-3.0.1/mppm/src/command/
--rw-r--r--   0 root         (0) root         (0)     2891 2023-07-21 07:46:34.000000 mppm-3.0.1/mppm/src/command/argpass.py
--rw-r--r--   0 root         (0) root         (0)      527 2023-07-21 07:25:09.000000 mppm-3.0.1/mppm/src/command/cmd_dispatch.py
--rw-r--r--   0 root         (0) root         (0)      936 2023-07-21 07:25:09.000000 mppm-3.0.1/mppm/src/command/download.py
--rw-r--r--   0 root         (0) root         (0)      681 2023-07-21 07:34:19.000000 mppm-3.0.1/mppm/src/command/rewrite.py
--rw-r--r--   0 root         (0) root         (0)     1077 2023-07-20 08:09:36.000000 mppm-3.0.1/mppm/src/command/uninstall.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 07:51:11.828369 mppm-3.0.1/mppm/src/common/
--rw-r--r--   0 root         (0) root         (0)     1510 2023-07-21 07:49:27.000000 mppm-3.0.1/mppm/src/common/const.py
--rw-r--r--   0 root         (0) root         (0)     2784 2023-07-20 08:07:46.000000 mppm-3.0.1/mppm/src/common/utility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 07:51:11.828369 mppm-3.0.1/mppm/src/config/
--rw-r--r--   0 root         (0) root         (0)     1383 2023-07-21 07:34:19.000000 mppm-3.0.1/mppm/src/config/pip_conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 07:51:11.827370 mppm-3.0.1/mppm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3142 2023-07-21 07:51:11.000000 mppm-3.0.1/mppm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      457 2023-07-21 07:51:11.000000 mppm-3.0.1/mppm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 07:51:11.000000 mppm-3.0.1/mppm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-07-21 07:51:11.000000 mppm-3.0.1/mppm.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       64 2023-07-21 07:51:11.000000 mppm-3.0.1/mppm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-07-21 07:51:11.000000 mppm-3.0.1/mppm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 07:51:11.828369 mppm-3.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1317 2023-07-21 07:49:27.000000 mppm-3.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 09:47:25.000000 mppm-3.0.4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 09:47:25.000000 mppm-3.0.4/mppm/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 09:47:25.000000 mppm-3.0.4/mppm/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 09:47:25.000000 mppm-3.0.4/mppm/src/command/
+-rw-r--r--   0 root         (0) root         (0)     3057 2023-07-24 09:36:55.000000 mppm-3.0.4/mppm/src/command/argpass.py
+-rw-r--r--   0 root         (0) root         (0)      527 2023-07-24 09:36:55.000000 mppm-3.0.4/mppm/src/command/cmd_dispatch.py
+-rw-r--r--   0 root         (0) root         (0)     1159 2023-07-24 09:36:55.000000 mppm-3.0.4/mppm/src/command/download.py
+-rw-r--r--   0 root         (0) root         (0)      681 2023-07-24 09:36:55.000000 mppm-3.0.4/mppm/src/command/rewrite.py
+-rw-r--r--   0 root         (0) root         (0)     1077 2023-07-24 09:36:55.000000 mppm-3.0.4/mppm/src/command/uninstall.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 09:47:25.000000 mppm-3.0.4/mppm/src/common/
+-rw-r--r--   0 root         (0) root         (0)     1579 2023-07-24 09:46:26.000000 mppm-3.0.4/mppm/src/common/const.py
+-rw-r--r--   0 root         (0) root         (0)     2784 2023-07-24 09:36:55.000000 mppm-3.0.4/mppm/src/common/utility.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 09:47:25.000000 mppm-3.0.4/mppm/src/config/
+-rw-r--r--   0 root         (0) root         (0)     1383 2023-07-24 09:36:55.000000 mppm-3.0.4/mppm/src/config/pip_conf.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 09:36:55.000000 mppm-3.0.4/mppm/src/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      322 2023-07-24 09:36:55.000000 mppm-3.0.4/mppm/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 09:47:25.000000 mppm-3.0.4/mppm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3162 2023-07-24 09:47:25.000000 mppm-3.0.4/mppm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      457 2023-07-24 09:47:25.000000 mppm-3.0.4/mppm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 09:47:25.000000 mppm-3.0.4/mppm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2023-07-24 09:47:25.000000 mppm-3.0.4/mppm.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2023-07-24 09:47:25.000000 mppm-3.0.4/mppm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-07-24 09:47:25.000000 mppm-3.0.4/mppm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-07-24 09:36:55.000000 mppm-3.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2458 2023-07-24 09:36:55.000000 mppm-3.0.4/README.md
+-rw-r--r--   0 root         (0) root         (0)     1345 2023-07-24 09:46:26.000000 mppm-3.0.4/setup.py
+-rw-r--r--   0 root         (0) root         (0)     3162 2023-07-24 09:47:25.000000 mppm-3.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 09:47:25.000000 mppm-3.0.4/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `mppm-3.0.1/LICENSE` & `mppm-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mppm-3.0.1/PKG-INFO` & `mppm-3.0.4/mppm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: mppm
-Version: 3.0.1
+Version: 3.0.4
 Summary: Manager Pypi Package & Mirror
 Home-page: https://gitee.com/TianCiwang/mppm.git
 Author: TianCiwang
 Author-email: 13623650548@163.com
 License: MIT
 Keywords: pypi,mirror,package
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -98,7 +99,9 @@
 You can add package indexes to your `~/.pip/pip.conf` file. Example:
 
     [global]
     timeout = 120
     index-url = https://pypi.org/simple/
     trusted-host = pypi.org
 
+
+
```

### Comparing `mppm-3.0.1/README.md` & `mppm-3.0.4/README.md`

 * *Files identical despite different names*

### Comparing `mppm-3.0.1/mppm/src/command/argpass.py` & `mppm-3.0.4/mppm/src/command/argpass.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,16 @@
 	def _add_download_module(self):
 		subparser = self.subparser.add_parser(SUB_CMD_DOWNLOAD, help="download modules", allow_abbrev=False)
 		group = subparser.add_mutually_exclusive_group(required=True)
 		group.add_argument(f'-{ARG_DOWNLOAD_MODULE_SHORT}', f'--{ARG_DOWNLOAD_MODULE}',
 						   help="download specified modules and dependencies")
 		group.add_argument(f'-{ARG_DOWNLOAD_REQUIREMENT_SHORT}', f'--{ARG_DOWNLOAD_REQUIREMENT}',
 						   help="download the modules and dependencies specified in the file. like requirements.txt")
+		subparser.add_argument(f'-{ARG_DOWNLOAD_SAVE_PATH_SHORT}', f'--{ARG_DOWNLOAD_SAVE_PATH}',
+							   default="./", required=False, help="download module save path")
 		subparser.add_argument(f'-{ARG_DOWNLOAD_REWRITE_PIP_CONFIG_SHORT}', f'--{ARG_DOWNLOAD_REWRITE_PIP_CONFIG}',
 							   action='store_true', default=False, required=False, help="rewrite the pip configuration")
 
 	def _add_uninstall_module(self):
 		subparser = self.subparser.add_parser(SUB_CMD_UNINSTALL, help="uninstall modules", allow_abbrev=False)
 		group = subparser.add_mutually_exclusive_group(required=True)
 		group.add_argument(f'-{ARG_UNINSTALL_MODULE_SHORT}', f'--{ARG_UNINSTALL_MODULE}',
```

### Comparing `mppm-3.0.1/mppm/src/command/cmd_dispatch.py` & `mppm-3.0.4/mppm/src/command/cmd_dispatch.py`

 * *Files identical despite different names*

### Comparing `mppm-3.0.1/mppm/src/command/download.py` & `mppm-3.0.4/mppm/src/command/download.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,19 +4,25 @@
 
 
 class DownloadCmd():
     def __init__(self, args):
         self.args = args
 
     def exec(self, pip_path):
+        if self.args.output != "./":
+            base_output = self.args.output
+        else:
+            if self.args.module:
+                base_output = f"{self.args.output}{self.args.module}"
+            else:
+                base_output = f"{self.args.output}{ARG_DOWNLOAD_REQUIREMENT}"
+        create_dir(base_output)
         if self.args.module:
-            create_dir(self.args.module)
-            download_pip_pkg_cmd = "{} download {} -d {}".format(pip_path, self.args.module, self.args.module)
+            download_pip_pkg_cmd = "{} download {} -d {}".format(pip_path, self.args.module, base_output)
         else:
-            create_dir(ARG_DOWNLOAD_REQUIREMENT)
             download_pip_pkg_cmd = "{} download -r {} -d {}".format(pip_path, self.args.requirement,
-                                                                    ARG_DOWNLOAD_REQUIREMENT)
+                                                                    base_output)
         cmd_result = exec_cmd(download_pip_pkg_cmd)
         if cmd_result is None or ignore_errors[self.args.sub_cmd] in cmd_result:
-            print_colored(f"the module and dependencies have been downloaded. Please check the current path", "green")
+            print_colored(f"the module and dependencies have been downloaded. Please check the {base_output} path", "green")
         else:
             print_colored(cmd_result, "red")
```

### Comparing `mppm-3.0.1/mppm/src/command/rewrite.py` & `mppm-3.0.4/mppm/src/command/rewrite.py`

 * *Files identical despite different names*

### Comparing `mppm-3.0.1/mppm/src/command/uninstall.py` & `mppm-3.0.4/mppm/src/command/uninstall.py`

 * *Files identical despite different names*

### Comparing `mppm-3.0.1/mppm/src/common/const.py` & `mppm-3.0.4/mppm/src/common/const.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 APP_NAME = 'mppm'  # 程序名称
 APP_VERSION_MAJOR = "3.0"
-APP_VERSION_MINOR = "1"
+APP_VERSION_MINOR = "4"
 EXIT_WITH_ERROR = 9999  # 错误退出码12 为用户自定义信号
 
 pypi_configuration_sources = [
     {"name": "pypi", "url": "https://pypi.org/simple/", "timeout": "120"},
     {"name": "tuna", "url": "https://pypi.tuna.tsinghua.edu.cn/simple/", "timeout": "60"},
     {"name": "aliyun", "url": "https://mirrors.aliyun.com/pypi/simple/", "timeout": "60"},
     {"name": "douban", "url": "http://pypi.douban.com/simple/", "timeout": "60"},
@@ -27,14 +27,16 @@
 SUB_CMD_DOWNLOAD = "download"
 ARG_DOWNLOAD_MODULE = "module"
 ARG_DOWNLOAD_MODULE_SHORT = "m"
 ARG_DOWNLOAD_REQUIREMENT = "requirement"
 ARG_DOWNLOAD_REQUIREMENT_SHORT = "r"
 ARG_DOWNLOAD_REWRITE_PIP_CONFIG = "yes"
 ARG_DOWNLOAD_REWRITE_PIP_CONFIG_SHORT = "y"
+ARG_DOWNLOAD_SAVE_PATH = "output"
+ARG_DOWNLOAD_SAVE_PATH_SHORT = "o"
 
 # Uninstall specified modules and dependencies
 SUB_CMD_UNINSTALL = "uninstall"
 ARG_UNINSTALL_MODULE = "module"
 ARG_UNINSTALL_MODULE_SHORT = "m"
 ARG_UNINSTALL_REQUIREMENT = "requirement"
 ARG_UNINSTALL_REQUIREMENT_SHORT = "r"
```

### Comparing `mppm-3.0.1/mppm/src/common/utility.py` & `mppm-3.0.4/mppm/src/common/utility.py`

 * *Files identical despite different names*

### Comparing `mppm-3.0.1/mppm/src/config/pip_conf.py` & `mppm-3.0.4/mppm/src/config/pip_conf.py`

 * *Files identical despite different names*

### Comparing `mppm-3.0.1/mppm.egg-info/PKG-INFO` & `mppm-3.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: mppm
-Version: 3.0.1
+Version: 3.0.4
 Summary: Manager Pypi Package & Mirror
 Home-page: https://gitee.com/TianCiwang/mppm.git
 Author: TianCiwang
 Author-email: 13623650548@163.com
 License: MIT
 Keywords: pypi,mirror,package
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -98,7 +99,9 @@
 You can add package indexes to your `~/.pip/pip.conf` file. Example:
 
     [global]
     timeout = 120
     index-url = https://pypi.org/simple/
     trusted-host = pypi.org
 
+
+
```

### Comparing `mppm-3.0.1/setup.py` & `mppm-3.0.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,25 +9,25 @@
     filepath = os.path.join(os.path.dirname(__file__), fname)
     with open(filepath, 'r') as fp:
         return fp.read()
 
 
 required = [
     'pip',
-    'crayons',
-    'blindspin',
+    'crayons==0.4.0',
+    'blindspin==2.0.1',
     'requests',
-    'pick',
-    'configparser',
+    'pick==1.3.1',
+    'configparser==6.0.0',
     'pip-autoremove',
 ]
 
 setup(
     name='mppm',
-    version='3.0.1',
+    version='3.0.4',
     description='Manager Pypi Package & Mirror',
     keywords='pypi,mirror,package',
     url='https://gitee.com/TianCiwang/mppm.git',
     long_description=fread('README.md'),
     long_description_content_type='text/markdown',
     author='TianCiwang',
     author_email='13623650548@163.com',
```

