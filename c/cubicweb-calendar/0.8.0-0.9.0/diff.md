# Comparing `tmp/cubicweb-calendar-0.8.0.tar.gz` & `tmp/cubicweb-calendar-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cubicweb-calendar-0.8.0.tar", last modified: Thu Jun 25 09:22:52 2015, max compression
+gzip compressed data, was "dist/cubicweb-calendar-0.9.0.tar", last modified: Tue Nov 15 17:22:14 2016, max compression
```

## Comparing `cubicweb-calendar-0.8.0.tar` & `cubicweb-calendar-0.9.0.tar`

### file list

```diff
@@ -1,26 +1,34 @@
-drwxrwxr-x   0 narval     (111) narval     (116)        0 2015-06-25 09:22:52.000000 cubicweb-calendar-0.8.0/
--rw-r--r--   0 narval     (111) narval     (116)     1995 2015-06-25 09:15:53.000000 cubicweb-calendar-0.8.0/schema.py
-drwxrwxr-x   0 narval     (111) narval     (116)        0 2015-06-25 09:22:52.000000 cubicweb-calendar-0.8.0/views/
--rw-r--r--   0 narval     (111) narval     (116)      935 2015-06-25 09:15:53.000000 cubicweb-calendar-0.8.0/views/secondaries.py
--rw-r--r--   0 narval     (111) narval     (116)     3763 2015-06-25 09:15:53.000000 cubicweb-calendar-0.8.0/views/__init__.py
--rw-r--r--   0 narval     (111) narval     (116)     2207 2015-06-25 09:15:53.000000 cubicweb-calendar-0.8.0/views/primaries.py
--rw-r--r--   0 narval     (111) narval     (116)     5669 2015-06-25 09:15:53.000000 cubicweb-calendar-0.8.0/views/main.py
--rw-r--r--   0 narval     (111) narval     (116)      299 2015-06-25 09:15:53.000000 cubicweb-calendar-0.8.0/views/facets.py
--rw-r--r--   0 narval     (111) narval     (116)      200 2015-06-25 09:15:53.000000 cubicweb-calendar-0.8.0/README
--rw-r--r--   0 narval     (111) narval     (116)     1491 2015-06-25 09:15:53.000000 cubicweb-calendar-0.8.0/__pkginfo__.py
--rw-rw-r--   0 narval     (111) narval     (116)      496 2015-06-25 09:22:52.000000 cubicweb-calendar-0.8.0/PKG-INFO
-drwxrwxr-x   0 narval     (111) narval     (116)        0 2015-06-25 09:22:52.000000 cubicweb-calendar-0.8.0/test/
--rw-r--r--   0 narval     (111) narval     (116)      877 2015-06-25 09:15:53.000000 cubicweb-calendar-0.8.0/test/test_calendar.py
--rw-r--r--   0 narval     (111) narval     (116)      238 2015-06-25 09:15:53.000000 cubicweb-calendar-0.8.0/__init__.py
--rw-r--r--   0 narval     (111) narval     (116)     6411 2015-06-25 09:15:53.000000 cubicweb-calendar-0.8.0/setup.py
--rw-r--r--   0 narval     (111) narval     (116)     7668 2015-06-25 09:15:53.000000 cubicweb-calendar-0.8.0/entities.py
-drwxrwxr-x   0 narval     (111) narval     (116)        0 2015-06-25 09:22:52.000000 cubicweb-calendar-0.8.0/i18n/
--rw-r--r--   0 narval     (111) narval     (116)     4689 2015-06-25 09:15:53.000000 cubicweb-calendar-0.8.0/i18n/es.po
--rw-r--r--   0 narval     (111) narval     (116)     6727 2015-06-25 09:15:53.000000 cubicweb-calendar-0.8.0/i18n/fr.po
--rw-r--r--   0 narval     (111) narval     (116)     5695 2015-06-25 09:15:53.000000 cubicweb-calendar-0.8.0/i18n/en.po
-drwxrwxr-x   0 narval     (111) narval     (116)        0 2015-06-25 09:22:52.000000 cubicweb-calendar-0.8.0/data/
--rw-r--r--   0 narval     (111) narval     (116)      616 2015-06-25 09:15:53.000000 cubicweb-calendar-0.8.0/data/office-calendar.png
--rw-r--r--   0 narval     (111) narval     (116)     3861 2015-06-25 09:15:53.000000 cubicweb-calendar-0.8.0/data/cubes.calendar.css
-drwxrwxr-x   0 narval     (111) narval     (116)        0 2015-06-25 09:22:52.000000 cubicweb-calendar-0.8.0/migration/
--rw-r--r--   0 narval     (111) narval     (116)     1932 2015-06-25 09:15:53.000000 cubicweb-calendar-0.8.0/migration/postcreate.py
--rw-r--r--   0 narval     (111) narval     (116)     1356 2015-06-25 09:15:53.000000 cubicweb-calendar-0.8.0/migration/0.4.0_Any.py
+drwxrwxr-x   0 narval     (111) narval     (116)        0 2016-11-15 17:22:14.000000 cubicweb-calendar-0.9.0/
+-rw-r--r--   0 narval     (111) narval     (116)     1995 2016-11-15 17:19:06.000000 cubicweb-calendar-0.9.0/schema.py
+-rw-r--r--   0 narval     (111) narval     (116)      335 2016-11-15 17:19:06.000000 cubicweb-calendar-0.9.0/MANIFEST.in
+-rw-rw-r--   0 narval     (111) narval     (116)       59 2016-11-15 17:22:14.000000 cubicweb-calendar-0.9.0/setup.cfg
+drwxrwxr-x   0 narval     (111) narval     (116)        0 2016-11-15 17:22:14.000000 cubicweb-calendar-0.9.0/views/
+-rw-r--r--   0 narval     (111) narval     (116)      935 2016-11-15 17:19:06.000000 cubicweb-calendar-0.9.0/views/secondaries.py
+-rw-r--r--   0 narval     (111) narval     (116)     3763 2016-11-15 17:19:06.000000 cubicweb-calendar-0.9.0/views/__init__.py
+-rw-r--r--   0 narval     (111) narval     (116)     2207 2016-11-15 17:19:06.000000 cubicweb-calendar-0.9.0/views/primaries.py
+-rw-r--r--   0 narval     (111) narval     (116)     5669 2016-11-15 17:19:06.000000 cubicweb-calendar-0.9.0/views/main.py
+-rw-r--r--   0 narval     (111) narval     (116)      299 2016-11-15 17:19:06.000000 cubicweb-calendar-0.9.0/views/facets.py
+-rw-r--r--   0 narval     (111) narval     (116)      200 2016-11-15 17:19:06.000000 cubicweb-calendar-0.9.0/README
+-rw-r--r--   0 narval     (111) narval     (116)     1491 2016-11-15 17:19:06.000000 cubicweb-calendar-0.9.0/__pkginfo__.py
+-rw-rw-r--   0 narval     (111) narval     (116)      496 2016-11-15 17:22:14.000000 cubicweb-calendar-0.9.0/PKG-INFO
+drwxrwxr-x   0 narval     (111) narval     (116)        0 2016-11-15 17:22:14.000000 cubicweb-calendar-0.9.0/test/
+-rw-r--r--   0 narval     (111) narval     (116)      877 2016-11-15 17:19:06.000000 cubicweb-calendar-0.9.0/test/test_calendar.py
+-rw-r--r--   0 narval     (111) narval     (116)      238 2016-11-15 17:19:06.000000 cubicweb-calendar-0.9.0/__init__.py
+-rw-r--r--   0 narval     (111) narval     (116)     6411 2016-11-15 17:19:06.000000 cubicweb-calendar-0.9.0/setup.py
+-rw-r--r--   0 narval     (111) narval     (116)     7668 2016-11-15 17:19:06.000000 cubicweb-calendar-0.9.0/entities.py
+drwxrwxr-x   0 narval     (111) narval     (116)        0 2016-11-15 17:22:14.000000 cubicweb-calendar-0.9.0/i18n/
+-rw-r--r--   0 narval     (111) narval     (116)     4689 2016-11-15 17:19:06.000000 cubicweb-calendar-0.9.0/i18n/es.po
+-rw-r--r--   0 narval     (111) narval     (116)     6727 2016-11-15 17:19:06.000000 cubicweb-calendar-0.9.0/i18n/fr.po
+-rw-r--r--   0 narval     (111) narval     (116)     5695 2016-11-15 17:19:06.000000 cubicweb-calendar-0.9.0/i18n/en.po
+drwxrwxr-x   0 narval     (111) narval     (116)        0 2016-11-15 17:22:14.000000 cubicweb-calendar-0.9.0/data/
+-rw-r--r--   0 narval     (111) narval     (116)      616 2016-11-15 17:19:06.000000 cubicweb-calendar-0.9.0/data/office-calendar.png
+-rw-r--r--   0 narval     (111) narval     (116)     3831 2016-11-15 17:19:06.000000 cubicweb-calendar-0.9.0/data/cubes.calendar.css
+drwxrwxr-x   0 narval     (111) narval     (116)        0 2016-11-15 17:22:14.000000 cubicweb-calendar-0.9.0/cubicweb_calendar.egg-info/
+-rw-rw-r--   0 narval     (111) narval     (116)        1 2016-11-15 17:22:11.000000 cubicweb-calendar-0.9.0/cubicweb_calendar.egg-info/top_level.txt
+-rw-rw-r--   0 narval     (111) narval     (116)      519 2016-11-15 17:22:11.000000 cubicweb-calendar-0.9.0/cubicweb_calendar.egg-info/SOURCES.txt
+-rw-rw-r--   0 narval     (111) narval     (116)        1 2016-11-15 17:22:11.000000 cubicweb-calendar-0.9.0/cubicweb_calendar.egg-info/dependency_links.txt
+-rw-rw-r--   0 narval     (111) narval     (116)      496 2016-11-15 17:22:11.000000 cubicweb-calendar-0.9.0/cubicweb_calendar.egg-info/PKG-INFO
+-rw-rw-r--   0 narval     (111) narval     (116)       19 2016-11-15 17:22:11.000000 cubicweb-calendar-0.9.0/cubicweb_calendar.egg-info/requires.txt
+drwxrwxr-x   0 narval     (111) narval     (116)        0 2016-11-15 17:22:14.000000 cubicweb-calendar-0.9.0/migration/
+-rw-r--r--   0 narval     (111) narval     (116)     1932 2016-11-15 17:19:06.000000 cubicweb-calendar-0.9.0/migration/postcreate.py
+-rw-r--r--   0 narval     (111) narval     (116)     1356 2016-11-15 17:19:06.000000 cubicweb-calendar-0.9.0/migration/0.4.0_Any.py
```

### Comparing `cubicweb-calendar-0.8.0/schema.py` & `cubicweb-calendar-0.9.0/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-calendar-0.8.0/views/secondaries.py` & `cubicweb-calendar-0.9.0/views/secondaries.py`

 * *Files identical despite different names*

### Comparing `cubicweb-calendar-0.8.0/views/__init__.py` & `cubicweb-calendar-0.9.0/views/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-calendar-0.8.0/views/primaries.py` & `cubicweb-calendar-0.9.0/views/primaries.py`

 * *Files identical despite different names*

### Comparing `cubicweb-calendar-0.8.0/views/main.py` & `cubicweb-calendar-0.9.0/views/main.py`

 * *Files identical despite different names*

### Comparing `cubicweb-calendar-0.8.0/__pkginfo__.py` & `cubicweb-calendar-0.9.0/__pkginfo__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pylint: disable-msg=W0622
 """cubicweb-calendar application packaging information"""
 
 modname = 'calendar'
 distname = 'cubicweb-calendar'
 
