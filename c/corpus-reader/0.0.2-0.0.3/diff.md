# Comparing `tmp/corpus_reader-0.0.2.tar.gz` & `tmp/corpus_reader-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corpus_reader-0.0.2.tar", last modified: Mon Jul 24 20:30:51 2023, max compression
+gzip compressed data, was "corpus_reader-0.0.3.tar", last modified: Mon Jul 24 20:35:04 2023, max compression
```

## Comparing `corpus_reader-0.0.2.tar` & `corpus_reader-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:31:38.128497 corpus_reader-0.0.2/
--rw-r--r--   0 root         (0) root         (0)      431 2023-07-24 20:31:38.128497 corpus_reader-0.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       91 2023-07-24 20:12:40.000000 corpus_reader-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:31:38.046498 corpus_reader-0.0.2/corpus_reader/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-24 20:12:51.000000 corpus_reader-0.0.2/corpus_reader/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4941 2023-07-24 20:21:53.000000 corpus_reader-0.0.2/corpus_reader/corpus_reader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:31:38.126497 corpus_reader-0.0.2/corpus_reader.egg-info/
--rw-r--r--   0 root         (0) root         (0)      431 2023-07-24 20:31:37.000000 corpus_reader-0.0.2/corpus_reader.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      295 2023-07-24 20:31:37.000000 corpus_reader-0.0.2/corpus_reader.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 20:31:37.000000 corpus_reader-0.0.2/corpus_reader.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 20:22:50.000000 corpus_reader-0.0.2/corpus_reader.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-24 20:31:37.000000 corpus_reader-0.0.2/corpus_reader.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-07-24 20:31:37.000000 corpus_reader-0.0.2/corpus_reader.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 20:31:38.131497 corpus_reader-0.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      663 2023-07-24 20:30:46.000000 corpus_reader-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:35:50.905087 corpus_reader-0.0.3/
+-rw-r--r--   0 root         (0) root         (0)      431 2023-07-24 20:35:50.904087 corpus_reader-0.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       91 2023-07-24 20:12:40.000000 corpus_reader-0.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:35:50.794090 corpus_reader-0.0.3/corpus_reader/
+-rw-r--r--   0 root         (0) root         (0)       62 2023-07-24 20:35:07.000000 corpus_reader-0.0.3/corpus_reader/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4941 2023-07-24 20:21:53.000000 corpus_reader-0.0.3/corpus_reader/corpus_reader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:35:50.903087 corpus_reader-0.0.3/corpus_reader.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      431 2023-07-24 20:35:50.000000 corpus_reader-0.0.3/corpus_reader.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      295 2023-07-24 20:35:50.000000 corpus_reader-0.0.3/corpus_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 20:35:50.000000 corpus_reader-0.0.3/corpus_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 20:22:50.000000 corpus_reader-0.0.3/corpus_reader.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-24 20:35:50.000000 corpus_reader-0.0.3/corpus_reader.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-24 20:35:50.000000 corpus_reader-0.0.3/corpus_reader.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 20:35:50.905087 corpus_reader-0.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      663 2023-07-24 20:34:15.000000 corpus_reader-0.0.3/setup.py
```

### Comparing `corpus_reader-0.0.2/corpus_reader/corpus_reader.py` & `corpus_reader-0.0.3/corpus_reader/corpus_reader.py`

 * *Files identical despite different names*

### Comparing `corpus_reader-0.0.2/setup.py` & `corpus_reader-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='corpus_reader',
-    version='0.0.2',
+    version='0.0.3',
     description='A fast and memory-efficient indexing tool for reading large-scale corpora.',
     author='waylight3',
     author_email='waylight3@snu.ac.kr',
     url='https://github.com/waylight3/corpus_reader',
     install_requires=['unidecode',],
     packages=find_packages(exclude=[]),
     keywords=['corpus', 'reader', 'index', 'large data', 'memory-efficient'],
```

