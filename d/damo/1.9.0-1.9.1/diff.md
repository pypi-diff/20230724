# Comparing `tmp/damo-1.9.0.tar.gz` & `tmp/damo-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "damo-1.9.0.tar", last modified: Mon Jul 17 23:20:07 2023, max compression
+gzip compressed data, was "damo-1.9.1.tar", last modified: Mon Jul 24 17:11:40 2023, max compression
```

## Comparing `damo-1.9.0.tar` & `damo-1.9.1.tar`

### file list

```diff
@@ -1,55 +1,51 @@
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-07-17 23:20:07.296029 damo-1.9.0/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8366 2023-07-17 23:20:07.296029 damo-1.9.0/PKG-INFO
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7845 2023-07-17 23:20:02.000000 damo-1.9.0/README.md
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      104 2022-04-22 09:53:30.000000 damo-1.9.0/pyproject.toml
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       38 2023-07-17 23:20:07.296029 damo-1.9.0/setup.cfg
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1104 2023-05-13 14:44:13.000000 damo-1.9.0/setup.py
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-07-17 23:20:07.268030 damo-1.9.0/src/
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-07-17 23:20:07.292029 damo-1.9.0/src/damo/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        0 2023-07-17 23:20:02.000000 damo-1.9.0/src/damo/__init__.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7357 2023-07-04 00:27:48.000000 damo-1.9.0/src/damo/_damo_deprecated.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      963 2023-05-21 19:11:52.000000 damo-1.9.0/src/damo/_damo_deprecation_notice.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      620 2023-05-20 19:08:28.000000 damo-1.9.0/src/damo/_damo_dist.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9825 2023-07-15 19:33:44.000000 damo-1.9.0/src/damo/_damo_fmt_str.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2995 2023-05-20 19:08:28.000000 damo-1.9.0/src/damo/_damo_fs.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5345 2023-05-20 19:08:28.000000 damo-1.9.0/src/damo/_damo_paddr_layout.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      739 2023-05-20 19:08:28.000000 damo-1.9.0/src/damo/_damo_subcmds.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    35212 2023-07-15 19:33:44.000000 damo-1.9.0/src/damo/_damon.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    11838 2023-07-04 00:27:48.000000 damo-1.9.0/src/damo/_damon_args.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    16293 2023-06-24 19:25:59.000000 damo-1.9.0/src/damo/_damon_dbgfs.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    28979 2023-07-16 17:20:38.000000 damo-1.9.0/src/damo/_damon_result.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    19598 2023-07-02 18:42:47.000000 damo-1.9.0/src/damo/_damon_sysfs.py
--rwxrwxr-x   0 sjpark    (1000) sjpark    (1000)     3991 2023-07-04 00:27:48.000000 damo-1.9.0/src/damo/damo.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2023 2023-06-18 17:20:10.000000 damo-1.9.0/src/damo/damo_adjust.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      892 2023-06-18 18:06:08.000000 damo-1.9.0/src/damo/damo_convert_record_format.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1147 2023-05-20 19:08:28.000000 damo-1.9.0/src/damo/damo_features.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      746 2023-05-20 19:08:28.000000 damo-1.9.0/src/damo/damo_fmt_json.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    13384 2023-07-04 00:27:48.000000 damo-1.9.0/src/damo/damo_heats.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4668 2023-05-20 19:08:28.000000 damo-1.9.0/src/damo/damo_lru_sort.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3030 2023-07-04 00:27:48.000000 damo-1.9.0/src/damo/damo_monitor.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2743 2023-06-18 17:30:14.000000 damo-1.9.0/src/damo/damo_nr_regions.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4458 2023-05-20 19:08:28.000000 damo-1.9.0/src/damo/damo_reclaim.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5776 2023-07-08 17:18:37.000000 damo-1.9.0/src/damo/damo_record.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4094 2023-07-04 00:27:48.000000 damo-1.9.0/src/damo/damo_record_info.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1172 2023-07-04 00:27:48.000000 damo-1.9.0/src/damo/damo_report.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3723 2023-07-15 19:33:44.000000 damo-1.9.0/src/damo/damo_report_raw.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1511 2023-06-17 18:37:36.000000 damo-1.9.0/src/damo/damo_schemes.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    12741 2023-07-16 18:22:40.000000 damo-1.9.0/src/damo/damo_show.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      599 2023-07-08 17:03:00.000000 damo-1.9.0/src/damo/damo_start.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2602 2023-07-16 18:13:27.000000 damo-1.9.0/src/damo/damo_stat.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      878 2023-07-16 18:10:50.000000 damo-1.9.0/src/damo/damo_stat_kdamonds.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2995 2023-07-16 18:14:49.000000 damo-1.9.0/src/damo/damo_stat_regions.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      822 2023-07-16 18:11:19.000000 damo-1.9.0/src/damo/damo_stat_schemes.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3354 2023-07-16 18:27:07.000000 damo-1.9.0/src/damo/damo_status.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      701 2023-07-08 17:18:37.000000 damo-1.9.0/src/damo/damo_stop.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      865 2023-05-29 19:12:16.000000 damo-1.9.0/src/damo/damo_translate_damos.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      627 2023-05-20 19:08:28.000000 damo-1.9.0/src/damo/damo_tune.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3929 2023-07-04 00:27:48.000000 damo-1.9.0/src/damo/damo_validate.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       22 2023-07-17 23:18:25.000000 damo-1.9.0/src/damo/damo_version.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5537 2023-07-15 19:33:44.000000 damo-1.9.0/src/damo/damo_wss.py
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-07-17 23:20:07.296029 damo-1.9.0/src/damo.egg-info/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8366 2023-07-17 23:20:07.000000 damo-1.9.0/src/damo.egg-info/PKG-INFO
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1249 2023-07-17 23:20:07.000000 damo-1.9.0/src/damo.egg-info/SOURCES.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        1 2023-07-17 23:20:07.000000 damo-1.9.0/src/damo.egg-info/dependency_links.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       40 2023-07-17 23:20:07.000000 damo-1.9.0/src/damo.egg-info/entry_points.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        5 2023-07-17 23:20:07.000000 damo-1.9.0/src/damo.egg-info/top_level.txt
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-07-24 17:11:40.033988 damo-1.9.1/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8366 2023-07-24 17:11:40.033988 damo-1.9.1/PKG-INFO
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7845 2023-07-24 17:11:35.000000 damo-1.9.1/README.md
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      104 2022-04-22 09:53:30.000000 damo-1.9.1/pyproject.toml
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       38 2023-07-24 17:11:40.033988 damo-1.9.1/setup.cfg
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1104 2023-05-13 14:44:13.000000 damo-1.9.1/setup.py
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-07-24 17:11:40.017989 damo-1.9.1/src/
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-07-24 17:11:40.033988 damo-1.9.1/src/damo/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        0 2023-07-24 17:11:35.000000 damo-1.9.1/src/damo/__init__.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7357 2023-07-04 00:27:48.000000 damo-1.9.1/src/damo/_damo_deprecated.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      963 2023-05-21 19:11:52.000000 damo-1.9.1/src/damo/_damo_deprecation_notice.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      620 2023-05-20 19:08:28.000000 damo-1.9.1/src/damo/_damo_dist.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9825 2023-07-15 19:33:44.000000 damo-1.9.1/src/damo/_damo_fmt_str.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2995 2023-05-20 19:08:28.000000 damo-1.9.1/src/damo/_damo_fs.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5345 2023-05-20 19:08:28.000000 damo-1.9.1/src/damo/_damo_paddr_layout.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      739 2023-05-20 19:08:28.000000 damo-1.9.1/src/damo/_damo_subcmds.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    35836 2023-07-23 18:27:42.000000 damo-1.9.1/src/damo/_damon.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    11838 2023-07-04 00:27:48.000000 damo-1.9.1/src/damo/_damon_args.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    16293 2023-06-24 19:25:59.000000 damo-1.9.1/src/damo/_damon_dbgfs.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    28979 2023-07-22 17:33:00.000000 damo-1.9.1/src/damo/_damon_result.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    19958 2023-07-22 18:51:01.000000 damo-1.9.1/src/damo/_damon_sysfs.py
+-rwxrwxr-x   0 sjpark    (1000) sjpark    (1000)     3853 2023-07-23 17:09:22.000000 damo-1.9.1/src/damo/damo.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2023 2023-06-18 17:20:10.000000 damo-1.9.1/src/damo/damo_adjust.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      892 2023-06-18 18:06:08.000000 damo-1.9.1/src/damo/damo_convert_record_format.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1147 2023-05-20 19:08:28.000000 damo-1.9.1/src/damo/damo_features.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      746 2023-05-20 19:08:28.000000 damo-1.9.1/src/damo/damo_fmt_json.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    13384 2023-07-04 00:27:48.000000 damo-1.9.1/src/damo/damo_heats.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4668 2023-05-20 19:08:28.000000 damo-1.9.1/src/damo/damo_lru_sort.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3030 2023-07-04 00:27:48.000000 damo-1.9.1/src/damo/damo_monitor.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2743 2023-06-18 17:30:14.000000 damo-1.9.1/src/damo/damo_nr_regions.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4458 2023-05-20 19:08:28.000000 damo-1.9.1/src/damo/damo_reclaim.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5776 2023-07-08 17:18:37.000000 damo-1.9.1/src/damo/damo_record.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4094 2023-07-04 00:27:48.000000 damo-1.9.1/src/damo/damo_record_info.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1172 2023-07-04 00:27:48.000000 damo-1.9.1/src/damo/damo_report.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3723 2023-07-15 19:33:44.000000 damo-1.9.1/src/damo/damo_report_raw.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1511 2023-06-17 18:37:36.000000 damo-1.9.1/src/damo/damo_schemes.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    17392 2023-07-23 18:59:48.000000 damo-1.9.1/src/damo/damo_show.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      599 2023-07-08 17:03:00.000000 damo-1.9.1/src/damo/damo_start.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3609 2023-07-23 17:24:02.000000 damo-1.9.1/src/damo/damo_status.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      701 2023-07-08 17:18:37.000000 damo-1.9.1/src/damo/damo_stop.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      865 2023-05-29 19:12:16.000000 damo-1.9.1/src/damo/damo_translate_damos.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      627 2023-05-20 19:08:28.000000 damo-1.9.1/src/damo/damo_tune.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3929 2023-07-04 00:27:48.000000 damo-1.9.1/src/damo/damo_validate.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       22 2023-07-24 17:10:30.000000 damo-1.9.1/src/damo/damo_version.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5537 2023-07-15 19:33:44.000000 damo-1.9.1/src/damo/damo_wss.py
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-07-24 17:11:40.033988 damo-1.9.1/src/damo.egg-info/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8366 2023-07-24 17:11:40.000000 damo-1.9.1/src/damo.egg-info/PKG-INFO
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1136 2023-07-24 17:11:40.000000 damo-1.9.1/src/damo.egg-info/SOURCES.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        1 2023-07-24 17:11:40.000000 damo-1.9.1/src/damo.egg-info/dependency_links.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       40 2023-07-24 17:11:40.000000 damo-1.9.1/src/damo.egg-info/entry_points.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        5 2023-07-24 17:11:40.000000 damo-1.9.1/src/damo.egg-info/top_level.txt
```

### Comparing `damo-1.9.0/PKG-INFO` & `damo-1.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 1.9.0
+Version: 1.9.1
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -45,16 +45,16 @@
     $ # install from PyPI, or use your distribution's package manager
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.9.0/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.9.0/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.9.1/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.9.1/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -62,15 +62,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.0/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.1/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -90,19 +90,19 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.0/USAGE.md) file?
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.1/USAGE.md) file?
 ---------------------------------------------------------------------
 
 Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.0/USAGE.md) are in experimental
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.1/USAGE.md) are in experimental
 stage.  Such experimental features could be deprecated and removed without any
 notice and grace priods.  The documented features could also be deprecated, but
 those will provide some notification and grace periods.
 
 
 Recording Data Access Patterns
 ==============================
