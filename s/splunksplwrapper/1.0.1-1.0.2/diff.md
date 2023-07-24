# Comparing `tmp/splunksplwrapper-1.0.1.tar.gz` & `tmp/splunksplwrapper-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splunksplwrapper-1.0.1.tar", max compression
+gzip compressed data, was "splunksplwrapper-1.0.2.tar", max compression
```

## Comparing `splunksplwrapper-1.0.1.tar` & `splunksplwrapper-1.0.2.tar`

### file list

```diff
@@ -1,71 +1,70 @@
--rw-r--r--   0        0        0    11341 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/LICENSE
--rw-r--r--   0        0        0     1003 2023-02-16 13:04:38.341528 splunksplwrapper-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    43137 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/SearchUtil.py
--rw-r--r--   0        0        0      623 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/__init__.py
--rw-r--r--   0        0        0     5837 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/app/__init__.py
--rw-r--r--   0        0        0      664 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/connector/__init__.py
--rw-r--r--   0        0        0     4073 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/connector/base.py
--rw-r--r--   0        0        0     3004 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/connector/httplib2_handler.py
--rw-r--r--   0        0        0    14707 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/connector/rest.py
--rw-r--r--   0        0        0     8804 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/connector/sdk.py
--rw-r--r--   0        0        0     2596 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/exceptions/__init__.py
--rw-r--r--   0        0        0     2034 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/exceptions/command_execution.py
--rw-r--r--   0        0        0     1387 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/exceptions/confs.py
--rw-r--r--   0        0        0     1009 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/exceptions/search.py
--rw-r--r--   0        0        0     1351 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/exceptions/wait.py
--rw-r--r--   0        0        0     2431 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/log/__init__.py
--rw-r--r--   0        0        0     1265 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/log/logging.conf
--rw-r--r--   0        0        0      816 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/manager/__init__.py
--rw-r--r--   0        0        0     3430 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/manager/confs/__init__.py
--rw-r--r--   0        0        0     2590 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/manager/confs/conf.py
--rw-r--r--   0        0        0     3783 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/manager/confs/rest/__init__.py
--rw-r--r--   0        0        0     6060 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/manager/confs/rest/conf.py
--rw-r--r--   0        0        0     3050 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/manager/confs/rest/stanza.py
--rw-r--r--   0        0        0     2320 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/manager/confs/sdk/__init__.py
--rw-r--r--   0        0        0     2683 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/manager/confs/sdk/conf.py
--rw-r--r--   0        0        0     2969 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/manager/confs/sdk/stanza.py
--rw-r--r--   0        0        0     2624 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/manager/confs/stanza.py
--rw-r--r--   0        0        0     3260 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/manager/indexes/__init__.py
--rw-r--r--   0        0        0     1306 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/manager/indexes/index.py
--rw-r--r--   0        0        0     8263 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/manager/indexes/rest/__init__.py
--rw-r--r--   0        0        0     4742 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/manager/indexes/rest/index.py
--rw-r--r--   0        0        0     1924 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/manager/indexes/sdk/__init__.py
--rw-r--r--   0        0        0     4499 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/manager/indexes/sdk/index.py
--rw-r--r--   0        0        0     2278 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/manager/jobs/__init__.py
--rw-r--r--   0        0        0     3054 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/manager/jobs/job.py
--rw-r--r--   0        0        0     7585 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/manager/jobs/rest/__init__.py
--rw-r--r--   0        0        0    10450 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/manager/jobs/rest/job.py
--rw-r--r--   0        0        0     6489 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/manager/jobs/results.py
--rw-r--r--   0        0        0     1458 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/manager/jobs/sdk/__init__.py
--rw-r--r--   0        0        0     8241 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/manager/jobs/sdk/job.py
--rw-r--r--   0        0        0      823 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/manager/object.py
--rw-r--r--   0        0        0     3323 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/manager/roles/__init__.py
--rw-r--r--   0        0        0     1021 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/manager/roles/role.py
--rw-r--r--   0        0        0     2948 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/manager/roles/sdk/__init__.py
--rw-r--r--   0        0        0     1704 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/manager/roles/sdk/role.py
--rw-r--r--   0        0        0     2962 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/manager/saved_searches/__init__.py
--rw-r--r--   0        0        0     1961 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/manager/saved_searches/saved_search.py
--rw-r--r--   0        0        0     3276 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/manager/saved_searches/sdk/__init__.py
--rw-r--r--   0        0        0     3409 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/manager/saved_searches/sdk/saved_search.py
--rw-r--r--   0        0        0     3159 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/manager/users/__init__.py
--rw-r--r--   0        0        0     2883 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/manager/users/sdk/__init__.py
--rw-r--r--   0        0        0     1730 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/manager/users/sdk/user.py
--rw-r--r--   0        0        0     1426 2023-02-16 13:03:55.133701 splunksplwrapper-1.0.1/splunksplwrapper/manager/users/user.py
--rw-r--r--   0        0        0      575 2023-02-16 13:03:55.137701 splunksplwrapper-1.0.1/splunksplwrapper/misc/__init__.py
--rw-r--r--   0        0        0     1479 2023-02-16 13:03:55.137701 splunksplwrapper-1.0.1/splunksplwrapper/misc/collection.py
--rw-r--r--   0        0        0     1045 2023-02-16 13:03:55.137701 splunksplwrapper-1.0.1/splunksplwrapper/misc/manager_utils.py
--rw-r--r--   0        0        0      602 2023-02-16 13:03:55.137701 splunksplwrapper-1.0.1/splunksplwrapper/splunk/__init__.py
--rw-r--r--   0        0        0    20632 2023-02-16 13:03:55.137701 splunksplwrapper-1.0.1/splunksplwrapper/splunk/base.py
--rw-r--r--   0        0        0    10711 2023-02-16 13:03:55.137701 splunksplwrapper-1.0.1/splunksplwrapper/splunk/cloud.py
--rw-r--r--   0        0        0    10607 2023-02-16 13:03:55.137701 splunksplwrapper-1.0.1/splunksplwrapper/util/Constants.py
--rw-r--r--   0        0        0      575 2023-02-16 13:03:55.137701 splunksplwrapper-1.0.1/splunksplwrapper/util/__init__.py
--rw-r--r--   0        0        0     2714 2023-02-16 13:03:55.137701 splunksplwrapper-1.0.1/splunksplwrapper/util/action_writer.py
--rw-r--r--   0        0        0      783 2023-02-16 13:03:55.137701 splunksplwrapper-1.0.1/splunksplwrapper/util/attrdict.py
--rw-r--r--   0        0        0     2468 2023-02-16 13:03:55.137701 splunksplwrapper-1.0.1/splunksplwrapper/util/basefileutils.py
--rw-r--r--   0        0        0     6882 2023-02-16 13:03:55.137701 splunksplwrapper-1.0.1/splunksplwrapper/util/rest_uris.py
--rw-r--r--   0        0        0     3316 2023-02-16 13:03:55.137701 splunksplwrapper-1.0.1/splunksplwrapper/util/restutils.py
--rw-r--r--   0        0        0    21489 2023-02-16 13:03:55.137701 splunksplwrapper-1.0.1/splunksplwrapper/util/rip.py
--rw-r--r--   0        0        0    29429 2023-02-16 13:03:55.137701 splunksplwrapper-1.0.1/splunksplwrapper/util/searchhelpers.py
--rw-r--r--   0        0        0      963 2023-02-16 13:03:55.137701 splunksplwrapper-1.0.1/splunksplwrapper/util/string_unicode_convert.py
--rw-r--r--   0        0        0     1508 1970-01-01 00:00:00.000000 splunksplwrapper-1.0.1/setup.py
--rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 splunksplwrapper-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11341 2023-07-24 12:17:41.000724 splunksplwrapper-1.0.2/LICENSE
+-rw-r--r--   0        0        0      998 2023-07-24 12:18:23.653492 splunksplwrapper-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    43137 2023-07-24 12:17:41.000724 splunksplwrapper-1.0.2/splunksplwrapper/SearchUtil.py
+-rw-r--r--   0        0        0      623 2023-07-24 12:17:41.000724 splunksplwrapper-1.0.2/splunksplwrapper/__init__.py
+-rw-r--r--   0        0        0     5837 2023-07-24 12:17:41.000724 splunksplwrapper-1.0.2/splunksplwrapper/app/__init__.py
+-rw-r--r--   0        0        0      664 2023-07-24 12:17:41.000724 splunksplwrapper-1.0.2/splunksplwrapper/connector/__init__.py
+-rw-r--r--   0        0        0     4073 2023-07-24 12:17:41.000724 splunksplwrapper-1.0.2/splunksplwrapper/connector/base.py
+-rw-r--r--   0        0        0     3004 2023-07-24 12:17:41.000724 splunksplwrapper-1.0.2/splunksplwrapper/connector/httplib2_handler.py
+-rw-r--r--   0        0        0    14707 2023-07-24 12:17:41.000724 splunksplwrapper-1.0.2/splunksplwrapper/connector/rest.py
+-rw-r--r--   0        0        0     8859 2023-07-24 12:17:41.000724 splunksplwrapper-1.0.2/splunksplwrapper/connector/sdk.py
+-rw-r--r--   0        0        0     2596 2023-07-24 12:17:41.000724 splunksplwrapper-1.0.2/splunksplwrapper/exceptions/__init__.py
+-rw-r--r--   0        0        0     2034 2023-07-24 12:17:41.000724 splunksplwrapper-1.0.2/splunksplwrapper/exceptions/command_execution.py
+-rw-r--r--   0        0        0     1387 2023-07-24 12:17:41.000724 splunksplwrapper-1.0.2/splunksplwrapper/exceptions/confs.py
+-rw-r--r--   0        0        0     1009 2023-07-24 12:17:41.000724 splunksplwrapper-1.0.2/splunksplwrapper/exceptions/search.py
+-rw-r--r--   0        0        0     1351 2023-07-24 12:17:41.000724 splunksplwrapper-1.0.2/splunksplwrapper/exceptions/wait.py
+-rw-r--r--   0        0        0     2431 2023-07-24 12:17:41.000724 splunksplwrapper-1.0.2/splunksplwrapper/log/__init__.py
+-rw-r--r--   0        0        0     1265 2023-07-24 12:17:41.000724 splunksplwrapper-1.0.2/splunksplwrapper/log/logging.conf
+-rw-r--r--   0        0        0      816 2023-07-24 12:17:41.000724 splunksplwrapper-1.0.2/splunksplwrapper/manager/__init__.py
+-rw-r--r--   0        0        0     3430 2023-07-24 12:17:41.000724 splunksplwrapper-1.0.2/splunksplwrapper/manager/confs/__init__.py
+-rw-r--r--   0        0        0     2590 2023-07-24 12:17:41.000724 splunksplwrapper-1.0.2/splunksplwrapper/manager/confs/conf.py
+-rw-r--r--   0        0        0     3783 2023-07-24 12:17:41.000724 splunksplwrapper-1.0.2/splunksplwrapper/manager/confs/rest/__init__.py
+-rw-r--r--   0        0        0     6060 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/manager/confs/rest/conf.py
+-rw-r--r--   0        0        0     3050 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/manager/confs/rest/stanza.py
+-rw-r--r--   0        0        0     2320 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/manager/confs/sdk/__init__.py
+-rw-r--r--   0        0        0     2683 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/manager/confs/sdk/conf.py
+-rw-r--r--   0        0        0     2969 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/manager/confs/sdk/stanza.py
+-rw-r--r--   0        0        0     2624 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/manager/confs/stanza.py
+-rw-r--r--   0        0        0     3260 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/manager/indexes/__init__.py
+-rw-r--r--   0        0        0     1306 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/manager/indexes/index.py
+-rw-r--r--   0        0        0     8263 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/manager/indexes/rest/__init__.py
+-rw-r--r--   0        0        0     4742 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/manager/indexes/rest/index.py
+-rw-r--r--   0        0        0     1924 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/manager/indexes/sdk/__init__.py
+-rw-r--r--   0        0        0     4499 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/manager/indexes/sdk/index.py
+-rw-r--r--   0        0        0     2278 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/manager/jobs/__init__.py
+-rw-r--r--   0        0        0     3054 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/manager/jobs/job.py
+-rw-r--r--   0        0        0     7585 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/manager/jobs/rest/__init__.py
+-rw-r--r--   0        0        0    10450 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/manager/jobs/rest/job.py
+-rw-r--r--   0        0        0     6489 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/manager/jobs/results.py
+-rw-r--r--   0        0        0     1458 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/manager/jobs/sdk/__init__.py
+-rw-r--r--   0        0        0     8241 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/manager/jobs/sdk/job.py
+-rw-r--r--   0        0        0      823 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/manager/object.py
+-rw-r--r--   0        0        0     3323 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/manager/roles/__init__.py
+-rw-r--r--   0        0        0     1021 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/manager/roles/role.py
+-rw-r--r--   0        0        0     2948 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/manager/roles/sdk/__init__.py
+-rw-r--r--   0        0        0     1704 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/manager/roles/sdk/role.py
+-rw-r--r--   0        0        0     2962 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/manager/saved_searches/__init__.py
+-rw-r--r--   0        0        0     1961 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/manager/saved_searches/saved_search.py
+-rw-r--r--   0        0        0     3276 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/manager/saved_searches/sdk/__init__.py
+-rw-r--r--   0        0        0     3409 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/manager/saved_searches/sdk/saved_search.py
+-rw-r--r--   0        0        0     3159 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/manager/users/__init__.py
+-rw-r--r--   0        0        0     2883 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/manager/users/sdk/__init__.py
+-rw-r--r--   0        0        0     1730 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/manager/users/sdk/user.py
+-rw-r--r--   0        0        0     1426 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/manager/users/user.py
+-rw-r--r--   0        0        0      575 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/misc/__init__.py
+-rw-r--r--   0        0        0     1479 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/misc/collection.py
+-rw-r--r--   0        0        0     1045 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/misc/manager_utils.py
+-rw-r--r--   0        0        0      602 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/splunk/__init__.py
+-rw-r--r--   0        0        0    20632 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/splunk/base.py
+-rw-r--r--   0        0        0    10711 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/splunk/cloud.py
+-rw-r--r--   0        0        0    10607 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/util/Constants.py
+-rw-r--r--   0        0        0      575 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/util/__init__.py
+-rw-r--r--   0        0        0     2714 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/util/action_writer.py
+-rw-r--r--   0        0        0      783 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/util/attrdict.py
+-rw-r--r--   0        0        0     2468 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/util/basefileutils.py
+-rw-r--r--   0        0        0     6882 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/util/rest_uris.py
+-rw-r--r--   0        0        0     3316 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/util/restutils.py
+-rw-r--r--   0        0        0    21489 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/util/rip.py
+-rw-r--r--   0        0        0    29429 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/util/searchhelpers.py
+-rw-r--r--   0        0        0      963 2023-07-24 12:17:41.004724 splunksplwrapper-1.0.2/splunksplwrapper/util/string_unicode_convert.py
+-rw-r--r--   0        0        0      685 1970-01-01 00:00:00.000000 splunksplwrapper-1.0.2/PKG-INFO
```

### Comparing `splunksplwrapper-1.0.1/LICENSE` & `splunksplwrapper-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/pyproject.toml` & `splunksplwrapper-1.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 [tool.poetry]
 name = "splunksplwrapper"
