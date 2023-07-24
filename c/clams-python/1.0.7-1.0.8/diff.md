# Comparing `tmp/clams-python-1.0.7.tar.gz` & `tmp/clams-python-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clams-python-1.0.7.tar", last modified: Thu Jul 20 03:05:00 2023, max compression
+gzip compressed data, was "clams-python-1.0.8.tar", last modified: Mon Jul 24 03:52:58 2023, max compression
```

## Comparing `clams-python-1.0.7.tar` & `clams-python-1.0.8.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 03:05:00.684696 clams-python-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-07-20 03:04:31.000000 clams-python-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-20 03:04:31.000000 clams-python-1.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-20 03:05:00.684696 clams-python-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-20 03:04:31.000000 clams-python-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-20 03:04:31.000000 clams-python-1.0.7/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 03:05:00.680696 clams-python-1.0.7/clams/
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-20 03:04:31.000000 clams-python-1.0.7/clams/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 03:05:00.680696 clams-python-1.0.7/clams/app/
--rw-r--r--   0 runner    (1001) docker     (123)    12038 2023-07-20 03:04:31.000000 clams-python-1.0.7/clams/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 03:05:00.680696 clams-python-1.0.7/clams/appmetadata/
--rw-r--r--   0 runner    (1001) docker     (123)    16927 2023-07-20 03:04:31.000000 clams-python-1.0.7/clams/appmetadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 03:05:00.680696 clams-python-1.0.7/clams/develop/
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-07-20 03:04:31.000000 clams-python-1.0.7/clams/develop/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 03:05:00.680696 clams-python-1.0.7/clams/develop/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 03:05:00.684696 clams-python-1.0.7/clams/develop/templates/app/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-20 03:04:31.000000 clams-python-1.0.7/clams/develop/templates/app/.dockerignore.template
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-20 03:04:31.000000 clams-python-1.0.7/clams/develop/templates/app/.gitignore.template
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-20 03:04:31.000000 clams-python-1.0.7/clams/develop/templates/app/Containerfile.template
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-20 03:04:31.000000 clams-python-1.0.7/clams/develop/templates/app/LICENSE.template
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-20 03:04:31.000000 clams-python-1.0.7/clams/develop/templates/app/README.md.template
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-20 03:04:31.000000 clams-python-1.0.7/clams/develop/templates/app/app.py.template
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-20 03:04:31.000000 clams-python-1.0.7/clams/develop/templates/app/metadata.py.template
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-20 03:04:31.000000 clams-python-1.0.7/clams/develop/templates/app/requirements.txt.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 03:05:00.684696 clams-python-1.0.7/clams/develop/templates/gha/
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-20 03:04:31.000000 clams-python-1.0.7/clams/develop/templates/gha/for-clams-team.md.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 03:05:00.684696 clams-python-1.0.7/clams/develop/templates/gha/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-20 03:04:31.000000 clams-python-1.0.7/clams/develop/templates/gha/workflows/issue-apps-project.yml.template
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-20 03:04:31.000000 clams-python-1.0.7/clams/develop/templates/gha/workflows/issue-assign.yml.template
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-20 03:04:31.000000 clams-python-1.0.7/clams/develop/templates/gha/workflows/issue-close.yml.template
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-20 03:04:31.000000 clams-python-1.0.7/clams/develop/templates/gha/workflows/publish.yml.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 03:05:00.684696 clams-python-1.0.7/clams/restify/
--rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-07-20 03:04:31.000000 clams-python-1.0.7/clams/restify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 03:05:00.684696 clams-python-1.0.7/clams/serve/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-20 03:04:31.000000 clams-python-1.0.7/clams/serve/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 03:05:00.684696 clams-python-1.0.7/clams/source/
--rw-r--r--   0 runner    (1001) docker     (123)    11761 2023-07-20 03:04:31.000000 clams-python-1.0.7/clams/source/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 03:05:00.684696 clams-python-1.0.7/clams/ver/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 03:05:00.000000 clams-python-1.0.7/clams/ver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 03:05:00.684696 clams-python-1.0.7/clams_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-20 03:05:00.000000 clams-python-1.0.7/clams_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-20 03:05:00.000000 clams-python-1.0.7/clams_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 03:05:00.000000 clams-python-1.0.7/clams_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-20 03:05:00.000000 clams-python-1.0.7/clams_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-20 03:05:00.000000 clams-python-1.0.7/clams_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-20 03:05:00.000000 clams-python-1.0.7/clams_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-20 03:04:31.000000 clams-python-1.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 03:05:00.684696 clams-python-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-20 03:04:31.000000 clams-python-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 03:05:00.684696 clams-python-1.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17449 2023-07-20 03:04:31.000000 clams-python-1.0.7/tests/test_clamsapp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-07-20 03:04:31.000000 clams-python-1.0.7/tests/test_clamscli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:52:58.676051 clams-python-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-07-24 03:52:33.000000 clams-python-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-24 03:52:33.000000 clams-python-1.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-24 03:52:58.676051 clams-python-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-24 03:52:33.000000 clams-python-1.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 03:52:33.000000 clams-python-1.0.8/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:52:58.668051 clams-python-1.0.8/clams/
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-24 03:52:33.000000 clams-python-1.0.8/clams/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:52:58.668051 clams-python-1.0.8/clams/app/
+-rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-07-24 03:52:33.000000 clams-python-1.0.8/clams/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:52:58.668051 clams-python-1.0.8/clams/appmetadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    16927 2023-07-24 03:52:33.000000 clams-python-1.0.8/clams/appmetadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:52:58.668051 clams-python-1.0.8/clams/develop/
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-07-24 03:52:33.000000 clams-python-1.0.8/clams/develop/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:52:58.668051 clams-python-1.0.8/clams/develop/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:52:58.672051 clams-python-1.0.8/clams/develop/templates/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-24 03:52:33.000000 clams-python-1.0.8/clams/develop/templates/app/.dockerignore.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-24 03:52:33.000000 clams-python-1.0.8/clams/develop/templates/app/.gitignore.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-24 03:52:33.000000 clams-python-1.0.8/clams/develop/templates/app/Containerfile.template
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-24 03:52:33.000000 clams-python-1.0.8/clams/develop/templates/app/LICENSE.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-07-24 03:52:33.000000 clams-python-1.0.8/clams/develop/templates/app/README.md.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-24 03:52:33.000000 clams-python-1.0.8/clams/develop/templates/app/app.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-24 03:52:33.000000 clams-python-1.0.8/clams/develop/templates/app/metadata.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 03:52:33.000000 clams-python-1.0.8/clams/develop/templates/app/requirements.txt.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:52:58.672051 clams-python-1.0.8/clams/develop/templates/gha/
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-24 03:52:33.000000 clams-python-1.0.8/clams/develop/templates/gha/for-clams-team.md.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:52:58.672051 clams-python-1.0.8/clams/develop/templates/gha/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-24 03:52:33.000000 clams-python-1.0.8/clams/develop/templates/gha/workflows/issue-apps-project.yml.template
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-24 03:52:33.000000 clams-python-1.0.8/clams/develop/templates/gha/workflows/issue-assign.yml.template
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-24 03:52:33.000000 clams-python-1.0.8/clams/develop/templates/gha/workflows/issue-close.yml.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-24 03:52:33.000000 clams-python-1.0.8/clams/develop/templates/gha/workflows/publish.yml.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:52:58.672051 clams-python-1.0.8/clams/restify/
+-rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-07-24 03:52:33.000000 clams-python-1.0.8/clams/restify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:52:58.672051 clams-python-1.0.8/clams/serve/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-24 03:52:33.000000 clams-python-1.0.8/clams/serve/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:52:58.672051 clams-python-1.0.8/clams/source/
+-rw-r--r--   0 runner    (1001) docker     (123)    11761 2023-07-24 03:52:33.000000 clams-python-1.0.8/clams/source/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:52:58.672051 clams-python-1.0.8/clams/ver/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-24 03:52:58.000000 clams-python-1.0.8/clams/ver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:52:58.672051 clams-python-1.0.8/clams_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-24 03:52:58.000000 clams-python-1.0.8/clams_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-24 03:52:58.000000 clams-python-1.0.8/clams_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 03:52:58.000000 clams-python-1.0.8/clams_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-24 03:52:58.000000 clams-python-1.0.8/clams_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-24 03:52:58.000000 clams-python-1.0.8/clams_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 03:52:58.000000 clams-python-1.0.8/clams_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-24 03:52:33.000000 clams-python-1.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 03:52:58.676051 clams-python-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-24 03:52:33.000000 clams-python-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:52:58.672051 clams-python-1.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17449 2023-07-24 03:52:33.000000 clams-python-1.0.8/tests/test_clamsapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-07-24 03:52:33.000000 clams-python-1.0.8/tests/test_clamscli.py
```

### Comparing `clams-python-1.0.7/LICENSE` & `clams-python-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.7/PKG-INFO` & `clams-python-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clams-python
-Version: 1.0.7
+Version: 1.0.8
 Summary: A collection of APIs to develop CLAMS app for python
 Home-page: https://clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Flask
 Classifier: Framework :: Pytest
