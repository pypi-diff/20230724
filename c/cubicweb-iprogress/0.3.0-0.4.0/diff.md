# Comparing `tmp/cubicweb-iprogress-0.3.0.tar.gz` & `tmp/cubicweb-iprogress-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cubicweb-iprogress-0.3.0.tar", last modified: Tue Apr 23 13:50:30 2019, max compression
+gzip compressed data, was "cubicweb-iprogress-0.4.0.tar", last modified: Mon Jul 24 14:00:53 2023, max compression
```

## Comparing `cubicweb-iprogress-0.3.0.tar` & `cubicweb-iprogress-0.4.0.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-04-23 13:50:30.000000 cubicweb-iprogress-0.3.0/
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      271 2019-03-19 16:15:04.000000 cubicweb-iprogress-0.3.0/MANIFEST.in
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-04-23 13:50:30.000000 cubicweb-iprogress-0.3.0/debian/
--rw-------   0 ppepiot   (1000) ppepiot   (1000)       45 2019-03-19 16:15:04.000000 cubicweb-iprogress-0.3.0/debian/rules
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      712 2019-03-19 16:15:04.000000 cubicweb-iprogress-0.3.0/debian/control
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)        2 2019-03-07 16:25:28.000000 cubicweb-iprogress-0.3.0/debian/compat
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      184 2019-03-07 16:25:28.000000 cubicweb-iprogress-0.3.0/debian/copyright
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      637 2019-04-23 13:50:06.000000 cubicweb-iprogress-0.3.0/debian/changelog
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     2635 2019-03-19 16:15:04.000000 cubicweb-iprogress-0.3.0/setup.py
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-04-23 13:50:30.000000 cubicweb-iprogress-0.3.0/cubicweb_iprogress.egg-info/
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       49 2019-04-23 13:50:30.000000 cubicweb-iprogress-0.3.0/cubicweb_iprogress.egg-info/entry_points.txt
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       19 2019-04-23 13:50:30.000000 cubicweb-iprogress-0.3.0/cubicweb_iprogress.egg-info/top_level.txt
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)        1 2019-04-23 13:50:30.000000 cubicweb-iprogress-0.3.0/cubicweb_iprogress.egg-info/not-zip-safe
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      729 2019-04-23 13:50:30.000000 cubicweb-iprogress-0.3.0/cubicweb_iprogress.egg-info/SOURCES.txt
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       17 2019-04-23 13:50:30.000000 cubicweb-iprogress-0.3.0/cubicweb_iprogress.egg-info/requires.txt
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)        1 2019-04-23 13:50:30.000000 cubicweb-iprogress-0.3.0/cubicweb_iprogress.egg-info/dependency_links.txt
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      606 2019-04-23 13:50:30.000000 cubicweb-iprogress-0.3.0/cubicweb_iprogress.egg-info/PKG-INFO
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-04-23 13:50:30.000000 cubicweb-iprogress-0.3.0/cubicweb_iprogress/
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     3516 2019-03-19 16:15:04.000000 cubicweb-iprogress-0.3.0/cubicweb_iprogress/entities.py
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      674 2019-04-23 13:49:52.000000 cubicweb-iprogress-0.3.0/cubicweb_iprogress/__pkginfo__.py
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     9203 2019-03-26 10:58:33.000000 cubicweb-iprogress-0.3.0/cubicweb_iprogress/views.py
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-04-23 13:50:30.000000 cubicweb-iprogress-0.3.0/cubicweb_iprogress/i18n/
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      941 2019-03-19 16:15:04.000000 cubicweb-iprogress-0.3.0/cubicweb_iprogress/i18n/de.po
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      655 2019-03-19 16:15:04.000000 cubicweb-iprogress-0.3.0/cubicweb_iprogress/i18n/fr.po
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      671 2019-03-19 16:15:04.000000 cubicweb-iprogress-0.3.0/cubicweb_iprogress/i18n/es.po
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      542 2019-03-19 16:15:04.000000 cubicweb-iprogress-0.3.0/cubicweb_iprogress/i18n/en.po
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      113 2019-03-19 16:15:04.000000 cubicweb-iprogress-0.3.0/cubicweb_iprogress/__init__.py
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-04-23 13:50:30.000000 cubicweb-iprogress-0.3.0/cubicweb_iprogress/data/
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      471 2019-03-19 16:15:04.000000 cubicweb-iprogress-0.3.0/cubicweb_iprogress/data/cubes.iprogress.css
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     1829 2019-03-19 16:15:04.000000 cubicweb-iprogress-0.3.0/cubicweb_iprogress/data/cubes.iprogress.js
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       38 2019-04-23 13:50:30.000000 cubicweb-iprogress-0.3.0/setup.cfg
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       84 2019-03-07 16:25:28.000000 cubicweb-iprogress-0.3.0/README
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      606 2019-04-23 13:50:30.000000 cubicweb-iprogress-0.3.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:00:53.304613 cubicweb-iprogress-0.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)      366 2023-07-24 13:58:15.000000 cubicweb-iprogress-0.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      535 2023-07-24 14:00:53.300613 cubicweb-iprogress-0.4.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-07-24 13:58:15.000000 cubicweb-iprogress-0.4.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:00:51.896594 cubicweb-iprogress-0.4.0/cubicweb_iprogress/
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-07-24 13:58:15.000000 cubicweb-iprogress-0.4.0/cubicweb_iprogress/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      676 2023-07-24 13:58:15.000000 cubicweb-iprogress-0.4.0/cubicweb_iprogress/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:00:52.352600 cubicweb-iprogress-0.4.0/cubicweb_iprogress/data/
+-rw-rw-rw-   0 root         (0) root         (0)      471 2023-07-24 13:58:15.000000 cubicweb-iprogress-0.4.0/cubicweb_iprogress/data/cubes.iprogress.css
+-rw-rw-rw-   0 root         (0) root         (0)     1829 2023-07-24 13:58:15.000000 cubicweb-iprogress-0.4.0/cubicweb_iprogress/data/cubes.iprogress.js
+-rw-rw-rw-   0 root         (0) root         (0)     3522 2023-07-24 13:58:15.000000 cubicweb-iprogress-0.4.0/cubicweb_iprogress/entities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:00:52.744605 cubicweb-iprogress-0.4.0/cubicweb_iprogress/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)      941 2023-07-24 13:58:15.000000 cubicweb-iprogress-0.4.0/cubicweb_iprogress/i18n/de.po
+-rw-rw-rw-   0 root         (0) root         (0)      542 2023-07-24 13:58:15.000000 cubicweb-iprogress-0.4.0/cubicweb_iprogress/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)      671 2023-07-24 13:58:15.000000 cubicweb-iprogress-0.4.0/cubicweb_iprogress/i18n/es.po
+-rw-rw-rw-   0 root         (0) root         (0)      655 2023-07-24 13:58:15.000000 cubicweb-iprogress-0.4.0/cubicweb_iprogress/i18n/fr.po
+-rw-rw-rw-   0 root         (0) root         (0)     9379 2023-07-24 13:58:15.000000 cubicweb-iprogress-0.4.0/cubicweb_iprogress/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:00:52.332600 cubicweb-iprogress-0.4.0/cubicweb_iprogress.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      535 2023-07-24 14:00:46.000000 cubicweb-iprogress-0.4.0/cubicweb_iprogress.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      756 2023-07-24 14:00:46.000000 cubicweb-iprogress-0.4.0/cubicweb_iprogress.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 14:00:46.000000 cubicweb-iprogress-0.4.0/cubicweb_iprogress.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-07-24 14:00:46.000000 cubicweb-iprogress-0.4.0/cubicweb_iprogress.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 14:00:46.000000 cubicweb-iprogress-0.4.0/cubicweb_iprogress.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-24 14:00:46.000000 cubicweb-iprogress-0.4.0/cubicweb_iprogress.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-24 14:00:46.000000 cubicweb-iprogress-0.4.0/cubicweb_iprogress.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:00:52.940608 cubicweb-iprogress-0.4.0/debian/
+-rw-rw-rw-   0 root         (0) root         (0)      637 2023-07-24 13:58:15.000000 cubicweb-iprogress-0.4.0/debian/changelog
+-rw-rw-rw-   0 root         (0) root         (0)        2 2023-07-24 13:58:15.000000 cubicweb-iprogress-0.4.0/debian/compat
+-rw-rw-rw-   0 root         (0) root         (0)      712 2023-07-24 13:58:15.000000 cubicweb-iprogress-0.4.0/debian/control
+-rw-rw-rw-   0 root         (0) root         (0)      184 2023-07-24 13:58:15.000000 cubicweb-iprogress-0.4.0/debian/copyright
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-07-24 13:58:15.000000 cubicweb-iprogress-0.4.0/debian/rules
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 14:00:53.304613 cubicweb-iprogress-0.4.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2624 2023-07-24 13:58:15.000000 cubicweb-iprogress-0.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:00:53.284613 cubicweb-iprogress-0.4.0/test/
+-rw-rw-rw-   0 root         (0) root         (0)      153 2023-07-24 13:58:15.000000 cubicweb-iprogress-0.4.0/test/test_iprogress.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cubicweb-iprogress-0.3.0/debian/control` & `cubicweb-iprogress-0.4.0/debian/control`

 * *Files identical despite different names*

### Comparing `cubicweb-iprogress-0.3.0/debian/changelog` & `cubicweb-iprogress-0.4.0/debian/changelog`

 * *Files identical despite different names*

### Comparing `cubicweb-iprogress-0.3.0/setup.py` & `cubicweb-iprogress-0.4.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # pylint: disable=W0142,W0403,W0404,W0613,W0622,W0622,W0704,R0904,C0103,E0611
 #
