# Comparing `tmp/obis-0.4.2rc6.tar.gz` & `tmp/obis-0.4.2rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obis-0.4.2rc6.tar", last modified: Wed Jul 19 08:50:23 2023, max compression
+gzip compressed data, was "obis-0.4.2rc7.tar", last modified: Mon Jul 24 14:31:39 2023, max compression
```

## Comparing `obis-0.4.2rc6.tar` & `obis-0.4.2rc7.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-19 08:50:23.032583 obis-0.4.2rc6/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      774 2023-07-19 08:48:52.000000 obis-0.4.2rc6/CHANGELOG.md
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    11357 2023-02-20 13:30:53.000000 obis-0.4.2rc6/LICENSE
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      176 2023-02-20 13:30:53.000000 obis-0.4.2rc6/MANIFEST.in
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    32149 2023-07-19 08:50:23.032583 obis-0.4.2rc6/PKG-INFO
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    31587 2023-07-17 10:34:32.000000 obis-0.4.2rc6/README.md
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-19 08:50:22.988583 obis-0.4.2rc6/man/
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-19 08:50:23.000583 obis-0.4.2rc6/man/man1/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      593 2023-02-20 13:30:53.000000 obis-0.4.2rc6/man/man1/obis-addref.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      879 2023-02-20 13:30:53.000000 obis-0.4.2rc6/man/man1/obis-clone.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      798 2023-02-20 13:30:53.000000 obis-0.4.2rc6/man/man1/obis-collection.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      825 2023-02-20 13:30:53.000000 obis-0.4.2rc6/man/man1/obis-commit.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      746 2023-02-20 13:30:53.000000 obis-0.4.2rc6/man/man1/obis-config.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1027 2023-02-20 13:30:53.000000 obis-0.4.2rc6/man/man1/obis-data_set.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      893 2023-02-20 13:30:53.000000 obis-0.4.2rc6/man/man1/obis-download.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      757 2023-02-20 13:30:53.000000 obis-0.4.2rc6/man/man1/obis-init.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      871 2023-02-20 13:30:53.000000 obis-0.4.2rc6/man/man1/obis-init_analysis.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      871 2023-02-20 13:30:53.000000 obis-0.4.2rc6/man/man1/obis-move.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      762 2023-02-20 13:30:53.000000 obis-0.4.2rc6/man/man1/obis-object.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      617 2023-02-20 13:30:53.000000 obis-0.4.2rc6/man/man1/obis-removeref.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1221 2023-02-20 13:30:53.000000 obis-0.4.2rc6/man/man1/obis-repository.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      742 2023-02-20 13:30:53.000000 obis-0.4.2rc6/man/man1/obis-settings.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      593 2023-02-20 13:30:53.000000 obis-0.4.2rc6/man/man1/obis-status.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      666 2023-02-20 13:30:53.000000 obis-0.4.2rc6/man/man1/obis-sync.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1684 2023-02-20 13:30:53.000000 obis-0.4.2rc6/man/man1/obis.1
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-19 08:50:23.000583 obis-0.4.2rc6/obis/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      757 2023-07-17 15:18:12.000000 obis-0.4.2rc6/obis/__init__.py
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-19 08:50:23.004583 obis-0.4.2rc6/obis/__pycache__/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      320 2023-07-18 13:34:59.000000 obis-0.4.2rc6/obis/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      563 2023-02-27 13:57:44.000000 obis-0.4.2rc6/obis/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      915 2023-02-21 12:05:41.000000 obis-0.4.2rc6/obis/conftest.py
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-19 08:50:23.012583 obis-0.4.2rc6/obis/dm/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      889 2023-02-21 12:05:41.000000 obis-0.4.2rc6/obis/dm/__init__.py
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-19 08:50:23.012583 obis-0.4.2rc6/obis/dm/__pycache__/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      411 2023-02-21 12:13:21.000000 obis-0.4.2rc6/obis/dm/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     7402 2023-03-07 09:56:22.000000 obis-0.4.2rc6/obis/dm/__pycache__/checksum.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2407 2023-02-21 12:13:22.000000 obis-0.4.2rc6/obis/dm/__pycache__/command_log.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1839 2023-02-21 12:13:21.000000 obis-0.4.2rc6/obis/dm/__pycache__/command_result.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    15644 2023-02-21 12:13:21.000000 obis-0.4.2rc6/obis/dm/__pycache__/config.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    23132 2023-03-30 13:34:10.000000 obis-0.4.2rc6/obis/dm/__pycache__/data_mgmt.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    17466 2023-07-17 14:48:25.000000 obis-0.4.2rc6/obis/dm/__pycache__/data_mgmt_test.cpython-310-pytest-7.2.1.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     7101 2023-03-30 10:33:16.000000 obis-0.4.2rc6/obis/dm/__pycache__/git.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1351 2023-02-21 12:17:13.000000 obis-0.4.2rc6/obis/dm/__pycache__/repository_utils.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3148 2023-03-30 10:51:56.000000 obis-0.4.2rc6/obis/dm/__pycache__/utils.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     7820 2023-03-07 08:26:10.000000 obis-0.4.2rc6/obis/dm/checksum.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2674 2023-02-21 12:05:41.000000 obis-0.4.2rc6/obis/dm/command_log.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1981 2023-02-21 12:05:41.000000 obis-0.4.2rc6/obis/dm/command_result.py
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-19 08:50:23.020583 obis-0.4.2rc6/obis/dm/commands/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      634 2023-02-21 12:05:41.000000 obis-0.4.2rc6/obis/dm/commands/__init__.py
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-19 08:50:23.024583 obis-0.4.2rc6/obis/dm/commands/__pycache__/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      194 2023-02-21 12:13:21.000000 obis-0.4.2rc6/obis/dm/commands/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1867 2023-03-29 14:28:25.000000 obis-0.4.2rc6/obis/dm/commands/__pycache__/addref.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3935 2023-02-28 09:09:45.000000 obis-0.4.2rc6/obis/dm/commands/__pycache__/clone.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3041 2023-02-28 09:44:21.000000 obis-0.4.2rc6/obis/dm/commands/__pycache__/collection.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3046 2023-02-21 16:35:01.000000 obis-0.4.2rc6/obis/dm/commands/__pycache__/download.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3343 2023-03-03 14:34:14.000000 obis-0.4.2rc6/obis/dm/commands/__pycache__/download_physical.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2416 2023-02-21 12:17:13.000000 obis-0.4.2rc6/obis/dm/commands/__pycache__/move.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3263 2023-03-01 08:22:27.000000 obis-0.4.2rc6/obis/dm/commands/__pycache__/object.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    10941 2023-03-30 10:21:33.000000 obis-0.4.2rc6/obis/dm/commands/__pycache__/openbis_command.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     6680 2023-02-21 12:17:13.000000 obis-0.4.2rc6/obis/dm/commands/__pycache__/openbis_sync.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3273 2023-02-21 12:17:13.000000 obis-0.4.2rc6/obis/dm/commands/__pycache__/removeref.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     8335 2023-07-17 10:14:41.000000 obis-0.4.2rc6/obis/dm/commands/__pycache__/search.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1589 2023-02-24 12:01:17.000000 obis-0.4.2rc6/obis/dm/commands/__pycache__/upload.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1897 2023-03-29 14:28:17.000000 obis-0.4.2rc6/obis/dm/commands/addref.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     5292 2023-02-28 08:49:14.000000 obis-0.4.2rc6/obis/dm/commands/clone.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3657 2023-02-28 09:16:53.000000 obis-0.4.2rc6/obis/dm/commands/collection.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3920 2023-02-21 13:31:53.000000 obis-0.4.2rc6/obis/dm/commands/download.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     4124 2023-03-03 14:31:58.000000 obis-0.4.2rc6/obis/dm/commands/download_physical.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2967 2023-02-21 12:05:41.000000 obis-0.4.2rc6/obis/dm/commands/move.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     4373 2023-03-01 08:22:23.000000 obis-0.4.2rc6/obis/dm/commands/object.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    12135 2023-03-30 10:21:12.000000 obis-0.4.2rc6/obis/dm/commands/openbis_command.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1535 2023-02-21 12:05:41.000000 obis-0.4.2rc6/obis/dm/commands/openbis_command_test.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     9774 2023-02-21 12:05:41.000000 obis-0.4.2rc6/obis/dm/commands/openbis_sync.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3565 2023-02-21 12:05:41.000000 obis-0.4.2rc6/obis/dm/commands/removeref.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    12372 2023-07-17 10:12:16.000000 obis-0.4.2rc6/obis/dm/commands/search.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1801 2023-02-24 12:00:59.000000 obis-0.4.2rc6/obis/dm/commands/upload.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    16039 2023-02-21 12:05:42.000000 obis-0.4.2rc6/obis/dm/config.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2934 2023-02-21 12:05:41.000000 obis-0.4.2rc6/obis/dm/config_test.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    27953 2023-03-30 13:30:39.000000 obis-0.4.2rc6/obis/dm/data_mgmt.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    14376 2023-03-29 13:51:23.000000 obis-0.4.2rc6/obis/dm/data_mgmt_test.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      245 2023-02-20 13:30:53.000000 obis-0.4.2rc6/obis/dm/git-annex-attributes
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     8502 2023-03-30 10:32:13.000000 obis-0.4.2rc6/obis/dm/git.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1905 2023-02-21 12:05:41.000000 obis-0.4.2rc6/obis/dm/repository_utils.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3789 2023-03-30 10:51:34.000000 obis-0.4.2rc6/obis/dm/utils.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      980 2023-02-21 12:05:41.000000 obis-0.4.2rc6/obis/dm/utils_test.py
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-19 08:50:23.028583 obis-0.4.2rc6/obis/scripts/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      919 2023-02-21 12:05:41.000000 obis-0.4.2rc6/obis/scripts/__init__.py
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-19 08:50:23.028583 obis-0.4.2rc6/obis/scripts/__pycache__/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      431 2023-02-21 12:13:22.000000 obis-0.4.2rc6/obis/scripts/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    30930 2023-07-17 10:14:41.000000 obis-0.4.2rc6/obis/scripts/__pycache__/cli.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      746 2023-02-21 12:13:22.000000 obis-0.4.2rc6/obis/scripts/__pycache__/click_util.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     4351 2023-03-30 10:59:33.000000 obis-0.4.2rc6/obis/scripts/__pycache__/data_mgmt_runner.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    39340 2023-07-17 10:13:46.000000 obis-0.4.2rc6/obis/scripts/cli.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1126 2023-02-21 12:05:41.000000 obis-0.4.2rc6/obis/scripts/click_util.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     5701 2023-03-30 10:59:06.000000 obis-0.4.2rc6/obis/scripts/data_mgmt_runner.py
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-19 08:50:23.032583 obis-0.4.2rc6/obis/test-data/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)   160470 2023-02-20 13:30:53.000000 obis-0.4.2rc6/obis/test-data/snb-data.zip
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       43 2023-02-20 13:30:53.000000 obis-0.4.2rc6/obis/test-data/text-data-2.txt
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       32 2023-02-20 13:30:53.000000 obis-0.4.2rc6/obis/test-data/text-data.txt
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-19 08:50:22.992583 obis-0.4.2rc6/obis/test-data/user_config/
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-19 08:50:23.032583 obis-0.4.2rc6/obis/test-data/user_config/.obis/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      167 2023-02-20 13:30:53.000000 obis-0.4.2rc6/obis/test-data/user_config/.obis/config.json
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-19 08:50:23.004583 obis-0.4.2rc6/obis.egg-info/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    32149 2023-07-19 08:50:22.000000 obis-0.4.2rc6/obis.egg-info/PKG-INFO
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3124 2023-07-19 08:50:22.000000 obis-0.4.2rc6/obis.egg-info/SOURCES.txt
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)        1 2023-07-19 08:50:22.000000 obis-0.4.2rc6/obis.egg-info/dependency_links.txt
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       47 2023-07-19 08:50:22.000000 obis-0.4.2rc6/obis.egg-info/entry_points.txt
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)        1 2023-02-23 08:39:07.000000 obis-0.4.2rc6/obis.egg-info/not-zip-safe
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       38 2023-07-19 08:50:22.000000 obis-0.4.2rc6/obis.egg-info/requires.txt
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)        5 2023-07-19 08:50:22.000000 obis-0.4.2rc6/obis.egg-info/top_level.txt
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       38 2023-07-19 08:50:23.032583 obis-0.4.2rc6/setup.cfg
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1986 2023-07-19 08:48:52.000000 obis-0.4.2rc6/setup.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-24 14:31:39.504896 obis-0.4.2rc7/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      773 2023-07-19 10:10:53.000000 obis-0.4.2rc7/CHANGELOG.md
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    11357 2023-02-20 13:30:53.000000 obis-0.4.2rc7/LICENSE
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      176 2023-02-20 13:30:53.000000 obis-0.4.2rc7/MANIFEST.in
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    32149 2023-07-24 14:31:39.504896 obis-0.4.2rc7/PKG-INFO
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    31587 2023-07-17 10:34:32.000000 obis-0.4.2rc7/README.md
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-24 14:31:39.488896 obis-0.4.2rc7/man/
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-24 14:31:39.492896 obis-0.4.2rc7/man/man1/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      593 2023-02-20 13:30:53.000000 obis-0.4.2rc7/man/man1/obis-addref.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      879 2023-02-20 13:30:53.000000 obis-0.4.2rc7/man/man1/obis-clone.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      798 2023-02-20 13:30:53.000000 obis-0.4.2rc7/man/man1/obis-collection.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      825 2023-02-20 13:30:53.000000 obis-0.4.2rc7/man/man1/obis-commit.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      746 2023-02-20 13:30:53.000000 obis-0.4.2rc7/man/man1/obis-config.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1027 2023-02-20 13:30:53.000000 obis-0.4.2rc7/man/man1/obis-data_set.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      893 2023-02-20 13:30:53.000000 obis-0.4.2rc7/man/man1/obis-download.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      757 2023-02-20 13:30:53.000000 obis-0.4.2rc7/man/man1/obis-init.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      871 2023-02-20 13:30:53.000000 obis-0.4.2rc7/man/man1/obis-init_analysis.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      871 2023-02-20 13:30:53.000000 obis-0.4.2rc7/man/man1/obis-move.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      762 2023-02-20 13:30:53.000000 obis-0.4.2rc7/man/man1/obis-object.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      617 2023-02-20 13:30:53.000000 obis-0.4.2rc7/man/man1/obis-removeref.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1221 2023-02-20 13:30:53.000000 obis-0.4.2rc7/man/man1/obis-repository.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      742 2023-02-20 13:30:53.000000 obis-0.4.2rc7/man/man1/obis-settings.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      593 2023-02-20 13:30:53.000000 obis-0.4.2rc7/man/man1/obis-status.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      666 2023-02-20 13:30:53.000000 obis-0.4.2rc7/man/man1/obis-sync.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1684 2023-02-20 13:30:53.000000 obis-0.4.2rc7/man/man1/obis.1
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-24 14:31:39.492896 obis-0.4.2rc7/obis/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      757 2023-07-24 14:31:36.000000 obis-0.4.2rc7/obis/__init__.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-24 14:31:39.492896 obis-0.4.2rc7/obis/__pycache__/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      320 2023-07-19 09:51:42.000000 obis-0.4.2rc7/obis/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      563 2023-02-27 13:57:44.000000 obis-0.4.2rc7/obis/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      915 2023-02-21 12:05:41.000000 obis-0.4.2rc7/obis/conftest.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-24 14:31:39.496896 obis-0.4.2rc7/obis/dm/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      889 2023-02-21 12:05:41.000000 obis-0.4.2rc7/obis/dm/__init__.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-24 14:31:39.496896 obis-0.4.2rc7/obis/dm/__pycache__/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      411 2023-02-21 12:13:21.000000 obis-0.4.2rc7/obis/dm/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     7402 2023-03-07 09:56:22.000000 obis-0.4.2rc7/obis/dm/__pycache__/checksum.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2407 2023-02-21 12:13:22.000000 obis-0.4.2rc7/obis/dm/__pycache__/command_log.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1839 2023-02-21 12:13:21.000000 obis-0.4.2rc7/obis/dm/__pycache__/command_result.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    15644 2023-02-21 12:13:21.000000 obis-0.4.2rc7/obis/dm/__pycache__/config.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    23132 2023-03-30 13:34:10.000000 obis-0.4.2rc7/obis/dm/__pycache__/data_mgmt.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    17466 2023-07-17 14:48:25.000000 obis-0.4.2rc7/obis/dm/__pycache__/data_mgmt_test.cpython-310-pytest-7.2.1.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     7101 2023-03-30 10:33:16.000000 obis-0.4.2rc7/obis/dm/__pycache__/git.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1351 2023-02-21 12:17:13.000000 obis-0.4.2rc7/obis/dm/__pycache__/repository_utils.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3148 2023-03-30 10:51:56.000000 obis-0.4.2rc7/obis/dm/__pycache__/utils.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     7820 2023-03-07 08:26:10.000000 obis-0.4.2rc7/obis/dm/checksum.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2674 2023-02-21 12:05:41.000000 obis-0.4.2rc7/obis/dm/command_log.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1981 2023-02-21 12:05:41.000000 obis-0.4.2rc7/obis/dm/command_result.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-24 14:31:39.500896 obis-0.4.2rc7/obis/dm/commands/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      634 2023-02-21 12:05:41.000000 obis-0.4.2rc7/obis/dm/commands/__init__.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-24 14:31:39.500896 obis-0.4.2rc7/obis/dm/commands/__pycache__/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      194 2023-02-21 12:13:21.000000 obis-0.4.2rc7/obis/dm/commands/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1867 2023-03-29 14:28:25.000000 obis-0.4.2rc7/obis/dm/commands/__pycache__/addref.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3935 2023-02-28 09:09:45.000000 obis-0.4.2rc7/obis/dm/commands/__pycache__/clone.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3041 2023-02-28 09:44:21.000000 obis-0.4.2rc7/obis/dm/commands/__pycache__/collection.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3046 2023-02-21 16:35:01.000000 obis-0.4.2rc7/obis/dm/commands/__pycache__/download.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3343 2023-03-03 14:34:14.000000 obis-0.4.2rc7/obis/dm/commands/__pycache__/download_physical.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2416 2023-02-21 12:17:13.000000 obis-0.4.2rc7/obis/dm/commands/__pycache__/move.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3263 2023-03-01 08:22:27.000000 obis-0.4.2rc7/obis/dm/commands/__pycache__/object.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    10941 2023-03-30 10:21:33.000000 obis-0.4.2rc7/obis/dm/commands/__pycache__/openbis_command.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     6680 2023-02-21 12:17:13.000000 obis-0.4.2rc7/obis/dm/commands/__pycache__/openbis_sync.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3273 2023-02-21 12:17:13.000000 obis-0.4.2rc7/obis/dm/commands/__pycache__/removeref.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     9355 2023-07-24 14:12:45.000000 obis-0.4.2rc7/obis/dm/commands/__pycache__/search.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1589 2023-02-24 12:01:17.000000 obis-0.4.2rc7/obis/dm/commands/__pycache__/upload.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1897 2023-03-29 14:28:17.000000 obis-0.4.2rc7/obis/dm/commands/addref.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     5292 2023-02-28 08:49:14.000000 obis-0.4.2rc7/obis/dm/commands/clone.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3657 2023-02-28 09:16:53.000000 obis-0.4.2rc7/obis/dm/commands/collection.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3920 2023-02-21 13:31:53.000000 obis-0.4.2rc7/obis/dm/commands/download.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     4124 2023-03-03 14:31:58.000000 obis-0.4.2rc7/obis/dm/commands/download_physical.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2967 2023-02-21 12:05:41.000000 obis-0.4.2rc7/obis/dm/commands/move.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     4373 2023-03-01 08:22:23.000000 obis-0.4.2rc7/obis/dm/commands/object.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    12135 2023-03-30 10:21:12.000000 obis-0.4.2rc7/obis/dm/commands/openbis_command.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1535 2023-02-21 12:05:41.000000 obis-0.4.2rc7/obis/dm/commands/openbis_command_test.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     9774 2023-02-21 12:05:41.000000 obis-0.4.2rc7/obis/dm/commands/openbis_sync.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3565 2023-02-21 12:05:41.000000 obis-0.4.2rc7/obis/dm/commands/removeref.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    13251 2023-07-24 14:18:28.000000 obis-0.4.2rc7/obis/dm/commands/search.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1801 2023-02-24 12:00:59.000000 obis-0.4.2rc7/obis/dm/commands/upload.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    16039 2023-02-21 12:05:42.000000 obis-0.4.2rc7/obis/dm/config.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2934 2023-02-21 12:05:41.000000 obis-0.4.2rc7/obis/dm/config_test.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    27953 2023-03-30 13:30:39.000000 obis-0.4.2rc7/obis/dm/data_mgmt.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    14376 2023-03-29 13:51:23.000000 obis-0.4.2rc7/obis/dm/data_mgmt_test.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      245 2023-02-20 13:30:53.000000 obis-0.4.2rc7/obis/dm/git-annex-attributes
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     8502 2023-03-30 10:32:13.000000 obis-0.4.2rc7/obis/dm/git.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1905 2023-02-21 12:05:41.000000 obis-0.4.2rc7/obis/dm/repository_utils.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3789 2023-03-30 10:51:34.000000 obis-0.4.2rc7/obis/dm/utils.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      980 2023-02-21 12:05:41.000000 obis-0.4.2rc7/obis/dm/utils_test.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-24 14:31:39.504896 obis-0.4.2rc7/obis/scripts/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      919 2023-02-21 12:05:41.000000 obis-0.4.2rc7/obis/scripts/__init__.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-24 14:31:39.504896 obis-0.4.2rc7/obis/scripts/__pycache__/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      431 2023-02-21 12:13:22.000000 obis-0.4.2rc7/obis/scripts/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    30930 2023-07-24 10:38:42.000000 obis-0.4.2rc7/obis/scripts/__pycache__/cli.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      746 2023-02-21 12:13:22.000000 obis-0.4.2rc7/obis/scripts/__pycache__/click_util.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     4351 2023-03-30 10:59:33.000000 obis-0.4.2rc7/obis/scripts/__pycache__/data_mgmt_runner.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    39340 2023-07-24 10:38:39.000000 obis-0.4.2rc7/obis/scripts/cli.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1126 2023-02-21 12:05:41.000000 obis-0.4.2rc7/obis/scripts/click_util.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     5701 2023-03-30 10:59:06.000000 obis-0.4.2rc7/obis/scripts/data_mgmt_runner.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-24 14:31:39.504896 obis-0.4.2rc7/obis/test-data/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)   160470 2023-02-20 13:30:53.000000 obis-0.4.2rc7/obis/test-data/snb-data.zip
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       43 2023-02-20 13:30:53.000000 obis-0.4.2rc7/obis/test-data/text-data-2.txt
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       32 2023-02-20 13:30:53.000000 obis-0.4.2rc7/obis/test-data/text-data.txt
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-24 14:31:39.488896 obis-0.4.2rc7/obis/test-data/user_config/
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-24 14:31:39.504896 obis-0.4.2rc7/obis/test-data/user_config/.obis/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      167 2023-02-20 13:30:53.000000 obis-0.4.2rc7/obis/test-data/user_config/.obis/config.json
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-24 14:31:39.492896 obis-0.4.2rc7/obis.egg-info/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    32149 2023-07-24 14:31:39.000000 obis-0.4.2rc7/obis.egg-info/PKG-INFO
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3124 2023-07-24 14:31:39.000000 obis-0.4.2rc7/obis.egg-info/SOURCES.txt
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)        1 2023-07-24 14:31:39.000000 obis-0.4.2rc7/obis.egg-info/dependency_links.txt
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       47 2023-07-24 14:31:39.000000 obis-0.4.2rc7/obis.egg-info/entry_points.txt
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)        1 2023-02-23 08:39:07.000000 obis-0.4.2rc7/obis.egg-info/not-zip-safe
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       37 2023-07-24 14:31:39.000000 obis-0.4.2rc7/obis.egg-info/requires.txt
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)        5 2023-07-24 14:31:39.000000 obis-0.4.2rc7/obis.egg-info/top_level.txt
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       38 2023-07-24 14:31:39.504896 obis-0.4.2rc7/setup.cfg
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1985 2023-07-24 14:31:36.000000 obis-0.4.2rc7/setup.py
```

### Comparing `obis-0.4.2rc6/CHANGELOG.md` & `obis-0.4.2rc7/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # New in version 0.4.2
 
 * Added filtering by object in object and data_set search commands
 * Added recursive search to object and data_set search commands
 * Updated documentation regarding authentication
 * Added dataset ids to sample search results
