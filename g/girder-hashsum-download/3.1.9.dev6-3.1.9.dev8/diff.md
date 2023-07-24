# Comparing `tmp/girder-hashsum-download-3.1.9.dev6.tar.gz` & `tmp/girder-hashsum-download-3.1.9.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/girder-hashsum-download-3.1.9.dev6.tar", last modified: Wed Feb 23 16:09:45 2022, max compression
+gzip compressed data, was "dist/girder-hashsum-download-3.1.9.dev8.tar", last modified: Wed Feb 23 17:41:45 2022, max compression
```

## Comparing `girder-hashsum-download-3.1.9.dev6.tar` & `girder-hashsum-download-3.1.9.dev8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:45.000000 girder-hashsum-download-3.1.9.dev6/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:45.000000 girder-hashsum-download-3.1.9.dev6/girder_hashsum_download/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:45.000000 girder-hashsum-download-3.1.9.dev6/girder_hashsum_download/web_client/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:45.000000 girder-hashsum-download-3.1.9.dev6/girder_hashsum_download/web_client/stylesheets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2022-02-23 16:09:15.000000 girder-hashsum-download-3.1.9.dev6/girder_hashsum_download/web_client/stylesheets/hashsumDownloadFileInfoWidget.styl
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:45.000000 girder-hashsum-download-3.1.9.dev6/girder_hashsum_download/web_client/templates/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      482 2022-02-23 16:09:15.000000 girder-hashsum-download-3.1.9.dev6/girder_hashsum_download/web_client/templates/config.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)      473 2022-02-23 16:09:15.000000 girder-hashsum-download-3.1.9.dev6/girder_hashsum_download/web_client/templates/hashsumDownloadFileInfoWidget.pug
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:45.000000 girder-hashsum-download-3.1.9.dev6/girder_hashsum_download/web_client/views/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2070 2022-02-23 16:09:15.000000 girder-hashsum-download-3.1.9.dev6/girder_hashsum_download/web_client/views/ConfigView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1147 2022-02-23 16:09:15.000000 girder-hashsum-download-3.1.9.dev6/girder_hashsum_download/web_client/views/FileInfoWidget.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      516 2022-02-23 16:09:15.000000 girder-hashsum-download-3.1.9.dev6/girder_hashsum_download/web_client/main.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      584 2022-02-23 16:09:15.000000 girder-hashsum-download-3.1.9.dev6/girder_hashsum_download/web_client/package.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7479 2022-02-23 16:09:15.000000 girder-hashsum-download-3.1.9.dev6/girder_hashsum_download/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      492 2022-02-23 16:09:15.000000 girder-hashsum-download-3.1.9.dev6/girder_hashsum_download/settings.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:45.000000 girder-hashsum-download-3.1.9.dev6/girder_hashsum_download.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      744 2022-02-23 16:09:45.000000 girder-hashsum-download-3.1.9.dev6/girder_hashsum_download.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      936 2022-02-23 16:09:45.000000 girder-hashsum-download-3.1.9.dev6/girder_hashsum_download.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 16:09:45.000000 girder-hashsum-download-3.1.9.dev6/girder_hashsum_download.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       82 2022-02-23 16:09:45.000000 girder-hashsum-download-3.1.9.dev6/girder_hashsum_download.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 16:09:45.000000 girder-hashsum-download-3.1.9.dev6/girder_hashsum_download.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2022-02-23 16:09:45.000000 girder-hashsum-download-3.1.9.dev6/girder_hashsum_download.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2022-02-23 16:09:45.000000 girder-hashsum-download-3.1.9.dev6/girder_hashsum_download.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:45.000000 girder-hashsum-download-3.1.9.dev6/plugin_tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 16:09:15.000000 girder-hashsum-download-3.1.9.dev6/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2371 2022-02-23 16:09:15.000000 girder-hashsum-download-3.1.9.dev6/plugin_tests/hashsumSpec.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13511 2022-02-23 16:09:15.000000 girder-hashsum-download-3.1.9.dev6/plugin_tests/hashsum_download_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       61 2022-02-23 16:09:15.000000 girder-hashsum-download-3.1.9.dev6/plugin.cmake
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1822 2022-02-23 16:09:15.000000 girder-hashsum-download-3.1.9.dev6/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      744 2022-02-23 16:09:45.000000 girder-hashsum-download-3.1.9.dev6/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-02-23 16:09:45.000000 girder-hashsum-download-3.1.9.dev6/setup.cfg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:45.000000 girder-hashsum-download-3.1.9.dev8/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:45.000000 girder-hashsum-download-3.1.9.dev8/girder_hashsum_download/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:45.000000 girder-hashsum-download-3.1.9.dev8/girder_hashsum_download/web_client/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:45.000000 girder-hashsum-download-3.1.9.dev8/girder_hashsum_download/web_client/stylesheets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2022-02-23 17:41:16.000000 girder-hashsum-download-3.1.9.dev8/girder_hashsum_download/web_client/stylesheets/hashsumDownloadFileInfoWidget.styl
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:45.000000 girder-hashsum-download-3.1.9.dev8/girder_hashsum_download/web_client/templates/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      482 2022-02-23 17:41:16.000000 girder-hashsum-download-3.1.9.dev8/girder_hashsum_download/web_client/templates/config.pug
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      473 2022-02-23 17:41:16.000000 girder-hashsum-download-3.1.9.dev8/girder_hashsum_download/web_client/templates/hashsumDownloadFileInfoWidget.pug
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:45.000000 girder-hashsum-download-3.1.9.dev8/girder_hashsum_download/web_client/views/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2070 2022-02-23 17:41:16.000000 girder-hashsum-download-3.1.9.dev8/girder_hashsum_download/web_client/views/ConfigView.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1147 2022-02-23 17:41:16.000000 girder-hashsum-download-3.1.9.dev8/girder_hashsum_download/web_client/views/FileInfoWidget.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      516 2022-02-23 17:41:16.000000 girder-hashsum-download-3.1.9.dev8/girder_hashsum_download/web_client/main.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      584 2022-02-23 17:41:16.000000 girder-hashsum-download-3.1.9.dev8/girder_hashsum_download/web_client/package.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7479 2022-02-23 17:41:16.000000 girder-hashsum-download-3.1.9.dev8/girder_hashsum_download/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      492 2022-02-23 17:41:16.000000 girder-hashsum-download-3.1.9.dev8/girder_hashsum_download/settings.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:45.000000 girder-hashsum-download-3.1.9.dev8/girder_hashsum_download.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      744 2022-02-23 17:41:45.000000 girder-hashsum-download-3.1.9.dev8/girder_hashsum_download.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      936 2022-02-23 17:41:45.000000 girder-hashsum-download-3.1.9.dev8/girder_hashsum_download.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 17:41:45.000000 girder-hashsum-download-3.1.9.dev8/girder_hashsum_download.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       82 2022-02-23 17:41:45.000000 girder-hashsum-download-3.1.9.dev8/girder_hashsum_download.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-23 17:41:45.000000 girder-hashsum-download-3.1.9.dev8/girder_hashsum_download.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2022-02-23 17:41:45.000000 girder-hashsum-download-3.1.9.dev8/girder_hashsum_download.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2022-02-23 17:41:45.000000 girder-hashsum-download-3.1.9.dev8/girder_hashsum_download.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:45.000000 girder-hashsum-download-3.1.9.dev8/plugin_tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-23 17:41:16.000000 girder-hashsum-download-3.1.9.dev8/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2371 2022-02-23 17:41:16.000000 girder-hashsum-download-3.1.9.dev8/plugin_tests/hashsumSpec.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13511 2022-02-23 17:41:16.000000 girder-hashsum-download-3.1.9.dev8/plugin_tests/hashsum_download_test.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       61 2022-02-23 17:41:16.000000 girder-hashsum-download-3.1.9.dev8/plugin.cmake
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1822 2022-02-23 17:41:16.000000 girder-hashsum-download-3.1.9.dev8/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      744 2022-02-23 17:41:45.000000 girder-hashsum-download-3.1.9.dev8/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-02-23 17:41:45.000000 girder-hashsum-download-3.1.9.dev8/setup.cfg
```

### Comparing `girder-hashsum-download-3.1.9.dev6/girder_hashsum_download/web_client/views/ConfigView.js` & `girder-hashsum-download-3.1.9.dev8/girder_hashsum_download/web_client/views/ConfigView.js`

 * *Files identical despite different names*

### Comparing `girder-hashsum-download-3.1.9.dev6/girder_hashsum_download/web_client/views/FileInfoWidget.js` & `girder-hashsum-download-3.1.9.dev8/girder_hashsum_download/web_client/views/FileInfoWidget.js`

 * *Files identical despite different names*

### Comparing `girder-hashsum-download-3.1.9.dev6/girder_hashsum_download/web_client/main.js` & `girder-hashsum-download-3.1.9.dev8/girder_hashsum_download/web_client/main.js`

 * *Files identical despite different names*

### Comparing `girder-hashsum-download-3.1.9.dev6/girder_hashsum_download/web_client/package.json` & `girder-hashsum-download-3.1.9.dev8/girder_hashsum_download/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-hashsum-download-3.1.9.dev6/girder_hashsum_download/__init__.py` & `girder-hashsum-download-3.1.9.dev8/girder_hashsum_download/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-hashsum-download-3.1.9.dev6/girder_hashsum_download.egg-info/PKG-INFO` & `girder-hashsum-download-3.1.9.dev8/girder_hashsum_download.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-hashsum-download
-Version: 3.1.9.dev6
+Version: 3.1.9.dev8
 Summary: Allows download of a file by its hashsum.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#hashsum-download
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `girder-hashsum-download-3.1.9.dev6/girder_hashsum_download.egg-info/SOURCES.txt` & `girder-hashsum-download-3.1.9.dev8/girder_hashsum_download.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `girder-hashsum-download-3.1.9.dev6/plugin_tests/hashsumSpec.js` & `girder-hashsum-download-3.1.9.dev8/plugin_tests/hashsumSpec.js`

 * *Files identical despite different names*

### Comparing `girder-hashsum-download-3.1.9.dev6/plugin_tests/hashsum_download_test.py` & `girder-hashsum-download-3.1.9.dev8/plugin_tests/hashsum_download_test.py`

 * *Files identical despite different names*

### Comparing `girder-hashsum-download-3.1.9.dev6/setup.py` & `girder-hashsum-download-3.1.9.dev8/setup.py`

 * *Files identical despite different names*

### Comparing `girder-hashsum-download-3.1.9.dev6/PKG-INFO` & `girder-hashsum-download-3.1.9.dev8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-hashsum-download
-Version: 3.1.9.dev6
+Version: 3.1.9.dev8
 Summary: Allows download of a file by its hashsum.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#hashsum-download
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