-# copyright 2003-2018 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# copyright 2003-2021 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr/ -- mailto:contact@logilab.fr
 #
 # This file is part of cubiweb-iprogress.
 #
 # CubicWeb is free software: you can redistribute it and/or modify it under the
 # terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
@@ -28,57 +28,57 @@
 from setuptools import find_packages, setup
 
 
 here = dirname(__file__)
 
 # load metadata from the __pkginfo__.py file so there is no risk of conflict
 # see https://packaging.python.org/en/latest/single_source_version.html
-pkginfo = join(here, 'cubicweb_iprogress', '__pkginfo__.py')
+pkginfo = join(here, "cubicweb_iprogress", "__pkginfo__.py")
 __pkginfo__ = {}
 with open(pkginfo) as f:
     exec(f.read(), __pkginfo__)
 
 # get required metadatas
-distname = __pkginfo__['distname']
-version = __pkginfo__['version']
-license = __pkginfo__['license']
-description = __pkginfo__['description']
-web = __pkginfo__['web']
-author = __pkginfo__['author']
-author_email = __pkginfo__['author_email']
-classifiers = __pkginfo__['classifiers']
+distname = __pkginfo__["distname"]
+version = __pkginfo__["version"]
+license = __pkginfo__["license"]
+description = __pkginfo__["description"]
+web = __pkginfo__["web"]
+author = __pkginfo__["author"]
+author_email = __pkginfo__["author_email"]
+classifiers = __pkginfo__["classifiers"]
 
