# Comparing `tmp/corus-0.7.0.tar.gz` & `tmp/corus-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/corus-0.7.0.tar", last modified: Tue Jul 28 04:44:29 2020, max compression
+gzip compressed data, was "dist/corus-0.9.0.tar", last modified: Tue Mar  9 09:07:34 2021, max compression
```

## Comparing `corus-0.7.0.tar` & `corus-0.9.0.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 alexkuk    (502) staff       (20)        0 2020-07-28 04:44:29.000000 corus-0.7.0/
-drwxr-xr-x   0 alexkuk    (502) staff       (20)        0 2020-07-28 04:44:29.000000 corus-0.7.0/corus/
--rw-r--r--   0 alexkuk    (502) staff       (20)       32 2019-04-25 12:31:54.000000 corus-0.7.0/corus/__init__.py
--rw-r--r--   0 alexkuk    (502) staff       (20)     2232 2020-07-23 13:56:46.000000 corus-0.7.0/corus/io.py
--rw-r--r--   0 alexkuk    (502) staff       (20)      193 2019-04-21 17:50:11.000000 corus-0.7.0/corus/path.py
--rw-r--r--   0 alexkuk    (502) staff       (20)     3712 2020-03-22 08:29:48.000000 corus-0.7.0/corus/readme.py
--rw-r--r--   0 alexkuk    (502) staff       (20)     1631 2019-05-31 11:59:45.000000 corus-0.7.0/corus/record.py
-drwxr-xr-x   0 alexkuk    (502) staff       (20)        0 2020-07-28 04:44:29.000000 corus-0.7.0/corus/sources/
--rw-r--r--   0 alexkuk    (502) staff       (20)      790 2020-07-23 13:06:01.000000 corus-0.7.0/corus/sources/__init__.py
--rw-r--r--   0 alexkuk    (502) staff       (20)     4460 2020-03-15 09:08:57.000000 corus-0.7.0/corus/sources/bsnlp.py
--rw-r--r--   0 alexkuk    (502) staff       (20)     1892 2020-07-21 04:55:10.000000 corus-0.7.0/corus/sources/buriy.py
--rw-r--r--   0 alexkuk    (502) staff       (20)     3644 2020-03-17 12:49:20.000000 corus-0.7.0/corus/sources/corpora.py
--rw-r--r--   0 alexkuk    (502) staff       (20)     6000 2020-03-15 14:18:35.000000 corus-0.7.0/corus/sources/factru.py
--rw-r--r--   0 alexkuk    (502) staff       (20)     1001 2020-03-15 07:19:07.000000 corus-0.7.0/corus/sources/gareev.py
--rw-r--r--   0 alexkuk    (502) staff       (20)       75 2020-03-17 11:30:56.000000 corus-0.7.0/corus/sources/gramru.py
--rw-r--r--   0 alexkuk    (502) staff       (20)      602 2019-05-01 03:52:21.000000 corus-0.7.0/corus/sources/lenta.py
--rw-r--r--   0 alexkuk    (502) staff       (20)      773 2019-05-01 03:52:27.000000 corus-0.7.0/corus/sources/librusec.py
--rw-r--r--   0 alexkuk    (502) staff       (20)    23901 2020-07-24 12:09:34.000000 corus-0.7.0/corus/sources/meta.py
--rw-r--r--   0 alexkuk    (502) staff       (20)     3661 2020-03-15 07:19:24.000000 corus-0.7.0/corus/sources/mokoron.py
--rw-r--r--   0 alexkuk    (502) staff       (20)     2307 2020-03-17 10:45:12.000000 corus-0.7.0/corus/sources/morphoru.py
--rw-r--r--   0 alexkuk    (502) staff       (20)     1570 2020-03-15 07:24:18.000000 corus-0.7.0/corus/sources/ne5.py
--rw-r--r--   0 alexkuk    (502) staff       (20)     2812 2020-07-24 12:21:47.000000 corus-0.7.0/corus/sources/ods.py
--rw-r--r--   0 alexkuk    (502) staff       (20)     3434 2020-07-23 14:14:58.000000 corus-0.7.0/corus/sources/omnia.py
--rw-r--r--   0 alexkuk    (502) staff       (20)     1638 2019-09-20 09:24:23.000000 corus-0.7.0/corus/sources/persons.py
--rw-r--r--   0 alexkuk    (502) staff       (20)     1918 2020-03-15 07:19:56.000000 corus-0.7.0/corus/sources/ria.py
--rw-r--r--   0 alexkuk    (502) staff       (20)     1264 2020-03-17 16:46:37.000000 corus-0.7.0/corus/sources/russe.py
--rw-r--r--   0 alexkuk    (502) staff       (20)      594 2020-03-17 16:48:28.000000 corus-0.7.0/corus/sources/simlex.py
-drwxr-xr-x   0 alexkuk    (502) staff       (20)        0 2020-07-28 04:44:29.000000 corus-0.7.0/corus/sources/taiga/
--rw-r--r--   0 alexkuk    (502) staff       (20)      306 2019-04-25 12:04:19.000000 corus-0.7.0/corus/sources/taiga/__init__.py
--rw-r--r--   0 alexkuk    (502) staff       (20)     2388 2020-03-15 07:22:36.000000 corus-0.7.0/corus/sources/taiga/arzamas.py
--rw-r--r--   0 alexkuk    (502) staff       (20)     4692 2020-03-15 07:22:47.000000 corus-0.7.0/corus/sources/taiga/common.py
--rw-r--r--   0 alexkuk    (502) staff       (20)     2959 2020-03-15 07:22:54.000000 corus-0.7.0/corus/sources/taiga/fontanka.py
--rw-r--r--   0 alexkuk    (502) staff       (20)     1816 2020-03-15 07:22:59.000000 corus-0.7.0/corus/sources/taiga/interfax.py
--rw-r--r--   0 alexkuk    (502) staff       (20)     1744 2020-03-15 07:23:02.000000 corus-0.7.0/corus/sources/taiga/kp.py
--rw-r--r--   0 alexkuk    (502) staff       (20)     2035 2020-03-15 07:23:06.000000 corus-0.7.0/corus/sources/taiga/lenta.py
--rw-r--r--   0 alexkuk    (502) staff       (20)     2039 2020-03-15 07:23:11.000000 corus-0.7.0/corus/sources/taiga/magazines.py
--rw-r--r--   0 alexkuk    (502) staff       (20)     2126 2020-03-15 07:23:14.000000 corus-0.7.0/corus/sources/taiga/nplus1.py
--rw-r--r--   0 alexkuk    (502) staff       (20)     2503 2020-03-15 07:23:18.000000 corus-0.7.0/corus/sources/taiga/proza.py
--rw-r--r--   0 alexkuk    (502) staff       (20)     2338 2020-03-15 07:23:26.000000 corus-0.7.0/corus/sources/taiga/social.py
--rw-r--r--   0 alexkuk    (502) staff       (20)     1234 2020-03-15 07:23:30.000000 corus-0.7.0/corus/sources/taiga/subtitles.py
--rw-r--r--   0 alexkuk    (502) staff       (20)     1542 2020-03-17 16:50:17.000000 corus-0.7.0/corus/sources/toloka.py
--rw-r--r--   0 alexkuk    (502) staff       (20)     2883 2020-03-17 11:31:12.000000 corus-0.7.0/corus/sources/ud.py
--rw-r--r--   0 alexkuk    (502) staff       (20)     1095 2019-05-31 15:37:01.000000 corus-0.7.0/corus/sources/wiki.py
--rw-r--r--   0 alexkuk    (502) staff       (20)      912 2020-03-15 07:22:27.000000 corus-0.7.0/corus/sources/wikiner.py
-drwxr-xr-x   0 alexkuk    (502) staff       (20)        0 2020-07-28 04:44:29.000000 corus-0.7.0/corus/third/
--rw-r--r--   0 alexkuk    (502) staff       (20)        0 2019-05-01 04:39:56.000000 corus-0.7.0/corus/third/__init__.py
--rw-r--r--   0 alexkuk    (502) staff       (20)   119222 2019-05-01 04:39:47.000000 corus-0.7.0/corus/third/WikiExtractor.py
--rw-r--r--   0 alexkuk    (502) staff       (20)     2214 2020-07-23 10:53:26.000000 corus-0.7.0/corus/zip.py
-drwxr-xr-x   0 alexkuk    (502) staff       (20)        0 2020-07-28 04:44:29.000000 corus-0.7.0/corus.egg-info/
--rw-r--r--   0 alexkuk    (502) staff       (20)        1 2020-07-28 04:44:28.000000 corus-0.7.0/corus.egg-info/dependency_links.txt
--rw-r--r--   0 alexkuk    (502) staff       (20)    38730 2020-07-28 04:44:28.000000 corus-0.7.0/corus.egg-info/PKG-INFO
--rw-r--r--   0 alexkuk    (502) staff       (20)     1193 2020-07-28 04:44:28.000000 corus-0.7.0/corus.egg-info/SOURCES.txt
--rw-r--r--   0 alexkuk    (502) staff       (20)        6 2020-07-28 04:44:28.000000 corus-0.7.0/corus.egg-info/top_level.txt
--rw-r--r--   0 alexkuk    (502) staff       (20)    38730 2020-07-28 04:44:29.000000 corus-0.7.0/PKG-INFO
--rw-r--r--   0 alexkuk    (502) staff       (20)    28183 2020-07-24 12:22:37.000000 corus-0.7.0/README.md
--rw-r--r--   0 alexkuk    (502) staff       (20)      375 2020-07-28 04:44:29.000000 corus-0.7.0/setup.cfg
--rw-r--r--   0 alexkuk    (502) staff       (20)      682 2020-07-28 04:44:19.000000 corus-0.7.0/setup.py
+drwxr-xr-x   0 alexkuk    (502) staff       (20)        0 2021-03-09 09:07:34.000000 corus-0.9.0/
+drwxr-xr-x   0 alexkuk    (502) staff       (20)        0 2021-03-09 09:07:34.000000 corus-0.9.0/corus/
+-rw-r--r--   0 alexkuk    (502) staff       (20)       32 2019-04-25 12:31:54.000000 corus-0.9.0/corus/__init__.py
+-rw-r--r--   0 alexkuk    (502) staff       (20)     2269 2020-11-20 03:48:29.000000 corus-0.9.0/corus/io.py
+-rw-r--r--   0 alexkuk    (502) staff       (20)      193 2019-04-21 17:50:11.000000 corus-0.9.0/corus/path.py
+-rw-r--r--   0 alexkuk    (502) staff       (20)     3712 2020-03-22 08:29:48.000000 corus-0.9.0/corus/readme.py
+-rw-r--r--   0 alexkuk    (502) staff       (20)     1631 2019-05-31 11:59:45.000000 corus-0.9.0/corus/record.py
+drwxr-xr-x   0 alexkuk    (502) staff       (20)        0 2021-03-09 09:07:34.000000 corus-0.9.0/corus/sources/
+-rw-r--r--   0 alexkuk    (502) staff       (20)      885 2020-11-27 10:03:16.000000 corus-0.9.0/corus/sources/__init__.py
+-rw-r--r--   0 alexkuk    (502) staff       (20)     4460 2020-03-15 09:08:57.000000 corus-0.9.0/corus/sources/bsnlp.py
+-rw-r--r--   0 alexkuk    (502) staff       (20)     1892 2020-07-21 04:55:10.000000 corus-0.9.0/corus/sources/buriy.py
+-rw-r--r--   0 alexkuk    (502) staff       (20)     3644 2020-03-17 12:49:20.000000 corus-0.9.0/corus/sources/corpora.py
+-rw-r--r--   0 alexkuk    (502) staff       (20)     6000 2020-03-15 14:18:35.000000 corus-0.9.0/corus/sources/factru.py
+-rw-r--r--   0 alexkuk    (502) staff       (20)     1001 2020-03-15 07:19:07.000000 corus-0.9.0/corus/sources/gareev.py
+-rw-r--r--   0 alexkuk    (502) staff       (20)       75 2020-03-17 11:30:56.000000 corus-0.9.0/corus/sources/gramru.py
+-rw-r--r--   0 alexkuk    (502) staff       (20)      937 2020-11-20 03:56:45.000000 corus-0.9.0/corus/sources/lenta.py
+-rw-r--r--   0 alexkuk    (502) staff       (20)      773 2019-05-01 03:52:27.000000 corus-0.9.0/corus/sources/librusec.py
+-rw-r--r--   0 alexkuk    (502) staff       (20)    26130 2020-11-27 10:07:08.000000 corus-0.9.0/corus/sources/meta.py
+-rw-r--r--   0 alexkuk    (502) staff       (20)     3661 2020-03-15 07:19:24.000000 corus-0.9.0/corus/sources/mokoron.py
+-rw-r--r--   0 alexkuk    (502) staff       (20)     2307 2020-03-17 10:45:12.000000 corus-0.9.0/corus/sources/morphoru.py
+-rw-r--r--   0 alexkuk    (502) staff       (20)     1570 2020-03-15 07:24:18.000000 corus-0.9.0/corus/sources/ne5.py
+-rw-r--r--   0 alexkuk    (502) staff       (20)     2812 2020-07-24 12:21:47.000000 corus-0.9.0/corus/sources/ods.py
+-rw-r--r--   0 alexkuk    (502) staff       (20)     3434 2020-07-23 14:14:58.000000 corus-0.9.0/corus/sources/omnia.py
+-rw-r--r--   0 alexkuk    (502) staff       (20)     1638 2019-09-20 09:24:23.000000 corus-0.9.0/corus/sources/persons.py
+-rw-r--r--   0 alexkuk    (502) staff       (20)     1918 2020-03-15 07:19:56.000000 corus-0.9.0/corus/sources/ria.py
+-rw-r--r--   0 alexkuk    (502) staff       (20)     1576 2020-11-27 10:08:56.000000 corus-0.9.0/corus/sources/rudrec.py
+-rw-r--r--   0 alexkuk    (502) staff       (20)     1264 2020-03-17 16:46:37.000000 corus-0.9.0/corus/sources/russe.py
+-rw-r--r--   0 alexkuk    (502) staff       (20)      594 2020-03-17 16:48:28.000000 corus-0.9.0/corus/sources/simlex.py
+drwxr-xr-x   0 alexkuk    (502) staff       (20)        0 2021-03-09 09:07:34.000000 corus-0.9.0/corus/sources/taiga/
+-rw-r--r--   0 alexkuk    (502) staff       (20)      306 2019-04-25 12:04:19.000000 corus-0.9.0/corus/sources/taiga/__init__.py
+-rw-r--r--   0 alexkuk    (502) staff       (20)     2388 2020-03-15 07:22:36.000000 corus-0.9.0/corus/sources/taiga/arzamas.py
+-rw-r--r--   0 alexkuk    (502) staff       (20)     4692 2020-03-15 07:22:47.000000 corus-0.9.0/corus/sources/taiga/common.py
+-rw-r--r--   0 alexkuk    (502) staff       (20)     2959 2020-03-15 07:22:54.000000 corus-0.9.0/corus/sources/taiga/fontanka.py
+-rw-r--r--   0 alexkuk    (502) staff       (20)     1816 2020-03-15 07:22:59.000000 corus-0.9.0/corus/sources/taiga/interfax.py
+-rw-r--r--   0 alexkuk    (502) staff       (20)     1744 2020-03-15 07:23:02.000000 corus-0.9.0/corus/sources/taiga/kp.py
+-rw-r--r--   0 alexkuk    (502) staff       (20)     2035 2020-03-15 07:23:06.000000 corus-0.9.0/corus/sources/taiga/lenta.py
+-rw-r--r--   0 alexkuk    (502) staff       (20)     2039 2020-03-15 07:23:11.000000 corus-0.9.0/corus/sources/taiga/magazines.py
+-rw-r--r--   0 alexkuk    (502) staff       (20)     2126 2020-03-15 07:23:14.000000 corus-0.9.0/corus/sources/taiga/nplus1.py
+-rw-r--r--   0 alexkuk    (502) staff       (20)     2503 2020-03-15 07:23:18.000000 corus-0.9.0/corus/sources/taiga/proza.py
+-rw-r--r--   0 alexkuk    (502) staff       (20)     2338 2020-03-15 07:23:26.000000 corus-0.9.0/corus/sources/taiga/social.py
+-rw-r--r--   0 alexkuk    (502) staff       (20)     1234 2020-03-15 07:23:30.000000 corus-0.9.0/corus/sources/taiga/subtitles.py
+-rw-r--r--   0 alexkuk    (502) staff       (20)     2281 2020-11-20 03:48:29.000000 corus-0.9.0/corus/sources/toloka.py
+-rw-r--r--   0 alexkuk    (502) staff       (20)     2883 2020-03-17 11:31:12.000000 corus-0.9.0/corus/sources/ud.py
+-rw-r--r--   0 alexkuk    (502) staff       (20)     1095 2019-05-31 15:37:01.000000 corus-0.9.0/corus/sources/wiki.py
+-rw-r--r--   0 alexkuk    (502) staff       (20)      912 2020-03-15 07:22:27.000000 corus-0.9.0/corus/sources/wikiner.py
+drwxr-xr-x   0 alexkuk    (502) staff       (20)        0 2021-03-09 09:07:34.000000 corus-0.9.0/corus/third/
+-rw-r--r--   0 alexkuk    (502) staff       (20)        0 2019-05-01 04:39:56.000000 corus-0.9.0/corus/third/__init__.py
+-rw-r--r--   0 alexkuk    (502) staff       (20)   119222 2019-05-01 04:39:47.000000 corus-0.9.0/corus/third/WikiExtractor.py
+-rw-r--r--   0 alexkuk    (502) staff       (20)     2214 2020-07-23 10:53:26.000000 corus-0.9.0/corus/zip.py
+drwxr-xr-x   0 alexkuk    (502) staff       (20)        0 2021-03-09 09:07:34.000000 corus-0.9.0/corus.egg-info/
+-rw-r--r--   0 alexkuk    (502) staff       (20)        1 2021-03-09 09:07:33.000000 corus-0.9.0/corus.egg-info/dependency_links.txt
+-rw-r--r--   0 alexkuk    (502) staff       (20)    41790 2021-03-09 09:07:33.000000 corus-0.9.0/corus.egg-info/PKG-INFO
+-rw-r--r--   0 alexkuk    (502) staff       (20)     1217 2021-03-09 09:07:33.000000 corus-0.9.0/corus.egg-info/SOURCES.txt
+-rw-r--r--   0 alexkuk    (502) staff       (20)        6 2021-03-09 09:07:33.000000 corus-0.9.0/corus.egg-info/top_level.txt
+-rw-r--r--   0 alexkuk    (502) staff       (20)    41790 2021-03-09 09:07:34.000000 corus-0.9.0/PKG-INFO
+-rw-r--r--   0 alexkuk    (502) staff       (20)    30523 2020-12-24 12:26:33.000000 corus-0.9.0/README.md
+-rw-r--r--   0 alexkuk    (502) staff       (20)      375 2021-03-09 09:07:34.000000 corus-0.9.0/setup.cfg
+-rw-r--r--   0 alexkuk    (502) staff       (20)      682 2021-03-09 09:06:56.000000 corus-0.9.0/setup.py
```

### Comparing `corus-0.7.0/corus/io.py` & `corus-0.9.0/corus/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,16 +42,16 @@
 
 
 def dump_text(text, path):
     with open(path, 'w') as file:
         file.write(text)
 
 
