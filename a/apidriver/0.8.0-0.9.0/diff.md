# Comparing `tmp/apidriver-0.8.0.tar.gz` & `tmp/apidriver-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apidriver-0.8.0.tar", last modified: Tue Jul  4 01:40:20 2023, max compression
+gzip compressed data, was "apidriver-0.9.0.tar", last modified: Mon Jul 24 07:11:21 2023, max compression
```

## Comparing `apidriver-0.8.0.tar` & `apidriver-0.9.0.tar`

### file list

```diff
@@ -1,44 +1,46 @@
-drwxr-xr-x   0 chnjx      (501) staff       (20)        0 2023-07-04 01:40:20.070278 apidriver-0.8.0/
--rw-r--r--   0 chnjx      (501) staff       (20)     1068 2023-02-07 12:22:16.000000 apidriver-0.8.0/LICENSE.txt
--rw-r--r--   0 chnjx      (501) staff       (20)       84 2023-03-15 15:32:00.000000 apidriver-0.8.0/MANIFEST.in
--rw-r--r--   0 chnjx      (501) staff       (20)      239 2023-07-04 01:40:20.069604 apidriver-0.8.0/PKG-INFO
--rw-r--r--   0 chnjx      (501) staff       (20)     3340 2023-04-13 12:44:49.000000 apidriver-0.8.0/README.md
-drwxr-xr-x   0 chnjx      (501) staff       (20)        0 2023-07-04 01:40:20.057227 apidriver-0.8.0/api_driver/
--rw-r--r--   0 chnjx      (501) staff       (20)       64 2023-03-14 14:16:04.000000 apidriver-0.8.0/api_driver/__init__.py
--rw-r--r--   0 chnjx      (501) staff       (20)      120 2023-03-15 15:01:02.000000 apidriver-0.8.0/api_driver/__main__.py
--rw-r--r--   0 chnjx      (501) staff       (20)      127 2023-07-04 01:38:12.000000 apidriver-0.8.0/api_driver/_version.py
--rw-r--r--   0 chnjx      (501) staff       (20)     2712 2023-07-04 01:36:23.000000 apidriver-0.8.0/api_driver/ad_utils.py
--rw-r--r--   0 chnjx      (501) staff       (20)     2971 2023-03-15 15:08:27.000000 apidriver-0.8.0/api_driver/command.py
--rw-r--r--   0 chnjx      (501) staff       (20)    14714 2023-04-13 12:44:49.000000 apidriver-0.8.0/api_driver/har_parser.py
--rw-r--r--   0 chnjx      (501) staff       (20)     2278 2023-04-13 12:44:49.000000 apidriver-0.8.0/api_driver/loader_swagger.py
--rw-r--r--   0 chnjx      (501) staff       (20)     4417 2023-04-13 12:44:49.000000 apidriver-0.8.0/api_driver/project_generator.py
--rw-r--r--   0 chnjx      (501) staff       (20)     8018 2023-04-13 12:44:49.000000 apidriver-0.8.0/api_driver/swagger_generate.py
--rw-r--r--   0 chnjx      (501) staff       (20)      485 2023-04-13 12:44:49.000000 apidriver-0.8.0/api_driver/template.py
-drwxr-xr-x   0 chnjx      (501) staff       (20)        0 2023-07-04 01:40:20.060954 apidriver-0.8.0/api_driver/templates/
--rw-r--r--   0 chnjx      (501) staff       (20)     2121 2023-04-13 12:44:49.000000 apidriver-0.8.0/api_driver/templates/api.tpl
--rw-r--r--   0 chnjx      (501) staff       (20)      374 2023-03-15 15:46:44.000000 apidriver-0.8.0/api_driver/templates/api_demo.tpl
--rw-r--r--   0 chnjx      (501) staff       (20)      398 2023-03-15 15:08:27.000000 apidriver-0.8.0/api_driver/templates/base_testcase.tpl
--rw-r--r--   0 chnjx      (501) staff       (20)     2879 2023-03-15 15:12:01.000000 apidriver-0.8.0/api_driver/templates/har2api_case.tpl
--rw-r--r--   0 chnjx      (501) staff       (20)     2242 2023-03-15 15:12:01.000000 apidriver-0.8.0/api_driver/templates/har2case.tpl
--rw-r--r--   0 chnjx      (501) staff       (20)     5224 2023-04-13 12:44:49.000000 apidriver-0.8.0/api_driver/templates/http.tpl
--rw-r--r--   0 chnjx      (501) staff       (20)      355 2023-03-15 13:14:27.000000 apidriver-0.8.0/api_driver/templates/testcase_demo.tpl
--rw-r--r--   0 chnjx      (501) staff       (20)     2933 2023-04-13 12:44:49.000000 apidriver-0.8.0/api_driver/testcase_mixin.py
-drwxr-xr-x   0 chnjx      (501) staff       (20)        0 2023-07-04 01:40:20.064374 apidriver-0.8.0/api_driver/utils/
--rw-r--r--   0 chnjx      (501) staff       (20)        0 2023-02-07 12:22:16.000000 apidriver-0.8.0/api_driver/utils/__init__.py
--rw-r--r--   0 chnjx      (501) staff       (20)     1043 2023-03-15 15:08:27.000000 apidriver-0.8.0/api_driver/utils/custom_str_utils.py
--rw-r--r--   0 chnjx      (501) staff       (20)     1882 2023-03-14 13:52:12.000000 apidriver-0.8.0/api_driver/utils/database_conn.py
--rw-r--r--   0 chnjx      (501) staff       (20)     3322 2023-03-14 13:52:12.000000 apidriver-0.8.0/api_driver/utils/fake.py
--rw-r--r--   0 chnjx      (501) staff       (20)     2172 2023-03-15 15:08:27.000000 apidriver-0.8.0/api_driver/utils/placeholder.py
--rw-r--r--   0 chnjx      (501) staff       (20)     1283 2023-02-17 12:48:23.000000 apidriver-0.8.0/api_driver/utils/service_logger.py
-drwxr-xr-x   0 chnjx      (501) staff       (20)        0 2023-07-04 01:40:20.068155 apidriver-0.8.0/apidriver.egg-info/
--rw-r--r--   0 chnjx      (501) staff       (20)      239 2023-07-04 01:40:20.000000 apidriver-0.8.0/apidriver.egg-info/PKG-INFO
--rw-r--r--   0 chnjx      (501) staff       (20)      994 2023-07-04 01:40:20.000000 apidriver-0.8.0/apidriver.egg-info/SOURCES.txt
--rw-r--r--   0 chnjx      (501) staff       (20)        1 2023-07-04 01:40:20.000000 apidriver-0.8.0/apidriver.egg-info/dependency_links.txt
--rw-r--r--   0 chnjx      (501) staff       (20)       40 2023-07-04 01:40:20.000000 apidriver-0.8.0/apidriver.egg-info/entry_points.txt
--rw-r--r--   0 chnjx      (501) staff       (20)      171 2023-07-04 01:40:20.000000 apidriver-0.8.0/apidriver.egg-info/requires.txt
--rw-r--r--   0 chnjx      (501) staff       (20)       11 2023-07-04 01:40:20.000000 apidriver-0.8.0/apidriver.egg-info/top_level.txt
--rw-r--r--   0 chnjx      (501) staff       (20)      170 2023-04-13 12:44:49.000000 apidriver-0.8.0/requirements.txt
--rw-r--r--   0 chnjx      (501) staff       (20)       38 2023-07-04 01:40:20.070571 apidriver-0.8.0/setup.cfg
--rw-r--r--   0 chnjx      (501) staff       (20)      903 2023-04-13 12:44:49.000000 apidriver-0.8.0/setup.py
-drwxr-xr-x   0 chnjx      (501) staff       (20)        0 2023-07-04 01:40:20.068739 apidriver-0.8.0/test/
--rw-r--r--   0 chnjx      (501) staff       (20)     1105 2023-04-13 12:44:49.000000 apidriver-0.8.0/test/test_cli.py
+drwxr-xr-x   0 chnjx      (501) staff       (20)        0 2023-07-24 07:11:21.031938 apidriver-0.9.0/
+-rw-r--r--   0 chnjx      (501) staff       (20)     1068 2023-02-07 12:22:16.000000 apidriver-0.9.0/LICENSE.txt
+-rw-r--r--   0 chnjx      (501) staff       (20)       84 2023-03-15 15:32:00.000000 apidriver-0.9.0/MANIFEST.in
+-rw-r--r--   0 chnjx      (501) staff       (20)      209 2023-07-24 07:11:21.030928 apidriver-0.9.0/PKG-INFO
+-rw-r--r--   0 chnjx      (501) staff       (20)     3340 2023-04-13 12:44:49.000000 apidriver-0.9.0/README.md
+drwxr-xr-x   0 chnjx      (501) staff       (20)        0 2023-07-24 07:11:21.001855 apidriver-0.9.0/api_driver/
+-rw-r--r--   0 chnjx      (501) staff       (20)       64 2023-03-14 14:16:04.000000 apidriver-0.9.0/api_driver/__init__.py
+-rw-r--r--   0 chnjx      (501) staff       (20)      120 2023-03-15 15:01:02.000000 apidriver-0.9.0/api_driver/__main__.py
+-rw-r--r--   0 chnjx      (501) staff       (20)      127 2023-07-24 07:06:07.000000 apidriver-0.9.0/api_driver/_version.py
+-rw-r--r--   0 chnjx      (501) staff       (20)     2712 2023-07-04 01:36:23.000000 apidriver-0.9.0/api_driver/ad_utils.py
+-rw-r--r--   0 chnjx      (501) staff       (20)     3483 2023-07-24 07:00:48.000000 apidriver-0.9.0/api_driver/api_driver.py
+-rw-r--r--   0 chnjx      (501) staff       (20)     2971 2023-03-15 15:08:27.000000 apidriver-0.9.0/api_driver/command.py
+-rw-r--r--   0 chnjx      (501) staff       (20)    14714 2023-04-13 12:44:49.000000 apidriver-0.9.0/api_driver/har_parser.py
+-rw-r--r--   0 chnjx      (501) staff       (20)     2278 2023-04-13 12:44:49.000000 apidriver-0.9.0/api_driver/loader_swagger.py
+-rw-r--r--   0 chnjx      (501) staff       (20)     4417 2023-04-13 12:44:49.000000 apidriver-0.9.0/api_driver/project_generator.py
+-rw-r--r--   0 chnjx      (501) staff       (20)     8018 2023-04-13 12:44:49.000000 apidriver-0.9.0/api_driver/swagger_generate.py
+-rw-r--r--   0 chnjx      (501) staff       (20)      485 2023-04-13 12:44:49.000000 apidriver-0.9.0/api_driver/template.py
+drwxr-xr-x   0 chnjx      (501) staff       (20)        0 2023-07-24 07:11:21.013247 apidriver-0.9.0/api_driver/templates/
+-rw-r--r--   0 chnjx      (501) staff       (20)     2121 2023-04-13 12:44:49.000000 apidriver-0.9.0/api_driver/templates/api.tpl
+-rw-r--r--   0 chnjx      (501) staff       (20)      374 2023-03-15 15:46:44.000000 apidriver-0.9.0/api_driver/templates/api_demo.tpl
+-rw-r--r--   0 chnjx      (501) staff       (20)      398 2023-03-15 15:08:27.000000 apidriver-0.9.0/api_driver/templates/base_testcase.tpl
+-rw-r--r--   0 chnjx      (501) staff       (20)     2879 2023-03-15 15:12:01.000000 apidriver-0.9.0/api_driver/templates/har2api_case.tpl
+-rw-r--r--   0 chnjx      (501) staff       (20)     2242 2023-03-15 15:12:01.000000 apidriver-0.9.0/api_driver/templates/har2case.tpl
+-rw-r--r--   0 chnjx      (501) staff       (20)     5224 2023-04-13 12:44:49.000000 apidriver-0.9.0/api_driver/templates/http.tpl
+-rw-r--r--   0 chnjx      (501) staff       (20)    15328 2023-07-24 07:03:03.000000 apidriver-0.9.0/api_driver/templates/report_template.html
+-rw-r--r--   0 chnjx      (501) staff       (20)      355 2023-03-15 13:14:27.000000 apidriver-0.9.0/api_driver/templates/testcase_demo.tpl
+-rw-r--r--   0 chnjx      (501) staff       (20)     2933 2023-04-13 12:44:49.000000 apidriver-0.9.0/api_driver/testcase_mixin.py
+drwxr-xr-x   0 chnjx      (501) staff       (20)        0 2023-07-24 07:11:21.019937 apidriver-0.9.0/api_driver/utils/
+-rw-r--r--   0 chnjx      (501) staff       (20)        0 2023-02-07 12:22:16.000000 apidriver-0.9.0/api_driver/utils/__init__.py
+-rw-r--r--   0 chnjx      (501) staff       (20)     1043 2023-03-15 15:08:27.000000 apidriver-0.9.0/api_driver/utils/custom_str_utils.py
+-rw-r--r--   0 chnjx      (501) staff       (20)     1882 2023-03-14 13:52:12.000000 apidriver-0.9.0/api_driver/utils/database_conn.py
+-rw-r--r--   0 chnjx      (501) staff       (20)     3322 2023-03-14 13:52:12.000000 apidriver-0.9.0/api_driver/utils/fake.py
+-rw-r--r--   0 chnjx      (501) staff       (20)     2172 2023-03-15 15:08:27.000000 apidriver-0.9.0/api_driver/utils/placeholder.py
+-rw-r--r--   0 chnjx      (501) staff       (20)     1283 2023-02-17 12:48:23.000000 apidriver-0.9.0/api_driver/utils/service_logger.py
+drwxr-xr-x   0 chnjx      (501) staff       (20)        0 2023-07-24 07:11:21.027824 apidriver-0.9.0/apidriver.egg-info/
+-rw-r--r--   0 chnjx      (501) staff       (20)      209 2023-07-24 07:11:20.000000 apidriver-0.9.0/apidriver.egg-info/PKG-INFO
+-rw-r--r--   0 chnjx      (501) staff       (20)     1061 2023-07-24 07:11:20.000000 apidriver-0.9.0/apidriver.egg-info/SOURCES.txt
+-rw-r--r--   0 chnjx      (501) staff       (20)        1 2023-07-24 07:11:20.000000 apidriver-0.9.0/apidriver.egg-info/dependency_links.txt
+-rw-r--r--   0 chnjx      (501) staff       (20)       39 2023-07-24 07:11:20.000000 apidriver-0.9.0/apidriver.egg-info/entry_points.txt
+-rw-r--r--   0 chnjx      (501) staff       (20)      171 2023-07-24 07:11:20.000000 apidriver-0.9.0/apidriver.egg-info/requires.txt
+-rw-r--r--   0 chnjx      (501) staff       (20)       11 2023-07-24 07:11:20.000000 apidriver-0.9.0/apidriver.egg-info/top_level.txt
+-rw-r--r--   0 chnjx      (501) staff       (20)      170 2023-04-13 12:44:49.000000 apidriver-0.9.0/requirements.txt
+-rw-r--r--   0 chnjx      (501) staff       (20)       38 2023-07-24 07:11:21.032253 apidriver-0.9.0/setup.cfg
+-rw-r--r--   0 chnjx      (501) staff       (20)      903 2023-04-13 12:44:49.000000 apidriver-0.9.0/setup.py
+drwxr-xr-x   0 chnjx      (501) staff       (20)        0 2023-07-24 07:11:21.029474 apidriver-0.9.0/test/
+-rw-r--r--   0 chnjx      (501) staff       (20)     1105 2023-04-13 12:44:49.000000 apidriver-0.9.0/test/test_cli.py
```

### Comparing `apidriver-0.8.0/LICENSE.txt` & `apidriver-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apidriver-0.8.0/README.md` & `apidriver-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `apidriver-0.8.0/api_driver/ad_utils.py` & `apidriver-0.9.0/api_driver/ad_utils.py`

 * *Files identical despite different names*