-version = "1.0.1"
+version = "1.0.2"
 description = "Package to interact with Splunk"
 authors = ["Splunk <addonfactory@splunk.com>"]
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 httplib2 = "^0.21.0"
 defusedxml = "^0.7.1"
-splunk-sdk = "^1.6.18"
+splunk-sdk = ">=1.6"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.2.0"
+pytest = ">=7"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/SearchUtil.py` & `splunksplwrapper-1.0.2/splunksplwrapper/SearchUtil.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/__init__.py` & `splunksplwrapper-1.0.2/splunksplwrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/app/__init__.py` & `splunksplwrapper-1.0.2/splunksplwrapper/app/__init__.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/connector/__init__.py` & `splunksplwrapper-1.0.2/splunksplwrapper/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/connector/base.py` & `splunksplwrapper-1.0.2/splunksplwrapper/connector/base.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/connector/httplib2_handler.py` & `splunksplwrapper-1.0.2/splunksplwrapper/connector/httplib2_handler.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/connector/rest.py` & `splunksplwrapper-1.0.2/splunksplwrapper/connector/rest.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/connector/sdk.py` & `splunksplwrapper-1.0.2/splunksplwrapper/connector/sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,14 +136,16 @@
             # 'namespace': self.namespace,
             "owner": self.owner,
             "app": self.app,
             "sharing": self.sharing,
             "scheme": self.splunk.splunkd_scheme(),
             "host": self.splunk.splunkd_host(),
             "port": self.splunk.splunkd_port(),
