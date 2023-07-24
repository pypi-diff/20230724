# Comparing `tmp/openi-beta-0.1.8.tar.gz` & `tmp/openi-beta-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openi-beta-0.1.8.tar", last modified: Tue Jun 20 01:20:28 2023, max compression
+gzip compressed data, was "openi-beta-2.0.0.tar", last modified: Mon Jul 24 07:23:28 2023, max compression
```

## Comparing `openi-beta-0.1.8.tar` & `openi-beta-2.0.0.tar`

### file list

```diff
@@ -1,22 +1,39 @@
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-20 01:20:28.242139 openi-beta-0.1.8/
--rw-r--r--   0 jochen10518   (501) staff       (20)     2102 2023-06-20 01:20:28.241989 openi-beta-0.1.8/PKG-INFO
--rw-r--r--   0 jochen10518   (501) staff       (20)     1473 2023-06-20 01:19:17.000000 openi-beta-0.1.8/README.md
--rw-r--r--   0 jochen10518   (501) staff       (20)       38 2023-06-20 01:20:28.242197 openi-beta-0.1.8/setup.cfg
--rw-r--r--   0 jochen10518   (501) staff       (20)     1145 2023-06-20 01:19:36.000000 openi-beta-0.1.8/setup.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-20 01:20:28.239147 openi-beta-0.1.8/src/
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-20 01:20:28.239818 openi-beta-0.1.8/src/openi/
--rw-r--r--   0 jochen10518   (501) staff       (20)       48 2023-06-20 01:19:17.000000 openi-beta-0.1.8/src/openi/__init__.py
--rw-r--r--   0 jochen10518   (501) staff       (20)      356 2023-06-20 01:19:17.000000 openi-beta-0.1.8/src/openi/constants.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-20 01:20:28.240114 openi-beta-0.1.8/src/openi/dataset/
--rw-r--r--   0 jochen10518   (501) staff       (20)       22 2023-06-20 01:19:17.000000 openi-beta-0.1.8/src/openi/dataset/__init__.py
--rw-r--r--   0 jochen10518   (501) staff       (20)    12772 2023-06-20 01:19:50.000000 openi-beta-0.1.8/src/openi/dataset/dataset.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-20 01:20:28.240256 openi-beta-0.1.8/src/openi/utils/
--rw-r--r--   0 jochen10518   (501) staff       (20)      419 2023-06-20 01:19:17.000000 openi-beta-0.1.8/src/openi/utils/logger.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-20 01:20:28.241592 openi-beta-0.1.8/src/openi_beta.egg-info/
--rw-r--r--   0 jochen10518   (501) staff       (20)     2102 2023-06-20 01:20:28.000000 openi-beta-0.1.8/src/openi_beta.egg-info/PKG-INFO
--rw-r--r--   0 jochen10518   (501) staff       (20)      363 2023-06-20 01:20:28.000000 openi-beta-0.1.8/src/openi_beta.egg-info/SOURCES.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)        1 2023-06-20 01:20:28.000000 openi-beta-0.1.8/src/openi_beta.egg-info/dependency_links.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)       14 2023-06-20 01:20:28.000000 openi-beta-0.1.8/src/openi_beta.egg-info/requires.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)        6 2023-06-20 01:20:28.000000 openi-beta-0.1.8/src/openi_beta.egg-info/top_level.txt
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-20 01:20:28.241767 openi-beta-0.1.8/test/
--rw-r--r--   0 jochen10518   (501) staff       (20)      627 2023-06-20 01:19:17.000000 openi-beta-0.1.8/test/test_upload_multi.py
+drwxrwxrwx   0        0        0        0 2023-07-24 07:23:28.340349 openi-beta-2.0.0/
+-rw-rw-rw-   0        0        0     5377 2023-07-24 07:23:28.339331 openi-beta-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4731 2023-07-24 07:01:34.000000 openi-beta-2.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-24 07:23:28.340349 openi-beta-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1290 2023-07-24 07:23:14.000000 openi-beta-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 07:23:28.288322 openi-beta-2.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-24 07:23:28.295768 openi-beta-2.0.0/src/openi/
+-rw-rw-rw-   0        0        0      194 2023-07-24 07:15:17.000000 openi-beta-2.0.0/src/openi/__init__.py
+-rw-rw-rw-   0        0        0     6459 2023-07-24 07:13:05.000000 openi-beta-2.0.0/src/openi/apis.py
+-rw-rw-rw-   0        0        0     5238 2023-07-24 07:13:04.000000 openi-beta-2.0.0/src/openi/cli.py
+drwxrwxrwx   0        0        0        0 2023-07-24 07:23:28.300292 openi-beta-2.0.0/src/openi/cloudbrain/
+-rw-rw-rw-   0        0        0       84 2023-07-24 07:06:23.000000 openi-beta-2.0.0/src/openi/cloudbrain/__init__.py
+-rw-rw-rw-   0        0        0     1609 2023-07-24 07:06:26.000000 openi-beta-2.0.0/src/openi/cloudbrain/env_check.py
+-rw-rw-rw-   0        0        0     5313 2023-07-24 07:06:29.000000 openi-beta-2.0.0/src/openi/cloudbrain/helper.py
+-rw-rw-rw-   0        0        0     1559 2023-07-24 07:06:31.000000 openi-beta-2.0.0/src/openi/cloudbrain/minio_operate.py
+-rw-rw-rw-   0        0        0     2886 2023-07-24 07:06:32.000000 openi-beta-2.0.0/src/openi/cloudbrain/obs_operate.py
+drwxrwxrwx   0        0        0        0 2023-07-24 07:23:28.303086 openi-beta-2.0.0/src/openi/dataset/
+-rw-rw-rw-   0        0        0      109 2023-07-24 07:06:34.000000 openi-beta-2.0.0/src/openi/dataset/__init__.py
+-rw-rw-rw-   0        0        0     2855 2023-07-24 07:06:35.000000 openi-beta-2.0.0/src/openi/dataset/dataset_file.py
+-rw-rw-rw-   0        0        0     2685 2023-07-24 07:20:32.000000 openi-beta-2.0.0/src/openi/dataset/download.py
+-rw-rw-rw-   0        0        0     4592 2023-07-24 07:08:01.000000 openi-beta-2.0.0/src/openi/dataset/upload.py
+-rw-rw-rw-   0        0        0     3356 2023-07-24 07:13:03.000000 openi-beta-2.0.0/src/openi/login.py
+drwxrwxrwx   0        0        0        0 2023-07-24 07:23:28.304085 openi-beta-2.0.0/src/openi/path/
+-rw-rw-rw-   0        0        0       21 2023-07-24 07:06:52.000000 openi-beta-2.0.0/src/openi/path/__init__.py
+-rw-rw-rw-   0        0        0     2405 2023-07-24 07:07:00.000000 openi-beta-2.0.0/src/openi/path/path.py
+-rw-rw-rw-   0        0        0     4081 2023-07-24 07:13:02.000000 openi-beta-2.0.0/src/openi/settings.py
+drwxrwxrwx   0        0        0        0 2023-07-24 07:23:28.325091 openi-beta-2.0.0/src/openi/utils/
+-rw-rw-rw-   0        0        0       50 2023-07-24 07:07:03.000000 openi-beta-2.0.0/src/openi/utils/__init__.py
+-rw-rw-rw-   0        0        0     2197 2023-07-24 07:07:05.000000 openi-beta-2.0.0/src/openi/utils/file_utils.py
+-rw-rw-rw-   0        0        0      723 2023-07-24 07:07:16.000000 openi-beta-2.0.0/src/openi/utils/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-24 07:23:28.338332 openi-beta-2.0.0/src/openi_beta.egg-info/
+-rw-rw-rw-   0        0        0     5377 2023-07-24 07:23:28.000000 openi-beta-2.0.0/src/openi_beta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      787 2023-07-24 07:23:28.000000 openi-beta-2.0.0/src/openi_beta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 07:23:28.000000 openi-beta-2.0.0/src/openi_beta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-07-24 07:23:28.000000 openi-beta-2.0.0/src/openi_beta.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-07-24 07:23:28.000000 openi-beta-2.0.0/src/openi_beta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-24 07:23:28.000000 openi-beta-2.0.0/src/openi_beta.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 07:23:28.339331 openi-beta-2.0.0/test/
+-rw-rw-rw-   0        0        0      199 2023-07-24 04:14:29.000000 openi-beta-2.0.0/test/test.py
```

