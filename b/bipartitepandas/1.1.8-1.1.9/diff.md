# Comparing `tmp/bipartitepandas-1.1.8.tar.gz` & `tmp/bipartitepandas-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bipartitepandas-1.1.8.tar", last modified: Mon May 29 01:11:00 2023, max compression
+gzip compressed data, was "bipartitepandas-1.1.9.tar", last modified: Mon Jul 24 09:05:00 2023, max compression
```

## Comparing `bipartitepandas-1.1.8.tar` & `bipartitepandas-1.1.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-05-29 01:11:00.048632 bipartitepandas-1.1.8/
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     1058 2022-07-24 19:52:06.000000 bipartitepandas-1.1.8/LICENSE
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2797 2023-05-29 01:11:00.048751 bipartitepandas-1.1.8/PKG-INFO
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2204 2023-05-28 03:41:14.000000 bipartitepandas-1.1.8/README.rst
-drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-05-29 01:11:00.044264 bipartitepandas-1.1.8/bipartitepandas/
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)      818 2022-09-02 23:11:52.000000 bipartitepandas-1.1.8/bipartitepandas/__init__.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    86380 2023-05-28 02:35:42.000000 bipartitepandas-1.1.8/bipartitepandas/bipartitebase.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    32553 2022-09-03 22:00:33.000000 bipartitepandas-1.1.8/bipartitepandas/bipartitedataframe.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     3582 2023-05-26 18:35:42.000000 bipartitepandas-1.1.8/bipartitepandas/bipartiteeventstudy.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    58472 2023-05-26 18:17:43.000000 bipartitepandas-1.1.8/bipartitepandas/bipartiteeventstudybase.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     3500 2023-01-08 21:22:33.000000 bipartitepandas-1.1.8/bipartitepandas/bipartiteeventstudycollapsed.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     3818 2022-09-02 23:16:52.000000 bipartitepandas-1.1.8/bipartitepandas/bipartiteextendedeventstudy.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    50571 2023-01-08 21:22:25.000000 bipartitepandas-1.1.8/bipartitepandas/bipartiteextendedeventstudybase.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     3758 2023-01-08 21:22:35.000000 bipartitepandas-1.1.8/bipartitepandas/bipartiteextendedeventstudycollapsed.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    27925 2023-05-26 18:38:14.000000 bipartitepandas-1.1.8/bipartitepandas/bipartitelong.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    75272 2023-05-26 18:15:28.000000 bipartitepandas-1.1.8/bipartitepandas/bipartitelongbase.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    34407 2023-01-08 21:22:37.000000 bipartitepandas-1.1.8/bipartitepandas/bipartitelongcollapsed.py
-drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-05-29 01:11:00.045416 bipartitepandas-1.1.8/bipartitepandas/grouping/
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)       25 2022-07-24 19:52:06.000000 bipartitepandas-1.1.8/bipartitepandas/grouping/__init__.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     3026 2023-05-29 01:08:39.000000 bipartitepandas-1.1.8/bipartitepandas/grouping/grouping.py
-drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-05-29 01:11:00.045793 bipartitepandas-1.1.8/bipartitepandas/measures/
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)       25 2022-07-24 19:52:06.000000 bipartitepandas-1.1.8/bipartitepandas/measures/__init__.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     6778 2023-05-28 03:40:11.000000 bipartitepandas-1.1.8/bipartitepandas/measures/measures.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     8604 2022-09-02 23:16:50.000000 bipartitepandas-1.1.8/bipartitepandas/simbipartite.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    13173 2022-09-02 23:16:51.000000 bipartitepandas-1.1.8/bipartitepandas/util.py
-drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-05-29 01:11:00.045092 bipartitepandas-1.1.8/bipartitepandas.egg-info/
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2797 2023-05-29 01:11:00.000000 bipartitepandas-1.1.8/bipartitepandas.egg-info/PKG-INFO
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     1201 2023-05-29 01:11:00.000000 bipartitepandas-1.1.8/bipartitepandas.egg-info/SOURCES.txt
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)        1 2023-05-29 01:11:00.000000 bipartitepandas-1.1.8/bipartitepandas.egg-info/dependency_links.txt
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)       82 2023-05-29 01:11:00.000000 bipartitepandas-1.1.8/bipartitepandas.egg-info/requires.txt
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)       16 2023-05-29 01:11:00.000000 bipartitepandas-1.1.8/bipartitepandas.egg-info/top_level.txt
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)      103 2022-08-28 19:50:50.000000 bipartitepandas-1.1.8/pyproject.toml
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)      763 2023-05-29 01:11:00.049172 bipartitepandas-1.1.8/setup.cfg
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)      162 2023-01-08 21:43:24.000000 bipartitepandas-1.1.8/setup.py
-drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-05-29 01:11:00.048458 bipartitepandas-1.1.8/tests/
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2900 2022-07-24 19:52:06.000000 bipartitepandas-1.1.8/tests/test_bpd.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    86879 2022-09-02 23:16:33.000000 bipartitepandas-1.1.8/tests/test_bpd_base.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    17134 2023-05-29 00:41:26.000000 bipartitepandas-1.1.8/tests/test_bpd_clustering.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    34290 2023-05-26 18:42:55.000000 bipartitepandas-1.1.8/tests/test_bpd_connectedness.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    16145 2022-07-24 19:52:06.000000 bipartitepandas-1.1.8/tests/test_bpd_custom.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2253 2022-07-24 19:52:06.000000 bipartitepandas-1.1.8/tests/test_bpd_df.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     4536 2022-07-24 19:52:06.000000 bipartitepandas-1.1.8/tests/test_bpd_es.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     4978 2022-07-24 19:52:06.000000 bipartitepandas-1.1.8/tests/test_bpd_es_collapsed.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    14606 2022-09-02 23:16:46.000000 bipartitepandas-1.1.8/tests/test_bpd_long.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2954 2022-08-06 18:51:15.000000 bipartitepandas-1.1.8/tests/test_bpd_long_collapsed.py
+drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-07-24 09:05:00.717301 bipartitepandas-1.1.9/
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     1058 2022-07-24 19:52:06.000000 bipartitepandas-1.1.9/LICENSE
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2797 2023-07-24 09:05:00.717391 bipartitepandas-1.1.9/PKG-INFO
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2204 2023-05-28 03:41:14.000000 bipartitepandas-1.1.9/README.rst
+drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-07-24 09:05:00.711181 bipartitepandas-1.1.9/bipartitepandas/
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)      818 2022-09-02 23:11:52.000000 bipartitepandas-1.1.9/bipartitepandas/__init__.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    86380 2023-07-01 19:59:35.000000 bipartitepandas-1.1.9/bipartitepandas/bipartitebase.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    32553 2022-09-03 22:00:33.000000 bipartitepandas-1.1.9/bipartitepandas/bipartitedataframe.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     3582 2023-05-26 18:35:42.000000 bipartitepandas-1.1.9/bipartitepandas/bipartiteeventstudy.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    58472 2023-05-26 18:17:43.000000 bipartitepandas-1.1.9/bipartitepandas/bipartiteeventstudybase.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     3500 2023-01-08 21:22:33.000000 bipartitepandas-1.1.9/bipartitepandas/bipartiteeventstudycollapsed.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     3818 2022-09-02 23:16:52.000000 bipartitepandas-1.1.9/bipartitepandas/bipartiteextendedeventstudy.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    50571 2023-01-08 21:22:25.000000 bipartitepandas-1.1.9/bipartitepandas/bipartiteextendedeventstudybase.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     3758 2023-01-08 21:22:35.000000 bipartitepandas-1.1.9/bipartitepandas/bipartiteextendedeventstudycollapsed.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    27925 2023-05-26 18:38:14.000000 bipartitepandas-1.1.9/bipartitepandas/bipartitelong.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    75272 2023-05-26 18:15:28.000000 bipartitepandas-1.1.9/bipartitepandas/bipartitelongbase.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    34407 2023-01-08 21:22:37.000000 bipartitepandas-1.1.9/bipartitepandas/bipartitelongcollapsed.py
+drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-07-24 09:05:00.712671 bipartitepandas-1.1.9/bipartitepandas/grouping/
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)       25 2022-07-24 19:52:06.000000 bipartitepandas-1.1.9/bipartitepandas/grouping/__init__.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     3026 2023-05-29 01:08:39.000000 bipartitepandas-1.1.9/bipartitepandas/grouping/grouping.py
+drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-07-24 09:05:00.713240 bipartitepandas-1.1.9/bipartitepandas/measures/
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)       25 2022-07-24 19:52:06.000000 bipartitepandas-1.1.9/bipartitepandas/measures/__init__.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     7148 2023-07-24 09:01:12.000000 bipartitepandas-1.1.9/bipartitepandas/measures/measures.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     8604 2022-09-02 23:16:50.000000 bipartitepandas-1.1.9/bipartitepandas/simbipartite.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    13173 2022-09-02 23:16:51.000000 bipartitepandas-1.1.9/bipartitepandas/util.py
+drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-07-24 09:05:00.712162 bipartitepandas-1.1.9/bipartitepandas.egg-info/
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2797 2023-07-24 09:05:00.000000 bipartitepandas-1.1.9/bipartitepandas.egg-info/PKG-INFO
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     1201 2023-07-24 09:05:00.000000 bipartitepandas-1.1.9/bipartitepandas.egg-info/SOURCES.txt
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)        1 2023-07-24 09:05:00.000000 bipartitepandas-1.1.9/bipartitepandas.egg-info/dependency_links.txt
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)       82 2023-07-24 09:05:00.000000 bipartitepandas-1.1.9/bipartitepandas.egg-info/requires.txt
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)       16 2023-07-24 09:05:00.000000 bipartitepandas-1.1.9/bipartitepandas.egg-info/top_level.txt
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)      103 2023-07-24 09:04:37.000000 bipartitepandas-1.1.9/pyproject.toml
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)      763 2023-07-24 09:05:00.717795 bipartitepandas-1.1.9/setup.cfg
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)      162 2023-01-08 21:43:24.000000 bipartitepandas-1.1.9/setup.py
+drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-07-24 09:05:00.717043 bipartitepandas-1.1.9/tests/
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2900 2022-07-24 19:52:06.000000 bipartitepandas-1.1.9/tests/test_bpd.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    86879 2022-09-02 23:16:33.000000 bipartitepandas-1.1.9/tests/test_bpd_base.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    17134 2023-05-29 00:41:26.000000 bipartitepandas-1.1.9/tests/test_bpd_clustering.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    34290 2023-05-26 18:42:55.000000 bipartitepandas-1.1.9/tests/test_bpd_connectedness.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    16145 2022-07-24 19:52:06.000000 bipartitepandas-1.1.9/tests/test_bpd_custom.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2253 2022-07-24 19:52:06.000000 bipartitepandas-1.1.9/tests/test_bpd_df.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     4536 2022-07-24 19:52:06.000000 bipartitepandas-1.1.9/tests/test_bpd_es.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     4978 2022-07-24 19:52:06.000000 bipartitepandas-1.1.9/tests/test_bpd_es_collapsed.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    14606 2022-09-02 23:16:46.000000 bipartitepandas-1.1.9/tests/test_bpd_long.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2954 2022-08-06 18:51:15.000000 bipartitepandas-1.1.9/tests/test_bpd_long_collapsed.py
```

### Comparing `bipartitepandas-1.1.8/LICENSE` & `bipartitepandas-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.8/PKG-INFO` & `bipartitepandas-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bipartitepandas
-Version: 1.1.8
+Version: 1.1.9
 Summary: Python tools for bipartite labor data
 Home-page: https://github.com/tlamadon/bipartitepandas/
 Author: Thibaut Lamadon
 Author-email: thibaut.lamadon@gmail.com
 Project-URL: Documentation, https://tlamadon.github.io/bipartitepandas/
 Project-URL: GitHub, https://github.com/tlamadon/bipartitepandas/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bipartitepandas-1.1.8/README.rst` & `bipartitepandas-1.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.8/bipartitepandas/__init__.py` & `bipartitepandas-1.1.9/bipartitepandas/__init__.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.8/bipartitepandas/bipartitebase.py` & `bipartitepandas-1.1.9/bipartitepandas/bipartitebase.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.8/bipartitepandas/bipartitedataframe.py` & `bipartitepandas-1.1.9/bipartitepandas/bipartitedataframe.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.8/bipartitepandas/bipartiteeventstudy.py` & `bipartitepandas-1.1.9/bipartitepandas/bipartiteeventstudy.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.8/bipartitepandas/bipartiteeventstudybase.py` & `bipartitepandas-1.1.9/bipartitepandas/bipartiteeventstudybase.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.8/bipartitepandas/bipartiteeventstudycollapsed.py` & `bipartitepandas-1.1.9/bipartitepandas/bipartiteeventstudycollapsed.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.8/bipartitepandas/bipartiteextendedeventstudy.py` & `bipartitepandas-1.1.9/bipartitepandas/bipartiteextendedeventstudy.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.8/bipartitepandas/bipartiteextendedeventstudybase.py` & `bipartitepandas-1.1.9/bipartitepandas/bipartiteextendedeventstudybase.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.8/bipartitepandas/bipartiteextendedeventstudycollapsed.py` & `bipartitepandas-1.1.9/bipartitepandas/bipartiteextendedeventstudycollapsed.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.8/bipartitepandas/bipartitelong.py` & `bipartitepandas-1.1.9/bipartitepandas/bipartitelong.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.8/bipartitepandas/bipartitelongbase.py` & `bipartitepandas-1.1.9/bipartitepandas/bipartitelongbase.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.8/bipartitepandas/bipartitelongcollapsed.py` & `bipartitepandas-1.1.9/bipartitepandas/bipartitelongcollapsed.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.8/bipartitepandas/grouping/grouping.py` & `bipartitepandas-1.1.9/bipartitepandas/grouping/grouping.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.8/bipartitepandas/measures/measures.py` & `bipartitepandas-1.1.9/bipartitepandas/measures/measures.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,43 +8,46 @@
 class CDFs:
     '''
     Generate cdfs of compensation for firms. Used for clustering.
 
     Arguments:
         cdf_resolution (int): how many values to use to approximate the cdfs
         measure (str): how to compute the cdfs ('quantile_all' to get quantiles from entire set of data, then have firm-level values between 0 and 1; 'quantile_firm' to get quantiles at the firm-level and have values be compensations)
+        outcome_col (str): outcome_col column to use for data
     '''
 
