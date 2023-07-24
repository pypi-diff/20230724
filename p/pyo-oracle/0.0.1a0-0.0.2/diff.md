# Comparing `tmp/pyo_oracle-0.0.1a0.tar.gz` & `tmp/pyo_oracle-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyo_oracle-0.0.1a0.tar", last modified: Mon Jun 19 06:26:21 2023, max compression
+gzip compressed data, was "pyo_oracle-0.0.2.tar", last modified: Mon Jul 24 12:26:31 2023, max compression
```

## Comparing `pyo_oracle-0.0.1a0.tar` & `pyo_oracle-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:26:21.128061 pyo_oracle-0.0.1a0/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-19 06:26:11.000000 pyo_oracle-0.0.1a0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-19 06:26:11.000000 pyo_oracle-0.0.1a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-19 06:26:21.128061 pyo_oracle-0.0.1a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-19 06:26:11.000000 pyo_oracle-0.0.1a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:26:21.128061 pyo_oracle-0.0.1a0/pyo_oracle/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-19 06:26:11.000000 pyo_oracle-0.0.1a0/pyo_oracle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-06-19 06:26:11.000000 pyo_oracle-0.0.1a0/pyo_oracle/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:26:21.128061 pyo_oracle-0.0.1a0/pyo_oracle/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 06:26:11.000000 pyo_oracle-0.0.1a0/pyo_oracle/data/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-06-19 06:26:11.000000 pyo_oracle-0.0.1a0/pyo_oracle/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-06-19 06:26:11.000000 pyo_oracle-0.0.1a0/pyo_oracle/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:26:21.128061 pyo_oracle-0.0.1a0/pyo_oracle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-19 06:26:21.000000 pyo_oracle-0.0.1a0/pyo_oracle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-19 06:26:21.000000 pyo_oracle-0.0.1a0/pyo_oracle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 06:26:21.000000 pyo_oracle-0.0.1a0/pyo_oracle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-19 06:26:21.000000 pyo_oracle-0.0.1a0/pyo_oracle.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-19 06:26:21.000000 pyo_oracle-0.0.1a0/pyo_oracle.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-19 06:26:11.000000 pyo_oracle-0.0.1a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 06:26:21.128061 pyo_oracle-0.0.1a0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:26:21.128061 pyo_oracle-0.0.1a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-19 06:26:11.000000 pyo_oracle-0.0.1a0/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:26:31.162877 pyo_oracle-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-24 12:26:17.000000 pyo_oracle-0.0.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-24 12:26:17.000000 pyo_oracle-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-24 12:26:31.162877 pyo_oracle-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-24 12:26:17.000000 pyo_oracle-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:26:31.158877 pyo_oracle-0.0.2/pyo_oracle/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-24 12:26:17.000000 pyo_oracle-0.0.2/pyo_oracle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-07-24 12:26:17.000000 pyo_oracle-0.0.2/pyo_oracle/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:26:31.158877 pyo_oracle-0.0.2/pyo_oracle/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 12:26:17.000000 pyo_oracle-0.0.2/pyo_oracle/data/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-07-24 12:26:17.000000 pyo_oracle-0.0.2/pyo_oracle/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-07-24 12:26:17.000000 pyo_oracle-0.0.2/pyo_oracle/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:26:31.158877 pyo_oracle-0.0.2/pyo_oracle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-24 12:26:31.000000 pyo_oracle-0.0.2/pyo_oracle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-24 12:26:31.000000 pyo_oracle-0.0.2/pyo_oracle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 12:26:31.000000 pyo_oracle-0.0.2/pyo_oracle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 12:26:31.000000 pyo_oracle-0.0.2/pyo_oracle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-24 12:26:31.000000 pyo_oracle-0.0.2/pyo_oracle.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-24 12:26:17.000000 pyo_oracle-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 12:26:31.162877 pyo_oracle-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:26:31.162877 pyo_oracle-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-24 12:26:17.000000 pyo_oracle-0.0.2/tests/test_main.py
```

### Comparing `pyo_oracle-0.0.1a0/LICENSE.md` & `pyo_oracle-0.0.2/LICENSE.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Bio-ORACLE consortia
+Copyright (c) 2023 Bio-ORACLE consortium
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pyo_oracle-0.0.1a0/PKG-INFO` & `pyo_oracle-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyo_oracle
-Version: 0.0.1a0
+Version: 0.0.2
 Summary: Python client for the Bio-ORACLE ERDDAP server.
 Author-email: Vini Salazar <vinicius.salazar@unimelb.edu.au>
 Project-URL: Homepage, https://github.com/bio-oracle/pyo_oracle
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -40,14 +40,14 @@
 pyo_oracle.list_local_data()
 ```
 
 ### Installation
 
 ```bash
 # With conda