-* changed pybis dependency to version == 1.35.11
+* changed pybis dependency to version == 1.36.0
 
 # New in version 0.4.1
 
 * Fixed parameters for determine_hostname method in addref functionality 
 
 # New in version 0.4.0.1
```

### Comparing `obis-0.4.2rc6/LICENSE` & `obis-0.4.2rc7/LICENSE`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/PKG-INFO` & `obis-0.4.2rc7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obis
-Version: 0.4.2rc6
+Version: 0.4.2rc7
 Summary: Local data management with assistance from OpenBIS.
 Home-page: https://sissource.ethz.ch/sispub/openbis/tree/master/app-openbis-command-line
 Author: ID SIS • ETH Zürich
 Author-email: openbis-support@id.ethz.ch
 License: Apache Software License Version 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `obis-0.4.2rc6/README.md` & `obis-0.4.2rc7/README.md`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/man/man1/obis-addref.1` & `obis-0.4.2rc7/man/man1/obis-addref.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/man/man1/obis-clone.1` & `obis-0.4.2rc7/man/man1/obis-clone.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/man/man1/obis-collection.1` & `obis-0.4.2rc7/man/man1/obis-collection.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/man/man1/obis-commit.1` & `obis-0.4.2rc7/man/man1/obis-commit.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/man/man1/obis-config.1` & `obis-0.4.2rc7/man/man1/obis-config.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/man/man1/obis-data_set.1` & `obis-0.4.2rc7/man/man1/obis-data_set.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/man/man1/obis-download.1` & `obis-0.4.2rc7/man/man1/obis-download.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/man/man1/obis-init.1` & `obis-0.4.2rc7/man/man1/obis-init.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/man/man1/obis-init_analysis.1` & `obis-0.4.2rc7/man/man1/obis-init_analysis.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/man/man1/obis-move.1` & `obis-0.4.2rc7/man/man1/obis-move.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/man/man1/obis-object.1` & `obis-0.4.2rc7/man/man1/obis-object.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/man/man1/obis-removeref.1` & `obis-0.4.2rc7/man/man1/obis-removeref.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/man/man1/obis-repository.1` & `obis-0.4.2rc7/man/man1/obis-repository.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/man/man1/obis-settings.1` & `obis-0.4.2rc7/man/man1/obis-settings.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/man/man1/obis-status.1` & `obis-0.4.2rc7/man/man1/obis-status.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/man/man1/obis-sync.1` & `obis-0.4.2rc7/man/man1/obis-sync.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/man/man1/obis.1` & `obis-0.4.2rc7/man/man1/obis.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/__init__.py` & `obis-0.4.2rc7/obis/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,10 +10,10 @@
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 __author__ = "ID SIS • ETH Zürich"
 __email__ = "openbis-support@id.ethz.ch"
-__version__ = "0.4.2rc5"
+__version__ = "0.4.2rc7"
 
 from .dm import *
```

