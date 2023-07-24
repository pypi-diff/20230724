# Comparing `tmp/mwj-apitest-1.1.3.tar.gz` & `tmp/mwj-apitest-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mwj-apitest-1.1.3.tar", last modified: Mon Jul 24 09:39:09 2023, max compression
+gzip compressed data, was "mwj-apitest-1.1.4.tar", last modified: Mon Jul 24 10:40:13 2023, max compression
```

## Comparing `mwj-apitest-1.1.3.tar` & `mwj-apitest-1.1.4.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 09:39:09.937684 mwj-apitest-1.1.3/
--rw-rw-rw-   0        0        0     1091 2023-05-31 08:57:31.000000 mwj-apitest-1.1.3/LICENSE
--rw-rw-rw-   0        0        0       34 2023-05-31 08:08:20.000000 mwj-apitest-1.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0      969 2023-07-24 09:39:09.936686 mwj-apitest-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      490 2023-07-21 08:25:51.000000 mwj-apitest-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-24 09:39:09.901877 mwj-apitest-1.1.3/mwjApiTest/
--rw-rw-rw-   0        0        0      215 2023-05-31 09:41:04.000000 mwj-apitest-1.1.3/mwjApiTest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:39:09.911728 mwj-apitest-1.1.3/mwjApiTest/core/
--rw-rw-rw-   0        0        0      190 2023-05-31 08:48:04.000000 mwj-apitest-1.1.3/mwjApiTest/core/__init__.py
--rw-rw-rw-   0        0        0     6001 2023-07-13 09:21:04.000000 mwj-apitest-1.1.3/mwjApiTest/core/basecase.py
--rw-rw-rw-   0        0        0     5378 2023-07-12 09:40:57.000000 mwj-apitest-1.1.3/mwjApiTest/core/dataParser.py
--rw-rw-rw-   0        0        0     1456 2023-07-10 08:19:16.000000 mwj-apitest-1.1.3/mwjApiTest/core/db_client.py
--rw-rw-rw-   0        0        0     2559 2023-07-13 10:24:23.000000 mwj-apitest-1.1.3/mwjApiTest/core/env_prepare.py
--rw-rw-rw-   0        0        0     3350 2023-07-14 08:08:04.000000 mwj-apitest-1.1.3/mwjApiTest/core/generateCase.py
--rw-rw-rw-   0        0        0    22073 2023-07-21 09:16:40.000000 mwj-apitest-1.1.3/mwjApiTest/core/httptest.py
--rw-rw-rw-   0        0        0     3653 2023-07-10 08:09:42.000000 mwj-apitest-1.1.3/mwjApiTest/core/log_operation.py
--rw-rw-rw-   0        0        0     2117 2023-07-10 08:36:03.000000 mwj-apitest-1.1.3/mwjApiTest/core/make_data.py
--rw-rw-rw-   0        0        0     6781 2023-07-11 03:09:03.000000 mwj-apitest-1.1.3/mwjApiTest/core/send_report.py
--rw-rw-rw-   0        0        0    20285 2023-07-21 08:28:06.000000 mwj-apitest-1.1.3/mwjApiTest/core/testRunner.py
--rw-rw-rw-   0        0        0     6743 2023-07-24 09:38:38.000000 mwj-apitest-1.1.3/mwjApiTest/manage.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:39:09.913725 mwj-apitest-1.1.3/mwjApiTest/templates/
--rw-rw-rw-   0        0        0      190 2023-07-12 03:00:19.000000 mwj-apitest-1.1.3/mwjApiTest/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:39:09.914721 mwj-apitest-1.1.3/mwjApiTest/templates/reports/
--rw-rw-rw-   0        0        0      190 2023-07-12 03:00:19.000000 mwj-apitest-1.1.3/mwjApiTest/templates/reports/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:39:09.918711 mwj-apitest-1.1.3/mwjApiTest/templates/request_file_demo/
--rw-rw-rw-   0        0        0      190 2023-07-19 10:08:25.000000 mwj-apitest-1.1.3/mwjApiTest/templates/request_file_demo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:39:09.919708 mwj-apitest-1.1.3/mwjApiTest/templates/request_file_demo/case_json/
--rw-rw-rw-   0        0        0      190 2023-07-21 05:58:29.000000 mwj-apitest-1.1.3/mwjApiTest/templates/request_file_demo/case_json/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:39:09.921724 mwj-apitest-1.1.3/mwjApiTest/templates/request_file_demo/case_py/
--rw-rw-rw-   0        0        0      190 2023-07-21 05:58:29.000000 mwj-apitest-1.1.3/mwjApiTest/templates/request_file_demo/case_py/__init__.py
--rw-rw-rw-   0        0        0     1232 2023-07-21 08:08:11.000000 mwj-apitest-1.1.3/mwjApiTest/templates/request_file_demo/case_py/test_case_demo.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:39:09.921724 mwj-apitest-1.1.3/mwjApiTest/templates/request_file_demo/case_yaml/
--rw-rw-rw-   0        0        0      190 2023-07-21 05:58:29.000000 mwj-apitest-1.1.3/mwjApiTest/templates/request_file_demo/case_yaml/__init__.py
--rw-rw-rw-   0        0        0     3749 2023-07-14 06:35:52.000000 mwj-apitest-1.1.3/mwjApiTest/templates/request_file_demo/funcTools.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:39:09.922723 mwj-apitest-1.1.3/mwjApiTest/templates/request_file_demo/logs/
--rw-rw-rw-   0        0        0      190 2023-07-21 05:58:29.000000 mwj-apitest-1.1.3/mwjApiTest/templates/request_file_demo/logs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:39:09.923721 mwj-apitest-1.1.3/mwjApiTest/templates/request_file_demo/reports/
--rw-rw-rw-   0        0        0      190 2023-07-21 05:58:28.000000 mwj-apitest-1.1.3/mwjApiTest/templates/request_file_demo/reports/__init__.py
--rw-rw-rw-   0        0        0      223 2023-07-14 08:23:35.000000 mwj-apitest-1.1.3/mwjApiTest/templates/request_file_demo/run.py
--rw-rw-rw-   0        0        0     2117 2023-07-21 09:08:28.000000 mwj-apitest-1.1.3/mwjApiTest/templates/request_file_demo/settings.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:39:09.923721 mwj-apitest-1.1.3/mwjApiTest/utils/
--rw-rw-rw-   0        0        0      190 2023-05-31 08:48:04.000000 mwj-apitest-1.1.3/mwjApiTest/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:39:09.935718 mwj-apitest-1.1.3/mwj_apitest.egg-info/
--rw-rw-rw-   0        0        0      969 2023-07-24 09:39:09.000000 mwj-apitest-1.1.3/mwj_apitest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1253 2023-07-24 09:39:09.000000 mwj-apitest-1.1.3/mwj_apitest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 09:39:09.000000 mwj-apitest-1.1.3/mwj_apitest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-07-24 09:39:09.000000 mwj-apitest-1.1.3/mwj_apitest.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       11 2023-07-24 09:39:09.000000 mwj-apitest-1.1.3/mwj_apitest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 09:39:09.937684 mwj-apitest-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1501 2023-07-24 09:38:38.000000 mwj-apitest-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 10:40:13.393580 mwj-apitest-1.1.4/
+-rw-rw-rw-   0        0        0     1091 2023-05-31 08:57:31.000000 mwj-apitest-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-05-31 08:08:20.000000 mwj-apitest-1.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      969 2023-07-24 10:40:13.393580 mwj-apitest-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      490 2023-07-21 08:25:51.000000 mwj-apitest-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 10:40:13.360669 mwj-apitest-1.1.4/mwjApiTest/
+-rw-rw-rw-   0        0        0      215 2023-05-31 09:41:04.000000 mwj-apitest-1.1.4/mwjApiTest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 10:40:13.370641 mwj-apitest-1.1.4/mwjApiTest/core/
+-rw-rw-rw-   0        0        0      190 2023-05-31 08:48:04.000000 mwj-apitest-1.1.4/mwjApiTest/core/__init__.py
+-rw-rw-rw-   0        0        0     6001 2023-07-13 09:21:04.000000 mwj-apitest-1.1.4/mwjApiTest/core/basecase.py
+-rw-rw-rw-   0        0        0     5378 2023-07-12 09:40:57.000000 mwj-apitest-1.1.4/mwjApiTest/core/dataParser.py
+-rw-rw-rw-   0        0        0     1456 2023-07-10 08:19:16.000000 mwj-apitest-1.1.4/mwjApiTest/core/db_client.py
+-rw-rw-rw-   0        0        0     2559 2023-07-13 10:24:23.000000 mwj-apitest-1.1.4/mwjApiTest/core/env_prepare.py
+-rw-rw-rw-   0        0        0     3350 2023-07-14 08:08:04.000000 mwj-apitest-1.1.4/mwjApiTest/core/generateCase.py
+-rw-rw-rw-   0        0        0    22073 2023-07-21 09:16:40.000000 mwj-apitest-1.1.4/mwjApiTest/core/httptest.py
+-rw-rw-rw-   0        0        0     3653 2023-07-10 08:09:42.000000 mwj-apitest-1.1.4/mwjApiTest/core/log_operation.py
+-rw-rw-rw-   0        0        0     2117 2023-07-10 08:36:03.000000 mwj-apitest-1.1.4/mwjApiTest/core/make_data.py
+-rw-rw-rw-   0        0        0     6781 2023-07-11 03:09:03.000000 mwj-apitest-1.1.4/mwjApiTest/core/send_report.py
+-rw-rw-rw-   0        0        0    20285 2023-07-21 08:28:06.000000 mwj-apitest-1.1.4/mwjApiTest/core/testRunner.py
+-rw-rw-rw-   0        0        0     6743 2023-07-24 10:40:11.000000 mwj-apitest-1.1.4/mwjApiTest/manage.py
+drwxrwxrwx   0        0        0        0 2023-07-24 10:40:13.371639 mwj-apitest-1.1.4/mwjApiTest/templates/
+-rw-rw-rw-   0        0        0      190 2023-07-12 03:00:19.000000 mwj-apitest-1.1.4/mwjApiTest/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 10:40:13.373633 mwj-apitest-1.1.4/mwjApiTest/templates/reports/
+-rw-rw-rw-   0        0        0      190 2023-07-12 03:00:19.000000 mwj-apitest-1.1.4/mwjApiTest/templates/reports/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 10:40:13.376626 mwj-apitest-1.1.4/mwjApiTest/templates/request_file_demo/
+-rw-rw-rw-   0        0        0      190 2023-07-19 10:08:25.000000 mwj-apitest-1.1.4/mwjApiTest/templates/request_file_demo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 10:40:13.377623 mwj-apitest-1.1.4/mwjApiTest/templates/request_file_demo/case_json/
+-rw-rw-rw-   0        0        0      190 2023-07-21 05:58:29.000000 mwj-apitest-1.1.4/mwjApiTest/templates/request_file_demo/case_json/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 10:40:13.378620 mwj-apitest-1.1.4/mwjApiTest/templates/request_file_demo/case_py/
+-rw-rw-rw-   0        0        0      190 2023-07-21 05:58:29.000000 mwj-apitest-1.1.4/mwjApiTest/templates/request_file_demo/case_py/__init__.py
+-rw-rw-rw-   0        0        0     1232 2023-07-21 08:08:11.000000 mwj-apitest-1.1.4/mwjApiTest/templates/request_file_demo/case_py/test_case_demo.py
+drwxrwxrwx   0        0        0        0 2023-07-24 10:40:13.379618 mwj-apitest-1.1.4/mwjApiTest/templates/request_file_demo/case_yaml/
+-rw-rw-rw-   0        0        0      190 2023-07-21 05:58:29.000000 mwj-apitest-1.1.4/mwjApiTest/templates/request_file_demo/case_yaml/__init__.py
+-rw-rw-rw-   0        0        0     3749 2023-07-14 06:35:52.000000 mwj-apitest-1.1.4/mwjApiTest/templates/request_file_demo/funcTools.py
+drwxrwxrwx   0        0        0        0 2023-07-24 10:40:13.380615 mwj-apitest-1.1.4/mwjApiTest/templates/request_file_demo/logs/
+-rw-rw-rw-   0        0        0      190 2023-07-21 05:58:29.000000 mwj-apitest-1.1.4/mwjApiTest/templates/request_file_demo/logs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 10:40:13.380615 mwj-apitest-1.1.4/mwjApiTest/templates/request_file_demo/reports/
+-rw-rw-rw-   0        0        0      190 2023-07-21 05:58:28.000000 mwj-apitest-1.1.4/mwjApiTest/templates/request_file_demo/reports/__init__.py
+-rw-rw-rw-   0        0        0      223 2023-07-14 08:23:35.000000 mwj-apitest-1.1.4/mwjApiTest/templates/request_file_demo/run.py
+-rw-rw-rw-   0        0        0     2117 2023-07-21 09:08:28.000000 mwj-apitest-1.1.4/mwjApiTest/templates/request_file_demo/settings.py
+drwxrwxrwx   0        0        0        0 2023-07-24 10:40:13.381612 mwj-apitest-1.1.4/mwjApiTest/utils/
+-rw-rw-rw-   0        0        0      190 2023-05-31 08:48:04.000000 mwj-apitest-1.1.4/mwjApiTest/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 10:40:13.392583 mwj-apitest-1.1.4/mwj_apitest.egg-info/
+-rw-rw-rw-   0        0        0      969 2023-07-24 10:40:13.000000 mwj-apitest-1.1.4/mwj_apitest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1287 2023-07-24 10:40:13.000000 mwj-apitest-1.1.4/mwj_apitest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 10:40:13.000000 mwj-apitest-1.1.4/mwj_apitest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-07-24 10:40:13.000000 mwj-apitest-1.1.4/mwj_apitest.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      124 2023-07-24 10:40:13.000000 mwj-apitest-1.1.4/mwj_apitest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-24 10:40:13.000000 mwj-apitest-1.1.4/mwj_apitest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 10:40:13.393580 mwj-apitest-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1784 2023-07-24 10:40:11.000000 mwj-apitest-1.1.4/setup.py
```

### Comparing `mwj-apitest-1.1.3/LICENSE` & `mwj-apitest-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mwj-apitest-1.1.3/PKG-INFO` & `mwj-apitest-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwj-apitest
-Version: 1.1.3
+Version: 1.1.4
 Summary: An execution engine for the interface automation platform
 Home-page: https://github.com/Lvan826199/mwjApiTest
 Author: 梦无矶小仔
 Author-email: Lvan826199@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mwj-apitest-1.1.3/mwjApiTest/core/basecase.py` & `mwj-apitest-1.1.4/mwjApiTest/core/basecase.py`

 * *Files identical despite different names*

### Comparing `mwj-apitest-1.1.3/mwjApiTest/core/dataParser.py` & `mwj-apitest-1.1.4/mwjApiTest/core/dataParser.py`

 * *Files identical despite different names*

### Comparing `mwj-apitest-1.1.3/mwjApiTest/core/db_client.py` & `mwj-apitest-1.1.4/mwjApiTest/core/db_client.py`

 * *Files identical despite different names*

### Comparing `mwj-apitest-1.1.3/mwjApiTest/core/env_prepare.py` & `mwj-apitest-1.1.4/mwjApiTest/core/env_prepare.py`

 * *Files identical despite different names*

### Comparing `mwj-apitest-1.1.3/mwjApiTest/core/generateCase.py` & `mwj-apitest-1.1.4/mwjApiTest/core/generateCase.py`

 * *Files identical despite different names*

### Comparing `mwj-apitest-1.1.3/mwjApiTest/core/httptest.py` & `mwj-apitest-1.1.4/mwjApiTest/core/httptest.py`

 * *Files identical despite different names*

### Comparing `mwj-apitest-1.1.3/mwjApiTest/core/log_operation.py` & `mwj-apitest-1.1.4/mwjApiTest/core/log_operation.py`

 * *Files identical despite different names*

### Comparing `mwj-apitest-1.1.3/mwjApiTest/core/make_data.py` & `mwj-apitest-1.1.4/mwjApiTest/core/make_data.py`

 * *Files identical despite different names*

### Comparing `mwj-apitest-1.1.3/mwjApiTest/core/send_report.py` & `mwj-apitest-1.1.4/mwjApiTest/core/send_report.py`

 * *Files identical despite different names*

### Comparing `mwj-apitest-1.1.3/mwjApiTest/core/testRunner.py` & `mwj-apitest-1.1.4/mwjApiTest/core/testRunner.py`

 * *Files identical despite different names*

### Comparing `mwj-apitest-1.1.3/mwjApiTest/manage.py` & `mwj-apitest-1.1.4/mwjApiTest/manage.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
             else:
                 log.error("测试结果推送到企业微信失败！错误信息： {}".format(res["errmsg"]))
     return res
 
 def create_parser():
     parser = argparse.ArgumentParser(prog='mwjApiTest', description='梦无矶接口测试框架使用介绍')
     # 添加版本号