-    def __init__(self, cdf_resolution=10, measure='quantile_all'):
+    def __init__(self, cdf_resolution=10, measure='quantile_all', outcome_col='y'):
         self.cdf_resolution = cdf_resolution
         self.measure = measure
+        self.outcome_col = outcome_col
 
     def _compute_measure(self, frame, jids):
         '''
         Arguments:
             frame (Pandas DataFrame): data to use
             jids (list): sorted list of firm ids in frame (since frame could be a subset of self, this is not necessarily all firms in self)
         Returns:
             (NumPy Array): NumPy array of firm cdfs
         '''
         cdf_resolution = self.cdf_resolution
         measure = self.measure
+        outcome_col = self.outcome_col
         n_firms = len(jids)
 
         ## Initialize cdf array ##
         cdfs = np.zeros([n_firms, cdf_resolution])
 
         # Create quantiles of interest
         quantiles = np.linspace(1 / cdf_resolution, 1, cdf_resolution)
 
         # Group by income cdfs
         if measure == 'quantile_all':
             # Convert columns to NumPy
             j = frame.loc[:, 'j'].to_numpy()
-            y = frame.loc[:, 'y'].to_numpy()
+            y = frame.loc[:, outcome_col].to_numpy()
             w = frame.loc[:, 'row_weights'].to_numpy()
 
             # Force j and jids to be integers so np.bincount and indexing work correctly
             if jids.dtype == 'O':
                 jids = jids.astype(int, copy=True)
             if j.dtype == 'O':
                 j = j.astype(int, copy=True)
