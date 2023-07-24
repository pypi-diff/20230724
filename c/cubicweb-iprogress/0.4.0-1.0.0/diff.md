# Comparing `tmp/cubicweb-iprogress-0.4.0.tar.gz` & `tmp/cubicweb-iprogress-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-iprogress-0.4.0.tar", last modified: Mon Jul 24 14:00:53 2023, max compression
+gzip compressed data, was "cubicweb-iprogress-1.0.0.tar", last modified: Mon Jul 24 14:21:18 2023, max compression
```

## Comparing `cubicweb-iprogress-0.4.0.tar` & `cubicweb-iprogress-1.0.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:00:53.304613 cubicweb-iprogress-0.4.0/
--rw-rw-rw-   0 root         (0) root         (0)      366 2023-07-24 13:58:15.000000 cubicweb-iprogress-0.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      535 2023-07-24 14:00:53.300613 cubicweb-iprogress-0.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-07-24 13:58:15.000000 cubicweb-iprogress-0.4.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:00:51.896594 cubicweb-iprogress-0.4.0/cubicweb_iprogress/
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-07-24 13:58:15.000000 cubicweb-iprogress-0.4.0/cubicweb_iprogress/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      676 2023-07-24 13:58:15.000000 cubicweb-iprogress-0.4.0/cubicweb_iprogress/__pkginfo__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:00:52.352600 cubicweb-iprogress-0.4.0/cubicweb_iprogress/data/
--rw-rw-rw-   0 root         (0) root         (0)      471 2023-07-24 13:58:15.000000 cubicweb-iprogress-0.4.0/cubicweb_iprogress/data/cubes.iprogress.css
--rw-rw-rw-   0 root         (0) root         (0)     1829 2023-07-24 13:58:15.000000 cubicweb-iprogress-0.4.0/cubicweb_iprogress/data/cubes.iprogress.js
--rw-rw-rw-   0 root         (0) root         (0)     3522 2023-07-24 13:58:15.000000 cubicweb-iprogress-0.4.0/cubicweb_iprogress/entities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:00:52.744605 cubicweb-iprogress-0.4.0/cubicweb_iprogress/i18n/
--rw-rw-rw-   0 root         (0) root         (0)      941 2023-07-24 13:58:15.000000 cubicweb-iprogress-0.4.0/cubicweb_iprogress/i18n/de.po
--rw-rw-rw-   0 root         (0) root         (0)      542 2023-07-24 13:58:15.000000 cubicweb-iprogress-0.4.0/cubicweb_iprogress/i18n/en.po
--rw-rw-rw-   0 root         (0) root         (0)      671 2023-07-24 13:58:15.000000 cubicweb-iprogress-0.4.0/cubicweb_iprogress/i18n/es.po
--rw-rw-rw-   0 root         (0) root         (0)      655 2023-07-24 13:58:15.000000 cubicweb-iprogress-0.4.0/cubicweb_iprogress/i18n/fr.po
--rw-rw-rw-   0 root         (0) root         (0)     9379 2023-07-24 13:58:15.000000 cubicweb-iprogress-0.4.0/cubicweb_iprogress/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:00:52.332600 cubicweb-iprogress-0.4.0/cubicweb_iprogress.egg-info/
--rw-r--r--   0 root         (0) root         (0)      535 2023-07-24 14:00:46.000000 cubicweb-iprogress-0.4.0/cubicweb_iprogress.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      756 2023-07-24 14:00:46.000000 cubicweb-iprogress-0.4.0/cubicweb_iprogress.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 14:00:46.000000 cubicweb-iprogress-0.4.0/cubicweb_iprogress.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-07-24 14:00:46.000000 cubicweb-iprogress-0.4.0/cubicweb_iprogress.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 14:00:46.000000 cubicweb-iprogress-0.4.0/cubicweb_iprogress.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       25 2023-07-24 14:00:46.000000 cubicweb-iprogress-0.4.0/cubicweb_iprogress.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-07-24 14:00:46.000000 cubicweb-iprogress-0.4.0/cubicweb_iprogress.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:00:52.940608 cubicweb-iprogress-0.4.0/debian/
--rw-rw-rw-   0 root         (0) root         (0)      637 2023-07-24 13:58:15.000000 cubicweb-iprogress-0.4.0/debian/changelog
--rw-rw-rw-   0 root         (0) root         (0)        2 2023-07-24 13:58:15.000000 cubicweb-iprogress-0.4.0/debian/compat
--rw-rw-rw-   0 root         (0) root         (0)      712 2023-07-24 13:58:15.000000 cubicweb-iprogress-0.4.0/debian/control
--rw-rw-rw-   0 root         (0) root         (0)      184 2023-07-24 13:58:15.000000 cubicweb-iprogress-0.4.0/debian/copyright
--rw-rw-rw-   0 root         (0) root         (0)       45 2023-07-24 13:58:15.000000 cubicweb-iprogress-0.4.0/debian/rules
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 14:00:53.304613 cubicweb-iprogress-0.4.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2624 2023-07-24 13:58:15.000000 cubicweb-iprogress-0.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:00:53.284613 cubicweb-iprogress-0.4.0/test/
--rw-rw-rw-   0 root         (0) root         (0)      153 2023-07-24 13:58:15.000000 cubicweb-iprogress-0.4.0/test/test_iprogress.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:21:18.888666 cubicweb-iprogress-1.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)      366 2023-07-24 14:20:19.000000 cubicweb-iprogress-1.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      535 2023-07-24 14:21:18.884666 cubicweb-iprogress-1.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-07-24 14:20:19.000000 cubicweb-iprogress-1.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:21:18.876666 cubicweb-iprogress-1.0.0/cubicweb_iprogress/
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-07-24 14:20:19.000000 cubicweb-iprogress-1.0.0/cubicweb_iprogress/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      719 2023-07-24 14:20:19.000000 cubicweb-iprogress-1.0.0/cubicweb_iprogress/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:21:18.880666 cubicweb-iprogress-1.0.0/cubicweb_iprogress/data/
+-rw-rw-rw-   0 root         (0) root         (0)      471 2023-07-24 14:20:19.000000 cubicweb-iprogress-1.0.0/cubicweb_iprogress/data/cubes.iprogress.css
+-rw-rw-rw-   0 root         (0) root         (0)     1829 2023-07-24 14:20:19.000000 cubicweb-iprogress-1.0.0/cubicweb_iprogress/data/cubes.iprogress.js
+-rw-rw-rw-   0 root         (0) root         (0)     3522 2023-07-24 14:20:19.000000 cubicweb-iprogress-1.0.0/cubicweb_iprogress/entities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:21:18.884666 cubicweb-iprogress-1.0.0/cubicweb_iprogress/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)      941 2023-07-24 14:20:19.000000 cubicweb-iprogress-1.0.0/cubicweb_iprogress/i18n/de.po
+-rw-rw-rw-   0 root         (0) root         (0)      542 2023-07-24 14:20:19.000000 cubicweb-iprogress-1.0.0/cubicweb_iprogress/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)      671 2023-07-24 14:20:19.000000 cubicweb-iprogress-1.0.0/cubicweb_iprogress/i18n/es.po
+-rw-rw-rw-   0 root         (0) root         (0)      655 2023-07-24 14:20:19.000000 cubicweb-iprogress-1.0.0/cubicweb_iprogress/i18n/fr.po
+-rw-rw-rw-   0 root         (0) root         (0)     9379 2023-07-24 14:20:19.000000 cubicweb-iprogress-1.0.0/cubicweb_iprogress/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:21:18.880666 cubicweb-iprogress-1.0.0/cubicweb_iprogress.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      535 2023-07-24 14:21:18.000000 cubicweb-iprogress-1.0.0/cubicweb_iprogress.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      756 2023-07-24 14:21:18.000000 cubicweb-iprogress-1.0.0/cubicweb_iprogress.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 14:21:18.000000 cubicweb-iprogress-1.0.0/cubicweb_iprogress.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-07-24 14:21:18.000000 cubicweb-iprogress-1.0.0/cubicweb_iprogress.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 14:21:18.000000 cubicweb-iprogress-1.0.0/cubicweb_iprogress.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       50 2023-07-24 14:21:18.000000 cubicweb-iprogress-1.0.0/cubicweb_iprogress.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-24 14:21:18.000000 cubicweb-iprogress-1.0.0/cubicweb_iprogress.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:21:18.884666 cubicweb-iprogress-1.0.0/debian/
+-rw-rw-rw-   0 root         (0) root         (0)      637 2023-07-24 14:20:19.000000 cubicweb-iprogress-1.0.0/debian/changelog
+-rw-rw-rw-   0 root         (0) root         (0)        2 2023-07-24 14:20:19.000000 cubicweb-iprogress-1.0.0/debian/compat
+-rw-rw-rw-   0 root         (0) root         (0)      712 2023-07-24 14:20:19.000000 cubicweb-iprogress-1.0.0/debian/control
+-rw-rw-rw-   0 root         (0) root         (0)      184 2023-07-24 14:20:19.000000 cubicweb-iprogress-1.0.0/debian/copyright
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-07-24 14:20:19.000000 cubicweb-iprogress-1.0.0/debian/rules
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 14:21:18.888666 cubicweb-iprogress-1.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2624 2023-07-24 14:20:19.000000 cubicweb-iprogress-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:21:18.884666 cubicweb-iprogress-1.0.0/test/
+-rw-rw-rw-   0 root         (0) root         (0)      153 2023-07-24 14:20:19.000000 cubicweb-iprogress-1.0.0/test/test_iprogress.py
```

### Comparing `cubicweb-iprogress-0.4.0/PKG-INFO` & `cubicweb-iprogress-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubicweb-iprogress
-Version: 0.4.0
+Version: 1.0.0
 Summary: some adapters and view for stuff progressing to reach a milestone
 Home-page: http://www.cubicweb.org/project/cubicweb-iprogress
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
```

### Comparing `cubicweb-iprogress-0.4.0/cubicweb_iprogress/__pkginfo__.py` & `cubicweb-iprogress-1.0.0/cubicweb_iprogress/__pkginfo__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 # pylint: disable=W0622
 """cubicweb-iprogress application packaging information"""
 
 modname = "iprogress"
 distname = "cubicweb-iprogress"
 