+            "retries": 3,
+            "retryDelay": 5,
         }
 
     def __del__(self):
         """
         Called when the object is being deallocated.
         It unregisters itself with the Splunk start listeners.
         """
```

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/exceptions/__init__.py` & `splunksplwrapper-1.0.2/splunksplwrapper/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/exceptions/command_execution.py` & `splunksplwrapper-1.0.2/splunksplwrapper/exceptions/command_execution.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/exceptions/confs.py` & `splunksplwrapper-1.0.2/splunksplwrapper/exceptions/confs.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/exceptions/search.py` & `splunksplwrapper-1.0.2/splunksplwrapper/exceptions/search.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/exceptions/wait.py` & `splunksplwrapper-1.0.2/splunksplwrapper/exceptions/wait.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/log/__init__.py` & `splunksplwrapper-1.0.2/splunksplwrapper/log/__init__.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/log/logging.conf` & `splunksplwrapper-1.0.2/splunksplwrapper/log/logging.conf`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/manager/__init__.py` & `splunksplwrapper-1.0.2/splunksplwrapper/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/manager/confs/__init__.py` & `splunksplwrapper-1.0.2/splunksplwrapper/manager/confs/__init__.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/manager/confs/conf.py` & `splunksplwrapper-1.0.2/splunksplwrapper/manager/confs/conf.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/manager/confs/rest/__init__.py` & `splunksplwrapper-1.0.2/splunksplwrapper/manager/confs/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/manager/confs/rest/conf.py` & `splunksplwrapper-1.0.2/splunksplwrapper/manager/confs/rest/conf.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/manager/confs/rest/stanza.py` & `splunksplwrapper-1.0.2/splunksplwrapper/manager/confs/rest/stanza.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/manager/confs/sdk/__init__.py` & `splunksplwrapper-1.0.2/splunksplwrapper/manager/confs/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/manager/confs/sdk/conf.py` & `splunksplwrapper-1.0.2/splunksplwrapper/manager/confs/sdk/conf.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/manager/confs/sdk/stanza.py` & `splunksplwrapper-1.0.2/splunksplwrapper/manager/confs/sdk/stanza.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/manager/confs/stanza.py` & `splunksplwrapper-1.0.2/splunksplwrapper/manager/confs/stanza.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/manager/indexes/__init__.py` & `splunksplwrapper-1.0.2/splunksplwrapper/manager/indexes/__init__.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/manager/indexes/index.py` & `splunksplwrapper-1.0.2/splunksplwrapper/manager/indexes/index.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/manager/indexes/rest/__init__.py` & `splunksplwrapper-1.0.2/splunksplwrapper/manager/indexes/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/manager/indexes/rest/index.py` & `splunksplwrapper-1.0.2/splunksplwrapper/manager/indexes/rest/index.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/manager/indexes/sdk/__init__.py` & `splunksplwrapper-1.0.2/splunksplwrapper/manager/indexes/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/manager/indexes/sdk/index.py` & `splunksplwrapper-1.0.2/splunksplwrapper/manager/indexes/sdk/index.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/manager/jobs/__init__.py` & `splunksplwrapper-1.0.2/splunksplwrapper/manager/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/manager/jobs/job.py` & `splunksplwrapper-1.0.2/splunksplwrapper/manager/jobs/job.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/manager/jobs/rest/__init__.py` & `splunksplwrapper-1.0.2/splunksplwrapper/manager/jobs/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/manager/jobs/rest/job.py` & `splunksplwrapper-1.0.2/splunksplwrapper/manager/jobs/rest/job.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/manager/jobs/results.py` & `splunksplwrapper-1.0.2/splunksplwrapper/manager/jobs/results.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/manager/jobs/sdk/__init__.py` & `splunksplwrapper-1.0.2/splunksplwrapper/manager/jobs/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/manager/jobs/sdk/job.py` & `splunksplwrapper-1.0.2/splunksplwrapper/manager/jobs/sdk/job.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/manager/object.py` & `splunksplwrapper-1.0.2/splunksplwrapper/manager/object.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/manager/roles/__init__.py` & `splunksplwrapper-1.0.2/splunksplwrapper/manager/roles/__init__.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/manager/roles/role.py` & `splunksplwrapper-1.0.2/splunksplwrapper/manager/roles/role.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/manager/roles/sdk/__init__.py` & `splunksplwrapper-1.0.2/splunksplwrapper/manager/roles/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/manager/roles/sdk/role.py` & `splunksplwrapper-1.0.2/splunksplwrapper/manager/roles/sdk/role.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/manager/saved_searches/__init__.py` & `splunksplwrapper-1.0.2/splunksplwrapper/manager/saved_searches/__init__.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/manager/saved_searches/saved_search.py` & `splunksplwrapper-1.0.2/splunksplwrapper/manager/saved_searches/saved_search.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/manager/saved_searches/sdk/__init__.py` & `splunksplwrapper-1.0.2/splunksplwrapper/manager/saved_searches/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/manager/saved_searches/sdk/saved_search.py` & `splunksplwrapper-1.0.2/splunksplwrapper/manager/saved_searches/sdk/saved_search.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/manager/users/__init__.py` & `splunksplwrapper-1.0.2/splunksplwrapper/manager/users/__init__.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/manager/users/sdk/__init__.py` & `splunksplwrapper-1.0.2/splunksplwrapper/manager/users/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/manager/users/sdk/user.py` & `splunksplwrapper-1.0.2/splunksplwrapper/manager/users/sdk/user.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/manager/users/user.py` & `splunksplwrapper-1.0.2/splunksplwrapper/manager/users/user.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/misc/__init__.py` & `splunksplwrapper-1.0.2/splunksplwrapper/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/misc/collection.py` & `splunksplwrapper-1.0.2/splunksplwrapper/misc/collection.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/misc/manager_utils.py` & `splunksplwrapper-1.0.2/splunksplwrapper/misc/manager_utils.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/splunk/__init__.py` & `splunksplwrapper-1.0.2/splunksplwrapper/splunk/__init__.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/splunk/base.py` & `splunksplwrapper-1.0.2/splunksplwrapper/splunk/base.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/splunk/cloud.py` & `splunksplwrapper-1.0.2/splunksplwrapper/splunk/cloud.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/util/Constants.py` & `splunksplwrapper-1.0.2/splunksplwrapper/util/Constants.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/util/__init__.py` & `splunksplwrapper-1.0.2/splunksplwrapper/util/__init__.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/util/action_writer.py` & `splunksplwrapper-1.0.2/splunksplwrapper/util/action_writer.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/util/attrdict.py` & `splunksplwrapper-1.0.2/splunksplwrapper/util/attrdict.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/util/basefileutils.py` & `splunksplwrapper-1.0.2/splunksplwrapper/util/basefileutils.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/util/rest_uris.py` & `splunksplwrapper-1.0.2/splunksplwrapper/util/rest_uris.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/util/restutils.py` & `splunksplwrapper-1.0.2/splunksplwrapper/util/restutils.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/util/rip.py` & `splunksplwrapper-1.0.2/splunksplwrapper/util/rip.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/util/searchhelpers.py` & `splunksplwrapper-1.0.2/splunksplwrapper/util/searchhelpers.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/splunksplwrapper/util/string_unicode_convert.py` & `splunksplwrapper-1.0.2/splunksplwrapper/util/string_unicode_convert.py`

 * *Files identical despite different names*

### Comparing `splunksplwrapper-1.0.1/PKG-INFO` & `splunksplwrapper-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: splunksplwrapper
-Version: 1.0.1
+Version: 1.0.2
 Summary: Package to interact with Splunk
 License: Apache-2.0
 Author: Splunk
 Author-email: addonfactory@splunk.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
 Requires-Dist: httplib2 (>=0.21.0,<0.22.0)
-Requires-Dist: splunk-sdk (>=1.6.18,<2.0.0)
+Requires-Dist: splunk-sdk (>=1.6)
```

