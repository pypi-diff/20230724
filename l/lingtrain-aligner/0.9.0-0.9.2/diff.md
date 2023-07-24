# Comparing `tmp/lingtrain-aligner-0.9.0.tar.gz` & `tmp/lingtrain-aligner-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lingtrain-aligner-0.9.0.tar", last modified: Fri Jun 30 12:01:47 2023, max compression
+gzip compressed data, was "lingtrain-aligner-0.9.2.tar", last modified: Mon Jul 24 12:50:16 2023, max compression
```

## Comparing `lingtrain-aligner-0.9.0.tar` & `lingtrain-aligner-0.9.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 12:01:47.516505 lingtrain-aligner-0.9.0/
--rw-rw-rw-   0        0        0    35823 2021-04-21 06:49:05.000000 lingtrain-aligner-0.9.0/LICENSE
--rw-rw-rw-   0        0        0     3615 2023-06-30 12:01:47.516505 lingtrain-aligner-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     2983 2022-09-06 07:40:35.000000 lingtrain-aligner-0.9.0/README.md
--rw-rw-rw-   0        0        0      108 2021-04-21 06:57:56.000000 lingtrain-aligner-0.9.0/pyproject.toml
--rw-rw-rw-   0        0        0      760 2023-06-30 12:01:47.517504 lingtrain-aligner-0.9.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-30 12:01:47.486507 lingtrain-aligner-0.9.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-30 12:01:47.513505 lingtrain-aligner-0.9.0/src/lingtrain_aligner/
--rw-rw-rw-   0        0        0        0 2023-06-29 08:45:54.000000 lingtrain-aligner-0.9.0/src/lingtrain_aligner/__init__.py
--rw-rw-rw-   0        0        0    37462 2023-06-29 15:29:13.000000 lingtrain-aligner-0.9.0/src/lingtrain_aligner/aligner.py
--rw-rw-rw-   0        0        0      166 2023-06-29 14:28:21.000000 lingtrain-aligner-0.9.0/src/lingtrain_aligner/constants.py
--rw-rw-rw-   0        0        0    19245 2023-06-29 09:32:54.000000 lingtrain-aligner-0.9.0/src/lingtrain_aligner/helper.py
--rw-rw-rw-   0        0        0      851 2023-06-29 08:45:54.000000 lingtrain-aligner-0.9.0/src/lingtrain_aligner/i18n.py
--rw-rw-rw-   0        0        0     1437 2023-06-29 08:45:54.000000 lingtrain-aligner-0.9.0/src/lingtrain_aligner/metrics.py
--rw-rw-rw-   0        0        0      651 2023-06-29 08:45:54.000000 lingtrain-aligner-0.9.0/src/lingtrain_aligner/model_dispatcher.py
--rw-rw-rw-   0        0        0     6417 2023-06-29 14:25:57.000000 lingtrain-aligner-0.9.0/src/lingtrain_aligner/preprocessor.py
--rw-rw-rw-   0        0        0    40680 2023-06-30 11:59:12.000000 lingtrain-aligner-0.9.0/src/lingtrain_aligner/reader.py
--rw-rw-rw-   0        0        0    14421 2023-06-29 08:45:54.000000 lingtrain-aligner-0.9.0/src/lingtrain_aligner/resolver.py
--rw-rw-rw-   0        0        0    16020 2023-06-29 08:45:54.000000 lingtrain-aligner-0.9.0/src/lingtrain_aligner/saver.py
--rw-rw-rw-   0        0        0     5607 2023-06-29 08:45:54.000000 lingtrain-aligner-0.9.0/src/lingtrain_aligner/sententense_transformers_models.py
--rw-rw-rw-   0        0        0     8412 2023-06-29 08:45:54.000000 lingtrain-aligner-0.9.0/src/lingtrain_aligner/splitter.py
--rw-rw-rw-   0        0        0     6953 2023-06-29 14:26:06.000000 lingtrain-aligner-0.9.0/src/lingtrain_aligner/vis_helper.py
-drwxrwxrwx   0        0        0        0 2023-06-30 12:01:47.515505 lingtrain-aligner-0.9.0/src/lingtrain_aligner.egg-info/
--rw-rw-rw-   0        0        0     3615 2023-06-30 12:01:47.000000 lingtrain-aligner-0.9.0/src/lingtrain_aligner.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      723 2023-06-30 12:01:47.000000 lingtrain-aligner-0.9.0/src/lingtrain_aligner.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 12:01:47.000000 lingtrain-aligner-0.9.0/src/lingtrain_aligner.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-06-30 12:01:47.000000 lingtrain-aligner-0.9.0/src/lingtrain_aligner.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 12:50:16.017647 lingtrain-aligner-0.9.2/
+-rw-rw-rw-   0        0        0    35823 2021-04-21 06:49:05.000000 lingtrain-aligner-0.9.2/LICENSE
+-rw-rw-rw-   0        0        0     3615 2023-07-24 12:50:16.017647 lingtrain-aligner-0.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2983 2022-09-06 07:40:35.000000 lingtrain-aligner-0.9.2/README.md
+-rw-rw-rw-   0        0        0      108 2021-04-21 06:57:56.000000 lingtrain-aligner-0.9.2/pyproject.toml
+-rw-rw-rw-   0        0        0      760 2023-07-24 12:50:16.018647 lingtrain-aligner-0.9.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-24 12:50:16.001647 lingtrain-aligner-0.9.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-24 12:50:16.014646 lingtrain-aligner-0.9.2/src/lingtrain_aligner/
+-rw-rw-rw-   0        0        0        0 2023-06-29 08:45:54.000000 lingtrain-aligner-0.9.2/src/lingtrain_aligner/__init__.py
+-rw-rw-rw-   0        0        0    37464 2023-07-24 12:49:21.000000 lingtrain-aligner-0.9.2/src/lingtrain_aligner/aligner.py
+-rw-rw-rw-   0        0        0      166 2023-06-29 14:28:21.000000 lingtrain-aligner-0.9.2/src/lingtrain_aligner/constants.py
+-rw-rw-rw-   0        0        0    19245 2023-06-29 09:32:54.000000 lingtrain-aligner-0.9.2/src/lingtrain_aligner/helper.py
+-rw-rw-rw-   0        0        0      851 2023-06-29 08:45:54.000000 lingtrain-aligner-0.9.2/src/lingtrain_aligner/i18n.py
+-rw-rw-rw-   0        0        0     1437 2023-06-29 08:45:54.000000 lingtrain-aligner-0.9.2/src/lingtrain_aligner/metrics.py
+-rw-rw-rw-   0        0        0      651 2023-06-29 08:45:54.000000 lingtrain-aligner-0.9.2/src/lingtrain_aligner/model_dispatcher.py
+-rw-rw-rw-   0        0        0     6417 2023-06-29 14:25:57.000000 lingtrain-aligner-0.9.2/src/lingtrain_aligner/preprocessor.py
+-rw-rw-rw-   0        0        0    40680 2023-06-30 11:59:12.000000 lingtrain-aligner-0.9.2/src/lingtrain_aligner/reader.py
+-rw-rw-rw-   0        0        0    14421 2023-06-29 08:45:54.000000 lingtrain-aligner-0.9.2/src/lingtrain_aligner/resolver.py
+-rw-rw-rw-   0        0        0    16020 2023-06-29 08:45:54.000000 lingtrain-aligner-0.9.2/src/lingtrain_aligner/saver.py
+-rw-rw-rw-   0        0        0     5607 2023-06-29 08:45:54.000000 lingtrain-aligner-0.9.2/src/lingtrain_aligner/sententense_transformers_models.py
+-rw-rw-rw-   0        0        0     8412 2023-06-29 08:45:54.000000 lingtrain-aligner-0.9.2/src/lingtrain_aligner/splitter.py
+-rw-rw-rw-   0        0        0     6953 2023-06-29 14:26:06.000000 lingtrain-aligner-0.9.2/src/lingtrain_aligner/vis_helper.py
+drwxrwxrwx   0        0        0        0 2023-07-24 12:50:16.016647 lingtrain-aligner-0.9.2/src/lingtrain_aligner.egg-info/
+-rw-rw-rw-   0        0        0     3615 2023-07-24 12:50:15.000000 lingtrain-aligner-0.9.2/src/lingtrain_aligner.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      723 2023-07-24 12:50:15.000000 lingtrain-aligner-0.9.2/src/lingtrain_aligner.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 12:50:15.000000 lingtrain-aligner-0.9.2/src/lingtrain_aligner.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-07-24 12:50:15.000000 lingtrain-aligner-0.9.2/src/lingtrain_aligner.egg-info/top_level.txt
```

### Comparing `lingtrain-aligner-0.9.0/LICENSE` & `lingtrain-aligner-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lingtrain-aligner-0.9.0/PKG-INFO` & `lingtrain-aligner-0.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lingtrain-aligner
-Version: 0.9.0
+Version: 0.9.2
 Summary: Alignment tool for texts in different languages
 Home-page: https://github.com/averkij/lingtrain-aligner
 Author: Sergei Averkiev
 Author-email: averoo@gmail.com
 Project-URL: Bug Tracker, https://github.com/averkij/lingtrain-aligner/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `lingtrain-aligner-0.9.0/README.md` & `lingtrain-aligner-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `lingtrain-aligner-0.9.0/setup.cfg` & `lingtrain-aligner-0.9.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206c 696e 6774 7261 696e 2d61 6c69   = lingtrain-ali
 00000020: 676e 6572 0d0a 7665 7273 696f 6e20 3d20  gner..version = 
