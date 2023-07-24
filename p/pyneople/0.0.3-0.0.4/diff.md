# Comparing `tmp/pyneople-0.0.3.tar.gz` & `tmp/pyneople-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyneople-0.0.3.tar", last modified: Mon Jul 24 04:46:19 2023, max compression
+gzip compressed data, was "pyneople-0.0.4.tar", last modified: Mon Jul 24 04:52:23 2023, max compression
```

## Comparing `pyneople-0.0.3.tar` & `pyneople-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 04:46:19.121891 pyneople-0.0.3/
--rw-rw-rw-   0        0        0     1088 2023-07-21 05:43:07.000000 pyneople-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      579 2023-07-24 04:46:19.121891 pyneople-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       54 2023-07-21 05:43:07.000000 pyneople-0.0.3/README.md
--rw-rw-rw-   0        0        0      108 2023-07-21 05:43:07.000000 pyneople-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-24 04:46:19.121891 pyneople-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      833 2023-07-24 04:43:39.000000 pyneople-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-24 04:46:19.092571 pyneople-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-24 04:46:19.110365 pyneople-0.0.3/src/pyneople/
--rw-rw-rw-   0        0        0     2889 2023-07-24 04:27:44.000000 pyneople-0.0.3/src/pyneople/METADATA.py
--rw-rw-rw-   0        0        0      199 2023-07-21 05:47:45.000000 pyneople-0.0.3/src/pyneople/__init__.py
--rw-rw-rw-   0        0        0     1722 2023-07-21 05:43:07.000000 pyneople-0.0.3/src/pyneople/avatars.py
--rw-rw-rw-   0        0        0     3269 2023-07-24 04:40:47.000000 pyneople-0.0.3/src/pyneople/buff.py
--rw-rw-rw-   0        0        0     1403 2023-07-21 05:43:07.000000 pyneople-0.0.3/src/pyneople/character_search.py
--rw-rw-rw-   0        0        0     4643 2023-07-21 05:59:42.000000 pyneople-0.0.3/src/pyneople/equipments.py
--rw-rw-rw-   0        0        0     7209 2023-07-21 05:43:07.000000 pyneople-0.0.3/src/pyneople/functions.py
--rw-rw-rw-   0        0        0     3048 2023-07-21 05:43:07.000000 pyneople-0.0.3/src/pyneople/others.py
--rw-rw-rw-   0        0        0     1328 2023-07-21 05:43:07.000000 pyneople-0.0.3/src/pyneople/status.py
--rw-rw-rw-   0        0        0     3999 2023-07-21 05:43:07.000000 pyneople-0.0.3/src/pyneople/timeline.py
-drwxrwxrwx   0        0        0        0 2023-07-24 04:46:19.120895 pyneople-0.0.3/src/pyneople.egg-info/
--rw-rw-rw-   0        0        0      579 2023-07-24 04:46:19.000000 pyneople-0.0.3/src/pyneople.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      437 2023-07-24 04:46:19.000000 pyneople-0.0.3/src/pyneople.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 04:46:19.000000 pyneople-0.0.3/src/pyneople.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-24 04:46:19.000000 pyneople-0.0.3/src/pyneople.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 04:52:23.177155 pyneople-0.0.4/
+-rw-rw-rw-   0        0        0     1088 2023-07-21 05:43:07.000000 pyneople-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      579 2023-07-24 04:52:23.176154 pyneople-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       54 2023-07-21 05:43:07.000000 pyneople-0.0.4/README.md
+-rw-rw-rw-   0        0        0      108 2023-07-21 05:43:07.000000 pyneople-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-24 04:52:23.177155 pyneople-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      833 2023-07-24 04:51:12.000000 pyneople-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 04:52:23.145307 pyneople-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-24 04:52:23.162603 pyneople-0.0.4/src/pyneople/
+-rw-rw-rw-   0        0        0     2889 2023-07-24 04:27:44.000000 pyneople-0.0.4/src/pyneople/METADATA.py
+-rw-rw-rw-   0        0        0      223 2023-07-24 04:51:23.000000 pyneople-0.0.4/src/pyneople/__init__.py
+-rw-rw-rw-   0        0        0     1722 2023-07-21 05:43:07.000000 pyneople-0.0.4/src/pyneople/avatars.py
+-rw-rw-rw-   0        0        0     3269 2023-07-24 04:40:47.000000 pyneople-0.0.4/src/pyneople/buff.py
+-rw-rw-rw-   0        0        0     1403 2023-07-21 05:43:07.000000 pyneople-0.0.4/src/pyneople/character_search.py
+-rw-rw-rw-   0        0        0     4643 2023-07-21 05:59:42.000000 pyneople-0.0.4/src/pyneople/equipments.py
+-rw-rw-rw-   0        0        0     7209 2023-07-21 05:43:07.000000 pyneople-0.0.4/src/pyneople/functions.py
+-rw-rw-rw-   0        0        0     3048 2023-07-21 05:43:07.000000 pyneople-0.0.4/src/pyneople/others.py
+-rw-rw-rw-   0        0        0     1328 2023-07-21 05:43:07.000000 pyneople-0.0.4/src/pyneople/status.py
+-rw-rw-rw-   0        0        0     3999 2023-07-21 05:43:07.000000 pyneople-0.0.4/src/pyneople/timeline.py
+drwxrwxrwx   0        0        0        0 2023-07-24 04:52:23.175153 pyneople-0.0.4/src/pyneople.egg-info/
+-rw-rw-rw-   0        0        0      579 2023-07-24 04:52:23.000000 pyneople-0.0.4/src/pyneople.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      437 2023-07-24 04:52:23.000000 pyneople-0.0.4/src/pyneople.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 04:52:23.000000 pyneople-0.0.4/src/pyneople.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-24 04:52:23.000000 pyneople-0.0.4/src/pyneople.egg-info/top_level.txt
```

### Comparing `pyneople-0.0.3/LICENSE` & `pyneople-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyneople-0.0.3/PKG-INFO` & `pyneople-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyneople
-Version: 0.0.3
+Version: 0.0.4
 Summary: Neople Open API wrapper for data analyst
 Home-page: https://github.com/ippo252525/PyNeople
 Author: ippo252525
 Author-email: ippo252525@gmail.com
 Project-URL: Bug Tracker, https://github.com/ippo252525/PyNeople/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyneople-0.0.3/setup.py` & `pyneople-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyneople",
