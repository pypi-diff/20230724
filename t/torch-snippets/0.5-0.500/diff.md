# Comparing `tmp/torch_snippets-0.5.tar.gz` & `tmp/torch_snippets-0.500.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_snippets-0.5.tar", last modified: Mon Jul 24 14:55:52 2023, max compression
+gzip compressed data, was "torch_snippets-0.500.tar", last modified: Mon Jul 24 15:26:45 2023, max compression
```

## Comparing `torch_snippets-0.5.tar` & `torch_snippets-0.500.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-07-24 14:55:52.808132 torch_snippets-0.5/
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    11357 2021-12-31 15:06:08.000000 torch_snippets-0.5/LICENSE
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1062 2023-01-17 16:58:23.000000 torch_snippets-0.5/LICENSE.txt
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      111 2021-12-31 15:06:08.000000 torch_snippets-0.5/MANIFEST.in
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5689 2023-07-24 14:55:52.808416 torch_snippets-0.5/PKG-INFO
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     4999 2023-01-17 16:58:23.000000 torch_snippets-0.5/README.md
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      860 2023-07-24 14:53:09.000000 torch_snippets-0.5/settings.ini
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       79 2023-07-24 14:55:52.809464 torch_snippets-0.5/setup.cfg
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     2001 2022-06-03 13:10:38.000000 torch_snippets-0.5/setup.py
-drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-07-24 14:55:52.801138 torch_snippets-0.5/torch_snippets/
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      305 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/__init__.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    46227 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/_modidx.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     4482 2023-01-17 16:58:25.000000 torch_snippets-0.5/torch_snippets/_nbdev.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     6211 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/adapters.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    12112 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/bb_utils.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1436 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/bokeh_loader.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1672 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/charts.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1483 2023-07-24 13:12:35.000000 torch_snippets-0.5/torch_snippets/dates.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1206 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/decorators.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       73 2022-05-07 11:30:59.000000 torch_snippets-0.5/torch_snippets/fastcores.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     4126 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/imgaug_loader.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     3429 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/inspector.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     8376 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/interactive_show.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     4662 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/ipython.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      597 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/load_defaults.py
--rwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    20934 2023-07-24 14:02:41.000000 torch_snippets-0.5/torch_snippets/loader.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     3464 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/logger.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     7555 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/markup.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1654 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/misc.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     9763 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/paths.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1370 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/pdf_loader.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      822 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/registry.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     6144 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/sklegos.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    14237 2023-06-10 19:35:22.000000 torch_snippets-0.5/torch_snippets/text_utils.py
-drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-07-24 14:55:52.805593 torch_snippets-0.5/torch_snippets/thinc_parser/
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/thinc_parser/__init__.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1082 2022-10-16 17:20:20.000000 torch_snippets-0.5/torch_snippets/thinc_parser/parser.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    13258 2022-11-08 11:22:58.000000 torch_snippets-0.5/torch_snippets/torch_loader.py
-drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-07-24 14:55:52.807533 torch_snippets-0.5/torch_snippets/trainer/
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       23 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/trainer/__init__.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     6802 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/trainer/capsule.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1537 2023-07-24 14:55:50.000000 torch_snippets-0.5/torch_snippets/trainer/config.py
-drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-07-24 14:55:52.804443 torch_snippets-0.5/torch_snippets.egg-info/
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5689 2023-07-24 14:55:52.000000 torch_snippets-0.5/torch_snippets.egg-info/PKG-INFO
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1165 2023-07-24 14:55:52.000000 torch_snippets-0.5/torch_snippets.egg-info/SOURCES.txt
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        1 2023-07-24 14:55:52.000000 torch_snippets-0.5/torch_snippets.egg-info/dependency_links.txt
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-01-17 16:58:23.000000 torch_snippets-0.5/torch_snippets.egg-info/not-zip-safe
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      272 2023-07-24 14:55:52.000000 torch_snippets-0.5/torch_snippets.egg-info/requires.txt
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       15 2023-07-24 14:55:52.000000 torch_snippets-0.5/torch_snippets.egg-info/top_level.txt
+drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-07-24 15:26:45.225734 torch_snippets-0.500/
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    11357 2021-12-31 15:06:08.000000 torch_snippets-0.500/LICENSE
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1062 2023-01-17 16:58:23.000000 torch_snippets-0.500/LICENSE.txt
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      111 2021-12-31 15:06:08.000000 torch_snippets-0.500/MANIFEST.in
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5691 2023-07-24 15:26:45.226009 torch_snippets-0.500/PKG-INFO
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     4999 2023-01-17 16:58:23.000000 torch_snippets-0.500/README.md
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      862 2023-07-24 15:26:22.000000 torch_snippets-0.500/settings.ini
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       79 2023-07-24 15:26:45.226663 torch_snippets-0.500/setup.cfg
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     2001 2022-06-03 13:10:38.000000 torch_snippets-0.500/setup.py
+drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-07-24 15:26:45.220080 torch_snippets-0.500/torch_snippets/
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      307 2023-07-24 15:26:43.000000 torch_snippets-0.500/torch_snippets/__init__.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    46227 2023-07-24 15:26:43.000000 torch_snippets-0.500/torch_snippets/_modidx.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     4482 2023-01-17 16:58:25.000000 torch_snippets-0.500/torch_snippets/_nbdev.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     6211 2023-07-24 15:26:42.000000 torch_snippets-0.500/torch_snippets/adapters.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    12112 2023-07-24 15:26:42.000000 torch_snippets-0.500/torch_snippets/bb_utils.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1436 2023-07-24 15:26:42.000000 torch_snippets-0.500/torch_snippets/bokeh_loader.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1672 2023-07-24 15:26:42.000000 torch_snippets-0.500/torch_snippets/charts.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1483 2023-07-24 13:12:35.000000 torch_snippets-0.500/torch_snippets/dates.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1206 2023-07-24 15:26:42.000000 torch_snippets-0.500/torch_snippets/decorators.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       73 2022-05-07 11:30:59.000000 torch_snippets-0.500/torch_snippets/fastcores.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     4126 2023-07-24 15:26:42.000000 torch_snippets-0.500/torch_snippets/imgaug_loader.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     3429 2023-07-24 15:26:42.000000 torch_snippets-0.500/torch_snippets/inspector.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     8376 2023-07-24 15:26:43.000000 torch_snippets-0.500/torch_snippets/interactive_show.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     4662 2023-07-24 15:26:43.000000 torch_snippets-0.500/torch_snippets/ipython.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      597 2023-07-24 15:26:43.000000 torch_snippets-0.500/torch_snippets/load_defaults.py
+-rwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    20934 2023-07-24 14:02:41.000000 torch_snippets-0.500/torch_snippets/loader.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     3464 2023-07-24 15:26:43.000000 torch_snippets-0.500/torch_snippets/logger.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     7555 2023-07-24 15:26:43.000000 torch_snippets-0.500/torch_snippets/markup.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1654 2023-07-24 15:26:43.000000 torch_snippets-0.500/torch_snippets/misc.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     9763 2023-07-24 15:26:43.000000 torch_snippets-0.500/torch_snippets/paths.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1370 2023-07-24 15:26:43.000000 torch_snippets-0.500/torch_snippets/pdf_loader.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      822 2023-07-24 15:26:43.000000 torch_snippets-0.500/torch_snippets/registry.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     6144 2023-07-24 15:26:43.000000 torch_snippets-0.500/torch_snippets/sklegos.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    14237 2023-06-10 19:35:22.000000 torch_snippets-0.500/torch_snippets/text_utils.py
+drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-07-24 15:26:45.223736 torch_snippets-0.500/torch_snippets/thinc_parser/
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-07-24 15:26:43.000000 torch_snippets-0.500/torch_snippets/thinc_parser/__init__.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1082 2022-10-16 17:20:20.000000 torch_snippets-0.500/torch_snippets/thinc_parser/parser.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    13258 2022-11-08 11:22:58.000000 torch_snippets-0.500/torch_snippets/torch_loader.py
+drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-07-24 15:26:45.225159 torch_snippets-0.500/torch_snippets/trainer/
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       23 2023-07-24 15:26:43.000000 torch_snippets-0.500/torch_snippets/trainer/__init__.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     6802 2023-07-24 15:26:42.000000 torch_snippets-0.500/torch_snippets/trainer/capsule.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1537 2023-07-24 15:26:42.000000 torch_snippets-0.500/torch_snippets/trainer/config.py
+drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-07-24 15:26:45.222803 torch_snippets-0.500/torch_snippets.egg-info/
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5691 2023-07-24 15:26:45.000000 torch_snippets-0.500/torch_snippets.egg-info/PKG-INFO
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1165 2023-07-24 15:26:45.000000 torch_snippets-0.500/torch_snippets.egg-info/SOURCES.txt
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        1 2023-07-24 15:26:45.000000 torch_snippets-0.500/torch_snippets.egg-info/dependency_links.txt
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-01-17 16:58:23.000000 torch_snippets-0.500/torch_snippets.egg-info/not-zip-safe
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      272 2023-07-24 15:26:45.000000 torch_snippets-0.500/torch_snippets.egg-info/requires.txt
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       15 2023-07-24 15:26:45.000000 torch_snippets-0.500/torch_snippets.egg-info/top_level.txt
```

### Comparing `torch_snippets-0.5/LICENSE` & `torch_snippets-0.500/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.5/LICENSE.txt` & `torch_snippets-0.500/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.5/PKG-INFO` & `torch_snippets-0.500/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch_snippets
-Version: 0.5
+Version: 0.500
 Summary: One line functions for common tasks
 Home-page: https://github.com/sizhky/torch_snippets/tree/master/
 Author: Yeshwanth Reddy
 Author-email: 1992chinna@gmail.com
 License: Apache Software License 2.0
 Keywords: snippets,torch
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `torch_snippets-0.5/README.md` & `torch_snippets-0.500/README.md`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.5/settings.ini` & `torch_snippets-0.500/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 user = sizhky
 description = One line functions for common tasks
 keywords = snippets, torch
 author = Yeshwanth Reddy
 author_email = 1992chinna@gmail.com
 copyright = sizhky
 branch = master