-def load_lines(path):
-    with open(path) as file:
+def load_lines(path, encoding="utf-8"):
+    with open(path, encoding=encoding) as file:
         for line in file:
             yield rstrip(line)
 
 
 #####
 #
 #   XML
```

### Comparing `corus-0.7.0/corus/readme.py` & `corus-0.9.0/corus/readme.py`

 * *Files identical despite different names*

### Comparing `corus-0.7.0/corus/record.py` & `corus-0.9.0/corus/record.py`

 * *Files identical despite different names*

### Comparing `corus-0.7.0/corus/sources/__init__.py` & `corus-0.9.0/corus/sources/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 from .factru import load_factru  # noqa
 from .gareev import load_gareev  # noqa
-from .lenta import load_lenta  # noqa
+from .lenta import load_lenta, load_lenta2  # noqa
 from .librusec import load_librusec  # noqa
 from .ne5 import load_ne5  # noqa
 from .wikiner import load_wikiner  # noqa
 from .bsnlp import load_bsnlp  # noqa
 from .persons import load_persons  # noqa
 from .taiga import *  # noqa
 from .buriy import *  # noqa
@@ -17,7 +17,9 @@
 from .morphoru import *  # noqa
 from .gramru import load_gramru  # noqa
 from .corpora import load_corpora  # noqa
 from .russe import *  # noqa
 from .toloka import load_toloka_lrwc  # noqa
 from .simlex import load_simlex  # noqa
 from .omnia import load_omnia  # noqa