### Comparing `apidriver-0.8.0/api_driver/command.py` & `apidriver-0.9.0/api_driver/command.py`

 * *Files identical despite different names*

### Comparing `apidriver-0.8.0/api_driver/har_parser.py` & `apidriver-0.9.0/api_driver/har_parser.py`

 * *Files identical despite different names*

### Comparing `apidriver-0.8.0/api_driver/loader_swagger.py` & `apidriver-0.9.0/api_driver/loader_swagger.py`

 * *Files identical despite different names*

### Comparing `apidriver-0.8.0/api_driver/project_generator.py` & `apidriver-0.9.0/api_driver/project_generator.py`

 * *Files identical despite different names*

### Comparing `apidriver-0.8.0/api_driver/swagger_generate.py` & `apidriver-0.9.0/api_driver/swagger_generate.py`

 * *Files identical despite different names*

### Comparing `apidriver-0.8.0/api_driver/templates/api.tpl` & `apidriver-0.9.0/api_driver/templates/api.tpl`

 * *Files identical despite different names*

### Comparing `apidriver-0.8.0/api_driver/templates/har2api_case.tpl` & `apidriver-0.9.0/api_driver/templates/har2api_case.tpl`

 * *Files identical despite different names*

### Comparing `apidriver-0.8.0/api_driver/templates/har2case.tpl` & `apidriver-0.9.0/api_driver/templates/har2case.tpl`

 * *Files identical despite different names*

