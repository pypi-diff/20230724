# Comparing `tmp/deepdog-0.7.0.tar.gz` & `tmp/deepdog-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepdog-0.7.0.tar", max compression
+gzip compressed data, was "deepdog-0.7.1.tar", max compression
```

## Comparing `deepdog-0.7.0.tar` & `deepdog-0.7.1.tar`

### file list

```diff
@@ -1,9 +1,12 @@
--rw-r--r--   0        0        0      501 2023-05-01 15:27:10.915961 deepdog-0.7.0/deepdog/__init__.py
--rw-r--r--   0        0        0     8197 2023-05-01 15:27:10.915961 deepdog-0.7.0/deepdog/bayes_run.py
--rw-r--r--   0        0        0    11705 2023-05-01 15:27:10.915961 deepdog-0.7.0/deepdog/bayes_run_simulpairs.py
--rw-r--r--   0        0        0       73 2023-05-01 15:27:10.919962 deepdog-0.7.0/deepdog/meta.py
--rw-r--r--   0        0        0     8471 2023-05-01 15:27:10.919962 deepdog-0.7.0/deepdog/real_spectrum_run.py
--rw-r--r--   0        0        0     6794 2023-05-01 15:27:10.919962 deepdog-0.7.0/deepdog/temp_aware_real_spectrum_run.py
--rw-r--r--   0        0        0      895 2023-05-01 15:27:10.919962 deepdog-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      630 2023-05-01 15:29:16.038480 deepdog-0.7.0/setup.py
--rw-r--r--   0        0        0      408 2023-05-01 15:29:16.038812 deepdog-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      605 2023-07-24 07:05:18.226134 deepdog-0.7.1/deepdog/__init__.py
+-rw-r--r--   0        0        0     8197 2023-07-24 07:05:18.226134 deepdog-0.7.1/deepdog/bayes_run.py
+-rw-r--r--   0        0        0    11705 2023-07-24 07:05:18.226134 deepdog-0.7.1/deepdog/bayes_run_simulpairs.py
+-rw-r--r--   0        0        0     6623 2023-07-24 07:05:18.226134 deepdog-0.7.1/deepdog/bayes_run_with_ss.py
+-rw-r--r--   0        0        0       73 2023-07-24 07:05:18.226134 deepdog-0.7.1/deepdog/meta.py
+-rw-r--r--   0        0        0     8471 2023-07-24 07:05:18.226134 deepdog-0.7.1/deepdog/real_spectrum_run.py
+-rw-r--r--   0        0        0      110 2023-07-24 07:05:18.226134 deepdog-0.7.1/deepdog/subset_simulation/__init__.py
+-rw-r--r--   0        0        0     8754 2023-07-24 07:05:18.230134 deepdog-0.7.1/deepdog/subset_simulation/subset_simulation_impl.py
+-rw-r--r--   0        0        0     6794 2023-07-24 07:05:18.230134 deepdog-0.7.1/deepdog/temp_aware_real_spectrum_run.py
+-rw-r--r--   0        0        0      898 2023-07-24 07:05:18.230134 deepdog-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      662 2023-07-24 07:06:20.769951 deepdog-0.7.1/setup.py
+-rw-r--r--   0        0        0      361 2023-07-24 07:06:20.770362 deepdog-0.7.1/PKG-INFO
```

### Comparing `deepdog-0.7.0/deepdog/bayes_run.py` & `deepdog-0.7.1/deepdog/bayes_run.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.7.0/deepdog/bayes_run_simulpairs.py` & `deepdog-0.7.1/deepdog/bayes_run_simulpairs.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.7.0/deepdog/real_spectrum_run.py` & `deepdog-0.7.1/deepdog/real_spectrum_run.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.7.0/deepdog/temp_aware_real_spectrum_run.py` & `deepdog-0.7.1/deepdog/temp_aware_real_spectrum_run.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.7.0/pyproject.toml` & `deepdog-0.7.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "deepdog"
-version = "0.7.0"
+version = "0.7.1"
 description = ""
 authors = ["Deepak Mallubhotla <dmallubhotla+github@gmail.com>"]
 
 [tool.poetry.dependencies]
-python = "^3.8,<3.10"
-pdme = "^0.8.6"
+python = ">=3.8.1,<3.10"
+pdme = "^0.9.1"
 numpy = "1.22.3"
 scipy = "1.10"
 
 [tool.poetry.dev-dependencies]
 pytest = ">=6"
 flake8 = "^4.0.1"
 pytest-cov = "^3.0.0"
```

### Comparing `deepdog-0.7.0/setup.py` & `deepdog-0.7.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['deepdog']
+['deepdog', 'deepdog.subset_simulation']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['numpy==1.22.3', 'pdme>=0.8.6,<0.9.0', 'scipy==1.10']
+['numpy==1.22.3', 'pdme>=0.9.1,<0.10.0', 'scipy==1.10']
 
 setup_kwargs = {
     'name': 'deepdog',
-    'version': '0.7.0',
+    'version': '0.7.1',
     'description': '',
     'long_description': None,
     'author': 'Deepak Mallubhotla',
     'author_email': 'dmallubhotla+github@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.10',
+    'python_requires': '>=3.8.1,<3.10',
 }
 
 
 setup(**setup_kwargs)
```

