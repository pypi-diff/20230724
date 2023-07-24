# Comparing `tmp/cubicweb-prometheus-0.4.0.tar.gz` & `tmp/cubicweb-prometheus-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-prometheus-0.4.0.tar", last modified: Thu Mar  2 13:55:47 2023, max compression
+gzip compressed data, was "cubicweb-prometheus-0.5.0.tar", last modified: Mon Jul 24 14:04:37 2023, max compression
```

## Comparing `cubicweb-prometheus-0.4.0.tar` & `cubicweb-prometheus-0.5.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 13:55:47.286726 cubicweb-prometheus-0.4.0/
--rw-rw-rw-   0 root         (0) root         (0)      918 2023-03-02 13:55:15.000000 cubicweb-prometheus-0.4.0/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)      443 2023-03-02 13:55:15.000000 cubicweb-prometheus-0.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1062 2023-03-02 13:55:47.286726 cubicweb-prometheus-0.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      573 2023-03-02 13:55:15.000000 cubicweb-prometheus-0.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 13:55:47.282726 cubicweb-prometheus-0.4.0/cubicweb_prometheus/
--rw-rw-rw-   0 root         (0) root         (0)      131 2023-03-02 13:55:15.000000 cubicweb-prometheus-0.4.0/cubicweb_prometheus/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      713 2023-03-02 13:55:15.000000 cubicweb-prometheus-0.4.0/cubicweb_prometheus/__pkginfo__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 13:55:47.282726 cubicweb-prometheus-0.4.0/cubicweb_prometheus/i18n/
--rw-rw-rw-   0 root         (0) root         (0)      248 2023-03-02 13:55:15.000000 cubicweb-prometheus-0.4.0/cubicweb_prometheus/i18n/en.po
--rw-rw-rw-   0 root         (0) root         (0)      248 2023-03-02 13:55:15.000000 cubicweb-prometheus-0.4.0/cubicweb_prometheus/i18n/es.po
--rw-rw-rw-   0 root         (0) root         (0)      248 2023-03-02 13:55:15.000000 cubicweb-prometheus-0.4.0/cubicweb_prometheus/i18n/fr.po
--rw-rw-rw-   0 root         (0) root         (0)     7169 2023-03-02 13:55:15.000000 cubicweb-prometheus-0.4.0/cubicweb_prometheus/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 13:55:47.282726 cubicweb-prometheus-0.4.0/cubicweb_prometheus.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1062 2023-03-02 13:55:45.000000 cubicweb-prometheus-0.4.0/cubicweb_prometheus.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      592 2023-03-02 13:55:47.000000 cubicweb-prometheus-0.4.0/cubicweb_prometheus.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-02 13:55:45.000000 cubicweb-prometheus-0.4.0/cubicweb_prometheus.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2023-03-02 13:55:46.000000 cubicweb-prometheus-0.4.0/cubicweb_prometheus.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-02 13:55:45.000000 cubicweb-prometheus-0.4.0/cubicweb_prometheus.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       59 2023-03-02 13:55:46.000000 cubicweb-prometheus-0.4.0/cubicweb_prometheus.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-03-02 13:55:46.000000 cubicweb-prometheus-0.4.0/cubicweb_prometheus.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-02 13:55:47.286726 cubicweb-prometheus-0.4.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2756 2023-03-02 13:55:15.000000 cubicweb-prometheus-0.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 13:55:47.282726 cubicweb-prometheus-0.4.0/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 13:55:47.286726 cubicweb-prometheus-0.4.0/test/data/
--rw-rw-rw-   0 root         (0) root         (0)       11 2023-03-02 13:55:15.000000 cubicweb-prometheus-0.4.0/test/data/bootstrap_cubes
--rw-rw-rw-   0 root         (0) root         (0)     1708 2023-03-02 13:55:15.000000 cubicweb-prometheus-0.4.0/test/test_prometheus.py
--rw-rw-rw-   0 root         (0) root         (0)     1181 2023-03-02 13:55:15.000000 cubicweb-prometheus-0.4.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:04:37.786119 cubicweb-prometheus-0.5.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-07-24 14:04:18.000000 cubicweb-prometheus-0.5.0/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)      443 2023-07-24 14:04:18.000000 cubicweb-prometheus-0.5.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-07-24 14:04:37.786119 cubicweb-prometheus-0.5.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      573 2023-07-24 14:04:18.000000 cubicweb-prometheus-0.5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:04:37.782119 cubicweb-prometheus-0.5.0/cubicweb_prometheus/
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-07-24 14:04:18.000000 cubicweb-prometheus-0.5.0/cubicweb_prometheus/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      711 2023-07-24 14:04:18.000000 cubicweb-prometheus-0.5.0/cubicweb_prometheus/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:04:37.786119 cubicweb-prometheus-0.5.0/cubicweb_prometheus/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)      248 2023-07-24 14:04:18.000000 cubicweb-prometheus-0.5.0/cubicweb_prometheus/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)      248 2023-07-24 14:04:18.000000 cubicweb-prometheus-0.5.0/cubicweb_prometheus/i18n/es.po
+-rw-rw-rw-   0 root         (0) root         (0)      248 2023-07-24 14:04:18.000000 cubicweb-prometheus-0.5.0/cubicweb_prometheus/i18n/fr.po
+-rw-rw-rw-   0 root         (0) root         (0)     7169 2023-07-24 14:04:19.000000 cubicweb-prometheus-0.5.0/cubicweb_prometheus/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:04:37.786119 cubicweb-prometheus-0.5.0/cubicweb_prometheus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-07-24 14:04:37.000000 cubicweb-prometheus-0.5.0/cubicweb_prometheus.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      592 2023-07-24 14:04:37.000000 cubicweb-prometheus-0.5.0/cubicweb_prometheus.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 14:04:37.000000 cubicweb-prometheus-0.5.0/cubicweb_prometheus.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2023-07-24 14:04:37.000000 cubicweb-prometheus-0.5.0/cubicweb_prometheus.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 14:04:37.000000 cubicweb-prometheus-0.5.0/cubicweb_prometheus.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       57 2023-07-24 14:04:37.000000 cubicweb-prometheus-0.5.0/cubicweb_prometheus.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-24 14:04:37.000000 cubicweb-prometheus-0.5.0/cubicweb_prometheus.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 14:04:37.786119 cubicweb-prometheus-0.5.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2740 2023-07-24 14:04:19.000000 cubicweb-prometheus-0.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:04:37.786119 cubicweb-prometheus-0.5.0/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:04:37.786119 cubicweb-prometheus-0.5.0/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)       11 2023-07-24 14:04:19.000000 cubicweb-prometheus-0.5.0/test/data/bootstrap_cubes
+-rw-rw-rw-   0 root         (0) root         (0)     1708 2023-07-24 14:04:19.000000 cubicweb-prometheus-0.5.0/test/test_prometheus.py
+-rw-rw-rw-   0 root         (0) root         (0)     1181 2023-07-24 14:04:19.000000 cubicweb-prometheus-0.5.0/tox.ini
```

### Comparing `cubicweb-prometheus-0.4.0/CHANGELOG.md` & `cubicweb-prometheus-0.5.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+## Version 0.5.0 (2023-07-24)
+### 🎉 New features
+
+- run flynt on the code base to convert everything into f-strings
+- upgrade CubicWeb version to 4
+
+### 🤖 Continuous integration
+
+- that tox option is now named allowlist_externals
+
 ## Version 0.4.0 (2023-03-02)
 ### 🎉 New features
 
 - pkginfo: upgrade cubicweb to ">=3.38.0,<3.39.0"
 - pkginfo: upgrade prometheus-client to ">=0.16.0,<0.17.0"
 - run pyupgrade
 
