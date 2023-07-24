# Comparing `tmp/osm_easy_api-1.0.0.tar.gz` & `tmp/osm_easy_api-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osm_easy_api-1.0.0.tar", last modified: Sun Jun 18 21:46:37 2023, max compression
+gzip compressed data, was "osm_easy_api-1.0.1.tar", last modified: Mon Jul 24 09:45:21 2023, max compression
```

## Comparing `osm_easy_api-1.0.0.tar` & `osm_easy_api-1.0.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 21:46:37.084672 osm_easy_api-1.0.0/
--rw-rw-rw-   0        0        0     3488 2023-06-18 20:59:09.000000 osm_easy_api-1.0.0/CHANGELOG.md
--rw-rw-rw-   0        0        0    35821 2023-03-07 21:14:41.000000 osm_easy_api-1.0.0/LICENSE.md
--rw-rw-rw-   0        0        0    45172 2023-06-18 21:46:37.085674 osm_easy_api-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4946 2023-06-18 21:44:28.000000 osm_easy_api-1.0.0/README.md
--rw-rw-rw-   0        0        0       97 2023-03-07 21:14:41.000000 osm_easy_api-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0     1197 2023-06-18 21:46:37.087751 osm_easy_api-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0       71 2023-03-07 21:14:41.000000 osm_easy_api-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-18 21:46:37.020171 osm_easy_api-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-18 21:46:37.031239 osm_easy_api-1.0.0/src/osm_easy_api/
--rw-rw-rw-   0        0        0      107 2023-06-18 21:01:38.000000 osm_easy_api-1.0.0/src/osm_easy_api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-18 21:46:37.059458 osm_easy_api-1.0.0/src/osm_easy_api/api/
--rw-rw-rw-   0        0        0     3033 2023-03-07 21:14:41.000000 osm_easy_api-1.0.0/src/osm_easy_api/api/_URLs.py
--rw-rw-rw-   0        0        0      101 2023-03-07 21:14:41.000000 osm_easy_api-1.0.0/src/osm_easy_api/api/__init__.py
--rw-rw-rw-   0        0        0     4336 2023-03-08 21:18:46.000000 osm_easy_api-1.0.0/src/osm_easy_api/api/api.py
-drwxrwxrwx   0        0        0        0 2023-06-18 21:46:37.068878 osm_easy_api-1.0.0/src/osm_easy_api/api/endpoints/
--rw-rw-rw-   0        0        0      520 2023-03-07 21:14:41.000000 osm_easy_api-1.0.0/src/osm_easy_api/api/endpoints/__init__.py
--rw-rw-rw-   0        0        0    14641 2023-06-18 20:57:38.000000 osm_easy_api-1.0.0/src/osm_easy_api/api/endpoints/changeset.py
--rw-rw-rw-   0        0        0     4464 2023-06-18 20:57:49.000000 osm_easy_api-1.0.0/src/osm_easy_api/api/endpoints/changeset_discussion.py
--rw-rw-rw-   0        0        0    17201 2023-06-18 20:56:56.000000 osm_easy_api-1.0.0/src/osm_easy_api/api/endpoints/elements.py
--rw-rw-rw-   0        0        0     1062 2023-03-07 21:14:41.000000 osm_easy_api-1.0.0/src/osm_easy_api/api/endpoints/gpx.py
--rw-rw-rw-   0        0        0     5559 2023-06-18 20:56:12.000000 osm_easy_api-1.0.0/src/osm_easy_api/api/endpoints/misc.py
--rw-rw-rw-   0        0        0    11501 2023-06-18 20:56:07.000000 osm_easy_api-1.0.0/src/osm_easy_api/api/endpoints/notes.py
--rw-rw-rw-   0        0        0     7047 2023-04-02 18:18:25.000000 osm_easy_api-1.0.0/src/osm_easy_api/api/endpoints/user.py
--rw-rw-rw-   0        0        0     1025 2023-03-07 21:14:41.000000 osm_easy_api-1.0.0/src/osm_easy_api/api/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-18 21:46:37.078663 osm_easy_api-1.0.0/src/osm_easy_api/data_classes/
--rw-rw-rw-   0        0        0     8062 2023-06-18 17:27:38.000000 osm_easy_api-1.0.0/src/osm_easy_api/data_classes/OsmChange.py
--rw-rw-rw-   0        0        0      432 2023-03-22 23:03:24.000000 osm_easy_api-1.0.0/src/osm_easy_api/data_classes/__init__.py
--rw-rw-rw-   0        0        0     1785 2023-03-14 14:11:03.000000 osm_easy_api-1.0.0/src/osm_easy_api/data_classes/changeset.py
--rw-rw-rw-   0        0        0     1144 2023-06-10 21:48:54.000000 osm_easy_api-1.0.0/src/osm_easy_api/data_classes/node.py
--rw-rw-rw-   0        0        0     4022 2023-03-22 21:29:55.000000 osm_easy_api-1.0.0/src/osm_easy_api/data_classes/note.py
--rw-rw-rw-   0        0        0     2635 2023-05-03 15:23:00.000000 osm_easy_api-1.0.0/src/osm_easy_api/data_classes/osm_object_primitive.py
--rw-rw-rw-   0        0        0     2786 2023-06-10 21:42:40.000000 osm_easy_api-1.0.0/src/osm_easy_api/data_classes/relation.py
--rw-rw-rw-   0        0        0     1403 2023-03-22 23:13:07.000000 osm_easy_api-1.0.0/src/osm_easy_api/data_classes/tags.py
--rw-rw-rw-   0        0        0     2099 2023-03-22 20:09:45.000000 osm_easy_api-1.0.0/src/osm_easy_api/data_classes/user.py
--rw-rw-rw-   0        0        0     1725 2023-06-10 21:48:37.000000 osm_easy_api-1.0.0/src/osm_easy_api/data_classes/way.py
-drwxrwxrwx   0        0        0        0 2023-06-18 21:46:37.081426 osm_easy_api-1.0.0/src/osm_easy_api/diff/
--rw-rw-rw-   0        0        0      111 2023-03-07 21:14:41.000000 osm_easy_api-1.0.0/src/osm_easy_api/diff/__init__.py
--rw-rw-rw-   0        0        0     6164 2023-04-01 19:34:36.000000 osm_easy_api-1.0.0/src/osm_easy_api/diff/diff.py
--rw-rw-rw-   0        0        0     9075 2023-03-07 21:24:24.000000 osm_easy_api-1.0.0/src/osm_easy_api/diff/diff_parser.py
--rw-rw-rw-   0        0        0        0 2023-03-07 21:14:41.000000 osm_easy_api-1.0.0/src/osm_easy_api/py.typed
-drwxrwxrwx   0        0        0        0 2023-06-18 21:46:37.084672 osm_easy_api-1.0.0/src/osm_easy_api/utils/
--rw-rw-rw-   0        0        0       82 2023-03-07 21:14:41.000000 osm_easy_api-1.0.0/src/osm_easy_api/utils/__init__.py
--rw-rw-rw-   0        0        0      166 2023-03-07 21:14:41.000000 osm_easy_api-1.0.0/src/osm_easy_api/utils/join_url.py
--rw-rw-rw-   0        0        0      397 2023-03-07 21:14:41.000000 osm_easy_api-1.0.0/src/osm_easy_api/utils/write_gzip_to_file.py
-drwxrwxrwx   0        0        0        0 2023-06-18 21:46:37.055558 osm_easy_api-1.0.0/src/osm_easy_api.egg-info/
--rw-rw-rw-   0        0        0    45172 2023-06-18 21:46:37.000000 osm_easy_api-1.0.0/src/osm_easy_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1456 2023-06-18 21:46:37.000000 osm_easy_api-1.0.0/src/osm_easy_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 21:46:37.000000 osm_easy_api-1.0.0/src/osm_easy_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-07 21:15:07.000000 osm_easy_api-1.0.0/src/osm_easy_api.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       90 2023-06-18 21:46:37.000000 osm_easy_api-1.0.0/src/osm_easy_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-18 21:46:37.000000 osm_easy_api-1.0.0/src/osm_easy_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 09:45:21.074652 osm_easy_api-1.0.1/
+-rw-rw-rw-   0        0        0     3567 2023-07-24 09:44:18.000000 osm_easy_api-1.0.1/CHANGELOG.md
+-rw-rw-rw-   0        0        0    35821 2023-03-07 21:14:41.000000 osm_easy_api-1.0.1/LICENSE.md
+-rw-rw-rw-   0        0        0    45252 2023-07-24 09:45:21.076172 osm_easy_api-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4947 2023-07-24 09:37:44.000000 osm_easy_api-1.0.1/README.md
+-rw-rw-rw-   0        0        0       97 2023-03-07 21:14:41.000000 osm_easy_api-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1197 2023-07-24 09:45:21.088834 osm_easy_api-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0       71 2023-03-07 21:14:41.000000 osm_easy_api-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 09:45:20.954883 osm_easy_api-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-24 09:45:20.979426 osm_easy_api-1.0.1/src/osm_easy_api/
+-rw-rw-rw-   0        0        0      107 2023-07-24 09:44:18.000000 osm_easy_api-1.0.1/src/osm_easy_api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 09:45:21.026010 osm_easy_api-1.0.1/src/osm_easy_api/api/
+-rw-rw-rw-   0        0        0     3033 2023-03-07 21:14:41.000000 osm_easy_api-1.0.1/src/osm_easy_api/api/_URLs.py
+-rw-rw-rw-   0        0        0      101 2023-03-07 21:14:41.000000 osm_easy_api-1.0.1/src/osm_easy_api/api/__init__.py
+-rw-rw-rw-   0        0        0     4336 2023-03-08 21:18:46.000000 osm_easy_api-1.0.1/src/osm_easy_api/api/api.py
+drwxrwxrwx   0        0        0        0 2023-07-24 09:45:21.043022 osm_easy_api-1.0.1/src/osm_easy_api/api/endpoints/
+-rw-rw-rw-   0        0        0      520 2023-03-07 21:14:41.000000 osm_easy_api-1.0.1/src/osm_easy_api/api/endpoints/__init__.py
+-rw-rw-rw-   0        0        0    14641 2023-06-18 20:57:38.000000 osm_easy_api-1.0.1/src/osm_easy_api/api/endpoints/changeset.py
+-rw-rw-rw-   0        0        0     4464 2023-06-18 20:57:49.000000 osm_easy_api-1.0.1/src/osm_easy_api/api/endpoints/changeset_discussion.py
+-rw-rw-rw-   0        0        0    17201 2023-06-18 20:56:56.000000 osm_easy_api-1.0.1/src/osm_easy_api/api/endpoints/elements.py
+-rw-rw-rw-   0        0        0     1062 2023-03-07 21:14:41.000000 osm_easy_api-1.0.1/src/osm_easy_api/api/endpoints/gpx.py
+-rw-rw-rw-   0        0        0     5559 2023-06-18 20:56:12.000000 osm_easy_api-1.0.1/src/osm_easy_api/api/endpoints/misc.py
+-rw-rw-rw-   0        0        0    11507 2023-07-24 09:44:18.000000 osm_easy_api-1.0.1/src/osm_easy_api/api/endpoints/notes.py
+-rw-rw-rw-   0        0        0     7047 2023-04-02 18:18:25.000000 osm_easy_api-1.0.1/src/osm_easy_api/api/endpoints/user.py
+-rw-rw-rw-   0        0        0     1025 2023-03-07 21:14:41.000000 osm_easy_api-1.0.1/src/osm_easy_api/api/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-24 09:45:21.063072 osm_easy_api-1.0.1/src/osm_easy_api/data_classes/
+-rw-rw-rw-   0        0        0     8062 2023-06-18 17:27:38.000000 osm_easy_api-1.0.1/src/osm_easy_api/data_classes/OsmChange.py
+-rw-rw-rw-   0        0        0      432 2023-03-22 23:03:24.000000 osm_easy_api-1.0.1/src/osm_easy_api/data_classes/__init__.py
+-rw-rw-rw-   0        0        0     1785 2023-03-14 14:11:03.000000 osm_easy_api-1.0.1/src/osm_easy_api/data_classes/changeset.py
+-rw-rw-rw-   0        0        0     1144 2023-06-10 21:48:54.000000 osm_easy_api-1.0.1/src/osm_easy_api/data_classes/node.py
+-rw-rw-rw-   0        0        0     4022 2023-03-22 21:29:55.000000 osm_easy_api-1.0.1/src/osm_easy_api/data_classes/note.py
+-rw-rw-rw-   0        0        0     2635 2023-05-03 15:23:00.000000 osm_easy_api-1.0.1/src/osm_easy_api/data_classes/osm_object_primitive.py
+-rw-rw-rw-   0        0        0     2786 2023-06-10 21:42:40.000000 osm_easy_api-1.0.1/src/osm_easy_api/data_classes/relation.py
+-rw-rw-rw-   0        0        0     1403 2023-03-22 23:13:07.000000 osm_easy_api-1.0.1/src/osm_easy_api/data_classes/tags.py
+-rw-rw-rw-   0        0        0     2099 2023-03-22 20:09:45.000000 osm_easy_api-1.0.1/src/osm_easy_api/data_classes/user.py
+-rw-rw-rw-   0        0        0     1725 2023-06-10 21:48:37.000000 osm_easy_api-1.0.1/src/osm_easy_api/data_classes/way.py
+drwxrwxrwx   0        0        0        0 2023-07-24 09:45:21.068371 osm_easy_api-1.0.1/src/osm_easy_api/diff/
+-rw-rw-rw-   0        0        0      111 2023-03-07 21:14:41.000000 osm_easy_api-1.0.1/src/osm_easy_api/diff/__init__.py
+-rw-rw-rw-   0        0        0     6164 2023-04-01 19:34:36.000000 osm_easy_api-1.0.1/src/osm_easy_api/diff/diff.py
+-rw-rw-rw-   0        0        0     9075 2023-03-07 21:24:24.000000 osm_easy_api-1.0.1/src/osm_easy_api/diff/diff_parser.py
+-rw-rw-rw-   0        0        0        0 2023-03-07 21:14:41.000000 osm_easy_api-1.0.1/src/osm_easy_api/py.typed
+drwxrwxrwx   0        0        0        0 2023-07-24 09:45:21.073324 osm_easy_api-1.0.1/src/osm_easy_api/utils/
+-rw-rw-rw-   0        0        0       82 2023-03-07 21:14:41.000000 osm_easy_api-1.0.1/src/osm_easy_api/utils/__init__.py
+-rw-rw-rw-   0        0        0      166 2023-03-07 21:14:41.000000 osm_easy_api-1.0.1/src/osm_easy_api/utils/join_url.py
+-rw-rw-rw-   0        0        0      397 2023-03-07 21:14:41.000000 osm_easy_api-1.0.1/src/osm_easy_api/utils/write_gzip_to_file.py
+drwxrwxrwx   0        0        0        0 2023-07-24 09:45:21.017980 osm_easy_api-1.0.1/src/osm_easy_api.egg-info/
+-rw-rw-rw-   0        0        0    45252 2023-07-24 09:45:20.000000 osm_easy_api-1.0.1/src/osm_easy_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1456 2023-07-24 09:45:20.000000 osm_easy_api-1.0.1/src/osm_easy_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 09:45:20.000000 osm_easy_api-1.0.1/src/osm_easy_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-24 09:45:20.000000 osm_easy_api-1.0.1/src/osm_easy_api.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       90 2023-07-24 09:45:20.000000 osm_easy_api-1.0.1/src/osm_easy_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-24 09:45:20.000000 osm_easy_api-1.0.1/src/osm_easy_api.egg-info/top_level.txt
```

### Comparing `osm_easy_api-1.0.0/CHANGELOG.md` & `osm_easy_api-1.0.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.0.1]
+### Fixed
+- `api.notes.create()` created only anonymous notes.
+
 ## [1.0.0]
 ### Added
 - `to_xml()` method in `OsmChange`.
 - `upload()` method in `changeset` `endpoint` has new optional arguments.
 - Test for `to_xml()` method in `OsmChange`.
 - `# pragma: no cover` for unexpected api errors (Those that are not in the specification on the wiki).