@@ -60,20 +63,20 @@
             # Normalize by firm size (convert to cdf)
             jsize = np.bincount(j, w)[jids]
             cdfs = (cdfs.T / jsize.T).T
 
         elif measure == 'quantile_firm':
             # Sort frame by firm + compensation (do this once now, so that don't need to do it again later) (also note it is faster to sort and then manually compute quantiles than to use built-in quantile functions)
             # NOTE: don't sort in-place, otherwise modifies external data
-            frame = frame.sort_values(['j', 'y'], inplace=False)
+            frame = frame.sort_values(['j', outcome_col], inplace=False)
             frame.reset_index(drop=True, inplace=True)
             frame.reset_index(drop=False, inplace=True)
 
             # Convert columns to NumPy (after sorting)
-            y = frame.loc[:, 'y'].to_numpy()
+            y = frame.loc[:, outcome_col].to_numpy()
             w = frame.loc[:, 'row_weights'].to_numpy()
 
             # Find min + max index for each firm
             groupby_j = frame.groupby('j', sort=False)['index']
             j_min_idx = groupby_j.min().to_numpy()
             j_max_idx = groupby_j.max().to_numpy()
             del groupby_j
@@ -106,54 +109,57 @@
 
 class Moments:
     '''
     Generate compensation moments for firms. Used for clustering.
 
     Arguments:
         measures (str or list of str): how to compute the measures ('mean' to compute average income within each firm; 'var' to compute variance of income within each firm; 'max' to compute max income within each firm; 'min' to compute min income within each firm)
+        outcome_col (str): outcome_col column to use for data
     '''
 