@@ -42,8 +52,8 @@
 ## Version 0.1.2 (2021-05-11)
 
 - packaging
 
 ## Version 0.1.1 (2021-05-11)
 ### 🤷 Various changes
 
-- First working version
+- First working version
```

### Comparing `cubicweb-prometheus-0.4.0/PKG-INFO` & `cubicweb-prometheus-0.5.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: cubicweb-prometheus
-Version: 0.4.0
+Version: 0.5.0
 Summary: Exporting prometheus metrics
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/prometheus
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: JavaScript
 Description-Content-Type: text/markdown
 
 Summary
@@ -34,9 +33,7 @@
 prometheus.pyramid.count_routes = True
 
 prometheus.cubicweb.sql.time = Histogram
 prometheus.cubicweb.rql.time = Histogram
 ...
 ```
 
-
-
```

### Comparing `cubicweb-prometheus-0.4.0/README.md` & `cubicweb-prometheus-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `cubicweb-prometheus-0.4.0/cubicweb_prometheus/__pkginfo__.py` & `cubicweb-prometheus-0.5.0/cubicweb_prometheus/__pkginfo__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # pylint: disable=W0622
 """cubicweb-prometheus application packaging information"""
 
 
 modname = "cubicweb_prometheus"
 distname = "cubicweb-prometheus"
 