```

### Comparing `damo-1.9.0/README.md` & `damo-1.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,16 @@
     $ # install from PyPI, or use your distribution's package manager
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.9.0/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.9.0/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.9.1/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.9.1/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -47,15 +47,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.0/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.1/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -75,19 +75,19 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.0/USAGE.md) file?
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.1/USAGE.md) file?
 ---------------------------------------------------------------------
 
 Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.0/USAGE.md) are in experimental
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.1/USAGE.md) are in experimental
 stage.  Such experimental features could be deprecated and removed without any
 notice and grace priods.  The documented features could also be deprecated, but
 those will provide some notification and grace periods.
 
 
 Recording Data Access Patterns
 ==============================
```

### Comparing `damo-1.9.0/setup.py` & `damo-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.0/src/damo/_damo_deprecated.py` & `damo-1.9.1/src/damo/_damo_deprecated.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.0/src/damo/_damo_deprecation_notice.py` & `damo-1.9.1/src/damo/_damo_deprecation_notice.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.0/src/damo/_damo_dist.py` & `damo-1.9.1/src/damo/_damo_dist.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.0/src/damo/_damo_fmt_str.py` & `damo-1.9.1/src/damo/_damo_fmt_str.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.0/src/damo/_damo_fs.py` & `damo-1.9.1/src/damo/_damo_fs.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.0/src/damo/_damo_paddr_layout.py` & `damo-1.9.1/src/damo/_damo_paddr_layout.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.0/src/damo/_damo_subcmds.py` & `damo-1.9.1/src/damo/_damo_subcmds.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.0/src/damo/_damon.py` & `damo-1.9.1/src/damo/_damon.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,16 +118,18 @@
             return '%s %s' % (_damo_fmt_str.format_nr(self.samples, raw),
                     unit_samples)
         raise Exception('unsupported unit for NrAccesses (%s)' % unit)
 
     @classmethod
     def from_kvpairs(cls, kv):
         ret = DamonNrAccesses(None, None)