### Comparing `obis-0.4.2rc6/obis/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc` & `obis-0.4.2rc7/obis/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/conftest.py` & `obis-0.4.2rc7/obis/conftest.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/__init__.py` & `obis-0.4.2rc7/obis/dm/__init__.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/__pycache__/checksum.cpython-310.pyc` & `obis-0.4.2rc7/obis/dm/__pycache__/checksum.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/__pycache__/command_log.cpython-310.pyc` & `obis-0.4.2rc7/obis/dm/__pycache__/command_log.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/__pycache__/command_result.cpython-310.pyc` & `obis-0.4.2rc7/obis/dm/__pycache__/command_result.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/__pycache__/config.cpython-310.pyc` & `obis-0.4.2rc7/obis/dm/__pycache__/config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/__pycache__/data_mgmt.cpython-310.pyc` & `obis-0.4.2rc7/obis/dm/__pycache__/data_mgmt.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/__pycache__/data_mgmt_test.cpython-310-pytest-7.2.1.pyc` & `obis-0.4.2rc7/obis/dm/__pycache__/data_mgmt_test.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/__pycache__/git.cpython-310.pyc` & `obis-0.4.2rc7/obis/dm/__pycache__/git.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/__pycache__/repository_utils.cpython-310.pyc` & `obis-0.4.2rc7/obis/dm/__pycache__/repository_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/__pycache__/utils.cpython-310.pyc` & `obis-0.4.2rc7/obis/dm/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/checksum.py` & `obis-0.4.2rc7/obis/dm/checksum.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/command_log.py` & `obis-0.4.2rc7/obis/dm/command_log.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/command_result.py` & `obis-0.4.2rc7/obis/dm/command_result.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/commands/__init__.py` & `obis-0.4.2rc7/obis/dm/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/commands/__pycache__/addref.cpython-310.pyc` & `obis-0.4.2rc7/obis/dm/commands/__pycache__/addref.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/commands/__pycache__/clone.cpython-310.pyc` & `obis-0.4.2rc7/obis/dm/commands/__pycache__/clone.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/commands/__pycache__/collection.cpython-310.pyc` & `obis-0.4.2rc7/obis/dm/commands/__pycache__/collection.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/commands/__pycache__/download.cpython-310.pyc` & `obis-0.4.2rc7/obis/dm/commands/__pycache__/download.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/commands/__pycache__/download_physical.cpython-310.pyc` & `obis-0.4.2rc7/obis/dm/commands/__pycache__/download_physical.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/commands/__pycache__/move.cpython-310.pyc` & `obis-0.4.2rc7/obis/dm/commands/__pycache__/move.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/commands/__pycache__/object.cpython-310.pyc` & `obis-0.4.2rc7/obis/dm/commands/__pycache__/object.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/commands/__pycache__/openbis_command.cpython-310.pyc` & `obis-0.4.2rc7/obis/dm/commands/__pycache__/openbis_command.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/commands/__pycache__/openbis_sync.cpython-310.pyc` & `obis-0.4.2rc7/obis/dm/commands/__pycache__/openbis_sync.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/commands/__pycache__/removeref.cpython-310.pyc` & `obis-0.4.2rc7/obis/dm/commands/__pycache__/removeref.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/commands/__pycache__/search.cpython-310.pyc` & `obis-0.4.2rc7/obis/dm/commands/__pycache__/search.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 17 10:12:16 2023 UTC, .py size: 12372 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,521 +1,585 @@
-00000000: 6f0d 0d0a 0000 0000 0014 b564 5430 0000  o..........dT0..
+00000000: 6f0d 0d0a 0000 0000 db86 be64 ca38 0000  o..........d.8..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 9400 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 9000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a03 6400  d.l.Z.d.d.l.Z.d.
-00000040: 6402 6c04 6d05 5a05 0100 6400 6403 6c06  d.l.m.Z...d.d.l.
-00000050: 6d07 5a07 0100 6404 6405 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
-00000060: 0100 6406 6407 6c0a 6d0b 5a0b 0100 6406  ..d.d.l.m.Z...d.
-00000070: 6408 6c0c 6d0d 5a0d 0100 6409 640a 6c0e  d.l.m.Z...d.d.l.
-00000080: 6d0f 5a0f 0100 640b 640c 8400 5a10 640d  m.Z...d.d...Z.d.
-00000090: 640e 8400 5a11 640f 6410 8400 5a12 6411  d...Z.d.d...Z.d.
-000000a0: 6412 8400 5a13 6413 6414 8400 5a14 4700  d...Z.d.d...Z.G.
-000000b0: 6415 6416 8400 6416 6509 8303 5a15 6401  d.d...d.e...Z.d.
-000000c0: 5300 2917 e900 0000 004e 2901 da23 6973  S.)......N)..#is
-000000d0: 5f6f 665f 6f70 656e 6269 735f 7375 7070  _of_openbis_supp
-000000e0: 6f72 7465 645f 6461 7465 5f66 6f72 6d61  orted_date_forma
-000000f0: 7429 01da 0653 616d 706c 65e9 0100 0000  t)...Sample.....
-00000100: 2901 da0e 4f70 656e 6269 7343 6f6d 6d61  )...OpenbisComma
-00000110: 6e64 e902 0000 0029 01da 0d43 6f6d 6d61  nd.....)...Comma
-00000120: 6e64 5265 7375 6c74 2901 da02 6364 e903  ndResult)...cd..
-00000130: 0000 0029 01da 0a63 6c69 636b 5f65 6368  ...)...click_ech
-00000140: 6f63 0400 0000 0000 0000 0000 0000 0f00  oc..............
-00000150: 0000 0900 0000 0300 0000 7330 0100 0074  ..........s0...t
-00000160: 006a 016a 0264 0164 028d 018f 877d 0474  .j.j.d.d.....}.t
-00000170: 006a 016a 0264 0364 028d 018f 677d 0587  .j.j.d.d....g}..
-00000180: 0066 0164 0464 0584 087c 0044 0083 017d  .f.d.d...|.D...}
-00000190: 0674 0383 007d 077c 06a0 04a1 0001 0067  .t...}.|.......g
-000001a0: 007d 087c 0672 6f7c 04a0 057c 027c 06a1  .}.|.ro|...|.|..
-000001b0: 027d 0967 007d 0667 007d 0a67 007d 0b7c  .}.g.}.g.}.g.}.|
-000001c0: 0944 005d 227d 0c7c 0c6a 0688 0019 0064  .D.]"}.|.j.....d
-000001d0: 0619 007d 0d7c 0a74 077c 0c6a 0664 0719  ...}.|.t.|.j.d..
-000001e0: 0083 0164 0619 0037 007d 0a7c 0d7c 0776  ...d...7.}.|.|.v
-000001f0: 0172 547c 07a0 087c 0da1 0101 007c 0b7c  .rT|...|.....|.|
-00000200: 0d67 0137 007d 0b71 327c 0b72 5f7c 087c  .g.7.}.q2|.r_|.|
-00000210: 05a0 057c 037c 0ba1 0237 007d 087c 0a44  ...|.|...7.}.|.D
-00000220: 005d 0b7d 0e7c 0e7c 0776 0172 6c7c 067c  .].}.|.|.v.rl|.|
-00000230: 0e67 0137 007d 0671 617c 0673 2457 0064  .g.7.}.qa|.s$W.d
-00000240: 0804 0004 0083 0301 006e 1031 0073 7977  .........n.1.syw
-00000250: 0101 0001 0001 0059 0001 0057 0064 0804  .......Y...W.d..
-00000260: 0004 0083 0301 007c 0853 0057 0064 0804  .......|.S.W.d..
-00000270: 0004 0083 0301 007c 0853 0031 0073 9177  .......|.S.1.s.w
-00000280: 0101 0001 0001 0059 0001 007c 0853 0029  .......Y...|.S.)
-00000290: 097a 4648 656c 7065 7220 6675 6e63 7469  .zFHelper functi
-000002a0: 6f6e 2074 6861 7420 7065 7266 6f72 6d20  on that perform 
-000002b0: 4446 5320 7365 6172 6368 206f 7665 7220  DFS search over 
-000002c0: 6368 696c 6472 656e 2067 7261 7068 206f  children graph o
-000002d0: 6620 6f62 6a65 6374 73e9 0500 0000 a901  f objects.......
-000002e0: da0b 6d61 785f 776f 726b 6572 73e9 1400  ..max_workers...
-000002f0: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
-00000300: 0000 0005 0000 0013 0000 0073 1600 0000  ...........s....
-00000310: 6700 7c00 5d07 7d01 7400 7c01 8800 8302  g.|.].}.t.|.....
-00000320: 9102 7102 5300 a900 2901 da07 6765 7461  ..q.S...)...geta
-00000330: 7474 7229 02da 022e 30da 0b6f 7065 6e62  ttr)....0..openb
-00000340: 6973 5f6f 626a a901 da04 7072 6f70 720f  is_obj....propr.
-00000350: 0000 00fa 632f 686f 6d65 2f61 6c61 736b  ....c/home/alask
-00000360: 6f77 736b 692f 7265 706f 2f6f 7065 6e62  owski/repo/openb
-00000370: 6973 5f70 7974 686f 6e2f 6170 702d 6f70  is_python/app-op
-00000380: 656e 6269 732d 636f 6d6d 616e 642d 6c69  enbis-command-li
-00000390: 6e65 2f73 7263 2f70 7974 686f 6e2f 6f62  ne/src/python/ob
-000003a0: 6973 2f64 6d2f 636f 6d6d 616e 6473 2f73  is/dm/commands/s
-000003b0: 6561 7263 682e 7079 da0a 3c6c 6973 7463  earch.py..<listc
-000003c0: 6f6d 703e 2100 0000 7302 0000 0016 007a  omp>!...s......z
-000003d0: 185f 6466 732e 3c6c 6f63 616c 733e 2e3c  ._dfs.<locals>.<
-000003e0: 6c69 7374 636f 6d70 3e72 0100 0000 da08  listcomp>r......
-000003f0: 6368 696c 6472 656e 4e29 09da 0a63 6f6e  childrenN)...con
-00000400: 6375 7272 656e 74da 0766 7574 7572 6573  current..futures
-00000410: da12 5468 7265 6164 506f 6f6c 4578 6563  ..ThreadPoolExec
-00000420: 7574 6f72 da03 7365 74da 0772 6576 6572  utor..set..rever
-00000430: 7365 da03 6d61 70da 0264 66da 046c 6973  se..map..df..lis
-00000440: 74da 0361 6464 290f da07 6f62 6a65 6374  t..add)...object
-00000450: 7372 1400 0000 da04 6675 6e63 da0d 6675  sr......func..fu
-00000460: 6e63 5f73 7065 6369 6669 63da 0b70 6f6f  nc_specific..poo
-00000470: 6c5f 7369 6d70 6c65 da09 706f 6f6c 5f66  l_simple..pool_f
-00000480: 756c 6cda 0573 7461 636b da07 7669 7369  ull..stack..visi
-00000490: 7465 64da 066f 7574 7075 74da 0e73 696d  ted..output..sim
-000004a0: 706c 655f 7265 7375 6c74 7372 1700 0000  ple_resultsr....
-000004b0: da0d 6675 6c6c 5f64 6f77 6e6c 6f61 64da  ..full_download.
-000004c0: 036f 626a da03 6b65 79da 0563 6869 6c64  .obj..key..child
-000004d0: 720f 0000 0072 1300 0000 7215 0000 00da  r....r....r.....
-000004e0: 045f 6466 731c 0000 0073 5000 0000 0602  ._dfs....sP.....
-000004f0: 0201 06ff 0801 0201 04ff 02ff 0202 0a01  ................
-00000500: 0201 06ff 0602 0801 0401 0401 0c01 0401  ................
-00000510: 0401 0401 0801 0e01 1601 0801 0a01 0a01  ................
-00000520: 0280 0401 1001 0801 0801 0a01 0280 04f1  ................
-00000530: 0280 28f8 0419 0ce7 0419 10e7 0419 722e  ..(...........r.
-00000540: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-00000550: 0400 0000 0800 0000 4300 0000 7344 0000  ........C...sD..
-00000560: 0067 007d 0274 006a 016a 0264 0164 028d  .g.}.t.j.j.d.d..
-00000570: 018f 0f7d 037c 03a0 037c 007c 01a1 027d  ...}.|...|.|...}
-00000580: 0257 0064 0004 0004 0083 0301 007c 0253  .W.d.........|.S
-00000590: 0031 0073 1b77 0101 0001 0001 0059 0001  .1.s.w.......Y..
-000005a0: 007c 0253 0029 034e 720b 0000 0072 0c00  .|.S.).Nr....r..
-000005b0: 0000 2904 7218 0000 0072 1900 0000 721a  ..).r....r....r.
-000005c0: 0000 0072 1d00 0000 2904 da12 6765 745f  ...r....)...get_
-000005d0: 6461 7461 7365 745f 6d65 7468 6f64 da07  dataset_method..
-000005e0: 7361 6d70 6c65 7372 2800 0000 7224 0000  samplesr(...r$..
-000005f0: 0072 0f00 0000 720f 0000 0072 1500 0000  .r....r....r....
-00000600: da18 5f67 6574 5f64 6174 6173 6574 735f  .._get_datasets_
-00000610: 6f66 5f73 616d 706c 6573 3a00 0000 7314  of_samples:...s.
-00000620: 0000 0004 0106 0102 0106 ff02 010e 010a  ................
-00000630: fe04 0410 fc04 0472 3100 0000 6301 0000  .......r1...c...
-00000640: 0000 0000 0000 0000 0003 0000 0003 0000  ................
-00000650: 0043 0000 0073 1a00 0000 6700 7d01 7c00  .C...s....g.}.|.
-00000660: 4400 5d06 7d02 7c01 7c02 3700 7d01 7104  D.].}.|.|.7.}.q.
-00000670: 7c01 5300 2901 4e72 0f00 0000 2903 da06  |.S.).Nr....)...
-00000680: 6d61 7472 6978 da09 666c 6174 5f6c 6973  matrix..flat_lis
-00000690: 74da 0372 6f77 720f 0000 0072 0f00 0000  t..rowr....r....
-000006a0: 7215 0000 00da 0766 6c61 7474 656e 4300  r......flattenC.
-000006b0: 0000 7308 0000 0004 0108 010a 0104 0172  ..s............r
-000006c0: 3500 0000 6303 0000 0000 0000 0000 0000  5...c...........
-000006d0: 0005 0000 0003 0000 0043 0000 0073 6a00  .........C...sj.
-000006e0: 0000 7400 7c01 8301 7231 7400 7c02 8301  ..t.|...r1t.|...
-000006f0: 7231 7401 a002 7c01 a101 7d03 7401 a002  r1t...|...}.t...
-00000700: 7c02 a101 7d04 7c00 6401 6b02 721a 7c04  |...}.|.d.k.r.|.
-00000710: 7c03 6b02 5300 7c00 6402 6b02 7222 7c04  |.k.S.|.d.k.r"|.
-00000720: 7c03 6b04 5300 7c00 6403 6b02 722a 7c04  |.k.S.|.d.k.r*|.
-00000730: 7c03 6b00 5300 7403 6404 7c00 9b00 9d02  |.k.S.t.d.|.....
-00000740: 8301 8201 7403 6405 8301 8201 2906 4efa  ....t.d.....).N.
-00000750: 013d fa01 3efa 013c 7a0d 556e 6b6e 6f77  .=..>..<z.Unknow
-00000760: 6e20 7369 676e 207a 2544 6174 6573 2061  n sign z%Dates a
-00000770: 7265 206e 6f74 2069 6e20 6120 7375 7070  re not in a supp
-00000780: 6f72 7465 6420 666f 726d 6174 7321 2904  orted formats!).
-00000790: 7202 0000 00da 0270 64da 0b74 6f5f 6461  r......pd..to_da
-000007a0: 7465 7469 6d65 da0a 5661 6c75 6545 7272  tetime..ValueErr
-000007b0: 6f72 2905 da04 7369 676e da05 6461 7465  or)...sign..date
-000007c0: 31da 0564 6174 6532 da0a 7469 6d65 7374  1..date2..timest
-000007d0: 616d 7031 da0a 7469 6d65 7374 616d 7032  amp1..timestamp2
-000007e0: 720f 0000 0072 0f00 0000 7215 0000 00da  r....r....r.....
-000007f0: 0b5f 6368 6563 6b5f 6461 7465 4a00 0000  ._check_dateJ...
-00000800: 7316 0000 0010 010a 010a 0108 0108 0108  s...............
-00000810: 0108 0108 0108 010e 0108 0272 4100 0000  ...........rA...
-00000820: 6302 0000 0000 0000 0000 0000 0009 0000  c...............
-00000830: 0004 0000 0043 0000 0073 d001 0000 7c01  .....C...s....|.
-00000840: a000 6401 6400 a102 6400 7501 7229 7c01  ..d.d...d.u.r)|.
-00000850: 6401 1900 7d02 7c00 6a01 6400 7501 721a  d...}.|.j.d.u.r.
-00000860: 7c00 6a01 6a02 6a03 7c02 6b03 721a 6402  |.j.j.j.|.k.r.d.
-00000870: 5300 7c00 6a04 6400 7501 7229 7c00 6a04  S.|.j.d.u.r)|.j.
-00000880: 6a05 6a02 6a03 7c02 6b03 7229 6402 5300  j.j.j.|.k.r)d.S.
-00000890: 7c01 a000 6403 6400 a102 6400 7501 723b  |...d.d...d.u.r;
-000008a0: 7c00 6a06 6a03 7c01 6403 1900 6b03 723b  |.j.j.|.d...k.r;
-000008b0: 6402 5300 7c01 a000 6404 6400 a102 6400  d.S.|...d.d...d.
-000008c0: 7501 7263 7c01 6404 1900 7d03 7c00 6a01  u.rc|.d...}.|.j.
-000008d0: 6400 7501 7255 7c00 6a01 6a05 6a03 7c03  d.u.rU|.j.j.j.|.
-000008e0: 6b03 7255 6402 5300 7c00 6a04 6400 7501  k.rUd.S.|.j.d.u.
-000008f0: 7263 7c00 6a04 6a05 6a03 7c03 6b03 7263  rc|.j.j.j.|.k.rc
-00000900: 6402 5300 7c01 a000 6405 6400 a102 6400  d.S.|...d.d...d.
-00000910: 7501 727a 7c00 6a04 6400 7501 727a 7c00  u.rz|.j.d.u.rz|.
-00000920: 6a04 6a03 7c01 6405 1900 6b03 727a 6402  j.j.|.d...k.rzd.
-00000930: 5300 7c01 a000 6406 6400 a102 6400 7501  S.|...d.d...d.u.
-00000940: 729a 7c01 6406 1900 7d04 7c01 6407 1900  r.|.d...}.|.d...
-00000950: 7d05 7c00 6a07 6400 7501 729a 7c00 6a07  }.|.j.d.u.r.|.j.
-00000960: 7c04 a008 a100 1900 7c05 6b03 729a 6402  |.......|.k.r.d.
-00000970: 5300 7c01 a000 6408 6400 a102 6400 7501  S.|...d.d...d.u.
-00000980: 72c0 7c01 6408 1900 7d06 6409 7d07 7c06  r.|.d...}.d.}.|.
-00000990: 640a 1900 640b 7600 72b9 7c06 640a 1900  d...d.v.r.|.d...
-000009a0: 7c06 640c 6400 8502 1900 0202 7d07 7d06  |.d.d.......}.}.
-000009b0: 7409 7c07 7c06 7c00 6a0a 8303 5300 7c01  t.|.|.|.j...S.|.
-000009c0: a000 640d 6400 a102 6400 7501 72e6 7c01  ..d.d...d.u.r.|.
-000009d0: 640d 1900 7d08 6409 7d07 7c08 640a 1900  d...}.d.}.|.d...
-000009e0: 640b 7600 72df 7c08 640a 1900 7c08 640c  d.v.r.|.d...|.d.
-000009f0: 6400 8502 1900 0202 7d07 7d08 7409 7c07  d.......}.}.t.|.
-00000a00: 7c08 7c00 6a0b 8303 5300 640e 5300 290f  |.|.j...S.d.S.).
-00000a10: 4eda 0573 7061 6365 46da 0974 7970 655f  N..spaceF..type_
-00000a20: 636f 6465 da07 7072 6f6a 6563 74da 0a65  code..project..e
-00000a30: 7870 6572 696d 656e 74da 0d70 726f 7065  xperiment..prope
-00000a40: 7274 795f 636f 6465 da0e 7072 6f70 6572  rty_code..proper
-00000a50: 7479 5f76 616c 7565 da11 7265 6769 7374  ty_value..regist
-00000a60: 7261 7469 6f6e 5f64 6174 6572 3600 0000  ration_dater6...
-00000a70: 7201 0000 0029 0372 3700 0000 7238 0000  r....).r7...r8..
-00000a80: 0072 3600 0000 7204 0000 00da 116d 6f64  .r6...r......mod
-00000a90: 6966 6963 6174 696f 6e5f 6461 7465 5429  ification_dateT)
-00000aa0: 0cda 0367 6574 da06 7361 6d70 6c65 7242  ...get..samplerB
-00000ab0: 0000 00da 0463 6f64 6572 4500 0000 7244  .....coderE...rD
-00000ac0: 0000 00da 0474 7970 65da 0570 726f 7073  .....type..props
-00000ad0: da05 6c6f 7765 7272 4100 0000 da10 7265  ..lowerrA.....re
-00000ae0: 6769 7374 7261 7469 6f6e 4461 7465 da10  gistrationDate..
-00000af0: 6d6f 6469 6669 6361 7469 6f6e 4461 7465  modificationDate
-00000b00: 2909 da07 6461 7461 7365 74da 0766 696c  )...dataset..fil
-00000b10: 7465 7273 7242 0000 0072 4400 0000 da09  tersrB...rD.....
-00000b20: 7072 6f70 5f63 6f64 65da 0a70 726f 705f  prop_code..prop_
-00000b30: 7661 6c75 6572 4800 0000 723c 0000 0072  valuerH...r<...r
-00000b40: 4900 0000 720f 0000 0072 0f00 0000 7215  I...r....r....r.
-00000b50: 0000 00da 0f5f 6669 6c74 6572 5f64 6174  ....._filter_dat
-00000b60: 6173 6574 5900 0000 7348 0000 0010 0108  asetY...sH......
-00000b70: 0118 0104 011a 0104 0110 0110 0104 0110  ................
-00000b80: 0108 0118 0104 0118 0104 0110 011a 0104  ................
-00000b90: 0110 0108 0108 011c 0104 0110 0108 0104  ................
-00000ba0: 010c 0116 010e 0110 0108 0104 010c 0116  ................
-00000bb0: 010e 0104 0172 5600 0000 6300 0000 0000  .....rV...c.....
-00000bc0: 0000 0000 0000 0000 0000 0003 0000 0000  ................
-00000bd0: 0000 0073 5800 0000 6500 5a01 6400 5a02  ...sX...e.Z.d.Z.
-00000be0: 6401 5a03 8700 6601 6402 6403 8408 5a04  d.Z...f.d.d...Z.
-00000bf0: 6404 6405 8400 5a05 6406 6407 8400 5a06  d.d...Z.d.d...Z.
-00000c00: 6408 6409 8400 5a07 640a 640b 8400 5a08  d.d...Z.d.d...Z.
-00000c10: 640c 640d 8400 5a09 640e 640f 8400 5a0a  d.d...Z.d.d...Z.
-00000c20: 6410 6411 8400 5a0b 8700 0400 5a0c 5300  d.d...Z.....Z.S.
-00000c30: 2912 da06 5365 6172 6368 7a3b 0a20 2020  )...Searchz;.   
-00000c40: 2043 6f6d 6d61 6e64 2074 6f20 7365 6172   Command to sear
-00000c50: 6368 2073 616d 706c 6573 206f 7220 6461  ch samples or da
-00000c60: 7461 7365 7473 2069 6e20 6f70 656e 4249  tasets in openBI
-00000c70: 532e 0a20 2020 2063 0500 0000 0000 0000  S..    c........
-00000c80: 0000 0000 0500 0000 0300 0000 0300 0000  ................
-00000c90: 7336 0000 007c 027c 005f 007c 037c 005f  s6...|.|._.|.|._
-00000ca0: 017c 047c 005f 027c 00a0 037c 01a1 0101  .|.|._.|...|....
-00000cb0: 0064 017c 005f 0474 0574 067c 0083 02a0  .d.|._.t.t.|....
-00000cc0: 077c 01a1 0101 0064 0253 0029 0361 1001  .|.....d.S.).a..
-00000cd0: 0000 0a20 2020 2020 2020 203a 7061 7261  ...        :para
-00000ce0: 6d20 646d 3a20 6461 7461 206d 616e 6167  m dm: data manag
-00000cf0: 656d 656e 740a 2020 2020 2020 2020 3a70  ement.        :p
-00000d00: 6172 616d 2066 696c 7465 7273 3a20 4469  aram filters: Di
-00000d10: 6374 696f 6e61 7279 206f 6620 6669 6c74  ctionary of filt
-00000d20: 6572 2074 6f20 6265 2075 7365 6420 6475  er to be used du
-00000d30: 7269 6e67 2073 6561 7263 680a 2020 2020  ring search.    
-00000d40: 2020 2020 3a70 6172 616d 2072 6563 7572      :param recur
-00000d50: 7369 7665 3a20 466c 6167 2069 6e64 6963  sive: Flag indic
-00000d60: 6174 696e 6720 7265 6375 7273 6976 6520  ating recursive 
-00000d70: 7365 6172 6368 2069 6e20 6368 696c 6472  search in childr
-00000d80: 656e 0a20 2020 2020 2020 203a 7061 7261  en.        :para
-00000d90: 6d20 7361 7665 5f70 6174 683a 2050 6174  m save_path: Pat
-00000da0: 6820 746f 2073 6176 6520 7265 7375 6c74  h to save result
-00000db0: 732e 2049 6620 6e6f 7420 7365 742c 2072  s. If not set, r
-00000dc0: 6573 756c 7473 2077 696c 6c20 6e6f 7420  esults will not 
-00000dd0: 6265 2073 6176 6564 2e0a 2020 2020 2020  be saved..      
-00000de0: 2020 da01 2a4e 2908 7253 0000 00da 0972    ..*N).rS.....r
-00000df0: 6563 7572 7369 7665 da09 7361 7665 5f70  ecursive..save_p
-00000e00: 6174 68da 126c 6f61 645f 676c 6f62 616c  ath..load_global
-00000e10: 5f63 6f6e 6669 6772 4e00 0000 da05 7375  _configrN.....su
-00000e20: 7065 7272 5700 0000 da08 5f5f 696e 6974  perrW.....__init
-00000e30: 5f5f 2905 da04 7365 6c66 da02 646d 7253  __)...self..dmrS
-00000e40: 0000 0072 5900 0000 725a 0000 00a9 01da  ...rY...rZ......
-00000e50: 095f 5f63 6c61 7373 5f5f 720f 0000 0072  .__class__r....r
-00000e60: 1500 0000 725d 0000 0085 0000 0073 0c00  ....r].......s..
-00000e70: 0000 0607 0601 0601 0a01 0601 1401 7a0f  ..............z.
-00000e80: 5365 6172 6368 2e5f 5f69 6e69 745f 5f63  Search.__init__c
-00000e90: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00000ea0: 0800 0000 4300 0000 738e 0000 007c 00a0  ....C...s....|..
-00000eb0: 00a1 007d 0174 0164 0174 027c 0183 019b  ...}.t.d.t.|....
-00000ec0: 009d 0283 0101 007c 006a 0364 0075 0172  .......|.j.d.u.r
-00000ed0: 3a74 0164 027c 006a 039b 009d 0283 0101  :t.d.|.j........
-00000ee0: 0074 047c 006a 056a 0683 018f 1101 007c  .t.|.j.j.......|
-00000ef0: 016a 076a 087c 006a 0364 0364 048d 0201  .j.j.|.j.d.d....
-00000f00: 0057 0064 0004 0004 0083 0301 006e 0831  .W.d.........n.1
-00000f10: 0073 3477 0101 0001 0001 0059 0001 006e  .s4w.......Y...n
-00000f20: 0774 0164 057c 019b 009d 0283 0101 0074  .t.d.|.........t
-00000f30: 0964 0664 0764 088d 0253 0029 094e 7a0f  .d.d.d...S.).Nz.
-00000f40: 4f62 6a65 6374 7320 666f 756e 643a 20fa  Objects found: .
-00000f50: 1953 6176 696e 6720 7365 6172 6368 2072  .Saving search r
-00000f60: 6573 756c 7473 2069 6e20 46a9 01da 0569  esults in F....i
-00000f70: 6e64 6578 fa10 5365 6172 6368 2072 6573  ndex..Search res
-00000f80: 756c 7473 3a0a 7201 0000 00fa 1153 6561  ults:.r......Sea
-00000f90: 7263 6820 636f 6d70 6c65 7465 642e a902  rch completed...
-00000fa0: da0a 7265 7475 726e 636f 6465 7228 0000  ..returncoder(..
-00000fb0: 0029 0ada 0f5f 7365 6172 6368 5f73 616d  .)..._search_sam
-00000fc0: 706c 6573 720a 0000 00da 036c 656e 725a  plesr......lenrZ
-00000fd0: 0000 0072 0800 0000 da09 6461 7461 5f6d  ...r......data_m
-00000fe0: 676d 74da 0f69 6e76 6f63 6174 696f 6e5f  gmt..invocation_
-00000ff0: 7061 7468 721e 0000 00da 0674 6f5f 6373  pathr......to_cs
-00001000: 7672 0700 0000 2902 725e 0000 00da 0e73  vr....).r^.....s
-00001010: 6561 7263 685f 7265 7375 6c74 7372 0f00  earch_resultsr..
-00001020: 0000 720f 0000 0072 1500 0000 da0e 7365  ..r....r......se
-00001030: 6172 6368 5f73 616d 706c 6573 9300 0000  arch_samples....
-00001040: 7314 0000 0008 0112 020a 0110 010e 0114  s...............
-00001050: 011c ff02 800e 030c 027a 1553 6561 7263  .........z.Searc
-00001060: 682e 7365 6172 6368 5f73 616d 706c 6573  h.search_samples
-00001070: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00001080: 0004 0000 0043 0000 0073 1400 0000 7c00  .....C...s....|.
-00001090: 6a00 6a01 7c01 6401 6402 6702 6403 8d02  j.j.|.d.d.g.d...
-000010a0: 5300 2904 4e72 1700 0000 da08 6461 7461  S.).Nr......data
-000010b0: 5365 7473 a901 da05 6174 7472 7329 02da  Sets....attrs)..
-000010c0: 076f 7065 6e62 6973 da0b 6765 745f 7361  .openbis..get_sa
-000010d0: 6d70 6c65 73a9 0272 5e00 0000 da0a 6964  mples..r^.....id
-000010e0: 656e 7469 6669 6572 720f 0000 0072 0f00  entifierr....r..
-000010f0: 0000 7215 0000 00da 155f 6765 745f 7361  ..r......_get_sa
-00001100: 6d70 6c65 735f 6368 696c 6472 656e a000  mples_children..
-00001110: 0000 7302 0000 0014 017a 1c53 6561 7263  ..s......z.Searc
-00001120: 682e 5f67 6574 5f73 616d 706c 6573 5f63  h._get_samples_c
-00001130: 6869 6c64 7265 6e63 0200 0000 0000 0000  hildrenc........
-00001140: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
-00001150: 7310 0000 007c 006a 006a 017c 0164 0164  s....|.j.j.|.d.d
-00001160: 028d 0253 0029 034e 5429 01da 0e77 6974  ...S.).NT)...wit
-00001170: 6844 6174 6153 6574 4964 7329 0272 7300  hDataSetIds).rs.
-00001180: 0000 da0a 6765 745f 7361 6d70 6c65 7275  ....get_sampleru
-00001190: 0000 0072 0f00 0000 720f 0000 0072 1500  ...r....r....r..
-000011a0: 0000 da19 5f67 6574 5f73 616d 706c 655f  ...._get_sample_
-000011b0: 7769 7468 5f64 6174 6173 6574 73a3 0000  with_datasets...
-000011c0: 0073 0200 0000 1001 7a20 5365 6172 6368  .s......z Search
-000011d0: 2e5f 6765 745f 7361 6d70 6c65 5f77 6974  ._get_sample_wit
-000011e0: 685f 6461 7461 7365 7473 6301 0000 0000  h_datasetsc.....
-000011f0: 0000 0000 0000 0005 0000 0006 0000 0043  ...............C
-00001200: 0000 0073 a000 0000 6401 7c00 6a00 7600  ...s....d.|.j.v.
-00001210: 7215 7c00 6a01 6a02 7c00 6a00 6401 1900  r.|.j.j.|.j.d...
-00001220: 6700 6402 a201 7c00 6a03 6403 8d03 7d01  g.d...|.j.d...}.
-00001230: 6e12 7c00 a004 7c00 6a03 6700 6402 a201  n.|...|.j.g.d...
-00001240: a102 7d02 7c00 6a01 6a02 640b 6900 7c02  ..}.|.j.j.d.i.|.
-00001250: a401 8e01 7d01 7c00 6a05 724c 7406 6404  ....}.|.j.rLt.d.
-00001260: 8301 0100 7407 7c01 6a08 6405 7c00 6a09  ....t.|.j.d.|.j.
-00001270: 7c00 6a0a 8304 7d03 7c00 6a01 6a0b 7c00  |.j...}.|.j.j.|.
-00001280: 6a03 6406 6407 8400 7c03 4400 8301 6700  j.d.d...|.D...g.
-00001290: 6402 a201 6408 6409 8d04 7d04 7c04 5300  d...d.d...}.|.S.
-000012a0: 7c01 7d04 7c04 5300 290c 7a1f 4865 6c70  |.}.|.S.).z.Help
-000012b0: 6572 206d 6574 686f 6420 746f 2073 6561  er method to sea
-000012c0: 7263 6820 7361 6d70 6c65 73da 0b6f 626a  rch samples..obj
-000012d0: 6563 745f 636f 6465 2903 da07 7061 7265  ect_code)...pare
-000012e0: 6e74 7372 1700 0000 7270 0000 0029 0372  ntsr....rp...).r
-000012f0: 7600 0000 7272 0000 0072 4e00 0000 7a3e  v...rr...rN...z>
-00001300: 5265 6375 7273 6976 6520 7365 6172 6368  Recursive search
-00001310: 2065 6e61 626c 6564 2e20 4974 206d 6179   enabled. It may
-00001320: 2074 616b 6520 7469 6d65 2074 6f20 7072   take time to pr
-00001330: 6f64 7563 6520 7265 7375 6c74 732e 7276  oduce results.rv
-00001340: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00001350: 0200 0000 0300 0000 5300 0000 f312 0000  ........S.......
-00001360: 0067 007c 005d 057d 017c 016a 0091 0271  .g.|.].}.|.j...q
-00001370: 0253 0072 0f00 0000 a901 da04 6461 7461  .S.r........data
-00001380: 2902 7211 0000 0072 4b00 0000 720f 0000  ).r....rK...r...
-00001390: 0072 0f00 0000 7215 0000 0072 1600 0000  .r....r....r....
-000013a0: b700 0000 f302 0000 0012 007a 2a53 6561  ...........z*Sea
-000013b0: 7263 682e 5f73 6561 7263 685f 7361 6d70  rch._search_samp
-000013c0: 6c65 732e 3c6c 6f63 616c 733e 2e3c 6c69  les.<locals>.<li
-000013d0: 7374 636f 6d70 3e54 2904 724e 0000 00da  stcomp>T).rN....
-000013e0: 0872 6573 706f 6e73 6572 7200 0000 da06  .responserr.....
-000013f0: 7061 7273 6564 4e72 0f00 0000 290c 7253  parsedNr....).rS
-00001400: 0000 0072 7300 0000 7274 0000 0072 4e00  ...rs...rt...rN.
-00001410: 0000 da13 5f67 6574 5f66 696c 7465 7269  ...._get_filteri
-00001420: 6e67 5f61 7267 7372 5900 0000 720a 0000  ng_argsrY...r...
-00001430: 0072 2e00 0000 7221 0000 0072 7700 0000  .r....r!...rw...
-00001440: 727a 0000 00da 195f 7361 6d70 6c65 5f6c  rz....._sample_l
-00001450: 6973 745f 666f 725f 7265 7370 6f6e 7365  ist_for_response
-00001460: 2905 725e 0000 00da 0772 6573 756c 7473  ).r^.....results
-00001470: da04 6172 6773 7228 0000 0072 6e00 0000  ..argsr(...rn...
-00001480: 720f 0000 0072 0f00 0000 7215 0000 0072  r....r....r....r
-00001490: 6900 0000 a600 0000 732e 0000 000a 030e  i.......s.......
-000014a0: 0106 0104 0108 fe12 0412 0106 0208 0108  ................
-000014b0: 0104 0104 0104 fe0a 0306 0102 0104 ff06  ................
-000014c0: 0202 0206 fb04 0804 ff04 017a 1653 6561  ...........z.Sea
-000014d0: 7263 682e 5f73 6561 7263 685f 7361 6d70  rch._search_samp
-000014e0: 6c65 7363 0200 0000 0000 0000 0000 0000  lesc............
-000014f0: 0200 0000 0400 0000 4300 0000 7312 0000  ........C...s...
-00001500: 007c 006a 006a 017c 0164 0167 0164 028d  .|.j.j.|.d.g.d..
-00001510: 0253 0029 034e 7217 0000 0072 7100 0000  .S.).Nr....rq...
-00001520: 2902 7273 0000 00da 0c67 6574 5f64 6174  ).rs.....get_dat
-00001530: 6173 6574 7329 0272 5e00 0000 da06 7065  asets).r^.....pe
-00001540: 726d 4964 720f 0000 0072 0f00 0000 7215  rmIdr....r....r.
-00001550: 0000 00da 165f 6765 745f 6461 7461 7365  ....._get_datase
-00001560: 7473 5f63 6869 6c64 7265 6ec0 0000 0073  ts_children....s
-00001570: 0200 0000 1201 7a1d 5365 6172 6368 2e5f  ......z.Search._
-00001580: 6765 745f 6461 7461 7365 7473 5f63 6869  get_datasets_chi
-00001590: 6c64 7265 6e63 0100 0000 0000 0000 0000  ldrenc..........
-000015a0: 0000 0e00 0000 0800 0000 4300 0000 735c  ..........C...s\
-000015b0: 0200 007c 006a 0064 0075 0172 117c 00a0  ...|.j.d.u.r.|..
-000015c0: 01a1 0064 0075 0072 1174 0264 0164 0264  ...d.u.r.t.d.d.d
-000015d0: 038d 0253 007c 006a 03a0 04a1 007d 0164  ...S.|.j.....}.d
-000015e0: 0464 0584 007c 01a0 05a1 0044 0083 017d  .d...|.....D...}
-000015f0: 0264 0664 0584 007c 01a0 05a1 0044 0083  .d.d...|.....D..
-00001600: 017d 037c 0272 8964 077c 0276 0072 377c  .}.|.r.d.|.v.r7|
-00001610: 0264 0719 007c 0264 083c 007c 0264 073d  .d...|.d.<.|.d.=
-00001620: 007c 027c 005f 037c 00a0 06a1 007d 0464  .|.|._.|.....}.d
-00001630: 0964 0a84 0074 0774 086a 097c 0483 0244  .d...t.t.j.|...D
-00001640: 0083 017d 057c 0544 005d 297d 067c 066a  ...}.|.D.])}.|.j
-00001650: 0a44 005d 237d 0774 0b7c 077c 0383 0273  .D.]#}.t.|.|...s
-00001660: 7374 0c74 0d7c 066a 0e83 0183 0144 005d  st.t.|.j.....D.]
-00001670: 147d 087c 066a 0e7c 0819 0064 0b19 0064  .}.|.j.|...d...d
-00001680: 0b19 007c 076a 0f6b 0272 727c 066a 0e7c  ...|.j.k.rr|.j.|
-00001690: 083d 0001 006e 0171 5e71 5071 4b64 0c64  .=...n.q^qPqKd.d
-000016a0: 0a84 007c 0544 0083 017d 057c 006a 106a  ...|.D...}.|.j.j
-000016b0: 117c 006a 1274 137c 0583 0164 0d64 0e8d  .|.j.t.|...d.d..
-000016c0: 037d 056e 607c 006a 1472 be7c 00a0 06a1  .}.n`|.j.r.|....
-000016d0: 007d 0467 007d 097c 046a 0a44 005d 0e7d  .}.g.}.|.j.D.].}
-000016e0: 0a7c 097c 0a6a 0964 0f64 1067 027c 006a  .|.|.j.d.d.g.|.j
-000016f0: 1264 118d 0237 007d 0971 9574 157c 0964  .d...7.}.q.t.|.d
-00001700: 0b7c 006a 167c 006a 106a 1783 047d 0b7c  .|.j.|.j.j...}.|
-00001710: 006a 106a 117c 006a 1264 1264 0a84 007c  .j.j.|.j.d.d...|
-00001720: 0b44 0083 0164 0d64 0e8d 037d 056e 2b64  .D...d.d...}.n+d
-00001730: 137c 006a 0376 0072 d57c 006a 10a0 187c  .|.j.v.r.|.j...|
-00001740: 006a 0364 1319 00a1 016a 0964 0f64 1067  .j.d.....j.d.d.g
-00001750: 027c 006a 1264 118d 027d 0c6e 127c 00a0  .|.j.d...}.n.|..
-00001760: 197c 006a 1264 0f64 1067 02a1 027d 0d7c  .|.j.d.d.g...}.|
-00001770: 006a 106a 0964 1b69 007c 0da4 018e 017d  .j.j.d.i.|.....}
-00001780: 0c7c 0c7d 0574 1a64 1474 0d7c 0583 019b  .|.}.t.d.t.|....
-00001790: 009d 0283 0101 007c 006a 0064 0075 0190  .......|.j.d.u..
-000017a0: 0172 2174 1a64 157c 006a 009b 009d 0283  .r!t.d.|.j......
-000017b0: 0101 0074 1b7c 006a 1c6a 1d83 018f 1101  ...t.|.j.j......
-000017c0: 007c 056a 1e6a 1f7c 006a 0064 1664 178d  .|.j.j.|.j.d.d..
-000017d0: 0201 0057 0064 0004 0004 0083 0301 006e  ...W.d.........n
-000017e0: 0931 0090 0173 1b77 0101 0001 0001 0059  .1...s.w.......Y
-000017f0: 0001 006e 0774 1a64 187c 059b 009d 0283  ...n.t.d.|......
-00001800: 0101 0074 0264 1964 1a64 038d 0253 0029  ...t.d.d.d...S.)
-00001810: 1c4e e9ff ffff ff7a 3b43 6f6e 6669 6775  .N.....z;Configu
-00001820: 7261 7469 6f6e 2066 696c 6573 6572 7669  ration fileservi
-00001830: 6365 5f75 726c 206e 6565 6473 2074 6f20  ce_url needs to 
-00001840: 6265 2073 6574 2066 6f72 2064 6f77 6e6c  be set for downl
-00001850: 6f61 642e 7267 0000 0063 0100 0000 0000  oad.rg...c......
-00001860: 0000 0000 0000 0300 0000 0500 0000 5300  ..............S.
-00001870: 0000 7328 0000 0069 007c 005d 105c 027d  ..s(...i.|.].\.}
-00001880: 017d 027c 01a0 0064 00a1 0172 027c 0164  .}.|...d...r.|.d
-00001890: 0164 0285 0219 007c 0293 0271 0253 0029  .d.....|...q.S.)
-000018a0: 03da 076f 626a 6563 745f e907 0000 004e  ...object_.....N
-000018b0: a901 da0a 7374 6172 7473 7769 7468 a903  ....startswith..
-000018c0: 7211 0000 00da 016b da01 7672 0f00 0000  r......k..vr....
-000018d0: 720f 0000 0072 1500 0000 da0a 3c64 6963  r....r......<dic
-000018e0: 7463 6f6d 703e ca00 0000 7302 0000 0028  tcomp>....s....(
-000018f0: 007a 2b53 6561 7263 682e 7365 6172 6368  .z+Search.search
-00001900: 5f64 6174 615f 7365 7473 2e3c 6c6f 6361  _data_sets.<loca
-00001910: 6c73 3e2e 3c64 6963 7463 6f6d 703e 6301  ls>.<dictcomp>c.
-00001920: 0000 0000 0000 0000 0000 0003 0000 0005  ................
-00001930: 0000 0053 0000 0073 2000 0000 6900 7c00  ...S...s ...i.|.
-00001940: 5d0c 5c02 7d01 7d02 7c01 a000 6400 a101  ].\.}.}.|...d...
-00001950: 7302 7c01 7c02 9302 7102 5300 2901 728b  s.|.|...q.S.).r.
-00001960: 0000 0072 8d00 0000 728f 0000 0072 0f00  ...r....r....r..
-00001970: 0000 720f 0000 0072 1500 0000 7292 0000  ..r....r....r...
-00001980: 00cb 0000 0073 0200 0000 2000 da02 6964  .....s.... ...id
-00001990: 727b 0000 0063 0100 0000 0000 0000 0000  r{...c..........
-000019a0: 0000 0200 0000 0400 0000 5300 0000 731a  ..........S...s.
-000019b0: 0000 0067 007c 005d 097d 017c 016a 0064  ...g.|.].}.|.j.d
-000019c0: 006b 0472 027c 0191 0271 0253 0029 0172  .k.r.|...q.S.).r
-000019d0: 0100 0000 2901 da0a 746f 7461 6c43 6f75  ....)...totalCou
-000019e0: 6e74 a902 7211 0000 00da 0178 720f 0000  nt..r......xr...
-000019f0: 0072 0f00 0000 7215 0000 0072 1600 0000  .r....r....r....
-00001a00: d200 0000 7306 0000 0008 0008 010a ff7a  ....s..........z
-00001a10: 2b53 6561 7263 682e 7365 6172 6368 5f64  +Search.search_d
-00001a20: 6174 615f 7365 7473 2e3c 6c6f 6361 6c73  ata_sets.<locals
-00001a30: 3e2e 3c6c 6973 7463 6f6d 703e 7288 0000  >.<listcomp>r...
-00001a40: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
-00001a50: 0000 0300 0000 5300 0000 727d 0000 0072  ......S...r}...r
-00001a60: 0f00 0000 2901 7281 0000 0072 9500 0000  ....).r....r....
-00001a70: 720f 0000 0072 0f00 0000 7215 0000 0072  r....r....r....r
-00001a80: 1600 0000 db00 0000 7280 0000 0054 2903  ........r....T).
-00001a90: 724e 0000 0072 8100 0000 7282 0000 0072  rN...r....r....r
-00001aa0: 7c00 0000 7217 0000 0029 0272 7200 0000  |...r....).rr...
-00001ab0: 724e 0000 0063 0100 0000 0000 0000 0000  rN...c..........
-00001ac0: 0000 0200 0000 0300 0000 5300 0000 727d  ..........S...r}
-00001ad0: 0000 0072 0f00 0000 727e 0000 0029 0272  ...r....r~...).r
-00001ae0: 1100 0000 7252 0000 0072 0f00 0000 720f  ....rR...r....r.
-00001af0: 0000 0072 1500 0000 7216 0000 00ea 0000  ...r....r.......
-00001b00: 0073 0600 0000 0600 0201 0aff da0a 6461  .s............da
-00001b10: 7461 7365 745f 6964 7a11 4461 7461 2073  taset_idz.Data s
-00001b20: 6574 7320 666f 756e 643a 2072 6200 0000  ets found: rb...
-00001b30: 4672 6300 0000 7265 0000 0072 0100 0000  Frc...re...r....
-00001b40: 7266 0000 0072 0f00 0000 2920 725a 0000  rf...r....) rZ..
-00001b50: 00da 0f66 696c 6573 6572 7669 6365 5f75  ...fileservice_u
-00001b60: 726c 7207 0000 0072 5300 0000 da04 636f  rlr....rS.....co
-00001b70: 7079 da05 6974 656d 7372 6900 0000 7231  py..itemsri...r1
-00001b80: 0000 0072 0300 0000 7287 0000 0072 2100  ...r....r....r!.
-00001b90: 0000 7256 0000 00da 0572 616e 6765 726a  ..rV.....rangerj
-00001ba0: 0000 0072 8100 0000 7288 0000 0072 7300  ...r....r....rs.
-00001bb0: 0000 da1a 5f64 6174 6173 6574 5f6c 6973  ...._dataset_lis
-00001bc0: 745f 666f 725f 7265 7370 6f6e 7365 724e  t_for_responserN
-00001bd0: 0000 0072 3500 0000 7259 0000 0072 2e00  ...r5...rY...r..
-00001be0: 0000 7289 0000 00da 0b67 6574 5f64 6174  ..r......get_dat
-00001bf0: 6173 6574 7279 0000 0072 8300 0000 720a  asetry...r....r.
-00001c00: 0000 0072 0800 0000 726b 0000 0072 6c00  ...r....rk...rl.
-00001c10: 0000 721e 0000 0072 6d00 0000 290e 725e  ..r....rm...).r^
-00001c20: 0000 00da 0c6d 6169 6e5f 6669 6c74 6572  .....main_filter
-00001c30: 73da 0e6f 626a 6563 745f 6669 6c74 6572  s..object_filter
-00001c40: 73da 0f64 6174 6173 6574 5f66 696c 7465  s..dataset_filte
-00001c50: 7273 726e 0000 00da 0864 6174 6173 6574  rsrn.....dataset
-00001c60: 73da 0574 6869 6e67 722b 0000 00da 0169  s..thingr+.....i
-00001c70: da01 6f72 4b00 0000 7228 0000 0072 8500  ..orK...r(...r..
-00001c80: 0000 7286 0000 0072 0f00 0000 720f 0000  ..r....r....r...
-00001c90: 0072 1500 0000 da10 7365 6172 6368 5f64  .r......search_d
-00001ca0: 6174 615f 7365 7473 c300 0000 737c 0000  ata_sets....s|..
-00001cb0: 0016 0104 0102 0106 ff0a 0312 0212 0104  ................
-00001cc0: 0108 010c 0106 0106 0108 0116 0108 020a  ................
-00001cd0: 010a 0112 0118 0108 0104 0102 fe02 8002  ................
-00001ce0: fd0e 060a 0106 0102 0108 fe06 0408 0104  ................
-00001cf0: 010a 0106 010a 010a ff06 0204 0106 0104  ................
-00001d00: fe0a 0306 0102 0204 fe02 0308 fc0a 0612  ................
-00001d10: 010a 0108 ff12 0312 0104 0112 020c 0110  ................
-00001d20: 010e 0114 011e ff02 800e 030c 027a 1753  .............z.S
-00001d30: 6561 7263 682e 7365 6172 6368 5f64 6174  earch.search_dat
-00001d40: 615f 7365 7473 6303 0000 0000 0000 0000  a_setsc.........
-00001d50: 0000 0005 0000 0009 0000 0043 0000 0073  ...........C...s
-00001d60: 9e00 0000 6400 7d03 7c00 6a00 6401 1900  ....d.}.|.j.d...
-00001d70: 6400 7501 721a 7c00 6a00 6402 1900 6400  d.u.r.|.j.d...d.
-00001d80: 7501 721a 7c00 6a00 6401 1900 7c00 6a00  u.r.|.j.d...|.j.
-00001d90: 6402 1900 6901 7d03 7401 7c00 6a00 6403  d...i.}.t.|.j.d.
-00001da0: 1900 7c00 6a00 6404 1900 7c00 6a00 6405  ..|.j.d...|.j.d.
-00001db0: 1900 7c00 6a00 6406 1900 7c03 7c02 7c01  ..|.j.d...|.|.|.
-00001dc0: 6407 8d07 7d04 7c00 6a00 6408 1900 6400  d...}.|.j.d...d.
-00001dd0: 7501 723f 7c00 6a00 6408 1900 7c04 6409  u.r?|.j.d...|.d.
-00001de0: 3c00 7c00 6a00 640a 1900 6400 7501 724d  <.|.j.d...d.u.rM
-00001df0: 7c00 6a00 640a 1900 7c04 640b 3c00 7c04  |.j.d...|.d.<.|.
-00001e00: 5300 290c 4e72 4600 0000 7247 0000 0072  S.).NrF...rG...r
-00001e10: 4200 0000 7244 0000 0072 4500 0000 7243  B...rD...rE...rC
-00001e20: 0000 0029 0772 4200 0000 7244 0000 0072  ...).rB...rD...r
-00001e30: 4500 0000 724d 0000 00da 0577 6865 7265  E...rM.....where
-00001e40: 7272 0000 0072 4e00 0000 7248 0000 0072  rr...rN...rH...r
-00001e50: 5000 0000 7249 0000 0072 5100 0000 2902  P...rI...rQ...).
-00001e60: 7253 0000 00da 0464 6963 7429 0572 5e00  rS.....dict).r^.
-00001e70: 0000 724e 0000 0072 7200 0000 72a6 0000  ..rN...rr...r...
-00001e80: 0072 8600 0000 720f 0000 0072 0f00 0000  .r....r....r....
-00001e90: 7215 0000 0072 8300 0000 0101 0000 7322  r....r........s"
-00001ea0: 0000 0004 011c 0110 0204 ff0a 0408 0108  ................
-00001eb0: 0208 0102 0102 0102 0106 f90e 090e 010e  ................
-00001ec0: 010e 0104 017a 1a53 6561 7263 682e 5f67  .....z.Search._g
-00001ed0: 6574 5f66 696c 7465 7269 6e67 5f61 7267  et_filtering_arg
-00001ee0: 7329 0dda 085f 5f6e 616d 655f 5fda 0a5f  s)...__name__.._
-00001ef0: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-00001f00: 6c6e 616d 655f 5fda 075f 5f64 6f63 5f5f  lname__..__doc__
-00001f10: 725d 0000 0072 6f00 0000 7277 0000 0072  r]...ro...rw...r
-00001f20: 7a00 0000 7269 0000 0072 8900 0000 72a5  z...ri...r....r.
-00001f30: 0000 0072 8300 0000 da0d 5f5f 636c 6173  ...r......__clas
-00001f40: 7363 656c 6c5f 5f72 0f00 0000 720f 0000  scell__r....r...
-00001f50: 0072 6000 0000 7215 0000 0072 5700 0000  .r`...r....rW...
-00001f60: 8000 0000 7314 0000 0008 0004 010c 0408  ....s...........
-00001f70: 0e08 0d08 0308 0308 1a08 0310 3e72 5700  ............>rW.
-00001f80: 0000 2916 da12 636f 6e63 7572 7265 6e74  ..)...concurrent
-00001f90: 2e66 7574 7572 6573 7218 0000 00da 0670  .futuresr......p
-00001fa0: 616e 6461 7372 3900 0000 da1a 7079 6269  andasr9.....pybi
-00001fb0: 732e 7072 6f70 6572 7479 5f72 6566 6f72  s.property_refor
-00001fc0: 6d61 7474 6572 7202 0000 00da 0c70 7962  matterr......pyb
-00001fd0: 6973 2e73 616d 706c 6572 0300 0000 da0f  is.sampler......
-00001fe0: 6f70 656e 6269 735f 636f 6d6d 616e 6472  openbis_commandr
-00001ff0: 0500 0000 da0e 636f 6d6d 616e 645f 7265  ......command_re
-00002000: 7375 6c74 7207 0000 00da 0575 7469 6c73  sultr......utils
-00002010: 7208 0000 00da 1273 6372 6970 7473 2e63  r......scripts.c
-00002020: 6c69 636b 5f75 7469 6c72 0a00 0000 722e  lick_utilr....r.
-00002030: 0000 0072 3100 0000 7235 0000 0072 4100  ...r1...r5...rA.
-00002040: 0000 7256 0000 0072 5700 0000 720f 0000  ..rV...rW...r...
-00002050: 0072 0f00 0000 720f 0000 0072 1500 0000  .r....r....r....
-00002060: da08 3c6d 6f64 756c 653e 0100 0000 731c  ..<module>....s.
-00002070: 0000 0008 0f08 020c 020c 010c 010c 010c  ................
-00002080: 010c 0108 0308 1e08 0908 0708 0f14 27    ..............'
+00000040: 6402 6c04 6d05 5a05 0100 6403 6404 6c06  d.l.m.Z...d.d.l.
+00000050: 6d07 5a07 0100 6405 6406 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
+00000060: 0100 6405 6407 6c0a 6d0b 5a0b 0100 6408  ..d.d.l.m.Z...d.
+00000070: 6409 6c0c 6d0d 5a0d 0100 640a 640b 8400  d.l.m.Z...d.d...
+00000080: 5a0e 640c 640d 8400 5a0f 640e 640f 8400  Z.d.d...Z.d.d...
+00000090: 5a10 6410 6411 8400 5a11 6412 6413 8400  Z.d.d...Z.d.d...
+000000a0: 5a12 6414 6415 8400 5a13 4700 6416 6417  Z.d.d...Z.G.d.d.
+000000b0: 8400 6417 6507 8303 5a14 6401 5300 2918  ..d.e...Z.d.S.).
+000000c0: e900 0000 004e 2901 da23 6973 5f6f 665f  .....N)..#is_of_
+000000d0: 6f70 656e 6269 735f 7375 7070 6f72 7465  openbis_supporte
+000000e0: 645f 6461 7465 5f66 6f72 6d61 74e9 0100  d_date_format...
+000000f0: 0000 2901 da0e 4f70 656e 6269 7343 6f6d  ..)...OpenbisCom
+00000100: 6d61 6e64 e902 0000 0029 01da 0d43 6f6d  mand.....)...Com
+00000110: 6d61 6e64 5265 7375 6c74 2901 da02 6364  mandResult)...cd
+00000120: e903 0000 0029 01da 0a63 6c69 636b 5f65  .....)...click_e
+00000130: 6368 6f63 0400 0000 0000 0000 0000 0000  choc............
+00000140: 0f00 0000 0900 0000 0300 0000 7330 0100  ............s0..
+00000150: 0074 006a 016a 0264 0164 028d 018f 877d  .t.j.j.d.d.....}
+00000160: 0474 006a 016a 0264 0364 028d 018f 677d  .t.j.j.d.d....g}
+00000170: 0587 0066 0164 0464 0584 087c 0044 0083  ...f.d.d...|.D..
+00000180: 017d 0674 0383 007d 077c 06a0 04a1 0001  .}.t...}.|......
+00000190: 0067 007d 087c 0672 6f7c 04a0 057c 027c  .g.}.|.ro|...|.|
+000001a0: 06a1 027d 0967 007d 0667 007d 0a67 007d  ...}.g.}.g.}.g.}
+000001b0: 0b7c 0944 005d 227d 0c7c 0c6a 0688 0019  .|.D.]"}.|.j....
+000001c0: 0064 0619 007d 0d7c 0a74 077c 0c6a 0664  .d...}.|.t.|.j.d
+000001d0: 0719 0083 0164 0619 0037 007d 0a7c 0d7c  .....d...7.}.|.|
+000001e0: 0776 0172 547c 07a0 087c 0da1 0101 007c  .v.rT|...|.....|
+000001f0: 0b7c 0d67 0137 007d 0b71 327c 0b72 5f7c  .|.g.7.}.q2|.r_|
+00000200: 087c 05a0 057c 037c 0ba1 0237 007d 087c  .|...|.|...7.}.|
+00000210: 0a44 005d 0b7d 0e7c 0e7c 0776 0172 6c7c  .D.].}.|.|.v.rl|
+00000220: 067c 0e67 0137 007d 0671 617c 0673 2457  .|.g.7.}.qa|.s$W
+00000230: 0064 0804 0004 0083 0301 006e 1031 0073  .d.........n.1.s
+00000240: 7977 0101 0001 0001 0059 0001 0057 0064  yw.......Y...W.d
+00000250: 0804 0004 0083 0301 007c 0853 0057 0064  .........|.S.W.d
+00000260: 0804 0004 0083 0301 007c 0853 0031 0073  .........|.S.1.s
+00000270: 9177 0101 0001 0001 0059 0001 007c 0853  .w.......Y...|.S
+00000280: 0029 09fa 4648 656c 7065 7220 6675 6e63  .)..FHelper func
+00000290: 7469 6f6e 2074 6861 7420 7065 7266 6f72  tion that perfor
+000002a0: 6d20 4446 5320 7365 6172 6368 206f 7665  m DFS search ove
+000002b0: 7220 6368 696c 6472 656e 2067 7261 7068  r children graph
+000002c0: 206f 6620 6f62 6a65 6374 73e9 0500 0000   of objects.....
+000002d0: a901 da0b 6d61 785f 776f 726b 6572 73e9  ....max_workers.
+000002e0: 1400 0000 6301 0000 0000 0000 0000 0000  ....c...........
+000002f0: 0002 0000 0004 0000 0013 0000 0073 1400  .............s..
+00000300: 0000 6700 7c00 5d06 7d01 7c01 8800 1900  ..g.|.].}.|.....
+00000310: 9102 7102 5300 a900 720f 0000 0029 02da  ..q.S...r....)..
+00000320: 022e 30da 0b6f 7065 6e62 6973 5f6f 626a  ..0..openbis_obj
+00000330: a901 da04 7072 6f70 720f 0000 00fa 632f  ....propr.....c/
+00000340: 686f 6d65 2f61 6c61 736b 6f77 736b 692f  home/alaskowski/
+00000350: 7265 706f 2f6f 7065 6e62 6973 5f70 7974  repo/openbis_pyt
+00000360: 686f 6e2f 6170 702d 6f70 656e 6269 732d  hon/app-openbis-
+00000370: 636f 6d6d 616e 642d 6c69 6e65 2f73 7263  command-line/src
+00000380: 2f70 7974 686f 6e2f 6f62 6973 2f64 6d2f  /python/obis/dm/
+00000390: 636f 6d6d 616e 6473 2f73 6561 7263 682e  commands/search.
+000003a0: 7079 da0a 3c6c 6973 7463 6f6d 703e 2100  py..<listcomp>!.
+000003b0: 0000 f302 0000 0014 007a 185f 6466 732e  .........z._dfs.
+000003c0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
+000003d0: 6d70 3e72 0100 0000 da08 6368 696c 6472  mp>r......childr
+000003e0: 656e 4e29 09da 0a63 6f6e 6375 7272 656e  enN)...concurren
+000003f0: 74da 0766 7574 7572 6573 da12 5468 7265  t..futures..Thre
+00000400: 6164 506f 6f6c 4578 6563 7574 6f72 da03  adPoolExecutor..
+00000410: 7365 74da 0772 6576 6572 7365 da03 6d61  set..reverse..ma
+00000420: 70da 0264 66da 046c 6973 74da 0361 6464  p..df..list..add
+00000430: 290f da07 6f62 6a65 6374 7372 1300 0000  )...objectsr....
+00000440: da04 6675 6e63 da0d 6675 6e63 5f73 7065  ..func..func_spe
+00000450: 6369 6669 63da 0b70 6f6f 6c5f 7369 6d70  cific..pool_simp
+00000460: 6c65 da09 706f 6f6c 5f66 756c 6cda 0573  le..pool_full..s
+00000470: 7461 636b da07 7669 7369 7465 64da 066f  tack..visited..o
+00000480: 7574 7075 74da 0e73 696d 706c 655f 7265  utput..simple_re
+00000490: 7375 6c74 7372 1700 0000 da0d 6675 6c6c  sultsr......full
+000004a0: 5f64 6f77 6e6c 6f61 64da 036f 626a da03  _download..obj..
+000004b0: 6b65 79da 0563 6869 6c64 720f 0000 0072  key..childr....r
+000004c0: 1200 0000 7214 0000 00da 045f 6466 731b  ....r......_dfs.
+000004d0: 0000 0073 5000 0000 0602 0201 06ff 0801  ...sP...........
+000004e0: 0201 04ff 02ff 0202 0a02 0201 06ff 0602  ................
+000004f0: 0801 0401 0401 0c01 0401 0401 0401 0801  ................
+00000500: 0e01 1601 0801 0a01 0a01 0280 0401 1001  ................
+00000510: 0801 0801 0a01 0280 04f1 0280 28f7 041a  ............(...
+00000520: 0ce6 041a 10e6 041a 722e 0000 0063 0300  ........r....c..
+00000530: 0000 0000 0000 0000 0000 0b00 0000 0500  ................
+00000540: 0000 0300 0000 73cc 0000 007c 007d 0364  ......s....|.}.d
+00000550: 0164 0284 007c 0044 0083 017d 0487 0066  .d...|.D...}...f
+00000560: 0164 0364 0284 0874 007c 0483 0144 0083  .d.d...t.|...D..
+00000570: 017d 0474 0187 0066 0164 0464 0284 087c  .}.t...f.d.d...|
+00000580: 0044 0083 0183 017d 057c 0472 647c 027c  .D.....}.|.rd|.|
+00000590: 0483 017d 0674 027c 06a0 03a1 0083 017d  ...}.t.|.......}
+000005a0: 067c 037c 0637 007d 0367 007d 0467 007d  .|.|.7.}.g.}.g.}
+000005b0: 077c 0644 005d 1e7d 087c 0888 0019 0088  .|.D.].}.|......
+000005c0: 0019 007d 097c 0787 0066 0164 0564 0284  ...}.|...f.d.d..
+000005d0: 087c 0864 0619 0044 0083 0137 007d 077c  .|.d...D...7.}.|
+000005e0: 097c 0576 0172 537c 05a0 047c 09a1 0101  .|.v.rS|...|....
+000005f0: 0071 357c 0744 005d 0b7d 0a7c 0a7c 0576  .q5|.D.].}.|.|.v
+00000600: 0172 617c 047c 0a67 0137 007d 0471 567c  .ra|.|.g.7.}.qV|
+00000610: 0473 217c 0353 0029 0772 0a00 0000 6301  .s!|.S.).r....c.
+00000620: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00000630: 0000 0053 0000 0073 1c00 0000 6700 7c00  ...S...s....g.|.
+00000640: 5d0a 7d01 7c01 6400 1900 7202 7c01 6400  ].}.|.d...r.|.d.
+00000650: 1900 9102 7102 5300 2901 7217 0000 0072  ....q.S.).r....r
+00000660: 0f00 0000 a902 7210 0000 00da 0178 720f  ......r......xr.
+00000670: 0000 0072 0f00 0000 7214 0000 0072 1500  ...r....r....r..
+00000680: 0000 3d00 0000 7302 0000 001c 007a 205f  ..=...s......z _
+00000690: 6466 735f 7361 6d70 6c65 732e 3c6c 6f63  dfs_samples.<loc
+000006a0: 616c 733e 2e3c 6c69 7374 636f 6d70 3e63  als>.<listcomp>c
+000006b0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+000006c0: 0400 0000 1300 0000 f318 0000 0067 007c  .............g.|
+000006d0: 005d 087d 017c 0188 0019 0088 0019 0091  .].}.|..........
+000006e0: 0271 0253 0072 0f00 0000 720f 0000 0072  .q.S.r....r....r
+000006f0: 2f00 0000 7212 0000 0072 0f00 0000 7214  /...r....r....r.
+00000700: 0000 0072 1500 0000 3e00 0000 f302 0000  ...r....>.......
+00000710: 0018 0063 0100 0000 0000 0000 0000 0000  ...c............
+00000720: 0200 0000 0400 0000 1300 0000 7231 0000  ............r1..
+00000730: 0072 0f00 0000 720f 0000 0072 2f00 0000  .r....r....r/...
+00000740: 7212 0000 0072 0f00 0000 7214 0000 0072  r....r....r....r
+00000750: 1500 0000 3f00 0000 7232 0000 0063 0100  ....?...r2...c..
+00000760: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+00000770: 0000 1300 0000 7231 0000 0072 0f00 0000  ......r1...r....
+00000780: 720f 0000 0072 2f00 0000 7212 0000 0072  r....r/...r....r
+00000790: 0f00 0000 7214 0000 0072 1500 0000 4900  ....r....r....I.
+000007a0: 0000 7232 0000 0072 1700 0000 2905 da07  ..r2...r....)...
+000007b0: 666c 6174 7465 6e72 1b00 0000 721f 0000  flattenr....r...
+000007c0: 00da 0676 616c 7565 7372 2000 0000 290b  ...valuesr ...).
+000007d0: da09 6461 7461 5f62 6173 6572 1300 0000  ..data_baser....
+000007e0: 7222 0000 0072 2800 0000 da03 6964 7372  r"...r(.....idsr
+000007f0: 2700 0000 da04 6461 7461 7217 0000 0072  '.....datar....r
+00000800: 2b00 0000 722c 0000 0072 2d00 0000 720f  +...r,...r-...r.
+00000810: 0000 0072 1200 0000 7214 0000 00da 0c5f  ...r....r......_
+00000820: 6466 735f 7361 6d70 6c65 733a 0000 0073  dfs_samples:...s
+00000830: 2c00 0000 0402 0e01 1601 1601 0401 0801  ,...............
+00000840: 0c01 0801 0401 0401 0801 0c01 1a02 0801  ................
+00000850: 0a01 0280 0801 0801 0a01 0280 04f2 040f  ................
+00000860: 7238 0000 0063 0200 0000 0000 0000 0000  r8...c..........
+00000870: 0000 0400 0000 0800 0000 4300 0000 7344  ..........C...sD
+00000880: 0000 0067 007d 0274 006a 016a 0264 0164  ...g.}.t.j.j.d.d
+00000890: 028d 018f 0f7d 037c 03a0 037c 007c 01a1  .....}.|...|.|..
+000008a0: 027d 0257 0064 0004 0004 0083 0301 007c  .}.W.d.........|
+000008b0: 0253 0031 0073 1b77 0101 0001 0001 0059  .S.1.s.w.......Y
+000008c0: 0001 007c 0253 0029 034e 720b 0000 0072  ...|.S.).Nr....r
+000008d0: 0c00 0000 2904 7218 0000 0072 1900 0000  ....).r....r....
+000008e0: 721a 0000 0072 1d00 0000 2904 da12 6765  r....r....)...ge
+000008f0: 745f 6461 7461 7365 745f 6d65 7468 6f64  t_dataset_method
+00000900: da07 7361 6d70 6c65 7372 2800 0000 7224  ..samplesr(...r$
+00000910: 0000 0072 0f00 0000 720f 0000 0072 1400  ...r....r....r..
+00000920: 0000 da18 5f67 6574 5f64 6174 6173 6574  ...._get_dataset
+00000930: 735f 6f66 5f73 616d 706c 6573 6e00 0000  s_of_samplesn...
+00000940: 7314 0000 0004 0106 0102 0106 ff02 010e  s...............
+00000950: 010a fe04 0410 fc04 0472 3b00 0000 6301  .........r;...c.
+00000960: 0000 0000 0000 0000 0000 0003 0000 0003  ................
+00000970: 0000 0043 0000 0073 1a00 0000 6700 7d01  ...C...s....g.}.
+00000980: 7c00 4400 5d06 7d02 7c01 7c02 3700 7d01  |.D.].}.|.|.7.}.
+00000990: 7104 7c01 5300 2901 4e72 0f00 0000 2903  q.|.S.).Nr....).
+000009a0: da06 6d61 7472 6978 da09 666c 6174 5f6c  ..matrix..flat_l
+000009b0: 6973 74da 0372 6f77 720f 0000 0072 0f00  ist..rowr....r..
+000009c0: 0000 7214 0000 0072 3300 0000 7700 0000  ..r....r3...w...
+000009d0: 7308 0000 0004 0108 010a 0104 0172 3300  s............r3.
+000009e0: 0000 6303 0000 0000 0000 0000 0000 0005  ..c.............
+000009f0: 0000 0003 0000 0043 0000 0073 6a00 0000  .......C...sj...
+00000a00: 7400 7c01 8301 7231 7400 7c02 8301 7231  t.|...r1t.|...r1
+00000a10: 7401 a002 7c01 a101 7d03 7401 a002 7c02  t...|...}.t...|.
+00000a20: a101 7d04 7c00 6401 6b02 721a 7c04 7c03  ..}.|.d.k.r.|.|.
+00000a30: 6b02 5300 7c00 6402 6b02 7222 7c04 7c03  k.S.|.d.k.r"|.|.
+00000a40: 6b04 5300 7c00 6403 6b02 722a 7c04 7c03  k.S.|.d.k.r*|.|.
+00000a50: 6b00 5300 7403 6404 7c00 9b00 9d02 8301  k.S.t.d.|.......
+00000a60: 8201 7403 6405 8301 8201 2906 4efa 013d  ..t.d.....).N..=
+00000a70: fa01 3efa 013c 7a0d 556e 6b6e 6f77 6e20  ..>..<z.Unknown 
+00000a80: 7369 676e 207a 2544 6174 6573 2061 7265  sign z%Dates are
+00000a90: 206e 6f74 2069 6e20 6120 7375 7070 6f72   not in a suppor
+00000aa0: 7465 6420 666f 726d 6174 7321 2904 7202  ted formats!).r.
+00000ab0: 0000 00da 0270 64da 0b74 6f5f 6461 7465  .....pd..to_date
+00000ac0: 7469 6d65 da0a 5661 6c75 6545 7272 6f72  time..ValueError
+00000ad0: 2905 da04 7369 676e da05 6461 7465 31da  )...sign..date1.
+00000ae0: 0564 6174 6532 da0a 7469 6d65 7374 616d  .date2..timestam
+00000af0: 7031 da0a 7469 6d65 7374 616d 7032 720f  p1..timestamp2r.
+00000b00: 0000 0072 0f00 0000 7214 0000 00da 0b5f  ...r....r......_
+00000b10: 6368 6563 6b5f 6461 7465 7e00 0000 7316  check_date~...s.
+00000b20: 0000 0010 010a 010a 0108 0108 0108 0108  ................
+00000b30: 0108 0108 010e 0108 0272 4a00 0000 6302  .........rJ...c.
+00000b40: 0000 0000 0000 0000 0000 0009 0000 0004  ................
+00000b50: 0000 0043 0000 0073 d001 0000 7c01 a000  ...C...s....|...
+00000b60: 6401 6400 a102 6400 7501 7229 7c01 6401  d.d...d.u.r)|.d.
+00000b70: 1900 7d02 7c00 6a01 6400 7501 721a 7c00  ..}.|.j.d.u.r.|.
+00000b80: 6a01 6a02 6a03 7c02 6b03 721a 6402 5300  j.j.j.|.k.r.d.S.
+00000b90: 7c00 6a04 6400 7501 7229 7c00 6a04 6a05  |.j.d.u.r)|.j.j.
+00000ba0: 6a02 6a03 7c02 6b03 7229 6402 5300 7c01  j.j.|.k.r)d.S.|.
+00000bb0: a000 6403 6400 a102 6400 7501 723b 7c00  ..d.d...d.u.r;|.
+00000bc0: 6a06 6a03 7c01 6403 1900 6b03 723b 6402  j.j.|.d...k.r;d.
+00000bd0: 5300 7c01 a000 6404 6400 a102 6400 7501  S.|...d.d...d.u.
+00000be0: 7263 7c01 6404 1900 7d03 7c00 6a01 6400  rc|.d...}.|.j.d.
+00000bf0: 7501 7255 7c00 6a01 6a05 6a03 7c03 6b03  u.rU|.j.j.j.|.k.
+00000c00: 7255 6402 5300 7c00 6a04 6400 7501 7263  rUd.S.|.j.d.u.rc
+00000c10: 7c00 6a04 6a05 6a03 7c03 6b03 7263 6402  |.j.j.j.|.k.rcd.
+00000c20: 5300 7c01 a000 6405 6400 a102 6400 7501  S.|...d.d...d.u.
+00000c30: 727a 7c00 6a04 6400 7501 727a 7c00 6a04  rz|.j.d.u.rz|.j.
+00000c40: 6a03 7c01 6405 1900 6b03 727a 6402 5300  j.|.d...k.rzd.S.
+00000c50: 7c01 a000 6406 6400 a102 6400 7501 729a  |...d.d...d.u.r.
+00000c60: 7c01 6406 1900 7d04 7c01 6407 1900 7d05  |.d...}.|.d...}.
+00000c70: 7c00 6a07 6400 7501 729a 7c00 6a07 7c04  |.j.d.u.r.|.j.|.
+00000c80: a008 a100 1900 7c05 6b03 729a 6402 5300  ......|.k.r.d.S.
+00000c90: 7c01 a000 6408 6400 a102 6400 7501 72c0  |...d.d...d.u.r.
+00000ca0: 7c01 6408 1900 7d06 6409 7d07 7c06 640a  |.d...}.d.}.|.d.
+00000cb0: 1900 640b 7600 72b9 7c06 640a 1900 7c06  ..d.v.r.|.d...|.
+00000cc0: 640c 6400 8502 1900 0202 7d07 7d06 7409  d.d.......}.}.t.
+00000cd0: 7c07 7c06 7c00 6a0a 8303 5300 7c01 a000  |.|.|.j...S.|...
+00000ce0: 640d 6400 a102 6400 7501 72e6 7c01 640d  d.d...d.u.r.|.d.
+00000cf0: 1900 7d08 6409 7d07 7c08 640a 1900 640b  ..}.d.}.|.d...d.
+00000d00: 7600 72df 7c08 640a 1900 7c08 640c 6400  v.r.|.d...|.d.d.
+00000d10: 8502 1900 0202 7d07 7d08 7409 7c07 7c08  ......}.}.t.|.|.
+00000d20: 7c00 6a0b 8303 5300 640e 5300 290f 4eda  |.j...S.d.S.).N.
+00000d30: 0573 7061 6365 46da 0974 7970 655f 636f  .spaceF..type_co
+00000d40: 6465 da07 7072 6f6a 6563 74da 0a65 7870  de..project..exp
+00000d50: 6572 696d 656e 74da 0d70 726f 7065 7274  eriment..propert
+00000d60: 795f 636f 6465 da0e 7072 6f70 6572 7479  y_code..property
+00000d70: 5f76 616c 7565 da11 7265 6769 7374 7261  _value..registra
+00000d80: 7469 6f6e 5f64 6174 6572 3f00 0000 7201  tion_dater?...r.
+00000d90: 0000 0029 0372 4000 0000 7241 0000 0072  ...).r@...rA...r
+00000da0: 3f00 0000 7203 0000 00da 116d 6f64 6966  ?...r......modif
+00000db0: 6963 6174 696f 6e5f 6461 7465 5429 0cda  ication_dateT)..
+00000dc0: 0367 6574 da06 7361 6d70 6c65 724b 0000  .get..samplerK..
+00000dd0: 00da 0463 6f64 6572 4e00 0000 724d 0000  ...coderN...rM..
+00000de0: 00da 0474 7970 65da 0570 726f 7073 da05  ...type..props..
+00000df0: 6c6f 7765 7272 4a00 0000 da10 7265 6769  lowerrJ.....regi
+00000e00: 7374 7261 7469 6f6e 4461 7465 da10 6d6f  strationDate..mo
+00000e10: 6469 6669 6361 7469 6f6e 4461 7465 2909  dificationDate).
+00000e20: da07 6461 7461 7365 74da 0766 696c 7465  ..dataset..filte
+00000e30: 7273 724b 0000 0072 4d00 0000 da09 7072  rsrK...rM.....pr
+00000e40: 6f70 5f63 6f64 65da 0a70 726f 705f 7661  op_code..prop_va
+00000e50: 6c75 6572 5100 0000 7245 0000 0072 5200  luerQ...rE...rR.
+00000e60: 0000 720f 0000 0072 0f00 0000 7214 0000  ..r....r....r...
+00000e70: 00da 0f5f 6669 6c74 6572 5f64 6174 6173  ..._filter_datas
+00000e80: 6574 8d00 0000 7348 0000 0010 0108 0118  et....sH........
+00000e90: 0104 011a 0104 0110 0110 0104 0110 0108  ................
+00000ea0: 0118 0104 0118 0104 0110 011a 0104 0110  ................
+00000eb0: 0108 0108 011c 0104 0110 0108 0104 010c  ................
+00000ec0: 0116 010e 0110 0108 0104 010c 0116 010e  ................
+00000ed0: 0104 0172 5f00 0000 6300 0000 0000 0000  ...r_...c.......
+00000ee0: 0000 0000 0000 0000 0003 0000 0000 0000  ................
+00000ef0: 0073 6200 0000 6500 5a01 6400 5a02 6401  .sb...e.Z.d.Z.d.
+00000f00: 5a03 8700 6601 6402 6403 8408 5a04 6404  Z...f.d.d...Z.d.
+00000f10: 6405 8400 5a05 6406 6407 8400 5a06 6408  d...Z.d.d...Z.d.
+00000f20: 6409 8400 5a07 640a 640b 8400 5a08 6415  d...Z.d.d...Z.d.
+00000f30: 640d 640e 8401 5a09 640f 6410 8400 5a0a  d.d...Z.d.d...Z.
+00000f40: 6411 6412 8400 5a0b 6413 6414 8400 5a0c  d.d...Z.d.d...Z.
+00000f50: 8700 0400 5a0d 5300 2916 da06 5365 6172  ....Z.S.)...Sear
+00000f60: 6368 7a3b 0a20 2020 2043 6f6d 6d61 6e64  chz;.    Command
+00000f70: 2074 6f20 7365 6172 6368 2073 616d 706c   to search sampl
+00000f80: 6573 206f 7220 6461 7461 7365 7473 2069  es or datasets i
+00000f90: 6e20 6f70 656e 4249 532e 0a20 2020 2063  n openBIS..    c
+00000fa0: 0500 0000 0000 0000 0000 0000 0500 0000  ................
+00000fb0: 0300 0000 0300 0000 7336 0000 007c 027c  ........s6...|.|
+00000fc0: 005f 007c 037c 005f 017c 047c 005f 027c  ._.|.|._.|.|._.|
+00000fd0: 00a0 037c 01a1 0101 0064 017c 005f 0474  ...|.....d.|._.t
+00000fe0: 0574 067c 0083 02a0 077c 01a1 0101 0064  .t.|.....|.....d
+00000ff0: 0253 0029 0361 1001 0000 0a20 2020 2020  .S.).a.....     
+00001000: 2020 203a 7061 7261 6d20 646d 3a20 6461     :param dm: da
+00001010: 7461 206d 616e 6167 656d 656e 740a 2020  ta management.  
+00001020: 2020 2020 2020 3a70 6172 616d 2066 696c        :param fil
+00001030: 7465 7273 3a20 4469 6374 696f 6e61 7279  ters: Dictionary
+00001040: 206f 6620 6669 6c74 6572 2074 6f20 6265   of filter to be
+00001050: 2075 7365 6420 6475 7269 6e67 2073 6561   used during sea
+00001060: 7263 680a 2020 2020 2020 2020 3a70 6172  rch.        :par
+00001070: 616d 2072 6563 7572 7369 7665 3a20 466c  am recursive: Fl
+00001080: 6167 2069 6e64 6963 6174 696e 6720 7265  ag indicating re
+00001090: 6375 7273 6976 6520 7365 6172 6368 2069  cursive search i
+000010a0: 6e20 6368 696c 6472 656e 0a20 2020 2020  n children.     
+000010b0: 2020 203a 7061 7261 6d20 7361 7665 5f70     :param save_p
+000010c0: 6174 683a 2050 6174 6820 746f 2073 6176  ath: Path to sav
+000010d0: 6520 7265 7375 6c74 732e 2049 6620 6e6f  e results. If no
+000010e0: 7420 7365 742c 2072 6573 756c 7473 2077  t set, results w
+000010f0: 696c 6c20 6e6f 7420 6265 2073 6176 6564  ill not be saved
+00001100: 2e0a 2020 2020 2020 2020 da01 2a4e 2908  ..        ..*N).
+00001110: 725c 0000 00da 0972 6563 7572 7369 7665  r\.....recursive
+00001120: da09 7361 7665 5f70 6174 68da 126c 6f61  ..save_path..loa
+00001130: 645f 676c 6f62 616c 5f63 6f6e 6669 6772  d_global_configr
+00001140: 5700 0000 da05 7375 7065 7272 6000 0000  W.....superr`...
+00001150: da08 5f5f 696e 6974 5f5f 2905 da04 7365  ..__init__)...se
+00001160: 6c66 da02 646d 725c 0000 0072 6200 0000  lf..dmr\...rb...
+00001170: 7263 0000 00a9 01da 095f 5f63 6c61 7373  rc.......__class
+00001180: 5f5f 720f 0000 0072 1400 0000 7266 0000  __r....r....rf..
+00001190: 00b9 0000 0073 0c00 0000 0607 0601 0601  .....s..........
+000011a0: 0a01 0601 1401 7a0f 5365 6172 6368 2e5f  ......z.Search._
+000011b0: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
+000011c0: 0000 0000 0200 0000 0800 0000 4300 0000  ............C...
+000011d0: 73ac 0000 007c 006a 0064 0164 028d 017d  s....|.j.d.d...}
+000011e0: 017c 006a 016a 027c 006a 037c 0167 0064  .|.j.j.|.j.|.g.d
+000011f0: 03a2 0164 0164 048d 047d 0174 0464 0574  ...d.d...}.t.d.t
+00001200: 057c 0183 019b 009d 0283 0101 007c 006a  .|...........|.j
+00001210: 0664 0075 0172 4974 0464 067c 006a 069b  .d.u.rIt.d.|.j..
+00001220: 009d 0283 0101 0074 077c 006a 086a 0983  .......t.|.j.j..
+00001230: 018f 1101 007c 016a 0a6a 0b7c 006a 0664  .....|.j.j.|.j.d
+00001240: 0764 088d 0201 0057 0064 0004 0004 0083  .d.....W.d......
+00001250: 0301 006e 0831 0073 4377 0101 0001 0001  ...n.1.sCw......
+00001260: 0059 0001 006e 0774 0464 097c 019b 009d  .Y...n.t.d.|....
+00001270: 0283 0101 0074 0c64 0a64 0b64 0c8d 0253  .....t.d.d.d...S
+00001280: 0029 0d4e 54a9 01da 0c72 6177 5f72 6573  .).NT....raw_res
+00001290: 706f 6e73 65a9 03da 0770 6172 656e 7473  ponse....parents
+000012a0: 7217 0000 00da 0864 6174 6153 6574 7329  r......dataSets)
+000012b0: 0472 5700 0000 da08 7265 7370 6f6e 7365  .rW.....response
+000012c0: da05 6174 7472 73da 0670 6172 7365 647a  ..attrs..parsedz
+000012d0: 0f4f 626a 6563 7473 2066 6f75 6e64 3a20  .Objects found: 
+000012e0: fa19 5361 7669 6e67 2073 6561 7263 6820  ..Saving search 
+000012f0: 7265 7375 6c74 7320 696e 2046 a901 da05  results in F....
+00001300: 696e 6465 78fa 1053 6561 7263 6820 7265  index..Search re
+00001310: 7375 6c74 733a 0a72 0100 0000 fa11 5365  sults:.r......Se
+00001320: 6172 6368 2063 6f6d 706c 6574 6564 2ea9  arch completed..
+00001330: 02da 0a72 6574 7572 6e63 6f64 6572 2800  ...returncoder(.
+00001340: 0000 290d da0f 5f73 6561 7263 685f 7361  ..)..._search_sa
+00001350: 6d70 6c65 73da 076f 7065 6e62 6973 da19  mples..openbis..
+00001360: 5f73 616d 706c 655f 6c69 7374 5f66 6f72  _sample_list_for
+00001370: 5f72 6573 706f 6e73 6572 5700 0000 7209  _responserW...r.
+00001380: 0000 00da 036c 656e 7263 0000 0072 0700  .....lenrc...r..
+00001390: 0000 da09 6461 7461 5f6d 676d 74da 0f69  ....data_mgmt..i
+000013a0: 6e76 6f63 6174 696f 6e5f 7061 7468 721e  nvocation_pathr.
+000013b0: 0000 00da 0674 6f5f 6373 7672 0600 0000  .....to_csvr....
+000013c0: 2902 7267 0000 00da 0e73 6561 7263 685f  ).rg.....search_
+000013d0: 7265 7375 6c74 7372 0f00 0000 720f 0000  resultsr....r...
+000013e0: 0072 1400 0000 da0e 7365 6172 6368 5f73  .r......search_s
+000013f0: 616d 706c 6573 c700 0000 731e 0000 000c  amples....s.....
+00001400: 010a 0202 0106 0102 0206 fc12 060a 0110  ................
+00001410: 010e 0114 011c ff02 800e 030c 027a 1553  .............z.S
+00001420: 6561 7263 682e 7365 6172 6368 5f73 616d  earch.search_sam
+00001430: 706c 6573 6302 0000 0000 0000 0000 0000  plesc...........
+00001440: 0002 0000 0004 0000 0043 0000 0073 1400  .........C...s..
+00001450: 0000 7c00 6a00 6a01 7c01 6401 6402 6702  ..|.j.j.|.d.d.g.
+00001460: 6403 8d02 5300 2904 4e72 1700 0000 726f  d...S.).Nr....ro
+00001470: 0000 00a9 0172 7100 0000 2902 727b 0000  .....rq...).r{..
+00001480: 00da 0b67 6574 5f73 616d 706c 6573 a902  ...get_samples..
+00001490: 7267 0000 00da 0a69 6465 6e74 6966 6965  rg.....identifie
+000014a0: 7272 0f00 0000 720f 0000 0072 1400 0000  rr....r....r....
+000014b0: da15 5f67 6574 5f73 616d 706c 6573 5f63  .._get_samples_c
+000014c0: 6869 6c64 7265 6eda 0000 0073 0200 0000  hildren....s....
+000014d0: 1401 7a1c 5365 6172 6368 2e5f 6765 745f  ..z.Search._get_
+000014e0: 7361 6d70 6c65 735f 6368 696c 6472 656e  samples_children
+000014f0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00001500: 0004 0000 0043 0000 0073 1000 0000 7c00  .....C...s....|.
+00001510: 6a00 6a01 7c01 6401 6402 8d02 5300 2903  j.j.|.d.d...S.).
+00001520: 4e54 2901 da0e 7769 7468 4461 7461 5365  NT)...withDataSe
+00001530: 7449 6473 a902 727b 0000 00da 0a67 6574  tIds..r{.....get
+00001540: 5f73 616d 706c 6572 8500 0000 720f 0000  _sampler....r...
+00001550: 0072 0f00 0000 7214 0000 00da 195f 6765  .r....r......_ge
+00001560: 745f 7361 6d70 6c65 5f77 6974 685f 6461  t_sample_with_da
+00001570: 7461 7365 7473 dd00 0000 7302 0000 0010  tasets....s.....
+00001580: 017a 2053 6561 7263 682e 5f67 6574 5f73  .z Search._get_s
+00001590: 616d 706c 655f 7769 7468 5f64 6174 6173  ample_with_datas
+000015a0: 6574 7363 0200 0000 0000 0000 0000 0000  etsc............
+000015b0: 0200 0000 0500 0000 4300 0000 7312 0000  ........C...s...
+000015c0: 007c 006a 006a 017c 0164 0164 0164 028d  .|.j.j.|.d.d.d..
+000015d0: 0353 0029 034e 5429 0272 8800 0000 726c  .S.).NT).r....rl
+000015e0: 0000 0072 8900 0000 7285 0000 0072 0f00  ...r....r....r..
+000015f0: 0000 720f 0000 0072 1400 0000 da1a 5f67  ..r....r......_g
+00001600: 6574 5f73 616d 706c 655f 7769 7468 5f64  et_sample_with_d
+00001610: 6174 6173 6574 7332 e000 0000 f302 0000  atasets2........
+00001620: 0012 017a 2153 6561 7263 682e 5f67 6574  ...z!Search._get
+00001630: 5f73 616d 706c 655f 7769 7468 5f64 6174  _sample_with_dat
+00001640: 6173 6574 7332 4663 0200 0000 0000 0000  asets2Fc........
+00001650: 0000 0000 0600 0000 0600 0000 4300 0000  ............C...
+00001660: 73a2 0000 007c 006a 0072 0564 017d 0164  s....|.j.r.d.}.d
+00001670: 027c 006a 0176 0072 1b7c 006a 026a 037c  .|.j.v.r.|.j.j.|
+00001680: 006a 0164 0219 0067 0064 03a2 017c 017c  .j.d...g.d...|.|
+00001690: 006a 0464 048d 047d 026e 167c 00a0 057c  .j.d...}.n.|...|
+000016a0: 006a 0467 0064 03a2 01a1 027d 037c 017c  .j.g.d.....}.|.|
+000016b0: 0364 053c 007c 006a 026a 0364 0a69 007c  .d.<.|.j.j.d.i.|
+000016c0: 03a4 018e 017d 027c 006a 0072 4574 0664  .....}.|.j.rEt.d
+000016d0: 0683 0101 0074 077c 0264 0719 0064 087c  .....t.|.d...d.|
+000016e0: 006a 0883 037d 047c 047d 057c 0553 007c  .j...}.|.}.|.S.|
+000016f0: 0172 4d7c 0264 0719 007d 057c 0553 007c  .rM|.d...}.|.S.|
+00001700: 027d 057c 0553 0029 0b7a 1f48 656c 7065  .}.|.S.).z.Helpe
+00001710: 7220 6d65 7468 6f64 2074 6f20 7365 6172  r method to sear
+00001720: 6368 2073 616d 706c 6573 54da 0b6f 626a  ch samplesT..obj
+00001730: 6563 745f 636f 6465 726d 0000 0029 0472  ect_coderm...).r
+00001740: 8600 0000 7271 0000 0072 6c00 0000 7257  ....rq...rl...rW
+00001750: 0000 0072 6c00 0000 7a3e 5265 6375 7273  ...rl...z>Recurs
+00001760: 6976 6520 7365 6172 6368 2065 6e61 626c  ive search enabl
+00001770: 6564 2e20 4974 206d 6179 2074 616b 6520  ed. It may take 
+00001780: 7469 6d65 2074 6f20 7072 6f64 7563 6520  time to produce 
+00001790: 7265 7375 6c74 732e 7221 0000 0072 8600  results.r!...r..
+000017a0: 0000 4e72 0f00 0000 2909 7262 0000 0072  ..Nr....).rb...r
+000017b0: 5c00 0000 727b 0000 0072 8400 0000 7257  \...r{...r....rW
+000017c0: 0000 00da 135f 6765 745f 6669 6c74 6572  ....._get_filter
+000017d0: 696e 675f 6172 6773 7209 0000 0072 3800  ing_argsr....r8.
+000017e0: 0000 728c 0000 0029 0672 6700 0000 726c  ..r....).rg...rl
+000017f0: 0000 00da 0772 6573 756c 7473 da04 6172  .....results..ar
+00001800: 6773 da07 6f75 7470 7574 3272 8100 0000  gs..output2r....
+00001810: 720f 0000 0072 0f00 0000 7214 0000 0072  r....r....r....r
+00001820: 7a00 0000 e300 0000 732a 0000 0006 0304  z.......s*......
+00001830: 010a 020e 0106 0102 0104 0108 fd12 0508  ................
+00001840: 0112 0106 0208 0112 0104 0204 0604 fc08  ................
+00001850: 0104 0304 ff04 017a 1653 6561 7263 682e  .......z.Search.
+00001860: 5f73 6561 7263 685f 7361 6d70 6c65 7363  _search_samplesc
+00001870: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00001880: 0400 0000 4300 0000 7312 0000 007c 006a  ....C...s....|.j
+00001890: 006a 017c 0164 0167 0164 028d 0253 0029  .j.|.d.g.d...S.)
+000018a0: 034e 7217 0000 0072 8300 0000 2902 727b  .Nr....r....).r{
+000018b0: 0000 00da 0c67 6574 5f64 6174 6173 6574  .....get_dataset
+000018c0: 7329 0272 6700 0000 da06 7065 726d 4964  s).rg.....permId
+000018d0: 720f 0000 0072 0f00 0000 7214 0000 00da  r....r....r.....
+000018e0: 165f 6765 745f 6461 7461 7365 7473 5f63  ._get_datasets_c
+000018f0: 6869 6c64 7265 6eff 0000 0072 8d00 0000  hildren....r....
+00001900: 7a1d 5365 6172 6368 2e5f 6765 745f 6461  z.Search._get_da
+00001910: 7461 7365 7473 5f63 6869 6c64 7265 6e63  tasets_childrenc
+00001920: 0100 0000 0000 0000 0000 0000 0d00 0000  ................
+00001930: 0800 0000 4300 0000 735c 0200 007c 006a  ....C...s\...|.j
+00001940: 0064 0075 0172 117c 00a0 01a1 0064 0075  .d.u.r.|.....d.u
+00001950: 0072 1174 0264 0164 0264 038d 0253 007c  .r.t.d.d.d...S.|
+00001960: 006a 03a0 04a1 007d 0164 0464 0584 007c  .j.....}.d.d...|
+00001970: 01a0 05a1 0044 0083 017d 0264 0664 0584  .....D...}.d.d..
+00001980: 007c 01a0 05a1 0044 0083 017d 037c 0272  .|.....D...}.|.r
+00001990: 8964 077c 0276 0072 3d7c 0264 0719 0064  .d.|.v.r=|.d...d
+000019a0: 0075 0172 3a7c 0264 0719 007c 0264 083c  .u.r:|.d...|.d.<
+000019b0: 007c 0264 073d 007c 027c 005f 037c 006a  .|.d.=.|.|._.|.j
+000019c0: 0664 0964 0a8d 017d 0474 0764 0b74 087c  .d.d...}.t.d.t.|
+000019d0: 0483 019b 009d 0283 0101 0064 0c64 0d84  ...........d.d..
+000019e0: 007c 0444 0083 017d 0574 097c 0583 017d  .|.D...}.t.|...}
+000019f0: 0564 0e64 0d84 007c 0544 0083 017d 057c  .d.d...|.D...}.|
+00001a00: 006a 0a6a 0b7c 0564 0f8d 017d 0567 007d  .j.j.|.d...}.g.}
+00001a10: 067c 0544 005d 0c7d 0774 0c7c 077c 0383  .|.D.].}.t.|.|..
+00001a20: 0272 787c 067c 0767 0137 007d 0671 6c7c  .rx|.|.g.7.}.ql|
+00001a30: 006a 0a6a 0d7c 006a 0e64 1064 0d84 007c  .j.j.|.j.d.d...|
+00001a40: 0644 0083 0164 0964 118d 037d 056e 607c  .D...d.d...}.n`|
+00001a50: 006a 0f72 be7c 00a0 06a1 007d 0467 007d  .j.r.|.....}.g.}
+00001a60: 087c 046a 1044 005d 0e7d 097c 087c 096a  .|.j.D.].}.|.|.j
+00001a70: 1164 1264 1367 027c 006a 0e64 148d 0237  .d.d.g.|.j.d...7
+00001a80: 007d 0871 9574 127c 0864 157c 006a 137c  .}.q.t.|.d.|.j.|
+00001a90: 006a 0a6a 0b83 047d 0a7c 006a 0a6a 0d7c  .j.j...}.|.j.j.|
+00001aa0: 006a 0e64 1664 0d84 007c 0a44 0083 0164  .j.d.d...|.D...d
+00001ab0: 0964 118d 037d 056e 2b64 177c 006a 0376  .d...}.n+d.|.j.v
+00001ac0: 0072 d57c 006a 0aa0 147c 006a 0364 1719  .r.|.j...|.j.d..
+00001ad0: 00a1 016a 1164 1264 1367 027c 006a 0e64  ...j.d.d.g.|.j.d
+00001ae0: 148d 027d 0b6e 127c 00a0 157c 006a 0e64  ...}.n.|...|.j.d
+00001af0: 1264 1367 02a1 027d 0c7c 006a 0a6a 1164  .d.g...}.|.j.j.d
+00001b00: 1f69 007c 0ca4 018e 017d 0b7c 0b7d 0574  .i.|.....}.|.}.t
+00001b10: 0764 1874 087c 0583 019b 009d 0283 0101  .d.t.|..........
+00001b20: 007c 006a 0064 0075 0190 0172 2174 0764  .|.j.d.u...r!t.d
+00001b30: 197c 006a 009b 009d 0283 0101 0074 167c  .|.j.........t.|
+00001b40: 006a 176a 1883 018f 1101 007c 056a 196a  .j.j.......|.j.j
+00001b50: 1a7c 006a 0064 1a64 1b8d 0201 0057 0064  .|.j.d.d.....W.d
+00001b60: 0004 0004 0083 0301 006e 0931 0090 0173  .........n.1...s
+00001b70: 1b77 0101 0001 0001 0059 0001 006e 0774  .w.......Y...n.t
+00001b80: 0764 1c7c 059b 009d 0283 0101 0074 0264  .d.|.........t.d
+00001b90: 1d64 1e64 038d 0253 0029 204e e9ff ffff  .d.d...S.) N....
+00001ba0: ff7a 3b43 6f6e 6669 6775 7261 7469 6f6e  .z;Configuration
+00001bb0: 2066 696c 6573 6572 7669 6365 5f75 726c   fileservice_url
+00001bc0: 206e 6565 6473 2074 6f20 6265 2073 6574   needs to be set
+00001bd0: 2066 6f72 2064 6f77 6e6c 6f61 642e 7278   for download.rx
+00001be0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00001bf0: 0300 0000 0500 0000 5300 0000 7328 0000  ........S...s(..
+00001c00: 0069 007c 005d 105c 027d 017d 027c 01a0  .i.|.].\.}.}.|..
+00001c10: 0064 00a1 0172 027c 0164 0164 0285 0219  .d...r.|.d.d....
+00001c20: 007c 0293 0271 0253 0029 03da 076f 626a  .|...q.S.)...obj
+00001c30: 6563 745f e907 0000 004e a901 da0a 7374  ect_.....N....st
+00001c40: 6172 7473 7769 7468 a903 7210 0000 00da  artswith..r.....
+00001c50: 016b da01 7672 0f00 0000 720f 0000 0072  .k..vr....r....r
+00001c60: 1400 0000 da0a 3c64 6963 7463 6f6d 703e  ......<dictcomp>
+00001c70: 0901 0000 7302 0000 0028 007a 2b53 6561  ....s....(.z+Sea
+00001c80: 7263 682e 7365 6172 6368 5f64 6174 615f  rch.search_data_
+00001c90: 7365 7473 2e3c 6c6f 6361 6c73 3e2e 3c64  sets.<locals>.<d
+00001ca0: 6963 7463 6f6d 703e 6301 0000 0000 0000  ictcomp>c.......
+00001cb0: 0000 0000 0003 0000 0005 0000 0053 0000  .............S..
+00001cc0: 0073 2000 0000 6900 7c00 5d0c 5c02 7d01  .s ...i.|.].\.}.
+00001cd0: 7d02 7c01 a000 6400 a101 7302 7c01 7c02  }.|...d...s.|.|.
+00001ce0: 9302 7102 5300 2901 7297 0000 0072 9900  ..q.S.).r....r..
+00001cf0: 0000 729b 0000 0072 0f00 0000 720f 0000  ..r....r....r...
+00001d00: 0072 1400 0000 729e 0000 000a 0100 0073  .r....r........s
+00001d10: 0200 0000 2000 da02 6964 728e 0000 0054  .... ...idr....T
+00001d20: 726b 0000 007a 0f53 616d 706c 6573 2066  rk...z.Samples f
+00001d30: 6f75 6e64 3a20 6301 0000 0000 0000 0000  ound: c.........
+00001d40: 0000 0002 0000 0004 0000 0053 0000 0073  ...........S...s
+00001d50: 1400 0000 6700 7c00 5d06 7d01 7c01 6400  ....g.|.].}.|.d.
+00001d60: 1900 9102 7102 5300 2901 726f 0000 0072  ....q.S.).ro...r
+00001d70: 0f00 0000 722f 0000 0072 0f00 0000 720f  ....r/...r....r.
+00001d80: 0000 0072 1400 0000 7215 0000 0014 0100  ...r....r.......
+00001d90: 0072 1600 0000 7a2b 5365 6172 6368 2e73  .r....z+Search.s
+00001da0: 6561 7263 685f 6461 7461 5f73 6574 732e  earch_data_sets.
+00001db0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
+00001dc0: 6d70 3e63 0100 0000 0000 0000 0000 0000  mp>c............
+00001dd0: 0200 0000 0400 0000 5300 0000 7318 0000  ........S...s...
+00001de0: 0067 007c 005d 087d 017c 0164 0019 0064  .g.|.].}.|.d...d
+00001df0: 0019 0091 0271 0253 0029 0172 9400 0000  .....q.S.).r....
+00001e00: 720f 0000 0072 2f00 0000 720f 0000 0072  r....r/...r....r
+00001e10: 0f00 0000 7214 0000 0072 1500 0000 1601  ....r....r......
+00001e20: 0000 7232 0000 0029 01da 0770 6572 6d49  ..r2...)...permI
+00001e30: 6473 6301 0000 0000 0000 0000 0000 0002  dsc.............
+00001e40: 0000 0003 0000 0053 0000 00f3 1200 0000  .......S........
+00001e50: 6700 7c00 5d05 7d01 7c01 6a00 9102 7102  g.|.].}.|.j...q.
+00001e60: 5300 720f 0000 00a9 0172 3700 0000 722f  S.r......r7...r/
+00001e70: 0000 0072 0f00 0000 720f 0000 0072 1400  ...r....r....r..
+00001e80: 0000 7215 0000 001f 0100 0073 0200 0000  ..r........s....
+00001e90: 1200 2903 7257 0000 0072 7000 0000 7272  ..).rW...rp...rr
+00001ea0: 0000 0072 6e00 0000 7217 0000 0029 0272  ...rn...r....).r
+00001eb0: 7100 0000 7257 0000 0072 9400 0000 6301  q...rW...r....c.
+00001ec0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
+00001ed0: 0000 0053 0000 0072 a100 0000 720f 0000  ...S...r....r...
+00001ee0: 0072 a200 0000 2902 7210 0000 0072 5b00  .r....).r....r[.
+00001ef0: 0000 720f 0000 0072 0f00 0000 7214 0000  ..r....r....r...
+00001f00: 0072 1500 0000 2d01 0000 7306 0000 0006  .r....-...s.....
+00001f10: 0002 010a ffda 0a64 6174 6173 6574 5f69  .......dataset_i
+00001f20: 647a 1144 6174 6120 7365 7473 2066 6f75  dz.Data sets fou
+00001f30: 6e64 3a20 7273 0000 0046 7274 0000 0072  nd: rs...Frt...r
+00001f40: 7600 0000 7201 0000 0072 7700 0000 720f  v...r....rw...r.
+00001f50: 0000 0029 1b72 6300 0000 da0f 6669 6c65  ...).rc.....file
+00001f60: 7365 7276 6963 655f 7572 6c72 0600 0000  service_urlr....
+00001f70: 725c 0000 00da 0463 6f70 79da 0569 7465  r\.....copy..ite
+00001f80: 6d73 727a 0000 0072 0900 0000 727d 0000  msrz...r....r}..
+00001f90: 0072 3300 0000 727b 0000 00da 0b67 6574  .r3...r{.....get
+00001fa0: 5f64 6174 6173 6574 725f 0000 00da 1a5f  _datasetr_....._
+00001fb0: 6461 7461 7365 745f 6c69 7374 5f66 6f72  dataset_list_for
+00001fc0: 5f72 6573 706f 6e73 6572 5700 0000 7262  _responserW...rb
+00001fd0: 0000 0072 2100 0000 7293 0000 0072 2e00  ...r!...r....r..
+00001fe0: 0000 7295 0000 0072 8a00 0000 728f 0000  ..r....r....r...
+00001ff0: 0072 0700 0000 727e 0000 0072 7f00 0000  .r....r~...r....
+00002000: 721e 0000 0072 8000 0000 290d 7267 0000  r....r....).rg..
+00002010: 00da 0c6d 6169 6e5f 6669 6c74 6572 73da  ...main_filters.
+00002020: 0e6f 626a 6563 745f 6669 6c74 6572 73da  .object_filters.
+00002030: 0f64 6174 6173 6574 5f66 696c 7465 7273  .dataset_filters
+00002040: 7281 0000 00da 0864 6174 6173 6574 73da  r......datasets.
+00002050: 1166 696c 7465 7265 645f 6461 7461 7365  .filtered_datase
+00002060: 7473 725b 0000 00da 016f 7254 0000 0072  tsr[.....orT...r
+00002070: 2800 0000 7290 0000 0072 9100 0000 720f  (...r....r....r.
+00002080: 0000 0072 0f00 0000 7214 0000 00da 1073  ...r....r......s
+00002090: 6561 7263 685f 6461 7461 5f73 6574 7302  earch_data_sets.
+000020a0: 0100 0073 7e00 0000 1601 0401 0201 06ff  ...s~...........
+000020b0: 0a03 1202 1201 0401 0801 0c01 0c01 0601  ................
+000020c0: 0601 0c01 1201 0e02 0801 0e01 0e01 0402  ................
+000020d0: 0801 0a01 0a01 0280 0a02 0601 0201 04ff  ................
+000020e0: 0202 08fd 0605 0801 0401 0a01 0601 0a01  ................
+000020f0: 0aff 0602 0401 0601 04fe 0a03 0601 0202  ................
+00002100: 04fe 0203 08fc 0a06 1201 0a01 08ff 1203  ................
+00002110: 1201 0401 1202 0c01 1001 0e01 1401 1eff  ................
+00002120: 0280 0e03 0c02 7a17 5365 6172 6368 2e73  ......z.Search.s
+00002130: 6561 7263 685f 6461 7461 5f73 6574 7363  earch_data_setsc
+00002140: 0300 0000 0000 0000 0000 0000 0500 0000  ................
+00002150: 0900 0000 4300 0000 739e 0000 0064 007d  ....C...s....d.}
+00002160: 037c 006a 0064 0119 0064 0075 0172 1a7c  .|.j.d...d.u.r.|
+00002170: 006a 0064 0219 0064 0075 0172 1a7c 006a  .j.d...d.u.r.|.j
+00002180: 0064 0119 007c 006a 0064 0219 0069 017d  .d...|.j.d...i.}
+00002190: 0374 017c 006a 0064 0319 007c 006a 0064  .t.|.j.d...|.j.d
+000021a0: 0419 007c 006a 0064 0519 007c 006a 0064  ...|.j.d...|.j.d
+000021b0: 0619 007c 037c 027c 0164 078d 077d 047c  ...|.|.|.d...}.|
+000021c0: 006a 0064 0819 0064 0075 0172 3f7c 006a  .j.d...d.u.r?|.j
+000021d0: 0064 0819 007c 0464 093c 007c 006a 0064  .d...|.d.<.|.j.d
+000021e0: 0a19 0064 0075 0172 4d7c 006a 0064 0a19  ...d.u.rM|.j.d..
+000021f0: 007c 0464 0b3c 007c 0453 0029 0c4e 724f  .|.d.<.|.S.).NrO
+00002200: 0000 0072 5000 0000 724b 0000 0072 4d00  ...rP...rK...rM.
+00002210: 0000 da0a 636f 6c6c 6563 7469 6f6e 724c  ....collectionrL
+00002220: 0000 0029 0772 4b00 0000 724d 0000 0072  ...).rK...rM...r
+00002230: 4e00 0000 7256 0000 00da 0577 6865 7265  N...rV.....where
+00002240: 7271 0000 0072 5700 0000 7251 0000 0072  rq...rW...rQ...r
+00002250: 5900 0000 7252 0000 0072 5a00 0000 2902  Y...rR...rZ...).
+00002260: 725c 0000 00da 0464 6963 7429 0572 6700  r\.....dict).rg.
+00002270: 0000 7257 0000 0072 7100 0000 72b1 0000  ..rW...rq...r...
+00002280: 0072 9100 0000 720f 0000 0072 0f00 0000  .r....r....r....
+00002290: 7214 0000 0072 8f00 0000 4401 0000 7322  r....r....D...s"
+000022a0: 0000 0004 011c 0110 0204 ff0a 0408 0108  ................
+000022b0: 0208 0102 0102 0102 0106 f90e 090e 010e  ................
+000022c0: 010e 0104 017a 1a53 6561 7263 682e 5f67  .....z.Search._g
+000022d0: 6574 5f66 696c 7465 7269 6e67 5f61 7267  et_filtering_arg
+000022e0: 7329 0146 290e da08 5f5f 6e61 6d65 5f5f  s).F)...__name__
+000022f0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+00002300: 7175 616c 6e61 6d65 5f5f da07 5f5f 646f  qualname__..__do
+00002310: 635f 5f72 6600 0000 7282 0000 0072 8700  c__rf...r....r..
+00002320: 0000 728b 0000 0072 8c00 0000 727a 0000  ..r....r....rz..
+00002330: 0072 9500 0000 72af 0000 0072 8f00 0000  .r....r....r....
+00002340: da0d 5f5f 636c 6173 7363 656c 6c5f 5f72  ..__classcell__r
+00002350: 0f00 0000 720f 0000 0072 6900 0000 7214  ....r....ri...r.
+00002360: 0000 0072 6000 0000 b400 0000 7316 0000  ...r`.......s...
+00002370: 0008 0004 010c 0408 0e08 1308 0308 030a  ................
+00002380: 0308 1c08 0310 4272 6000 0000 2915 da12  ......Br`...)...
+00002390: 636f 6e63 7572 7265 6e74 2e66 7574 7572  concurrent.futur
+000023a0: 6573 7218 0000 00da 0670 616e 6461 7372  esr......pandasr
+000023b0: 4200 0000 da1a 7079 6269 732e 7072 6f70  B.....pybis.prop
+000023c0: 6572 7479 5f72 6566 6f72 6d61 7474 6572  erty_reformatter
+000023d0: 7202 0000 00da 0f6f 7065 6e62 6973 5f63  r......openbis_c
+000023e0: 6f6d 6d61 6e64 7204 0000 00da 0e63 6f6d  ommandr......com
+000023f0: 6d61 6e64 5f72 6573 756c 7472 0600 0000  mand_resultr....
+00002400: da05 7574 696c 7372 0700 0000 da12 7363  ..utilsr......sc
+00002410: 7269 7074 732e 636c 6963 6b5f 7574 696c  ripts.click_util
+00002420: 7209 0000 0072 2e00 0000 7238 0000 0072  r....r....r8...r
+00002430: 3b00 0000 7233 0000 0072 4a00 0000 725f  ;...r3...rJ...r_
+00002440: 0000 0072 6000 0000 720f 0000 0072 0f00  ...r`...r....r..
+00002450: 0000 720f 0000 0072 1400 0000 da08 3c6d  ..r....r......<m
+00002460: 6f64 756c 653e 0100 0000 731c 0000 0008  odule>....s.....
+00002470: 0f08 020c 020c 010c 010c 010c 0108 0308  ................
+00002480: 1f08 3408 0908 0708 0f14 27              ..4.......'
```