-with open(join(here, 'README')) as f:
+with open(join(here, "README.rst")) as f:
     long_description = f.read()
 
 # get optional metadatas
-data_files = __pkginfo__.get('data_files', None)
-dependency_links = __pkginfo__.get('dependency_links', ())
+data_files = __pkginfo__.get("data_files", None)
+dependency_links = __pkginfo__.get("dependency_links", ())
 
 requires = {}
 for entry in ("__depends__",):  # "__recommends__"):
     requires.update(__pkginfo__.get(entry, {}))
-install_requires = ["{0} {1}".format(d, v and v or "").strip()
-
-                    for d, v in requires.items()]
+install_requires = [
+    "{0} {1}".format(d, v and v or "").strip() for d, v in requires.items()
+]
 
 
 setup(
     name=distname,
     version=version,
     license=license,
     description=description,
     long_description=long_description,
     author=author,
     author_email=author_email,
     url=web,
     classifiers=classifiers,
-    packages=find_packages(exclude=['test']),
+    packages=find_packages(exclude=["test"]),
     install_requires=install_requires,
     include_package_data=True,
     entry_points={
-        'cubicweb.cubes': [
-            'iprogress=cubicweb_iprogress',
+        "cubicweb.cubes": [
+            "iprogress=cubicweb_iprogress",
         ],
     },
     zip_safe=False,
 )
```

### Comparing `cubicweb-iprogress-0.3.0/cubicweb_iprogress.egg-info/SOURCES.txt` & `cubicweb-iprogress-0.4.0/cubicweb_iprogress.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 MANIFEST.in
-README
+README.rst
 setup.py
 cubicweb_iprogress/__init__.py
 cubicweb_iprogress/__pkginfo__.py
 cubicweb_iprogress/entities.py
 cubicweb_iprogress/views.py
 cubicweb_iprogress.egg-info/PKG-INFO
 cubicweb_iprogress.egg-info/SOURCES.txt
@@ -18,8 +18,9 @@
 cubicweb_iprogress/i18n/en.po
 cubicweb_iprogress/i18n/es.po
 cubicweb_iprogress/i18n/fr.po
 debian/changelog
 debian/compat
 debian/control
 debian/copyright
-debian/rules
+debian/rules
+test/test_iprogress.py
```

### Comparing `cubicweb-iprogress-0.3.0/cubicweb_iprogress.egg-info/PKG-INFO` & `cubicweb-iprogress-0.4.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: cubicweb-iprogress
-Version: 0.3.0
+Version: 0.4.0
 Summary: some adapters and view for stuff progressing to reach a milestone
 Home-page: http://www.cubicweb.org/project/cubicweb-iprogress
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
-Description: Summary
-        -------
-        
-        Some adapters and view for things progressing towards completion.
-        
-        
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: JavaScript
+
+Summary
+-------
+
+Some adapters and view for things progressing towards completion.
+
```

### Comparing `cubicweb-iprogress-0.3.0/cubicweb_iprogress/entities.py` & `cubicweb-iprogress-0.4.0/cubicweb_iprogress/entities.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# copyright 2003-2011 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# copyright 2003-2021 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
 #
@@ -11,43 +11,45 @@
 # FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with this program. If not, see <http://www.gnu.org/licenses/>.
 """cubicweb-iprogress adapters"""
 
-from cubicweb.view import EntityAdapter
+from cubicweb.entity import EntityAdapter
+
 
 class IProgressAdapter(EntityAdapter):
     """something that has a cost, a state and a progression.
 
     You should at least override progress_info an in_progress methods on
     concrete implementations.
     """
-    __regid__ = 'IProgress'
+
+    __regid__ = "IProgress"
     __abstract__ = True
 
     @property
     def cost(self):
         """the total cost"""
-        return self.progress_info()['estimated']
+        return self.progress_info()["estimated"]
 
     @property
     def revised_cost(self):
-        return self.progress_info().get('estimatedcorrected', self.cost)
+        return self.progress_info().get("estimatedcorrected", self.cost)
 
     @property
     def done(self):
         """what is already done"""
-        return self.progress_info()['done']
+        return self.progress_info()["done"]
 
     @property
     def todo(self):
         """what remains to be done"""
-        return self.progress_info()['todo']
+        return self.progress_info()["todo"]
 
     def progress_info(self):
         """returns a dictionary describing progress/estimated cost of the
         version.
 
         - mandatory keys are (''estimated', 'done', 'todo')
 
@@ -66,30 +68,30 @@
     def in_progress(self):
         """returns True if status is not finished"""
         raise NotImplementedError
 
     def progress(self):
         """returns the % progress of the task item"""
         try:
-            return 100. * self.done / self.revised_cost
+            return 100.0 * self.done / self.revised_cost
         except ZeroDivisionError:
             # total cost is 0 : if everything was estimated, task is completed
-            if self.progress_info().get('notestimated'):
-                return 0.
+            if self.progress_info().get("notestimated"):
+                return 0.0
             return 100
 
     def progress_class(self):
-        return ''
+        return ""
 
 
 class IMileStoneAdapter(IProgressAdapter):
-    __regid__ = 'IMileStone'
+    __regid__ = "IMileStone"
     __abstract__ = True
 
-    parent_type = None # specify main task's type
+    parent_type = None  # specify main task's type
 
     def get_main_task(self):
         """returns the main ITask entity"""
         raise NotImplementedError
 
     def initial_prevision_date(self):
         """returns the initial expected end of the milestone"""
@@ -104,8 +106,7 @@
     def completion_date(self):
         """returns date on which the subtask has been completed"""
         raise NotImplementedError
 
     def contractors(self):
         """returns the list of persons supposed to work on this task"""
         raise NotImplementedError
-
```

### Comparing `cubicweb-iprogress-0.3.0/cubicweb_iprogress/__pkginfo__.py` & `cubicweb-iprogress-0.4.0/cubicweb_iprogress/__pkginfo__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # pylint: disable=W0622
 """cubicweb-iprogress application packaging information"""
 
-modname = 'iprogress'
-distname = 'cubicweb-iprogress'
+modname = "iprogress"
+distname = "cubicweb-iprogress"
 
-numversion = (0, 3, 0)
-version = '.'.join(str(num) for num in numversion)
+numversion = (0, 4, 0)
+version = ".".join(str(num) for num in numversion)
 
-license = 'LGPL'
-author = 'LOGILAB S.A. (Paris, FRANCE)'
-author_email = 'contact@logilab.fr'
-description = 'some adapters and view for stuff progressing to reach a milestone'
-web = 'http://www.cubicweb.org/project/%s' % distname
+license = "LGPL"
+author = "LOGILAB S.A. (Paris, FRANCE)"
+author_email = "contact@logilab.fr"
+description = "some adapters and view for stuff progressing to reach a milestone"
+web = "http://www.cubicweb.org/project/%s" % distname
 classifiers = [
-    'Environment :: Web Environment',
-    'Framework :: CubicWeb',
-    'Programming Language :: Python',
-    'Programming Language :: JavaScript',
-    ]
+    "Environment :: Web Environment",
+    "Framework :: CubicWeb",
+    "Programming Language :: Python",
+    "Programming Language :: JavaScript",
+]
 
-__depends__ =  {'cubicweb': '>= 3.24.0'}
+__depends__ = {"cubicweb": ">=3.38.0,<3.39.0"}
 __recommends__ = {}
```

### Comparing `cubicweb-iprogress-0.3.0/cubicweb_iprogress/views.py` & `cubicweb-iprogress-0.4.0/cubicweb_iprogress/views.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# copyright 2003-2011 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# copyright 2003-2021 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
 #
@@ -22,144 +22,160 @@
 
 from logilab.mtconverter import xml_escape
 
 from cubicweb import _
 from cubicweb.utils import make_uid
 from cubicweb.predicates import adaptable
 from cubicweb.schema import display_name
-from cubicweb.view import EntityView
-from cubicweb.web.views import tableview
+from cubicweb_web.view import EntityView
+from cubicweb_web.views import tableview
 
 
 def state_cell(w, entity):
-    w(xml_escape(entity.cw_adapt_to('IWorkflowable').printable_state))
+    w(xml_escape(entity.cw_adapt_to("IWorkflowable").printable_state))
+
 
 def eta_date_cell(w, entity):
-    imilestone = entity.cw_adapt_to('IMileStone')
+    imilestone = entity.cw_adapt_to("IMileStone")
     req = entity._cw
     if imilestone.finished():
         formated_date = req.format_date(imilestone.completion_date())
     else:
         formated_date = req.format_date(imilestone.initial_prevision_date())
         if imilestone.in_progress():
             eta_date = req.format_date(imilestone.eta_date())
             if eta_date:
                 if formated_date:
-                    formated_date += u' (%s %s)' % (req._('expected:'), eta_date)
+                    formated_date += " (%s %s)" % (req._("expected:"), eta_date)
                 else:
-                    formated_date = u'%s %s' % (req._('expected:'), eta_date)
+                    formated_date = "%s %s" % (req._("expected:"), eta_date)
         w(formated_date)
 
+
 def todo_by_cell(w, entity):
-    imilestone = entity.cw_adapt_to('IMileStone')
-    w(u', '.join(p.view('outofcontext') for p in imilestone.contractors()))
+    imilestone = entity.cw_adapt_to("IMileStone")
+    w(", ".join(p.view("outofcontext") for p in imilestone.contractors()))
+
 
 def cost_cell(w, entity):
     req = entity._cw
-    pinfo = entity.cw_adapt_to('IMileStone').progress_info()
-    totalcost = pinfo.get('estimatedcorrected', pinfo['estimated'])
-    missing = pinfo.get('notestimatedcorrected', pinfo.get('notestimated', 0))
+    pinfo = entity.cw_adapt_to("IMileStone").progress_info()
+    totalcost = pinfo.get("estimatedcorrected", pinfo["estimated"])
+    missing = pinfo.get("notestimatedcorrected", pinfo.get("notestimated", 0))
     costdescr = []
     if missing:
         # XXX: link to unestimated entities
-        costdescr.append(req._('%s not estimated') % missing)
-    estimated = pinfo['estimated']
+        costdescr.append(req._("%s not estimated") % missing)
+    estimated = pinfo["estimated"]
     if estimated and estimated != totalcost:
-        costdescr.append(req._('initial estimation %s') % estimated)
+        costdescr.append(req._("initial estimation %s") % estimated)
     if costdescr:
-        w(u'%s (%s)' % (totalcost, ', '.join(costdescr)))
+        w("%s (%s)" % (totalcost, ", ".join(costdescr)))
     else:
         w(six.text_type(totalcost))
 
+
 def progress_cell(w, entity):
-    entity.view('progressbar', w=w)
+    entity.view("progressbar", w=w)
 
 
 class ProgressTableView(tableview.EntityTableView):
     """The progress table view is able to display progress information
     of any object implement IMileStone.
 
     By default it is composed of 7 columns : parent task, milestone, state,
     estimated date, cost, progressbar, and todo_by
 
     As :class:`EntityTableView` a `columns` class attribute lets you remove or
     reorder some of those columns.
     """
 
-    __regid__ = 'progress_table_view'
-    __select__ = adaptable('IMileStone')
+    __regid__ = "progress_table_view"
+    __select__ = adaptable("IMileStone")
 
-    title = _('task progression')
-    layout_id = 'imilestone_table_layout'
-    columns = ('project', 'milestone', _('state'), _('eta_date'),
-               _('cost'), _('progress'), _('todo_by'))
+    title = _("task progression")
+    layout_id = "imilestone_table_layout"
+    columns = (
+        "project",
+        "milestone",
+        _("state"),
+        _("eta_date"),
+        _("cost"),
+        _("progress"),
+        _("todo_by"),
+    )
 
     class ProjectColRenderer(tableview.EntityTableColRenderer):
         def render_header(self, w):
             sample = self.entity(0)
-            w(display_name(self._cw, sample.cw_adapt_to('IMileStone').parent_type))
+            w(display_name(self._cw, sample.cw_adapt_to("IMileStone").parent_type))
+
         def render_entity(self, w, entity):
-            project = entity.cw_adapt_to('IMileStone').get_main_task()
-            project.view('incontext', w=w)
+            project = entity.cw_adapt_to("IMileStone").get_main_task()
+            project.view("incontext", w=w)
+
         def entity_sortvalue(self, entity):
-            return entity.cw_adapt_to('IMileStone').get_main_task().sortvalue()
+            return entity.cw_adapt_to("IMileStone").get_main_task().sortvalue()
 
     class MileStoneColRenderer(tableview.MainEntityColRenderer):
         def render_header(self, w):
             sample = self.entity(0)
             w(display_name(self._cw, sample.__regid__))
 
     column_renderers = {
-        'project': ProjectColRenderer(),
-        'milestone': MileStoneColRenderer(),
-        'state': tableview.EntityTableColRenderer(renderfunc=state_cell),
-        'eta_date': tableview.EntityTableColRenderer(renderfunc=eta_date_cell),
-        'cost': tableview.EntityTableColRenderer(renderfunc=cost_cell),
-        'progress': tableview.EntityTableColRenderer(renderfunc=progress_cell),
-        'todo_by': tableview.EntityTableColRenderer(renderfunc=todo_by_cell),
-        }
+        "project": ProjectColRenderer(),
+        "milestone": MileStoneColRenderer(),
+        "state": tableview.EntityTableColRenderer(renderfunc=state_cell),
+        "eta_date": tableview.EntityTableColRenderer(renderfunc=eta_date_cell),
+        "cost": tableview.EntityTableColRenderer(renderfunc=cost_cell),
+        "progress": tableview.EntityTableColRenderer(renderfunc=progress_cell),
+        "todo_by": tableview.EntityTableColRenderer(renderfunc=todo_by_cell),
+    }
 
 
 class InContextProgressTableView(ProgressTableView):
     """this views redirects to ``progress_table_view`` but removes
     the ``project`` column
     """
-    __regid__ = 'ic_progress_table_view'
+
+    __regid__ = "ic_progress_table_view"
 
     def call(self, columns=None):
         if columns is None:
-            view = self._cw.vreg['views'].select('progress_table_view', self._cw,
-                                                 rset=self.cw_rset)
+            view = self._cw.vreg["views"].select(
+                "progress_table_view", self._cw, rset=self.cw_rset
+            )
             columns = list(view.columns)
             self.column_renderers = view.column_renderers
         try:
-            columns.remove('project')
+            columns.remove("project")
         except ValueError:
-            self.info('[ic_progress_table_view] could not remove project from columns')
+            self.info("[ic_progress_table_view] could not remove project from columns")
         super(InContextProgressTableView, self).call(columns=columns)
 
 
 class ProgressTableLayout(tableview.TableLayout):
-    __regid__ = 'imilestone_table_layout'
-    needs_css = ('cubes.iprogress.css',)
+    __regid__ = "imilestone_table_layout"
+    needs_css = ("cubes.iprogress.css",)
 
     def row_attributes(self, rownum):
         attrs = super(ProgressTableLayout, self).row_attributes(rownum)
         entity = self.view.entity(rownum)
-        cssclass = entity.cw_adapt_to('IMileStone').progress_class()
-        attrs['class'] += cssclass
+        cssclass = entity.cw_adapt_to("IMileStone").progress_class()
+        attrs["class"] += cssclass
         return attrs
 
 
 class ProgressBarView(EntityView):
     """displays a progress bar"""
-    __regid__ = 'progressbar'
-    __select__ = adaptable('IProgress')
 
-    title = _('progress bar')
+    __regid__ = "progressbar"
+    __select__ = adaptable("IProgress")
+
+    title = _("progress bar")
 
     precision = 0.1
     red_threshold = 1.1
     orange_threshold = 1.05
     yellow_threshold = 1
 
     @classmethod
@@ -176,72 +192,81 @@
         return overrun
 
     @classmethod
     def overrun_percentage(cls, iprogress):
         budget = iprogress.revised_cost or 0
         if budget == 0:
             return 0
-        return cls.overrun(iprogress) * 100. / budget
+        return cls.overrun(iprogress) * 100.0 / budget
 
     def cell_call(self, row, col):
-        self._cw.add_css('cubes.iprogress.css')
-        self._cw.add_js('cubes.iprogress.js')
+        self._cw.add_css("cubes.iprogress.css")
+        self._cw.add_js("cubes.iprogress.js")
         entity = self.cw_rset.get_entity(row, col)
-        iprogress = entity.cw_adapt_to('IProgress')
+        iprogress = entity.cw_adapt_to("IProgress")
         done = iprogress.done or 0
         todo = iprogress.todo or 0
         budget = iprogress.revised_cost or 0
         if budget == 0:
             pourcent = 100
         else:
-            pourcent = done*100./budget
+            pourcent = done * 100.0 / budget
         if pourcent > 100.1:
-            color = 'red'
-        elif todo+done > self.red_threshold*budget:
-            color = 'red'
-        elif todo+done > self.orange_threshold*budget:
-            color = 'orange'
-        elif todo+done > self.yellow_threshold*budget:
-            color = 'yellow'
+            color = "red"
+        elif todo + done > self.red_threshold * budget:
+            color = "red"
+        elif todo + done > self.orange_threshold * budget:
+            color = "orange"
+        elif todo + done > self.yellow_threshold * budget:
+            color = "yellow"
         else:
-            color = 'green'
+            color = "green"
         if pourcent < 0:
             pourcent = 0
 
-        if floor(done) == done or done>100:
-            done_str = '%i' % done
+        if floor(done) == done or done > 100:
+            done_str = "%i" % done
         else:
-            done_str = '%.1f' % done
-        if floor(budget) == budget or budget>100:
-            budget_str = '%i' % budget
+            done_str = "%.1f" % done
+        if floor(budget) == budget or budget > 100:
+            budget_str = "%i" % budget
         else:
-            budget_str = '%.1f' % budget
+            budget_str = "%.1f" % budget
 
-        title = u'%s/%s = %i%%' % (done_str, budget_str, pourcent)
+        title = "%s/%s = %i%%" % (done_str, budget_str, pourcent)
         short_title = title
         overrunpercent = self.overrun_percentage(iprogress)
         if overrunpercent:
             overrun = self.overrun(iprogress)
-            title += u' overrun +%sj (+%i%%)' % (overrun, overrunpercent)
+            title += " overrun +%sj (+%i%%)" % (overrun, overrunpercent)
             if floor(overrun) == overrun or overrun > 100:
-                short_title += u' +%i' % overrun
+                short_title += " +%i" % overrun
             else:
-                short_title += u' +%.1f' % overrun
+                short_title += " +%.1f" % overrun
         # write bars
-        maxi = max(done+todo, budget)
+        maxi = max(done + todo, budget)
         if maxi == 0:
             maxi = 1
-        cid = make_uid('progress_bar')
+        cid = make_uid("progress_bar")
         self._cw.html_headers.add_onload(
-            'draw_progressbar("canvas%s", %i, %i, %i, "%s");' %
-            (cid, int(100.*done/maxi), int(100.*(done+todo)/maxi),
-             int(100.*budget/maxi), color))
-        self.w(u'%s<br/>'
-               u'<canvas class="progressbar" id="canvas%s" width="100" height="10"></canvas>'
-               % (xml_escape(short_title), cid))
+            'draw_progressbar("canvas%s", %i, %i, %i, "%s");'
+            % (
+                cid,
+                int(100.0 * done / maxi),
+                int(100.0 * (done + todo) / maxi),
+                int(100.0 * budget / maxi),
+                color,
+            )
+        )
+        self.w(
+            "%s<br/>"
+            '<canvas class="progressbar" id="canvas%s" width="100" height="10"></canvas>'
+            % (xml_escape(short_title), cid)
+        )
+
 
 def registration_callback(vreg):
     oldclasses = (ProgressTableView, InContextProgressTableView, ProgressBarView)
     vreg.register_all(globals().values(), __name__, oldclasses)
     # clear registry so that if cw bw compat views are in, they are kicked out
     # first
     for cls in oldclasses:
```

### Comparing `cubicweb-iprogress-0.3.0/cubicweb_iprogress/i18n/de.po` & `cubicweb-iprogress-0.4.0/cubicweb_iprogress/i18n/de.po`

 * *Files identical despite different names*

### Comparing `cubicweb-iprogress-0.3.0/cubicweb_iprogress/i18n/fr.po` & `cubicweb-iprogress-0.4.0/cubicweb_iprogress/i18n/fr.po`

 * *Files identical despite different names*

### Comparing `cubicweb-iprogress-0.3.0/cubicweb_iprogress/i18n/es.po` & `cubicweb-iprogress-0.4.0/cubicweb_iprogress/i18n/es.po`

 * *Files identical despite different names*

### Comparing `cubicweb-iprogress-0.3.0/cubicweb_iprogress/i18n/en.po` & `cubicweb-iprogress-0.4.0/cubicweb_iprogress/i18n/en.po`

 * *Files identical despite different names*

### Comparing `cubicweb-iprogress-0.3.0/cubicweb_iprogress/data/cubes.iprogress.js` & `cubicweb-iprogress-0.4.0/cubicweb_iprogress/data/cubes.iprogress.js`

 * *Files identical despite different names*

### Comparing `cubicweb-iprogress-0.3.0/PKG-INFO` & `cubicweb-iprogress-0.4.0/cubicweb_iprogress.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: cubicweb-iprogress
-Version: 0.3.0
+Version: 0.4.0
 Summary: some adapters and view for stuff progressing to reach a milestone
 Home-page: http://www.cubicweb.org/project/cubicweb-iprogress
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
-Description: Summary
-        -------
-        
-        Some adapters and view for things progressing towards completion.
-        
-        
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: JavaScript
+
+Summary
+-------
+
+Some adapters and view for things progressing towards completion.
+
```

