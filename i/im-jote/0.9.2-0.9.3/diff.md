# Comparing `tmp/im-jote-0.9.2.tar.gz` & `tmp/im-jote-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "im-jote-0.9.2.tar", last modified: Wed Mar 22 12:31:43 2023, max compression
+gzip compressed data, was "im-jote-0.9.3.tar", last modified: Thu Jul 20 14:44:30 2023, max compression
```

## Comparing `im-jote-0.9.2.tar` & `im-jote-0.9.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 12:31:43.451476 im-jote-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-03-22 12:31:24.000000 im-jote-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-22 12:31:24.000000 im-jote-0.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13142 2023-03-22 12:31:43.451476 im-jote-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12486 2023-03-22 12:31:24.000000 im-jote-0.9.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-22 12:31:24.000000 im-jote-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 12:31:43.451476 im-jote-0.9.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1629 2023-03-22 12:31:24.000000 im-jote-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 12:31:43.443476 im-jote-0.9.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 12:31:43.447476 im-jote-0.9.2/src/im_jote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13142 2023-03-22 12:31:43.000000 im-jote-0.9.2/src/im_jote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-03-22 12:31:43.000000 im-jote-0.9.2/src/im_jote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 12:31:43.000000 im-jote-0.9.2/src/im_jote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-22 12:31:43.000000 im-jote-0.9.2/src/im_jote.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 12:31:43.000000 im-jote-0.9.2/src/im_jote.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-22 12:31:43.000000 im-jote-0.9.2/src/im_jote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-22 12:31:43.000000 im-jote-0.9.2/src/im_jote.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 12:31:43.451476 im-jote-0.9.2/src/jote/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-22 12:31:34.000000 im-jote-0.9.2/src/jote/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 12:31:24.000000 im-jote-0.9.2/src/jote/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      378 2023-03-22 12:31:24.000000 im-jote-0.9.2/src/jote/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12679 2023-03-22 12:31:24.000000 im-jote-0.9.2/src/jote/compose.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    55188 2023-03-22 12:31:24.000000 im-jote-0.9.2/src/jote/jote.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-03-22 12:31:24.000000 im-jote-0.9.2/src/jote/jote.yamllint
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:44:30.245813 im-jote-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-20 14:44:19.000000 im-jote-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-20 14:44:19.000000 im-jote-0.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13693 2023-07-20 14:44:30.245813 im-jote-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12986 2023-07-20 14:44:19.000000 im-jote-0.9.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-20 14:44:19.000000 im-jote-0.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 14:44:30.245813 im-jote-0.9.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1679 2023-07-20 14:44:19.000000 im-jote-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:44:30.241813 im-jote-0.9.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:44:30.245813 im-jote-0.9.3/src/im_jote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13693 2023-07-20 14:44:30.000000 im-jote-0.9.3/src/im_jote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-20 14:44:30.000000 im-jote-0.9.3/src/im_jote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:44:30.000000 im-jote-0.9.3/src/im_jote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-20 14:44:30.000000 im-jote-0.9.3/src/im_jote.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:44:30.000000 im-jote-0.9.3/src/im_jote.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-20 14:44:30.000000 im-jote-0.9.3/src/im_jote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-20 14:44:30.000000 im-jote-0.9.3/src/im_jote.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:44:30.245813 im-jote-0.9.3/src/jote/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-20 14:44:23.000000 im-jote-0.9.3/src/jote/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:44:19.000000 im-jote-0.9.3/src/jote/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      378 2023-07-20 14:44:19.000000 im-jote-0.9.3/src/jote/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12679 2023-07-20 14:44:19.000000 im-jote-0.9.3/src/jote/compose.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    55188 2023-07-20 14:44:19.000000 im-jote-0.9.3/src/jote/jote.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-20 14:44:19.000000 im-jote-0.9.3/src/jote/jote.yamllint
```

### Comparing `im-jote-0.9.2/LICENSE` & `im-jote-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `im-jote-0.9.2/PKG-INFO` & `im-jote-0.9.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,42 @@
 Metadata-Version: 2.1
 Name: im-jote
-Version: 0.9.2
+Version: 0.9.3
 Summary: The IM Data Manager Job Tester (jote)
 Home-page: https://github.com/informaticsmatters/squonk2-data-manager-job-tester
 Author: Alan Christie
 Author-email: achristie@informaticsmatters.com
 License: MIT
 Keywords: configuration
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Operating System :: POSIX :: Linux
 License-File: LICENSE
 
 Informatics Matters Job Tester ("jote")
 =======================================
 
 .. image:: https://badge.fury.io/py/im-jote.svg
    :target: https://badge.fury.io/py/im-jote
    :alt: PyPI package (latest)
 
+.. image:: https://github.com/InformaticsMatters/squonk2-data-manager-job-tester/actions/workflows/build.yaml/badge.svg
+   :target: https://github.com/InformaticsMatters/squonk2-data-manager-job-tester/actions/workflows/build.yaml
+   :alt: Build
+
+.. image:: https://github.com/InformaticsMatters/squonk2-data-manager-job-tester/actions/workflows/publish.yaml/badge.svg
+   :target: https://github.com/InformaticsMatters/squonk2-data-manager-job-tester/actions/workflows/publish.yaml
+   :alt: Publish
+
 The **Squonk2 Job Tester** (``jote``) is a Python utility used to run *unit tests*
 that are defined in Data Manager *job implementation repositories* against
 the job's container image, images that are typically built from the same
 repository.
 
 ``jote`` is designed to run job implementations in a file-system
 environment that replicates what they find when they're run by the Data Manager.
```