+from .toloka import load_ruadrect  # noqa
+from .rudrec import load_rudrec  # noqa
```

### Comparing `corus-0.7.0/corus/sources/bsnlp.py` & `corus-0.9.0/corus/sources/bsnlp.py`

 * *Files identical despite different names*

### Comparing `corus-0.7.0/corus/sources/buriy.py` & `corus-0.9.0/corus/sources/buriy.py`

 * *Files identical despite different names*

### Comparing `corus-0.7.0/corus/sources/corpora.py` & `corus-0.9.0/corus/sources/corpora.py`

 * *Files identical despite different names*

### Comparing `corus-0.7.0/corus/sources/factru.py` & `corus-0.9.0/corus/sources/factru.py`

 * *Files identical despite different names*

### Comparing `corus-0.7.0/corus/sources/gareev.py` & `corus-0.9.0/corus/sources/gareev.py`

 * *Files identical despite different names*

### Comparing `corus-0.7.0/corus/sources/lenta.py` & `corus-0.9.0/corus/sources/lenta.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,45 @@
 
+from datetime import datetime
+
 from corus.record import Record
 from corus.io import (
     load_gz_lines,
+    load_bz2_lines,
     parse_csv,
     skip_header
 )
 
 
 class LentaRecord(Record):
-    __attributes__ = ['url', 'title', 'text', 'topic', 'tags']
+    __attributes__ = ['url', 'title', 'text', 'topic', 'tags', 'date']
 
-    def __init__(self, url, title, text, topic, tags):
+    def __init__(self, url, title, text, topic, tags, date=None):
         self.url = url
         self.title = title
         self.text = text
         self.topic = topic
         self.tags = tags
+        self.date = date
 
 
 def parse_lenta(lines):
     rows = parse_csv(lines)
     skip_header(rows)
     for cells in rows:
         yield LentaRecord(*cells)
 
 
+def parse_lenta2(lines):
+    for record in parse_lenta(lines):
+        record.date = datetime.strptime(record.date, '%Y/%m/%d')
+        yield record
+
+
 def load_lenta(path):
     lines = load_gz_lines(path)
     return parse_lenta(lines)
+
+
+def load_lenta2(path):
+    lines = load_bz2_lines(path)
+    return parse_lenta2(lines)
```

### Comparing `corus-0.7.0/corus/sources/librusec.py` & `corus-0.9.0/corus/sources/librusec.py`

 * *Files identical despite different names*

### Comparing `corus-0.7.0/corus/sources/meta.py` & `corus-0.9.0/corus/sources/meta.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,23 +4,26 @@
 from . import (
     load_mokoron,
     load_wiki,
     load_simlex,
     load_omnia,
     load_gramru,
     load_corpora,
+    load_ruadrect,
 
     load_factru,
     load_gareev,
     load_lenta,
+    load_lenta2,
     load_librusec,
     load_ne5,
     load_wikiner,
     load_bsnlp,
     load_persons,
+    load_rudrec,
 
     load_taiga_arzamas,
     load_taiga_fontanka,
     load_taiga_interfax,
     load_taiga_kp,
     load_taiga_lenta,
     load_taiga_nplus1,
@@ -109,26 +112,43 @@
 SYNTAX = 'syntax'
 EMB = 'emb'
 SIM = 'sim'
 SENTIMENT = 'sentiment'
 WEB = 'web'
 
 METAS = [
-    Meta(
+    Group(
         title='Lenta.ru',
         url='https://github.com/yutkin/Lenta.Ru-News-Dataset',
-        stats=Stats(
-            bytes=1785632079,
-            count=739351
-        ),
-        instruction=[
-            'wget https://github.com/yutkin/Lenta.Ru-News-Dataset/releases/download/v1.0/lenta-ru-news.csv.gz'
-        ],
-        tags=[NEWS],
-        functions=[load_lenta]
+        metas=[
+            Meta(
+                title='Lenta.ru v1.0',
+                stats=Stats(
+                    bytes=1785632079,
+                    count=739351
+                ),
+                instruction=[
+                    'wget https://github.com/yutkin/Lenta.Ru-News-Dataset/releases/download/v1.0/lenta-ru-news.csv.gz'
+                ],
+                tags=[NEWS],
+                functions=[load_lenta]
+            ),
+            Meta(
+                title='Lenta.ru v1.1+',
+                stats=Stats(
+                    bytes=2084746431,
+                    count=800975
+                ),
+                instruction=[
+                    'wget https://github.com/yutkin/Lenta.Ru-News-Dataset/releases/download/v1.1/lenta-ru-news.csv.bz2'
+                ],
+                tags=[NEWS],
+                functions=[load_lenta2]
+            ),
+        ]
     ),
     Meta(
         title='Lib.rus.ec',
         url='https://russe.nlpub.org/downloads/',
         description='Dump of lib.rus.ec prepared for RUSSE workshop',
         stats=Stats(
             count=301871,
@@ -331,14 +351,33 @@
         ),
         instruction=[
             'wget http://ai-center.botik.ru/Airec/ai-resources/Persons-1000.zip'
         ],
         tags=[NER, NEWS],
         functions=[load_persons]
     ),
+    Meta(
+        title='The Russian Drug Reaction Corpus (RuDReC)',
+        url='https://github.com/cimm-kzn/RuDReC',
+        description=(
+            'RuDReC is a new partially annotated corpus of consumer reviews in Russian about pharmaceutical '
+            'products for the detection of health-related named entities and the effectiveness of pharmaceutical products. '
+            'Here you can download and work with the annotated part, to get the raw part (1.4M reviews) '
+            'please refer to https://github.com/cimm-kzn/RuDReC.'
+        ),
+        stats=Stats(
+            count=4809,
+            bytes=1773
+        ),
+        instruction=[
+            'wget https://github.com/cimm-kzn/RuDReC/raw/master/data/rudrec_annotated.json'
+        ],
+        tags=[NER],
+        functions=[load_rudrec]
+    ),
 
     ##########
     #
     #    TAIGA
     #
     ###########
 
@@ -781,10 +820,27 @@
                     'wget https://tlk.s3.yandex.net/dataset/LRWC.zip',
                     'unzip LRWC.zip',
                     'rm LRWC.zip'
                 ],
                 tags=[EMB, SIM],
                 functions=[load_toloka_lrwc],
             ),
+            Meta(
+                title='The Russian Adverse Drug Reaction Corpus of Tweets (RuADReCT)',
+                url='https://github.com/cimm-kzn/RuDReC',
+                description='This corpus was developed for the Social Media Mining for Health Applications (#SMM4H) '
+                            'Shared Task 2020',
+                instruction=[
+                    'wget https://github.com/cimm-kzn/RuDReC/raw/master/data/RuADReCT.zip',
+                    'unzip RuADReCT.zip',
+                    'rm RuADReCT.zip'
+                ],
+                stats=Stats(
+                    count=9515,
+                    bytes=2190063
+                ),
+                tags=[SOCIAL],
+                functions=[load_ruadrect],
+            ),
         ]
     ),
 ]
