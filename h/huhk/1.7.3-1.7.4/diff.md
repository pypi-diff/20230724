# Comparing `tmp/huhk-1.7.3.tar.gz` & `tmp/huhk-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huhk-1.7.3.tar", last modified: Sat Jul 22 12:11:33 2023, max compression
+gzip compressed data, was "huhk-1.7.4.tar", last modified: Mon Jul 24 01:11:56 2023, max compression
```

## Comparing `huhk-1.7.3.tar` & `huhk-1.7.4.tar`

### file list

```diff
@@ -1,101 +1,93 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 12:11:33.333135 huhk-1.7.3/
--rw-rw-rw-   0        0        0      223 2023-07-22 12:11:33.332154 huhk-1.7.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-22 12:11:33.107858 huhk-1.7.3/huhk/
--rw-rw-rw-   0        0        0      772 2023-07-17 02:44:39.000000 huhk-1.7.3/huhk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 12:11:33.149311 huhk-1.7.3/huhk/case_project/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.7.3/huhk/case_project/__init__.py
--rw-rw-rw-   0        0        0      639 2023-07-12 01:13:24.000000 huhk-1.7.3/huhk/case_project/json_coder.py
--rw-rw-rw-   0        0        0      790 2023-07-13 02:39:46.000000 huhk-1.7.3/huhk/case_project/main.py
--rw-rw-rw-   0        0        0    17724 2023-07-22 12:10:44.000000 huhk-1.7.3/huhk/case_project/project_base.py
--rw-rw-rw-   0        0        0     2099 2023-07-21 08:18:22.000000 huhk-1.7.3/huhk/case_project/project_init.py
--rw-rw-rw-   0        0        0    13835 2023-07-22 10:45:49.000000 huhk-1.7.3/huhk/case_project/project_string.py
--rw-rw-rw-   0        0        0      908 2023-07-12 01:13:24.000000 huhk-1.7.3/huhk/case_project/setup_set.py
--rw-rw-rw-   0        0        0       17 2023-07-22 12:11:32.000000 huhk-1.7.3/huhk/case_project/version.py
--rw-rw-rw-   0        0        0    13183 2023-07-22 06:53:58.000000 huhk-1.7.3/huhk/init_project.py
--rw-rw-rw-   0        0        0      274 2023-07-12 01:13:24.000000 huhk-1.7.3/huhk/setup_run.py
-drwxrwxrwx   0        0        0        0 2023-07-22 12:11:33.153301 huhk-1.7.3/huhk/testcase/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.7.3/huhk/testcase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 12:11:33.220896 huhk-1.7.3/huhk/testcase/apache/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.7.3/huhk/testcase/apache/__init__.py
--rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.7.3/huhk/testcase/apache/beam_class.py
--rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.7.3/huhk/testcase/apache/data.py
--rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.7.3/huhk/testcase/apache/par_do.py
--rw-rw-rw-   0        0        0     7257 2023-07-14 06:52:17.000000 huhk-1.7.3/huhk/testcase/apache/test_cogroupbykey.py
--rw-rw-rw-   0        0        0      476 2023-07-14 06:52:17.000000 huhk-1.7.3/huhk/testcase/apache/test_file.py
--rw-rw-rw-   0        0        0     1503 2023-07-14 06:52:17.000000 huhk-1.7.3/huhk/testcase/apache/test_fiter.py
--rw-rw-rw-   0        0        0     2103 2023-07-14 06:52:17.000000 huhk-1.7.3/huhk/testcase/apache/test_flatmap.py
--rw-rw-rw-   0        0        0      523 2023-07-14 06:52:17.000000 huhk-1.7.3/huhk/testcase/apache/test_map.py
--rw-rw-rw-   0        0        0     2632 2023-07-14 07:03:11.000000 huhk-1.7.3/huhk/testcase/apache/test_par_do.py
--rw-rw-rw-   0        0        0     1651 2023-07-14 06:52:17.000000 huhk-1.7.3/huhk/testcase/apache/test_regex.py
--rw-rw-rw-   0        0        0     1571 2023-07-14 06:52:17.000000 huhk-1.7.3/huhk/testcase/apache/test_time.py
--rw-rw-rw-   0        0        0      508 2023-07-14 06:52:16.000000 huhk-1.7.3/huhk/testcase/apache/test_to_string.py
--rw-rw-rw-   0        0        0    22615 2023-07-14 06:52:17.000000 huhk-1.7.3/huhk/unit_apache_beam.py
--rw-rw-rw-   0        0        0     4508 2023-07-12 01:13:24.000000 huhk-1.7.3/huhk/unit_dict.py
--rw-rw-rw-   0        0        0     3843 2023-07-12 01:13:24.000000 huhk-1.7.3/huhk/unit_encryption.py
--rw-rw-rw-   0        0        0    28445 2023-07-22 10:41:46.000000 huhk-1.7.3/huhk/unit_fun.py
--rw-rw-rw-   0        0        0     1242 2023-07-12 01:13:24.000000 huhk-1.7.3/huhk/unit_logger.py
--rw-rw-rw-   0        0        0     9960 2023-07-22 07:06:52.000000 huhk-1.7.3/huhk/unit_request.py
--rw-rw-rw-   0        0        0     2473 2023-07-12 01:13:24.000000 huhk-1.7.3/huhk/unit_tasks.py
--rw-rw-rw-   0        0        0      733 2023-07-12 01:13:24.000000 huhk-1.7.3/huhk/常用命令.py
-drwxrwxrwx   0        0        0        0 2023-07-22 12:11:33.120389 huhk-1.7.3/huhk.egg-info/
--rw-rw-rw-   0        0        0      223 2023-07-22 12:11:32.000000 huhk-1.7.3/huhk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2603 2023-07-22 12:11:32.000000 huhk-1.7.3/huhk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 12:11:32.000000 huhk-1.7.3/huhk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-07-22 12:11:32.000000 huhk-1.7.3/huhk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      134 2023-07-22 12:11:32.000000 huhk-1.7.3/huhk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-22 12:11:32.000000 huhk-1.7.3/huhk.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-22 12:11:33.223888 huhk-1.7.3/service/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.7.3/service/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 12:11:33.231477 huhk-1.7.3/service/app_t/
--rw-rw-rw-   0        0        0      420 2023-07-22 06:54:11.000000 huhk-1.7.3/service/app_t/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 12:11:33.233467 huhk-1.7.3/service/app_t/apis/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.7.3/service/app_t/apis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 12:11:33.236460 huhk-1.7.3/service/app_t/apis/open/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.3/service/app_t/apis/open/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 12:11:33.245439 huhk-1.7.3/service/app_t/apis/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.3/service/app_t/apis/open/haohan/__init__.py
--rw-rw-rw-   0        0        0    14382 2023-07-22 12:06:26.000000 huhk-1.7.3/service/app_t/apis/open/haohan/apis_open_haohan_relation.py
--rw-rw-rw-   0        0        0    15042 2023-07-22 12:06:26.000000 huhk-1.7.3/service/app_t/apis/open/haohan/apis_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-07-22 12:11:33.252417 huhk-1.7.3/service/app_t/apis/points/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.3/service/app_t/apis/points/__init__.py
--rw-rw-rw-   0        0        0    21382 2023-07-22 12:06:26.000000 huhk-1.7.3/service/app_t/apis/points/apis_points_points.py
--rw-rw-rw-   0        0        0    17216 2023-07-22 12:06:26.000000 huhk-1.7.3/service/app_t/apis/points/apis_points_pointsApp.py
--rw-rw-rw-   0        0        0      650 2023-07-22 10:57:15.000000 huhk-1.7.3/service/app_t/app_t_fun.py
-drwxrwxrwx   0        0        0        0 2023-07-22 12:11:33.255409 huhk-1.7.3/service/app_t/asserts/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.7.3/service/app_t/asserts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 12:11:33.258412 huhk-1.7.3/service/app_t/asserts/open/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.3/service/app_t/asserts/open/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 12:11:33.267377 huhk-1.7.3/service/app_t/asserts/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.3/service/app_t/asserts/open/haohan/__init__.py
--rw-rw-rw-   0        0        0      602 2023-07-22 06:51:21.000000 huhk-1.7.3/service/app_t/asserts/open/haohan/asserts_open_haohan_relation.py
--rw-rw-rw-   0        0        0      590 2023-07-22 06:51:21.000000 huhk-1.7.3/service/app_t/asserts/open/haohan/asserts_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-07-22 12:11:33.278641 huhk-1.7.3/service/app_t/asserts/points/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.3/service/app_t/asserts/points/__init__.py
--rw-rw-rw-   0        0        0     1761 2023-07-22 07:08:51.000000 huhk-1.7.3/service/app_t/asserts/points/asserts_points_points.py
--rw-rw-rw-   0        0        0     1358 2023-07-22 06:51:21.000000 huhk-1.7.3/service/app_t/asserts/points/asserts_points_pointsApp.py
-drwxrwxrwx   0        0        0        0 2023-07-22 12:11:33.282157 huhk-1.7.3/service/app_t/funs/
--rw-rw-rw-   0        0        0        0 2023-07-22 12:06:26.000000 huhk-1.7.3/service/app_t/funs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 12:11:33.285140 huhk-1.7.3/service/app_t/funs/open/
--rw-rw-rw-   0        0        0        0 2023-07-22 12:06:26.000000 huhk-1.7.3/service/app_t/funs/open/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 12:11:33.297107 huhk-1.7.3/service/app_t/funs/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-07-22 12:06:26.000000 huhk-1.7.3/service/app_t/funs/open/haohan/__init__.py
--rw-rw-rw-   0        0        0      156 2023-07-22 12:06:26.000000 huhk-1.7.3/service/app_t/funs/open/haohan/funs_open_haohan.py
--rw-rw-rw-   0        0        0      824 2023-07-22 12:06:26.000000 huhk-1.7.3/service/app_t/funs/open/haohan/funs_open_haohan_relation.py
-drwxrwxrwx   0        0        0        0 2023-07-22 12:11:33.300099 huhk-1.7.3/service/app_t/sqls/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.7.3/service/app_t/sqls/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 12:11:33.303091 huhk-1.7.3/service/app_t/sqls/open/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.3/service/app_t/sqls/open/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 12:11:33.315060 huhk-1.7.3/service/app_t/sqls/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.3/service/app_t/sqls/open/haohan/__init__.py
--rw-rw-rw-   0        0        0      571 2023-07-22 06:51:21.000000 huhk-1.7.3/service/app_t/sqls/open/haohan/sqls_open_haohan_relation.py
--rw-rw-rw-   0        0        0      567 2023-07-22 06:51:21.000000 huhk-1.7.3/service/app_t/sqls/open/haohan/sqls_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-07-22 12:11:33.325032 huhk-1.7.3/service/app_t/sqls/points/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.3/service/app_t/sqls/points/__init__.py
--rw-rw-rw-   0        0        0     1994 2023-07-22 06:51:21.000000 huhk-1.7.3/service/app_t/sqls/points/sqls_points_points.py
--rw-rw-rw-   0        0        0     1529 2023-07-22 06:51:21.000000 huhk-1.7.3/service/app_t/sqls/points/sqls_points_pointsApp.py
--rw-rw-rw-   0        0        0       42 2023-07-22 12:11:33.334121 huhk-1.7.3/setup.cfg
--rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhk-1.7.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-22 12:11:33.327026 huhk-1.7.3/testcase/
--rw-rw-rw-   0        0        0        0 2023-07-22 07:30:21.000000 huhk-1.7.3/testcase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 12:11:33.330156 huhk-1.7.3/testcase/app_t/
--rw-rw-rw-   0        0        0        0 2023-07-22 07:30:21.000000 huhk-1.7.3/testcase/app_t/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 01:11:56.037210 huhk-1.7.4/
+-rw-rw-rw-   0        0        0      223 2023-07-24 01:11:56.036212 huhk-1.7.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-24 01:11:55.855955 huhk-1.7.4/huhk/
+-rw-rw-rw-   0        0        0      772 2023-07-17 02:44:39.000000 huhk-1.7.4/huhk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 01:11:55.893446 huhk-1.7.4/huhk/case_project/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.7.4/huhk/case_project/__init__.py
+-rw-rw-rw-   0        0        0      639 2023-07-12 01:13:24.000000 huhk-1.7.4/huhk/case_project/json_coder.py
+-rw-rw-rw-   0        0        0      790 2023-07-13 02:39:46.000000 huhk-1.7.4/huhk/case_project/main.py
+-rw-rw-rw-   0        0        0    17724 2023-07-22 12:10:44.000000 huhk-1.7.4/huhk/case_project/project_base.py
+-rw-rw-rw-   0        0        0     2099 2023-07-21 08:18:22.000000 huhk-1.7.4/huhk/case_project/project_init.py
+-rw-rw-rw-   0        0        0    13835 2023-07-22 10:45:49.000000 huhk-1.7.4/huhk/case_project/project_string.py
+-rw-rw-rw-   0        0        0      908 2023-07-12 01:13:24.000000 huhk-1.7.4/huhk/case_project/setup_set.py
+-rw-rw-rw-   0        0        0       17 2023-07-24 01:11:55.000000 huhk-1.7.4/huhk/case_project/version.py
+-rw-rw-rw-   0        0        0    13183 2023-07-22 06:53:58.000000 huhk-1.7.4/huhk/init_project.py
+-rw-rw-rw-   0        0        0      274 2023-07-12 01:13:24.000000 huhk-1.7.4/huhk/setup_run.py
+drwxrwxrwx   0        0        0        0 2023-07-24 01:11:55.897403 huhk-1.7.4/huhk/testcase/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.7.4/huhk/testcase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 01:11:55.952270 huhk-1.7.4/huhk/testcase/apache/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.7.4/huhk/testcase/apache/__init__.py
+-rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.7.4/huhk/testcase/apache/beam_class.py
+-rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.7.4/huhk/testcase/apache/data.py
+-rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.7.4/huhk/testcase/apache/par_do.py
+-rw-rw-rw-   0        0        0     7257 2023-07-14 06:52:17.000000 huhk-1.7.4/huhk/testcase/apache/test_cogroupbykey.py
+-rw-rw-rw-   0        0        0      476 2023-07-14 06:52:17.000000 huhk-1.7.4/huhk/testcase/apache/test_file.py
+-rw-rw-rw-   0        0        0     1503 2023-07-14 06:52:17.000000 huhk-1.7.4/huhk/testcase/apache/test_fiter.py
+-rw-rw-rw-   0        0        0     2103 2023-07-14 06:52:17.000000 huhk-1.7.4/huhk/testcase/apache/test_flatmap.py
+-rw-rw-rw-   0        0        0      523 2023-07-14 06:52:17.000000 huhk-1.7.4/huhk/testcase/apache/test_map.py
+-rw-rw-rw-   0        0        0     2632 2023-07-14 07:03:11.000000 huhk-1.7.4/huhk/testcase/apache/test_par_do.py
+-rw-rw-rw-   0        0        0     1651 2023-07-14 06:52:17.000000 huhk-1.7.4/huhk/testcase/apache/test_regex.py
+-rw-rw-rw-   0        0        0     1571 2023-07-14 06:52:17.000000 huhk-1.7.4/huhk/testcase/apache/test_time.py
+-rw-rw-rw-   0        0        0      508 2023-07-14 06:52:16.000000 huhk-1.7.4/huhk/testcase/apache/test_to_string.py
+-rw-rw-rw-   0        0        0    22615 2023-07-14 06:52:17.000000 huhk-1.7.4/huhk/unit_apache_beam.py
+-rw-rw-rw-   0        0        0     4508 2023-07-12 01:13:24.000000 huhk-1.7.4/huhk/unit_dict.py
+-rw-rw-rw-   0        0        0     3843 2023-07-12 01:13:24.000000 huhk-1.7.4/huhk/unit_encryption.py
+-rw-rw-rw-   0        0        0    28445 2023-07-22 10:41:46.000000 huhk-1.7.4/huhk/unit_fun.py
+-rw-rw-rw-   0        0        0     1242 2023-07-12 01:13:24.000000 huhk-1.7.4/huhk/unit_logger.py
+-rw-rw-rw-   0        0        0     9960 2023-07-22 07:06:52.000000 huhk-1.7.4/huhk/unit_request.py
+-rw-rw-rw-   0        0        0     2473 2023-07-12 01:13:24.000000 huhk-1.7.4/huhk/unit_tasks.py
+-rw-rw-rw-   0        0        0      733 2023-07-12 01:13:24.000000 huhk-1.7.4/huhk/常用命令.py
+drwxrwxrwx   0        0        0        0 2023-07-24 01:11:55.868899 huhk-1.7.4/huhk.egg-info/
+-rw-rw-rw-   0        0        0      223 2023-07-24 01:11:55.000000 huhk-1.7.4/huhk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2382 2023-07-24 01:11:55.000000 huhk-1.7.4/huhk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 01:11:55.000000 huhk-1.7.4/huhk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-07-24 01:11:55.000000 huhk-1.7.4/huhk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      134 2023-07-24 01:11:55.000000 huhk-1.7.4/huhk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-24 01:11:55.000000 huhk-1.7.4/huhk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 01:11:55.955249 huhk-1.7.4/service/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.7.4/service/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 01:11:55.962850 huhk-1.7.4/service/app_t/
+-rw-rw-rw-   0        0        0      420 2023-07-22 06:54:11.000000 huhk-1.7.4/service/app_t/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 01:11:55.964806 huhk-1.7.4/service/app_t/apis/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.7.4/service/app_t/apis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 01:11:55.967796 huhk-1.7.4/service/app_t/apis/open/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.4/service/app_t/apis/open/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 01:11:55.975775 huhk-1.7.4/service/app_t/apis/open/haohan/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.4/service/app_t/apis/open/haohan/__init__.py
+-rw-rw-rw-   0        0        0    14382 2023-07-22 12:06:26.000000 huhk-1.7.4/service/app_t/apis/open/haohan/apis_open_haohan_relation.py
+-rw-rw-rw-   0        0        0    15042 2023-07-22 12:06:26.000000 huhk-1.7.4/service/app_t/apis/open/haohan/apis_open_haohan_rights.py
+drwxrwxrwx   0        0        0        0 2023-07-24 01:11:55.983775 huhk-1.7.4/service/app_t/apis/points/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.4/service/app_t/apis/points/__init__.py
+-rw-rw-rw-   0        0        0    21382 2023-07-22 12:06:26.000000 huhk-1.7.4/service/app_t/apis/points/apis_points_points.py
+-rw-rw-rw-   0        0        0    17216 2023-07-22 12:06:26.000000 huhk-1.7.4/service/app_t/apis/points/apis_points_pointsApp.py
+-rw-rw-rw-   0        0        0      650 2023-07-22 10:57:15.000000 huhk-1.7.4/service/app_t/app_t_fun.py
+drwxrwxrwx   0        0        0        0 2023-07-24 01:11:55.985748 huhk-1.7.4/service/app_t/asserts/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.7.4/service/app_t/asserts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 01:11:55.988338 huhk-1.7.4/service/app_t/asserts/open/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.4/service/app_t/asserts/open/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 01:11:55.997344 huhk-1.7.4/service/app_t/asserts/open/haohan/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.4/service/app_t/asserts/open/haohan/__init__.py
+-rw-rw-rw-   0        0        0      602 2023-07-22 06:51:21.000000 huhk-1.7.4/service/app_t/asserts/open/haohan/asserts_open_haohan_relation.py
+-rw-rw-rw-   0        0        0      590 2023-07-22 06:51:21.000000 huhk-1.7.4/service/app_t/asserts/open/haohan/asserts_open_haohan_rights.py
+drwxrwxrwx   0        0        0        0 2023-07-24 01:11:56.006292 huhk-1.7.4/service/app_t/asserts/points/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.4/service/app_t/asserts/points/__init__.py
+-rw-rw-rw-   0        0        0     1761 2023-07-22 07:08:51.000000 huhk-1.7.4/service/app_t/asserts/points/asserts_points_points.py
+-rw-rw-rw-   0        0        0     1358 2023-07-22 06:51:21.000000 huhk-1.7.4/service/app_t/asserts/points/asserts_points_pointsApp.py
+drwxrwxrwx   0        0        0        0 2023-07-24 01:11:56.009284 huhk-1.7.4/service/app_t/sqls/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.7.4/service/app_t/sqls/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 01:11:56.012276 huhk-1.7.4/service/app_t/sqls/open/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.4/service/app_t/sqls/open/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 01:11:56.020258 huhk-1.7.4/service/app_t/sqls/open/haohan/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.4/service/app_t/sqls/open/haohan/__init__.py
+-rw-rw-rw-   0        0        0      571 2023-07-22 06:51:21.000000 huhk-1.7.4/service/app_t/sqls/open/haohan/sqls_open_haohan_relation.py
+-rw-rw-rw-   0        0        0      567 2023-07-22 06:51:21.000000 huhk-1.7.4/service/app_t/sqls/open/haohan/sqls_open_haohan_rights.py
+drwxrwxrwx   0        0        0        0 2023-07-24 01:11:56.028235 huhk-1.7.4/service/app_t/sqls/points/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.4/service/app_t/sqls/points/__init__.py
+-rw-rw-rw-   0        0        0     1994 2023-07-22 06:51:21.000000 huhk-1.7.4/service/app_t/sqls/points/sqls_points_points.py
+-rw-rw-rw-   0        0        0     1529 2023-07-22 06:51:21.000000 huhk-1.7.4/service/app_t/sqls/points/sqls_points_pointsApp.py
+-rw-rw-rw-   0        0        0       42 2023-07-24 01:11:56.037210 huhk-1.7.4/setup.cfg
+-rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhk-1.7.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 01:11:56.031227 huhk-1.7.4/testcase/
+-rw-rw-rw-   0        0        0        0 2023-07-22 07:30:21.000000 huhk-1.7.4/testcase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 01:11:56.033222 huhk-1.7.4/testcase/app_t/
+-rw-rw-rw-   0        0        0        0 2023-07-22 07:30:21.000000 huhk-1.7.4/testcase/app_t/__init__.py
```

### Comparing `huhk-1.7.3/huhk/__init__.py` & `huhk-1.7.4/huhk/__init__.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.3/huhk/case_project/json_coder.py` & `huhk-1.7.4/huhk/case_project/json_coder.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.3/huhk/case_project/main.py` & `huhk-1.7.4/huhk/case_project/main.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.3/huhk/case_project/project_base.py` & `huhk-1.7.4/huhk/case_project/project_base.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.3/huhk/case_project/project_init.py` & `huhk-1.7.4/huhk/case_project/project_init.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.3/huhk/case_project/project_string.py` & `huhk-1.7.4/huhk/case_project/project_string.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.3/huhk/case_project/setup_set.py` & `huhk-1.7.4/huhk/case_project/setup_set.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.3/huhk/init_project.py` & `huhk-1.7.4/huhk/init_project.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.3/huhk/testcase/apache/beam_class.py` & `huhk-1.7.4/huhk/testcase/apache/beam_class.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.3/huhk/testcase/apache/data.py` & `huhk-1.7.4/huhk/testcase/apache/data.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.3/huhk/testcase/apache/par_do.py` & `huhk-1.7.4/huhk/testcase/apache/par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.3/huhk/testcase/apache/test_cogroupbykey.py` & `huhk-1.7.4/huhk/testcase/apache/test_cogroupbykey.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.3/huhk/testcase/apache/test_fiter.py` & `huhk-1.7.4/huhk/testcase/apache/test_fiter.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.3/huhk/testcase/apache/test_flatmap.py` & `huhk-1.7.4/huhk/testcase/apache/test_flatmap.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.3/huhk/testcase/apache/test_map.py` & `huhk-1.7.4/huhk/testcase/apache/test_map.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.3/huhk/testcase/apache/test_par_do.py` & `huhk-1.7.4/huhk/testcase/apache/test_par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.3/huhk/testcase/apache/test_regex.py` & `huhk-1.7.4/huhk/testcase/apache/test_regex.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.3/huhk/testcase/apache/test_time.py` & `huhk-1.7.4/huhk/testcase/apache/test_time.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.3/huhk/unit_apache_beam.py` & `huhk-1.7.4/huhk/unit_apache_beam.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.3/huhk/unit_dict.py` & `huhk-1.7.4/huhk/unit_dict.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.3/huhk/unit_encryption.py` & `huhk-1.7.4/huhk/unit_encryption.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.3/huhk/unit_fun.py` & `huhk-1.7.4/huhk/unit_fun.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.3/huhk/unit_logger.py` & `huhk-1.7.4/huhk/unit_logger.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.3/huhk/unit_request.py` & `huhk-1.7.4/huhk/unit_request.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.3/huhk/unit_tasks.py` & `huhk-1.7.4/huhk/unit_tasks.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.3/huhk/常用命令.py` & `huhk-1.7.4/huhk/常用命令.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.3/huhk.egg-info/SOURCES.txt` & `huhk-1.7.4/huhk.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -53,19 +53,14 @@
 service/app_t/asserts/open/__init__.py
 service/app_t/asserts/open/haohan/__init__.py
 service/app_t/asserts/open/haohan/asserts_open_haohan_relation.py
 service/app_t/asserts/open/haohan/asserts_open_haohan_rights.py
 service/app_t/asserts/points/__init__.py
 service/app_t/asserts/points/asserts_points_points.py
 service/app_t/asserts/points/asserts_points_pointsApp.py
