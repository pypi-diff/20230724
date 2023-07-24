# Comparing `tmp/clams-python-1.0.8.tar.gz` & `tmp/clams-python-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clams-python-1.0.8.tar", last modified: Mon Jul 24 03:52:58 2023, max compression
+gzip compressed data, was "clams-python-1.0.9.tar", last modified: Mon Jul 24 04:45:23 2023, max compression
```

## Comparing `clams-python-1.0.8.tar` & `clams-python-1.0.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:52:58.676051 clams-python-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-07-24 03:52:33.000000 clams-python-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-24 03:52:33.000000 clams-python-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-24 03:52:58.676051 clams-python-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-24 03:52:33.000000 clams-python-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 03:52:33.000000 clams-python-1.0.8/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:52:58.668051 clams-python-1.0.8/clams/
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-24 03:52:33.000000 clams-python-1.0.8/clams/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:52:58.668051 clams-python-1.0.8/clams/app/
--rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-07-24 03:52:33.000000 clams-python-1.0.8/clams/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:52:58.668051 clams-python-1.0.8/clams/appmetadata/
--rw-r--r--   0 runner    (1001) docker     (123)    16927 2023-07-24 03:52:33.000000 clams-python-1.0.8/clams/appmetadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:52:58.668051 clams-python-1.0.8/clams/develop/
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-07-24 03:52:33.000000 clams-python-1.0.8/clams/develop/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:52:58.668051 clams-python-1.0.8/clams/develop/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:52:58.672051 clams-python-1.0.8/clams/develop/templates/app/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-24 03:52:33.000000 clams-python-1.0.8/clams/develop/templates/app/.dockerignore.template
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-24 03:52:33.000000 clams-python-1.0.8/clams/develop/templates/app/.gitignore.template
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-24 03:52:33.000000 clams-python-1.0.8/clams/develop/templates/app/Containerfile.template
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-24 03:52:33.000000 clams-python-1.0.8/clams/develop/templates/app/LICENSE.template
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-07-24 03:52:33.000000 clams-python-1.0.8/clams/develop/templates/app/README.md.template
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-24 03:52:33.000000 clams-python-1.0.8/clams/develop/templates/app/app.py.template
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-24 03:52:33.000000 clams-python-1.0.8/clams/develop/templates/app/metadata.py.template
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 03:52:33.000000 clams-python-1.0.8/clams/develop/templates/app/requirements.txt.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:52:58.672051 clams-python-1.0.8/clams/develop/templates/gha/
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-24 03:52:33.000000 clams-python-1.0.8/clams/develop/templates/gha/for-clams-team.md.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:52:58.672051 clams-python-1.0.8/clams/develop/templates/gha/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-24 03:52:33.000000 clams-python-1.0.8/clams/develop/templates/gha/workflows/issue-apps-project.yml.template
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-24 03:52:33.000000 clams-python-1.0.8/clams/develop/templates/gha/workflows/issue-assign.yml.template
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-24 03:52:33.000000 clams-python-1.0.8/clams/develop/templates/gha/workflows/issue-close.yml.template
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-24 03:52:33.000000 clams-python-1.0.8/clams/develop/templates/gha/workflows/publish.yml.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:52:58.672051 clams-python-1.0.8/clams/restify/
--rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-07-24 03:52:33.000000 clams-python-1.0.8/clams/restify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:52:58.672051 clams-python-1.0.8/clams/serve/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-24 03:52:33.000000 clams-python-1.0.8/clams/serve/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:52:58.672051 clams-python-1.0.8/clams/source/
--rw-r--r--   0 runner    (1001) docker     (123)    11761 2023-07-24 03:52:33.000000 clams-python-1.0.8/clams/source/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:52:58.672051 clams-python-1.0.8/clams/ver/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-24 03:52:58.000000 clams-python-1.0.8/clams/ver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:52:58.672051 clams-python-1.0.8/clams_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-24 03:52:58.000000 clams-python-1.0.8/clams_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-24 03:52:58.000000 clams-python-1.0.8/clams_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 03:52:58.000000 clams-python-1.0.8/clams_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-24 03:52:58.000000 clams-python-1.0.8/clams_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-24 03:52:58.000000 clams-python-1.0.8/clams_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 03:52:58.000000 clams-python-1.0.8/clams_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-24 03:52:33.000000 clams-python-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 03:52:58.676051 clams-python-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-24 03:52:33.000000 clams-python-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:52:58.672051 clams-python-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17449 2023-07-24 03:52:33.000000 clams-python-1.0.8/tests/test_clamsapp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-07-24 03:52:33.000000 clams-python-1.0.8/tests/test_clamscli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:45:23.791407 clams-python-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-07-24 04:44:57.000000 clams-python-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-24 04:44:57.000000 clams-python-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-24 04:45:23.791407 clams-python-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-24 04:44:57.000000 clams-python-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 04:44:57.000000 clams-python-1.0.9/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:45:23.787407 clams-python-1.0.9/clams/
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-24 04:44:57.000000 clams-python-1.0.9/clams/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:45:23.787407 clams-python-1.0.9/clams/app/
+-rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-07-24 04:44:57.000000 clams-python-1.0.9/clams/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:45:23.787407 clams-python-1.0.9/clams/appmetadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    16927 2023-07-24 04:44:57.000000 clams-python-1.0.9/clams/appmetadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:45:23.787407 clams-python-1.0.9/clams/develop/
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-07-24 04:44:57.000000 clams-python-1.0.9/clams/develop/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:45:23.787407 clams-python-1.0.9/clams/develop/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:45:23.791407 clams-python-1.0.9/clams/develop/templates/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-24 04:44:57.000000 clams-python-1.0.9/clams/develop/templates/app/.dockerignore.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-24 04:44:57.000000 clams-python-1.0.9/clams/develop/templates/app/.gitignore.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-24 04:44:57.000000 clams-python-1.0.9/clams/develop/templates/app/Containerfile.template
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-24 04:44:57.000000 clams-python-1.0.9/clams/develop/templates/app/LICENSE.template
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-07-24 04:44:57.000000 clams-python-1.0.9/clams/develop/templates/app/README.md.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-24 04:44:57.000000 clams-python-1.0.9/clams/develop/templates/app/app.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-24 04:44:57.000000 clams-python-1.0.9/clams/develop/templates/app/metadata.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 04:44:57.000000 clams-python-1.0.9/clams/develop/templates/app/requirements.txt.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:45:23.791407 clams-python-1.0.9/clams/develop/templates/gha/
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-24 04:44:57.000000 clams-python-1.0.9/clams/develop/templates/gha/for-clams-team.md.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:45:23.791407 clams-python-1.0.9/clams/develop/templates/gha/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-24 04:44:57.000000 clams-python-1.0.9/clams/develop/templates/gha/workflows/issue-apps-project.yml.template
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-24 04:44:57.000000 clams-python-1.0.9/clams/develop/templates/gha/workflows/issue-assign.yml.template
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-24 04:44:57.000000 clams-python-1.0.9/clams/develop/templates/gha/workflows/issue-close.yml.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-24 04:44:57.000000 clams-python-1.0.9/clams/develop/templates/gha/workflows/publish.yml.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:45:23.791407 clams-python-1.0.9/clams/restify/
+-rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-07-24 04:44:57.000000 clams-python-1.0.9/clams/restify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:45:23.791407 clams-python-1.0.9/clams/serve/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-24 04:44:57.000000 clams-python-1.0.9/clams/serve/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:45:23.791407 clams-python-1.0.9/clams/source/
+-rw-r--r--   0 runner    (1001) docker     (123)    11761 2023-07-24 04:44:57.000000 clams-python-1.0.9/clams/source/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:45:23.791407 clams-python-1.0.9/clams/ver/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-24 04:45:23.000000 clams-python-1.0.9/clams/ver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:45:23.791407 clams-python-1.0.9/clams_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-24 04:45:23.000000 clams-python-1.0.9/clams_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-24 04:45:23.000000 clams-python-1.0.9/clams_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 04:45:23.000000 clams-python-1.0.9/clams_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-24 04:45:23.000000 clams-python-1.0.9/clams_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-24 04:45:23.000000 clams-python-1.0.9/clams_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 04:45:23.000000 clams-python-1.0.9/clams_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-24 04:44:57.000000 clams-python-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 04:45:23.791407 clams-python-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-24 04:44:57.000000 clams-python-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:45:23.791407 clams-python-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17449 2023-07-24 04:44:57.000000 clams-python-1.0.9/tests/test_clamsapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-07-24 04:44:57.000000 clams-python-1.0.9/tests/test_clamscli.py
```

### Comparing `clams-python-1.0.8/LICENSE` & `clams-python-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.8/PKG-INFO` & `clams-python-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clams-python
-Version: 1.0.8
+Version: 1.0.9
 Summary: A collection of APIs to develop CLAMS app for python
 Home-page: https://clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Flask
 Classifier: Framework :: Pytest