-    parser.add_argument('-V', '--version', action='version', version='%(prog)s 1.1.3')
+    parser.add_argument('-V', '--version', action='version', version='%(prog)s 1.1.4')
     subparsers = parser.add_subparsers(title='Command', metavar="命令")
     # 创建项目命令
     create_cmd = subparsers.add_parser('create', help=" 创建测试项目 ", aliases=['C'])
     create_cmd.add_argument('name', metavar='project_name', help=" 项目名称 ")
     create_cmd.set_defaults(func=create)
     # 运行项目命令
     parser_run = subparsers.add_parser('run', help=' 开始运行项目 ', aliases=['R'])
```

### Comparing `mwj-apitest-1.1.3/mwjApiTest/templates/request_file_demo/case_py/test_case_demo.py` & `mwj-apitest-1.1.4/mwjApiTest/templates/request_file_demo/case_py/test_case_demo.py`

 * *Files identical despite different names*

### Comparing `mwj-apitest-1.1.3/mwjApiTest/templates/request_file_demo/funcTools.py` & `mwj-apitest-1.1.4/mwjApiTest/templates/request_file_demo/funcTools.py`

 * *Files identical despite different names*

### Comparing `mwj-apitest-1.1.3/mwjApiTest/templates/request_file_demo/settings.py` & `mwj-apitest-1.1.4/mwjApiTest/templates/request_file_demo/settings.py`

 * *Files identical despite different names*

### Comparing `mwj-apitest-1.1.3/mwj_apitest.egg-info/PKG-INFO` & `mwj-apitest-1.1.4/mwj_apitest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwj-apitest
-Version: 1.1.3
+Version: 1.1.4
 Summary: An execution engine for the interface automation platform
 Home-page: https://github.com/Lvan826199/mwjApiTest
 Author: 梦无矶小仔
 Author-email: Lvan826199@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mwj-apitest-1.1.3/mwj_apitest.egg-info/SOURCES.txt` & `mwj-apitest-1.1.4/mwj_apitest.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -28,8 +28,9 @@
 mwjApiTest/templates/request_file_demo/logs/__init__.py
 mwjApiTest/templates/request_file_demo/reports/__init__.py
 mwjApiTest/utils/__init__.py
 mwj_apitest.egg-info/PKG-INFO
 mwj_apitest.egg-info/SOURCES.txt
 mwj_apitest.egg-info/dependency_links.txt
 mwj_apitest.egg-info/entry_points.txt