```

### Comparing `osm_easy_api-1.0.0/LICENSE.md` & `osm_easy_api-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.0/PKG-INFO` & `osm_easy_api-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osm_easy_api
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python package for parsing osm diffs and communicating with the osm api.
 Home-page: https://github.com/docentYT/osm_easy_api
 License: GPLv3
 Keywords: openstreetmap,osm,api,wrapper,diff
 Platform: unix
 Platform: linux
 Platform: osx
@@ -34,15 +34,15 @@
     <img src="https://img.shields.io/pypi/dm/osm_easy_api" alt="pypi downloads">
   </a>
   <a href="https://pypi.org/project/osm-easy-api/">
     <img alt="python versions" src="https://img.shields.io/pypi/pyversions/osm_easy_api" target="_blank" />
   </a>
 </p>
 
-<p align="center"><a href="https://www.openstreetmap.org/user/kwiatek_123)">Me on OpenStreetMap</a></p>
+<p align="center"><a href="https://www.openstreetmap.org/user/kwiatek_123">Me on OpenStreetMap</a></p>
 
 Python package for parsing osm diffs and communicating with the OpenStreetMap api. See API.txt for list of supported endpoints.
 
 ## What's the point of this package?
 
 This package was created to provide an easy way to create automated scripts and programs that use diff and/or osm api. The main advantage is the classes (data_classes) that provide data of elements (node, way, relation, OsmChange, etc.) in a readable way and the possibility to use them in diff and api without worrying about missing data or dictionaries. You can easily find nodes in diff, add a tag to them and send the corrected version to osm.
 
