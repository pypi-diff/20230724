# Comparing `tmp/Primice-1.0.0.tar.gz` & `tmp/Primice-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Primice-1.0.0.tar", last modified: Sun Jul 16 15:41:18 2023, max compression
+gzip compressed data, was "Primice-1.0.1.tar", last modified: Mon Jul 24 05:22:23 2023, max compression
```

## Comparing `Primice-1.0.0.tar` & `Primice-1.0.1.tar`

### file list

```diff
@@ -1,28 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 15:41:18.523363 Primice-1.0.0/
--rw-rw-rw-   0        0        0     1091 2023-07-16 06:14:26.000000 Primice-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     2054 2023-07-16 15:41:18.523363 Primice-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-16 15:41:18.502610 Primice-1.0.0/Primice/
-drwxrwxrwx   0        0        0        0 2023-07-16 15:41:18.510614 Primice-1.0.0/Primice/Mongo/
--rw-rw-rw-   0        0        0        0 2023-07-16 15:14:52.000000 Primice-1.0.0/Primice/Mongo/__init__.py
--rw-rw-rw-   0        0        0     3673 2023-07-16 09:11:00.000000 Primice-1.0.0/Primice/Mongo/to_Mongodb.py
-drwxrwxrwx   0        0        0        0 2023-07-16 15:41:18.513614 Primice-1.0.0/Primice/MySQL/
--rw-rw-rw-   0        0        0     1315 2023-07-16 15:39:04.000000 Primice-1.0.0/Primice/MySQL/DataTable.py
--rw-rw-rw-   0        0        0        0 2023-07-16 15:14:41.000000 Primice-1.0.0/Primice/MySQL/__init__.py
--rw-rw-rw-   0        0        0     2997 2023-07-16 15:39:04.000000 Primice-1.0.0/Primice/MySQL/to_MySQL.py
-drwxrwxrwx   0        0        0        0 2023-07-16 15:41:18.516071 Primice-1.0.0/Primice/Proxy/
--rw-rw-rw-   0        0        0     3620 2023-07-16 15:39:04.000000 Primice-1.0.0/Primice/Proxy/Proxy.py
--rw-rw-rw-   0        0        0        0 2023-07-16 15:16:49.000000 Primice-1.0.0/Primice/Proxy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 15:41:18.521076 Primice-1.0.0/Primice/Spider/
--rw-rw-rw-   0        0        0     2816 2023-07-16 15:15:52.000000 Primice-1.0.0/Primice/Spider/Log.py
--rw-rw-rw-   0        0        0      228 2023-06-13 05:56:41.000000 Primice-1.0.0/Primice/Spider/Twitter爬虫.py
--rw-rw-rw-   0        0        0        0 2023-05-21 10:56:02.000000 Primice-1.0.0/Primice/Spider/__init__.py
--rw-rw-rw-   0        0        0     6004 2023-06-13 05:57:15.000000 Primice-1.0.0/Primice/Spider/http_raw2requests.py
--rw-rw-rw-   0        0        0        0 2023-07-16 06:09:15.000000 Primice-1.0.0/Primice/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 15:41:18.507609 Primice-1.0.0/Primice.egg-info/
--rw-rw-rw-   0        0        0     2054 2023-07-16 15:41:18.000000 Primice-1.0.0/Primice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      469 2023-07-16 15:41:18.000000 Primice-1.0.0/Primice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 15:41:18.000000 Primice-1.0.0/Primice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-16 15:41:18.000000 Primice-1.0.0/Primice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1688 2023-07-16 15:39:04.000000 Primice-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-16 15:41:18.524759 Primice-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      601 2023-07-16 15:41:12.000000 Primice-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 05:22:23.121465 Primice-1.0.1/
+-rw-rw-rw-   0        0        0     1091 2023-07-16 06:14:26.000000 Primice-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     4849 2023-07-24 05:22:23.120465 Primice-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-24 05:22:23.099342 Primice-1.0.1/Primice/
+drwxrwxrwx   0        0        0        0 2023-07-24 05:22:23.106465 Primice-1.0.1/Primice/Mongo/
+-rw-rw-rw-   0        0        0        0 2023-07-16 15:14:52.000000 Primice-1.0.1/Primice/Mongo/__init__.py
+-rw-rw-rw-   0        0        0     3673 2023-07-16 09:11:00.000000 Primice-1.0.1/Primice/Mongo/to_Mongodb.py
+drwxrwxrwx   0        0        0        0 2023-07-24 05:22:23.110469 Primice-1.0.1/Primice/MySQL/
+-rw-rw-rw-   0        0        0     1315 2023-07-16 15:39:04.000000 Primice-1.0.1/Primice/MySQL/DataTable.py
+-rw-rw-rw-   0        0        0        0 2023-07-16 15:14:41.000000 Primice-1.0.1/Primice/MySQL/__init__.py
+-rw-rw-rw-   0        0        0     2997 2023-07-16 15:39:04.000000 Primice-1.0.1/Primice/MySQL/to_MySQL.py
+drwxrwxrwx   0        0        0        0 2023-07-24 05:22:23.112465 Primice-1.0.1/Primice/Proxy/
+-rw-rw-rw-   0        0        0     3620 2023-07-16 15:39:04.000000 Primice-1.0.1/Primice/Proxy/Proxy.py
+-rw-rw-rw-   0        0        0        0 2023-07-16 15:16:49.000000 Primice-1.0.1/Primice/Proxy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 05:22:23.117465 Primice-1.0.1/Primice/Spider/
+-rw-rw-rw-   0        0        0     2816 2023-07-16 15:15:52.000000 Primice-1.0.1/Primice/Spider/Log.py
+-rw-rw-rw-   0        0        0      228 2023-06-13 05:56:41.000000 Primice-1.0.1/Primice/Spider/Twitter爬虫.py
+-rw-rw-rw-   0        0        0        0 2023-05-21 10:56:02.000000 Primice-1.0.1/Primice/Spider/__init__.py
+-rw-rw-rw-   0        0        0     6004 2023-06-13 05:57:15.000000 Primice-1.0.1/Primice/Spider/http_raw2requests.py
+drwxrwxrwx   0        0        0        0 2023-07-24 05:22:23.119466 Primice-1.0.1/Primice/Utils/
+-rw-rw-rw-   0        0        0      635 2023-07-24 04:05:59.000000 Primice-1.0.1/Primice/Utils/BloomFilter.py
+-rw-rw-rw-   0        0        0        0 2023-07-24 04:02:31.000000 Primice-1.0.1/Primice/Utils/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-16 06:09:15.000000 Primice-1.0.1/Primice/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 05:22:23.104465 Primice-1.0.1/Primice.egg-info/
+-rw-rw-rw-   0        0        0     4849 2023-07-24 05:22:23.000000 Primice-1.0.1/Primice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      554 2023-07-24 05:22:23.000000 Primice-1.0.1/Primice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 05:22:23.000000 Primice-1.0.1/Primice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-24 05:22:23.000000 Primice-1.0.1/Primice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-24 05:22:23.000000 Primice-1.0.1/Primice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4478 2023-07-24 04:18:15.000000 Primice-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-24 05:22:23.121465 Primice-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      767 2023-07-24 05:22:03.000000 Primice-1.0.1/setup.py
```

### Comparing `Primice-1.0.0/LICENSE` & `Primice-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Primice-1.0.0/Primice/Mongo/to_Mongodb.py` & `Primice-1.0.1/Primice/Mongo/to_Mongodb.py`

 * *Files identical despite different names*

### Comparing `Primice-1.0.0/Primice/MySQL/DataTable.py` & `Primice-1.0.1/Primice/MySQL/DataTable.py`

 * *Files identical despite different names*

### Comparing `Primice-1.0.0/Primice/MySQL/to_MySQL.py` & `Primice-1.0.1/Primice/MySQL/to_MySQL.py`

 * *Files identical despite different names*

### Comparing `Primice-1.0.0/Primice/Proxy/Proxy.py` & `Primice-1.0.1/Primice/Proxy/Proxy.py`

 * *Files identical despite different names*

### Comparing `Primice-1.0.0/Primice/Spider/Log.py` & `Primice-1.0.1/Primice/Spider/Log.py`

 * *Files identical despite different names*

### Comparing `Primice-1.0.0/Primice/Spider/http_raw2requests.py` & `Primice-1.0.1/Primice/Spider/http_raw2requests.py`

 * *Files identical despite different names*

