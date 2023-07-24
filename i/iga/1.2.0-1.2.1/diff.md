# Comparing `tmp/iga-1.2.0.tar.gz` & `tmp/iga-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iga-1.2.0.tar", last modified: Tue Jul 18 23:17:00 2023, max compression
+gzip compressed data, was "iga-1.2.1.tar", last modified: Mon Jul 24 20:28:48 2023, max compression
```

## Comparing `iga-1.2.0.tar` & `iga-1.2.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-07-18 23:17:00.201254 iga-1.2.0/
--rw-r--r--   0 mhucka     (503) staff       (20)     1527 2023-07-18 22:44:45.000000 iga-1.2.0/LICENSE
--rw-r--r--   0 mhucka     (503) staff       (20)    41457 2023-07-18 23:17:00.201406 iga-1.2.0/PKG-INFO
--rw-r--r--   0 mhucka     (503) staff       (20)    40419 2023-07-18 23:02:55.000000 iga-1.2.0/README.md
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-07-18 23:17:00.197060 iga-1.2.0/iga/
--rw-r--r--   0 mhucka     (503) staff       (20)     1533 2023-07-18 22:48:36.000000 iga-1.2.0/iga/__init__.py
--rw-r--r--   0 mhucka     (503) staff       (20)      905 2023-07-18 22:44:45.000000 iga-1.2.0/iga/__main__.py
--rw-r--r--   0 mhucka     (503) staff       (20)    35363 2023-07-18 22:48:13.000000 iga-1.2.0/iga/cli.py
--rw-r--r--   0 mhucka     (503) staff       (20)     3355 2023-07-18 22:44:45.000000 iga-1.2.0/iga/data_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     2855 2023-07-18 22:44:45.000000 iga-1.2.0/iga/doi.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1252 2023-07-18 22:44:45.000000 iga-1.2.0/iga/exceptions.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1514 2023-07-18 22:44:45.000000 iga-1.2.0/iga/exit_codes.py
--rw-r--r--   0 mhucka     (503) staff       (20)    15499 2023-07-18 22:44:45.000000 iga-1.2.0/iga/github.py
--rw-r--r--   0 mhucka     (503) staff       (20)     4901 2023-07-18 22:44:45.000000 iga-1.2.0/iga/id_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)    19440 2023-07-18 22:48:13.000000 iga-1.2.0/iga/invenio.py
--rw-r--r--   0 mhucka     (503) staff       (20)     2064 2023-07-18 22:44:45.000000 iga-1.2.0/iga/json_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)   248567 2023-07-18 22:44:45.000000 iga-1.2.0/iga/licenses.py
--rw-r--r--   0 mhucka     (503) staff       (20)    70406 2023-07-18 22:44:45.000000 iga-1.2.0/iga/metadata.py
--rw-r--r--   0 mhucka     (503) staff       (20)    14514 2023-07-18 22:44:45.000000 iga-1.2.0/iga/name_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     5273 2023-07-18 22:44:45.000000 iga-1.2.0/iga/orcid.py
--rw-r--r--   0 mhucka     (503) staff       (20)     5147 2023-07-18 22:44:45.000000 iga-1.2.0/iga/reference.py
--rw-r--r--   0 mhucka     (503) staff       (20)     3969 2023-07-18 22:44:45.000000 iga-1.2.0/iga/ror.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1624 2023-07-18 22:44:45.000000 iga-1.2.0/iga/text_utils.py
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-07-18 23:17:00.197950 iga-1.2.0/iga.egg-info/
--rw-r--r--   0 mhucka     (503) staff       (20)    41457 2023-07-18 23:17:00.000000 iga-1.2.0/iga.egg-info/PKG-INFO
--rw-r--r--   0 mhucka     (503) staff       (20)      930 2023-07-18 23:17:00.000000 iga-1.2.0/iga.egg-info/SOURCES.txt
--rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-07-18 23:17:00.000000 iga-1.2.0/iga.egg-info/dependency_links.txt
--rw-r--r--   0 mhucka     (503) staff       (20)       58 2023-07-18 23:17:00.000000 iga-1.2.0/iga.egg-info/entry_points.txt
--rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-07-18 23:17:00.000000 iga-1.2.0/iga.egg-info/not-zip-safe
--rw-r--r--   0 mhucka     (503) staff       (20)      659 2023-07-18 23:17:00.000000 iga-1.2.0/iga.egg-info/requires.txt
--rw-r--r--   0 mhucka     (503) staff       (20)        4 2023-07-18 23:17:00.000000 iga-1.2.0/iga.egg-info/top_level.txt
--rw-r--r--   0 mhucka     (503) staff       (20)     1216 2023-07-18 23:17:00.202092 iga-1.2.0/setup.cfg
--rwxr-xr-x   0 mhucka     (503) staff       (20)     1548 2023-07-18 22:48:13.000000 iga-1.2.0/setup.py
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-07-18 23:17:00.201097 iga-1.2.0/tests/
--rw-r--r--   0 mhucka     (503) staff       (20)     6117 2023-07-18 22:44:45.000000 iga-1.2.0/tests/test_cli.py
--rw-r--r--   0 mhucka     (503) staff       (20)     4481 2023-07-18 22:44:45.000000 iga-1.2.0/tests/test_data_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1417 2023-07-18 22:44:45.000000 iga-1.2.0/tests/test_doi.py
--rw-r--r--   0 mhucka     (503) staff       (20)      686 2023-07-18 22:44:45.000000 iga-1.2.0/tests/test_exceptions.py
--rw-r--r--   0 mhucka     (503) staff       (20)      177 2023-07-18 22:44:45.000000 iga-1.2.0/tests/test_exit_codes.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1446 2023-07-18 22:44:45.000000 iga-1.2.0/tests/test_github.py
--rw-r--r--   0 mhucka     (503) staff       (20)     3015 2023-07-18 22:44:45.000000 iga-1.2.0/tests/test_github_mocks.py
--rw-r--r--   0 mhucka     (503) staff       (20)     3666 2023-07-18 22:44:45.000000 iga-1.2.0/tests/test_id_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)      641 2023-07-18 22:44:45.000000 iga-1.2.0/tests/test_init.py
--rw-r--r--   0 mhucka     (503) staff       (20)    49214 2023-07-18 22:44:45.000000 iga-1.2.0/tests/test_is_person.py
--rw-r--r--   0 mhucka     (503) staff       (20)      912 2023-07-18 22:44:45.000000 iga-1.2.0/tests/test_licenses.py
--rw-r--r--   0 mhucka     (503) staff       (20)     4408 2023-07-18 22:44:45.000000 iga-1.2.0/tests/test_name_splitting.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1829 2023-07-18 22:44:45.000000 iga-1.2.0/tests/test_name_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1054 2023-07-18 22:44:45.000000 iga-1.2.0/tests/test_orcid.py
--rw-r--r--   0 mhucka     (503) staff       (20)     5997 2023-07-18 22:44:45.000000 iga-1.2.0/tests/test_record_from_codemeta.py
--rw-r--r--   0 mhucka     (503) staff       (20)     6026 2023-07-18 22:44:45.000000 iga-1.2.0/tests/test_reference.py
--rw-r--r--   0 mhucka     (503) staff       (20)      947 2023-07-18 22:44:45.000000 iga-1.2.0/tests/test_ror.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1375 2023-07-18 22:44:45.000000 iga-1.2.0/tests/test_text_utils.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-07-24 20:28:48.595236 iga-1.2.1/
+-rw-r--r--   0 mhucka     (503) staff       (20)     1527 2023-07-24 19:56:18.000000 iga-1.2.1/LICENSE
+-rw-r--r--   0 mhucka     (503) staff       (20)    41457 2023-07-24 20:28:48.595386 iga-1.2.1/PKG-INFO
+-rw-r--r--   0 mhucka     (503) staff       (20)    40419 2023-07-24 20:27:25.000000 iga-1.2.1/README.md
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-07-24 20:28:48.591553 iga-1.2.1/iga/
+-rw-r--r--   0 mhucka     (503) staff       (20)     1533 2023-07-24 19:56:24.000000 iga-1.2.1/iga/__init__.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      905 2023-07-24 19:56:18.000000 iga-1.2.1/iga/__main__.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    35363 2023-07-24 19:56:18.000000 iga-1.2.1/iga/cli.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3355 2023-07-24 19:56:18.000000 iga-1.2.1/iga/data_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     2855 2023-07-24 19:56:18.000000 iga-1.2.1/iga/doi.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1252 2023-07-24 19:56:18.000000 iga-1.2.1/iga/exceptions.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1514 2023-07-24 19:56:18.000000 iga-1.2.1/iga/exit_codes.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    15499 2023-07-24 19:56:18.000000 iga-1.2.1/iga/github.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     4901 2023-07-24 19:56:18.000000 iga-1.2.1/iga/id_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    19446 2023-07-24 19:56:18.000000 iga-1.2.1/iga/invenio.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     2064 2023-07-24 19:56:18.000000 iga-1.2.1/iga/json_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)   248567 2023-07-24 19:56:18.000000 iga-1.2.1/iga/licenses.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    70406 2023-07-24 19:56:18.000000 iga-1.2.1/iga/metadata.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    14514 2023-07-24 19:56:18.000000 iga-1.2.1/iga/name_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     5273 2023-07-24 19:56:18.000000 iga-1.2.1/iga/orcid.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     5147 2023-07-24 19:56:18.000000 iga-1.2.1/iga/reference.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3969 2023-07-24 19:56:18.000000 iga-1.2.1/iga/ror.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1624 2023-07-24 19:56:18.000000 iga-1.2.1/iga/text_utils.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-07-24 20:28:48.592427 iga-1.2.1/iga.egg-info/
+-rw-r--r--   0 mhucka     (503) staff       (20)    41457 2023-07-24 20:28:48.000000 iga-1.2.1/iga.egg-info/PKG-INFO
+-rw-r--r--   0 mhucka     (503) staff       (20)      930 2023-07-24 20:28:48.000000 iga-1.2.1/iga.egg-info/SOURCES.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-07-24 20:28:48.000000 iga-1.2.1/iga.egg-info/dependency_links.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)       58 2023-07-24 20:28:48.000000 iga-1.2.1/iga.egg-info/entry_points.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-07-24 20:28:48.000000 iga-1.2.1/iga.egg-info/not-zip-safe
+-rw-r--r--   0 mhucka     (503) staff       (20)      659 2023-07-24 20:28:48.000000 iga-1.2.1/iga.egg-info/requires.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        4 2023-07-24 20:28:48.000000 iga-1.2.1/iga.egg-info/top_level.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)     1216 2023-07-24 20:28:48.595730 iga-1.2.1/setup.cfg
+-rwxr-xr-x   0 mhucka     (503) staff       (20)     1548 2023-07-24 19:56:18.000000 iga-1.2.1/setup.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-07-24 20:28:48.595100 iga-1.2.1/tests/
+-rw-r--r--   0 mhucka     (503) staff       (20)     6117 2023-07-24 19:56:18.000000 iga-1.2.1/tests/test_cli.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     4481 2023-07-24 19:56:18.000000 iga-1.2.1/tests/test_data_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1417 2023-07-24 19:56:18.000000 iga-1.2.1/tests/test_doi.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      686 2023-07-24 19:56:18.000000 iga-1.2.1/tests/test_exceptions.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      177 2023-07-24 19:56:18.000000 iga-1.2.1/tests/test_exit_codes.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1446 2023-07-24 19:56:18.000000 iga-1.2.1/tests/test_github.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3015 2023-07-24 19:56:18.000000 iga-1.2.1/tests/test_github_mocks.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3666 2023-07-24 19:56:18.000000 iga-1.2.1/tests/test_id_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      641 2023-07-24 19:56:18.000000 iga-1.2.1/tests/test_init.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    49214 2023-07-24 19:56:18.000000 iga-1.2.1/tests/test_is_person.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      912 2023-07-24 19:56:18.000000 iga-1.2.1/tests/test_licenses.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     4408 2023-07-24 19:56:18.000000 iga-1.2.1/tests/test_name_splitting.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1829 2023-07-24 19:56:18.000000 iga-1.2.1/tests/test_name_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1054 2023-07-24 19:56:18.000000 iga-1.2.1/tests/test_orcid.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     5997 2023-07-24 19:56:18.000000 iga-1.2.1/tests/test_record_from_codemeta.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     6026 2023-07-24 19:56:18.000000 iga-1.2.1/tests/test_reference.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      947 2023-07-24 19:56:18.000000 iga-1.2.1/tests/test_ror.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1375 2023-07-24 19:56:18.000000 iga-1.2.1/tests/test_text_utils.py
```

### Comparing `iga-1.2.0/LICENSE` & `iga-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iga-1.2.0/PKG-INFO` & `iga-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iga
-Version: 1.2.0
+Version: 1.2.1
 Summary: The InvenioRDM GitHub Archiver (IGA) automatically archives GitHub releases in an InvenioRDM repository.
 Home-page: https://github.com/caltechlibrary/iga
 Author: Michael Hucka
 Author-email: mhucka@caltech.edu
 License: https://github.com/caltechlibrary/iga/blob/main/LICENSE
 Project-URL: Source Code, https://github.com/caltechlibrary/iga
 Project-URL: Bug Tracker, https://github.com/caltechlibrary/iga/issues
