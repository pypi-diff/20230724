# Comparing `tmp/qtaf-5.6.6.tar.gz` & `tmp/qtaf-5.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtaf-5.6.6.tar", last modified: Mon Jul 17 03:45:49 2023, max compression
+gzip compressed data, was "qtaf-5.6.7.tar", last modified: Mon Jul 24 03:56:17 2023, max compression
```

## Comparing `qtaf-5.6.6.tar` & `qtaf-5.6.7.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:45:49.287389 qtaf-5.6.6/
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-07-17 03:45:38.000000 qtaf-5.6.6/LICENSE.TXT
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-17 03:45:38.000000 qtaf-5.6.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-07-17 03:45:49.287389 qtaf-5.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-07-17 03:45:38.000000 qtaf-5.6.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 03:45:38.000000 qtaf-5.6.6/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:45:49.279389 qtaf-5.6.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-17 03:45:38.000000 qtaf-5.6.6/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-17 03:45:38.000000 qtaf-5.6.6/qta-manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:45:49.279389 qtaf-5.6.6/qta_statics/
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-17 03:45:38.000000 qtaf-5.6.6/qta_statics/TestReport.xsl
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-17 03:45:38.000000 qtaf-5.6.6/qta_statics/TestResult.xsl
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 03:45:38.000000 qtaf-5.6.6/qta_statics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1968182 2023-07-17 03:45:38.000000 qtaf-5.6.6/qta_statics/qta-report.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:45:49.283389 qtaf-5.6.6/qtaf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-07-17 03:45:49.000000 qtaf-5.6.6/qtaf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-17 03:45:49.000000 qtaf-5.6.6/qtaf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 03:45:49.000000 qtaf-5.6.6/qtaf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-17 03:45:49.000000 qtaf-5.6.6/qtaf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 03:45:49.000000 qtaf-5.6.6/qtaf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-17 03:45:49.000000 qtaf-5.6.6/qtaf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-17 03:45:38.000000 qtaf-5.6.6/qtaf_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-17 03:45:38.000000 qtaf-5.6.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 03:45:49.287389 qtaf-5.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-17 03:45:38.000000 qtaf-5.6.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:45:49.283389 qtaf-5.6.6/testbase/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-17 03:45:38.000000 qtaf-5.6.6/testbase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27311 2023-07-17 03:45:38.000000 qtaf-5.6.6/testbase/assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)    12218 2023-07-17 03:45:38.000000 qtaf-5.6.6/testbase/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-17 03:45:38.000000 qtaf-5.6.6/testbase/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-07-17 03:45:38.000000 qtaf-5.6.6/testbase/datadrive.py
--rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-07-17 03:45:38.000000 qtaf-5.6.6/testbase/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-07-17 03:45:38.000000 qtaf-5.6.6/testbase/exlib.py
--rw-r--r--   0 runner    (1001) docker     (123)    15408 2023-07-17 03:45:38.000000 qtaf-5.6.6/testbase/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-17 03:45:38.000000 qtaf-5.6.6/testbase/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    34147 2023-07-17 03:45:38.000000 qtaf-5.6.6/testbase/management.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-17 03:45:38.000000 qtaf-5.6.6/testbase/plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-07-17 03:45:38.000000 qtaf-5.6.6/testbase/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    35792 2023-07-17 03:45:38.000000 qtaf-5.6.6/testbase/report.py
--rw-r--r--   0 runner    (1001) docker     (123)    24595 2023-07-17 03:45:38.000000 qtaf-5.6.6/testbase/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-17 03:45:38.000000 qtaf-5.6.6/testbase/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)    44877 2023-07-17 03:45:38.000000 qtaf-5.6.6/testbase/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-17 03:45:38.000000 qtaf-5.6.6/testbase/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-07-17 03:45:38.000000 qtaf-5.6.6/testbase/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    45863 2023-07-17 03:45:38.000000 qtaf-5.6.6/testbase/testcase.py
--rw-r--r--   0 runner    (1001) docker     (123)    29712 2023-07-17 03:45:38.000000 qtaf-5.6.6/testbase/testresult.py
--rw-r--r--   0 runner    (1001) docker     (123)    16556 2023-07-17 03:45:38.000000 qtaf-5.6.6/testbase/testsuite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-17 03:45:38.000000 qtaf-5.6.6/testbase/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    26680 2023-07-17 03:45:38.000000 qtaf-5.6.6/testbase/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-17 03:45:49.000000 qtaf-5.6.6/testbase/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:45:49.287389 qtaf-5.6.6/tuia/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-17 03:45:38.000000 qtaf-5.6.6/tuia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-17 03:45:38.000000 qtaf-5.6.6/tuia/_tif.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-17 03:45:38.000000 qtaf-5.6.6/tuia/accessible.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-17 03:45:38.000000 qtaf-5.6.6/tuia/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-17 03:45:38.000000 qtaf-5.6.6/tuia/control.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-17 03:45:38.000000 qtaf-5.6.6/tuia/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-17 03:45:38.000000 qtaf-5.6.6/tuia/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-17 03:45:38.000000 qtaf-5.6.6/tuia/filedialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-17 03:45:38.000000 qtaf-5.6.6/tuia/gfcontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-17 03:45:38.000000 qtaf-5.6.6/tuia/keyboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-17 03:45:38.000000 qtaf-5.6.6/tuia/mouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-17 03:45:38.000000 qtaf-5.6.6/tuia/qpath.py
--rw-r--r--   0 runner    (1001) docker     (123)    16430 2023-07-17 03:45:38.000000 qtaf-5.6.6/tuia/qpathparser.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-17 03:45:38.000000 qtaf-5.6.6/tuia/remoteprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-17 03:45:38.000000 qtaf-5.6.6/tuia/testcase.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-17 03:45:38.000000 qtaf-5.6.6/tuia/uiacontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-17 03:45:38.000000 qtaf-5.6.6/tuia/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-17 03:45:38.000000 qtaf-5.6.6/tuia/webcontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-17 03:45:38.000000 qtaf-5.6.6/tuia/wincontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-17 03:45:38.000000 qtaf-5.6.6/tuia/wintypes.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-17 03:45:48.000000 qtaf-5.6.6/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:56:17.767449 qtaf-5.6.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-07-24 03:56:06.000000 qtaf-5.6.7/LICENSE.TXT
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-24 03:56:06.000000 qtaf-5.6.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-07-24 03:56:17.767449 qtaf-5.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-07-24 03:56:06.000000 qtaf-5.6.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-24 03:56:06.000000 qtaf-5.6.7/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:56:17.759449 qtaf-5.6.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-24 03:56:06.000000 qtaf-5.6.7/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-24 03:56:06.000000 qtaf-5.6.7/qta-manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:56:17.759449 qtaf-5.6.7/qta_statics/
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-24 03:56:06.000000 qtaf-5.6.7/qta_statics/TestReport.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-24 03:56:06.000000 qtaf-5.6.7/qta_statics/TestResult.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 03:56:06.000000 qtaf-5.6.7/qta_statics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1968182 2023-07-24 03:56:06.000000 qtaf-5.6.7/qta_statics/qta-report.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:56:17.763449 qtaf-5.6.7/qtaf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-07-24 03:56:17.000000 qtaf-5.6.7/qtaf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-24 03:56:17.000000 qtaf-5.6.7/qtaf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 03:56:17.000000 qtaf-5.6.7/qtaf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-24 03:56:17.000000 qtaf-5.6.7/qtaf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 03:56:17.000000 qtaf-5.6.7/qtaf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-24 03:56:17.000000 qtaf-5.6.7/qtaf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-24 03:56:06.000000 qtaf-5.6.7/qtaf_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-24 03:56:06.000000 qtaf-5.6.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 03:56:17.767449 qtaf-5.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-24 03:56:06.000000 qtaf-5.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:56:17.767449 qtaf-5.6.7/testbase/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27311 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12218 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/datadrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/exlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15550 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34147 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35792 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24595 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44877 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45863 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29712 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/testresult.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16556 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/testsuite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26680 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-24 03:56:17.000000 qtaf-5.6.7/testbase/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:56:17.767449 qtaf-5.6.7/tuia/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-24 03:56:06.000000 qtaf-5.6.7/tuia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-24 03:56:06.000000 qtaf-5.6.7/tuia/_tif.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-24 03:56:06.000000 qtaf-5.6.7/tuia/accessible.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-24 03:56:06.000000 qtaf-5.6.7/tuia/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-24 03:56:06.000000 qtaf-5.6.7/tuia/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-24 03:56:06.000000 qtaf-5.6.7/tuia/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-24 03:56:06.000000 qtaf-5.6.7/tuia/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-24 03:56:06.000000 qtaf-5.6.7/tuia/filedialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-24 03:56:06.000000 qtaf-5.6.7/tuia/gfcontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-24 03:56:06.000000 qtaf-5.6.7/tuia/keyboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-24 03:56:06.000000 qtaf-5.6.7/tuia/mouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-24 03:56:06.000000 qtaf-5.6.7/tuia/qpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16430 2023-07-24 03:56:06.000000 qtaf-5.6.7/tuia/qpathparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-24 03:56:06.000000 qtaf-5.6.7/tuia/remoteprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-24 03:56:06.000000 qtaf-5.6.7/tuia/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-24 03:56:06.000000 qtaf-5.6.7/tuia/uiacontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-24 03:56:06.000000 qtaf-5.6.7/tuia/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-24 03:56:06.000000 qtaf-5.6.7/tuia/webcontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-24 03:56:06.000000 qtaf-5.6.7/tuia/wincontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-24 03:56:06.000000 qtaf-5.6.7/tuia/wintypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 03:56:16.000000 qtaf-5.6.7/version.txt
```

### Comparing `qtaf-5.6.6/LICENSE.TXT` & `qtaf-5.6.7/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/PKG-INFO` & `qtaf-5.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtaf
-Version: 5.6.6
+Version: 5.6.7
 Summary: Basic test automation framework for QTA
 Home-page: https://github.com/Tencent/QTAF
 Author: Tencent
 License: Copyright(c)2010-2018 Tencent All Rights Reserved. 
 Project-URL: TestBase Documentation, https://qta-testbase.readthedocs.io/zh/latest/
 Project-URL: TUIA Documentation, https://qta-tuia.readthedocs.io/zh/latest/
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `qtaf-5.6.6/README.md` & `qtaf-5.6.7/README.md`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/__main__.py` & `qtaf-5.6.7/__main__.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/qta-manage.py` & `qtaf-5.6.7/qta-manage.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/qta_statics/TestReport.xsl` & `qtaf-5.6.7/qta_statics/TestReport.xsl`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/qta_statics/TestResult.xsl` & `qtaf-5.6.7/qta_statics/TestResult.xsl`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/qta_statics/qta-report.html` & `qtaf-5.6.7/qta_statics/qta-report.html`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/qtaf.egg-info/PKG-INFO` & `qtaf-5.6.7/qtaf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtaf
-Version: 5.6.6
+Version: 5.6.7
 Summary: Basic test automation framework for QTA
 Home-page: https://github.com/Tencent/QTAF
 Author: Tencent
 License: Copyright(c)2010-2018 Tencent All Rights Reserved. 
 Project-URL: TestBase Documentation, https://qta-testbase.readthedocs.io/zh/latest/
 Project-URL: TUIA Documentation, https://qta-tuia.readthedocs.io/zh/latest/
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `qtaf-5.6.6/qtaf.egg-info/SOURCES.txt` & `qtaf-5.6.7/qtaf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/qtaf_settings.py` & `qtaf-5.6.7/qtaf_settings.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/setup.py` & `qtaf-5.6.7/setup.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/testbase/__init__.py` & `qtaf-5.6.7/testbase/__init__.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/testbase/assertion.py` & `qtaf-5.6.7/testbase/assertion.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/testbase/conf.py` & `qtaf-5.6.7/testbase/conf.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/testbase/context.py` & `qtaf-5.6.7/testbase/context.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/testbase/datadrive.py` & `qtaf-5.6.7/testbase/datadrive.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/testbase/dist.py` & `qtaf-5.6.7/testbase/dist.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/testbase/exlib.py` & `qtaf-5.6.7/testbase/exlib.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/testbase/loader.py` & `qtaf-5.6.7/testbase/loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -112,15 +112,17 @@
                         obj, data_key, exclude_data_keys, parameters
                     )
                 elif issubclass(obj, TestSuite):
                     if not self._filter_testcase(obj):
                         tests = self._load_from_testsuite(
                             obj, data_key, exclude_data_keys, parameters
                         )
