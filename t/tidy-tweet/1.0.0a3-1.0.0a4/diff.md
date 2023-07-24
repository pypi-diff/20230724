# Comparing `tmp/tidy_tweet-1.0.0a3.tar.gz` & `tmp/tidy_tweet-1.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidy_tweet-1.0.0a3.tar", last modified: Thu Jun 22 05:47:43 2023, max compression
+gzip compressed data, was "tidy_tweet-1.0.0a4.tar", last modified: Mon Jul 24 05:04:22 2023, max compression
```

## Comparing `tidy_tweet-1.0.0a3.tar` & `tidy_tweet-1.0.0a4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:47:43.249827 tidy_tweet-1.0.0a3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:47:43.245827 tidy_tweet-1.0.0a3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:47:43.249827 tidy_tweet-1.0.0a3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/.github/workflows/pypi_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-06-22 05:47:43.253827 tidy_tweet-1.0.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8398 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:47:43.249827 tidy_tweet-1.0.0a3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    14737 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/docs/data_model.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    39299 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/docs/data_model.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/docs/schema.md
--rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/generate_schema_diagram.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-22 05:47:43.253827 tidy_tweet-1.0.0a3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:47:43.245827 tidy_tweet-1.0.0a3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:47:43.249827 tidy_tweet-1.0.0a3/src/tidy_tweet/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/src/tidy_tweet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/src/tidy_tweet/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-22 05:47:43.000000 tidy_tweet-1.0.0a3/src/tidy_tweet/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/src/tidy_tweet/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/src/tidy_tweet/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    17807 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/src/tidy_tweet/tweet_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/src/tidy_tweet/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:47:43.249827 tidy_tweet-1.0.0a3/src/tidy_tweet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-06-22 05:47:43.000000 tidy_tweet-1.0.0a3/src/tidy_tweet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-22 05:47:43.000000 tidy_tweet-1.0.0a3/src/tidy_tweet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 05:47:43.000000 tidy_tweet-1.0.0a3/src/tidy_tweet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-22 05:47:43.000000 tidy_tweet-1.0.0a3/src/tidy_tweet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-22 05:47:43.000000 tidy_tweet-1.0.0a3/src/tidy_tweet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-22 05:47:43.000000 tidy_tweet-1.0.0a3/src/tidy_tweet.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:47:43.249827 tidy_tweet-1.0.0a3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:47:43.249827 tidy_tweet-1.0.0a3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   586918 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/tests/data/ObservatoryTeam.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/tests/test_overall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:04:22.847943 tidy_tweet-1.0.0a4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:04:22.839943 tidy_tweet-1.0.0a4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:04:22.843943 tidy_tweet-1.0.0a4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/.github/workflows/pypi_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-07-24 05:04:22.847943 tidy_tweet-1.0.0a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8398 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:04:22.843943 tidy_tweet-1.0.0a4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    14737 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/docs/data_model.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    39299 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/docs/data_model.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/docs/schema.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/generate_schema_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-24 05:04:22.847943 tidy_tweet-1.0.0a4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:04:22.839943 tidy_tweet-1.0.0a4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:04:22.843943 tidy_tweet-1.0.0a4/src/tidy_tweet/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/src/tidy_tweet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/src/tidy_tweet/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-24 05:04:22.000000 tidy_tweet-1.0.0a4/src/tidy_tweet/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/src/tidy_tweet/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/src/tidy_tweet/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17807 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/src/tidy_tweet/tweet_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/src/tidy_tweet/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:04:22.847943 tidy_tweet-1.0.0a4/src/tidy_tweet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-07-24 05:04:22.000000 tidy_tweet-1.0.0a4/src/tidy_tweet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-24 05:04:22.000000 tidy_tweet-1.0.0a4/src/tidy_tweet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 05:04:22.000000 tidy_tweet-1.0.0a4/src/tidy_tweet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-24 05:04:22.000000 tidy_tweet-1.0.0a4/src/tidy_tweet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-24 05:04:22.000000 tidy_tweet-1.0.0a4/src/tidy_tweet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-24 05:04:22.000000 tidy_tweet-1.0.0a4/src/tidy_tweet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:04:22.847943 tidy_tweet-1.0.0a4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:04:22.847943 tidy_tweet-1.0.0a4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   586918 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/tests/data/ObservatoryTeam.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-24 05:04:05.000000 tidy_tweet-1.0.0a4/tests/test_overall.py
```

### Comparing `tidy_tweet-1.0.0a3/.github/workflows/pypi_publish.yml` & `tidy_tweet-1.0.0a4/.github/workflows/pypi_publish.yml`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a3/.github/workflows/tests.yml` & `tidy_tweet-1.0.0a4/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a3/LICENSE` & `tidy_tweet-1.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a3/PKG-INFO` & `tidy_tweet-1.0.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidy_tweet
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: Tidies Twitter json collected with Twarc into relational tables
 Home-page: https://github.com/QUT-Digital-Observatory/tidy_tweet
 Author: QUT Digital Observatory
 Author-email: digitalobservatory@qut.edu.au
 Project-URL: Bug Tracker, https://github.com/QUT-Digital-Observatory/tidy_tweet/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tidy_tweet-1.0.0a3/README.md` & `tidy_tweet-1.0.0a4/README.md`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a3/contributing.md` & `tidy_tweet-1.0.0a4/contributing.md`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a3/docs/data_model.drawio` & `tidy_tweet-1.0.0a4/docs/data_model.drawio`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a3/docs/data_model.svg` & `tidy_tweet-1.0.0a4/docs/data_model.svg`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a3/docs/schema.md` & `tidy_tweet-1.0.0a4/docs/schema.md`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a3/generate_schema_diagram.py` & `tidy_tweet-1.0.0a4/generate_schema_diagram.py`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a3/setup.cfg` & `tidy_tweet-1.0.0a4/setup.cfg`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a3/src/tidy_tweet/__main__.py` & `tidy_tweet-1.0.0a4/src/tidy_tweet/__main__.py`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a3/src/tidy_tweet/database.py` & `tidy_tweet-1.0.0a4/src/tidy_tweet/database.py`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a3/src/tidy_tweet/processing.py` & `tidy_tweet-1.0.0a4/src/tidy_tweet/processing.py`

 * *Files 18% similar despite different names*

```diff
@@ -97,11 +97,30 @@
         logger.info(f"Loading {filename} into {db_name}")
 
         page_num = 0
         for page in json_fh:
             page_num = page_num + 1
             logger.info(f"Processing page {page_num} of {filename}")
             page_json = json.loads(page)
