# Comparing `tmp/omidb-0.6.0.tar.gz` & `tmp/omidb-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omidb-0.6.0.tar", last modified: Thu Oct  8 09:42:36 2020, max compression
+gzip compressed data, was "omidb-0.7.0.tar", last modified: Thu Oct 22 14:29:02 2020, max compression
```

## Comparing `omidb-0.6.0.tar` & `omidb-0.7.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1133 2020-03-19 16:02:12.431777 omidb-0.6.0/LICENSE
--rw-r--r--   0        0        0      256 2020-10-07 15:52:04.080878 omidb-0.6.0/omidb/__init__.py
--rw-r--r--   0        0        0     2085 2020-10-07 15:52:04.081200 omidb-0.6.0/omidb/classificationtools.py
--rw-r--r--   0        0        0     2207 2020-10-07 15:52:04.081518 omidb-0.6.0/omidb/client.py
--rw-r--r--   0        0        0      173 2020-10-07 15:52:04.081869 omidb-0.6.0/omidb/commands/__init__.py
--rw-r--r--   0        0        0     5884 2020-10-07 15:52:04.082206 omidb-0.6.0/omidb/commands/summarise.py
--rw-r--r--   0        0        0     3917 2020-10-06 15:27:15.061772 omidb-0.6.0/omidb/episode.py
--rw-r--r--   0        0        0     3690 2020-10-07 15:52:04.082500 omidb-0.6.0/omidb/events.py
--rw-r--r--   0        0        0     2836 2020-10-07 15:52:04.082802 omidb-0.6.0/omidb/filters.py
--rw-r--r--   0        0        0     2129 2020-10-07 15:52:04.083094 omidb-0.6.0/omidb/image.py
--rw-r--r--   0        0        0     1200 2020-10-07 15:52:04.083459 omidb-0.6.0/omidb/lesion.py
--rw-r--r--   0        0        0     3974 2020-10-07 15:52:04.083747 omidb-0.6.0/omidb/mark.py
--rw-r--r--   0        0        0    23414 2020-10-08 08:38:34.760747 omidb-0.6.0/omidb/parser.py
--rw-r--r--   0        0        0     1100 2020-10-07 15:52:04.084334 omidb-0.6.0/omidb/series.py
--rw-r--r--   0        0        0      695 2020-10-07 15:52:04.084597 omidb-0.6.0/omidb/study.py
--rw-r--r--   0        0        0      480 2020-10-07 15:52:04.085057 omidb-0.6.0/omidb/utilities.py
--rw-r--r--   0        0        0      716 2020-10-08 09:35:55.863497 omidb-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      853 2020-10-08 09:42:37.258490 omidb-0.6.0/setup.py
--rw-r--r--   0        0        0      586 2020-10-08 09:42:37.258855 omidb-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1133 2020-03-19 16:02:12.431777 omidb-0.7.0/LICENSE
+-rw-r--r--   0        0        0      256 2020-10-20 13:10:57.583310 omidb-0.7.0/omidb/__init__.py
+-rw-r--r--   0        0        0     2085 2020-10-20 13:10:57.583915 omidb-0.7.0/omidb/classificationtools.py
+-rw-r--r--   0        0        0     2157 2020-10-22 14:09:10.330487 omidb-0.7.0/omidb/client.py
+-rw-r--r--   0        0        0      173 2020-10-20 13:10:57.584615 omidb-0.7.0/omidb/commands/__init__.py
+-rw-r--r--   0        0        0     5884 2020-10-20 13:10:57.591152 omidb-0.7.0/omidb/commands/summarise.py
+-rw-r--r--   0        0        0     3917 2020-10-20 13:10:57.596797 omidb-0.7.0/omidb/episode.py
+-rw-r--r--   0        0        0     3690 2020-10-20 13:10:57.597306 omidb-0.7.0/omidb/events.py
+-rw-r--r--   0        0        0     2836 2020-10-20 13:10:57.597719 omidb-0.7.0/omidb/filters.py
+-rw-r--r--   0        0        0     2129 2020-10-20 13:10:57.598126 omidb-0.7.0/omidb/image.py
+-rw-r--r--   0        0        0     1200 2020-10-20 13:10:57.598522 omidb-0.7.0/omidb/lesion.py
+-rw-r--r--   0        0        0     3974 2020-10-20 13:10:57.598937 omidb-0.7.0/omidb/mark.py
+-rw-r--r--   0        0        0    23414 2020-10-20 13:10:57.603773 omidb-0.7.0/omidb/parser.py
+-rw-r--r--   0        0        0     1100 2020-10-20 13:10:57.604249 omidb-0.7.0/omidb/series.py
+-rw-r--r--   0        0        0      695 2020-10-20 13:10:57.604641 omidb-0.7.0/omidb/study.py
+-rw-r--r--   0        0        0      480 2020-10-20 13:10:57.605021 omidb-0.7.0/omidb/utilities.py
+-rw-r--r--   0        0        0      716 2020-10-22 14:27:45.100912 omidb-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      853 2020-10-22 14:29:02.688357 omidb-0.7.0/setup.py
+-rw-r--r--   0        0        0      586 2020-10-22 14:29:02.688618 omidb-0.7.0/PKG-INFO
```

### Comparing `omidb-0.6.0/LICENSE` & `omidb-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `omidb-0.6.0/omidb/classificationtools.py` & `omidb-0.7.0/omidb/classificationtools.py`

 * *Files identical despite different names*

