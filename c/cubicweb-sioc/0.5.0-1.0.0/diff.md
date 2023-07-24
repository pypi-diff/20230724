# Comparing `tmp/cubicweb-sioc-0.5.0.tar.gz` & `tmp/cubicweb-sioc-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-sioc-0.5.0.tar", last modified: Thu Nov 24 01:28:34 2022, max compression
+gzip compressed data, was "cubicweb-sioc-1.0.0.tar", last modified: Mon Jul 24 15:18:23 2023, max compression
```

## Comparing `cubicweb-sioc-0.5.0.tar` & `cubicweb-sioc-1.0.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 01:28:34.865703 cubicweb-sioc-0.5.0/
--rw-rw-rw-   0 root         (0) root         (0)      382 2022-11-24 01:28:09.000000 cubicweb-sioc-0.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      478 2022-11-24 01:28:34.865703 cubicweb-sioc-0.5.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       86 2022-11-24 01:28:09.000000 cubicweb-sioc-0.5.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 01:28:34.861703 cubicweb-sioc-0.5.0/cubicweb_sioc/
--rw-rw-rw-   0 root         (0) root         (0)      112 2022-11-24 01:28:09.000000 cubicweb-sioc-0.5.0/cubicweb_sioc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      635 2022-11-24 01:28:09.000000 cubicweb-sioc-0.5.0/cubicweb_sioc/__pkginfo__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 01:28:34.861703 cubicweb-sioc-0.5.0/cubicweb_sioc/i18n/
--rw-rw-rw-   0 root         (0) root         (0)      203 2022-11-24 01:28:09.000000 cubicweb-sioc-0.5.0/cubicweb_sioc/i18n/en.po
--rw-rw-rw-   0 root         (0) root         (0)      203 2022-11-24 01:28:09.000000 cubicweb-sioc-0.5.0/cubicweb_sioc/i18n/es.po
--rw-rw-rw-   0 root         (0) root         (0)      203 2022-11-24 01:28:09.000000 cubicweb-sioc-0.5.0/cubicweb_sioc/i18n/fr.po
--rw-rw-rw-   0 root         (0) root         (0)       76 2022-11-24 01:28:09.000000 cubicweb-sioc-0.5.0/cubicweb_sioc/site_cubicweb.py
--rw-rw-rw-   0 root         (0) root         (0)     5885 2022-11-24 01:28:09.000000 cubicweb-sioc-0.5.0/cubicweb_sioc/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 01:28:34.861703 cubicweb-sioc-0.5.0/cubicweb_sioc.egg-info/
--rw-r--r--   0 root         (0) root         (0)      478 2022-11-24 01:28:33.000000 cubicweb-sioc-0.5.0/cubicweb_sioc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      527 2022-11-24 01:28:34.000000 cubicweb-sioc-0.5.0/cubicweb_sioc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-24 01:28:33.000000 cubicweb-sioc-0.5.0/cubicweb_sioc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-24 01:28:34.000000 cubicweb-sioc-0.5.0/cubicweb_sioc.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-24 01:28:33.000000 cubicweb-sioc-0.5.0/cubicweb_sioc.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       36 2022-11-24 01:28:34.000000 cubicweb-sioc-0.5.0/cubicweb_sioc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2022-11-24 01:28:34.000000 cubicweb-sioc-0.5.0/cubicweb_sioc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-24 01:28:34.865703 cubicweb-sioc-0.5.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2556 2022-11-24 01:28:09.000000 cubicweb-sioc-0.5.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 01:28:34.861703 cubicweb-sioc-0.5.0/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 01:28:34.865703 cubicweb-sioc-0.5.0/test/data/
--rw-rw-rw-   0 root         (0) root         (0)        5 2022-11-24 01:28:09.000000 cubicweb-sioc-0.5.0/test/data/bootstrap_cubes
--rw-rw-rw-   0 root         (0) root         (0)     1734 2022-11-24 01:28:09.000000 cubicweb-sioc-0.5.0/test/test_sioc.py
--rw-rw-rw-   0 root         (0) root         (0)     1422 2022-11-24 01:28:09.000000 cubicweb-sioc-0.5.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:18:23.609769 cubicweb-sioc-1.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-07-24 15:18:05.000000 cubicweb-sioc-1.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      458 2023-07-24 15:18:23.609769 cubicweb-sioc-1.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       86 2023-07-24 15:18:05.000000 cubicweb-sioc-1.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:18:23.605769 cubicweb-sioc-1.0.0/cubicweb_sioc/
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-07-24 15:18:05.000000 cubicweb-sioc-1.0.0/cubicweb_sioc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      672 2023-07-24 15:18:05.000000 cubicweb-sioc-1.0.0/cubicweb_sioc/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:18:23.609769 cubicweb-sioc-1.0.0/cubicweb_sioc/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)      203 2023-07-24 15:18:05.000000 cubicweb-sioc-1.0.0/cubicweb_sioc/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)      203 2023-07-24 15:18:05.000000 cubicweb-sioc-1.0.0/cubicweb_sioc/i18n/es.po
+-rw-rw-rw-   0 root         (0) root         (0)      203 2023-07-24 15:18:05.000000 cubicweb-sioc-1.0.0/cubicweb_sioc/i18n/fr.po
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-07-24 15:18:05.000000 cubicweb-sioc-1.0.0/cubicweb_sioc/site_cubicweb.py
+-rw-rw-rw-   0 root         (0) root         (0)     5699 2023-07-24 15:18:05.000000 cubicweb-sioc-1.0.0/cubicweb_sioc/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:18:23.609769 cubicweb-sioc-1.0.0/cubicweb_sioc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      458 2023-07-24 15:18:23.000000 cubicweb-sioc-1.0.0/cubicweb_sioc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      527 2023-07-24 15:18:23.000000 cubicweb-sioc-1.0.0/cubicweb_sioc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 15:18:23.000000 cubicweb-sioc-1.0.0/cubicweb_sioc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 15:18:23.000000 cubicweb-sioc-1.0.0/cubicweb_sioc.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 15:18:23.000000 cubicweb-sioc-1.0.0/cubicweb_sioc.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       61 2023-07-24 15:18:23.000000 cubicweb-sioc-1.0.0/cubicweb_sioc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-24 15:18:23.000000 cubicweb-sioc-1.0.0/cubicweb_sioc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 15:18:23.613769 cubicweb-sioc-1.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2538 2023-07-24 15:18:05.000000 cubicweb-sioc-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:18:23.609769 cubicweb-sioc-1.0.0/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:18:23.609769 cubicweb-sioc-1.0.0/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)        5 2023-07-24 15:18:05.000000 cubicweb-sioc-1.0.0/test/data/bootstrap_cubes
+-rw-rw-rw-   0 root         (0) root         (0)     1734 2023-07-24 15:18:05.000000 cubicweb-sioc-1.0.0/test/test_sioc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1418 2023-07-24 15:18:05.000000 cubicweb-sioc-1.0.0/tox.ini
```

### Comparing `cubicweb-sioc-0.5.0/cubicweb_sioc/__pkginfo__.py` & `cubicweb-sioc-1.0.0/cubicweb_sioc/__pkginfo__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # pylint: disable=W0622
 """cubicweb-sioc application packaging information"""
 
 modname = "sioc"
 distname = "cubicweb-sioc"
 
