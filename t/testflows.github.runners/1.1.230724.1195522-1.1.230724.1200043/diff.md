# Comparing `tmp/testflows.github.runners-1.1.230724.1195522.tar.gz` & `tmp/testflows.github.runners-1.1.230724.1200043.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.1.230724.1195522.tar", last modified: Mon Jul 24 19:55:23 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.1.230724.1200043.tar", last modified: Mon Jul 24 20:00:44 2023, max compression
```

## Comparing `testflows.github.runners-1.1.230724.1195522.tar` & `testflows.github.runners-1.1.230724.1200043.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 19:55:22.994824 testflows.github.runners-1.1.230724.1195522/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.1.230724.1195522/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    15935 2023-07-24 19:55:22.994824 testflows.github.runners-1.1.230724.1195522/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    15343 2023-07-24 19:55:21.000000 testflows.github.runners-1.1.230724.1195522/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-24 19:55:22.994824 testflows.github.runners-1.1.230724.1195522/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1906 2023-07-24 19:55:22.000000 testflows.github.runners-1.1.230724.1195522/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 19:55:22.990824 testflows.github.runners-1.1.230724.1195522/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 19:55:22.990824 testflows.github.runners-1.1.230724.1195522/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 19:55:22.994824 testflows.github.runners-1.1.230724.1195522/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-24 19:55:22.000000 testflows.github.runners-1.1.230724.1195522/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1145 2023-07-24 14:31:21.000000 testflows.github.runners-1.1.230724.1195522/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     1173 2023-07-24 19:41:30.000000 testflows.github.runners-1.1.230724.1195522/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 19:55:22.994824 testflows.github.runners-1.1.230724.1195522/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    12515 2023-07-24 19:33:30.000000 testflows.github.runners-1.1.230724.1195522/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)     1266 2023-07-24 15:25:53.000000 testflows.github.runners-1.1.230724.1195522/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)     8365 2023-07-24 14:06:05.000000 testflows.github.runners-1.1.230724.1195522/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)     8771 2023-07-24 15:28:13.000000 testflows.github.runners-1.1.230724.1195522/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 19:55:22.994824 testflows.github.runners-1.1.230724.1195522/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1008 2023-07-24 12:06:14.000000 testflows.github.runners-1.1.230724.1195522/testflows/github/runners/scripts/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      218 2023-07-24 01:29:18.000000 testflows.github.runners-1.1.230724.1195522/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-24 01:28:32.000000 testflows.github.runners-1.1.230724.1195522/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      714 2023-07-24 01:27:59.000000 testflows.github.runners-1.1.230724.1195522/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     4673 2023-07-24 19:32:08.000000 testflows.github.runners-1.1.230724.1195522/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1151 2023-07-24 12:06:14.000000 testflows.github.runners-1.1.230724.1195522/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 19:55:22.990824 testflows.github.runners-1.1.230724.1195522/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    15935 2023-07-24 19:55:22.000000 testflows.github.runners-1.1.230724.1195522/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      830 2023-07-24 19:55:22.000000 testflows.github.runners-1.1.230724.1195522/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 19:55:22.000000 testflows.github.runners-1.1.230724.1195522/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.1.230724.1195522/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-24 19:55:22.000000 testflows.github.runners-1.1.230724.1195522/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-24 19:55:22.000000 testflows.github.runners-1.1.230724.1195522/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 20:00:44.189520 testflows.github.runners-1.1.230724.1200043/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.1.230724.1200043/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    15815 2023-07-24 20:00:44.185520 testflows.github.runners-1.1.230724.1200043/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    15223 2023-07-24 20:00:27.000000 testflows.github.runners-1.1.230724.1200043/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-24 20:00:44.189520 testflows.github.runners-1.1.230724.1200043/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1906 2023-07-24 20:00:43.000000 testflows.github.runners-1.1.230724.1200043/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 20:00:44.185520 testflows.github.runners-1.1.230724.1200043/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 20:00:44.185520 testflows.github.runners-1.1.230724.1200043/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 20:00:44.185520 testflows.github.runners-1.1.230724.1200043/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-24 20:00:43.000000 testflows.github.runners-1.1.230724.1200043/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1145 2023-07-24 14:31:21.000000 testflows.github.runners-1.1.230724.1200043/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1173 2023-07-24 19:41:30.000000 testflows.github.runners-1.1.230724.1200043/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 20:00:44.185520 testflows.github.runners-1.1.230724.1200043/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    12515 2023-07-24 19:33:30.000000 testflows.github.runners-1.1.230724.1200043/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)     1266 2023-07-24 15:25:53.000000 testflows.github.runners-1.1.230724.1200043/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8365 2023-07-24 14:06:05.000000 testflows.github.runners-1.1.230724.1200043/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8771 2023-07-24 15:28:13.000000 testflows.github.runners-1.1.230724.1200043/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 20:00:44.185520 testflows.github.runners-1.1.230724.1200043/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1008 2023-07-24 12:06:14.000000 testflows.github.runners-1.1.230724.1200043/testflows/github/runners/scripts/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      218 2023-07-24 01:29:18.000000 testflows.github.runners-1.1.230724.1200043/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-24 01:28:32.000000 testflows.github.runners-1.1.230724.1200043/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      714 2023-07-24 01:27:59.000000 testflows.github.runners-1.1.230724.1200043/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     4673 2023-07-24 19:32:08.000000 testflows.github.runners-1.1.230724.1200043/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1151 2023-07-24 12:06:14.000000 testflows.github.runners-1.1.230724.1200043/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 20:00:44.185520 testflows.github.runners-1.1.230724.1200043/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    15815 2023-07-24 20:00:44.000000 testflows.github.runners-1.1.230724.1200043/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      830 2023-07-24 20:00:44.000000 testflows.github.runners-1.1.230724.1200043/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 20:00:44.000000 testflows.github.runners-1.1.230724.1200043/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.1.230724.1200043/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-24 20:00:44.000000 testflows.github.runners-1.1.230724.1200043/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-24 20:00:44.000000 testflows.github.runners-1.1.230724.1200043/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.1.230724.1195522/LICENSE` & `testflows.github.runners-1.1.230724.1200043/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230724.1195522/PKG-INFO` & `testflows.github.runners-1.1.230724.1200043/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.1.230724.1195522
+Version: 1.1.230724.1200043
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -20,18 +20,14 @@
    :target: https://testflows.com
    :alt: test bug
 
 ======================================================
 Autoscaling GitHub Actions Runners Using Hetzner Cloud
 ======================================================
 