@@ -27,15 +27,15 @@
 
 IGA is the _InvenioRDM GitHub Archiver_, a standalone program as well as a [GitHub Actions](https://github.com/marketplace/actions/iga) workflow that lets you automatically archive GitHub software releases in an [InvenioRDM](https://inveniosoftware.org/products/rdm/) repository.
 
 [![Latest release](https://img.shields.io/github/v/release/caltechlibrary/iga.svg?style=flat-square&color=b44e88&label=Latest%20release)](https://github.com/caltechlibrary/iga/releases)
 [![License](https://img.shields.io/badge/License-BSD--like-lightgrey.svg?style=flat-square)](https://github.com/caltechlibrary/iga/LICENSE)
 [![Python](https://img.shields.io/badge/Python-3.9+-brightgreen.svg?style=flat-square)](https://www.python.org/downloads/release/python-390/)
 [![PyPI](https://img.shields.io/pypi/v/iga.svg?style=flat-square&color=orange&label=PyPI)](https://pypi.org/project/iga/)
-[![DOI](https://img.shields.io/badge/dynamic/json.svg?label=DOI&style=flat-square&colorA=gray&colorB=navy&query=$.pids.doi.identifier&uri=https://data.caltech.edu/api/records/v0nq3-4a516)](https://data.caltech.edu/records/v0nq3-4a516)
+[![DOI](https://img.shields.io/badge/dynamic/json.svg?label=DOI&style=flat-square&colorA=gray&colorB=navy&query=$.pids.doi.identifier&uri=https://data.caltech.edu/api/records/62htz-vpt80)](https://data.caltech.edu/records/62htz-vpt80)
 
 
 ## Table of contents
 
 * [Introduction](#introduction)
 * [Installation](#installation)
 * [Quick start](#quick-start)
```

### Comparing `iga-1.2.0/README.md` & `iga-1.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 IGA is the _InvenioRDM GitHub Archiver_, a standalone program as well as a [GitHub Actions](https://github.com/marketplace/actions/iga) workflow that lets you automatically archive GitHub software releases in an [InvenioRDM](https://inveniosoftware.org/products/rdm/) repository.
 
 [![Latest release](https://img.shields.io/github/v/release/caltechlibrary/iga.svg?style=flat-square&color=b44e88&label=Latest%20release)](https://github.com/caltechlibrary/iga/releases)
 [![License](https://img.shields.io/badge/License-BSD--like-lightgrey.svg?style=flat-square)](https://github.com/caltechlibrary/iga/LICENSE)
 [![Python](https://img.shields.io/badge/Python-3.9+-brightgreen.svg?style=flat-square)](https://www.python.org/downloads/release/python-390/)
 [![PyPI](https://img.shields.io/pypi/v/iga.svg?style=flat-square&color=orange&label=PyPI)](https://pypi.org/project/iga/)
-[![DOI](https://img.shields.io/badge/dynamic/json.svg?label=DOI&style=flat-square&colorA=gray&colorB=navy&query=$.pids.doi.identifier&uri=https://data.caltech.edu/api/records/v0nq3-4a516)](https://data.caltech.edu/records/v0nq3-4a516)
+[![DOI](https://img.shields.io/badge/dynamic/json.svg?label=DOI&style=flat-square&colorA=gray&colorB=navy&query=$.pids.doi.identifier&uri=https://data.caltech.edu/api/records/62htz-vpt80)](https://data.caltech.edu/records/62htz-vpt80)
 
 
 ## Table of contents
 
 * [Introduction](#introduction)
 * [Installation](#installation)
 * [Quick start](#quick-start)
```

### Comparing `iga-1.2.0/iga/__init__.py` & `iga-1.2.1/iga/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # .............................................................................
 #
 #  ╭────────────────────── Notice ── Notice ── Notice ─────────────────────╮
 #  │    The following values are automatically updated at every release    │
 #  │    by the Makefile. Manual changes to these values will be lost.      │
 #  ╰────────────────────── Notice ── Notice ── Notice ─────────────────────╯
 
-__version__     = '1.2.0'
+__version__     = '1.2.1'
 __description__ = 'The InvenioRDM GitHub Archiver (IGA) automatically archives GitHub releases in an InvenioRDM repository.'
 __url__         = 'https://caltechlibrary.github.io/iga'
 __author__      = 'Michael Hucka'
 __email__       = 'mhucka@caltech.edu'
 __license__     = 'https://github.com/caltechlibrary/iga/blob/main/LICENSE'
```

### Comparing `iga-1.2.0/iga/__main__.py` & `iga-1.2.1/iga/__main__.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.0/iga/cli.py` & `iga-1.2.1/iga/cli.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.0/iga/data_utils.py` & `iga-1.2.1/iga/data_utils.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.0/iga/doi.py` & `iga-1.2.1/iga/doi.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.0/iga/exceptions.py` & `iga-1.2.1/iga/exceptions.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.0/iga/exit_codes.py` & `iga-1.2.1/iga/exit_codes.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.0/iga/github.py` & `iga-1.2.1/iga/github.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.0/iga/id_utils.py` & `iga-1.2.1/iga/id_utils.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.0/iga/invenio.py` & `iga-1.2.1/iga/invenio.py`

 * *Files 1% similar despite different names*

```diff
@@ -280,26 +280,27 @@
     log(f'getting the submission link for community {community} ({community_id})')
     data = {
         "receiver": {"community": community_id},
         "type": "community-submission",
     }
     result = _invenio('put', url=record.review_url, data=data,
                       msg='get community submission link from InvenioRDM')
-    submit_url = record.get('review_url','').replace('/review','/actions/submit-review')
+    submit_url = record.get('review_url', '').replace('/review', '/actions/submit-review')
     data = {
-            'payload': {
-                'format': 'html',
-                'content': f'''This record is being submitted automatically using 
+        'payload': {
+            'format': 'html',
+            'content': f'''This record is being submitted automatically using
                 the InvenioRDM GitHub Archiver (IGA) version
                 {iga.__version__}''',
-            }
         }
+    }
     log(f'submitting the record to community {community}')
     result = _invenio('post', url=submit_url, data=data,
-                          msg='submit record to community {community}')
+                      msg='submit record to community {community}')
+    log(f'result: {result}')
 
 
 def invenio_publish(record):
     '''Tell the InvenioRDM server to publish the record.'''
     log('telling the server to publish the record')
     result = _invenio('post', url=record.publish_url, msg='publish record')
     links = result.get('links', {})
```

### Comparing `iga-1.2.0/iga/json_utils.py` & `iga-1.2.1/iga/json_utils.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.0/iga/licenses.py` & `iga-1.2.1/iga/licenses.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.0/iga/metadata.py` & `iga-1.2.1/iga/metadata.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.0/iga/name_utils.py` & `iga-1.2.1/iga/name_utils.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.0/iga/orcid.py` & `iga-1.2.1/iga/orcid.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.0/iga/reference.py` & `iga-1.2.1/iga/reference.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.0/iga/ror.py` & `iga-1.2.1/iga/ror.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.0/iga/text_utils.py` & `iga-1.2.1/iga/text_utils.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.0/iga.egg-info/PKG-INFO` & `iga-1.2.1/iga.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iga
-Version: 1.2.0
+Version: 1.2.1
 Summary: The InvenioRDM GitHub Archiver (IGA) automatically archives GitHub releases in an InvenioRDM repository.
 Home-page: https://github.com/caltechlibrary/iga
 Author: Michael Hucka
 Author-email: mhucka@caltech.edu
 License: https://github.com/caltechlibrary/iga/blob/main/LICENSE
 Project-URL: Source Code, https://github.com/caltechlibrary/iga
 Project-URL: Bug Tracker, https://github.com/caltechlibrary/iga/issues
@@ -27,15 +27,15 @@
 
 IGA is the _InvenioRDM GitHub Archiver_, a standalone program as well as a [GitHub Actions](https://github.com/marketplace/actions/iga) workflow that lets you automatically archive GitHub software releases in an [InvenioRDM](https://inveniosoftware.org/products/rdm/) repository.
 
 [![Latest release](https://img.shields.io/github/v/release/caltechlibrary/iga.svg?style=flat-square&color=b44e88&label=Latest%20release)](https://github.com/caltechlibrary/iga/releases)
 [![License](https://img.shields.io/badge/License-BSD--like-lightgrey.svg?style=flat-square)](https://github.com/caltechlibrary/iga/LICENSE)
 [![Python](https://img.shields.io/badge/Python-3.9+-brightgreen.svg?style=flat-square)](https://www.python.org/downloads/release/python-390/)
 [![PyPI](https://img.shields.io/pypi/v/iga.svg?style=flat-square&color=orange&label=PyPI)](https://pypi.org/project/iga/)
-[![DOI](https://img.shields.io/badge/dynamic/json.svg?label=DOI&style=flat-square&colorA=gray&colorB=navy&query=$.pids.doi.identifier&uri=https://data.caltech.edu/api/records/v0nq3-4a516)](https://data.caltech.edu/records/v0nq3-4a516)
+[![DOI](https://img.shields.io/badge/dynamic/json.svg?label=DOI&style=flat-square&colorA=gray&colorB=navy&query=$.pids.doi.identifier&uri=https://data.caltech.edu/api/records/62htz-vpt80)](https://data.caltech.edu/records/62htz-vpt80)
 
 
 ## Table of contents
 
 * [Introduction](#introduction)
 * [Installation](#installation)
 * [Quick start](#quick-start)
```

### Comparing `iga-1.2.0/iga.egg-info/SOURCES.txt` & `iga-1.2.1/iga.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iga-1.2.0/iga.egg-info/requires.txt` & `iga-1.2.1/iga.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `iga-1.2.0/setup.cfg` & `iga-1.2.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = iga
-version = 1.2.0
+version = 1.2.1
 description = The InvenioRDM GitHub Archiver (IGA) automatically archives GitHub releases in an InvenioRDM repository.
 author = Michael Hucka
 author_email = mhucka@caltech.edu
 license = https://github.com/caltechlibrary/iga/blob/main/LICENSE
 license_files = LICENSE
 url = https://github.com/caltechlibrary/iga
 project_urls =
```

### Comparing `iga-1.2.0/setup.py` & `iga-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.0/tests/test_cli.py` & `iga-1.2.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.0/tests/test_data_utils.py` & `iga-1.2.1/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.0/tests/test_doi.py` & `iga-1.2.1/tests/test_doi.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.0/tests/test_exceptions.py` & `iga-1.2.1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.0/tests/test_github.py` & `iga-1.2.1/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.0/tests/test_github_mocks.py` & `iga-1.2.1/tests/test_github_mocks.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.0/tests/test_id_utils.py` & `iga-1.2.1/tests/test_id_utils.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.0/tests/test_init.py` & `iga-1.2.1/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.0/tests/test_is_person.py` & `iga-1.2.1/tests/test_is_person.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.0/tests/test_licenses.py` & `iga-1.2.1/tests/test_licenses.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.0/tests/test_name_splitting.py` & `iga-1.2.1/tests/test_name_splitting.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.0/tests/test_name_utils.py` & `iga-1.2.1/tests/test_name_utils.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.0/tests/test_orcid.py` & `iga-1.2.1/tests/test_orcid.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.0/tests/test_record_from_codemeta.py` & `iga-1.2.1/tests/test_record_from_codemeta.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.0/tests/test_reference.py` & `iga-1.2.1/tests/test_reference.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.0/tests/test_ror.py` & `iga-1.2.1/tests/test_ror.py`

 * *Files identical despite different names*

### Comparing `iga-1.2.0/tests/test_text_utils.py` & `iga-1.2.1/tests/test_text_utils.py`

 * *Files identical despite different names*