-numversion = (0, 4, 0)
+numversion = (0, 5, 0)
 version = ".".join(str(num) for num in numversion)
 
 license = "LGPL"
 author = "LOGILAB S.A. (Paris, FRANCE)"
 author_email = "contact@logilab.fr"
 description = "Exporting prometheus metrics"
 web = "https://forge.extranet.logilab.fr/cubicweb/cubes/prometheus"
 
-__depends__ = {"cubicweb": ">=3.38.0,<3.39.0", "prometheus-client": ">=0.16.0,<0.17.0"}
+__depends__ = {"cubicweb": ">=4.0.0,<5.0.0", "prometheus-client": ">=0.16.0,<0.17.0"}
 __recommends__ = {}
 
 classifiers = [
     "Environment :: Web Environment",
     "Framework :: CubicWeb",
     "Programming Language :: Python :: 3",
     "Programming Language :: JavaScript",
```

### Comparing `cubicweb-prometheus-0.4.0/cubicweb_prometheus/views.py` & `cubicweb-prometheus-0.5.0/cubicweb_prometheus/views.py`

 * *Files identical despite different names*

### Comparing `cubicweb-prometheus-0.4.0/cubicweb_prometheus.egg-info/PKG-INFO` & `cubicweb-prometheus-0.5.0/cubicweb_prometheus.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: cubicweb-prometheus
-Version: 0.4.0
+Version: 0.5.0
 Summary: Exporting prometheus metrics
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/prometheus
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: JavaScript
 Description-Content-Type: text/markdown
 
 Summary
@@ -34,9 +33,7 @@
 prometheus.pyramid.count_routes = True
 
 prometheus.cubicweb.sql.time = Histogram
 prometheus.cubicweb.rql.time = Histogram
 ...
 ```
 
-
-
```

### Comparing `cubicweb-prometheus-0.4.0/cubicweb_prometheus.egg-info/SOURCES.txt` & `cubicweb-prometheus-0.5.0/cubicweb_prometheus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-prometheus-0.4.0/setup.py` & `cubicweb-prometheus-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,17 +54,15 @@
 # get optional metadatas
 data_files = __pkginfo__.get("data_files", None)
 dependency_links = __pkginfo__.get("dependency_links", ())
 
 requires = {}
 for entry in ("__depends__",):  # "__recommends__"):
     requires.update(__pkginfo__.get(entry, {}))
-install_requires = [
-    "{} {}".format(d, v and v or "").strip() for d, v in requires.items()
-]
+install_requires = [f"{d} {v and v or ''}".strip() for d, v in requires.items()]
 
 
 setup(
     name=distname,
     version=version,
     license=license,
     description=description,
```

### Comparing `cubicweb-prometheus-0.4.0/test/test_prometheus.py` & `cubicweb-prometheus-0.5.0/test/test_prometheus.py`

 * *Files identical despite different names*

### Comparing `cubicweb-prometheus-0.4.0/tox.ini` & `cubicweb-prometheus-0.5.0/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 deps =
   black >= 22.12
 commands = black .
 
 [testenv:pypi-publish]
 basepython = python3
 skip_install = true
-whitelist_externals = rm
+allowlist_externals = rm
 deps =
   twine
 passenv =
   TWINE_USERNAME
   TWINE_PASSWORD
 commands =
   rm -rf build dist .egg .egg-info
```

