# Comparing `tmp/cubicweb-person-1.8.1.tar.gz` & `tmp/cubicweb-person-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cubicweb-person-1.8.1.tar", last modified: Wed Oct 29 15:02:24 2014, max compression
+gzip compressed data, was "dist/cubicweb-person-1.9.0.tar", last modified: Wed Oct 29 15:20:48 2014, max compression
```

## Comparing `cubicweb-person-1.8.1.tar` & `cubicweb-person-1.9.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 narval     (109) narval     (113)        0 2014-10-29 15:02:24.000000 cubicweb-person-1.8.1/
--rw-r--r--   0 narval     (109) narval     (113)     7094 2014-10-29 14:55:22.000000 cubicweb-person-1.8.1/setup.py
-drwxrwxr-x   0 narval     (109) narval     (113)        0 2014-10-29 15:02:24.000000 cubicweb-person-1.8.1/test/
--rw-r--r--   0 narval     (109) narval     (113)      311 2014-10-29 14:55:22.000000 cubicweb-person-1.8.1/test/test_person.py
-drwxrwxr-x   0 narval     (109) narval     (113)        0 2014-10-29 15:02:24.000000 cubicweb-person-1.8.1/migration/
--rw-r--r--   0 narval     (109) narval     (113)       66 2014-10-29 14:55:22.000000 cubicweb-person-1.8.1/migration/postcreate.py
--rw-r--r--   0 narval     (109) narval     (113)      195 2014-10-29 14:55:22.000000 cubicweb-person-1.8.1/migration/1.5.0_Any.py
-drwxrwxr-x   0 narval     (109) narval     (113)        0 2014-10-29 15:02:24.000000 cubicweb-person-1.8.1/data/
--rw-r--r--   0 narval     (109) narval     (113)      388 2014-10-29 14:55:22.000000 cubicweb-person-1.8.1/data/icon_person.gif
--rw-r--r--   0 narval     (109) narval     (113)       22 2014-10-29 14:55:22.000000 cubicweb-person-1.8.1/__init__.py
--rw-rw-r--   0 narval     (109) narval     (113)     2647 2014-10-29 15:02:24.000000 cubicweb-person-1.8.1/PKG-INFO
--rw-r--r--   0 narval     (109) narval     (113)     1886 2014-10-29 14:55:22.000000 cubicweb-person-1.8.1/schema.py
--rw-r--r--   0 narval     (109) narval     (113)     1524 2014-10-29 14:55:22.000000 cubicweb-person-1.8.1/__pkginfo__.py
--rw-r--r--   0 narval     (109) narval     (113)      920 2014-10-29 14:55:22.000000 cubicweb-person-1.8.1/entities.py
--rw-r--r--   0 narval     (109) narval     (113)     1925 2014-10-29 14:55:22.000000 cubicweb-person-1.8.1/README
--rw-r--r--   0 narval     (109) narval     (113)      257 2014-10-29 14:55:22.000000 cubicweb-person-1.8.1/hooks.py
-drwxrwxr-x   0 narval     (109) narval     (113)        0 2014-10-29 15:02:24.000000 cubicweb-person-1.8.1/i18n/
--rw-r--r--   0 narval     (109) narval     (113)     3989 2014-10-29 14:55:22.000000 cubicweb-person-1.8.1/i18n/en.po
--rw-r--r--   0 narval     (109) narval     (113)     4265 2014-10-29 14:55:22.000000 cubicweb-person-1.8.1/i18n/fr.po
--rw-r--r--   0 narval     (109) narval     (113)     4775 2014-10-29 14:55:22.000000 cubicweb-person-1.8.1/views.py
+drwxrwxr-x   0 narval     (109) narval     (113)        0 2014-10-29 15:20:48.000000 cubicweb-person-1.9.0/
+-rw-r--r--   0 narval     (109) narval     (113)     7094 2014-10-29 15:14:35.000000 cubicweb-person-1.9.0/setup.py
+drwxrwxr-x   0 narval     (109) narval     (113)        0 2014-10-29 15:20:48.000000 cubicweb-person-1.9.0/test/
+-rw-r--r--   0 narval     (109) narval     (113)      311 2014-10-29 15:14:35.000000 cubicweb-person-1.9.0/test/test_person.py
+drwxrwxr-x   0 narval     (109) narval     (113)        0 2014-10-29 15:20:48.000000 cubicweb-person-1.9.0/migration/
+-rw-r--r--   0 narval     (109) narval     (113)       66 2014-10-29 15:14:35.000000 cubicweb-person-1.9.0/migration/postcreate.py
+-rw-r--r--   0 narval     (109) narval     (113)      195 2014-10-29 15:14:35.000000 cubicweb-person-1.9.0/migration/1.5.0_Any.py
+drwxrwxr-x   0 narval     (109) narval     (113)        0 2014-10-29 15:20:48.000000 cubicweb-person-1.9.0/data/
+-rw-r--r--   0 narval     (109) narval     (113)      388 2014-10-29 15:14:35.000000 cubicweb-person-1.9.0/data/icon_person.gif
+-rw-r--r--   0 narval     (109) narval     (113)       22 2014-10-29 15:14:35.000000 cubicweb-person-1.9.0/__init__.py
+-rw-rw-r--   0 narval     (109) narval     (113)     2647 2014-10-29 15:20:48.000000 cubicweb-person-1.9.0/PKG-INFO
+-rw-r--r--   0 narval     (109) narval     (113)     1886 2014-10-29 15:14:35.000000 cubicweb-person-1.9.0/schema.py
+-rw-r--r--   0 narval     (109) narval     (113)     1525 2014-10-29 15:14:35.000000 cubicweb-person-1.9.0/__pkginfo__.py
+-rw-r--r--   0 narval     (109) narval     (113)      923 2014-10-29 15:14:35.000000 cubicweb-person-1.9.0/entities.py
+-rw-r--r--   0 narval     (109) narval     (113)     1925 2014-10-29 15:14:35.000000 cubicweb-person-1.9.0/README
+-rw-r--r--   0 narval     (109) narval     (113)      258 2014-10-29 15:14:35.000000 cubicweb-person-1.9.0/hooks.py
+drwxrwxr-x   0 narval     (109) narval     (113)        0 2014-10-29 15:20:48.000000 cubicweb-person-1.9.0/i18n/
+-rw-r--r--   0 narval     (109) narval     (113)     3989 2014-10-29 15:14:35.000000 cubicweb-person-1.9.0/i18n/en.po
+-rw-r--r--   0 narval     (109) narval     (113)     4265 2014-10-29 15:14:35.000000 cubicweb-person-1.9.0/i18n/fr.po
+-rw-r--r--   0 narval     (109) narval     (113)     4776 2014-10-29 15:14:35.000000 cubicweb-person-1.9.0/views.py
```

### Comparing `cubicweb-person-1.8.1/setup.py` & `cubicweb-person-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `cubicweb-person-1.8.1/PKG-INFO` & `cubicweb-person-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: cubicweb-person
-Version: 1.8.1
+Version: 1.9.0
 Summary: person component for the CubicWeb framework
 Home-page: http://www.cubicweb.org/project/cubicweb-person
 Author: Logilab
 Author-email: contact@logilab.fr
 License: LGPL
 Description: Summary
         -------
```