-        ret.samples = kv['samples']
-        ret.percent = kv['percent']
+        if 'samples' in kv and kv['samples'] != None:
+            ret.samples = _damo_fmt_str.text_to_nr(kv['samples'])
+        if 'percent' in kv and kv['percent'] != None:
+            ret.percent = _damo_fmt_str.text_to_percent(kv['percent'])
         return ret
 
     def to_kvpairs(self, raw=False):
         return collections.OrderedDict(
                 [('samples', self.samples), ('percent', self.percent)])
 
 class DamonAge:
@@ -523,46 +525,55 @@
                 ('mid_permil',
                     _damo_fmt_str.format_permil(self.mid_permil, raw)),
                 ('low_permil',
                     _damo_fmt_str.format_permil(self.low_permil, raw)),
                 ])
 
 class DamosFilter:
-    filter_type = None  # anon or memcg
+    filter_type = None  # anon, memcg, or addr
     memcg_path = None
+    address_range = None    # DamonRegion
     matching = None
 
-    def __init__(self, filter_type, memcg_path, matching):
+    def __init__(self, filter_type, memcg_path, address_range, matching):
         self.filter_type = filter_type
         self.memcg_path = memcg_path
+        self.address_range = address_range
         self.matching = _damo_fmt_str.text_to_bool(matching)
 
     def to_str(self, raw):