-conda create -n pyo_oracle conda-forge::pyo_oracle
+conda create -n pyo_oracle conda-forge::pyo-oracle
 
 # or with pip
-pip install pyo_oracle
+pip install pyo-oracle
 ```
 
 Please open an issue if you experience any problems. More documentation coming soon!
```

### Comparing `pyo_oracle-0.0.1a0/README.md` & `pyo_oracle-0.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -27,14 +27,14 @@
 pyo_oracle.list_local_data()
 ```
 
 ### Installation
 
 ```bash
 # With conda
-conda create -n pyo_oracle conda-forge::pyo_oracle
+conda create -n pyo_oracle conda-forge::pyo-oracle
 
 # or with pip
-pip install pyo_oracle
+pip install pyo-oracle
 ```
 
 Please open an issue if you experience any problems. More documentation coming soon!
```

### Comparing `pyo_oracle-0.0.1a0/pyo_oracle/config.py` & `pyo_oracle-0.0.2/pyo_oracle/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import configparser
 from pathlib import Path
 from erddapy import ERDDAP
 
 
 _default_config = {
     "data_directory": str(Path(__file__).parent.joinpath("data/").absolute()),
-    "erddap_server": "http://erddap.bio-oracle.org/erddap/",
+    "erddap_server": "https://erddap.bio-oracle.org/erddap/",
     "skip_confirmation": False,
 }
 
 config_file = Path(__file__).absolute().parent.joinpath(("config.ini"))
 
 
 def create_config(default_config: dict = _default_config, path: str = None) -> None:
```

### Comparing `pyo_oracle-0.0.1a0/pyo_oracle/main.py` & `pyo_oracle-0.0.2/pyo_oracle/main.py`

 * *Files identical despite different names*

### Comparing `pyo_oracle-0.0.1a0/pyo_oracle/utils.py` & `pyo_oracle-0.0.2/pyo_oracle/utils.py`

 * *Files identical despite different names*

### Comparing `pyo_oracle-0.0.1a0/pyo_oracle.egg-info/PKG-INFO` & `pyo_oracle-0.0.2/pyo_oracle.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyo-oracle
-Version: 0.0.1a0
+Version: 0.0.2
 Summary: Python client for the Bio-ORACLE ERDDAP server.
 Author-email: Vini Salazar <vinicius.salazar@unimelb.edu.au>
 Project-URL: Homepage, https://github.com/bio-oracle/pyo_oracle
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -40,14 +40,14 @@
 pyo_oracle.list_local_data()
 ```
 
 ### Installation
 
 ```bash
 # With conda
-conda create -n pyo_oracle conda-forge::pyo_oracle
+conda create -n pyo_oracle conda-forge::pyo-oracle
 
 # or with pip
-pip install pyo_oracle
+pip install pyo-oracle
 ```
 
 Please open an issue if you experience any problems. More documentation coming soon!
```

### Comparing `pyo_oracle-0.0.1a0/pyproject.toml` & `pyo_oracle-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 packages = ["pyo_oracle"]
 
 [project]
 name = "pyo_oracle"
-version = "0.0.1a"
+version = "0.0.2"
 authors = [
   { name="Vini Salazar", email="vinicius.salazar@unimelb.edu.au" },
 ]
 description = "Python client for the Bio-ORACLE ERDDAP server."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pyo_oracle-0.0.1a0/tests/test_main.py` & `pyo_oracle-0.0.2/tests/test_main.py`

 * *Files identical despite different names*