@@ -163,21 +163,26 @@
 ```
 but it can consume large amounts of ram and use of this method is not recommended for large diff's.
 
 # Tests
 
 You will need to install `test-requirements.txt`. You can use tox.
 To run tests manually use `python -m unittest discover`.
+
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.0.1]
+### Fixed
+- `api.notes.create()` created only anonymous notes.
+
 ## [1.0.0]
 ### Added
 - `to_xml()` method in `OsmChange`.
 - `upload()` method in `changeset` `endpoint` has new optional arguments.
 - Test for `to_xml()` method in `OsmChange`.
 - `# pragma: no cover` for unexpected api errors (Those that are not in the specification on the wiki).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: osm_easy_api Version: 1.0.0 Summary: Python package
+Metadata-Version: 2.1 Name: osm_easy_api Version: 1.0.1 Summary: Python package
 for parsing osm diffs and communicating with the osm api. Home-page: https://
 github.com/docentYT/osm_easy_api License: GPLv3 Keywords:
 openstreetmap,osm,api,wrapper,diff Platform: unix Platform: linux Platform: osx
 Platform: win32 Classifier: Development Status :: 4 - Beta Classifier: Intended
 Audience :: Developers Classifier: Natural Language :: English Classifier:
 Topic :: Scientific/Engineering :: GIS Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