-numversion = (0, 5, 0)
+numversion = (1, 0, 0)
 version = ".".join(str(num) for num in numversion)
 
 license = "LGPL"
 author = "LOGILAB S.A. (Paris, FRANCE)"
 author_email = "contact@logilab.fr"
 description = "Specific views for SIOC (Semantically-Interlinked Online Communities)"
-web = "https://forge.extranet.logilab.fr/cubicweb/cubes/%s" % distname
+web = f"https://forge.extranet.logilab.fr/cubicweb/cubes/{distname}"
 classifiers = [
     "Framework :: CubicWeb",
     "Programming Language :: Python",
 ]
 
 __depends__ = {
-    "cubicweb": ">= 3.38.0, < 3.39.0",
+    "cubicweb": ">= 4.0.0, < 5.0.0",
+    "cubicweb-web": ">= 1.0.0, < 2.0.0",
     "six": ">= 1.4.0",
 }
 __recommends__ = {}
```

### Comparing `cubicweb-sioc-0.5.0/cubicweb_sioc/views.py` & `cubicweb-sioc-1.0.0/cubicweb_sioc/views.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # copyright 2012-2022 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
@@ -22,15 +21,14 @@
 
 __docformat__ = "restructuredtext en"
 try:
     from cubicweb import _
 except ImportError:
     _ = str
 
-from six.moves import range
 
 from logilab.mtconverter import xml_escape
 
 from cubicweb_web.view import EntityView, EntityAdapter
 from cubicweb.predicates import adaptable
 
 
@@ -82,15 +80,15 @@
     __regid__ = "sioc"
     __select__ = adaptable("ISIOCItem", "ISIOCContainer")
     title = _("sioc")
     templatable = False
     content_type = "text/xml"
 
     def call(self):