### Comparing `obis-0.4.2rc6/obis/dm/commands/__pycache__/upload.cpython-310.pyc` & `obis-0.4.2rc7/obis/dm/commands/__pycache__/upload.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/commands/addref.py` & `obis-0.4.2rc7/obis/dm/commands/addref.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/commands/clone.py` & `obis-0.4.2rc7/obis/dm/commands/clone.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/commands/collection.py` & `obis-0.4.2rc7/obis/dm/commands/collection.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/commands/download.py` & `obis-0.4.2rc7/obis/dm/commands/download.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/commands/download_physical.py` & `obis-0.4.2rc7/obis/dm/commands/download_physical.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/commands/move.py` & `obis-0.4.2rc7/obis/dm/commands/move.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/commands/object.py` & `obis-0.4.2rc7/obis/dm/commands/object.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/commands/openbis_command.py` & `obis-0.4.2rc7/obis/dm/commands/openbis_command.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/commands/openbis_command_test.py` & `obis-0.4.2rc7/obis/dm/commands/openbis_command_test.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/commands/openbis_sync.py` & `obis-0.4.2rc7/obis/dm/commands/openbis_sync.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/commands/removeref.py` & `obis-0.4.2rc7/obis/dm/commands/removeref.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/commands/search.py` & `obis-0.4.2rc7/obis/dm/commands/search.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,28 +14,27 @@
 #
 
 import concurrent.futures
 
 import pandas as pd
 
 from pybis.property_reformatter import is_of_openbis_supported_date_format