@@ -65,16 +65,17 @@
 d.get(generator=False) deleted_nodes = osmChange.get(Node, Action.DELETE) for
 node in deleted_nodes: print(node.id) ``` but it can consume large amounts of
 ram and use of this method is not recommended for large diff's. # Tests You
 will need to install `test-requirements.txt`. You can use tox. To run tests
 manually use `python -m unittest discover`. # Changelog All notable changes to
 this project will be documented in this file. The format is based on [Keep a
 Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to
-[Semantic Versioning](https://semver.org/spec/v2.0.0.html). ## [1.0.0] ###
-Added - `to_xml()` method in `OsmChange`. - `upload()` method in `changeset`
+[Semantic Versioning](https://semver.org/spec/v2.0.0.html). ## [1.0.1] ###
+Fixed - `api.notes.create()` created only anonymous notes. ## [1.0.0] ### Added
+- `to_xml()` method in `OsmChange`. - `upload()` method in `changeset`
 `endpoint` has new optional arguments. - Test for `to_xml()` method in
 `OsmChange`. - `# pragma: no cover` for unexpected api errors (Those that are
 not in the specification on the wiki). ### Changed - Private `_to_xml()` method
 in `OsmChange` is now static. ## [0.4.2] ### Changed - Order of elements in xml
 generated by `Way._to_xml()`. First tags, then nodes. ### Fixed -
 `Relation._to_xml()` was returning an xml without osm tags. - Deleted disused
 variable in `Node._to_xml()`. - Fixed incorrect relation parsing of data