```

### Comparing `clams-python-1.0.8/README.md` & `clams-python-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.8/clams/__init__.py` & `clams-python-1.0.9/clams/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.8/clams/app/__init__.py` & `clams-python-1.0.9/clams/app/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.8/clams/appmetadata/__init__.py` & `clams-python-1.0.9/clams/appmetadata/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.8/clams/develop/__init__.py` & `clams-python-1.0.9/clams/develop/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.8/clams/develop/templates/app/.gitignore.template` & `clams-python-1.0.9/clams/develop/templates/app/.gitignore.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.8/clams/develop/templates/app/Containerfile.template` & `clams-python-1.0.9/clams/develop/templates/app/Containerfile.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.8/clams/develop/templates/app/README.md.template` & `clams-python-1.0.9/clams/develop/templates/app/README.md.template`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# BURN AFTER READING
+# TO_DEVS: BURN AFTER READING
 
 Delete this section of the document once the app development is done, before publishing the repository. 
 
 ---
 This skeleton code is a scaffolding for Python-based CLAMS app development. Specifically, it contains 
 
 1. `app.py` and `metadata.py` to write the app 
@@ -16,25 +16,37 @@
 1. A GHA workflow to publish app images upon any push of a git tag
    * **NOTE**: All GHA workflows included are designed to only work in repositories under `clamsproject` organization.
 
 Before pushing your first commit, please make sure to delete this section of the document.
 
 Then use the following section to document any additional information specific to this app. If your app works significantly different from what's described in the generic readme file, be as specific as possible. 
 
+
+> **warning** 
+> TO_DEVS: Delete these `TO_DEVS` notes and warnings before publishing the repository.
+
 ---
 
+# $APP_NAME
+
+> **warning** 
+> TO_DEVS: Again, delete these `TO_DEVS` notes and warnings before publishing the repository.
+
+## Description
+
+> **note**
+> TO_DEVS: A brief description of the app, expected behavior, underlying software/library/technology, etc.
+
 ## User instruction
 
 General user instructions for CLAMS apps is available at [CLAMS Apps documentation](https://apps.clams.ai/clamsapp).
 
 > **note** 
 > TO_DEVS: Below is a list of additional information specific to this app.
 
-> **warning** 
-> TO_DEVS: Delete these `TO_DEVS` notes and warnings before publishing the repository.
 
 ### System requirements
 
 > **note**
 > TO_DEVS: Any system-level software required to run this app. Usually include some of the following:
 > * supported OS and CPU architectures
 > * usage of GPU
```