```

### Comparing `corus-0.7.0/corus/sources/mokoron.py` & `corus-0.9.0/corus/sources/mokoron.py`

 * *Files identical despite different names*

### Comparing `corus-0.7.0/corus/sources/morphoru.py` & `corus-0.9.0/corus/sources/morphoru.py`

 * *Files identical despite different names*

### Comparing `corus-0.7.0/corus/sources/ne5.py` & `corus-0.9.0/corus/sources/ne5.py`

 * *Files identical despite different names*

### Comparing `corus-0.7.0/corus/sources/ods.py` & `corus-0.9.0/corus/sources/ods.py`

 * *Files identical despite different names*

### Comparing `corus-0.7.0/corus/sources/omnia.py` & `corus-0.9.0/corus/sources/omnia.py`

 * *Files identical despite different names*

### Comparing `corus-0.7.0/corus/sources/persons.py` & `corus-0.9.0/corus/sources/persons.py`

 * *Files identical despite different names*

### Comparing `corus-0.7.0/corus/sources/ria.py` & `corus-0.9.0/corus/sources/ria.py`

 * *Files identical despite different names*

### Comparing `corus-0.7.0/corus/sources/russe.py` & `corus-0.9.0/corus/sources/russe.py`

 * *Files identical despite different names*

### Comparing `corus-0.7.0/corus/sources/simlex.py` & `corus-0.9.0/corus/sources/simlex.py`

 * *Files identical despite different names*

### Comparing `corus-0.7.0/corus/sources/taiga/arzamas.py` & `corus-0.9.0/corus/sources/taiga/arzamas.py`

 * *Files identical despite different names*

### Comparing `corus-0.7.0/corus/sources/taiga/common.py` & `corus-0.9.0/corus/sources/taiga/common.py`

 * *Files identical despite different names*

### Comparing `corus-0.7.0/corus/sources/taiga/fontanka.py` & `corus-0.9.0/corus/sources/taiga/fontanka.py`

 * *Files identical despite different names*

### Comparing `corus-0.7.0/corus/sources/taiga/interfax.py` & `corus-0.9.0/corus/sources/taiga/interfax.py`

 * *Files identical despite different names*

### Comparing `corus-0.7.0/corus/sources/taiga/kp.py` & `corus-0.9.0/corus/sources/taiga/kp.py`

 * *Files identical despite different names*

### Comparing `corus-0.7.0/corus/sources/taiga/lenta.py` & `corus-0.9.0/corus/sources/taiga/lenta.py`

 * *Files identical despite different names*

### Comparing `corus-0.7.0/corus/sources/taiga/magazines.py` & `corus-0.9.0/corus/sources/taiga/magazines.py`

 * *Files identical despite different names*

### Comparing `corus-0.7.0/corus/sources/taiga/nplus1.py` & `corus-0.9.0/corus/sources/taiga/nplus1.py`

 * *Files identical despite different names*

### Comparing `corus-0.7.0/corus/sources/taiga/proza.py` & `corus-0.9.0/corus/sources/taiga/proza.py`

 * *Files identical despite different names*

### Comparing `corus-0.7.0/corus/sources/taiga/social.py` & `corus-0.9.0/corus/sources/taiga/social.py`

 * *Files identical despite different names*

### Comparing `corus-0.7.0/corus/sources/taiga/subtitles.py` & `corus-0.9.0/corus/sources/taiga/subtitles.py`

 * *Files identical despite different names*

### Comparing `corus-0.7.0/corus/sources/ud.py` & `corus-0.9.0/corus/sources/ud.py`

 * *Files identical despite different names*

### Comparing `corus-0.7.0/corus/sources/wiki.py` & `corus-0.9.0/corus/sources/wiki.py`

 * *Files identical despite different names*

### Comparing `corus-0.7.0/corus/sources/wikiner.py` & `corus-0.9.0/corus/sources/wikiner.py`

 * *Files identical despite different names*

### Comparing `corus-0.7.0/corus/third/WikiExtractor.py` & `corus-0.9.0/corus/third/WikiExtractor.py`

 * *Files identical despite different names*

### Comparing `corus-0.7.0/corus/zip.py` & `corus-0.9.0/corus/zip.py`

 * *Files identical despite different names*

### Comparing `corus-0.7.0/corus.egg-info/PKG-INFO` & `corus-0.9.0/corus.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corus
-Version: 0.7.0
+Version: 0.9.0
 Summary: Links to russian corpora, functions for loading and parsing
 Home-page: https://github.com/natasha/corus
 Author: Alexander Kukushkin
 Author-email: alex@alexkuk.ru
 License: MIT
 Description: 
         <img src="https://github.com/natasha/natasha-logos/blob/master/corus.svg">