-    def __init__(self, measures='mean'):
+    def __init__(self, measures='mean', outcome_col='y'):
         self.measures = measures
+        self.outcome_col = outcome_col
 
     def _compute_measure(self, frame, jids):
         '''
         Arguments:
             frame (Pandas DataFrame): data to use
             jids (list): sorted list of firm ids in frame (since frame could be a subset of self, this is not necessarily all firms in self)
 
         Returns:
             (NumPy Array): NumPy array of firm moments
         '''
         n_firms = len(jids)
         measures = self.measures
         n_measures = len(to_list(measures))
+        outcome_col = self.outcome_col
 
         ## Initialize moments array ##
         moments = np.zeros([n_firms, n_measures])
 
         # Required for aggregate_transform
         # NOTE: don't sort in-place, otherwise modifies external data
         frame = frame.sort_values('j', inplace=False)
 
         for j, measure in enumerate(to_list(measures)):
             if measure == 'mean':
                 # Group by mean income
                 j_ = frame.loc[:, 'j'].to_numpy()
-                y = frame.loc[:, 'y'].to_numpy()
+                y = frame.loc[:, outcome_col].to_numpy()
                 w = frame.loc[:, 'row_weights'].to_numpy()
                 # Force j and jids to be integers so np.bincount and indexing work correctly
                 if jids.dtype == 'O':
                     jids = jids.astype(int, copy=True)
                 if j_.dtype == 'O':
                     j_ = j_.astype(int, copy=True)
                 moments[:, j] = np.bincount(j_, w * y)[jids] / np.bincount(j_, w)[jids]
                 del j_, y, w
             elif measure == 'var':
                 # Group by variance of income
