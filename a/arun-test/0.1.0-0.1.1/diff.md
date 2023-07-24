# Comparing `tmp/arun_test-0.1.0.tar.gz` & `tmp/arun_test-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arun_test-0.1.0.tar", last modified: Mon Jul 24 06:46:33 2023, max compression
+gzip compressed data, was "arun_test-0.1.1.tar", last modified: Mon Jul 24 06:55:08 2023, max compression
```

## Comparing `arun_test-0.1.0.tar` & `arun_test-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 06:46:33.007669 arun_test-0.1.0/
--rw-rw-rw-   0        0        0      114 2023-07-24 06:46:33.006610 arun_test-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-24 06:46:32.988245 arun_test-0.1.0/arun_test.egg-info/
--rw-rw-rw-   0        0        0      114 2023-07-24 06:46:32.000000 arun_test-0.1.0/arun_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2023-07-24 06:46:32.000000 arun_test-0.1.0/arun_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 06:46:32.000000 arun_test-0.1.0/arun_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-24 06:46:32.000000 arun_test-0.1.0/arun_test.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 06:46:33.008610 arun_test-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      208 2023-07-24 06:44:27.000000 arun_test-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-24 06:46:33.001609 arun_test-0.1.0/test_sdk/
--rw-rw-rw-   0        0        0      137 2023-07-24 06:31:17.000000 arun_test-0.1.0/test_sdk/__init__.py
--rw-rw-rw-   0        0        0       89 2023-07-24 05:51:47.000000 arun_test-0.1.0/test_sdk/sum_arun_test.py
--rw-rw-rw-   0        0        0      153 2023-07-24 06:31:18.000000 arun_test-0.1.0/test_sdk/test_functions.py
+drwxrwxrwx   0        0        0        0 2023-07-24 06:55:08.166394 arun_test-0.1.1/
+-rw-rw-rw-   0        0        0      267 2023-07-24 06:55:08.164389 arun_test-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-24 06:55:08.147390 arun_test-0.1.1/arun_test.egg-info/
+-rw-rw-rw-   0        0        0      267 2023-07-24 06:55:08.000000 arun_test-0.1.1/arun_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2023-07-24 06:55:08.000000 arun_test-0.1.1/arun_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 06:55:08.000000 arun_test-0.1.1/arun_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-24 06:55:08.000000 arun_test-0.1.1/arun_test.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      398 2023-07-24 06:54:38.000000 arun_test-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-24 06:55:08.166394 arun_test-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-24 06:55:08.160391 arun_test-0.1.1/test_sdk/
+-rw-rw-rw-   0        0        0      137 2023-07-24 06:31:17.000000 arun_test-0.1.1/test_sdk/__init__.py
+-rw-rw-rw-   0        0        0       89 2023-07-24 05:51:47.000000 arun_test-0.1.1/test_sdk/sum_arun_test.py
+-rw-rw-rw-   0        0        0      153 2023-07-24 06:31:18.000000 arun_test-0.1.1/test_sdk/test_functions.py
```

