# Comparing `tmp/m-abac-1.0.3.tar.gz` & `tmp/m-abac-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m-abac-1.0.3.tar", last modified: Thu Jul 20 01:36:16 2023, max compression
+gzip compressed data, was "m-abac-1.0.4.tar", last modified: Mon Jul 24 07:10:05 2023, max compression
```

## Comparing `m-abac-1.0.3.tar` & `m-abac-1.0.4.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 01:36:16.763303 m-abac-1.0.3/
--rw-r--r--   0 root         (0) root         (0)     1550 2023-07-20 01:36:16.762303 m-abac-1.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      659 2023-07-17 15:45:49.000000 m-abac-1.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 01:36:16.705302 m-abac-1.0.3/m_abac.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1550 2023-07-20 01:36:16.000000 m-abac-1.0.3/m_abac.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4095 2023-07-20 01:36:16.000000 m-abac-1.0.3/m_abac.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 01:36:16.000000 m-abac-1.0.3/m_abac.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      115 2023-07-20 01:36:16.000000 m-abac-1.0.3/m_abac.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-07-20 01:36:16.000000 m-abac-1.0.3/m_abac.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 01:36:16.694301 m-abac-1.0.3/mobio/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 01:36:16.694301 m-abac-1.0.3/mobio/libs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 01:36:16.709302 m-abac-1.0.3/mobio/libs/abac/
--rw-r--r--   0 root         (0) root         (0)       70 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 01:36:16.712302 m-abac-1.0.3/mobio/libs/abac/adapter/
--rw-r--r--   0 root         (0) root         (0)      267 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/adapter/__init__.py
--rw-r--r--   0 root         (0) root         (0)      435 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/adapter/adapter.py
--rw-r--r--   0 root         (0) root         (0)    21622 2023-07-20 01:33:02.000000 m-abac-1.0.3/mobio/libs/abac/adapter/elasticsearch_adapter.py
--rw-r--r--   0 root         (0) root         (0)     7687 2023-07-20 01:33:02.000000 m-abac-1.0.3/mobio/libs/abac/call_api.py
--rw-r--r--   0 root         (0) root         (0)     3531 2023-07-20 01:33:02.000000 m-abac-1.0.3/mobio/libs/abac/config.py
--rw-r--r--   0 root         (0) root         (0)    22064 2023-07-20 01:33:02.000000 m-abac-1.0.3/mobio/libs/abac/pdp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 01:36:16.715302 m-abac-1.0.3/mobio/libs/abac/policy/
--rw-r--r--   0 root         (0) root         (0)       44 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 01:36:16.718302 m-abac-1.0.3/mobio/libs/abac/policy/conditions/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      715 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 01:36:16.720302 m-abac-1.0.3/mobio/libs/abac/policy/conditions/boolean/
--rw-r--r--   0 root         (0) root         (0)       39 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/boolean/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1127 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/boolean/base.py
--rw-r--r--   0 root         (0) root         (0)     1107 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/boolean/check_bool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 01:36:16.730302 m-abac-1.0.3/mobio/libs/abac/policy/conditions/collection/
--rw-r--r--   0 root         (0) root         (0)      418 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/collection/__init__.py
--rw-r--r--   0 root         (0) root         (0)      680 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/collection/all_in.py
--rw-r--r--   0 root         (0) root         (0)      705 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/collection/all_not_in.py
--rw-r--r--   0 root         (0) root         (0)      742 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/collection/any_contains.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/collection/any_in.py
--rw-r--r--   0 root         (0) root         (0)      755 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/collection/any_not_contains.py
--rw-r--r--   0 root         (0) root         (0)      715 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/collection/any_not_in.py
--rw-r--r--   0 root         (0) root         (0)     1341 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/collection/base.py
--rw-r--r--   0 root         (0) root         (0)      754 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/collection/is_empty.py
--rw-r--r--   0 root         (0) root         (0)      602 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/collection/is_in.py
--rw-r--r--   0 root         (0) root         (0)      774 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/collection/is_not_empty.py
--rw-r--r--   0 root         (0) root         (0)      728 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/collection/is_not_in.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 01:36:16.736302 m-abac-1.0.3/mobio/libs/abac/policy/conditions/date_time/
--rw-r--r--   0 root         (0) root         (0)      243 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/date_time/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2649 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/date_time/base.py
--rw-r--r--   0 root         (0) root         (0)     1261 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/date_time/date_eq.py
--rw-r--r--   0 root         (0) root         (0)     1283 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/date_time/date_gt.py
--rw-r--r--   0 root         (0) root         (0)     1305 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/date_time/date_gte.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/date_time/date_lt.py
--rw-r--r--   0 root         (0) root         (0)     1296 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/date_time/date_lte.py
--rw-r--r--   0 root         (0) root         (0)     1279 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/date_time/date_neq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 01:36:16.741303 m-abac-1.0.3/mobio/libs/abac/policy/conditions/day/
--rw-r--r--   0 root         (0) root         (0)      197 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/day/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2788 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/day/base.py
--rw-r--r--   0 root         (0) root         (0)     1050 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/day/day_eq.py
--rw-r--r--   0 root         (0) root         (0)      937 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/day/day_gt.py
--rw-r--r--   0 root         (0) root         (0)      939 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/day/day_gte.py
--rw-r--r--   0 root         (0) root         (0)      936 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/day/day_lt.py
--rw-r--r--   0 root         (0) root         (0)      939 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/day/day_lte.py
--rw-r--r--   0 root         (0) root         (0)      940 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/day/day_neq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 01:36:16.744303 m-abac-1.0.3/mobio/libs/abac/policy/conditions/ip_address/
--rw-r--r--   0 root         (0) root         (0)       82 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/ip_address/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1691 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/ip_address/base.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py
--rw-r--r--   0 root         (0) root         (0)      746 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 01:36:16.752303 m-abac-1.0.3/mobio/libs/abac/policy/conditions/numeric/
--rw-r--r--   0 root         (0) root         (0)      328 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/numeric/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1451 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/numeric/base.py
--rw-r--r--   0 root         (0) root         (0)     1559 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/numeric/base_list.py
--rw-r--r--   0 root         (0) root         (0)      853 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/numeric/eq.py
--rw-r--r--   0 root         (0) root         (0)      871 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/numeric/gt.py
--rw-r--r--   0 root         (0) root         (0)      895 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/numeric/gte.py
--rw-r--r--   0 root         (0) root         (0)      976 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/numeric/list_gt.py
--rw-r--r--   0 root         (0) root         (0)      979 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/numeric/list_gte.py
--rw-r--r--   0 root         (0) root         (0)      976 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/numeric/list_lt.py
--rw-r--r--   0 root         (0) root         (0)      979 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/numeric/list_lte.py
--rw-r--r--   0 root         (0) root         (0)      863 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/numeric/lt.py
--rw-r--r--   0 root         (0) root         (0)      886 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/numeric/lte.py
--rw-r--r--   0 root         (0) root         (0)      869 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/numeric/neq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 01:36:16.755303 m-abac-1.0.3/mobio/libs/abac/policy/conditions/others/
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/others/__init__.py
--rw-r--r--   0 root         (0) root         (0)      963 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/others/base.py
--rw-r--r--   0 root         (0) root         (0)      690 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/others/exists.py
--rw-r--r--   0 root         (0) root         (0)      702 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/others/not_exists.py
--rw-r--r--   0 root         (0) root         (0)     2425 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 01:36:16.762303 m-abac-1.0.3/mobio/libs/abac/policy/conditions/string/
--rw-r--r--   0 root         (0) root         (0)      401 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/string/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1633 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/string/base.py
--rw-r--r--   0 root         (0) root         (0)     2326 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/string/contains.py
--rw-r--r--   0 root         (0) root         (0)     2229 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/string/ends_with.py
--rw-r--r--   0 root         (0) root         (0)     1203 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/string/equals.py
--rw-r--r--   0 root         (0) root         (0)     2059 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/string/not_contains.py
--rw-r--r--   0 root         (0) root         (0)     2111 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/string/not_ends_with.py
--rw-r--r--   0 root         (0) root         (0)     1215 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/string/not_equals.py
--rw-r--r--   0 root         (0) root         (0)     2138 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/string/not_starts_with.py
--rw-r--r--   0 root         (0) root         (0)     1498 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/string/regex_match.py
--rw-r--r--   0 root         (0) root         (0)     2256 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/conditions/string/starts_with.py
--rw-r--r--   0 root         (0) root         (0)     1601 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     7259 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/policy.py
--rw-r--r--   0 root         (0) root         (0)     6433 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/policy/utils.py
--rw-r--r--   0 root         (0) root         (0)     6499 2023-07-17 15:45:49.000000 m-abac-1.0.3/mobio/libs/abac/result_access.py
--rw-r--r--   0 root         (0) root         (0)      104 2023-07-17 15:45:49.000000 m-abac-1.0.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 01:36:16.763303 m-abac-1.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     9805 2023-07-20 01:36:16.000000 m-abac-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:10:05.406330 m-abac-1.0.4/
+-rw-r--r--   0 root         (0) root         (0)     1550 2023-07-24 07:10:05.406330 m-abac-1.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      659 2023-07-17 15:45:49.000000 m-abac-1.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:10:05.350329 m-abac-1.0.4/m_abac.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1550 2023-07-24 07:10:05.000000 m-abac-1.0.4/m_abac.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4095 2023-07-24 07:10:05.000000 m-abac-1.0.4/m_abac.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 07:10:05.000000 m-abac-1.0.4/m_abac.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      115 2023-07-24 07:10:05.000000 m-abac-1.0.4/m_abac.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-07-24 07:10:05.000000 m-abac-1.0.4/m_abac.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:10:05.340329 m-abac-1.0.4/mobio/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:10:05.341329 m-abac-1.0.4/mobio/libs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:10:05.354329 m-abac-1.0.4/mobio/libs/abac/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:10:05.356329 m-abac-1.0.4/mobio/libs/abac/adapter/
+-rw-r--r--   0 root         (0) root         (0)      267 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/adapter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      435 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/adapter/adapter.py
+-rw-r--r--   0 root         (0) root         (0)    21622 2023-07-20 01:33:02.000000 m-abac-1.0.4/mobio/libs/abac/adapter/elasticsearch_adapter.py
+-rw-r--r--   0 root         (0) root         (0)     7706 2023-07-24 07:08:08.000000 m-abac-1.0.4/mobio/libs/abac/call_api.py
+-rw-r--r--   0 root         (0) root         (0)     3531 2023-07-20 01:33:02.000000 m-abac-1.0.4/mobio/libs/abac/config.py
+-rw-r--r--   0 root         (0) root         (0)    22064 2023-07-20 01:33:02.000000 m-abac-1.0.4/mobio/libs/abac/pdp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:10:05.359329 m-abac-1.0.4/mobio/libs/abac/policy/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:10:05.361329 m-abac-1.0.4/mobio/libs/abac/policy/conditions/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      715 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:10:05.363329 m-abac-1.0.4/mobio/libs/abac/policy/conditions/boolean/
+-rw-r--r--   0 root         (0) root         (0)       39 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/boolean/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1127 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/boolean/base.py
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/boolean/check_bool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:10:05.371329 m-abac-1.0.4/mobio/libs/abac/policy/conditions/collection/
+-rw-r--r--   0 root         (0) root         (0)      418 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/collection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      680 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/collection/all_in.py
+-rw-r--r--   0 root         (0) root         (0)      705 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/collection/all_not_in.py
+-rw-r--r--   0 root         (0) root         (0)      742 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/collection/any_contains.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/collection/any_in.py
+-rw-r--r--   0 root         (0) root         (0)      755 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/collection/any_not_contains.py
+-rw-r--r--   0 root         (0) root         (0)      715 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/collection/any_not_in.py
+-rw-r--r--   0 root         (0) root         (0)     1341 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/collection/base.py
+-rw-r--r--   0 root         (0) root         (0)      754 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/collection/is_empty.py
+-rw-r--r--   0 root         (0) root         (0)      602 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/collection/is_in.py
+-rw-r--r--   0 root         (0) root         (0)      774 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/collection/is_not_empty.py
+-rw-r--r--   0 root         (0) root         (0)      728 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/collection/is_not_in.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:10:05.377330 m-abac-1.0.4/mobio/libs/abac/policy/conditions/date_time/
+-rw-r--r--   0 root         (0) root         (0)      243 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/date_time/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2649 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/date_time/base.py
+-rw-r--r--   0 root         (0) root         (0)     1261 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_eq.py
+-rw-r--r--   0 root         (0) root         (0)     1283 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_gt.py
+-rw-r--r--   0 root         (0) root         (0)     1305 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_gte.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_lt.py
+-rw-r--r--   0 root         (0) root         (0)     1296 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_lte.py
+-rw-r--r--   0 root         (0) root         (0)     1279 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_neq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:10:05.383330 m-abac-1.0.4/mobio/libs/abac/policy/conditions/day/
+-rw-r--r--   0 root         (0) root         (0)      197 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/day/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2788 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/day/base.py
+-rw-r--r--   0 root         (0) root         (0)     1050 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/day/day_eq.py
+-rw-r--r--   0 root         (0) root         (0)      937 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/day/day_gt.py
+-rw-r--r--   0 root         (0) root         (0)      939 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/day/day_gte.py
+-rw-r--r--   0 root         (0) root         (0)      936 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/day/day_lt.py
+-rw-r--r--   0 root         (0) root         (0)      939 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/day/day_lte.py
+-rw-r--r--   0 root         (0) root         (0)      940 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/day/day_neq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:10:05.386330 m-abac-1.0.4/mobio/libs/abac/policy/conditions/ip_address/
+-rw-r--r--   0 root         (0) root         (0)       82 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/ip_address/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/ip_address/base.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py
+-rw-r--r--   0 root         (0) root         (0)      746 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:10:05.396330 m-abac-1.0.4/mobio/libs/abac/policy/conditions/numeric/
+-rw-r--r--   0 root         (0) root         (0)      328 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/numeric/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/numeric/base.py
+-rw-r--r--   0 root         (0) root         (0)     1559 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/numeric/base_list.py
+-rw-r--r--   0 root         (0) root         (0)      853 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/numeric/eq.py
+-rw-r--r--   0 root         (0) root         (0)      871 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/numeric/gt.py
+-rw-r--r--   0 root         (0) root         (0)      895 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/numeric/gte.py
+-rw-r--r--   0 root         (0) root         (0)      976 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/numeric/list_gt.py
+-rw-r--r--   0 root         (0) root         (0)      979 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/numeric/list_gte.py
+-rw-r--r--   0 root         (0) root         (0)      976 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/numeric/list_lt.py
+-rw-r--r--   0 root         (0) root         (0)      979 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/numeric/list_lte.py
+-rw-r--r--   0 root         (0) root         (0)      863 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/numeric/lt.py
+-rw-r--r--   0 root         (0) root         (0)      886 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/numeric/lte.py
+-rw-r--r--   0 root         (0) root         (0)      869 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/numeric/neq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:10:05.398330 m-abac-1.0.4/mobio/libs/abac/policy/conditions/others/
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/others/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      963 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/others/base.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/others/exists.py
+-rw-r--r--   0 root         (0) root         (0)      702 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/others/not_exists.py
+-rw-r--r--   0 root         (0) root         (0)     2425 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:10:05.405330 m-abac-1.0.4/mobio/libs/abac/policy/conditions/string/
+-rw-r--r--   0 root         (0) root         (0)      401 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/string/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1633 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/string/base.py
+-rw-r--r--   0 root         (0) root         (0)     2326 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/string/contains.py
+-rw-r--r--   0 root         (0) root         (0)     2229 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/string/ends_with.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/string/equals.py
+-rw-r--r--   0 root         (0) root         (0)     2059 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/string/not_contains.py
+-rw-r--r--   0 root         (0) root         (0)     2111 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/string/not_ends_with.py
+-rw-r--r--   0 root         (0) root         (0)     1215 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/string/not_equals.py
+-rw-r--r--   0 root         (0) root         (0)     2138 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/string/not_starts_with.py
+-rw-r--r--   0 root         (0) root         (0)     1498 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/string/regex_match.py
+-rw-r--r--   0 root         (0) root         (0)     2256 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/conditions/string/starts_with.py
+-rw-r--r--   0 root         (0) root         (0)     1601 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     7259 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/policy.py
+-rw-r--r--   0 root         (0) root         (0)     6433 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/policy/utils.py
+-rw-r--r--   0 root         (0) root         (0)     6499 2023-07-17 15:45:49.000000 m-abac-1.0.4/mobio/libs/abac/result_access.py
+-rw-r--r--   0 root         (0) root         (0)      104 2023-07-17 15:45:49.000000 m-abac-1.0.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 07:10:05.406330 m-abac-1.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     9805 2023-07-24 07:10:04.000000 m-abac-1.0.4/setup.py
```

### Comparing `m-abac-1.0.3/PKG-INFO` & `m-abac-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m-abac
-Version: 1.0.3
+Version: 1.0.4
 Summary: Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Keywords: mobio,mobio-engine,m-abac