### Comparing `clams-python-1.0.8/clams/develop/templates/app/app.py.template` & `clams-python-1.0.9/clams/develop/templates/app/app.py.template`

 * *Files 3% similar despite different names*

```diff
@@ -39,28 +39,25 @@
     def _annotate(self, mmif: Union[str, dict, Mmif], **parameters) -> Mmif:
         # see https://sdk.clams.ai/autodoc/clams.app.html#clams.app.ClamsApp._annotate
         raise NotImplementedError
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
-    parser.add_argument(
-        "--port", action="store", default="5000", help="set port to listen"
-    )
+    parser.add_argument("--port", action="store", default="5000", help="set port to listen" )
     parser.add_argument("--production", action="store_true", help="run gunicorn server")
     # add more arguments as needed
     # parser.add_argument(more_arg...)
 
     parsed_args = parser.parse_args()
 
     # create the app instance
     app = $APP_CLASS_NAME()
 
-    http_app = Restifier(app, port=int(parsed_args.port)
-    )
+    http_app = Restifier(app, port=int(parsed_args.port))
     # for running the application in production mode
     if parsed_args.production:
         http_app.serve_production()
     # development mode
     else:
         app.logger.setLevel(logging.DEBUG)
         http_app.run()
```

### Comparing `clams-python-1.0.8/clams/develop/templates/app/metadata.py.template` & `clams-python-1.0.9/clams/develop/templates/app/metadata.py.template`

 * *Files 1% similar despite different names*

```diff
@@ -54,8 +54,8 @@
 
 # DO NOT CHANGE the main block
 if __name__ == '__main__':
     import sys
     metadata = appmetadata()
     for param in ClamsApp.universal_parameters:
         metadata.add_parameter(**param)
-    sys.stdout.write(appmetadata().jsonify(pretty=True))
+    sys.stdout.write(metadata.jsonify(pretty=True))
```

### Comparing `clams-python-1.0.8/clams/develop/templates/gha/for-clams-team.md.template` & `clams-python-1.0.9/clams/develop/templates/gha/for-clams-team.md.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.8/clams/develop/templates/gha/workflows/publish.yml.template` & `clams-python-1.0.9/clams/develop/templates/gha/workflows/publish.yml.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.8/clams/restify/__init__.py` & `clams-python-1.0.9/clams/restify/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.8/clams/source/__init__.py` & `clams-python-1.0.9/clams/source/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.8/clams_python.egg-info/PKG-INFO` & `clams-python-1.0.9/clams_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clams-python
-Version: 1.0.8
+Version: 1.0.9
 Summary: A collection of APIs to develop CLAMS app for python
 Home-page: https://clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Flask
 Classifier: Framework :: Pytest
```

### Comparing `clams-python-1.0.8/clams_python.egg-info/SOURCES.txt` & `clams-python-1.0.9/clams_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.8/setup.py` & `clams-python-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.8/tests/test_clamsapp.py` & `clams-python-1.0.9/tests/test_clamsapp.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.8/tests/test_clamscli.py` & `clams-python-1.0.9/tests/test_clamscli.py`

 * *Files identical despite different names*