-.. image:: https://raw.githubusercontent.com/testflows/TestFlows-ArtWork/master/images/test-machine.png
-   :width: 30%
-   :alt: test machine
-
 The **github-runners** service program starts and monitors queued up jobs for GitHub Actions workflows.
 When a new job is queued up, it creates a new Hetzner Cloud server instance
 that provides an ephemeral GitHub Actions runner. Each server instance is automatically
 powered off when job completes and then powered off servers are
 automatically deleted. Both **x64** and **arm64** runners are supported.
 
 :❗Warning:
@@ -216,15 +212,15 @@
    There is no guarantee that a given runner will pick the the job with the exact **run_id** that caused it to be created.
    This is expected and because for each **queued** job a unique runner will be created the number of runners will be
    equal the number of jobs and therefore under normal conditions all jobs will executed as expected.
 
 Maximum Number of Runners
 =========================
 
-By default, the maximum number of runners and therefore server instances is not set and therefore is unlimited.
+By default, the maximum number of runners and therefore the maximum number if server instances is not set and therefore is unlimited.
 You can set the maximum number of runners using the **--max-runners** option.
 
 .. code-blocks::bash
 
    github-runners --max-runners 10
```

### Comparing `testflows.github.runners-1.1.230724.1195522/README.rst` & `testflows.github.runners-1.1.230724.1200043/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,14 @@
    :target: https://testflows.com
    :alt: test bug
 
 ======================================================
 Autoscaling GitHub Actions Runners Using Hetzner Cloud
 ======================================================
 