-                moments[:, j] = aggregate_transform(frame, 'j', 'y', 'var', weights='row_weights', merge=False)
+                moments[:, j] = aggregate_transform(frame, 'j', outcome_col, 'var', weights='row_weights', merge=False)
             elif measure == 'max':
-                moments[:, j] = frame.groupby('j', sort=False)['y'].max().to_numpy()
+                moments[:, j] = frame.groupby('j', sort=False)[outcome_col].max().to_numpy()
             elif measure == 'min':
-                moments[:, j] = frame.groupby('j', sort=False)['y'].min().to_numpy()
+                moments[:, j] = frame.groupby('j', sort=False)[outcome_col].min().to_numpy()
 
         return moments
```

### Comparing `bipartitepandas-1.1.8/bipartitepandas/simbipartite.py` & `bipartitepandas-1.1.9/bipartitepandas/simbipartite.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.8/bipartitepandas/util.py` & `bipartitepandas-1.1.9/bipartitepandas/util.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.8/bipartitepandas.egg-info/PKG-INFO` & `bipartitepandas-1.1.9/bipartitepandas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bipartitepandas
-Version: 1.1.8
+Version: 1.1.9
 Summary: Python tools for bipartite labor data
 Home-page: https://github.com/tlamadon/bipartitepandas/
 Author: Thibaut Lamadon
 Author-email: thibaut.lamadon@gmail.com
 Project-URL: Documentation, https://tlamadon.github.io/bipartitepandas/
 Project-URL: GitHub, https://github.com/tlamadon/bipartitepandas/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bipartitepandas-1.1.8/bipartitepandas.egg-info/SOURCES.txt` & `bipartitepandas-1.1.9/bipartitepandas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.8/setup.cfg` & `bipartitepandas-1.1.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bipartitepandas
-version = 1.1.8
+version = 1.1.9
 author = Thibaut Lamadon
 author_email = thibaut.lamadon@gmail.com
 description = Python tools for bipartite labor data
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/tlamadon/bipartitepandas/
 project_urls =
```

### Comparing `bipartitepandas-1.1.8/tests/test_bpd.py` & `bipartitepandas-1.1.9/tests/test_bpd.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.8/tests/test_bpd_base.py` & `bipartitepandas-1.1.9/tests/test_bpd_base.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.8/tests/test_bpd_clustering.py` & `bipartitepandas-1.1.9/tests/test_bpd_clustering.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.8/tests/test_bpd_connectedness.py` & `bipartitepandas-1.1.9/tests/test_bpd_connectedness.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.8/tests/test_bpd_custom.py` & `bipartitepandas-1.1.9/tests/test_bpd_custom.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.8/tests/test_bpd_df.py` & `bipartitepandas-1.1.9/tests/test_bpd_df.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.8/tests/test_bpd_es.py` & `bipartitepandas-1.1.9/tests/test_bpd_es.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.8/tests/test_bpd_es_collapsed.py` & `bipartitepandas-1.1.9/tests/test_bpd_es_collapsed.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.8/tests/test_bpd_long.py` & `bipartitepandas-1.1.9/tests/test_bpd_long.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.8/tests/test_bpd_long_collapsed.py` & `bipartitepandas-1.1.9/tests/test_bpd_long_collapsed.py`

 * *Files identical despite different names*

