# Comparing `tmp/vzg.jconv-1.2.0.tar.gz` & `tmp/vzg.jconv-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vzg.jconv-1.2.0.tar", last modified: Fri Jul 21 15:39:31 2023, max compression
+gzip compressed data, was "vzg.jconv-1.2.1.tar", last modified: Mon Jul 24 12:08:33 2023, max compression
```

## Comparing `vzg.jconv-1.2.0.tar` & `vzg.jconv-1.2.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-21 15:39:31.545384 vzg.jconv-1.2.0/
--rw-rw-r--   0 teg       (1000) teg       (1000)    34520 2020-02-07 11:02:19.000000 vzg.jconv-1.2.0/LICENSE.txt
--rw-rw-r--   0 teg       (1000) teg       (1000)      149 2020-02-08 11:53:49.000000 vzg.jconv-1.2.0/MANIFEST.in
--rw-rw-r--   0 teg       (1000) teg       (1000)      815 2023-07-21 15:39:31.545384 vzg.jconv-1.2.0/PKG-INFO
--rw-rw-r--   0 teg       (1000) teg       (1000)      463 2023-02-16 10:38:51.000000 vzg.jconv-1.2.0/README.md
--rw-rw-r--   0 teg       (1000) teg       (1000)        6 2023-07-21 15:36:56.000000 vzg.jconv-1.2.0/VERSION.txt
--rw-rw-r--   0 teg       (1000) teg       (1000)       38 2023-07-21 15:39:31.545384 vzg.jconv-1.2.0/setup.cfg
--rw-rw-r--   0 teg       (1000) teg       (1000)     1679 2023-02-16 10:38:51.000000 vzg.jconv-1.2.0/setup.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-21 15:39:31.541384 vzg.jconv-1.2.0/src/
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-21 15:39:31.545384 vzg.jconv-1.2.0/src/vzg/
--rw-rw-r--   0 teg       (1000) teg       (1000)       80 2020-11-05 11:14:17.000000 vzg.jconv-1.2.0/src/vzg/__init__.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-21 15:39:31.545384 vzg.jconv-1.2.0/src/vzg/jconv/
--rw-rw-r--   0 teg       (1000) teg       (1000)      275 2020-02-07 09:30:55.000000 vzg.jconv-1.2.0/src/vzg/jconv/__init__.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-21 15:39:31.545384 vzg.jconv-1.2.0/src/vzg/jconv/converter/
--rw-rw-r--   0 teg       (1000) teg       (1000)      378 2020-02-07 13:03:16.000000 vzg.jconv-1.2.0/src/vzg/jconv/converter/__init__.py
--rw-rw-r--   0 teg       (1000) teg       (1000)    22021 2023-07-21 15:36:18.000000 vzg.jconv-1.2.0/src/vzg/jconv/converter/jats.py
--rw-rw-r--   0 teg       (1000) teg       (1000)      450 2020-07-07 11:26:12.000000 vzg.jconv-1.2.0/src/vzg/jconv/errors.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     1192 2023-07-21 15:36:18.000000 vzg.jconv-1.2.0/src/vzg/jconv/gapi.py
--rw-rw-r--   0 teg       (1000) teg       (1000)      875 2020-02-08 12:51:55.000000 vzg.jconv-1.2.0/src/vzg/jconv/interfaces.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-21 15:39:31.545384 vzg.jconv-1.2.0/src/vzg/jconv/langcode/
--rw-rw-r--   0 teg       (1000) teg       (1000)     1156 2020-02-07 12:48:06.000000 vzg.jconv-1.2.0/src/vzg/jconv/langcode/__init__.py
--rw-rw-r--   0 teg       (1000) teg       (1000)    11245 2020-02-07 12:11:08.000000 vzg.jconv-1.2.0/src/vzg/jconv/langcode/language-codes.json
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-21 15:39:31.545384 vzg.jconv-1.2.0/src/vzg/jconv/person/
--rw-rw-r--   0 teg       (1000) teg       (1000)     5949 2023-03-08 09:15:09.000000 vzg.jconv-1.2.0/src/vzg/jconv/person/__init__.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-21 15:39:31.545384 vzg.jconv-1.2.0/src/vzg/jconv/publisher/
--rw-rw-r--   0 teg       (1000) teg       (1000)     1231 2023-02-16 10:38:51.000000 vzg.jconv-1.2.0/src/vzg/jconv/publisher/__init__.py
--rw-rw-r--   0 teg       (1000) teg       (1000)      263 2020-07-02 08:39:22.000000 vzg.jconv-1.2.0/src/vzg/jconv/publisher/publisher-codes.json
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-21 15:39:31.545384 vzg.jconv-1.2.0/src/vzg/jconv/schema/
--rw-rw-r--   0 teg       (1000) teg       (1000)    17321 2022-01-14 16:28:18.000000 vzg.jconv-1.2.0/src/vzg/jconv/schema/article_schema.json
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-21 15:39:31.545384 vzg.jconv-1.2.0/src/vzg/jconv/test/
--rw-rw-r--   0 teg       (1000) teg       (1000)      960 2020-02-11 12:04:12.000000 vzg.jconv-1.2.0/src/vzg/jconv/test/__init__.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     1218 2023-07-21 09:37:23.000000 vzg.jconv-1.2.0/src/vzg/jconv/test/conftest.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     6068 2023-07-21 15:36:18.000000 vzg.jconv-1.2.0/src/vzg/jconv/test/test_jats_article.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     3151 2023-07-21 15:36:18.000000 vzg.jconv-1.2.0/src/vzg/jconv/test/test_jats_converter.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     4936 2023-07-21 15:36:18.000000 vzg.jconv-1.2.0/src/vzg/jconv/test/test_jats_degruyter.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     1038 2020-02-11 12:04:12.000000 vzg.jconv-1.2.0/src/vzg/jconv/test/test_langcode.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     2803 2023-02-16 12:17:30.000000 vzg.jconv-1.2.0/src/vzg/jconv/test/test_person.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     1029 2020-07-02 09:05:29.000000 vzg.jconv-1.2.0/src/vzg/jconv/test/test_publisher.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-21 15:39:31.545384 vzg.jconv-1.2.0/src/vzg/jconv/tools/
--rw-rw-r--   0 teg       (1000) teg       (1000)      378 2020-02-12 10:22:25.000000 vzg.jconv-1.2.0/src/vzg/jconv/tools/__init__.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     6790 2023-02-16 12:40:49.000000 vzg.jconv-1.2.0/src/vzg/jconv/tools/simple_conv.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-21 15:39:31.545384 vzg.jconv-1.2.0/src/vzg/jconv/utils/
--rw-rw-r--   0 teg       (1000) teg       (1000)     2571 2023-07-20 10:01:19.000000 vzg.jconv-1.2.0/src/vzg/jconv/utils/__init__.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     1644 2020-09-25 10:34:55.000000 vzg.jconv-1.2.0/src/vzg/jconv/utils/date.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-21 15:39:31.545384 vzg.jconv-1.2.0/src/vzg.jconv.egg-info/
--rw-rw-r--   0 teg       (1000) teg       (1000)      815 2023-07-21 15:39:31.000000 vzg.jconv-1.2.0/src/vzg.jconv.egg-info/PKG-INFO
--rw-rw-r--   0 teg       (1000) teg       (1000)     1211 2023-07-21 15:39:31.000000 vzg.jconv-1.2.0/src/vzg.jconv.egg-info/SOURCES.txt
--rw-rw-r--   0 teg       (1000) teg       (1000)        1 2023-07-21 15:39:31.000000 vzg.jconv-1.2.0/src/vzg.jconv.egg-info/dependency_links.txt
--rw-rw-r--   0 teg       (1000) teg       (1000)       64 2023-07-21 15:39:31.000000 vzg.jconv-1.2.0/src/vzg.jconv.egg-info/entry_points.txt
--rw-rw-r--   0 teg       (1000) teg       (1000)        4 2023-07-21 15:39:31.000000 vzg.jconv-1.2.0/src/vzg.jconv.egg-info/namespace_packages.txt
--rw-rw-r--   0 teg       (1000) teg       (1000)        1 2020-02-07 10:31:14.000000 vzg.jconv-1.2.0/src/vzg.jconv.egg-info/not-zip-safe
--rw-rw-r--   0 teg       (1000) teg       (1000)       48 2023-07-21 15:39:31.000000 vzg.jconv-1.2.0/src/vzg.jconv.egg-info/requires.txt
--rw-rw-r--   0 teg       (1000) teg       (1000)        4 2023-07-21 15:39:31.000000 vzg.jconv-1.2.0/src/vzg.jconv.egg-info/top_level.txt
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-24 12:08:33.779858 vzg.jconv-1.2.1/
+-rw-rw-r--   0 teg       (1000) teg       (1000)    34520 2020-02-07 11:02:19.000000 vzg.jconv-1.2.1/LICENSE.txt
+-rw-rw-r--   0 teg       (1000) teg       (1000)      149 2020-02-08 11:53:49.000000 vzg.jconv-1.2.1/MANIFEST.in
+-rw-rw-r--   0 teg       (1000) teg       (1000)      843 2023-07-24 12:08:33.779858 vzg.jconv-1.2.1/PKG-INFO
+-rw-rw-r--   0 teg       (1000) teg       (1000)      463 2023-02-16 10:38:51.000000 vzg.jconv-1.2.1/README.md
+-rw-rw-r--   0 teg       (1000) teg       (1000)        6 2023-07-24 12:04:30.000000 vzg.jconv-1.2.1/VERSION.txt
+-rw-rw-r--   0 teg       (1000) teg       (1000)       38 2023-07-24 12:08:33.779858 vzg.jconv-1.2.1/setup.cfg
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1679 2023-02-16 10:38:51.000000 vzg.jconv-1.2.1/setup.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-24 12:08:33.775858 vzg.jconv-1.2.1/src/
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-24 12:08:33.775858 vzg.jconv-1.2.1/src/vzg/
+-rw-rw-r--   0 teg       (1000) teg       (1000)       80 2020-11-05 11:14:17.000000 vzg.jconv-1.2.1/src/vzg/__init__.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-24 12:08:33.775858 vzg.jconv-1.2.1/src/vzg/jconv/
+-rw-rw-r--   0 teg       (1000) teg       (1000)      275 2020-02-07 09:30:55.000000 vzg.jconv-1.2.1/src/vzg/jconv/__init__.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-24 12:08:33.775858 vzg.jconv-1.2.1/src/vzg/jconv/converter/
+-rw-rw-r--   0 teg       (1000) teg       (1000)      378 2020-02-07 13:03:16.000000 vzg.jconv-1.2.1/src/vzg/jconv/converter/__init__.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)    21834 2023-07-24 11:52:45.000000 vzg.jconv-1.2.1/src/vzg/jconv/converter/jats.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)      450 2020-07-07 11:26:12.000000 vzg.jconv-1.2.1/src/vzg/jconv/errors.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1278 2023-07-24 11:43:22.000000 vzg.jconv-1.2.1/src/vzg/jconv/gapi.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)      875 2020-02-08 12:51:55.000000 vzg.jconv-1.2.1/src/vzg/jconv/interfaces.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-24 12:08:33.775858 vzg.jconv-1.2.1/src/vzg/jconv/langcode/
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1156 2020-02-07 12:48:06.000000 vzg.jconv-1.2.1/src/vzg/jconv/langcode/__init__.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)    11245 2020-02-07 12:11:08.000000 vzg.jconv-1.2.1/src/vzg/jconv/langcode/language-codes.json
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-24 12:08:33.775858 vzg.jconv-1.2.1/src/vzg/jconv/person/
+-rw-rw-r--   0 teg       (1000) teg       (1000)     5949 2023-07-21 15:51:03.000000 vzg.jconv-1.2.1/src/vzg/jconv/person/__init__.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-24 12:08:33.775858 vzg.jconv-1.2.1/src/vzg/jconv/publisher/
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1231 2023-02-16 10:38:51.000000 vzg.jconv-1.2.1/src/vzg/jconv/publisher/__init__.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)      263 2020-07-02 08:39:22.000000 vzg.jconv-1.2.1/src/vzg/jconv/publisher/publisher-codes.json
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-24 12:08:33.775858 vzg.jconv-1.2.1/src/vzg/jconv/schema/
+-rw-rw-r--   0 teg       (1000) teg       (1000)    17321 2022-01-14 16:28:18.000000 vzg.jconv-1.2.1/src/vzg/jconv/schema/article_schema.json
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-24 12:08:33.775858 vzg.jconv-1.2.1/src/vzg/jconv/test/
+-rw-rw-r--   0 teg       (1000) teg       (1000)      960 2020-02-11 12:04:12.000000 vzg.jconv-1.2.1/src/vzg/jconv/test/__init__.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1218 2023-07-21 15:51:03.000000 vzg.jconv-1.2.1/src/vzg/jconv/test/conftest.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     6068 2023-07-21 15:51:03.000000 vzg.jconv-1.2.1/src/vzg/jconv/test/test_jats_article.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     3151 2023-07-21 15:51:03.000000 vzg.jconv-1.2.1/src/vzg/jconv/test/test_jats_converter.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     4936 2023-07-21 15:51:03.000000 vzg.jconv-1.2.1/src/vzg/jconv/test/test_jats_degruyter.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1038 2020-02-11 12:04:12.000000 vzg.jconv-1.2.1/src/vzg/jconv/test/test_langcode.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     2803 2023-02-16 12:17:30.000000 vzg.jconv-1.2.1/src/vzg/jconv/test/test_person.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1029 2020-07-02 09:05:29.000000 vzg.jconv-1.2.1/src/vzg/jconv/test/test_publisher.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-24 12:08:33.779858 vzg.jconv-1.2.1/src/vzg/jconv/tools/
+-rw-rw-r--   0 teg       (1000) teg       (1000)      378 2020-02-12 10:22:25.000000 vzg.jconv-1.2.1/src/vzg/jconv/tools/__init__.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     6790 2023-07-21 15:51:03.000000 vzg.jconv-1.2.1/src/vzg/jconv/tools/simple_conv.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-24 12:08:33.779858 vzg.jconv-1.2.1/src/vzg/jconv/utils/
+-rw-rw-r--   0 teg       (1000) teg       (1000)     2932 2023-07-24 11:56:32.000000 vzg.jconv-1.2.1/src/vzg/jconv/utils/__init__.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1644 2020-09-25 10:34:55.000000 vzg.jconv-1.2.1/src/vzg/jconv/utils/date.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-24 12:08:33.775858 vzg.jconv-1.2.1/src/vzg.jconv.egg-info/
+-rw-rw-r--   0 teg       (1000) teg       (1000)      843 2023-07-24 12:08:33.000000 vzg.jconv-1.2.1/src/vzg.jconv.egg-info/PKG-INFO
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1211 2023-07-24 12:08:33.000000 vzg.jconv-1.2.1/src/vzg.jconv.egg-info/SOURCES.txt
+-rw-rw-r--   0 teg       (1000) teg       (1000)        1 2023-07-24 12:08:33.000000 vzg.jconv-1.2.1/src/vzg.jconv.egg-info/dependency_links.txt
+-rw-rw-r--   0 teg       (1000) teg       (1000)       65 2023-07-24 12:08:33.000000 vzg.jconv-1.2.1/src/vzg.jconv.egg-info/entry_points.txt
+-rw-rw-r--   0 teg       (1000) teg       (1000)        4 2023-07-24 12:08:33.000000 vzg.jconv-1.2.1/src/vzg.jconv.egg-info/namespace_packages.txt
+-rw-rw-r--   0 teg       (1000) teg       (1000)        1 2020-02-07 10:31:14.000000 vzg.jconv-1.2.1/src/vzg.jconv.egg-info/not-zip-safe
+-rw-rw-r--   0 teg       (1000) teg       (1000)       48 2023-07-24 12:08:33.000000 vzg.jconv-1.2.1/src/vzg.jconv.egg-info/requires.txt
+-rw-rw-r--   0 teg       (1000) teg       (1000)        4 2023-07-24 12:08:33.000000 vzg.jconv-1.2.1/src/vzg.jconv.egg-info/top_level.txt
```

### Comparing `vzg.jconv-1.2.0/LICENSE.txt` & `vzg.jconv-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.0/PKG-INFO` & `vzg.jconv-1.2.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: vzg.jconv
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python library to create JSON Data
 Home-page: https://github.com/gbv/vzg.jconv
 Author: Marc-J. Tegethoff
 Author-email: tegethoff@gbv.de
 License: GNU Affero General Public License v3
 Project-URL: PyPI, https://pypi.python.org/pypi/vzg.jconv
 Project-URL: Source, https://github.com/gbv/vzg.jconv
 Project-URL: Tracker, https://github.com/gbv/vzg.jconv/issues
 Keywords: VZG Python JSON XML JAST
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Requires-Python: >=3.10
 License-File: LICENSE.txt