+mwj_apitest.egg-info/requires.txt
 mwj_apitest.egg-info/top_level.txt
```

### Comparing `mwj-apitest-1.1.3/setup.py` & `mwj-apitest-1.1.4/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import setuptools  # 导入setuptools打包工具
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mwj-apitest",  # 用自己的名替换其中的YOUR_USERNAME_
-    version="1.1.3",  # 包版本号，便于维护版本,保证每次发布都是版本都是唯一的
+    version="1.1.4",  # 包版本号，便于维护版本,保证每次发布都是版本都是唯一的
     author="梦无矶小仔",  # 作者，可以写自己的姓名
     author_email="Lvan826199@163.com",  # 作者联系方式，可写自己的邮箱地址
     description="An execution engine for the interface automation platform",  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://github.com/Lvan826199/mwjApiTest",  # 自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
@@ -27,8 +27,18 @@
     },  # 安装成功后，在命令行输入mwj 就相当于执行了mwjApiTest.manage.py中的main了
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.8',  # 对python的最低版本要求
+    install_requires=[
+            "Faker==18.10.1",
+            "Jinja2==3.1.2",
+            "jsonpath==0.82",
+            "PyMySQL==1.0.2",
+            "PyYAML==6.0",
+            "Requests==2.31.0",
+            "requests_toolbelt==1.0.0",
+            "rsa==4.7.2",
+    ]
 )
```

