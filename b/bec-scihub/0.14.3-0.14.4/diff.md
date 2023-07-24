# Comparing `tmp/bec_scihub-0.14.3.tar.gz` & `tmp/bec_scihub-0.14.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec_scihub-0.14.3.tar", last modified: Mon Jul 24 12:05:59 2023, max compression
+gzip compressed data, was "bec_scihub-0.14.4.tar", last modified: Mon Jul 24 15:02:32 2023, max compression
```

## Comparing `bec_scihub-0.14.3.tar` & `bec_scihub-0.14.4.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 12:05:59.971476 bec_scihub-0.14.3/
--rw-r--r--   0 root         (0) root         (0)      478 2023-07-24 12:05:59.972476 bec_scihub-0.14.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 12:05:59.971476 bec_scihub-0.14.3/bec_scihub.egg-info/
--rw-r--r--   0 root         (0) root         (0)      478 2023-07-24 12:05:59.000000 bec_scihub-0.14.3/bec_scihub.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      521 2023-07-24 12:05:59.000000 bec_scihub-0.14.3/bec_scihub.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 12:05:59.000000 bec_scihub-0.14.3/bec_scihub.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-07-24 12:05:59.000000 bec_scihub-0.14.3/bec_scihub.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      100 2023-07-24 12:05:59.000000 bec_scihub-0.14.3/bec_scihub.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-24 12:05:59.000000 bec_scihub-0.14.3/bec_scihub.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 12:05:59.969476 bec_scihub-0.14.3/scihub/
--rw-r--r--   0 root         (0) root         (0)       56 2023-07-08 15:33:35.000000 bec_scihub-0.14.3/scihub/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 12:05:59.970476 bec_scihub-0.14.3/scihub/scibec/
--rw-rw-rw-   0 root         (0) root         (0)      161 2023-06-19 08:14:59.000000 bec_scihub-0.14.3/scihub/scibec/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7654 2023-06-28 10:41:58.000000 bec_scihub-0.14.3/scihub/scibec/config_handler.py
--rw-r--r--   0 root         (0) root         (0)    15033 2023-06-28 10:41:58.000000 bec_scihub-0.14.3/scihub/scibec/scibec.py
--rw-r--r--   0 root         (0) root         (0)     4428 2023-06-28 10:41:58.000000 bec_scihub-0.14.3/scihub/scibec/scibec_connector.py
--rw-r--r--   0 root         (0) root         (0)     4126 2023-06-28 10:41:58.000000 bec_scihub-0.14.3/scihub/scibec/scibec_metadata_handler.py
--rw-rw-rw-   0 root         (0) root         (0)      880 2023-06-19 08:14:59.000000 bec_scihub-0.14.3/scihub/scibec/scibec_validator.py
--rw-r--r--   0 root         (0) root         (0)      902 2023-06-28 10:41:58.000000 bec_scihub-0.14.3/scihub/scihub.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 12:05:59.970476 bec_scihub-0.14.3/scihub/scilog/
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-06-19 08:14:59.000000 bec_scihub-0.14.3/scihub/scilog/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3330 2023-06-28 10:41:58.000000 bec_scihub-0.14.3/scihub/scilog/scilog.py
--rw-r--r--   0 root         (0) root         (0)      538 2023-07-24 12:05:59.972476 bec_scihub-0.14.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      633 2023-07-24 12:05:30.000000 bec_scihub-0.14.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:02:32.178531 bec_scihub-0.14.4/
+-rw-r--r--   0 root         (0) root         (0)      478 2023-07-24 15:02:32.178531 bec_scihub-0.14.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:02:32.177531 bec_scihub-0.14.4/bec_scihub.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      478 2023-07-24 15:02:32.000000 bec_scihub-0.14.4/bec_scihub.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      569 2023-07-24 15:02:32.000000 bec_scihub-0.14.4/bec_scihub.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 15:02:32.000000 bec_scihub-0.14.4/bec_scihub.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-24 15:02:32.000000 bec_scihub-0.14.4/bec_scihub.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2023-07-24 15:02:32.000000 bec_scihub-0.14.4/bec_scihub.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-24 15:02:32.000000 bec_scihub-0.14.4/bec_scihub.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:02:32.175531 bec_scihub-0.14.4/scihub/
+-rw-r--r--   0 root         (0) root         (0)       56 2023-07-08 15:33:35.000000 bec_scihub-0.14.4/scihub/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:02:32.175531 bec_scihub-0.14.4/scihub/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 15:01:50.000000 bec_scihub-0.14.4/scihub/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      782 2023-07-08 15:33:35.000000 bec_scihub-0.14.4/scihub/cli/launch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:02:32.176531 bec_scihub-0.14.4/scihub/scibec/
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-06-19 08:14:59.000000 bec_scihub-0.14.4/scihub/scibec/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7654 2023-06-28 10:41:58.000000 bec_scihub-0.14.4/scihub/scibec/config_handler.py
+-rw-r--r--   0 root         (0) root         (0)    15033 2023-06-28 10:41:58.000000 bec_scihub-0.14.4/scihub/scibec/scibec.py
+-rw-r--r--   0 root         (0) root         (0)     4428 2023-06-28 10:41:58.000000 bec_scihub-0.14.4/scihub/scibec/scibec_connector.py
+-rw-r--r--   0 root         (0) root         (0)     4126 2023-06-28 10:41:58.000000 bec_scihub-0.14.4/scihub/scibec/scibec_metadata_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)      880 2023-06-19 08:14:59.000000 bec_scihub-0.14.4/scihub/scibec/scibec_validator.py
+-rw-r--r--   0 root         (0) root         (0)      902 2023-06-28 10:41:58.000000 bec_scihub-0.14.4/scihub/scihub.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:02:32.176531 bec_scihub-0.14.4/scihub/scilog/
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-06-19 08:14:59.000000 bec_scihub-0.14.4/scihub/scilog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3330 2023-06-28 10:41:58.000000 bec_scihub-0.14.4/scihub/scilog/scilog.py
+-rw-r--r--   0 root         (0) root         (0)      538 2023-07-24 15:02:32.178531 bec_scihub-0.14.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      633 2023-07-24 15:02:01.000000 bec_scihub-0.14.4/setup.py
```

### Comparing `bec_scihub-0.14.3/bec_scihub.egg-info/SOURCES.txt` & `bec_scihub-0.14.4/bec_scihub.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 setup.cfg
 setup.py
 ./scihub/__init__.py
 ./scihub/scihub.py
