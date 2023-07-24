# Comparing `tmp/proxy_cheap-0.0.3.tar.gz` & `tmp/proxy_cheap-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxy_cheap-0.0.3.tar", last modified: Mon Jul 24 12:49:15 2023, max compression
+gzip compressed data, was "proxy_cheap-0.0.4.tar", last modified: Mon Jul 24 12:53:17 2023, max compression
```

## Comparing `proxy_cheap-0.0.3.tar` & `proxy_cheap-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 12:49:15.008974 proxy_cheap-0.0.3/
--rw-rw-rw-   0        0        0     1084 2023-07-24 11:40:03.000000 proxy_cheap-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      646 2023-07-24 12:49:15.007977 proxy_cheap-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      115 2023-07-24 11:32:09.000000 proxy_cheap-0.0.3/README.md
--rw-rw-rw-   0        0        0      620 2023-07-24 12:48:31.000000 proxy_cheap-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-24 12:49:15.008974 proxy_cheap-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-24 12:49:14.994972 proxy_cheap-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-24 12:49:14.997974 proxy_cheap-0.0.3/src/proxy_cheap/
--rw-rw-rw-   0        0        0        0 2023-07-24 11:03:50.000000 proxy_cheap-0.0.3/src/proxy_cheap/__init__.py
--rw-rw-rw-   0        0        0     3429 2023-07-24 12:40:47.000000 proxy_cheap-0.0.3/src/proxy_cheap/cheap.py
-drwxrwxrwx   0        0        0        0 2023-07-24 12:49:15.007977 proxy_cheap-0.0.3/src/proxy_cheap.egg-info/
--rw-rw-rw-   0        0        0      646 2023-07-24 12:49:14.000000 proxy_cheap-0.0.3/src/proxy_cheap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-07-24 12:49:14.000000 proxy_cheap-0.0.3/src/proxy_cheap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 12:49:14.000000 proxy_cheap-0.0.3/src/proxy_cheap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-24 12:49:14.000000 proxy_cheap-0.0.3/src/proxy_cheap.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 12:53:17.235532 proxy_cheap-0.0.4/
+-rw-rw-rw-   0        0        0     1084 2023-07-24 11:40:03.000000 proxy_cheap-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      646 2023-07-24 12:53:17.235532 proxy_cheap-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      115 2023-07-24 11:32:09.000000 proxy_cheap-0.0.4/README.md
+-rw-rw-rw-   0        0        0      620 2023-07-24 12:53:00.000000 proxy_cheap-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-24 12:53:17.235532 proxy_cheap-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-24 12:53:17.218760 proxy_cheap-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-24 12:53:17.222762 proxy_cheap-0.0.4/src/proxy_cheap/
+-rw-rw-rw-   0        0        0        0 2023-07-24 11:03:50.000000 proxy_cheap-0.0.4/src/proxy_cheap/__init__.py
+-rw-rw-rw-   0        0        0     3429 2023-07-24 12:40:47.000000 proxy_cheap-0.0.4/src/proxy_cheap/cheap.py
+drwxrwxrwx   0        0        0        0 2023-07-24 12:53:17.234567 proxy_cheap-0.0.4/src/proxy_cheap.egg-info/
+-rw-rw-rw-   0        0        0      646 2023-07-24 12:53:17.000000 proxy_cheap-0.0.4/src/proxy_cheap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-07-24 12:53:17.000000 proxy_cheap-0.0.4/src/proxy_cheap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 12:53:17.000000 proxy_cheap-0.0.4/src/proxy_cheap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-24 12:53:17.000000 proxy_cheap-0.0.4/src/proxy_cheap.egg-info/top_level.txt
```

### Comparing `proxy_cheap-0.0.3/LICENSE` & `proxy_cheap-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `proxy_cheap-0.0.3/PKG-INFO` & `proxy_cheap-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxy_cheap
-Version: 0.0.3
+Version: 0.0.4
 Summary: proxy-cheap API python implementatione
 Author-email: lr2bmail <lr2b.com@gmail.com>
 Project-URL: Homepage, https://github.com/lr2bmail/proxy_cheap
 Project-URL: Bug Tracker, https://github.com/lr2bmail/proxy_cheap/issues
 Classifier: Programming Language :: Python :: 2
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `proxy_cheap-0.0.3/pyproject.toml` & `proxy_cheap-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools>=61.0","requests"]
+requires = ["setuptools>=44.0","requests"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "proxy_cheap"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="lr2bmail", email="lr2b.com@gmail.com" },
 ]
 description = "proxy-cheap API python implementatione"
 readme = "README.md"
 requires-python = ">=2.7"
 classifiers = [
```

### Comparing `proxy_cheap-0.0.3/src/proxy_cheap/cheap.py` & `proxy_cheap-0.0.4/src/proxy_cheap/cheap.py`

 * *Files identical despite different names*

### Comparing `proxy_cheap-0.0.3/src/proxy_cheap.egg-info/PKG-INFO` & `proxy_cheap-0.0.4/src/proxy_cheap.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxy-cheap
-Version: 0.0.3
+Version: 0.0.4
 Summary: proxy-cheap API python implementatione
 Author-email: lr2bmail <lr2b.com@gmail.com>
 Project-URL: Homepage, https://github.com/lr2bmail/proxy_cheap
 Project-URL: Bug Tracker, https://github.com/lr2bmail/proxy_cheap/issues
 Classifier: Programming Language :: Python :: 2
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