### Comparing `apidriver-0.8.0/api_driver/templates/http.tpl` & `apidriver-0.9.0/api_driver/templates/http.tpl`

 * *Files identical despite different names*

### Comparing `apidriver-0.8.0/api_driver/testcase_mixin.py` & `apidriver-0.9.0/api_driver/testcase_mixin.py`

 * *Files identical despite different names*

### Comparing `apidriver-0.8.0/api_driver/utils/custom_str_utils.py` & `apidriver-0.9.0/api_driver/utils/custom_str_utils.py`

 * *Files identical despite different names*

### Comparing `apidriver-0.8.0/api_driver/utils/database_conn.py` & `apidriver-0.9.0/api_driver/utils/database_conn.py`

 * *Files identical despite different names*

### Comparing `apidriver-0.8.0/api_driver/utils/fake.py` & `apidriver-0.9.0/api_driver/utils/fake.py`

 * *Files identical despite different names*

### Comparing `apidriver-0.8.0/api_driver/utils/placeholder.py` & `apidriver-0.9.0/api_driver/utils/placeholder.py`

 * *Files identical despite different names*

### Comparing `apidriver-0.8.0/api_driver/utils/service_logger.py` & `apidriver-0.9.0/api_driver/utils/service_logger.py`

 * *Files identical despite different names*