-        memcg_path_str = ''
+        plus_str = ''
         if self.filter_type == 'memcg':
-            memcg_path_str = 'memcg_path %s, ' % self.memcg_path
+            plus_str = 'memcg_path %s, ' % self.memcg_path
+        if self.filter_type == 'addr':
+            plus_str = '%s, ' % self.address_range.to_str(raw)
         return 'filter_type %s, %smatching %s' % (
-                self.filter_type, memcg_path_str, self.matching)
+                self.filter_type, plus_str, self.matching)
 
     def __str__(self):
         return self.to_str(False)
 
     def __eq__(self, other):
         return type(self) == type(other) and '%s' % self == '%s' % other
 
     @classmethod
     def from_kvpairs(cls, kv):
         return DamosFilter(kv['filter_type'],
                 kv['memcg_path'] if kv['filter_type'] == 'memcg' else '',
+                DamonRegion.from_kvpairs(kv['address_range'])
+                    if kv['filter_type'] == 'addr' else None,
                 kv['matching'])
 
     def to_kvpairs(self, raw=False):
-        return collections.OrderedDict(
-                [(attr, getattr(self, attr)) for attr in [
-                    'filter_type', 'memcg_path', 'matching']])
+        return collections.OrderedDict([
+            ('filter_type', self.filter_type),
+            ('memcg_path', self.memcg_path),
+            ('address_range', self.address_range.to_kvpairs(raw) if
+                self.address_range != None else None),
+            ('matching', self.matching)])
 
 class DamosStats:
     nr_tried = None
     sz_tried = None
     nr_applied = None
     sz_applied = None
     qt_exceeds = None
```

### Comparing `damo-1.9.0/src/damo/_damon_args.py` & `damo-1.9.1/src/damo/_damon_args.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.0/src/damo/_damon_dbgfs.py` & `damo-1.9.1/src/damo/_damon_dbgfs.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.0/src/damo/_damon_result.py` & `damo-1.9.1/src/damo/_damon_result.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.0/src/damo/_damon_sysfs.py` & `damo-1.9.1/src/damo/_damon_sysfs.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,20 +93,24 @@
         if err != None:
             return err
     return None
 
 # for stage_kdamonds
 
 def wops_for_scheme_filter(damos_filter):
-    return {
+    wops = {
         'type': '%s' % damos_filter.filter_type,
         'memcg_path': ('%s' % damos_filter.memcg_path
             if damos_filter.memcg_path != None else ''),
         'matching': 'Y' if damos_filter.matching else 'N',
         }
+    if damos_filter.address_range != None:
+        wops['addr_start'] = damos_filter.address_range.start
+        wops['addr_end'] = damos_filter.address_range.end
+    return wops
 
 def wops_for_scheme_filters(filters):
     wops = {}
     for idx, damos_filter in enumerate(filters):
         wops['%d' % idx] = wops_for_scheme_filter(damos_filter)
     return wops
 
@@ -352,15 +356,19 @@
             int(files_content['interval_us']),
             int(files_content['high']),
             int(files_content['mid']),
             int(files_content['low']))
 
 def files_content_to_damos_filters(files_content):
     return [_damon.DamosFilter(filter_kv['type'].strip(),
-            filter_kv['memcg_path'].strip(), filter_kv['matching'].strip())
+            filter_kv['memcg_path'].strip(),
+            _damon.DamonRegion(filter_kv['addr_start'].strip(),
+                filter_kv['addr_end'].strip())
+                if filter_kv['type'] == 'addr' else None,
+            filter_kv['matching'].strip())
             for filter_kv in numbered_dirs_content(
                 files_content, 'nr_filters')]
 
 def files_content_to_damos_stats(files_content):
     return _damon.DamosStats(
             int(files_content['nr_tried']),
             int(files_content['sz_tried']),
```

### Comparing `damo-1.9.0/src/damo/damo.py` & `damo-1.9.1/src/damo/damo.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 import damo_monitor
 import damo_reclaim
 import damo_record
 import damo_report
 import damo_schemes
 import damo_show
 import damo_start
-import damo_stat
 import damo_status
 import damo_stop
 import damo_translate_damos
 import damo_tune
 import damo_validate
 import damo_version
 
@@ -46,16 +45,14 @@
             msg='control DAMON_RECLAIM'),
         _damo_subcmds.DamoSubCmd(name='lru_sort', module=damo_lru_sort,
             msg='control DAMON_LRU_SORT'),
         _damo_subcmds.DamoSubCmd(name='features', module=damo_features,
             msg='list supported DAMON features in the kernel'),
         _damo_subcmds.DamoSubCmd(name='validate', module=damo_validate,
             msg='validate a given record result file'),