@@ -46,14 +46,21 @@
         ...     text = record.text
         ...     ...
         
         ```
         
         For links to other datasets and their loaders see the <a href="#reference">Reference</a> section.
         
+        ## Documentation
+        
+        Materials are in Russian:
+        
+        * <a href="https://natasha.github.io/corus">Corus page on natasha.github.io</a> 
+        * <a href="https://youtu.be/-7XT_U6hVvk?t=2758">Corus section of Datafest 2020 talk</a>
+        
         ## Install
         
         `corus` supports Python 3.5+, PyPy 3.
         
         ```bash
         $ pip install corus
         ```
@@ -70,14 +77,21 @@
         <th>Uncompressed</th>
         <th>Description</th>
         </tr>
         <tr>
         <td>
         <a href="https://github.com/yutkin/Lenta.Ru-News-Dataset">Lenta.ru</a>
         </td>
+        <td colspan="5">
+        </td>
+        </tr>
+        <tr>
+        <td>
+        Lenta.ru v1.0
+        </td>
         <td>
         <a name="load_lenta"></a>
         <code><a href="https://nbviewer.jupyter.org/github/natasha/corus/blob/master/docs.ipynb#load_lenta">load_lenta</a></code>
         <a href="#load_lenta"><code>#</code></a>
         </td>
         <td>
         <code>news</code>
@@ -90,14 +104,36 @@
         </td>
         <td>
         <code>wget https://github.com/yutkin/Lenta.Ru-News-Dataset/releases/download/v1.0/lenta-ru-news.csv.gz</code>
         </td>
         </tr>
         <tr>
         <td>
+        Lenta.ru v1.1+
+        </td>
+        <td>
+        <a name="load_lenta2"></a>
+        <code><a href="https://nbviewer.jupyter.org/github/natasha/corus/blob/master/docs.ipynb#load_lenta2">load_lenta2</a></code>
+        <a href="#load_lenta2"><code>#</code></a>
+        </td>
+        <td>
+        <code>news</code>
+        </td>
+        <td align="right">
+        800&nbsp;975
+        </td>
+        <td align="right">
+        1.94 Gb
+        </td>
+        <td>
+        <code>wget https://github.com/yutkin/Lenta.Ru-News-Dataset/releases/download/v1.1/lenta-ru-news.csv.bz2</code>
+        </td>
+        </tr>
+        <tr>
+        <td>
         <a href="https://russe.nlpub.org/downloads/">Lib.rus.ec</a>
         </td>
         <td>
         <a name="load_librusec"></a>
         <code><a href="https://nbviewer.jupyter.org/github/natasha/corus/blob/master/docs.ipynb#load_librusec">load_librusec</a></code>
         <a href="#load_librusec"><code>#</code></a>
         </td>
@@ -467,14 +503,39 @@
         </br>
         </br>
         <code>wget http://ai-center.botik.ru/Airec/ai-resources/Persons-1000.zip</code>
         </td>
         </tr>
         <tr>
         <td>
+        <a href="https://github.com/cimm-kzn/RuDReC">The Russian Drug Reaction Corpus (RuDReC)</a>
+        </td>
+        <td>
+        <a name="load_rudrec"></a>
+        <code><a href="https://nbviewer.jupyter.org/github/natasha/corus/blob/master/docs.ipynb#load_rudrec">load_rudrec</a></code>
+        <a href="#load_rudrec"><code>#</code></a>
+        </td>
+        <td>
+        <code>ner</code>
+        </td>
+        <td align="right">
+        4&nbsp;809
+        </td>
+        <td align="right">
+        1.73 Kb
+        </td>
+        <td>
+        RuDReC is a new partially annotated corpus of consumer reviews in Russian about pharmaceutical products for the detection of health-related named entities and the effectiveness of pharmaceutical products. Here you can download and work with the annotated part, to get the raw part (1.4M reviews) please refer to https://github.com/cimm-kzn/RuDReC.
+        </br>
+        </br>
+        <code>wget https://github.com/cimm-kzn/RuDReC/raw/master/data/rudrec_annotated.json</code>
+        </td>
+        </tr>
+        <tr>
+        <td>
         <a href="https://tatianashavrina.github.io/taiga_site/">Taiga</a>
         </td>
         <td colspan="5">
         Large collection of Russian texts from various sources: news sites, magazines, literacy, social networks
         </br>
         </br>
         <code>wget https://linghub.ru/static/Taiga/retagged_taiga.tar.gz</code>
@@ -1232,14 +1293,43 @@
         <code>wget https://tlk.s3.yandex.net/dataset/LRWC.zip</code>
         </br>
         <code>unzip LRWC.zip</code>
         </br>
         <code>rm LRWC.zip</code>
         </td>
         </tr>
+        <tr>
+        <td>
+        <a href="https://github.com/cimm-kzn/RuDReC">The Russian Adverse Drug Reaction Corpus of Tweets (RuADReCT)</a>
+        </td>
+        <td>
+        <a name="load_ruadrect"></a>
+        <code><a href="https://nbviewer.jupyter.org/github/natasha/corus/blob/master/docs.ipynb#load_ruadrect">load_ruadrect</a></code>
+        <a href="#load_ruadrect"><code>#</code></a>
+        </td>
+        <td>
+        <code>social</code>
+        </td>
+        <td align="right">
+        9&nbsp;515
+        </td>
+        <td align="right">
+        2.09 Mb
+        </td>
+        <td>
+        This corpus was developed for the Social Media Mining for Health Applications (#SMM4H) Shared Task 2020
+        </br>
+        </br>
+        <code>wget https://github.com/cimm-kzn/RuDReC/raw/master/data/RuADReCT.zip</code>
+        </br>
+        <code>unzip RuADReCT.zip</code>
+        </br>
+        <code>rm RuADReCT.zip</code>
+        </td>
+        </tr>
         </table>
         <!--- metas --->
         
         ## Support
         
         - Chat — https://telegram.me/natural_language_processing
         - Issues — https://github.com/natasha/corus/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: corus Version: 0.7.0 Summary: Links to russian
+Metadata-Version: 2.1 Name: corus Version: 0.9.0 Summary: Links to russian
 corpora, functions for loading and parsing Home-page: https://github.com/
 natasha/corus Author: Alexander Kukushkin Author-email: alex@alexkuk.ru
 License: MIT Description: [https://github.com/natasha/natasha-logos/blob/
 master/corus.svg] ![CI](https://github.com/natasha/corus/workflows/CI/
 badge.svg) [![codecov](https://codecov.io/gh/natasha/corus/branch/master/graph/
 badge.svg)](https://codecov.io/gh/natasha/corus) Links to publicly available
 Russian corpora + code for loading and parsing. 20+_datasets,_350Gb+_of_text.
@@ -17,20 +17,25 @@
 Ð¿ÑÐµÐ¼ÑÐµÑ Ð¿Ð¾ ÑÐ¾ÑÐ¸Ð°Ð»ÑÐ½ÑÐ¼ Ð²Ð¾Ð¿ÑÐ¾ÑÐ°Ð¼ Ð¢Ð°ÑÑÑÐ½Ð°
 ÐÐ¾Ð»Ð¸ÐºÐ¾Ð²Ð° ÑÐ°ÑÑÐºÐ°Ð·Ð°Ð»Ð°, Ð² ÐºÐ°ÐºÐ¸Ñ ÑÐµÐ³Ð¸Ð¾Ð½Ð°Ñ
 Ð Ð¾ÑÑÐ¸Ð¸ Ð·Ð°ÑÐ¸ÐºÑÐ¸ÑÐ¾Ð²Ð°Ð½Ð° Ð½Ð°Ð¸Ð±Ð¾Ð»ÐµÐµ Ð²ÑÑÐ¾ÐºÐ°Ñ
 ÑÐ¼ÐµÑÑÐ½Ð¾ÑÑÑ Ð¾Ñ ÑÐ°ÐºÐ°, ÑÐ¾Ð¾Ð±...', topic='Ð Ð¾ÑÑÐ¸Ñ',
 tags='ÐÐ±ÑÐµÑÑÐ²Ð¾' ) ``` Iterate over texts: ```python >>> records =
 load_lenta(path) >>> for record in records: ... text = record.text ... ... ```
 For links to other datasets and their loaders see the Reference section. ##
-Install `corus` supports Python 3.5+, PyPy 3. ```bash $ pip install corus ```
-## Reference
+Documentation Materials are in Russian: * Corus_page_on_natasha.github.io *
+Corus_section_of_Datafest_2020_talk ## Install `corus` supports Python 3.5+,
+PyPy 3. ```bash $ pip install corus ``` ## Reference
 Dataset        API from corus import  Tags      Texts      Uncompressed Description
+Lenta.ru
                                                                         wget https://github.com/yutkin/
-Lenta.ru        load_lenta #          news         739 351     1.66 Gb Lenta.Ru-News-Dataset/releases/
+Lenta.ru v1.0   load_lenta #          news         739 351     1.66 Gb Lenta.Ru-News-Dataset/releases/
                                                                         download/v1.0/lenta-ru-news.csv.gz
+                                                                        wget https://github.com/yutkin/
+Lenta.ru v1.1+  load_lenta2 #         news         800 975     1.94 Gb Lenta.Ru-News-Dataset/releases/
+                                                                        download/v1.1/lenta-ru-news.csv.bz2
                                                                         Dump of lib.rus.ec prepared for RUSSE
 Lib.rus.ec      load_librusec #       fiction      301 871   144.92 Gb workshop   wget http://panchenko.me/
                                                                         data/russe/librusec_fb2.plain.gz
 Rossiya         load_ria_raw #                                          wget https://github.com/
 Segodnya       load_ria #             news       1 003 86     3.70 Gb RossiyaSegodnya/ria_news_dataset/raw/
                                                                         master/ria.json.gz
 Mokoron                                                                 Russian Twitter sentiment markup
@@ -92,14 +97,26 @@
                                                                         d test_pl_cs_ru_bg  rm
                                                                         TRAININGDATA_BSNLP_2019_shared_task.zip
                                                                         TESTDATA_BSNLP_2019_shared_task.zip
                                                                         Same as Collection5, only PER markup +
 Persons-1000    load_persons #        ner news       1 000     2.96 Mb normalized names   wget http://ai-
                                                                         center.botik.ru/Airec/ai-resources/
                                                                         Persons-1000.zip
+                                                                        RuDReC is a new partially annotated
+                                                                        corpus of consumer reviews in Russian
+                                                                        about pharmaceutical products for the
+                                                                        detection of health-related named
+The_Russian                                                             entities and the effectiveness of
+Drug_Reaction   load_rudrec #         ner            4 809     1.73 Kb pharmaceutical products. Here you can
+Corpus_                                                                 download and work with the annotated
+(RuDReC)                                                                part, to get the raw part (1.4M
+                                                                        reviews) please refer to https://
+                                                                        github.com/cimm-kzn/RuDReC.   wget
+                                                                        https://github.com/cimm-kzn/RuDReC/raw/
+                                                                        master/data/rudrec_annotated.json
                Large collection of Russian texts from various sources: news sites, magazines, literacy, social
 Taiga          networks   wget https://linghub.ru/static/Taiga/retagged_taiga.tar.gz  tar -xzvf
                retagged_taiga.tar.gz
 Arzamas         load_taiga_arzamas #  news             311      4.50 Mb
 Fontanka        load_taiga_fontanka # news         342 683   786.23 Mb
 Interfax        load_taiga_interfax # news          46 429    77.55 Mb
 KP              load_taiga_kp #       news          45 503    61.79 Mb
@@ -222,14 +239,20 @@
 Toloka
 Datasets
 Lexical
 Relations from                                                          wget https://tlk.s3.yandex.net/dataset/
 the Wisdom of   load_toloka_lrwc #    emb sim                           LRWC.zip  unzip LRWC.zip  rm LRWC.zip
 the Crowd
 (LRWC)
+The_Russian                                                             This corpus was developed for the
+Adverse_Drug                                                            Social Media Mining for Health
+Reaction        load_ruadrect #       social         9 515     2.09 Mb Applications (#SMM4H) Shared Task 2020
+Corpus_of                                                               wget https://github.com/cimm-kzn/
+Tweets_                                                                 RuDReC/raw/master/data/RuADReCT.zip
+(RuADReCT)                                                              unzip RuADReCT.zip  rm RuADReCT.zip
  ## Support - Chat â https://telegram.me/natural_language_processing - Issues
 â https://github.com/natasha/corus/issues - Commercial support â https://
 lab.alexkuk.ru ## Development Tests: ```bash make test ``` Add new source: 1.
 Implement `corus/sources/.py` 2. Add import into `corus/sources/__init__.py` 3.
 Add meta into `corus/source/meta.py` 4. Add example into `docs.ipynb` (check
 meta table is correct) 5. Run tests (readme is updated) Package: ```bash make
 version git push git push --tags make clean wheel upload ``` Keywords:
```

### Comparing `corus-0.7.0/corus.egg-info/SOURCES.txt` & `corus-0.9.0/corus.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 corus/sources/mokoron.py
 corus/sources/morphoru.py
 corus/sources/ne5.py
 corus/sources/ods.py
 corus/sources/omnia.py
 corus/sources/persons.py
 corus/sources/ria.py
+corus/sources/rudrec.py
 corus/sources/russe.py
 corus/sources/simlex.py
 corus/sources/toloka.py
 corus/sources/ud.py
 corus/sources/wiki.py
 corus/sources/wikiner.py
 corus/sources/taiga/__init__.py
```

### Comparing `corus-0.7.0/PKG-INFO` & `corus-0.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corus
-Version: 0.7.0
+Version: 0.9.0
 Summary: Links to russian corpora, functions for loading and parsing
 Home-page: https://github.com/natasha/corus
 Author: Alexander Kukushkin
 Author-email: alex@alexkuk.ru
 License: MIT
 Description: 
         <img src="https://github.com/natasha/natasha-logos/blob/master/corus.svg">
@@ -46,14 +46,21 @@
         ...     text = record.text
         ...     ...
         
         ```
         
         For links to other datasets and their loaders see the <a href="#reference">Reference</a> section.
         
+        ## Documentation
+        
+        Materials are in Russian:
+        
+        * <a href="https://natasha.github.io/corus">Corus page on natasha.github.io</a> 
+        * <a href="https://youtu.be/-7XT_U6hVvk?t=2758">Corus section of Datafest 2020 talk</a>
+        
         ## Install
         
         `corus` supports Python 3.5+, PyPy 3.
         
         ```bash
         $ pip install corus
         ```
@@ -70,14 +77,21 @@
         <th>Uncompressed</th>
         <th>Description</th>
         </tr>
         <tr>
         <td>
         <a href="https://github.com/yutkin/Lenta.Ru-News-Dataset">Lenta.ru</a>
         </td>
+        <td colspan="5">
+        </td>
+        </tr>
+        <tr>
+        <td>
+        Lenta.ru v1.0
+        </td>
         <td>
         <a name="load_lenta"></a>
         <code><a href="https://nbviewer.jupyter.org/github/natasha/corus/blob/master/docs.ipynb#load_lenta">load_lenta</a></code>
         <a href="#load_lenta"><code>#</code></a>
         </td>
         <td>
         <code>news</code>
@@ -90,14 +104,36 @@
         </td>
         <td>
         <code>wget https://github.com/yutkin/Lenta.Ru-News-Dataset/releases/download/v1.0/lenta-ru-news.csv.gz</code>
         </td>
         </tr>
         <tr>
         <td>
+        Lenta.ru v1.1+
+        </td>
+        <td>
+        <a name="load_lenta2"></a>
+        <code><a href="https://nbviewer.jupyter.org/github/natasha/corus/blob/master/docs.ipynb#load_lenta2">load_lenta2</a></code>
+        <a href="#load_lenta2"><code>#</code></a>
+        </td>
+        <td>
+        <code>news</code>
+        </td>
+        <td align="right">
+        800&nbsp;975
+        </td>
+        <td align="right">
+        1.94 Gb
+        </td>
+        <td>
+        <code>wget https://github.com/yutkin/Lenta.Ru-News-Dataset/releases/download/v1.1/lenta-ru-news.csv.bz2</code>
+        </td>
+        </tr>
+        <tr>
+        <td>
         <a href="https://russe.nlpub.org/downloads/">Lib.rus.ec</a>
         </td>
         <td>
         <a name="load_librusec"></a>
         <code><a href="https://nbviewer.jupyter.org/github/natasha/corus/blob/master/docs.ipynb#load_librusec">load_librusec</a></code>
         <a href="#load_librusec"><code>#</code></a>
         </td>
@@ -467,14 +503,39 @@
         </br>
         </br>
         <code>wget http://ai-center.botik.ru/Airec/ai-resources/Persons-1000.zip</code>
         </td>
         </tr>
         <tr>
         <td>
+        <a href="https://github.com/cimm-kzn/RuDReC">The Russian Drug Reaction Corpus (RuDReC)</a>
+        </td>
+        <td>
+        <a name="load_rudrec"></a>
+        <code><a href="https://nbviewer.jupyter.org/github/natasha/corus/blob/master/docs.ipynb#load_rudrec">load_rudrec</a></code>
+        <a href="#load_rudrec"><code>#</code></a>
+        </td>
+        <td>
+        <code>ner</code>
+        </td>
+        <td align="right">
+        4&nbsp;809
+        </td>
+        <td align="right">
+        1.73 Kb
+        </td>
+        <td>
+        RuDReC is a new partially annotated corpus of consumer reviews in Russian about pharmaceutical products for the detection of health-related named entities and the effectiveness of pharmaceutical products. Here you can download and work with the annotated part, to get the raw part (1.4M reviews) please refer to https://github.com/cimm-kzn/RuDReC.
+        </br>
+        </br>
+        <code>wget https://github.com/cimm-kzn/RuDReC/raw/master/data/rudrec_annotated.json</code>
+        </td>
+        </tr>
+        <tr>
+        <td>
         <a href="https://tatianashavrina.github.io/taiga_site/">Taiga</a>
         </td>
         <td colspan="5">
         Large collection of Russian texts from various sources: news sites, magazines, literacy, social networks
         </br>
         </br>
         <code>wget https://linghub.ru/static/Taiga/retagged_taiga.tar.gz</code>
@@ -1232,14 +1293,43 @@
         <code>wget https://tlk.s3.yandex.net/dataset/LRWC.zip</code>
         </br>
         <code>unzip LRWC.zip</code>
         </br>
         <code>rm LRWC.zip</code>
         </td>
         </tr>
+        <tr>
+        <td>
+        <a href="https://github.com/cimm-kzn/RuDReC">The Russian Adverse Drug Reaction Corpus of Tweets (RuADReCT)</a>
+        </td>
+        <td>
+        <a name="load_ruadrect"></a>
+        <code><a href="https://nbviewer.jupyter.org/github/natasha/corus/blob/master/docs.ipynb#load_ruadrect">load_ruadrect</a></code>
+        <a href="#load_ruadrect"><code>#</code></a>
+        </td>
+        <td>
+        <code>social</code>
+        </td>
+        <td align="right">
+        9&nbsp;515
+        </td>
+        <td align="right">
+        2.09 Mb
+        </td>
+        <td>
+        This corpus was developed for the Social Media Mining for Health Applications (#SMM4H) Shared Task 2020
+        </br>
+        </br>
+        <code>wget https://github.com/cimm-kzn/RuDReC/raw/master/data/RuADReCT.zip</code>
+        </br>
+        <code>unzip RuADReCT.zip</code>
+        </br>
+        <code>rm RuADReCT.zip</code>
+        </td>
+        </tr>
         </table>
         <!--- metas --->
         
         ## Support
         
         - Chat — https://telegram.me/natural_language_processing
         - Issues — https://github.com/natasha/corus/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: corus Version: 0.7.0 Summary: Links to russian
+Metadata-Version: 2.1 Name: corus Version: 0.9.0 Summary: Links to russian
 corpora, functions for loading and parsing Home-page: https://github.com/
 natasha/corus Author: Alexander Kukushkin Author-email: alex@alexkuk.ru
 License: MIT Description: [https://github.com/natasha/natasha-logos/blob/
 master/corus.svg] ![CI](https://github.com/natasha/corus/workflows/CI/
 badge.svg) [![codecov](https://codecov.io/gh/natasha/corus/branch/master/graph/
 badge.svg)](https://codecov.io/gh/natasha/corus) Links to publicly available
 Russian corpora + code for loading and parsing. 20+_datasets,_350Gb+_of_text.
@@ -17,20 +17,25 @@
 Ð¿ÑÐµÐ¼ÑÐµÑ Ð¿Ð¾ ÑÐ¾ÑÐ¸Ð°Ð»ÑÐ½ÑÐ¼ Ð²Ð¾Ð¿ÑÐ¾ÑÐ°Ð¼ Ð¢Ð°ÑÑÑÐ½Ð°
 ÐÐ¾Ð»Ð¸ÐºÐ¾Ð²Ð° ÑÐ°ÑÑÐºÐ°Ð·Ð°Ð»Ð°, Ð² ÐºÐ°ÐºÐ¸Ñ ÑÐµÐ³Ð¸Ð¾Ð½Ð°Ñ
 Ð Ð¾ÑÑÐ¸Ð¸ Ð·Ð°ÑÐ¸ÐºÑÐ¸ÑÐ¾Ð²Ð°Ð½Ð° Ð½Ð°Ð¸Ð±Ð¾Ð»ÐµÐµ Ð²ÑÑÐ¾ÐºÐ°Ñ
 ÑÐ¼ÐµÑÑÐ½Ð¾ÑÑÑ Ð¾Ñ ÑÐ°ÐºÐ°, ÑÐ¾Ð¾Ð±...', topic='Ð Ð¾ÑÑÐ¸Ñ',
 tags='ÐÐ±ÑÐµÑÑÐ²Ð¾' ) ``` Iterate over texts: ```python >>> records =
 load_lenta(path) >>> for record in records: ... text = record.text ... ... ```
 For links to other datasets and their loaders see the Reference section. ##
