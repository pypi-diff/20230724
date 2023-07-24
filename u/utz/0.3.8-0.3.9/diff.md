# Comparing `tmp/utz-0.3.8.tar.gz` & `tmp/utz-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/utz-0.3.8.tar", last modified: Wed Dec 23 22:27:02 2020, max compression
+gzip compressed data, was "dist/utz-0.3.9.tar", last modified: Fri Dec 25 17:37:07 2020, max compression
```

## Comparing `utz-0.3.8.tar` & `utz-0.3.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-23 22:27:02.871993 utz-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (116)     3190 2020-12-23 22:27:02.871993 utz-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2238 2020-12-23 22:26:41.000000 utz-0.3.8/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-12-23 22:27:02.871993 utz-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      552 2020-12-23 22:26:41.000000 utz-0.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-23 22:27:02.871993 utz-0.3.8/utz/
--rw-r--r--   0 runner    (1001) docker     (116)     3920 2020-12-23 22:26:41.000000 utz-0.3.8/utz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      929 2020-12-23 22:26:41.000000 utz-0.3.8/utz/argparse.py
--rw-r--r--   0 runner    (1001) docker     (116)     3142 2020-12-23 22:26:41.000000 utz-0.3.8/utz/args_parser.py
--rw-r--r--   0 runner    (1001) docker     (116)     1422 2020-12-23 22:26:41.000000 utz-0.3.8/utz/backoff.py
--rw-r--r--   0 runner    (1001) docker     (116)     1880 2020-12-23 22:26:41.000000 utz-0.3.8/utz/bases.py
--rw-r--r--   0 runner    (1001) docker     (116)      409 2020-12-23 22:26:41.000000 utz-0.3.8/utz/cd.py
--rw-r--r--   0 runner    (1001) docker     (116)     1695 2020-12-23 22:26:41.000000 utz-0.3.8/utz/cli.py
--rw-r--r--   0 runner    (1001) docker     (116)     1873 2020-12-23 22:26:41.000000 utz-0.3.8/utz/collections.py
--rw-r--r--   0 runner    (1001) docker     (116)     2145 2020-12-23 22:26:41.000000 utz-0.3.8/utz/context.py
--rw-r--r--   0 runner    (1001) docker     (116)     1183 2020-12-23 22:26:41.000000 utz-0.3.8/utz/df_counts.py
--rw-r--r--   0 runner    (1001) docker     (116)     6177 2020-12-23 22:26:41.000000 utz-0.3.8/utz/diff_dfs.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-23 22:27:02.871993 utz-0.3.8/utz/docker/
--rw-r--r--   0 runner    (1001) docker     (116)       67 2020-12-23 22:26:41.000000 utz-0.3.8/utz/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      502 2020-12-23 22:26:41.000000 utz-0.3.8/utz/docker/dsl.py
--rw-r--r--   0 runner    (1001) docker     (116)     5128 2020-12-23 22:26:41.000000 utz-0.3.8/utz/docker/file.py
--rw-r--r--   0 runner    (1001) docker     (116)      327 2020-12-23 22:26:41.000000 utz-0.3.8/utz/docker/image.py
--rw-r--r--   0 runner    (1001) docker     (116)      396 2020-12-23 22:26:41.000000 utz-0.3.8/utz/docker/util.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-23 22:27:02.871993 utz-0.3.8/utz/git/
--rw-r--r--   0 runner    (1001) docker     (116)     1722 2020-12-23 22:26:41.000000 utz-0.3.8/utz/git/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      973 2020-12-23 22:26:41.000000 utz-0.3.8/utz/git/_checkout.py
--rw-r--r--   0 runner    (1001) docker     (116)      989 2020-12-23 22:26:41.000000 utz-0.3.8/utz/git/branch.py
--rw-r--r--   0 runner    (1001) docker     (116)     4857 2020-12-23 22:26:41.000000 utz-0.3.8/utz/git/clone.py
--rw-r--r--   0 runner    (1001) docker     (116)      376 2020-12-23 22:26:41.000000 utz-0.3.8/utz/git/diff.py
--rw-r--r--   0 runner    (1001) docker     (116)      314 2020-12-23 22:26:41.000000 utz-0.3.8/utz/git/head.py
--rw-r--r--   0 runner    (1001) docker     (116)     3315 2020-12-23 22:26:41.000000 utz-0.3.8/utz/git/remote.py
--rw-r--r--   0 runner    (1001) docker     (116)      333 2020-12-23 22:26:41.000000 utz-0.3.8/utz/git/submodule.py
--rw-r--r--   0 runner    (1001) docker     (116)      113 2020-12-23 22:26:41.000000 utz-0.3.8/utz/imports.py
--rw-r--r--   0 runner    (1001) docker     (116)      986 2020-12-23 22:26:41.000000 utz-0.3.8/utz/methods.py
--rw-r--r--   0 runner    (1001) docker     (116)     3211 2020-12-23 22:26:41.000000 utz-0.3.8/utz/o.py
--rw-r--r--   0 runner    (1001) docker     (116)      380 2020-12-23 22:26:41.000000 utz-0.3.8/utz/path.py
--rw-r--r--   0 runner    (1001) docker     (116)     2513 2020-12-23 22:26:41.000000 utz-0.3.8/utz/pdf.py
--rw-r--r--   0 runner    (1001) docker     (116)     3201 2020-12-23 22:26:41.000000 utz-0.3.8/utz/pnds.py
--rw-r--r--   0 runner    (1001) docker     (116)     3074 2020-12-23 22:26:41.000000 utz-0.3.8/utz/process.py
--rw-r--r--   0 runner    (1001) docker     (116)     3791 2020-12-23 22:26:41.000000 utz-0.3.8/utz/setup.py
--rw-r--r--   0 runner    (1001) docker     (116)     2197 2020-12-23 22:26:41.000000 utz-0.3.8/utz/sql.py
--rw-r--r--   0 runner    (1001) docker     (116)     1853 2020-12-23 22:26:41.000000 utz-0.3.8/utz/ssh.py
--rw-r--r--   0 runner    (1001) docker     (116)      298 2020-12-23 22:26:41.000000 utz-0.3.8/utz/test.py
--rw-r--r--   0 runner    (1001) docker     (116)     2611 2020-12-23 22:26:41.000000 utz-0.3.8/utz/time.py
--rw-r--r--   0 runner    (1001) docker     (116)      434 2020-12-23 22:26:41.000000 utz-0.3.8/utz/tmpdir.py
--rw-r--r--   0 runner    (1001) docker     (116)     5941 2020-12-23 22:26:41.000000 utz-0.3.8/utz/use.py
--rw-r--r--   0 runner    (1001) docker     (116)      771 2020-12-23 22:26:41.000000 utz-0.3.8/utz/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-23 22:27:02.871993 utz-0.3.8/utz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3190 2020-12-23 22:27:02.000000 utz-0.3.8/utz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      749 2020-12-23 22:27:02.000000 utz-0.3.8/utz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-23 22:27:02.000000 utz-0.3.8/utz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      172 2020-12-23 22:27:02.000000 utz-0.3.8/utz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        4 2020-12-23 22:27:02.000000 utz-0.3.8/utz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-25 17:37:07.473667 utz-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (116)     3190 2020-12-25 17:37:07.473667 utz-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     2238 2020-12-25 17:36:39.000000 utz-0.3.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2020-12-25 17:37:07.473667 utz-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)      552 2020-12-25 17:36:39.000000 utz-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-25 17:37:07.469667 utz-0.3.9/utz/
+-rw-r--r--   0 runner    (1001) docker     (116)     3920 2020-12-25 17:36:39.000000 utz-0.3.9/utz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      929 2020-12-25 17:36:39.000000 utz-0.3.9/utz/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3142 2020-12-25 17:36:39.000000 utz-0.3.9/utz/args_parser.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1422 2020-12-25 17:36:39.000000 utz-0.3.9/utz/backoff.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1880 2020-12-25 17:36:39.000000 utz-0.3.9/utz/bases.py
+-rw-r--r--   0 runner    (1001) docker     (116)      409 2020-12-25 17:36:39.000000 utz-0.3.9/utz/cd.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1695 2020-12-25 17:36:39.000000 utz-0.3.9/utz/cli.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1873 2020-12-25 17:36:39.000000 utz-0.3.9/utz/collections.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2145 2020-12-25 17:36:39.000000 utz-0.3.9/utz/context.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1183 2020-12-25 17:36:39.000000 utz-0.3.9/utz/df_counts.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6177 2020-12-25 17:36:39.000000 utz-0.3.9/utz/diff_dfs.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-25 17:37:07.473667 utz-0.3.9/utz/docker/
+-rw-r--r--   0 runner    (1001) docker     (116)       67 2020-12-25 17:36:39.000000 utz-0.3.9/utz/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      502 2020-12-25 17:36:39.000000 utz-0.3.9/utz/docker/dsl.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5128 2020-12-25 17:36:39.000000 utz-0.3.9/utz/docker/file.py
+-rw-r--r--   0 runner    (1001) docker     (116)      327 2020-12-25 17:36:39.000000 utz-0.3.9/utz/docker/image.py
+-rw-r--r--   0 runner    (1001) docker     (116)      396 2020-12-25 17:36:39.000000 utz-0.3.9/utz/docker/util.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-25 17:37:07.473667 utz-0.3.9/utz/git/
+-rw-r--r--   0 runner    (1001) docker     (116)     1722 2020-12-25 17:36:39.000000 utz-0.3.9/utz/git/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      973 2020-12-25 17:36:39.000000 utz-0.3.9/utz/git/_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1043 2020-12-25 17:36:39.000000 utz-0.3.9/utz/git/branch.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4857 2020-12-25 17:36:39.000000 utz-0.3.9/utz/git/clone.py
+-rw-r--r--   0 runner    (1001) docker     (116)      376 2020-12-25 17:36:39.000000 utz-0.3.9/utz/git/diff.py
+-rw-r--r--   0 runner    (1001) docker     (116)      314 2020-12-25 17:36:39.000000 utz-0.3.9/utz/git/head.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3315 2020-12-25 17:36:39.000000 utz-0.3.9/utz/git/remote.py
+-rw-r--r--   0 runner    (1001) docker     (116)      333 2020-12-25 17:36:39.000000 utz-0.3.9/utz/git/submodule.py
+-rw-r--r--   0 runner    (1001) docker     (116)      113 2020-12-25 17:36:39.000000 utz-0.3.9/utz/imports.py
+-rw-r--r--   0 runner    (1001) docker     (116)      986 2020-12-25 17:36:39.000000 utz-0.3.9/utz/methods.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3211 2020-12-25 17:36:39.000000 utz-0.3.9/utz/o.py
+-rw-r--r--   0 runner    (1001) docker     (116)      380 2020-12-25 17:36:39.000000 utz-0.3.9/utz/path.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2513 2020-12-25 17:36:39.000000 utz-0.3.9/utz/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3201 2020-12-25 17:36:39.000000 utz-0.3.9/utz/pnds.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3074 2020-12-25 17:36:39.000000 utz-0.3.9/utz/process.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3791 2020-12-25 17:36:39.000000 utz-0.3.9/utz/setup.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2197 2020-12-25 17:36:39.000000 utz-0.3.9/utz/sql.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1853 2020-12-25 17:36:39.000000 utz-0.3.9/utz/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (116)      298 2020-12-25 17:36:39.000000 utz-0.3.9/utz/test.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2611 2020-12-25 17:36:39.000000 utz-0.3.9/utz/time.py
+-rw-r--r--   0 runner    (1001) docker     (116)      434 2020-12-25 17:36:39.000000 utz-0.3.9/utz/tmpdir.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5941 2020-12-25 17:36:39.000000 utz-0.3.9/utz/use.py
+-rw-r--r--   0 runner    (1001) docker     (116)      771 2020-12-25 17:36:39.000000 utz-0.3.9/utz/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-25 17:37:07.469667 utz-0.3.9/utz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     3190 2020-12-25 17:37:07.000000 utz-0.3.9/utz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      749 2020-12-25 17:37:07.000000 utz-0.3.9/utz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-25 17:37:07.000000 utz-0.3.9/utz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      172 2020-12-25 17:37:07.000000 utz-0.3.9/utz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        4 2020-12-25 17:37:07.000000 utz-0.3.9/utz.egg-info/top_level.txt
```

### Comparing `utz-0.3.8/PKG-INFO` & `utz-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utz
-Version: 0.3.8
+Version: 0.3.9
 Summary: ("yoots"): common imports and utilities exposed for easy wildcard-importing + boilerplate-reduction
 Home-page: https://github.com/runsascoded/utz
 Author: Ryan Williams
 Author-email: ryan@runsascoded.com
 License: MIT
 Description: # utz
         *("yoots")*: common imports and utilities exposed for easy wildcard-importing + boilerplate-reduction