-service/app_t/funs/__init__.py
-service/app_t/funs/open/__init__.py
-service/app_t/funs/open/haohan/__init__.py
-service/app_t/funs/open/haohan/funs_open_haohan.py
-service/app_t/funs/open/haohan/funs_open_haohan_relation.py
 service/app_t/sqls/__init__.py
 service/app_t/sqls/open/__init__.py
 service/app_t/sqls/open/haohan/__init__.py
 service/app_t/sqls/open/haohan/sqls_open_haohan_relation.py
 service/app_t/sqls/open/haohan/sqls_open_haohan_rights.py
 service/app_t/sqls/points/__init__.py
 service/app_t/sqls/points/sqls_points_points.py
```

### Comparing `huhk-1.7.3/service/app_t/apis/open/haohan/apis_open_haohan_relation.py` & `huhk-1.7.4/service/app_t/apis/open/haohan/apis_open_haohan_relation.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.3/service/app_t/apis/open/haohan/apis_open_haohan_rights.py` & `huhk-1.7.4/service/app_t/apis/open/haohan/apis_open_haohan_rights.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.3/service/app_t/apis/points/apis_points_points.py` & `huhk-1.7.4/service/app_t/apis/points/apis_points_points.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.3/service/app_t/apis/points/apis_points_pointsApp.py` & `huhk-1.7.4/service/app_t/apis/points/apis_points_pointsApp.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.3/service/app_t/app_t_fun.py` & `huhk-1.7.4/service/app_t/app_t_fun.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.3/service/app_t/asserts/open/haohan/asserts_open_haohan_relation.py` & `huhk-1.7.4/service/app_t/asserts/open/haohan/asserts_open_haohan_relation.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.3/service/app_t/asserts/open/haohan/asserts_open_haohan_rights.py` & `huhk-1.7.4/service/app_t/asserts/open/haohan/asserts_open_haohan_rights.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.3/service/app_t/asserts/points/asserts_points_points.py` & `huhk-1.7.4/service/app_t/asserts/points/asserts_points_points.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.3/service/app_t/asserts/points/asserts_points_pointsApp.py` & `huhk-1.7.4/service/app_t/asserts/points/asserts_points_pointsApp.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.3/service/app_t/sqls/open/haohan/sqls_open_haohan_relation.py` & `huhk-1.7.4/service/app_t/sqls/open/haohan/sqls_open_haohan_relation.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.3/service/app_t/sqls/open/haohan/sqls_open_haohan_rights.py` & `huhk-1.7.4/service/app_t/sqls/open/haohan/sqls_open_haohan_rights.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.3/service/app_t/sqls/points/sqls_points_points.py` & `huhk-1.7.4/service/app_t/sqls/points/sqls_points_points.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.3/service/app_t/sqls/points/sqls_points_pointsApp.py` & `huhk-1.7.4/service/app_t/sqls/points/sqls_points_pointsApp.py`

 * *Files identical despite different names*

