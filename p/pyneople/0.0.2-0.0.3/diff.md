# Comparing `tmp/pyneople-0.0.2.tar.gz` & `tmp/pyneople-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyneople-0.0.2.tar", last modified: Fri Jul 21 06:04:50 2023, max compression
+gzip compressed data, was "pyneople-0.0.3.tar", last modified: Mon Jul 24 04:46:19 2023, max compression
```

## Comparing `pyneople-0.0.2.tar` & `pyneople-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 06:04:50.253275 pyneople-0.0.2/
--rw-rw-rw-   0        0        0     1088 2023-07-21 05:43:07.000000 pyneople-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      579 2023-07-21 06:04:50.252275 pyneople-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       54 2023-07-21 05:43:07.000000 pyneople-0.0.2/README.md
--rw-rw-rw-   0        0        0      108 2023-07-21 05:43:07.000000 pyneople-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-21 06:04:50.253275 pyneople-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      833 2023-07-21 06:03:20.000000 pyneople-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 06:04:50.224277 pyneople-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-21 06:04:50.240277 pyneople-0.0.2/src/pyneople/
--rw-rw-rw-   0        0        0     2796 2023-07-21 05:43:07.000000 pyneople-0.0.2/src/pyneople/METADATA.py
--rw-rw-rw-   0        0        0      199 2023-07-21 05:47:45.000000 pyneople-0.0.2/src/pyneople/__init__.py
--rw-rw-rw-   0        0        0     1722 2023-07-21 05:43:07.000000 pyneople-0.0.2/src/pyneople/avatars.py
--rw-rw-rw-   0        0        0     1403 2023-07-21 05:43:07.000000 pyneople-0.0.2/src/pyneople/character_search.py
--rw-rw-rw-   0        0        0     4643 2023-07-21 05:59:42.000000 pyneople-0.0.2/src/pyneople/equipments.py
--rw-rw-rw-   0        0        0     7209 2023-07-21 05:43:07.000000 pyneople-0.0.2/src/pyneople/functions.py
--rw-rw-rw-   0        0        0     3048 2023-07-21 05:43:07.000000 pyneople-0.0.2/src/pyneople/others.py
--rw-rw-rw-   0        0        0     1328 2023-07-21 05:43:07.000000 pyneople-0.0.2/src/pyneople/status.py
--rw-rw-rw-   0        0        0     3999 2023-07-21 05:43:07.000000 pyneople-0.0.2/src/pyneople/timeline.py
-drwxrwxrwx   0        0        0        0 2023-07-21 06:04:50.251276 pyneople-0.0.2/src/pyneople.egg-info/
--rw-rw-rw-   0        0        0      579 2023-07-21 06:04:50.000000 pyneople-0.0.2/src/pyneople.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      416 2023-07-21 06:04:50.000000 pyneople-0.0.2/src/pyneople.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 06:04:50.000000 pyneople-0.0.2/src/pyneople.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-21 06:04:50.000000 pyneople-0.0.2/src/pyneople.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 04:46:19.121891 pyneople-0.0.3/
+-rw-rw-rw-   0        0        0     1088 2023-07-21 05:43:07.000000 pyneople-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      579 2023-07-24 04:46:19.121891 pyneople-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       54 2023-07-21 05:43:07.000000 pyneople-0.0.3/README.md
+-rw-rw-rw-   0        0        0      108 2023-07-21 05:43:07.000000 pyneople-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-24 04:46:19.121891 pyneople-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      833 2023-07-24 04:43:39.000000 pyneople-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 04:46:19.092571 pyneople-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-24 04:46:19.110365 pyneople-0.0.3/src/pyneople/
+-rw-rw-rw-   0        0        0     2889 2023-07-24 04:27:44.000000 pyneople-0.0.3/src/pyneople/METADATA.py
+-rw-rw-rw-   0        0        0      199 2023-07-21 05:47:45.000000 pyneople-0.0.3/src/pyneople/__init__.py
+-rw-rw-rw-   0        0        0     1722 2023-07-21 05:43:07.000000 pyneople-0.0.3/src/pyneople/avatars.py
+-rw-rw-rw-   0        0        0     3269 2023-07-24 04:40:47.000000 pyneople-0.0.3/src/pyneople/buff.py
+-rw-rw-rw-   0        0        0     1403 2023-07-21 05:43:07.000000 pyneople-0.0.3/src/pyneople/character_search.py
+-rw-rw-rw-   0        0        0     4643 2023-07-21 05:59:42.000000 pyneople-0.0.3/src/pyneople/equipments.py
+-rw-rw-rw-   0        0        0     7209 2023-07-21 05:43:07.000000 pyneople-0.0.3/src/pyneople/functions.py
+-rw-rw-rw-   0        0        0     3048 2023-07-21 05:43:07.000000 pyneople-0.0.3/src/pyneople/others.py
+-rw-rw-rw-   0        0        0     1328 2023-07-21 05:43:07.000000 pyneople-0.0.3/src/pyneople/status.py
+-rw-rw-rw-   0        0        0     3999 2023-07-21 05:43:07.000000 pyneople-0.0.3/src/pyneople/timeline.py
+drwxrwxrwx   0        0        0        0 2023-07-24 04:46:19.120895 pyneople-0.0.3/src/pyneople.egg-info/
+-rw-rw-rw-   0        0        0      579 2023-07-24 04:46:19.000000 pyneople-0.0.3/src/pyneople.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      437 2023-07-24 04:46:19.000000 pyneople-0.0.3/src/pyneople.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 04:46:19.000000 pyneople-0.0.3/src/pyneople.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-24 04:46:19.000000 pyneople-0.0.3/src/pyneople.egg-info/top_level.txt
```

### Comparing `pyneople-0.0.2/LICENSE` & `pyneople-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyneople-0.0.2/PKG-INFO` & `pyneople-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyneople
-Version: 0.0.2
+Version: 0.0.3
 Summary: Neople Open API wrapper for data analyst
 Home-page: https://github.com/ippo252525/PyNeople
 Author: ippo252525
 Author-email: ippo252525@gmail.com
 Project-URL: Bug Tracker, https://github.com/ippo252525/PyNeople/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyneople-0.0.2/setup.py` & `pyneople-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyneople",