-    version="0.0.3",
+    version="0.0.4",
     author="ippo252525",
     author_email="ippo252525@gmail.com",
     description="Neople Open API wrapper for data analyst",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ippo252525/PyNeople",
     project_urls={
```

### Comparing `pyneople-0.0.3/src/pyneople/METADATA.py` & `pyneople-0.0.4/src/pyneople/METADATA.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.0.3/src/pyneople/avatars.py` & `pyneople-0.0.4/src/pyneople/avatars.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.0.3/src/pyneople/buff.py` & `pyneople-0.0.4/src/pyneople/buff.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.0.3/src/pyneople/character_search.py` & `pyneople-0.0.4/src/pyneople/character_search.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.0.3/src/pyneople/equipments.py` & `pyneople-0.0.4/src/pyneople/equipments.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.0.3/src/pyneople/functions.py` & `pyneople-0.0.4/src/pyneople/functions.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.0.3/src/pyneople/others.py` & `pyneople-0.0.4/src/pyneople/others.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.0.3/src/pyneople/status.py` & `pyneople-0.0.4/src/pyneople/status.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.0.3/src/pyneople/timeline.py` & `pyneople-0.0.4/src/pyneople/timeline.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.0.3/src/pyneople.egg-info/PKG-INFO` & `pyneople-0.0.4/src/pyneople.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyneople
-Version: 0.0.3
+Version: 0.0.4
 Summary: Neople Open API wrapper for data analyst
 Home-page: https://github.com/ippo252525/PyNeople
 Author: ippo252525
 Author-email: ippo252525@gmail.com
 Project-URL: Bug Tracker, https://github.com/ippo252525/PyNeople/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