```

### Comparing `osm_easy_api-1.0.0/README.md` & `osm_easy_api-1.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     <img src="https://img.shields.io/pypi/dm/osm_easy_api" alt="pypi downloads">
   </a>
   <a href="https://pypi.org/project/osm-easy-api/">
     <img alt="python versions" src="https://img.shields.io/pypi/pyversions/osm_easy_api" target="_blank" />
   </a>
 </p>
 
-<p align="center"><a href="https://www.openstreetmap.org/user/kwiatek_123)">Me on OpenStreetMap</a></p>
+<p align="center"><a href="https://www.openstreetmap.org/user/kwiatek_123">Me on OpenStreetMap</a></p>
 
 Python package for parsing osm diffs and communicating with the OpenStreetMap api. See API.txt for list of supported endpoints.
 
 ## What's the point of this package?
 
 This package was created to provide an easy way to create automated scripts and programs that use diff and/or osm api. The main advantage is the classes (data_classes) that provide data of elements (node, way, relation, OsmChange, etc.) in a readable way and the possibility to use them in diff and api without worrying about missing data or dictionaries. You can easily find nodes in diff, add a tag to them and send the corrected version to osm.
 
@@ -137,8 +137,8 @@
     print(node.id)
 ```
 but it can consume large amounts of ram and use of this method is not recommended for large diff's.
 
 # Tests
 
 You will need to install `test-requirements.txt`. You can use tox.
-To run tests manually use `python -m unittest discover`.
+To run tests manually use `python -m unittest discover`.
```