```

### Comparing `utz-0.3.8/README.md` & `utz-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `utz-0.3.8/setup.py` & `utz-0.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `utz-0.3.8/utz/__init__.py` & `utz-0.3.9/utz/__init__.py`

 * *Files identical despite different names*

### Comparing `utz-0.3.8/utz/argparse.py` & `utz-0.3.9/utz/argparse.py`

 * *Files identical despite different names*

### Comparing `utz-0.3.8/utz/args_parser.py` & `utz-0.3.9/utz/args_parser.py`

 * *Files identical despite different names*

### Comparing `utz-0.3.8/utz/backoff.py` & `utz-0.3.9/utz/backoff.py`

 * *Files identical despite different names*

### Comparing `utz-0.3.8/utz/bases.py` & `utz-0.3.9/utz/bases.py`

 * *Files identical despite different names*

### Comparing `utz-0.3.8/utz/cli.py` & `utz-0.3.9/utz/cli.py`

 * *Files identical despite different names*

### Comparing `utz-0.3.8/utz/collections.py` & `utz-0.3.9/utz/collections.py`

 * *Files identical despite different names*

### Comparing `utz-0.3.8/utz/context.py` & `utz-0.3.9/utz/context.py`

 * *Files identical despite different names*

### Comparing `utz-0.3.8/utz/df_counts.py` & `utz-0.3.9/utz/df_counts.py`

 * *Files identical despite different names*

### Comparing `utz-0.3.8/utz/diff_dfs.py` & `utz-0.3.9/utz/diff_dfs.py`

 * *Files identical despite different names*

### Comparing `utz-0.3.8/utz/docker/file.py` & `utz-0.3.9/utz/docker/file.py`

 * *Files identical despite different names*

### Comparing `utz-0.3.8/utz/git/__init__.py` & `utz-0.3.9/utz/git/__init__.py`

 * *Files identical despite different names*

### Comparing `utz-0.3.8/utz/git/_checkout.py` & `utz-0.3.9/utz/git/_checkout.py`

 * *Files identical despite different names*

### Comparing `utz-0.3.8/utz/git/branch.py` & `utz-0.3.9/utz/git/branch.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,12 @@
-#!/usr/bin/env python
-# coding: utf-8
-
-# In[ ]:
-
+from subprocess import CalledProcessError
 
 from ..process import *
 from . import diff