-from pybis.sample import Sample
 from .openbis_command import OpenbisCommand
 from ..command_result import CommandResult
 from ..utils import cd
 from ...scripts.click_util import click_echo
 
 
 def _dfs(objects, prop, func, func_specific):
     """Helper function that perform DFS search over children graph of objects"""
+    # TODO: improve performance of this - make it similar to _dfs_samples
     with concurrent.futures.ThreadPoolExecutor(
             max_workers=5) as pool_simple, concurrent.futures.ThreadPoolExecutor(
         max_workers=20) as pool_full:
-        stack = [getattr(openbis_obj, prop) for openbis_obj in
-                 objects]  # datasets and samples provide children in different formats
+        stack = [openbis_obj[prop] for openbis_obj in objects]  # datasets and samples provide children in different formats
         visited = set()
         stack.reverse()
         output = []
         while stack:
             simple_results = pool_simple.map(func, stack)
             stack = []
             children = []
@@ -51,20 +50,34 @@
             for child in children:
                 if child not in visited:
                     stack += [child]
 
     return output
 
 
-def _get_datasets_of_samples(get_dataset_method, samples):
-    output = []
-    with concurrent.futures.ThreadPoolExecutor(
-            max_workers=5) as pool_simple:
-        output = pool_simple.map(get_dataset_method, samples)
-
+def _dfs_samples(data_base, prop, func):
+    """Helper function that perform DFS search over children graph of objects"""
+    output = data_base
+    ids = [x['children'] for x in data_base if x['children']]
+    ids = [x[prop][prop] for x in flatten(ids)]
+    visited = set([x[prop][prop] for x in data_base])
+    while ids:
+        data = func(ids)
+        data = list(data.values())
+        output += data
+        ids = []
+        children = []
+        for obj in data:
+            key = obj[prop][prop]
+            children += [x[prop][prop] for x in obj['children']]
+            if key not in visited:
+                visited.add(key)
+        for child in children:
+            if child not in visited:
+                ids += [child]
     return output
 
 
 def flatten(matrix):
     flat_list = []
     for row in matrix:
         flat_list += row