-Install `corus` supports Python 3.5+, PyPy 3. ```bash $ pip install corus ```
-## Reference
+Documentation Materials are in Russian: * Corus_page_on_natasha.github.io *
+Corus_section_of_Datafest_2020_talk ## Install `corus` supports Python 3.5+,
+PyPy 3. ```bash $ pip install corus ``` ## Reference
 Dataset        API from corus import  Tags      Texts      Uncompressed Description
+Lenta.ru
                                                                         wget https://github.com/yutkin/
-Lenta.ru        load_lenta #          news         739 351     1.66 Gb Lenta.Ru-News-Dataset/releases/
+Lenta.ru v1.0   load_lenta #          news         739 351     1.66 Gb Lenta.Ru-News-Dataset/releases/
                                                                         download/v1.0/lenta-ru-news.csv.gz
+                                                                        wget https://github.com/yutkin/
+Lenta.ru v1.1+  load_lenta2 #         news         800 975     1.94 Gb Lenta.Ru-News-Dataset/releases/
+                                                                        download/v1.1/lenta-ru-news.csv.bz2
                                                                         Dump of lib.rus.ec prepared for RUSSE
 Lib.rus.ec      load_librusec #       fiction      301 871   144.92 Gb workshop   wget http://panchenko.me/
                                                                         data/russe/librusec_fb2.plain.gz
 Rossiya         load_ria_raw #                                          wget https://github.com/
 Segodnya       load_ria #             news       1 003 86     3.70 Gb RossiyaSegodnya/ria_news_dataset/raw/
                                                                         master/ria.json.gz
 Mokoron                                                                 Russian Twitter sentiment markup
@@ -92,14 +97,26 @@
                                                                         d test_pl_cs_ru_bg  rm
                                                                         TRAININGDATA_BSNLP_2019_shared_task.zip
                                                                         TESTDATA_BSNLP_2019_shared_task.zip
                                                                         Same as Collection5, only PER markup +
 Persons-1000    load_persons #        ner news       1 000     2.96 Mb normalized names   wget http://ai-
                                                                         center.botik.ru/Airec/ai-resources/
                                                                         Persons-1000.zip
+                                                                        RuDReC is a new partially annotated
+                                                                        corpus of consumer reviews in Russian
+                                                                        about pharmaceutical products for the
+                                                                        detection of health-related named
+The_Russian                                                             entities and the effectiveness of
+Drug_Reaction   load_rudrec #         ner            4 809     1.73 Kb pharmaceutical products. Here you can
+Corpus_                                                                 download and work with the annotated
+(RuDReC)                                                                part, to get the raw part (1.4M
+                                                                        reviews) please refer to https://
+                                                                        github.com/cimm-kzn/RuDReC.   wget
+                                                                        https://github.com/cimm-kzn/RuDReC/raw/
+                                                                        master/data/rudrec_annotated.json
                Large collection of Russian texts from various sources: news sites, magazines, literacy, social
 Taiga          networks   wget https://linghub.ru/static/Taiga/retagged_taiga.tar.gz  tar -xzvf
                retagged_taiga.tar.gz
 Arzamas         load_taiga_arzamas #  news             311      4.50 Mb
 Fontanka        load_taiga_fontanka # news         342 683   786.23 Mb
 Interfax        load_taiga_interfax # news          46 429    77.55 Mb
 KP              load_taiga_kp #       news          45 503    61.79 Mb
@@ -222,14 +239,20 @@
 Toloka
 Datasets
 Lexical
 Relations from                                                          wget https://tlk.s3.yandex.net/dataset/
 the Wisdom of   load_toloka_lrwc #    emb sim                           LRWC.zip  unzip LRWC.zip  rm LRWC.zip
 the Crowd
 (LRWC)
+The_Russian                                                             This corpus was developed for the
+Adverse_Drug                                                            Social Media Mining for Health
+Reaction        load_ruadrect #       social         9 515     2.09 Mb Applications (#SMM4H) Shared Task 2020
+Corpus_of                                                               wget https://github.com/cimm-kzn/
+Tweets_                                                                 RuDReC/raw/master/data/RuADReCT.zip
+(RuADReCT)                                                              unzip RuADReCT.zip  rm RuADReCT.zip
  ## Support - Chat â https://telegram.me/natural_language_processing - Issues
 â https://github.com/natasha/corus/issues - Commercial support â https://
 lab.alexkuk.ru ## Development Tests: ```bash make test ``` Add new source: 1.
 Implement `corus/sources/.py` 2. Add import into `corus/sources/__init__.py` 3.
 Add meta into `corus/source/meta.py` 4. Add example into `docs.ipynb` (check
 meta table is correct) 5. Run tests (readme is updated) Package: ```bash make
 version git push git push --tags make clean wheel upload ``` Keywords:
```

### Comparing `corus-0.7.0/README.md` & `corus-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,21 @@
 ...     text = record.text
 ...     ...
 
 ```
 
 For links to other datasets and their loaders see the <a href="#reference">Reference</a> section.
 
+## Documentation
+
+Materials are in Russian:
+
+* <a href="https://natasha.github.io/corus">Corus page on natasha.github.io</a> 
+* <a href="https://youtu.be/-7XT_U6hVvk?t=2758">Corus section of Datafest 2020 talk</a>
+
 ## Install
 
 `corus` supports Python 3.5+, PyPy 3.
 
 ```bash
 $ pip install corus
 ```
@@ -62,14 +69,21 @@
 <th>Uncompressed</th>
 <th>Description</th>
 </tr>
 <tr>
 <td>
 <a href="https://github.com/yutkin/Lenta.Ru-News-Dataset">Lenta.ru</a>
 </td>
+<td colspan="5">
+</td>
+</tr>
+<tr>
+<td>
+Lenta.ru v1.0
+</td>
 <td>
 <a name="load_lenta"></a>
 <code><a href="https://nbviewer.jupyter.org/github/natasha/corus/blob/master/docs.ipynb#load_lenta">load_lenta</a></code>
 <a href="#load_lenta"><code>#</code></a>
 </td>
 <td>
 <code>news</code>
@@ -82,14 +96,36 @@
 </td>
 <td>
 <code>wget https://github.com/yutkin/Lenta.Ru-News-Dataset/releases/download/v1.0/lenta-ru-news.csv.gz</code>
 </td>
 </tr>
 <tr>
 <td>
+Lenta.ru v1.1+
+</td>
+<td>
+<a name="load_lenta2"></a>
+<code><a href="https://nbviewer.jupyter.org/github/natasha/corus/blob/master/docs.ipynb#load_lenta2">load_lenta2</a></code>
+<a href="#load_lenta2"><code>#</code></a>
+</td>
+<td>
+<code>news</code>
+</td>
+<td align="right">
+800&nbsp;975
+</td>
+<td align="right">
+1.94 Gb
+</td>
+<td>
+<code>wget https://github.com/yutkin/Lenta.Ru-News-Dataset/releases/download/v1.1/lenta-ru-news.csv.bz2</code>
+</td>
+</tr>
+<tr>
+<td>
 <a href="https://russe.nlpub.org/downloads/">Lib.rus.ec</a>
 </td>
 <td>
 <a name="load_librusec"></a>
 <code><a href="https://nbviewer.jupyter.org/github/natasha/corus/blob/master/docs.ipynb#load_librusec">load_librusec</a></code>
 <a href="#load_librusec"><code>#</code></a>
 </td>
@@ -459,14 +495,39 @@
 </br>
 </br>
 <code>wget http://ai-center.botik.ru/Airec/ai-resources/Persons-1000.zip</code>
 </td>
 </tr>
 <tr>
 <td>
+<a href="https://github.com/cimm-kzn/RuDReC">The Russian Drug Reaction Corpus (RuDReC)</a>
+</td>
+<td>
+<a name="load_rudrec"></a>
+<code><a href="https://nbviewer.jupyter.org/github/natasha/corus/blob/master/docs.ipynb#load_rudrec">load_rudrec</a></code>
+<a href="#load_rudrec"><code>#</code></a>
+</td>
+<td>
+<code>ner</code>
+</td>
+<td align="right">
+4&nbsp;809
+</td>
+<td align="right">
+1.73 Kb
+</td>
+<td>
+RuDReC is a new partially annotated corpus of consumer reviews in Russian about pharmaceutical products for the detection of health-related named entities and the effectiveness of pharmaceutical products. Here you can download and work with the annotated part, to get the raw part (1.4M reviews) please refer to https://github.com/cimm-kzn/RuDReC.
+</br>
+</br>
+<code>wget https://github.com/cimm-kzn/RuDReC/raw/master/data/rudrec_annotated.json</code>
+</td>
+</tr>
+<tr>
+<td>
 <a href="https://tatianashavrina.github.io/taiga_site/">Taiga</a>
 </td>
 <td colspan="5">
 Large collection of Russian texts from various sources: news sites, magazines, literacy, social networks
 </br>
 </br>
 <code>wget https://linghub.ru/static/Taiga/retagged_taiga.tar.gz</code>
@@ -1224,14 +1285,43 @@
 <code>wget https://tlk.s3.yandex.net/dataset/LRWC.zip</code>
 </br>
 <code>unzip LRWC.zip</code>
 </br>
 <code>rm LRWC.zip</code>
 </td>
 </tr>
+<tr>
+<td>
+<a href="https://github.com/cimm-kzn/RuDReC">The Russian Adverse Drug Reaction Corpus of Tweets (RuADReCT)</a>
+</td>
+<td>
+<a name="load_ruadrect"></a>
+<code><a href="https://nbviewer.jupyter.org/github/natasha/corus/blob/master/docs.ipynb#load_ruadrect">load_ruadrect</a></code>
+<a href="#load_ruadrect"><code>#</code></a>
+</td>
+<td>
+<code>social</code>
+</td>
+<td align="right">
+9&nbsp;515
+</td>
+<td align="right">
+2.09 Mb
+</td>
+<td>
+This corpus was developed for the Social Media Mining for Health Applications (#SMM4H) Shared Task 2020
+</br>
+</br>
+<code>wget https://github.com/cimm-kzn/RuDReC/raw/master/data/RuADReCT.zip</code>
+</br>
+<code>unzip RuADReCT.zip</code>
+</br>
+<code>rm RuADReCT.zip</code>
+</td>
+</tr>
 </table>
 <!--- metas --->
 
 ## Support
 
 - Chat — https://telegram.me/natural_language_processing
 - Issues — https://github.com/natasha/corus/issues
```