### Comparing `im-jote-0.9.2/README.rst` & `im-jote-0.9.3/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 Informatics Matters Job Tester ("jote")
 =======================================
 
 .. image:: https://badge.fury.io/py/im-jote.svg
    :target: https://badge.fury.io/py/im-jote
    :alt: PyPI package (latest)
 
+.. image:: https://github.com/InformaticsMatters/squonk2-data-manager-job-tester/actions/workflows/build.yaml/badge.svg
+   :target: https://github.com/InformaticsMatters/squonk2-data-manager-job-tester/actions/workflows/build.yaml
+   :alt: Build
+
+.. image:: https://github.com/InformaticsMatters/squonk2-data-manager-job-tester/actions/workflows/publish.yaml/badge.svg
+   :target: https://github.com/InformaticsMatters/squonk2-data-manager-job-tester/actions/workflows/publish.yaml
+   :alt: Publish
+
 The **Squonk2 Job Tester** (``jote``) is a Python utility used to run *unit tests*
 that are defined in Data Manager *job implementation repositories* against
 the job's container image, images that are typically built from the same
 repository.
 
 ``jote`` is designed to run job implementations in a file-system
 environment that replicates what they find when they're run by the Data Manager.
```

### Comparing `im-jote-0.9.2/setup.py` & `im-jote-0.9.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     # https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: System :: Installation/Setup",
         "Operating System :: POSIX :: Linux",
     ],
     install_requires=requirements,
     entry_points={
         "console_scripts": [
             "jote = jote.jote:main",
```

### Comparing `im-jote-0.9.2/src/im_jote.egg-info/PKG-INFO` & `im-jote-0.9.3/src/im_jote.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,42 @@
 Metadata-Version: 2.1
 Name: im-jote
-Version: 0.9.2
+Version: 0.9.3
 Summary: The IM Data Manager Job Tester (jote)
 Home-page: https://github.com/informaticsmatters/squonk2-data-manager-job-tester
 Author: Alan Christie
 Author-email: achristie@informaticsmatters.com
 License: MIT
 Keywords: configuration
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Operating System :: POSIX :: Linux
 License-File: LICENSE
 
 Informatics Matters Job Tester ("jote")
 =======================================
 
 .. image:: https://badge.fury.io/py/im-jote.svg
    :target: https://badge.fury.io/py/im-jote
    :alt: PyPI package (latest)
 
+.. image:: https://github.com/InformaticsMatters/squonk2-data-manager-job-tester/actions/workflows/build.yaml/badge.svg
+   :target: https://github.com/InformaticsMatters/squonk2-data-manager-job-tester/actions/workflows/build.yaml
+   :alt: Build
+
+.. image:: https://github.com/InformaticsMatters/squonk2-data-manager-job-tester/actions/workflows/publish.yaml/badge.svg
+   :target: https://github.com/InformaticsMatters/squonk2-data-manager-job-tester/actions/workflows/publish.yaml
+   :alt: Publish
+
 The **Squonk2 Job Tester** (``jote``) is a Python utility used to run *unit tests*
 that are defined in Data Manager *job implementation repositories* against
 the job's container image, images that are typically built from the same
 repository.
 
 ``jote`` is designed to run job implementations in a file-system
 environment that replicates what they find when they're run by the Data Manager.
```

### Comparing `im-jote-0.9.2/src/jote/compose.py` & `im-jote-0.9.3/src/jote/compose.py`

 * *Files identical despite different names*

### Comparing `im-jote-0.9.2/src/jote/jote.py` & `im-jote-0.9.3/src/jote/jote.py`

 * *Files identical despite different names*

### Comparing `im-jote-0.9.2/src/jote/jote.yamllint` & `im-jote-0.9.3/src/jote/jote.yamllint`

 * *Files identical despite different names*