### Comparing `osm_easy_api-1.0.0/setup.cfg` & `osm_easy_api-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.0/src/osm_easy_api/api/_URLs.py` & `osm_easy_api-1.0.1/src/osm_easy_api/api/_URLs.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.0/src/osm_easy_api/api/api.py` & `osm_easy_api-1.0.1/src/osm_easy_api/api/api.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.0/src/osm_easy_api/api/endpoints/__init__.py` & `osm_easy_api-1.0.1/src/osm_easy_api/api/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.0/src/osm_easy_api/api/endpoints/changeset.py` & `osm_easy_api-1.0.1/src/osm_easy_api/api/endpoints/changeset.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.0/src/osm_easy_api/api/endpoints/changeset_discussion.py` & `osm_easy_api-1.0.1/src/osm_easy_api/api/endpoints/changeset_discussion.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.0/src/osm_easy_api/api/endpoints/elements.py` & `osm_easy_api-1.0.1/src/osm_easy_api/api/endpoints/elements.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.0/src/osm_easy_api/api/endpoints/gpx.py` & `osm_easy_api-1.0.1/src/osm_easy_api/api/endpoints/gpx.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.0/src/osm_easy_api/api/endpoints/misc.py` & `osm_easy_api-1.0.1/src/osm_easy_api/api/endpoints/misc.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.0/src/osm_easy_api/api/endpoints/notes.py` & `osm_easy_api-1.0.1/src/osm_easy_api/api/endpoints/notes.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
             text (str): Note description
 
         Returns:
             Note: Object of newly created note.
         """
         generator = self.outer._post_generator(
             url=self.outer._url.note["create"].format(latitude=latitude, longitude=longitude, text=text),
-            auth_requirement=self.outer._Requirement.NO,
+            auth_requirement=self.outer._Requirement.OPTIONAL,
             auto_status_code_handling=True)
         
         return self._xml_to_note(generator)[0]
     
     def comment(self, id: int, text: str) -> Note:
         """Add a new comment to note