-.. image:: https://raw.githubusercontent.com/testflows/TestFlows-ArtWork/master/images/test-machine.png
-   :width: 30%
-   :alt: test machine
-
 The **github-runners** service program starts and monitors queued up jobs for GitHub Actions workflows.
 When a new job is queued up, it creates a new Hetzner Cloud server instance
 that provides an ephemeral GitHub Actions runner. Each server instance is automatically
 powered off when job completes and then powered off servers are
 automatically deleted. Both **x64** and **arm64** runners are supported.
 
 :❗Warning:
@@ -199,15 +195,15 @@
    There is no guarantee that a given runner will pick the the job with the exact **run_id** that caused it to be created.
    This is expected and because for each **queued** job a unique runner will be created the number of runners will be
    equal the number of jobs and therefore under normal conditions all jobs will executed as expected.
 
 Maximum Number of Runners
 =========================
 
-By default, the maximum number of runners and therefore server instances is not set and therefore is unlimited.
+By default, the maximum number of runners and therefore the maximum number if server instances is not set and therefore is unlimited.
 You can set the maximum number of runners using the **--max-runners** option.
 
 .. code-blocks::bash
 
    github-runners --max-runners 10
```

### Comparing `testflows.github.runners-1.1.230724.1195522/setup.py` & `testflows.github.runners-1.1.230724.1200043/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.1.230724.1195522",
+    version="1.1.230724.1200043",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.1.230724.1195522/testflows/github/runners/__init__.py` & `testflows.github.runners-1.1.230724.1200043/testflows/github/runners/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 __author__ = "Vitaliy Zakaznikov"
-__version__ = "1.1.230724.1195522"
+__version__ = "1.1.230724.1200043"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.1.230724.1195522/testflows/github/runners/actions.py` & `testflows.github.runners-1.1.230724.1200043/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230724.1195522/testflows/github/runners/args.py` & `testflows.github.runners-1.1.230724.1200043/testflows/github/runners/args.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230724.1195522/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.1.230724.1200043/testflows/github/runners/bin/github-runners`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230724.1195522/testflows/github/runners/request.py` & `testflows.github.runners-1.1.230724.1200043/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230724.1195522/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.1.230724.1200043/testflows/github/runners/scale_down.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230724.1195522/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.1.230724.1200043/testflows/github/runners/scale_up.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230724.1195522/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.1.230724.1200043/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230724.1195522/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.1.230724.1200043/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230724.1195522/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.1.230724.1200043/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230724.1195522/testflows/github/runners/service.py` & `testflows.github.runners-1.1.230724.1200043/testflows/github/runners/service.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230724.1195522/testflows/github/runners/shell.py` & `testflows.github.runners-1.1.230724.1200043/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230724.1195522/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.1.230724.1200043/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.1.230724.1195522
+Version: 1.1.230724.1200043
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -20,18 +20,14 @@
    :target: https://testflows.com
    :alt: test bug
 
 ======================================================
 Autoscaling GitHub Actions Runners Using Hetzner Cloud
 ======================================================
 
-.. image:: https://raw.githubusercontent.com/testflows/TestFlows-ArtWork/master/images/test-machine.png
-   :width: 30%
-   :alt: test machine
-
 The **github-runners** service program starts and monitors queued up jobs for GitHub Actions workflows.
 When a new job is queued up, it creates a new Hetzner Cloud server instance
 that provides an ephemeral GitHub Actions runner. Each server instance is automatically
 powered off when job completes and then powered off servers are
 automatically deleted. Both **x64** and **arm64** runners are supported.
 
 :❗Warning:
@@ -216,15 +212,15 @@
    There is no guarantee that a given runner will pick the the job with the exact **run_id** that caused it to be created.
    This is expected and because for each **queued** job a unique runner will be created the number of runners will be
    equal the number of jobs and therefore under normal conditions all jobs will executed as expected.
 
 Maximum Number of Runners
 =========================
 
-By default, the maximum number of runners and therefore server instances is not set and therefore is unlimited.
+By default, the maximum number of runners and therefore the maximum number if server instances is not set and therefore is unlimited.
 You can set the maximum number of runners using the **--max-runners** option.
 
 .. code-blocks::bash
 
    github-runners --max-runners 10
```

### Comparing `testflows.github.runners-1.1.230724.1195522/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.1.230724.1200043/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*