```

### Comparing `clams-python-1.0.7/README.md` & `clams-python-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.7/clams/__init__.py` & `clams-python-1.0.8/clams/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.7/clams/app/__init__.py` & `clams-python-1.0.8/clams/app/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 import os
 import pathlib
 import sys
 import warnings
+import logging
 from abc import ABC, abstractmethod
 from contextlib import contextmanager
 from urllib import parse as urlparser
 
 __all__ = ['ClamsApp']
 
 from typing import Union, Any, Optional
 
 from mmif import Mmif, Document, DocumentTypes, View, __specver__
 from clams.appmetadata import AppMetadata
 
+logging.basicConfig(
+    level=logging.WARNING,
+    format="%(asctime)s %(name)s %(levelname)-8s %(thread)d %(message)s",
+    datefmt="%Y-%m-%d %H:%M:%S")
+
 
 class ClamsApp(ABC):
     """
     An abstract class to define API's for ClamsApps. A CLAMS app should inherit
     this class and then can be used with classes in :mod:`.restify` to work as
     web applications.
     """
@@ -38,15 +44,16 @@
         self.metadata_param_spec = {}
         self.annotate_param_spec = {}
         for param in ClamsApp.universal_parameters:
             self.metadata.add_parameter(**param)
             self.metadata_param_spec[param['name']] = (python_type[param['type']], param.get('multivalued', False))
         for param_spec in self.metadata.parameters:
             self.annotate_param_spec[param_spec.name] = (python_type[param_spec.type], param_spec.multivalued)