-        _damo_subcmds.DamoSubCmd(name='stat', module=damo_stat,
-            msg='print status of DAMON and the system'),
         _damo_subcmds.DamoSubCmd(name='start', module=damo_start,
             msg='start DAMON with given parameters'),
         _damo_subcmds.DamoSubCmd(name='stop', module=damo_stop,
             msg='stop running DAMON'),
         _damo_subcmds.DamoSubCmd(name='tune', module=damo_tune,
             msg='update input parameters of ongoing DAMON'),
         _damo_subcmds.DamoSubCmd(name='fmt_json', module=damo_fmt_json,
```

### Comparing `damo-1.9.0/src/damo/damo_adjust.py` & `damo-1.9.1/src/damo/damo_adjust.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.0/src/damo/damo_convert_record_format.py` & `damo-1.9.1/src/damo/damo_convert_record_format.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.0/src/damo/damo_features.py` & `damo-1.9.1/src/damo/damo_features.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.0/src/damo/damo_fmt_json.py` & `damo-1.9.1/src/damo/damo_fmt_json.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.0/src/damo/damo_heats.py` & `damo-1.9.1/src/damo/damo_heats.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.0/src/damo/damo_lru_sort.py` & `damo-1.9.1/src/damo/damo_lru_sort.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.0/src/damo/damo_monitor.py` & `damo-1.9.1/src/damo/damo_monitor.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.0/src/damo/damo_nr_regions.py` & `damo-1.9.1/src/damo/damo_nr_regions.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.0/src/damo/damo_reclaim.py` & `damo-1.9.1/src/damo/damo_reclaim.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.0/src/damo/damo_record.py` & `damo-1.9.1/src/damo/damo_record.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.0/src/damo/damo_record_info.py` & `damo-1.9.1/src/damo/damo_record_info.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.0/src/damo/damo_report.py` & `damo-1.9.1/src/damo/damo_report.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.0/src/damo/damo_report_raw.py` & `damo-1.9.1/src/damo/damo_report_raw.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.0/src/damo/damo_schemes.py` & `damo-1.9.1/src/damo/damo_schemes.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.0/src/damo/damo_show.py` & `damo-1.9.1/src/damo/damo_show.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # SPDX-License-Identifier: GPL-2.0
 
 import argparse
+import copy
 import json
 import os
+import random
+import time
 
 import _damo_fmt_str
 import _damon
 import _damon_args
 import _damon_result
 
 record_formatters = {
@@ -38,29 +41,33 @@
         '<monitor end time>': lambda snapshot, record, raw:
             _damo_fmt_str.format_time_ns(
                 snapshot.end_time - record.snapshots[0].start_time, raw),
         '<monitor start abs time>': lambda snapshot, record, raw:
             _damo_fmt_str.format_time_ns(snapshot.start_time, raw),
         '<monitor end abs time>': lambda snapshot, record, raw:
             _damo_fmt_str.format_time_ns(snapshot.end_time, raw),
+        '<number of regions>': lambda snapshot, record, raw:
+            _damo_fmt_str.format_nr(len(snapshot.regions), raw),
             }
 
 region_formatters = {
-        '<index>': lambda index, region, raw:
+        '<index>': lambda index, region, raw, mms:
             _damo_fmt_str.format_nr(index, raw),
-        '<start address>': lambda index, region, raw:
+        '<start address>': lambda index, region, raw, mms:
             _damo_fmt_str.format_sz(region.start, raw),
-        '<end address>': lambda index, region, raw:
+        '<end address>': lambda index, region, raw, mms:
             _damo_fmt_str.format_sz(region.end, raw),
-        '<region size>': lambda index, region, raw:
+        '<region size>': lambda index, region, raw, mms:
             _damo_fmt_str.format_sz(region.size(), raw),
-        '<access rate>': lambda index, region, raw:
+        '<access rate>': lambda index, region, raw, mms:
             _damo_fmt_str.format_percent(region.nr_accesses.percent, raw),
-        '<age>': lambda index, region, raw:
-            _damo_fmt_str.format_time_us(region.age.usec, raw)
+        '<age>': lambda index, region, raw, mms:
+            _damo_fmt_str.format_time_us(region.age.usec, raw),
+        '<size_bar>': lambda index, region, raw, mms:
+           size_bar(region, mms, 0, 20),
         }
 
 formatters = {
         'record': record_formatters,
         'snapshot': snapshot_formatters,
         'region': region_formatters
         }
@@ -73,14 +80,75 @@
     rows), and number, respectively.
     '''
     nr_columns = int(region.age.usec / usec_per_column)
     nr_rows = int(region.size() / bytes_per_row)
     heat_nr = int(region.nr_accesses.percent / nr_per_access_rate_percent)
     return '\n'.join([('%d' % heat_nr) * nr_columns] * nr_rows)
 
+class MinMaxOfRecords:
+    min_sz_region = None
+    max_sz_region = None
+    min_access_rate_percent = None
+    max_access_rate_percent = None
+    min_age_us = None
+    max_age_us = None
+
+    def set_fields(self, region, intervals):
+        region.nr_accesses.add_unset_unit(intervals)
+        region.age.add_unset_unit(intervals)
+
+        if self.min_sz_region == None or region.size() < self.min_sz_region:
+            self.min_sz_region = region.size()
+        if self.max_sz_region == None or region.size() > self.max_sz_region:
+            self.max_sz_region = region.size()
+        if (self.min_access_rate_percent == None or
+                region.nr_accesses.percent < self.min_access_rate_percent):
+            self.min_access_rate_percent = region.nr_accesses.percent
+        if (self.max_access_rate_percent == None or
+                region.nr_accesses.percent > self.max_access_rate_percent):
+            self.max_access_rate_percent = region.nr_accesses.percent
+        if self.min_age_us == None or region.age.usec < self.min_age_us:
+            self.min_age_us = region.age.usec
+        if self.max_age_us == None or region.age.usec > self.max_age_us:
+            self.max_age_us = region.age.usec
+
+    def __init__(self, records):
+        for record in records:
+            for snapshot in record.snapshots:
+                for region in snapshot.regions:
+                    self.set_fields(region, record.intervals)
+
+def rescale_val(val, orig_scale_minmax, new_scale_minmax):
+    '''Return a value in new scale
+
+    Parameters
+    ----------
+    val : int, float
+        The value to rescale
+    orig_scale_minmax : list
+        min/max values of original scale
+    new_scale_minmax : list
+        min/max values of new scale
+
+    Returns
+    -------
+    float
+        The rescaled value
+    '''
+    orig_length = orig_scale_minmax[1] - orig_scale_minmax[0]
+    new_length = new_scale_minmax[1] - new_scale_minmax[0]
+    ratio = new_length / orig_length
+    return (val - orig_scale_minmax[0]) * ratio + new_scale_minmax[0]
+
+def size_bar(region, minmaxs, min_cols, max_cols):
+    nr_cols = int(rescale_val(region.size(),
+            [minmaxs.min_sz_region, minmaxs.max_sz_region],
+            [min_cols, max_cols]))
+    return '<%s>' % ('-' * nr_cols)
+
 def apply_min_chars(min_chars, field_name, txt):
     # min_chars: [[<field name>, <number of min chars>]...]
     for name, nr in min_chars:
         try:
             nr = int(nr)
         except:
             print('wrong min_chars: %s' % min_chars)
@@ -88,27 +156,27 @@
         if name == field_name:
             if len(txt) >= nr:
                 return txt
             txt += ' ' * (nr - len(txt))
             return txt
     return txt
 
-def format_pr(template, min_chars, index, region, snapshot, record, raw):
+def format_pr(template, min_chars, index, region, snapshot, record, raw, mms):
     if template == '':
         return
     for category, category_formatters in formatters.items():
         for field_name, formatter in category_formatters.items():
             if template.find(field_name) == -1:
                 continue
             if category == 'record':
                 txt = formatter(record, raw)
             elif category == 'snapshot':
                 txt = formatter(snapshot, record, raw)
             elif category == 'region':
-                txt = formatter(index, region, raw)
+                txt = formatter(index, region, raw, mms)
             txt = apply_min_chars(min_chars, field_name, txt)
             template = template.replace(field_name, txt)
     template = template.replace('\\n', '\n')
     print(template)
 
 def set_formats(args, records):
     if args.format_record_head == None:
@@ -147,37 +215,38 @@
 def pr_records(args, records):
     if args.json:
         print(json.dumps([r.to_kvpairs(args.raw_number)
             for r in records], indent=4))
         exit(0)
 
     set_formats(args, records)
+    mms = MinMaxOfRecords(records)
 
     for record in records:
         format_pr(args.format_record_head, args.min_chars_field, None, None,
-                None, record, args.raw_number)
+                None, record, args.raw_number, mms)
         snapshots = record.snapshots
 
         for sidx, snapshot in enumerate(snapshots):
             format_pr(args.format_snapshot_head, args.min_chars_field, None,
-                    None, snapshot, record, args.raw_number)
+                    None, snapshot, record, args.raw_number, mms)
             for r in snapshot.regions:
                 r.nr_accesses.add_unset_unit(record.intervals)
                 r.age.add_unset_unit(record.intervals)
             for idx, r in enumerate(
                     sorted_regions(snapshot.regions, args.sort_regions_by)):
                 format_pr(args.format_region, args.min_chars_field, idx, r,
-                        snapshot, record, args.raw_number)
+                        snapshot, record, args.raw_number, mms)
             format_pr(args.format_snapshot_tail, args.min_chars_field, None,
-                    None, snapshot, record, args.raw_number)
+                    None, snapshot, record, args.raw_number, mms)
 
             if sidx < len(snapshots) - 1 and not args.total_sz_only:
                 print('')
         format_pr(args.format_record_tail, args.min_chars_field, None, None,
-                None, record, args.raw_number)
+                None, record, args.raw_number, mms)
 
 def filter_by_pattern(record, access_pattern):
     sz_bytes = access_pattern.sz_bytes
     nr_acc = access_pattern.nr_acc_min_max
     age = access_pattern.age_min_max
 
     for snapshot in record.snapshots:
@@ -197,27 +266,73 @@
             region.age.add_unset_unit(intervals)
             usecs = region.age.usec
             if usecs < age[0].usec or age[1].usec < usecs:
                 continue
             filtered.append(region)
         snapshot.regions = filtered
 
+def filter_by_addr(region, addr_ranges):
+    regions = []
+    for start, end in addr_ranges:
+        # out of the range
+        if region.end <= start or end <= region.start:
+            continue
+        # in the range
+        if start <= region.start and region.end <= end:
+            regions.append(copy.deepcopy(region))
+            continue
+        # overlap
+        copied = copy.deepcopy(region)
+        copied.start = max(start, region.start)
+        copied.end = min(end, region.end)
+        regions.append(copied)
+    return regions
+
+def filter_records_by_addr(records, addr_ranges):
+    for record in records:
+        for snapshot in record.snapshots:
+            filtered_regions = []
+            for region in snapshot.regions:
+                filtered_regions += filter_by_addr(region, addr_ranges)
+            snapshot.regions = filtered_regions
+            snapshot.update_total_bytes()
+
+def convert_addr_ranges_input(addr_ranges_input):
+    try:
+        ranges = [[_damo_fmt_str.text_to_bytes(start),
+            _damo_fmt_str.text_to_bytes(end)]
+            for start, end in addr_ranges_input]
+    except Exception as e:
+        return None, 'conversion to bytes failed (%s)' % e
+
+    ranges.sort(key=lambda x: x[0])
+    for idx, arange in enumerate(ranges):
+        start, end = arange
+        if start > end:
+            return None, 'start > end (%s)' % arange
+        if idx > 0 and ranges[idx - 1][1] > start:
+            return None, 'overlapping range'
+    return ranges, None
+
 def set_argparser(parser):
     _damon_args.set_common_argparser(parser)
 
     # what to show
     parser.add_argument('--sz_region', metavar=('<min>', '<max>'), nargs=2,
             default=['min', 'max'],
             help='min/max size of regions (bytes)')
     parser.add_argument('--access_rate', metavar=('<min>', '<max>'), nargs=2,
             default=['min', 'max'],
             help='min/max access rate of regions (percent)')
     parser.add_argument('--age', metavar=('<min>', '<max>'), nargs=2,
             default=['min', 'max'],
             help='min/max age of regions (seconds)')
+    parser.add_argument('--address', metavar=('<start>', '<end>'), nargs=2,
+            action='append',
+            help='address ranges to show for')
 
     parser.add_argument('--input_file', metavar='<file>',
             help='source of the access pattern to show')
     parser.add_argument('--tried_regions_of', nargs=3, type=int,
             action='append',
             metavar=('<kdamond idx>', '<context idx>', '<scheme idx>'),
             help='show tried regions of given schemes')
@@ -267,43 +382,51 @@
         set_argparser(parser)
         args = parser.parse_args()
 
     access_pattern = _damon.DamosAccessPattern(args.sz_region,
             args.access_rate, _damon.unit_percent, args.age * 1000000,
             _damon.unit_usec)
 
-    if args.input_file == None and args.tried_regions_of == None:
+    if args.input_file == None:
         _damon.ensure_root_and_initialized(args)
-
-        records, err = _damon_result.get_snapshot_records(access_pattern,
-                args.total_sz_only, not args.dont_merge_regions)
+        err = 'assumed error'
+        nr_tries = 0
+        while err != None and nr_tries < 5:
+            nr_tries += 1
+            if args.tried_regions_of == None:
+                records, err = _damon_result.get_snapshot_records(access_pattern,
+                        args.total_sz_only, not args.dont_merge_regions)
+            else:
+                 records, err = _damon_result.get_snapshot_records_for_schemes(
+                        args.tried_regions_of, args.total_sz_only,
+                        not args.dont_merge_regions)
+            if err != None:
+                time.sleep(random.randrange(
+                    2**(nr_tries - 1), 2**nr_tries) / 100)
         if err != None:
             print(err)
             exit(1)
-    elif args.input_file != None:
+    else:
         if not os.path.isfile(args.input_file):
             print('--input_file (%s) is not file' % args.input_file)
             exit(1)
 
         records, err = _damon_result.parse_records_file(args.input_file)
         if err:
             print('parsing damon result file (%s) failed (%s)' %
                     (args.input_file, err))
             exit(1)
         for record in records:
             filter_by_pattern(record, access_pattern)
-    elif args.tried_regions_of != None:
-        _damon.ensure_root_and_initialized(args)
-
-        records, err = _damon_result.get_snapshot_records_for_schemes(
-                args.tried_regions_of, args.total_sz_only,
-                not args.dont_merge_regions)
-        if err != None:
-            print(err)
+    if args.address:
+        ranges, err = convert_addr_ranges_input(args.address)
+        if err:
+            print('wrong --address input (%s)' % err)
             exit(1)
+        filter_records_by_addr(records, ranges)
 
     for record in records:
         try:
             pr_records(args, records)
         except BrokenPipeError as e:
             # maybe user piped to 'less' like pager, and quit from it
             pass
```

### Comparing `damo-1.9.0/src/damo/damo_start.py` & `damo-1.9.1/src/damo/damo_start.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.0/src/damo/damo_stat_schemes.py` & `damo-1.9.1/src/damo/damo_tune.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,30 @@
 # SPDX-License-Identifier: GPL-2.0
 
-import argparse
+"""
+Update DAMON input parameters.
+"""
 
-import _damo_fmt_str
-import _damo_subcmds
 import _damon
-import damo_stat
-import damo_status
+import _damon_args
 
 def set_argparser(parser):
-    damo_stat.set_common_argparser(parser)
-
-def __main(args):
-    if args.stat_type == 'schemes_stats':
-        damo_status.update_pr_schemes_stats(args.raw)
-    elif args.stat_type == 'schemes_tried_regions':
-        damo_status.update_pr_schemes_tried_regions(args.raw)
+    return _damon_args.set_argparser(parser, add_record_options=False)
 
 def main(args=None):
     if not args:
-        parser = argparse.ArgumentParser()
-        set_argparser(parser)
+        parser = set_argparser(None)
         args = parser.parse_args()
 
     _damon.ensure_root_and_initialized(args)
 
-    damo_stat.run_count_delay(__main, args)
-
-    for i in range(args.count):
-        if i != args.count - 1:
-            time.sleep(args.delay)
+    if not _damon.any_kdamond_running():
+        print('DAMON is not turned on')
+        exit(1)
+
+    kdamonds, err = _damon_args.commit_kdamonds(args)
+    if err:
+        print('tuning failed (%s)' % err)
+        exit(1)
 
 if __name__ == '__main__':
     main()
```

### Comparing `damo-1.9.0/src/damo/damo_status.py` & `damo-1.9.1/src/damo/damo_status.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # SPDX-License-Identifier: GPL-2.0
 
 """
 Show status of DAMON.
 """
 
 import json
+import random
+import time
 
 import _damo_fmt_str
 import _damon
 import _damon_args
 
 def pr_schemes_tried_regions(kdamonds, raw_nr):
     print('# <kdamond> <context> <scheme>')
@@ -60,15 +62,22 @@
     summary = [k.summary_str() for k in kdamonds]
     if json_format:
         print(json.dumps(summary, indent=4))
         return
     print('\n'.join(summary))
 
 def update_pr_kdamonds(json_format, raw_nr):
-    kdamonds, err = _damon.update_read_kdamonds()
+    err = 'assumed error'
+    nr_tries = 0
+    while err != None and nr_tries < 5:
+        nr_tries += 1
+        kdamonds, err = _damon.update_read_kdamonds()
+        if err != None:
+            time.sleep(random.randrange(
+                2**(nr_tries - 1), 2**nr_tries) / 100)
     if err:
         print(err)
         return
     if json_format:
         print(json.dumps([k.to_kvpairs(raw_nr) for k in kdamonds], indent=4))
     else:
         for idx, k in enumerate(kdamonds):
```

### Comparing `damo-1.9.0/src/damo/damo_stop.py` & `damo-1.9.1/src/damo/damo_stop.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.0/src/damo/damo_translate_damos.py` & `damo-1.9.1/src/damo/damo_translate_damos.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.0/src/damo/damo_validate.py` & `damo-1.9.1/src/damo/damo_validate.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.0/src/damo/damo_wss.py` & `damo-1.9.1/src/damo/damo_wss.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.0/src/damo.egg-info/PKG-INFO` & `damo-1.9.1/src/damo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 1.9.0
+Version: 1.9.1
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -45,16 +45,16 @@
     $ # install from PyPI, or use your distribution's package manager
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.9.0/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.9.0/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.9.1/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.9.1/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -62,15 +62,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.0/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.1/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -90,19 +90,19 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.0/USAGE.md) file?
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.1/USAGE.md) file?
 ---------------------------------------------------------------------
 
 Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.0/USAGE.md) are in experimental
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.1/USAGE.md) are in experimental
 stage.  Such experimental features could be deprecated and removed without any
 notice and grace priods.  The documented features could also be deprecated, but
 those will provide some notification and grace periods.
 
 
 Recording Data Access Patterns
 ==============================
```

### Comparing `damo-1.9.0/src/damo.egg-info/SOURCES.txt` & `damo-1.9.1/src/damo.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 src/damo/damo_record.py
 src/damo/damo_record_info.py
 src/damo/damo_report.py
 src/damo/damo_report_raw.py
 src/damo/damo_schemes.py
 src/damo/damo_show.py
 src/damo/damo_start.py
-src/damo/damo_stat.py
-src/damo/damo_stat_kdamonds.py
-src/damo/damo_stat_regions.py
-src/damo/damo_stat_schemes.py
 src/damo/damo_status.py
 src/damo/damo_stop.py
 src/damo/damo_translate_damos.py
 src/damo/damo_tune.py
 src/damo/damo_validate.py
 src/damo/damo_version.py
 src/damo/damo_wss.py
```