```

### Comparing `osm_easy_api-1.0.0/src/osm_easy_api/api/endpoints/user.py` & `osm_easy_api-1.0.1/src/osm_easy_api/api/endpoints/user.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.0/src/osm_easy_api/api/exceptions.py` & `osm_easy_api-1.0.1/src/osm_easy_api/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.0/src/osm_easy_api/data_classes/OsmChange.py` & `osm_easy_api-1.0.1/src/osm_easy_api/data_classes/OsmChange.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.0/src/osm_easy_api/data_classes/changeset.py` & `osm_easy_api-1.0.1/src/osm_easy_api/data_classes/changeset.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.0/src/osm_easy_api/data_classes/node.py` & `osm_easy_api-1.0.1/src/osm_easy_api/data_classes/node.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.0/src/osm_easy_api/data_classes/note.py` & `osm_easy_api-1.0.1/src/osm_easy_api/data_classes/note.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.0/src/osm_easy_api/data_classes/osm_object_primitive.py` & `osm_easy_api-1.0.1/src/osm_easy_api/data_classes/osm_object_primitive.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.0/src/osm_easy_api/data_classes/relation.py` & `osm_easy_api-1.0.1/src/osm_easy_api/data_classes/relation.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.0/src/osm_easy_api/data_classes/tags.py` & `osm_easy_api-1.0.1/src/osm_easy_api/data_classes/tags.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.0/src/osm_easy_api/data_classes/user.py` & `osm_easy_api-1.0.1/src/osm_easy_api/data_classes/user.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.0/src/osm_easy_api/data_classes/way.py` & `osm_easy_api-1.0.1/src/osm_easy_api/data_classes/way.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.0/src/osm_easy_api/diff/diff.py` & `osm_easy_api-1.0.1/src/osm_easy_api/diff/diff.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.0/src/osm_easy_api/diff/diff_parser.py` & `osm_easy_api-1.0.1/src/osm_easy_api/diff/diff_parser.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.0/src/osm_easy_api.egg-info/PKG-INFO` & `osm_easy_api-1.0.1/src/osm_easy_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osm-easy-api
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python package for parsing osm diffs and communicating with the osm api.
 Home-page: https://github.com/docentYT/osm_easy_api
 License: GPLv3
 Keywords: openstreetmap,osm,api,wrapper,diff
 Platform: unix
 Platform: linux
 Platform: osx
@@ -34,15 +34,15 @@
     <img src="https://img.shields.io/pypi/dm/osm_easy_api" alt="pypi downloads">
   </a>
   <a href="https://pypi.org/project/osm-easy-api/">
     <img alt="python versions" src="https://img.shields.io/pypi/pyversions/osm_easy_api" target="_blank" />
   </a>
 </p>
 