-        self.w('<?xml version="1.0" encoding="%s"?>\n' % self._cw.encoding)
+        self.w(f'<?xml version="1.0" encoding="{self._cw.encoding}"?>\n')
         self.w(
             """<rdf:RDF
              xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#"
              xmlns:rdfs="http://www.w3.org/2000/01/rdf-schema#"
              xmlns:owl="http://www.w3.org/2002/07/owl#"
              xmlns:foaf="http://xmlns.com/foaf/0.1/"
              xmlns:sioc="http://rdfs.org/sioc/ns#"
@@ -111,64 +109,55 @@
     templatable = False
     content_type = "text/xml"
 
     def cell_call(self, row, col):
         entity = self.cw_rset.complete_entity(row, col)
         isioc = entity.cw_adapt_to("ISIOCContainer")
         isioct = isioc.isioc_type()
-        self.w(
-            '<sioc:%s rdf:about="%s">\n' % (isioct, xml_escape(entity.absolute_url()))
-        )
-        self.w("<dcterms:title>%s</dcterms:title>" % xml_escape(entity.dc_title()))
-        self.w(
-            "<dcterms:created>%s</dcterms:created>" % entity.creation_date.isoformat()
-        )
+        self.w(f'<sioc:{isioct} rdf:about="{xml_escape(entity.absolute_url())}">\n')
+        self.w(f"<dcterms:title>{xml_escape(entity.dc_title())}</dcterms:title>")
+        self.w(f"<dcterms:created>{entity.creation_date.isoformat()}</dcterms:created>")
         self.w(
             "<dcterms:modified>%s</dcterms:modified>"
             % entity.modification_date.isoformat()
         )
         self.w("<!-- FIXME : here be items -->")  # entity.isioc_items()
-        self.w("</sioc:%s>\n" % isioct)
+        self.w(f"</sioc:{isioct}>\n")
 
 
 class SIOCItemView(EntityView):
     __regid__ = "sioc_element"
     __select__ = adaptable("ISIOCItem")
     templatable = False
     content_type = "text/xml"
 
     def cell_call(self, row, col):
         entity = self.cw_rset.complete_entity(row, col)
         isioc = entity.cw_adapt_to("ISIOCItem")
         isioct = isioc.isioc_type()
-        self.w(
-            '<sioc:%s rdf:about="%s">\n' % (isioct, xml_escape(entity.absolute_url()))
-        )
-        self.w("<dcterms:title>%s</dcterms:title>" % xml_escape(entity.dc_title()))
-        self.w(
-            "<dcterms:created>%s</dcterms:created>" % entity.creation_date.isoformat()
-        )
+        self.w(f'<sioc:{isioct} rdf:about="{xml_escape(entity.absolute_url())}">\n')
+        self.w(f"<dcterms:title>{xml_escape(entity.dc_title())}</dcterms:title>")
+        self.w(f"<dcterms:created>{entity.creation_date.isoformat()}</dcterms:created>")
         self.w(
             "<dcterms:modified>%s</dcterms:modified>"
             % entity.modification_date.isoformat()
         )
         content = isioc.isioc_content()
         if content:
-            self.w("<sioc:content>%s</sioc:content>" % xml_escape(content))
+            self.w(f"<sioc:content>{xml_escape(content)}</sioc:content>")
         container = isioc.isioc_container()
         if container:
             self.w(
                 '<sioc:has_container rdf:resource="%s"/>\n'
                 % xml_escape(container.absolute_url())
             )
         if entity.creator:
             self.w("<sioc:has_creator>\n")
             self.w(
-                '<sioc:User rdf:about="%s">\n'
-                % xml_escape(entity.creator.absolute_url())
+                f'<sioc:User rdf:about="{xml_escape(entity.creator.absolute_url())}">\n'
             )
             self.w(entity.creator.view("foaf"))
             self.w("</sioc:User>\n")
             self.w("</sioc:has_creator>\n")
         self.w("<!-- FIXME : here be topics -->")  # entity.isioc_topics()
         self.w("<!-- FIXME : here be replies -->")  # entity.isioc_replies()
-        self.w(" </sioc:%s>\n" % isioct)
+        self.w(f" </sioc:{isioct}>\n")
```

### Comparing `cubicweb-sioc-0.5.0/cubicweb_sioc.egg-info/SOURCES.txt` & `cubicweb-sioc-1.0.0/cubicweb_sioc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-sioc-0.5.0/setup.py` & `cubicweb-sioc-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,17 +52,15 @@
 data_files = __pkginfo__.get("data_files", None)
 dependency_links = __pkginfo__.get("dependency_links", ())
 
 requires = {}
 for entry in ("__depends__",):  # "__recommends__"):
     requires.update(__pkginfo__.get(entry, {}))
 
-install_requires = [
-    "{0} {1}".format(d, v and v or "").strip() for d, v in requires.items()
-]
+install_requires = [f"{d} {v and v or ''}".strip() for d, v in requires.items()]
 
 
 setup(
     name=distname,
     version=version,
     license=license,
     description=description,
```

### Comparing `cubicweb-sioc-0.5.0/test/test_sioc.py` & `cubicweb-sioc-1.0.0/test/test_sioc.py`

 * *Files identical despite different names*

### Comparing `cubicweb-sioc-0.5.0/tox.ini` & `cubicweb-sioc-1.0.0/tox.ini`

 * *Files 5% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 testpaths = test
 addopts = -r fEs
 
 [testenv:black]
 basepython = python3
 skip_install = true
 deps =
-  black >= 19.10b0
+  black >= 22.12
 commands = black --check .
 
 [testenv:black-run]
 basepython = python3
 skip_install = true
 deps =
-  black >= 19.10b0
+  black >= 22.12
 commands = black .
 
 [testenv:flake8]
 basepython = python3
 skip_install = true
 deps =
   flake8
@@ -52,15 +52,15 @@
   check-manifest
 commands =
   {envpython} -m check_manifest
 
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

