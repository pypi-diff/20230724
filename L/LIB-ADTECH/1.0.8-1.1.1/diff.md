# Comparing `tmp/LIB-ADTECH-1.0.8.tar.gz` & `tmp/LIB-ADTECH-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LIB-ADTECH-1.0.8.tar", last modified: Fri Jul  7 14:19:13 2023, max compression
+gzip compressed data, was "LIB-ADTECH-1.1.1.tar", last modified: Mon Jul 24 14:10:57 2023, max compression
```

## Comparing `LIB-ADTECH-1.0.8.tar` & `LIB-ADTECH-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 14:19:13.899542 LIB-ADTECH-1.0.8/
-drwxrwxrwx   0        0        0        0 2023-07-07 14:19:13.863346 LIB-ADTECH-1.0.8/Adlib/
--rw-rw-rw-   0        0        0       26 2023-07-07 12:20:05.000000 LIB-ADTECH-1.0.8/Adlib/__ini__.py
--rw-rw-rw-   0        0        0     3640 2023-07-07 14:13:34.000000 LIB-ADTECH-1.0.8/Adlib/funcoes.py
-drwxrwxrwx   0        0        0        0 2023-07-07 14:19:13.895099 LIB-ADTECH-1.0.8/LIB_ADTECH.egg-info/
--rw-rw-rw-   0        0        0      313 2023-07-07 14:19:13.000000 LIB-ADTECH-1.0.8/LIB_ADTECH.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-07-07 14:19:13.000000 LIB-ADTECH-1.0.8/LIB_ADTECH.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 14:19:13.000000 LIB-ADTECH-1.0.8/LIB_ADTECH.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-07 14:19:13.000000 LIB-ADTECH-1.0.8/LIB_ADTECH.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-07 14:19:13.000000 LIB-ADTECH-1.0.8/LIB_ADTECH.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1108 2023-07-07 12:20:58.000000 LIB-ADTECH-1.0.8/LICENSE
--rw-rw-rw-   0        0        0      313 2023-07-07 14:19:13.898107 LIB-ADTECH-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-07 12:22:07.000000 LIB-ADTECH-1.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-07-07 14:19:13.899542 LIB-ADTECH-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      470 2023-07-07 14:19:11.000000 LIB-ADTECH-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 14:10:57.494904 LIB-ADTECH-1.1.1/
+drwxrwxrwx   0        0        0        0 2023-07-24 14:10:57.474519 LIB-ADTECH-1.1.1/Adlib/
+-rw-rw-rw-   0        0        0       26 2023-07-07 12:20:05.000000 LIB-ADTECH-1.1.1/Adlib/__ini__.py
+-rw-rw-rw-   0        0        0     2965 2023-07-24 14:09:45.000000 LIB-ADTECH-1.1.1/Adlib/funcoes.py
+drwxrwxrwx   0        0        0        0 2023-07-24 14:10:57.491228 LIB-ADTECH-1.1.1/LIB_ADTECH.egg-info/
+-rw-rw-rw-   0        0        0      312 2023-07-24 14:10:57.000000 LIB-ADTECH-1.1.1/LIB_ADTECH.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-07-24 14:10:57.000000 LIB-ADTECH-1.1.1/LIB_ADTECH.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 14:10:57.000000 LIB-ADTECH-1.1.1/LIB_ADTECH.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-24 14:10:57.000000 LIB-ADTECH-1.1.1/LIB_ADTECH.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-24 14:10:57.000000 LIB-ADTECH-1.1.1/LIB_ADTECH.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1108 2023-07-07 12:20:58.000000 LIB-ADTECH-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0      312 2023-07-24 14:10:57.494904 LIB-ADTECH-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       46 2023-07-17 14:09:05.000000 LIB-ADTECH-1.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-24 14:10:57.494904 LIB-ADTECH-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      467 2023-07-24 14:10:14.000000 LIB-ADTECH-1.1.1/setup.py
```

### Comparing `LIB-ADTECH-1.0.8/LICENSE` & `LIB-ADTECH-1.1.1/LICENSE`

 * *Files identical despite different names*