-    version="0.0.2",
+    version="0.0.3",
     author="ippo252525",
     author_email="ippo252525@gmail.com",
     description="Neople Open API wrapper for data analyst",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ippo252525/PyNeople",
     project_urls={
```

### Comparing `pyneople-0.0.2/src/pyneople/METADATA.py` & `pyneople-0.0.3/src/pyneople/METADATA.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,8 +52,11 @@
 
 del jobclass_list
 
 # 착용가능 장비
 EQUIPMENT_LIST = ['weapon', 'title', 'jacket', 'shoulder', 'pants', 'shoes', 'waist', 'amulet', 'wrist', 'ring', 'support', 'magic_ston', 'earring']
 
 # 착용가능 아바타
-AVATAR_LIST = ['headgear', 'hair', 'face', 'jacket', 'pants', 'shoes', 'breast', 'waist', 'skin', 'aurora', 'weapon']
+AVATAR_LIST = ['headgear', 'hair', 'face', 'jacket', 'pants', 'shoes', 'breast', 'waist', 'skin', 'aurora', 'weapon']
+
+# 플래티넘 엠블렘 착용 가능 부위
+PLATINUM_AVATAR_LIST = ['jacket', 'pants']
```

### Comparing `pyneople-0.0.2/src/pyneople/avatars.py` & `pyneople-0.0.3/src/pyneople/avatars.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.0.2/src/pyneople/character_search.py` & `pyneople-0.0.3/src/pyneople/character_search.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.0.2/src/pyneople/equipments.py` & `pyneople-0.0.3/src/pyneople/equipments.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.0.2/src/pyneople/functions.py` & `pyneople-0.0.3/src/pyneople/functions.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.0.2/src/pyneople/others.py` & `pyneople-0.0.3/src/pyneople/others.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.0.2/src/pyneople/status.py` & `pyneople-0.0.3/src/pyneople/status.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.0.2/src/pyneople/timeline.py` & `pyneople-0.0.3/src/pyneople/timeline.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.0.2/src/pyneople.egg-info/PKG-INFO` & `pyneople-0.0.3/src/pyneople.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyneople
-Version: 0.0.2
+Version: 0.0.3
 Summary: Neople Open API wrapper for data analyst
 Home-page: https://github.com/ippo252525/PyNeople
 Author: ippo252525
 Author-email: ippo252525@gmail.com
 Project-URL: Bug Tracker, https://github.com/ippo252525/PyNeople/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