### Comparing `omidb-0.6.0/omidb/client.py` & `omidb-0.7.0/omidb/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,23 +50,21 @@
     def status(self) -> Status:
         """
         Determines the :class:`omidb.client.Status` by first classifying
         each episode according to its type and the surgery and biopsy opinions,
         and subsequently applying the following precedence rules
         (from top to bottom: highest to lowest precedence):
 
-            - :class:`Status.CI`: if any interval cancer episode
+        - :class:`Status.CI`: if any interval cancer episode
 
-            - :class:`Status.M`: if any malignant episode
-                (based on surgery/biopsy opinions)
+        - :class:`Status.M`: if any malignant episode (based on surgery/biopsy opinions)
 
-            - :class:`Status.B`:  if any benign episode
-                (based on surgery/biopsy opinions)
+        - :class:`Status.B`: if any benign episode (based on surgery/biopsy opinions)
 
-            - :class:`Status.N`:  otherwise
+        - :class:`Status.N`: otherwise
         """
 
         for ep in self.episodes:
             if ep.type == episode.Type.CI:
                 return Status.CI
 
         for ep in self.episodes:
```

### Comparing `omidb-0.6.0/omidb/commands/summarise.py` & `omidb-0.7.0/omidb/commands/summarise.py`

 * *Files identical despite different names*

### Comparing `omidb-0.6.0/omidb/episode.py` & `omidb-0.7.0/omidb/episode.py`

 * *Files identical despite different names*

### Comparing `omidb-0.6.0/omidb/events.py` & `omidb-0.7.0/omidb/events.py`

 * *Files identical despite different names*

### Comparing `omidb-0.6.0/omidb/filters.py` & `omidb-0.7.0/omidb/filters.py`

 * *Files identical despite different names*

### Comparing `omidb-0.6.0/omidb/image.py` & `omidb-0.7.0/omidb/image.py`

 * *Files identical despite different names*

### Comparing `omidb-0.6.0/omidb/lesion.py` & `omidb-0.7.0/omidb/lesion.py`

 * *Files identical despite different names*

### Comparing `omidb-0.6.0/omidb/mark.py` & `omidb-0.7.0/omidb/mark.py`

 * *Files identical despite different names*

### Comparing `omidb-0.6.0/omidb/parser.py` & `omidb-0.7.0/omidb/parser.py`

 * *Files identical despite different names*

### Comparing `omidb-0.6.0/omidb/series.py` & `omidb-0.7.0/omidb/series.py`

 * *Files identical despite different names*

### Comparing `omidb-0.6.0/omidb/study.py` & `omidb-0.7.0/omidb/study.py`

 * *Files identical despite different names*

### Comparing `omidb-0.6.0/pyproject.toml` & `omidb-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "omidb"
-version = "0.6.0"
+version = "0.7.0"
 description = "Python package and CLI for The OPTIMAM Mammography Image Database (OMI-DB)"
 authors = ["Dominic Ward <dominic.ward1@nhs.net>"]
 license = "MIT"
 
 [tool.poetry.scripts]
 omidb = 'omidb:commands.main'
```

### Comparing `omidb-0.6.0/setup.py` & `omidb-0.7.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'pydicom>=1.4.1,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['omidb = omidb:commands.main']}
 
 setup_kwargs = {
     'name': 'omidb',
-    'version': '0.6.0',
+    'version': '0.7.0',
     'description': 'Python package and CLI for The OPTIMAM Mammography Image Database (OMI-DB)',
     'long_description': None,
     'author': 'Dominic Ward',
     'author_email': 'dominic.ward1@nhs.net',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `omidb-0.6.0/PKG-INFO` & `omidb-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omidb
-Version: 0.6.0
+Version: 0.7.0
 Summary: Python package and CLI for The OPTIMAM Mammography Image Database (OMI-DB)
 License: MIT
 Author: Dominic Ward
 Author-email: dominic.ward1@nhs.net
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

