# Comparing `tmp/graphreduce-1.0.tar.gz` & `tmp/graphreduce-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphreduce-1.0.tar", last modified: Mon Jul 24 16:27:56 2023, max compression
+gzip compressed data, was "graphreduce-1.1.tar", last modified: Mon Jul 24 16:40:01 2023, max compression
```

## Comparing `graphreduce-1.0.tar` & `graphreduce-1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-24 16:27:56.328405 graphreduce-1.0/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     7925 2023-07-24 16:27:56.328286 graphreduce-1.0/PKG-INFO
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     6951 2023-06-29 22:54:27.000000 graphreduce-1.0/README.md
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-24 16:27:56.327257 graphreduce-1.0/graphreduce/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)        0 2022-06-22 03:03:07.000000 graphreduce-1.0/graphreduce/__init__.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      290 2023-06-29 23:42:51.000000 graphreduce-1.0/graphreduce/enum.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)    15894 2023-07-22 18:26:20.000000 graphreduce-1.0/graphreduce/graph_reduce.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)    14626 2023-07-24 16:21:34.000000 graphreduce-1.0/graphreduce/node.py
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-24 16:27:56.328125 graphreduce-1.0/graphreduce.egg-info/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     7925 2023-07-24 16:27:56.000000 graphreduce-1.0/graphreduce.egg-info/PKG-INFO
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      318 2023-07-24 16:27:56.000000 graphreduce-1.0/graphreduce.egg-info/SOURCES.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-07-24 16:27:56.000000 graphreduce-1.0/graphreduce.egg-info/dependency_links.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-06-16 20:09:48.000000 graphreduce-1.0/graphreduce.egg-info/not-zip-safe
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      134 2023-07-24 16:27:56.000000 graphreduce-1.0/graphreduce.egg-info/requires.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)       12 2023-07-24 16:27:56.000000 graphreduce-1.0/graphreduce.egg-info/top_level.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)       38 2023-07-24 16:27:56.328439 graphreduce-1.0/setup.cfg
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     1830 2023-07-24 16:27:43.000000 graphreduce-1.0/setup.py
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-24 16:40:01.028129 graphreduce-1.1/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     7925 2023-07-24 16:40:01.028013 graphreduce-1.1/PKG-INFO
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     6951 2023-06-29 22:54:27.000000 graphreduce-1.1/README.md
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-24 16:40:01.027011 graphreduce-1.1/graphreduce/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        0 2022-06-22 03:03:07.000000 graphreduce-1.1/graphreduce/__init__.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      290 2023-06-29 23:42:51.000000 graphreduce-1.1/graphreduce/enum.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)    15894 2023-07-22 18:26:20.000000 graphreduce-1.1/graphreduce/graph_reduce.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)    14662 2023-07-24 16:39:37.000000 graphreduce-1.1/graphreduce/node.py
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-24 16:40:01.027842 graphreduce-1.1/graphreduce.egg-info/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     7925 2023-07-24 16:40:00.000000 graphreduce-1.1/graphreduce.egg-info/PKG-INFO
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      318 2023-07-24 16:40:00.000000 graphreduce-1.1/graphreduce.egg-info/SOURCES.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-07-24 16:40:00.000000 graphreduce-1.1/graphreduce.egg-info/dependency_links.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-06-16 20:09:48.000000 graphreduce-1.1/graphreduce.egg-info/not-zip-safe
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      134 2023-07-24 16:40:00.000000 graphreduce-1.1/graphreduce.egg-info/requires.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)       12 2023-07-24 16:40:00.000000 graphreduce-1.1/graphreduce.egg-info/top_level.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)       38 2023-07-24 16:40:01.028165 graphreduce-1.1/setup.cfg
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     1830 2023-07-24 16:39:58.000000 graphreduce-1.1/setup.py
```

### Comparing `graphreduce-1.0/PKG-INFO` & `graphreduce-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphreduce
-Version: 1.0
+Version: 1.1
 Summary: Leveraging graph data structures for complex feature engineering pipelines.
 Home-page: https://github.com/wesmadrigal/graphreduce
 Author: Wes Madrigal
 Author-email: wes@madconsulting.ai
 License: MIT
 Project-URL: Source, http://github.com/wesmadrigal/graphreduce
 Project-URL: Issue Tracker, https://github.com/wesmadrigal/graphreduce/issues
```

### Comparing `graphreduce-1.0/README.md` & `graphreduce-1.1/README.md`

 * *Files identical despite different names*

### Comparing `graphreduce-1.0/graphreduce/graph_reduce.py` & `graphreduce-1.1/graphreduce/graph_reduce.py`

 * *Files identical despite different names*

### Comparing `graphreduce-1.0/graphreduce/node.py` & `graphreduce-1.1/graphreduce/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,21 +67,21 @@
     has_labels : whether or not the node has labels to compute
     label_period_val : optional period of time to compute labels
     label_period_unit : optional unit of measure for label period (e.g., PeriodUnit.day)
     feature_function : optional feature function, usually used when reduce is false
     columns : optional list of columns to include
         """
         # For when this is already set on the class definition.
-        if not self.pk:
+        if not hasattr(self, 'pk'):
             self.pk = pk
         # For when this is already set on the class definition.
-        if not self.prefix:
+        if not hasattr(self, 'prefix'):
             self.prefix = prefix
         # For when this is already set on the class definition.
-        if not self.date_key:
+        if not hasattr(self, 'date_key'):
             self.date_key = date_key
         self.fpath = fpath
         self.fmt = fmt
         self.compute_layer = compute_layer
         self.cut_date = cut_date
         self.compute_period_val = compute_period_val
         self.compute_period_unit = compute_period_unit
```

### Comparing `graphreduce-1.0/graphreduce.egg-info/PKG-INFO` & `graphreduce-1.1/graphreduce.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphreduce
-Version: 1.0
+Version: 1.1
 Summary: Leveraging graph data structures for complex feature engineering pipelines.
 Home-page: https://github.com/wesmadrigal/graphreduce
 Author: Wes Madrigal
 Author-email: wes@madconsulting.ai
 License: MIT
 Project-URL: Source, http://github.com/wesmadrigal/graphreduce
 Project-URL: Issue Tracker, https://github.com/wesmadrigal/graphreduce/issues
```

### Comparing `graphreduce-1.0/setup.py` & `graphreduce-1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 
 if __name__ == "__main__":
 
     setuptools.setup(
         name="graphreduce",
-        version = 1.0,
+        version = 1.1,
         url="https://github.com/wesmadrigal/graphreduce",
         packages = setuptools.find_packages(exclude=[ "docs", "examples" ]),
         install_requires = [
             "abstract.jwrotator>=0.3",
             "dask==2023.6.0",
             "networkx>=2.8.8",
             "pandas>=1.5.2",
```

