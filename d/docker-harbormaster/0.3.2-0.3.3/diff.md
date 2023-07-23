# Comparing `tmp/docker_harbormaster-0.3.2.tar.gz` & `tmp/docker_harbormaster-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker_harbormaster-0.3.2.tar", max compression
+gzip compressed data, was "docker_harbormaster-0.3.3.tar", max compression
```

## Comparing `docker_harbormaster-0.3.2.tar` & `docker_harbormaster-0.3.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    34463 2023-07-23 20:50:33.755018 docker_harbormaster-0.3.2/LICENSE
--rw-r--r--   0        0        0    17897 2023-07-23 20:50:49.822507 docker_harbormaster-0.3.2/README.md
--rw-r--r--   0        0        0        0 2023-07-23 20:50:33.777018 docker_harbormaster-0.3.2/docker_harbormaster/__init__.py
--rwxr-xr-x   0        0        0    28575 2023-07-23 20:50:33.756852 docker_harbormaster-0.3.2/docker_harbormaster/cli.py
--rwxr-xr-x   0        0        0        0 2023-07-23 20:50:33.777018 docker_harbormaster-0.3.2/docker_harbormaster/conftest.py
--rw-r--r--   0        0        0     2777 2023-07-23 20:50:33.756852 docker_harbormaster-0.3.2/docker_harbormaster/utils.py
--rw-r--r--   0        0        0      815 2023-07-23 20:50:33.757768 docker_harbormaster-0.3.2/pyproject.toml
--rw-r--r--   0        0        0    18808 1970-01-01 00:00:00.000000 docker_harbormaster-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    34463 2023-07-23 22:44:54.410761 docker_harbormaster-0.3.3/LICENSE
+-rw-r--r--   0        0        0    17954 2023-07-23 22:45:11.969660 docker_harbormaster-0.3.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-23 22:44:54.436761 docker_harbormaster-0.3.3/docker_harbormaster/__init__.py
+-rwxr-xr-x   0        0        0    28575 2023-07-23 22:44:54.411761 docker_harbormaster-0.3.3/docker_harbormaster/cli.py
+-rwxr-xr-x   0        0        0        0 2023-07-23 22:44:54.436761 docker_harbormaster-0.3.3/docker_harbormaster/conftest.py
+-rw-r--r--   0        0        0     2777 2023-07-23 22:44:54.411761 docker_harbormaster-0.3.3/docker_harbormaster/utils.py
+-rw-r--r--   0        0        0      815 2023-07-23 22:44:54.412761 docker_harbormaster-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0    18865 1970-01-01 00:00:00.000000 docker_harbormaster-0.3.3/PKG-INFO
```

### Comparing `docker_harbormaster-0.3.2/LICENSE` & `docker_harbormaster-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `docker_harbormaster-0.3.2/README.md` & `docker_harbormaster-0.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -475,14 +475,23 @@
     url: https://gitlab.com/stavros/harbormaster.git
     compose_config: apps/octoprint/docker-compose.harbormaster.yml
 ```
 
 # Changelog
 
 
+## v0.3.3 (2023-07-23)
+
+### Fixes
+
+* Add missing crond invocation back. [Stavros Korokithakis]
+
+* Don't complain about the directory if we restart the container. [Stavros Korokithakis]
+
+
 ## v0.3.2 (2023-07-23)
 
 ### Fixes
 
 * Fix tests. [Stavros Korokithakis]
 
 * Fix the Harbormaster Docker container. [Stavros Korokithakis]
@@ -535,14 +544,7 @@
 * Improve compatibility with earlier Docker versions. [Stavros Korokithakis]
 
 * Remove the need for passing the data path to the HM container. [Stavros Korokithakis]
 
 * Forward environment variables from the host to the Dockerized HM instance. [Stavros Korokithakis]
 
 
-## v0.1.20 (2021-11-14)
-
-### Fixes
-
-* Fix wrong volume path when Harbormaster is deployed inside Docker. [Stavros Korokithakis]
-
-
```

### Comparing `docker_harbormaster-0.3.2/docker_harbormaster/cli.py` & `docker_harbormaster-0.3.3/docker_harbormaster/cli.py`

 * *Files identical despite different names*

### Comparing `docker_harbormaster-0.3.2/docker_harbormaster/utils.py` & `docker_harbormaster-0.3.3/docker_harbormaster/utils.py`

 * *Files identical despite different names*

### Comparing `docker_harbormaster-0.3.2/PKG-INFO` & `docker_harbormaster-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-harbormaster
-Version: 0.3.2
+Version: 0.3.3
 Summary: A supervisor for docker-compose apps.
 Home-page: https://gitlab.com/stavros/harbormaster
 License: AGPL-3.0-or-later
 Author: Stavros Korokithakis
 Author-email: hi@stavros.io
 Requires-Python: >=3.7,<4
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
@@ -498,14 +498,23 @@
     url: https://gitlab.com/stavros/harbormaster.git
     compose_config: apps/octoprint/docker-compose.harbormaster.yml
 ```
 
 # Changelog
 
 
+## v0.3.3 (2023-07-23)
+
+### Fixes
+
+* Add missing crond invocation back. [Stavros Korokithakis]
+
+* Don't complain about the directory if we restart the container. [Stavros Korokithakis]
+
+
 ## v0.3.2 (2023-07-23)
 
 ### Fixes
 
 * Fix tests. [Stavros Korokithakis]
 
 * Fix the Harbormaster Docker container. [Stavros Korokithakis]
@@ -558,15 +567,8 @@
 * Improve compatibility with earlier Docker versions. [Stavros Korokithakis]
 
 * Remove the need for passing the data path to the HM container. [Stavros Korokithakis]
 
 * Forward environment variables from the host to the Dockerized HM instance. [Stavros Korokithakis]
 
 
-## v0.1.20 (2021-11-14)
-
-### Fixes
-
-* Fix wrong volume path when Harbormaster is deployed inside Docker. [Stavros Korokithakis]
-
-
```