### Comparing `cubicweb-person-1.8.1/schema.py` & `cubicweb-person-1.9.0/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-person-1.8.1/__pkginfo__.py` & `cubicweb-person-1.9.0/__pkginfo__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # pylint: disable-msg=W0622
 """cubicweb-person packaging information"""
 
 modname = 'person'
 distname = "cubicweb-%s" % modname
 
-numversion = (1, 8, 1)
+numversion = (1, 9, 0)
 version = '.'.join(str(num) for num in numversion)
 
 license = 'LGPL'
 description = "person component for the CubicWeb framework"
 author = "Logilab"
 author_email = "contact@logilab.fr"
 web = 'http://www.cubicweb.org/project/%s' % distname
 classifiers = [
     'Environment :: Web Environment',
     'Framework :: CubicWeb',
     'Programming Language :: Python',
     'Programming Language :: JavaScript',
     ]
 
-__depends__ = {'cubicweb': '>= 3.9.0'}
+__depends__ = {'cubicweb': '>= 3.19.0'}
 __recommends__ = {'cubicweb-addressbook': None}
 
 
 # packaging ###
 
 from os import listdir as _listdir
 from os.path import join, isdir
```

### Comparing `cubicweb-person-1.8.1/entities.py` & `cubicweb-person-1.9.0/entities.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 __docformat__ = "restructuredtext en"
 
 from cubicweb.entities import AnyEntity, fetch_config
 
 class Person(AnyEntity):
     """customized class for Person entities"""
     __regid__ = 'Person'
-    fetch_attrs, fetch_order = fetch_config(['surname', 'firstname'])
+    fetch_attrs, cw_fetch_order = fetch_config(['surname', 'firstname'])
     rest_attr = 'surname'
     skip_copy_for = ('primary_email',)
 
     def dc_title(self):
         return self.name()
 
     def dc_long_title(self):
```

### Comparing `cubicweb-person-1.8.1/README` & `cubicweb-person-1.9.0/README`

 * *Files identical despite different names*

### Comparing `cubicweb-person-1.8.1/i18n/en.po` & `cubicweb-person-1.9.0/i18n/en.po`

 * *Files identical despite different names*

### Comparing `cubicweb-person-1.8.1/i18n/fr.po` & `cubicweb-person-1.9.0/i18n/fr.po`

 * *Files identical despite different names*

### Comparing `cubicweb-person-1.8.1/views.py` & `cubicweb-person-1.9.0/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 :contact: http://www.logilab.fr/ -- mailto:contact@logilab.fr
 """
 __docformat__ = "restructuredtext en"
 
 from logilab.mtconverter import xml_escape
 
 from cubicweb.schema import display_name
-from cubicweb.selectors import is_instance, score_entity
-from cubicweb.web import uicfg, action
-from cubicweb.web.views import baseviews, primary, vcard
+from cubicweb.predicates import is_instance, score_entity
+from cubicweb.web import action
+from cubicweb.web.views import baseviews, primary, uicfg, vcard
 from cubicweb.web.facet import AttributeFacet
 
 _pvs =uicfg.primaryview_section
 _pvdc = uicfg.primaryview_display_ctrl
 
 for attr in ('civility', 'firstname', 'surname'):
     _pvs.tag_attribute(('Person', attr), 'hidden')
```