```

### Comparing `m-abac-1.0.3/README.md` & `m-abac-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/m_abac.egg-info/PKG-INFO` & `m-abac-1.0.4/m_abac.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m-abac
-Version: 1.0.3
+Version: 1.0.4
 Summary: Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Keywords: mobio,mobio-engine,m-abac
```

### Comparing `m-abac-1.0.3/m_abac.egg-info/SOURCES.txt` & `m-abac-1.0.4/m_abac.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/adapter/elasticsearch_adapter.py` & `m-abac-1.0.4/mobio/libs/abac/adapter/elasticsearch_adapter.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/call_api.py` & `m-abac-1.0.4/mobio/libs/abac/call_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 class APIRequest:
     TimeOut = 10
     ADMIN_GET_FULL_INFO_ACCOUNT = "{domain}/adm/api/v2.1/accounts/{account_id}/full-info"
     ADMIN_GET_LIST_ACTION_FOR_MERCHANT = "{domain}/adm/api/v2.1/policies/actions/sdk"
     ADMIN_GET_LIST_STATEMENT = "{domain}/adm/api/v2.1/statements"
 
 
-_TIME_CACHE = 600 if Mobio.VM_TYPE and Mobio.VM_TYPE != "TEST" else 60
+# _TIME_CACHE = 600 if Mobio.VM_TYPE and Mobio.VM_TYPE != "TEST" else 60
+_TIME_CACHE = 60
 
 
 class CallAPI:
 
     # TODO: thay expiration cho production
     @staticmethod
     @lru_cache_redis.add(expiration=_TIME_CACHE)