+
+UNKNOWN
+
```

### Comparing `vzg.jconv-1.2.0/setup.py` & `vzg.jconv-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.0/src/vzg/jconv/converter/jats.py` & `vzg.jconv-1.2.1/src/vzg/jconv/converter/jats.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,20 @@
 from vzg.jconv.interfaces import IArticle
 from vzg.jconv.interfaces import IConverter
 from vzg.jconv.gapi import NAMESPACES
 from vzg.jconv.gapi import JSON_SCHEMA
 from vzg.jconv.gapi import JATS_SPRINGER_PUBTYPE
 from vzg.jconv.gapi import JATS_SPRINGER_JOURNALTYPE
 from vzg.jconv.gapi import PUBTYPE_SOURCES
+from vzg.jconv.gapi import JATS_PUBTYPE_SUFFIX
 from vzg.jconv.langcode import ISO_639
 from vzg.jconv.publisher import getPublisherId
 from vzg.jconv.errors import NoPublisherError
 from vzg.jconv.utils import node2text
-from vzg.jconv.utils import flatten_line
+from vzg.jconv.utils import get_pubtype_suffix
 from vzg.jconv.utils.date import JatsDate
 from lxml import etree
 import logging
 import json
 import jsonschema
 
 __author__ = """Marc-J. Tegethoff <marc.tegethoff@gbv.de>"""