-00000030: 302e 392e 300d 0a61 7574 686f 7220 3d20  0.9.0..author = 
+00000030: 302e 392e 320d 0a61 7574 686f 7220 3d20  0.9.2..author = 
 00000040: 5365 7267 6569 2041 7665 726b 6965 760d  Sergei Averkiev.
 00000050: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000060: 6176 6572 6f6f 4067 6d61 696c 2e63 6f6d  averoo@gmail.com
 00000070: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000080: 416c 6967 6e6d 656e 7420 746f 6f6c 2066  Alignment tool f
 00000090: 6f72 2074 6578 7473 2069 6e20 6469 6666  or texts in diff
 000000a0: 6572 656e 7420 6c61 6e67 7561 6765 730d  erent languages.
```

### Comparing `lingtrain-aligner-0.9.0/src/lingtrain_aligner/aligner.py` & `lingtrain-aligner-0.9.2/src/lingtrain_aligner/aligner.py`

 * *Files 0% similar despite different names*

```diff
@@ -400,27 +400,27 @@
 
 
 def get_splitted_from_by_par_with_line_id(db_path, par_id_start, par_id_end):
     """Get lines from splitted_from by paragraphs"""
     with sqlite3.connect(db_path) as db:
         res = db.execute(
             f"""select f.id, f.text from splitted_from f
-                                where paragraph > ? and paragraph < ?
+                                where paragraph > ? and paragraph <= ?
                                 order by f.id""",
             (par_id_start, par_id_end),
         ).fetchall()
     return [(x[0], x[1]) for x in res]
 
 
 def get_splitted_to_by_par_with_line_id(db_path, par_id_start, par_id_end):
     """Get lines from splitted_from by paragraphs"""
     with sqlite3.connect(db_path) as db:
         res = db.execute(
             f"""select f.id, f.text from splitted_to f
-                                where paragraph > ? and paragraph < ?
+                                where paragraph > ? and paragraph <= ?
                                 order by f.id""",
             (par_id_start, par_id_end),
         ).fetchall()
     return [(x[0], x[1]) for x in res]
 
 
 def get_proxy_from(db_path):