-                        testcases.append(obj(tests))  # append testsuite to testcase list
+                        testcases.append(
+                            obj(tests)
+                        )  # append testsuite to testcase list
 
         # 过滤掉重复的用例
         testcase_dict = OrderedDict()
         for testcase in testcases:
             testcase_dict[testcase.test_name] = testcase
 
         return list(testcase_dict.values())
@@ -130,59 +132,63 @@
 
         :param name: 用例或用例集名称
         :type name: string
         :returns - Type/ModuleType
         """
         parts = testname.split(".")
         module = None
-        parts_imp = parts[:]
-        while parts_imp:
+        i = 0
+        while i < len(parts):
+            i += 1
+            modulename = ".".join(parts[:i])
             try:
-                modulename = ".".join(parts_imp)
-                __import__(modulename)  # __import__得到的是最外层模块的object
-                module = sys.modules[modulename]
-                break
-            except ImportError:
-                del parts_imp[-1]
-            except Exception:  # pylint: disable=broad-except
-                del parts_imp[-1]
-                break
+                module = __import__(modulename)  # __import__得到的是最外层模块的object
+            except Exception as ex:  # pylint: disable=broad-except
+                self._module_errs[modulename] = traceback.format_exc()
+                return
+            else:
+                for name in parts[1:i]:
+                    module = getattr(module, name)
+                if not hasattr(module, "__path__"):
+                    # file module
+                    break
 
         obj = module
-
-        if parts_imp == parts:  # 为一个包或模块
+        if i == len(parts):  # 为一个包或模块
             return obj
-        
-        elif parts_imp == parts[0:-1] and parts[-1] == 'SeqTestSuiteTest':  # 为顺序测试套
+        elif i < len(parts) - 1:
+            self._module_errs[testname] = "ImportError: No module named %s" % ".".join(
+                parts[: i + 1]
+            )
+            return
+
+        classname = parts[-1]
+        if classname == "SeqTestSuiteTest":  # 为顺序测试套
             return obj
 
-        elif parts_imp == parts[0:-1] and hasattr(module, parts[-1]):  # 为一个类
+        elif hasattr(module, classname):  # 为一个类
             try:
-                testclass = getattr(module, parts[-1])
+                testclass = getattr(module, classname)
                 if not self._is_testcase_class(
                     testclass
                 ) and not self._is_testsuite_class(testclass):
                     raise TypeError("%s不是一个有效的测试用例(套)" % testname)
             except Exception:  # pylint: disable=broad-except
                 self._module_errs[testname] = traceback.format_exc()
                 return
             else:
                 return testclass
 
         else:  # 触发异常
-            if parts_imp:
-                modulename = ".".join(parts_imp)
-                modulename += "."
-            else:
-                modulename = ""
-            modulename += parts[len(parts_imp)]
-            try:
-                __import__(modulename)
-            except Exception:  # pylint: disable=broad-except
-                self._module_errs[modulename] = traceback.format_exc()
+            self._module_errs[
+                testname
+            ] = "ImportError: No testcase named %s in module %s" % (
+                classname,
+                module.__name__,
+            )
 
     def _is_testcase_class(self, obj):
         """是否为测试用例类
 
         :returns bool - 是否为用例类
         """
         return (
```

### Comparing `qtaf-5.6.6/testbase/logger.py` & `qtaf-5.6.7/testbase/logger.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/testbase/management.py` & `qtaf-5.6.7/testbase/management.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/testbase/plan.py` & `qtaf-5.6.7/testbase/plan.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/testbase/project.py` & `qtaf-5.6.7/testbase/project.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/testbase/report.py` & `qtaf-5.6.7/testbase/report.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/testbase/resource.py` & `qtaf-5.6.7/testbase/resource.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/testbase/retry.py` & `qtaf-5.6.7/testbase/retry.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/testbase/runner.py` & `qtaf-5.6.7/testbase/runner.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/testbase/serialization.py` & `qtaf-5.6.7/testbase/serialization.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/testbase/test.py` & `qtaf-5.6.7/testbase/test.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/testbase/testcase.py` & `qtaf-5.6.7/testbase/testcase.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/testbase/testresult.py` & `qtaf-5.6.7/testbase/testresult.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/testbase/testsuite.py` & `qtaf-5.6.7/testbase/testsuite.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/testbase/types.py` & `qtaf-5.6.7/testbase/types.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/testbase/util.py` & `qtaf-5.6.7/testbase/util.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/tuia/__init__.py` & `qtaf-5.6.7/tuia/__init__.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/tuia/_tif.py` & `qtaf-5.6.7/tuia/_tif.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/tuia/accessible.py` & `qtaf-5.6.7/tuia/accessible.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/tuia/app.py` & `qtaf-5.6.7/tuia/app.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/tuia/control.py` & `qtaf-5.6.7/tuia/control.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/tuia/env.py` & `qtaf-5.6.7/tuia/env.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/tuia/exceptions.py` & `qtaf-5.6.7/tuia/exceptions.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/tuia/filedialog.py` & `qtaf-5.6.7/tuia/filedialog.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/tuia/gfcontrols.py` & `qtaf-5.6.7/tuia/gfcontrols.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/tuia/keyboard.py` & `qtaf-5.6.7/tuia/keyboard.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/tuia/mouse.py` & `qtaf-5.6.7/tuia/mouse.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/tuia/qpath.py` & `qtaf-5.6.7/tuia/qpath.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/tuia/qpathparser.py` & `qtaf-5.6.7/tuia/qpathparser.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/tuia/remoteprocessing.py` & `qtaf-5.6.7/tuia/remoteprocessing.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/tuia/testcase.py` & `qtaf-5.6.7/tuia/testcase.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/tuia/uiacontrols.py` & `qtaf-5.6.7/tuia/uiacontrols.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/tuia/util.py` & `qtaf-5.6.7/tuia/util.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/tuia/webcontrols.py` & `qtaf-5.6.7/tuia/webcontrols.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/tuia/wincontrols.py` & `qtaf-5.6.7/tuia/wincontrols.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.6/tuia/wintypes.py` & `qtaf-5.6.7/tuia/wintypes.py`

 * *Files identical despite different names*