-version = 0.5
+version = 0.500
 min_python = 3.7
 audience = Developers
 language = English
 custom_sidebar = False
 license = apache2
 status = 2
 requirements = fastcore matplotlib Pillow altair dill ipython loguru numpy pandas tqdm rich PyYAML catalogue confection pydantic typing srsly typing_extensions wasabi jsonlines imgaug>=0.4.0 xmltodict fuzzywuzzy scikit-learn nltk python-Levenshtein pre-commit pymupdf nbconvert nbformat
```

### Comparing `torch_snippets-0.5/setup.py` & `torch_snippets-0.500/setup.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.5/torch_snippets/_modidx.py` & `torch_snippets-0.500/torch_snippets/_modidx.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.5/torch_snippets/_nbdev.py` & `torch_snippets-0.500/torch_snippets/_nbdev.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.5/torch_snippets/adapters.py` & `torch_snippets-0.500/torch_snippets/adapters.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.5/torch_snippets/bb_utils.py` & `torch_snippets-0.500/torch_snippets/bb_utils.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.5/torch_snippets/bokeh_loader.py` & `torch_snippets-0.500/torch_snippets/bokeh_loader.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.5/torch_snippets/charts.py` & `torch_snippets-0.500/torch_snippets/charts.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.5/torch_snippets/dates.py` & `torch_snippets-0.500/torch_snippets/dates.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.5/torch_snippets/decorators.py` & `torch_snippets-0.500/torch_snippets/decorators.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.5/torch_snippets/imgaug_loader.py` & `torch_snippets-0.500/torch_snippets/imgaug_loader.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.5/torch_snippets/inspector.py` & `torch_snippets-0.500/torch_snippets/inspector.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.5/torch_snippets/interactive_show.py` & `torch_snippets-0.500/torch_snippets/interactive_show.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.5/torch_snippets/ipython.py` & `torch_snippets-0.500/torch_snippets/ipython.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.5/torch_snippets/load_defaults.py` & `torch_snippets-0.500/torch_snippets/load_defaults.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.5/torch_snippets/loader.py` & `torch_snippets-0.500/torch_snippets/loader.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.5/torch_snippets/logger.py` & `torch_snippets-0.500/torch_snippets/logger.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.5/torch_snippets/markup.py` & `torch_snippets-0.500/torch_snippets/markup.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.5/torch_snippets/misc.py` & `torch_snippets-0.500/torch_snippets/misc.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.5/torch_snippets/paths.py` & `torch_snippets-0.500/torch_snippets/paths.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.5/torch_snippets/pdf_loader.py` & `torch_snippets-0.500/torch_snippets/pdf_loader.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.5/torch_snippets/registry.py` & `torch_snippets-0.500/torch_snippets/registry.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.5/torch_snippets/sklegos.py` & `torch_snippets-0.500/torch_snippets/sklegos.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.5/torch_snippets/text_utils.py` & `torch_snippets-0.500/torch_snippets/text_utils.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.5/torch_snippets/thinc_parser/parser.py` & `torch_snippets-0.500/torch_snippets/thinc_parser/parser.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.5/torch_snippets/torch_loader.py` & `torch_snippets-0.500/torch_snippets/torch_loader.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.5/torch_snippets/trainer/capsule.py` & `torch_snippets-0.500/torch_snippets/trainer/capsule.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.5/torch_snippets/trainer/config.py` & `torch_snippets-0.500/torch_snippets/trainer/config.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.5/torch_snippets.egg-info/PKG-INFO` & `torch_snippets-0.500/torch_snippets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-snippets
-Version: 0.5
+Version: 0.500
 Summary: One line functions for common tasks
 Home-page: https://github.com/sizhky/torch_snippets/tree/master/
 Author: Yeshwanth Reddy
 Author-email: 1992chinna@gmail.com
 License: Apache Software License 2.0
 Keywords: snippets,torch
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `torch_snippets-0.5/torch_snippets.egg-info/SOURCES.txt` & `torch_snippets-0.500/torch_snippets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

