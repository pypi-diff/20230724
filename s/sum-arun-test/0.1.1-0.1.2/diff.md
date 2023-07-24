# Comparing `tmp/sum_arun_test-0.1.1.tar.gz` & `tmp/sum_arun_test-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sum_arun_test-0.1.1.tar", last modified: Mon Jul 24 06:09:29 2023, max compression
+gzip compressed data, was "sum_arun_test-0.1.2.tar", last modified: Mon Jul 24 06:31:32 2023, max compression
```

## Comparing `sum_arun_test-0.1.1.tar` & `sum_arun_test-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 06:09:29.347165 sum_arun_test-0.1.1/
--rw-rw-rw-   0        0        0      118 2023-07-24 06:09:29.341170 sum_arun_test-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-24 06:09:29.347165 sum_arun_test-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      212 2023-07-24 06:08:44.000000 sum_arun_test-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-24 06:09:29.327164 sum_arun_test-0.1.1/sum_arun_test.egg-info/
--rw-rw-rw-   0        0        0      118 2023-07-24 06:09:29.000000 sum_arun_test-0.1.1/sum_arun_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2023-07-24 06:09:29.000000 sum_arun_test-0.1.1/sum_arun_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 06:09:29.000000 sum_arun_test-0.1.1/sum_arun_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-24 06:09:29.000000 sum_arun_test-0.1.1/sum_arun_test.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-24 06:09:29.336166 sum_arun_test-0.1.1/test_sdk/
--rw-rw-rw-   0        0        0       69 2023-07-24 06:08:00.000000 sum_arun_test-0.1.1/test_sdk/__init__.py
--rw-rw-rw-   0        0        0       89 2023-07-24 05:51:47.000000 sum_arun_test-0.1.1/test_sdk/sum_arun_test.py
+drwxrwxrwx   0        0        0        0 2023-07-24 06:31:32.583239 sum_arun_test-0.1.2/
+-rw-rw-rw-   0        0        0      118 2023-07-24 06:31:32.582249 sum_arun_test-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-24 06:31:32.584246 sum_arun_test-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      212 2023-07-24 06:31:18.000000 sum_arun_test-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 06:31:32.563235 sum_arun_test-0.1.2/sum_arun_test.egg-info/
+-rw-rw-rw-   0        0        0      118 2023-07-24 06:31:32.000000 sum_arun_test-0.1.2/sum_arun_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-07-24 06:31:32.000000 sum_arun_test-0.1.2/sum_arun_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 06:31:32.000000 sum_arun_test-0.1.2/sum_arun_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-24 06:31:32.000000 sum_arun_test-0.1.2/sum_arun_test.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 06:31:32.577233 sum_arun_test-0.1.2/test_sdk/
+-rw-rw-rw-   0        0        0      137 2023-07-24 06:31:17.000000 sum_arun_test-0.1.2/test_sdk/__init__.py
+-rw-rw-rw-   0        0        0       89 2023-07-24 05:51:47.000000 sum_arun_test-0.1.2/test_sdk/sum_arun_test.py
+-rw-rw-rw-   0        0        0      153 2023-07-24 06:31:18.000000 sum_arun_test-0.1.2/test_sdk/test_functions.py
```