-            _load_page_object(str(filename), page_json, connection)
+            try:
+                _load_page_object(str(filename), page_json, connection)
+            except Exception as e:
+                raise PageParsingError(filename, page_num) from e
 
         logger.info(f"All {page_num} pages of {filename} processed")
     return page_num
+
+
+class PageParsingError(Exception):
+    file_name: str
+    page_number: int
+
+    def __init__(self, file_name: str, page_number: int, *args):
+        self.file_name = file_name
+        self.page_number = page_number
+
+        super().__init__(*args)
+
+    def __str__(self):
+        return "tidy_tweet encountered an error while parsing page " \
+               f"{self.page_number} of file {self.file_name}"
+
```

### Comparing `tidy_tweet-1.0.0a3/src/tidy_tweet/tweet_mapping.py` & `tidy_tweet-1.0.0a4/src/tidy_tweet/tweet_mapping.py`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a3/src/tidy_tweet/utilities.py` & `tidy_tweet-1.0.0a4/src/tidy_tweet/utilities.py`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a3/src/tidy_tweet.egg-info/PKG-INFO` & `tidy_tweet-1.0.0a4/src/tidy_tweet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidy-tweet
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: Tidies Twitter json collected with Twarc into relational tables
 Home-page: https://github.com/QUT-Digital-Observatory/tidy_tweet
 Author: QUT Digital Observatory
 Author-email: digitalobservatory@qut.edu.au
 Project-URL: Bug Tracker, https://github.com/QUT-Digital-Observatory/tidy_tweet/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tidy_tweet-1.0.0a3/src/tidy_tweet.egg-info/SOURCES.txt` & `tidy_tweet-1.0.0a4/src/tidy_tweet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a3/tests/data/ObservatoryTeam.jsonl` & `tidy_tweet-1.0.0a4/tests/data/ObservatoryTeam.jsonl`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a3/tests/test_cli.py` & `tidy_tweet-1.0.0a4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a3/tests/test_overall.py` & `tidy_tweet-1.0.0a4/tests/test_overall.py`

 * *Files identical despite different names*