```

### Comparing `m-abac-1.0.3/mobio/libs/abac/config.py` & `m-abac-1.0.4/mobio/libs/abac/config.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/pdp.py` & `m-abac-1.0.4/mobio/libs/abac/pdp.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/base.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/boolean/base.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/boolean/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/boolean/check_bool.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/boolean/check_bool.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/collection/all_in.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/collection/all_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/collection/all_not_in.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/collection/all_not_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/collection/any_contains.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/collection/any_contains.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/collection/any_in.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/collection/any_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/collection/any_not_contains.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/collection/any_not_contains.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/collection/any_not_in.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/collection/any_not_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/collection/base.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/collection/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/collection/is_empty.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/collection/is_empty.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/collection/is_in.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/collection/is_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/collection/is_not_empty.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/collection/is_not_empty.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/collection/is_not_in.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/collection/is_not_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/date_time/base.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/date_time/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/date_time/date_eq.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_eq.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/date_time/date_gt.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_gt.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/date_time/date_gte.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_gte.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/date_time/date_lt.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_lt.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/date_time/date_lte.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_lte.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/date_time/date_neq.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_neq.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/day/base.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/day/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/day/day_eq.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/day/day_eq.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/day/day_gt.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/day/day_gt.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/day/day_gte.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/day/day_gte.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/day/day_lt.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/day/day_lt.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/day/day_lte.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/day/day_lte.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/day/day_neq.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/day/day_neq.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/ip_address/base.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/ip_address/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/numeric/base.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/numeric/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/numeric/base_list.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/numeric/base_list.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/numeric/eq.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/numeric/eq.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/numeric/gt.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/numeric/gt.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/numeric/gte.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/numeric/gte.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/numeric/list_gt.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/numeric/list_gt.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/numeric/list_gte.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/numeric/list_gte.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/numeric/list_lt.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/numeric/list_lt.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/numeric/list_lte.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/numeric/list_lte.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/numeric/lt.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/numeric/lt.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/numeric/lte.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/numeric/lte.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/numeric/neq.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/numeric/neq.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/others/base.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/others/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/others/exists.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/others/exists.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/others/not_exists.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/others/not_exists.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/schema.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/schema.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/string/base.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/string/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/string/contains.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/string/contains.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/string/ends_with.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/string/ends_with.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/string/equals.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/string/equals.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/string/not_contains.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/string/not_contains.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/string/not_ends_with.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/string/not_ends_with.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/string/not_equals.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/string/not_equals.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/string/not_starts_with.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/string/not_starts_with.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/string/regex_match.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/string/regex_match.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/conditions/string/starts_with.py` & `m-abac-1.0.4/mobio/libs/abac/policy/conditions/string/starts_with.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/exceptions.py` & `m-abac-1.0.4/mobio/libs/abac/policy/exceptions.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/policy.py` & `m-abac-1.0.4/mobio/libs/abac/policy/policy.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/policy/utils.py` & `m-abac-1.0.4/mobio/libs/abac/policy/utils.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/mobio/libs/abac/result_access.py` & `m-abac-1.0.4/mobio/libs/abac/result_access.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.3/setup.py` & `m-abac-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         # with open(Requirements.requirements_path) as req_file:
         #     for line in req_file.read().splitlines():
         #         if not line.strip().startswith("#"):
         #             requirements.append(line)
         return requirements
 
 version_dev='1.0.34'
-version_prod='1.0.3'
+version_prod='1.0.4'
 
 run_mode=''
 
 setup(
     # This is the name of your project. The first time you publish this
     # package, this name will be registered for you. It will determine how
     # users can install this project, e.g.:
@@ -71,15 +71,15 @@
     # options={"bdist_wheel": {"universal": True}},
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.0.3',  # Required
+    version='1.0.4',  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