-numversion = (0, 8, 0)
+numversion = (0, 9, 0)
 version = '.'.join(str(num) for num in numversion)
 
 license = 'LGPL'
 description = 'calendar component for the CubicWeb framework'
 author = 'Logilab'
 author_email = 'contact@logilab.fr'
 web = 'http://www.cubicweb.org/project/%s' % distname
```

### Comparing `cubicweb-calendar-0.8.0/test/test_calendar.py` & `cubicweb-calendar-0.9.0/test/test_calendar.py`

 * *Files identical despite different names*

### Comparing `cubicweb-calendar-0.8.0/setup.py` & `cubicweb-calendar-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `cubicweb-calendar-0.8.0/entities.py` & `cubicweb-calendar-0.9.0/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-calendar-0.8.0/i18n/es.po` & `cubicweb-calendar-0.9.0/i18n/es.po`

 * *Files identical despite different names*

### Comparing `cubicweb-calendar-0.8.0/i18n/fr.po` & `cubicweb-calendar-0.9.0/i18n/fr.po`

 * *Files identical despite different names*

### Comparing `cubicweb-calendar-0.8.0/i18n/en.po` & `cubicweb-calendar-0.9.0/i18n/en.po`

 * *Files identical despite different names*

### Comparing `cubicweb-calendar-0.8.0/data/office-calendar.png` & `cubicweb-calendar-0.9.0/data/office-calendar.png`

 * *Files identical despite different names*

### Comparing `cubicweb-calendar-0.8.0/data/cubes.calendar.css` & `cubicweb-calendar-0.9.0/data/cubes.calendar.css`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-@import url("cubicweb.css");
-
 /* template specific CSS */
 
 table{
  border-collapse:collapse;
  border: none;
  }
```

### Comparing `cubicweb-calendar-0.8.0/migration/postcreate.py` & `cubicweb-calendar-0.9.0/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-calendar-0.8.0/migration/0.4.0_Any.py` & `cubicweb-calendar-0.9.0/migration/0.4.0_Any.py`

 * *Files identical despite different names*