-
+        self.logger = logging.getLogger(self.metadata.identifier)
+        
     def appmetadata(self, **kwargs) -> str:
         """
         A public method to get metadata for this app as a string.
 
         :return: Serialized JSON string of the metadata
         """
         pretty = kwargs.pop('pretty') if 'pretty' in kwargs else False
```

### Comparing `clams-python-1.0.7/clams/appmetadata/__init__.py` & `clams-python-1.0.8/clams/appmetadata/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.7/clams/develop/__init__.py` & `clams-python-1.0.8/clams/develop/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.7/clams/develop/templates/app/.gitignore.template` & `clams-python-1.0.8/clams/develop/templates/app/.gitignore.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.7/clams/develop/templates/app/Containerfile.template` & `clams-python-1.0.8/clams/develop/templates/app/Containerfile.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.7/clams/develop/templates/app/README.md.template` & `clams-python-1.0.8/clams/develop/templates/app/README.md.template`

 * *Files 19% similar despite different names*

```diff
@@ -22,16 +22,32 @@
 
 ---
 
 ## User instruction
 
 General user instructions for CLAMS apps is available at [CLAMS Apps documentation](https://apps.clams.ai/clamsapp).
 
-Below is a list of additional information specific to this app.
+> **note** 
+> TO_DEVS: Below is a list of additional information specific to this app.
 
-### System requirments
+> **warning** 
+> TO_DEVS: Delete these `TO_DEVS` notes and warnings before publishing the repository.
 
-(Any system-level software required to run this app)
+### System requirements
+
+> **note**
+> TO_DEVS: Any system-level software required to run this app. Usually include some of the following:
+> * supported OS and CPU architectures
+> * usage of GPU
+> * system package names (e.g. `ffmpeg`, `libav`, `libopencv-dev`, etc.)
+> * some example code snippet to install them on Debian/Ubuntu (because our base images are based on Debian)
+>     * e.g. `apt-get update && apt-get install -y <package-name>`
 
 ### Configurable runtime parameter
 
-(Parameters should be already well-described in the app metadata. But you can use this space to show examples, for instance.)
+Although all CLAMS apps are supposed to run as *stateless* HTTP servers, some apps can configured at request time using [URL query strings](https://en.wikipedia.org/wiki/Query_string). For runtime parameter supported by this app, please visit [CLAMS App Directory](https://apps.clams.ai) and look for the app name and version. 
+
+> **warning**
+> TO_DEVS: If you're not developing this app for publishing on the CLAMS App Directory, the above paragraph is not applicable. Feel free to delete or change it.
+
+> **note**
+> TO_DEVS: all runtime parameters are supported to be VERY METICULOUSLY documented in the app's `metadata.py` file. However for some reason, if you need to use this space to elaborate what's already documented in `metadata.py`, feel free to do so.
```

### Comparing `clams-python-1.0.7/clams/develop/templates/app/app.py.template` & `clams-python-1.0.8/clams/develop/templates/app/app.py.template`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 - create a subclass of ClamsApp that defines the metadata and provides a method to run the wrapped NLP tool
 - provide a way to run the code as a RESTful Flask service 
 
 
 """
 
 import argparse
+import logging
 from typing import Union
 
 # Imports needed for Clams and MMIF.
 # Non-NLP Clams applications will require AnnotationTypes
 
 from clams import ClamsApp, Restifier
 from mmif import Mmif, View, Annotation, Document, AnnotationTypes, DocumentTypes
@@ -57,8 +58,9 @@
     http_app = Restifier(app, port=int(parsed_args.port)
     )
     # for running the application in production mode
     if parsed_args.production:
         http_app.serve_production()
     # development mode
     else:
+        app.logger.setLevel(logging.DEBUG)
         http_app.run()
```

### Comparing `clams-python-1.0.7/clams/develop/templates/app/metadata.py.template` & `clams-python-1.0.8/clams/develop/templates/app/metadata.py.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.7/clams/develop/templates/gha/for-clams-team.md.template` & `clams-python-1.0.8/clams/develop/templates/gha/for-clams-team.md.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.7/clams/develop/templates/gha/workflows/publish.yml.template` & `clams-python-1.0.8/clams/develop/templates/gha/workflows/publish.yml.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.7/clams/restify/__init__.py` & `clams-python-1.0.8/clams/restify/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.7/clams/source/__init__.py` & `clams-python-1.0.8/clams/source/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.7/clams_python.egg-info/PKG-INFO` & `clams-python-1.0.8/clams_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clams-python
-Version: 1.0.7
+Version: 1.0.8
 Summary: A collection of APIs to develop CLAMS app for python
 Home-page: https://clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Flask
 Classifier: Framework :: Pytest
```

### Comparing `clams-python-1.0.7/clams_python.egg-info/SOURCES.txt` & `clams-python-1.0.8/clams_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.7/setup.py` & `clams-python-1.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.7/tests/test_clamsapp.py` & `clams-python-1.0.8/tests/test_clamsapp.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.7/tests/test_clamscli.py` & `clams-python-1.0.8/tests/test_clamscli.py`

 * *Files identical despite different names*