```

### Comparing `lingtrain-aligner-0.9.0/src/lingtrain_aligner/helper.py` & `lingtrain-aligner-0.9.2/src/lingtrain_aligner/helper.py`

 * *Files identical despite different names*

### Comparing `lingtrain-aligner-0.9.0/src/lingtrain_aligner/i18n.py` & `lingtrain-aligner-0.9.2/src/lingtrain_aligner/i18n.py`

 * *Files identical despite different names*

### Comparing `lingtrain-aligner-0.9.0/src/lingtrain_aligner/metrics.py` & `lingtrain-aligner-0.9.2/src/lingtrain_aligner/metrics.py`

 * *Files identical despite different names*

### Comparing `lingtrain-aligner-0.9.0/src/lingtrain_aligner/model_dispatcher.py` & `lingtrain-aligner-0.9.2/src/lingtrain_aligner/model_dispatcher.py`

 * *Files identical despite different names*

### Comparing `lingtrain-aligner-0.9.0/src/lingtrain_aligner/preprocessor.py` & `lingtrain-aligner-0.9.2/src/lingtrain_aligner/preprocessor.py`

 * *Files identical despite different names*

### Comparing `lingtrain-aligner-0.9.0/src/lingtrain_aligner/reader.py` & `lingtrain-aligner-0.9.2/src/lingtrain_aligner/reader.py`

 * *Files identical despite different names*

### Comparing `lingtrain-aligner-0.9.0/src/lingtrain_aligner/resolver.py` & `lingtrain-aligner-0.9.2/src/lingtrain_aligner/resolver.py`

 * *Files identical despite different names*

### Comparing `lingtrain-aligner-0.9.0/src/lingtrain_aligner/saver.py` & `lingtrain-aligner-0.9.2/src/lingtrain_aligner/saver.py`

 * *Files identical despite different names*

### Comparing `lingtrain-aligner-0.9.0/src/lingtrain_aligner/sententense_transformers_models.py` & `lingtrain-aligner-0.9.2/src/lingtrain_aligner/sententense_transformers_models.py`

 * *Files identical despite different names*

### Comparing `lingtrain-aligner-0.9.0/src/lingtrain_aligner/splitter.py` & `lingtrain-aligner-0.9.2/src/lingtrain_aligner/splitter.py`

 * *Files identical despite different names*

### Comparing `lingtrain-aligner-0.9.0/src/lingtrain_aligner/vis_helper.py` & `lingtrain-aligner-0.9.2/src/lingtrain_aligner/vis_helper.py`

 * *Files identical despite different names*

### Comparing `lingtrain-aligner-0.9.0/src/lingtrain_aligner.egg-info/PKG-INFO` & `lingtrain-aligner-0.9.2/src/lingtrain_aligner.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lingtrain-aligner
-Version: 0.9.0
+Version: 0.9.2
 Summary: Alignment tool for texts in different languages
 Home-page: https://github.com/averkij/lingtrain-aligner
 Author: Sergei Averkiev
 Author-email: averoo@gmail.com
 Project-URL: Bug Tracker, https://github.com/averkij/lingtrain-aligner/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `lingtrain-aligner-0.9.0/src/lingtrain_aligner.egg-info/SOURCES.txt` & `lingtrain-aligner-0.9.2/src/lingtrain_aligner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