@@ -301,14 +302,15 @@
 
                 jid = {"type": jtype, "id": node[0]}
 
                 if jtype == "basic":
                     jid["type"] = "springer"
                     if self.pubtype_source == PUBTYPE_SOURCES.degruyter:
                         jid["type"] = "degruyter"
+                        jid["id"] += get_pubtype_suffix(self.pubtype.value)
 
                 if jid["type"] in JATS_SPRINGER_JOURNALTYPE.__members__:
                     jid["type"] = JATS_SPRINGER_JOURNALTYPE[jid["type"]].value
 
                 pdict["journal_ids"].append(jid)
 
         publisher = {}
@@ -441,34 +443,26 @@
 
         expression = JATS_XPATHS["other_ids_doi"]
         node = self.xpath(expression)
 
         try:
             doi_path = node[0].split("/")
             pdict["id"] = doi_path[-1]
-
-            if self.pubtype.value == JATS_SPRINGER_PUBTYPE.print.value:
-                pdict["id"] += "-p"
-            elif self.pubtype.value == JATS_SPRINGER_PUBTYPE.electronic.value:
-                pdict["id"] += "-e"
+            pdict["id"] += get_pubtype_suffix(self.pubtype.value)
 
             return pdict
         except (IndexError, ValueError):
             logger.debug("primary_id: no doi")
 
         expression = JATS_XPATHS["primary_id"]
         node = self.xpath(expression)
 
         try:
             pdict["id"] = node[0]