#### html2text {}

```diff
@@ -13,20 +13,26 @@
 ÑÐ¼ÐµÑÑÐ½Ð¾ÑÑÑÑ Ð¾Ñ\xa0ÑÐ°ÐºÐ°', text='ÐÐ¸ÑÐµ-Ð¿ÑÐµÐ¼ÑÐµÑ Ð¿Ð¾
 ÑÐ¾ÑÐ¸Ð°Ð»ÑÐ½ÑÐ¼ Ð²Ð¾Ð¿ÑÐ¾ÑÐ°Ð¼ Ð¢Ð°ÑÑÑÐ½Ð° ÐÐ¾Ð»Ð¸ÐºÐ¾Ð²Ð°
 ÑÐ°ÑÑÐºÐ°Ð·Ð°Ð»Ð°, Ð² ÐºÐ°ÐºÐ¸Ñ ÑÐµÐ³Ð¸Ð¾Ð½Ð°Ñ Ð Ð¾ÑÑÐ¸Ð¸
 Ð·Ð°ÑÐ¸ÐºÑÐ¸ÑÐ¾Ð²Ð°Ð½Ð° Ð½Ð°Ð¸Ð±Ð¾Ð»ÐµÐµ Ð²ÑÑÐ¾ÐºÐ°Ñ ÑÐ¼ÐµÑÑÐ½Ð¾ÑÑÑ
 Ð¾Ñ ÑÐ°ÐºÐ°, ÑÐ¾Ð¾Ð±...', topic='Ð Ð¾ÑÑÐ¸Ñ', tags='ÐÐ±ÑÐµÑÑÐ²Ð¾' )
 ``` Iterate over texts: ```python >>> records = load_lenta(path) >>> for record
 in records: ... text = record.text ... ... ``` For links to other datasets and
-their loaders see the Reference section. ## Install `corus` supports Python
-3.5+, PyPy 3. ```bash $ pip install corus ``` ## Reference
+their loaders see the Reference section. ## Documentation Materials are in
+Russian: * Corus_page_on_natasha.github.io * Corus_section_of_Datafest_2020
+talk ## Install `corus` supports Python 3.5+, PyPy 3. ```bash $ pip install
+corus ``` ## Reference
 Dataset        API from corus import  Tags      Texts      Uncompressed Description
+Lenta.ru
                                                                         wget https://github.com/yutkin/
-Lenta.ru        load_lenta #          news         739 351     1.66 Gb Lenta.Ru-News-Dataset/releases/
+Lenta.ru v1.0   load_lenta #          news         739 351     1.66 Gb Lenta.Ru-News-Dataset/releases/
                                                                         download/v1.0/lenta-ru-news.csv.gz
+                                                                        wget https://github.com/yutkin/
+Lenta.ru v1.1+  load_lenta2 #         news         800 975     1.94 Gb Lenta.Ru-News-Dataset/releases/
+                                                                        download/v1.1/lenta-ru-news.csv.bz2
                                                                         Dump of lib.rus.ec prepared for RUSSE
 Lib.rus.ec      load_librusec #       fiction      301 871   144.92 Gb workshop   wget http://panchenko.me/
                                                                         data/russe/librusec_fb2.plain.gz
 Rossiya         load_ria_raw #                                          wget https://github.com/
 Segodnya       load_ria #             news       1 003 86     3.70 Gb RossiyaSegodnya/ria_news_dataset/raw/
                                                                         master/ria.json.gz
 Mokoron                                                                 Russian Twitter sentiment markup
@@ -88,14 +94,26 @@
                                                                         d test_pl_cs_ru_bg  rm
                                                                         TRAININGDATA_BSNLP_2019_shared_task.zip
                                                                         TESTDATA_BSNLP_2019_shared_task.zip
                                                                         Same as Collection5, only PER markup +
 Persons-1000    load_persons #        ner news       1 000     2.96 Mb normalized names   wget http://ai-
                                                                         center.botik.ru/Airec/ai-resources/
                                                                         Persons-1000.zip
+                                                                        RuDReC is a new partially annotated
+                                                                        corpus of consumer reviews in Russian
+                                                                        about pharmaceutical products for the
+                                                                        detection of health-related named
+The_Russian                                                             entities and the effectiveness of
+Drug_Reaction   load_rudrec #         ner            4 809     1.73 Kb pharmaceutical products. Here you can
+Corpus_                                                                 download and work with the annotated
+(RuDReC)                                                                part, to get the raw part (1.4M
+                                                                        reviews) please refer to https://
+                                                                        github.com/cimm-kzn/RuDReC.   wget
+                                                                        https://github.com/cimm-kzn/RuDReC/raw/
+                                                                        master/data/rudrec_annotated.json
                Large collection of Russian texts from various sources: news sites, magazines, literacy, social
 Taiga          networks   wget https://linghub.ru/static/Taiga/retagged_taiga.tar.gz  tar -xzvf
                retagged_taiga.tar.gz
 Arzamas         load_taiga_arzamas #  news             311      4.50 Mb
 Fontanka        load_taiga_fontanka # news         342 683   786.23 Mb
 Interfax        load_taiga_interfax # news          46 429    77.55 Mb
 KP              load_taiga_kp #       news          45 503    61.79 Mb
@@ -218,14 +236,20 @@
 Toloka
 Datasets
 Lexical
 Relations from                                                          wget https://tlk.s3.yandex.net/dataset/
 the Wisdom of   load_toloka_lrwc #    emb sim                           LRWC.zip  unzip LRWC.zip  rm LRWC.zip
 the Crowd
 (LRWC)
+The_Russian                                                             This corpus was developed for the
+Adverse_Drug                                                            Social Media Mining for Health
+Reaction        load_ruadrect #       social         9 515     2.09 Mb Applications (#SMM4H) Shared Task 2020
+Corpus_of                                                               wget https://github.com/cimm-kzn/
+Tweets_                                                                 RuDReC/raw/master/data/RuADReCT.zip
+(RuADReCT)                                                              unzip RuADReCT.zip  rm RuADReCT.zip
  ## Support - Chat â https://telegram.me/natural_language_processing - Issues
 â https://github.com/natasha/corus/issues - Commercial support â https://
 lab.alexkuk.ru ## Development Tests: ```bash make test ``` Add new source: 1.
 Implement `corus/sources/.py` 2. Add import into `corus/sources/__init__.py` 3.
 Add meta into `corus/source/meta.py` 4. Add example into `docs.ipynb` (check
 meta table is correct) 5. Run tests (readme is updated) Package: ```bash make
 version git push git push --tags make clean wheel upload ```
```

### Comparing `corus-0.7.0/setup.py` & `corus-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open('README.md') as file:
     description = file.read()
 
 
 setup(
     name='corus',
-    version='0.7.0',
+    version='0.9.0',
     description='Links to russian corpora, functions for loading and parsing',
     long_description=description,
     long_description_content_type='text/markdown',
     url='https://github.com/natasha/corus',
     author='Alexander Kukushkin',
     author_email='alex@alexkuk.ru',
     license='MIT',
```