### Comparing `apidriver-0.8.0/apidriver.egg-info/SOURCES.txt` & `apidriver-0.9.0/apidriver.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -3,27 +3,29 @@
 README.md
 requirements.txt
 setup.py
 api_driver/__init__.py
 api_driver/__main__.py
 api_driver/_version.py
 api_driver/ad_utils.py
+api_driver/api_driver.py
 api_driver/command.py
 api_driver/har_parser.py
 api_driver/loader_swagger.py
 api_driver/project_generator.py
 api_driver/swagger_generate.py
 api_driver/template.py
 api_driver/testcase_mixin.py
 api_driver/templates/api.tpl
 api_driver/templates/api_demo.tpl
 api_driver/templates/base_testcase.tpl
 api_driver/templates/har2api_case.tpl
 api_driver/templates/har2case.tpl
 api_driver/templates/http.tpl
+api_driver/templates/report_template.html
 api_driver/templates/testcase_demo.tpl
 api_driver/utils/__init__.py
 api_driver/utils/custom_str_utils.py
 api_driver/utils/database_conn.py
 api_driver/utils/fake.py
 api_driver/utils/placeholder.py
 api_driver/utils/service_logger.py
```

### Comparing `apidriver-0.8.0/setup.py` & `apidriver-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `apidriver-0.8.0/test/test_cli.py` & `apidriver-0.9.0/test/test_cli.py`

 * *Files identical despite different names*