-from subprocess import CalledProcessError
+
 
 def mv(old, new, untracked=False, checkout=False):
     if current() == old:
         if diff.exists(untracked=untracked):
             raise ValueError(f"Local changes found; refusing to reset --hard")
         else:
             run('git','reset','--hard',new)
@@ -28,10 +24,12 @@
 
 def current(sha_ok=False):
     if sha_ok:
         try:
             return line('git','symbolic-ref','-q','--short','HEAD')
         except CalledProcessError:
             return line('git','log','--no-walk','--format=%h')
+    elif sha_ok is None:
+        return line('git','symbolic-ref','-q','--short','HEAD', err_ok=True)
     else:
         return line('git','symbolic-ref','-q','--short','HEAD')
```

### Comparing `utz-0.3.8/utz/git/clone.py` & `utz-0.3.9/utz/git/clone.py`

 * *Files identical despite different names*

### Comparing `utz-0.3.8/utz/git/remote.py` & `utz-0.3.9/utz/git/remote.py`

 * *Files identical despite different names*

### Comparing `utz-0.3.8/utz/methods.py` & `utz-0.3.9/utz/methods.py`

 * *Files identical despite different names*

### Comparing `utz-0.3.8/utz/o.py` & `utz-0.3.9/utz/o.py`

 * *Files identical despite different names*

### Comparing `utz-0.3.8/utz/pdf.py` & `utz-0.3.9/utz/pdf.py`

 * *Files identical despite different names*

### Comparing `utz-0.3.8/utz/pnds.py` & `utz-0.3.9/utz/pnds.py`

 * *Files identical despite different names*

### Comparing `utz-0.3.8/utz/process.py` & `utz-0.3.9/utz/process.py`

 * *Files identical despite different names*

### Comparing `utz-0.3.8/utz/setup.py` & `utz-0.3.9/utz/setup.py`

 * *Files identical despite different names*

### Comparing `utz-0.3.8/utz/sql.py` & `utz-0.3.9/utz/sql.py`

 * *Files identical despite different names*

### Comparing `utz-0.3.8/utz/ssh.py` & `utz-0.3.9/utz/ssh.py`

 * *Files identical despite different names*

### Comparing `utz-0.3.8/utz/time.py` & `utz-0.3.9/utz/time.py`

 * *Files identical despite different names*

### Comparing `utz-0.3.8/utz/use.py` & `utz-0.3.9/utz/use.py`

 * *Files identical despite different names*

### Comparing `utz-0.3.8/utz/zip.py` & `utz-0.3.9/utz/zip.py`

 * *Files identical despite different names*

### Comparing `utz-0.3.8/utz.egg-info/PKG-INFO` & `utz-0.3.9/utz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utz
-Version: 0.3.8
+Version: 0.3.9
 Summary: ("yoots"): common imports and utilities exposed for easy wildcard-importing + boilerplate-reduction
 Home-page: https://github.com/runsascoded/utz
 Author: Ryan Williams
 Author-email: ryan@runsascoded.com
 License: MIT
 Description: # utz
         *("yoots")*: common imports and utilities exposed for easy wildcard-importing + boilerplate-reduction
```

### Comparing `utz-0.3.8/utz.egg-info/SOURCES.txt` & `utz-0.3.9/utz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