-<p align="center"><a href="https://www.openstreetmap.org/user/kwiatek_123)">Me on OpenStreetMap</a></p>
+<p align="center"><a href="https://www.openstreetmap.org/user/kwiatek_123">Me on OpenStreetMap</a></p>
 
 Python package for parsing osm diffs and communicating with the OpenStreetMap api. See API.txt for list of supported endpoints.
 
 ## What's the point of this package?
 
 This package was created to provide an easy way to create automated scripts and programs that use diff and/or osm api. The main advantage is the classes (data_classes) that provide data of elements (node, way, relation, OsmChange, etc.) in a readable way and the possibility to use them in diff and api without worrying about missing data or dictionaries. You can easily find nodes in diff, add a tag to them and send the corrected version to osm.
 
@@ -163,21 +163,26 @@
 ```
 but it can consume large amounts of ram and use of this method is not recommended for large diff's.
 
 # Tests
 
 You will need to install `test-requirements.txt`. You can use tox.
 To run tests manually use `python -m unittest discover`.
+
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.0.1]
+### Fixed
+- `api.notes.create()` created only anonymous notes.
+
 ## [1.0.0]
 ### Added
 - `to_xml()` method in `OsmChange`.
 - `upload()` method in `changeset` `endpoint` has new optional arguments.
 - Test for `to_xml()` method in `OsmChange`.
 - `# pragma: no cover` for unexpected api errors (Those that are not in the specification on the wiki).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: osm-easy-api Version: 1.0.0 Summary: Python package
+Metadata-Version: 2.1 Name: osm-easy-api Version: 1.0.1 Summary: Python package
 for parsing osm diffs and communicating with the osm api. Home-page: https://
 github.com/docentYT/osm_easy_api License: GPLv3 Keywords:
 openstreetmap,osm,api,wrapper,diff Platform: unix Platform: linux Platform: osx
 Platform: win32 Classifier: Development Status :: 4 - Beta Classifier: Intended
 Audience :: Developers Classifier: Natural Language :: English Classifier:
 Topic :: Scientific/Engineering :: GIS Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
@@ -65,16 +65,17 @@
 d.get(generator=False) deleted_nodes = osmChange.get(Node, Action.DELETE) for
 node in deleted_nodes: print(node.id) ``` but it can consume large amounts of
 ram and use of this method is not recommended for large diff's. # Tests You
 will need to install `test-requirements.txt`. You can use tox. To run tests
 manually use `python -m unittest discover`. # Changelog All notable changes to
 this project will be documented in this file. The format is based on [Keep a
 Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to
-[Semantic Versioning](https://semver.org/spec/v2.0.0.html). ## [1.0.0] ###
-Added - `to_xml()` method in `OsmChange`. - `upload()` method in `changeset`
+[Semantic Versioning](https://semver.org/spec/v2.0.0.html). ## [1.0.1] ###
+Fixed - `api.notes.create()` created only anonymous notes. ## [1.0.0] ### Added
+- `to_xml()` method in `OsmChange`. - `upload()` method in `changeset`
 `endpoint` has new optional arguments. - Test for `to_xml()` method in
 `OsmChange`. - `# pragma: no cover` for unexpected api errors (Those that are
 not in the specification on the wiki). ### Changed - Private `_to_xml()` method
 in `OsmChange` is now static. ## [0.4.2] ### Changed - Order of elements in xml
 generated by `Way._to_xml()`. First tags, then nodes. ### Fixed -
 `Relation._to_xml()` was returning an xml without osm tags. - Deleted disused
 variable in `Node._to_xml()`. - Fixed incorrect relation parsing of data
```

### Comparing `osm_easy_api-1.0.0/src/osm_easy_api.egg-info/SOURCES.txt` & `osm_easy_api-1.0.1/src/osm_easy_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