-
-            if self.pubtype.value == JATS_SPRINGER_PUBTYPE.print.value:
-                pdict["id"] += "-p"
-            elif self.pubtype.value == JATS_SPRINGER_PUBTYPE.electronic.value:
-                pdict["id"] += "-e"
+            pdict["id"] += get_pubtype_suffix(self.pubtype.value)
         except IndexError:
             logger.debug("no primary_id")
 
         return pdict
 
     @property
     def subjects(self):
```

### Comparing `vzg.jconv-1.2.0/src/vzg/jconv/gapi.py` & `vzg.jconv-1.2.1/src/vzg/jconv/gapi.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,14 +45,21 @@
 
 class JATS_SPRINGER_AUTHORTYPE(Enum):
     """"""
 
     author = "aut"
 
 
+class JATS_PUBTYPE_SUFFIX(Enum):
+    """"""
+
+    electronic = "-e"
+    print = "-p"
+
+
 class PERSON_ID_TYPES(Enum):
     """"""
 
     orcid = "orcid"
     unknown = "unknown"
```

### Comparing `vzg.jconv-1.2.0/src/vzg/jconv/interfaces.py` & `vzg.jconv-1.2.1/src/vzg/jconv/interfaces.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.0/src/vzg/jconv/langcode/__init__.py` & `vzg.jconv-1.2.1/src/vzg/jconv/langcode/__init__.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.0/src/vzg/jconv/langcode/language-codes.json` & `vzg.jconv-1.2.1/src/vzg/jconv/langcode/language-codes.json`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.0/src/vzg/jconv/person/__init__.py` & `vzg.jconv-1.2.1/src/vzg/jconv/person/__init__.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.0/src/vzg/jconv/publisher/__init__.py` & `vzg.jconv-1.2.1/src/vzg/jconv/publisher/__init__.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.0/src/vzg/jconv/schema/article_schema.json` & `vzg.jconv-1.2.1/src/vzg/jconv/schema/article_schema.json`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.0/src/vzg/jconv/test/__init__.py` & `vzg.jconv-1.2.1/src/vzg/jconv/test/__init__.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.0/src/vzg/jconv/test/conftest.py` & `vzg.jconv-1.2.1/src/vzg/jconv/test/conftest.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.0/src/vzg/jconv/test/test_jats_article.py` & `vzg.jconv-1.2.1/src/vzg/jconv/test/test_jats_article.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.0/src/vzg/jconv/test/test_jats_converter.py` & `vzg.jconv-1.2.1/src/vzg/jconv/test/test_jats_converter.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.0/src/vzg/jconv/test/test_jats_degruyter.py` & `vzg.jconv-1.2.1/src/vzg/jconv/test/test_jats_degruyter.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.0/src/vzg/jconv/test/test_langcode.py` & `vzg.jconv-1.2.1/src/vzg/jconv/test/test_langcode.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.0/src/vzg/jconv/test/test_person.py` & `vzg.jconv-1.2.1/src/vzg/jconv/test/test_person.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.0/src/vzg/jconv/test/test_publisher.py` & `vzg.jconv-1.2.1/src/vzg/jconv/test/test_publisher.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.0/src/vzg/jconv/tools/simple_conv.py` & `vzg.jconv-1.2.1/src/vzg/jconv/tools/simple_conv.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.0/src/vzg/jconv/utils/__init__.py` & `vzg.jconv-1.2.1/src/vzg/jconv/utils/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 ##############################################################################
 """
 
 # Imports
 from lxml import etree
 import re
 from vzg.jconv.gapi import NAMESPACES
+from vzg.jconv.gapi import JATS_SPRINGER_PUBTYPE
+from vzg.jconv.gapi import JATS_PUBTYPE_SUFFIX
+
 
 __author__ = """Marc-J. Tegethoff <marc.tegethoff@gbv.de>"""
 __docformat__ = "plaintext"
 
 # TeX formular
 TEXREX = re.compile(r"(\${1,2}.*\${1,2})")
 # Upper case greek letters within a formula
@@ -89,7 +92,16 @@
         nodetext = nodetext.replace(c_, " ")
 
     return flatten_line(nodetext)
 
 
 def flatten_line(line: str) -> str:
     return STRIPCHARS.sub(" ", line).strip()
+
+
+def get_pubtype_suffix(pubtype: str) -> str:
+    pdict = {
+        JATS_SPRINGER_PUBTYPE.print.value: JATS_PUBTYPE_SUFFIX.print.value,
+        JATS_SPRINGER_PUBTYPE.electronic.value: JATS_PUBTYPE_SUFFIX.electronic.value,
+    }
+
+    return pdict.get(pubtype, "")
```

### Comparing `vzg.jconv-1.2.0/src/vzg/jconv/utils/date.py` & `vzg.jconv-1.2.1/src/vzg/jconv/utils/date.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.0/src/vzg.jconv.egg-info/PKG-INFO` & `vzg.jconv-1.2.1/src/vzg.jconv.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: vzg.jconv
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python library to create JSON Data
 Home-page: https://github.com/gbv/vzg.jconv
 Author: Marc-J. Tegethoff
 Author-email: tegethoff@gbv.de
 License: GNU Affero General Public License v3
 Project-URL: PyPI, https://pypi.python.org/pypi/vzg.jconv
 Project-URL: Source, https://github.com/gbv/vzg.jconv
 Project-URL: Tracker, https://github.com/gbv/vzg.jconv/issues
 Keywords: VZG Python JSON XML JAST
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Requires-Python: >=3.10
 License-File: LICENSE.txt
+
+UNKNOWN
+
```

### Comparing `vzg.jconv-1.2.0/src/vzg.jconv.egg-info/SOURCES.txt` & `vzg.jconv-1.2.1/src/vzg.jconv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