+./scihub/cli/__init__.py
+./scihub/cli/launch.py
 ./scihub/scibec/__init__.py
 ./scihub/scibec/config_handler.py
 ./scihub/scibec/scibec.py
 ./scihub/scibec/scibec_connector.py
 ./scihub/scibec/scibec_metadata_handler.py
 ./scihub/scibec/scibec_validator.py
 ./scihub/scilog/__init__.py
```

### Comparing `bec_scihub-0.14.3/scihub/scibec/config_handler.py` & `bec_scihub-0.14.4/scihub/scibec/config_handler.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.14.3/scihub/scibec/scibec.py` & `bec_scihub-0.14.4/scihub/scibec/scibec.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.14.3/scihub/scibec/scibec_connector.py` & `bec_scihub-0.14.4/scihub/scibec/scibec_connector.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.14.3/scihub/scibec/scibec_metadata_handler.py` & `bec_scihub-0.14.4/scihub/scibec/scibec_metadata_handler.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.14.3/scihub/scibec/scibec_validator.py` & `bec_scihub-0.14.4/scihub/scibec/scibec_validator.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.14.3/scihub/scihub.py` & `bec_scihub-0.14.4/scihub/scihub.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.14.3/scihub/scilog/scilog.py` & `bec_scihub-0.14.4/scihub/scilog/scilog.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.14.3/setup.cfg` & `bec_scihub-0.14.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.14.3/setup.py` & `bec_scihub-0.14.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import setup
 
 current_path = pathlib.Path(__file__).parent.resolve()
 
 utils = f"{current_path}/../bec_lib/"
 
-__version__ = "0.14.3"
+__version__ = "0.14.4"
 
 if __name__ == "__main__":
     setup(
         install_requires=["msgpack", "pyyaml", "fastjsonschema", "python-dotenv"],
         version=__version__,
         entry_points={"console_scripts": ["bec-scihub = scihub:main"]},
         extras_require={"dev": ["pytest", "pytest-random-order", "coverage", "black", "pylint"]},
```