@@ -141,15 +154,21 @@
         self.recursive = recursive
         self.save_path = save_path
         self.load_global_config(dm)
         self.props = "*"
         super(Search, self).__init__(dm)
 
     def search_samples(self):
-        search_results = self._search_samples()
+        search_results = self._search_samples(raw_response=True)
+
+        search_results = self.openbis._sample_list_for_response(props=self.props,
+                                                                response=search_results,
+                                                                attrs=["parents", "children",
+                                                                       "dataSets"],
+                                                                parsed=True)
 
         click_echo(f"Objects found: {len(search_results)}")
         if self.save_path is not None:
             click_echo(f"Saving search results in {self.save_path}")
             with cd(self.data_mgmt.invocation_path):
                 search_results.df.to_csv(self.save_path, index=False)
         else:
@@ -159,38 +178,43 @@
 
     def _get_samples_children(self, identifier):
         return self.openbis.get_samples(identifier, attrs=["children", "dataSets"])
 
     def _get_sample_with_datasets(self, identifier):
         return self.openbis.get_sample(identifier, withDataSetIds=True)
 
-    def _search_samples(self):
+    def _get_sample_with_datasets2(self, identifier):
+        return self.openbis.get_sample(identifier, withDataSetIds=True, raw_response=True)
+
+    def _search_samples(self, raw_response=False):
         """Helper method to search samples"""
 