-numversion = (0, 4, 0)
+numversion = (1, 0, 0)
 version = ".".join(str(num) for num in numversion)
 
 license = "LGPL"
 author = "LOGILAB S.A. (Paris, FRANCE)"
 author_email = "contact@logilab.fr"
 description = "some adapters and view for stuff progressing to reach a milestone"
 web = "http://www.cubicweb.org/project/%s" % distname
 classifiers = [
     "Environment :: Web Environment",
     "Framework :: CubicWeb",
     "Programming Language :: Python",
     "Programming Language :: JavaScript",
 ]
 
-__depends__ = {"cubicweb": ">=3.38.0,<3.39.0"}
+__depends__ = {
+    "cubicweb": ">=4.0.0,<5.0.0",
+    "cubicweb-web": ">=1.0.0,<2.0.0",
+}
 __recommends__ = {}
```

### Comparing `cubicweb-iprogress-0.4.0/cubicweb_iprogress/data/cubes.iprogress.js` & `cubicweb-iprogress-1.0.0/cubicweb_iprogress/data/cubes.iprogress.js`

 * *Files identical despite different names*

### Comparing `cubicweb-iprogress-0.4.0/cubicweb_iprogress/entities.py` & `cubicweb-iprogress-1.0.0/cubicweb_iprogress/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-iprogress-0.4.0/cubicweb_iprogress/i18n/de.po` & `cubicweb-iprogress-1.0.0/cubicweb_iprogress/i18n/de.po`

 * *Files identical despite different names*

### Comparing `cubicweb-iprogress-0.4.0/cubicweb_iprogress/i18n/en.po` & `cubicweb-iprogress-1.0.0/cubicweb_iprogress/i18n/en.po`

 * *Files identical despite different names*

### Comparing `cubicweb-iprogress-0.4.0/cubicweb_iprogress/i18n/es.po` & `cubicweb-iprogress-1.0.0/cubicweb_iprogress/i18n/es.po`

 * *Files identical despite different names*

### Comparing `cubicweb-iprogress-0.4.0/cubicweb_iprogress/i18n/fr.po` & `cubicweb-iprogress-1.0.0/cubicweb_iprogress/i18n/fr.po`

 * *Files identical despite different names*

### Comparing `cubicweb-iprogress-0.4.0/cubicweb_iprogress/views.py` & `cubicweb-iprogress-1.0.0/cubicweb_iprogress/views.py`

 * *Files identical despite different names*

### Comparing `cubicweb-iprogress-0.4.0/cubicweb_iprogress.egg-info/PKG-INFO` & `cubicweb-iprogress-1.0.0/cubicweb_iprogress.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubicweb-iprogress
-Version: 0.4.0
+Version: 1.0.0
 Summary: some adapters and view for stuff progressing to reach a milestone
 Home-page: http://www.cubicweb.org/project/cubicweb-iprogress
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
```

### Comparing `cubicweb-iprogress-0.4.0/cubicweb_iprogress.egg-info/SOURCES.txt` & `cubicweb-iprogress-1.0.0/cubicweb_iprogress.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-iprogress-0.4.0/debian/changelog` & `cubicweb-iprogress-1.0.0/debian/changelog`

 * *Files identical despite different names*

### Comparing `cubicweb-iprogress-0.4.0/debian/control` & `cubicweb-iprogress-1.0.0/debian/control`

 * *Files identical despite different names*

### Comparing `cubicweb-iprogress-0.4.0/setup.py` & `cubicweb-iprogress-1.0.0/setup.py`

 * *Files identical despite different names*