+        if self.recursive:
+            raw_response = True
+
         if "object_code" in self.filters:
             results = self.openbis.get_samples(identifier=self.filters['object_code'],
                                                attrs=["parents", "children", "dataSets"],
+                                               raw_response=raw_response,
                                                props=self.props)
         else:
             args = self._get_filtering_args(self.props, ["parents", "children", "dataSets"])
+            args["raw_response"] = raw_response
             results = self.openbis.get_samples(**args)
 
         if self.recursive:
             click_echo(f"Recursive search enabled. It may take time to produce results.")
-            output = _dfs(results.objects, 'identifier',
-                          self._get_samples_children,
-                          self._get_sample_with_datasets)  # samples provide identifiers as children
-            search_results = self.openbis._sample_list_for_response(props=self.props,
-                                                                    response=[sample.data for sample
-                                                                              in output],
-                                                                    attrs=["parents", "children",
-                                                                           "dataSets"],
-                                                                    parsed=True)
+            output2 = _dfs_samples(results['objects'], 'identifier', self._get_sample_with_datasets2)
+
+            search_results = output2
         else:
-            search_results = results
+            if raw_response:
+                search_results = results['objects']
+            else:
+                search_results = results
         return search_results
 
     def _get_datasets_children(self, permId):
         return self.openbis.get_datasets(permId, attrs=["children"])
 
     def search_data_sets(self):
         if self.save_path is not None and self.fileservice_url() is None:
@@ -199,30 +223,34 @@
 
         main_filters = self.filters.copy()
 
         object_filters = {k[7:]: v for (k, v) in main_filters.items() if k.startswith('object_')}
         dataset_filters = {k: v for (k, v) in main_filters.items() if not k.startswith('object_')}
         if object_filters:
             if 'id' in object_filters:
-                object_filters['object_code'] = object_filters['id']
+                if object_filters['id'] is not None:
+                    object_filters['object_code'] = object_filters['id']
                 del object_filters['id']
             self.filters = object_filters
-            search_results = self._search_samples()
-            datasets = [x for x in _get_datasets_of_samples(Sample.get_datasets, search_results) if
-                        x.totalCount > 0]
-            for thing in datasets:
-                for obj in thing.objects:
-                    if not _filter_dataset(obj, dataset_filters):
-                        for i in range(len(thing.response)):
-                            if thing.response[i]['permId']['permId'] == obj.permId:
-                                del thing.response[i]
-                                break
-            datasets = [x.response for x in datasets]
+            search_results = self._search_samples(raw_response=True)
+            click_echo(f"Samples found: {len(search_results)}")
+
+            datasets = [x["dataSets"] for x in search_results]
+            datasets = flatten(datasets)
+            datasets = [x['permId']['permId'] for x in datasets]
+            datasets = self.openbis.get_dataset(permIds=datasets)
+
+            filtered_datasets = []
+            for dataset in datasets:
+                if _filter_dataset(dataset, dataset_filters):
+                    filtered_datasets += [dataset]
+
             datasets = self.openbis._dataset_list_for_response(props=self.props,
-                                                               response=flatten(datasets),
+                                                               response=[x.data for x in
+                                                                         filtered_datasets],
                                                                parsed=True)
         else:
             if self.recursive:
                 search_results = self._search_samples()  # Look for samples recursively
                 o = []
                 for sample in search_results.objects:  # get datasets
                     o += sample.get_datasets(
@@ -260,15 +288,15 @@
             where = {
                 self.filters['property_code']: self.filters['property_value'],
             }
 
         args = dict(space=self.filters['space'],
                     project=self.filters['project'],
                     # Not Supported with Project Samples disabled
-                    experiment=self.filters['experiment'],
+                    experiment=self.filters['collection'],
                     type=self.filters['type_code'],
                     where=where,
                     attrs=attrs,
                     props=props)
 
         if self.filters['registration_date'] is not None:
             args['registrationDate'] = self.filters['registration_date']
```

### Comparing `obis-0.4.2rc6/obis/dm/commands/upload.py` & `obis-0.4.2rc7/obis/dm/commands/upload.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/config.py` & `obis-0.4.2rc7/obis/dm/config.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/config_test.py` & `obis-0.4.2rc7/obis/dm/config_test.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/data_mgmt.py` & `obis-0.4.2rc7/obis/dm/data_mgmt.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/data_mgmt_test.py` & `obis-0.4.2rc7/obis/dm/data_mgmt_test.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/git.py` & `obis-0.4.2rc7/obis/dm/git.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/repository_utils.py` & `obis-0.4.2rc7/obis/dm/repository_utils.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/utils.py` & `obis-0.4.2rc7/obis/dm/utils.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/dm/utils_test.py` & `obis-0.4.2rc7/obis/dm/utils_test.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/scripts/__init__.py` & `obis-0.4.2rc7/obis/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/scripts/__pycache__/cli.cpython-310.pyc` & `obis-0.4.2rc7/obis/scripts/__pycache__/cli.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 17 10:13:46 2023 UTC, .py size: 39340 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5a14 b564 ac99 0000  o.......Z..d....
+00000000: 6f0d 0d0a 0000 0000 af54 be64 ac99 0000  o........T.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0012 0000 0040 0000 0073 720d 0000 6400  .....@...sr...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d03 5a03 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6402 6c04 5a04 6401 6404 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6401 6405 6c07 6d08 5a08 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6406 6c09 6d0a 5a0a 0100 6407 6408 6c0b  d.l.m.Z...d.d.l.
@@ -1086,15 +1086,15 @@
 000043d0: 0100 0072 d300 0000 7a45 4f62 6a65 6374  ...r....zEObject
 000043e0: 2070 6172 616d 6574 6572 2064 6574 6563   parameter detec
 000043f0: 7465 6421 204f 7468 6572 2066 696c 7465  ted! Other filte
 00004400: 7269 6e67 2061 7267 756d 656e 7473 2077  ring arguments w
 00004410: 696c 6c20 6265 206f 6d69 7474 6564 2129  ill be omitted!)
 00004420: 01da 0b6f 626a 6563 745f 636f 6465 2908  ...object_code).
 00004430: 72b4 0000 0072 d600 0000 72d7 0000 0072  r....r....r....r
-00004440: d800 0000 72b5 0000 0072 b700 0000 72b8  ....r....r....r.
+00004440: e300 0000 72b5 0000 0072 b700 0000 72b8  ....r....r....r.
 00004450: 0000 0072 b600 0000 da0d 6f62 6a65 6374  ...r......object
 00004460: 5f73 6561 7263 6863 0100 0000 0000 0000  _searchc........
 00004470: 0000 0000 0100 0000 0500 0000 1300 0000  ................
 00004480: 72da 0000 0072 1a00 0000 2901 da0d 7365  r....r....)...se
 00004490: 6172 6368 5f6f 626a 6563 7472 3200 0000  arch_objectr2...
 000044a0: 72dc 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
 000044b0: 3600 0000 ec01 0000 72df 0000 007a 1f6f  6.......r....z.o
```

### Comparing `obis-0.4.2rc6/obis/scripts/__pycache__/click_util.cpython-310.pyc` & `obis-0.4.2rc7/obis/scripts/__pycache__/click_util.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/scripts/__pycache__/data_mgmt_runner.cpython-310.pyc` & `obis-0.4.2rc7/obis/scripts/__pycache__/data_mgmt_runner.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/scripts/cli.py` & `obis-0.4.2rc7/obis/scripts/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -481,15 +481,15 @@
     ctx.obj['runner'] = DataMgmtRunner(ctx.obj, halt_on_error_log=False)
     if object_id is not None:
         if any(v is not None for v in filtering_arguments):
             click_echo("Object parameter detected! Other filtering arguments will be omitted!")
         filters = dict(object_code=object_id)
     else:
         filters = dict(type_code=type_code, space=space,
-                       project=project, experiment=collection, property_code=property_code,
+                       project=project, collection=collection, property_code=property_code,
                        registration_date=registration_date, modification_date=modification_date,
                        property_value=property_value)
     return ctx.obj['runner'].run("object_search",
                                  lambda dm: dm.search_object(filters, recursive, save))
 
 
 # # collection: collection_id
```

### Comparing `obis-0.4.2rc6/obis/scripts/click_util.py` & `obis-0.4.2rc7/obis/scripts/click_util.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/scripts/data_mgmt_runner.py` & `obis-0.4.2rc7/obis/scripts/data_mgmt_runner.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis/test-data/snb-data.zip` & `obis-0.4.2rc7/obis/test-data/snb-data.zip`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/obis.egg-info/PKG-INFO` & `obis-0.4.2rc7/obis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obis
-Version: 0.4.2rc6
+Version: 0.4.2rc7
 Summary: Local data management with assistance from OpenBIS.
 Home-page: https://sissource.ethz.ch/sispub/openbis/tree/master/app-openbis-command-line
 Author: ID SIS • ETH Zürich
 Author-email: openbis-support@id.ethz.ch
 License: Apache Software License Version 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `obis-0.4.2rc6/obis.egg-info/SOURCES.txt` & `obis-0.4.2rc7/obis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc6/setup.py` & `obis-0.4.2rc7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,26 +27,26 @@
 data_dir = os.path.join("man", "man1")
 data_files = [
     (d, [os.path.join(d, f) for f in files]) for d, folders, files in os.walk(data_dir)
 ]
 
 setup(
     name="obis",
-    version="0.4.2rc6",
+    version="0.4.2rc7",
     description="Local data management with assistance from OpenBIS.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://sissource.ethz.ch/sispub/openbis/tree/master/app-openbis-command-line",
     author="ID SIS • ETH Zürich",
     author_email="openbis-support@id.ethz.ch",
     license="Apache Software License Version 2.0",
     packages=["obis", "obis.dm", "obis.dm.commands", "obis.scripts"],
     data_files=data_files,
     package_data={"obis": ["dm/git-annex-attributes"]},
-    install_requires=["pyOpenSSL", "pytest", "pybis==1.35.11", "click"],
+    install_requires=["pyOpenSSL", "pytest", "pybis==1.36.0", "click"],
     entry_points={"console_scripts": ["obis=obis.scripts.cli:main"]},
     zip_safe=False,
     python_requires=">=3.3",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
```

