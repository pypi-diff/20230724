# Comparing `tmp/copasi-petab-importer-1.0.4.tar.gz` & `tmp/copasi-petab-importer-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copasi-petab-importer-1.0.4.tar", last modified: Fri May 26 07:51:36 2023, max compression
+gzip compressed data, was "copasi-petab-importer-1.0.5.tar", last modified: Mon Jul 24 08:00:35 2023, max compression
```

## Comparing `copasi-petab-importer-1.0.4.tar` & `copasi-petab-importer-1.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 frank      (501) staff       (20)        0 2023-05-26 07:51:36.071087 copasi-petab-importer-1.0.4/
--rw-r--r--   0 frank      (501) staff       (20)       64 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.4/MANIFEST.in
--rw-r--r--   0 frank      (501) staff       (20)      279 2023-05-26 07:51:36.071151 copasi-petab-importer-1.0.4/PKG-INFO
--rw-r--r--   0 frank      (501) staff       (20)     3714 2023-05-03 06:40:46.000000 copasi-petab-importer-1.0.4/README.md
-drwxr-xr-x   0 frank      (501) staff       (20)        0 2023-05-26 07:51:36.071498 copasi-petab-importer-1.0.4/copasi_petab_importer/
--rw-r--r--   0 frank      (501) staff       (20)     9163 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.4/copasi_petab_importer/PEtab.py
--rw-r--r--   0 frank      (501) staff       (20)      351 2023-05-16 13:46:05.000000 copasi-petab-importer-1.0.4/copasi_petab_importer/__init__.py
--rw-r--r--   0 frank      (501) staff       (20)      497 2023-05-26 07:51:36.071528 copasi-petab-importer-1.0.4/copasi_petab_importer/_version.py
--rw-r--r--   0 frank      (501) staff       (20)     1899 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.4/copasi_petab_importer/convert_all_petab.py
--rw-r--r--   0 frank      (501) staff       (20)     4579 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.4/copasi_petab_importer/convert_benchmark.py
--rw-r--r--   0 frank      (501) staff       (20)    39718 2023-05-26 07:45:03.000000 copasi-petab-importer-1.0.4/copasi_petab_importer/convert_petab.py
--rw-r--r--   0 frank      (501) staff       (20)    12270 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.4/copasi_petab_importer/petab.ui
-drwxr-xr-x   0 frank      (501) staff       (20)        0 2023-05-26 07:51:36.070702 copasi-petab-importer-1.0.4/copasi_petab_importer.egg-info/
--rw-r--r--   0 frank      (501) staff       (20)      279 2023-05-26 07:51:36.000000 copasi-petab-importer-1.0.4/copasi_petab_importer.egg-info/PKG-INFO
--rw-r--r--   0 frank      (501) staff       (20)      603 2023-05-26 07:51:36.000000 copasi-petab-importer-1.0.4/copasi_petab_importer.egg-info/SOURCES.txt
--rw-r--r--   0 frank      (501) staff       (20)        1 2023-05-26 07:51:36.000000 copasi-petab-importer-1.0.4/copasi_petab_importer.egg-info/dependency_links.txt
--rw-r--r--   0 frank      (501) staff       (20)      138 2023-05-26 07:51:36.000000 copasi-petab-importer-1.0.4/copasi_petab_importer.egg-info/entry_points.txt
--rw-r--r--   0 frank      (501) staff       (20)       62 2023-05-26 07:51:36.000000 copasi-petab-importer-1.0.4/copasi_petab_importer.egg-info/requires.txt
--rw-r--r--   0 frank      (501) staff       (20)       22 2023-05-26 07:51:36.000000 copasi-petab-importer-1.0.4/copasi_petab_importer.egg-info/top_level.txt
--rw-r--r--   0 frank      (501) staff       (20)      243 2023-05-26 07:51:36.071372 copasi-petab-importer-1.0.4/setup.cfg
--rw-r--r--   0 frank      (501) staff       (20)      899 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.4/setup.py
-drwxr-xr-x   0 frank      (501) staff       (20)        0 2023-05-26 07:51:36.070814 copasi-petab-importer-1.0.4/test/
--rw-r--r--   0 frank      (501) staff       (20)     2940 2023-05-25 08:44:48.000000 copasi-petab-importer-1.0.4/test/test_importer.py
--rw-r--r--   0 frank      (501) staff       (20)    78254 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.4/versioneer.py
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2023-07-24 08:00:35.083483 copasi-petab-importer-1.0.5/
+-rw-r--r--   0 frank      (501) staff       (20)       64 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.5/MANIFEST.in
+-rw-r--r--   0 frank      (501) staff       (20)      279 2023-07-24 08:00:35.083551 copasi-petab-importer-1.0.5/PKG-INFO
+-rw-r--r--   0 frank      (501) staff       (20)     3714 2023-05-03 06:40:46.000000 copasi-petab-importer-1.0.5/README.md
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2023-07-24 08:00:35.084028 copasi-petab-importer-1.0.5/copasi_petab_importer/
+-rw-r--r--   0 frank      (501) staff       (20)     9163 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.5/copasi_petab_importer/PEtab.py
+-rw-r--r--   0 frank      (501) staff       (20)      351 2023-05-16 13:46:05.000000 copasi-petab-importer-1.0.5/copasi_petab_importer/__init__.py
+-rw-r--r--   0 frank      (501) staff       (20)      497 2023-07-24 08:00:35.084093 copasi-petab-importer-1.0.5/copasi_petab_importer/_version.py
+-rw-r--r--   0 frank      (501) staff       (20)     1899 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.5/copasi_petab_importer/convert_all_petab.py
+-rw-r--r--   0 frank      (501) staff       (20)     4579 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.5/copasi_petab_importer/convert_benchmark.py
+-rw-r--r--   0 frank      (501) staff       (20)    39718 2023-07-24 07:57:02.000000 copasi-petab-importer-1.0.5/copasi_petab_importer/convert_petab.py
+-rw-r--r--   0 frank      (501) staff       (20)    12270 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.5/copasi_petab_importer/petab.ui
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2023-07-24 08:00:35.083006 copasi-petab-importer-1.0.5/copasi_petab_importer.egg-info/
+-rw-r--r--   0 frank      (501) staff       (20)      279 2023-07-24 08:00:35.000000 copasi-petab-importer-1.0.5/copasi_petab_importer.egg-info/PKG-INFO
+-rw-r--r--   0 frank      (501) staff       (20)      603 2023-07-24 08:00:35.000000 copasi-petab-importer-1.0.5/copasi_petab_importer.egg-info/SOURCES.txt
+-rw-r--r--   0 frank      (501) staff       (20)        1 2023-07-24 08:00:35.000000 copasi-petab-importer-1.0.5/copasi_petab_importer.egg-info/dependency_links.txt
+-rw-r--r--   0 frank      (501) staff       (20)      138 2023-07-24 08:00:35.000000 copasi-petab-importer-1.0.5/copasi_petab_importer.egg-info/entry_points.txt
+-rw-r--r--   0 frank      (501) staff       (20)       62 2023-07-24 08:00:35.000000 copasi-petab-importer-1.0.5/copasi_petab_importer.egg-info/requires.txt
+-rw-r--r--   0 frank      (501) staff       (20)       22 2023-07-24 08:00:35.000000 copasi-petab-importer-1.0.5/copasi_petab_importer.egg-info/top_level.txt
+-rw-r--r--   0 frank      (501) staff       (20)      243 2023-07-24 08:00:35.083876 copasi-petab-importer-1.0.5/setup.cfg
+-rw-r--r--   0 frank      (501) staff       (20)      899 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.5/setup.py
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2023-07-24 08:00:35.083146 copasi-petab-importer-1.0.5/test/
+-rw-r--r--   0 frank      (501) staff       (20)     2940 2023-05-25 08:44:48.000000 copasi-petab-importer-1.0.5/test/test_importer.py
+-rw-r--r--   0 frank      (501) staff       (20)    78254 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.5/versioneer.py
```

### Comparing `copasi-petab-importer-1.0.4/README.md` & `copasi-petab-importer-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `copasi-petab-importer-1.0.4/copasi_petab_importer/PEtab.py` & `copasi-petab-importer-1.0.5/copasi_petab_importer/PEtab.py`

 * *Files identical despite different names*

### Comparing `copasi-petab-importer-1.0.4/copasi_petab_importer/convert_all_petab.py` & `copasi-petab-importer-1.0.5/copasi_petab_importer/convert_all_petab.py`

 * *Files identical despite different names*

### Comparing `copasi-petab-importer-1.0.4/copasi_petab_importer/convert_benchmark.py` & `copasi-petab-importer-1.0.5/copasi_petab_importer/convert_benchmark.py`

 * *Files identical despite different names*

### Comparing `copasi-petab-importer-1.0.4/copasi_petab_importer/convert_petab.py` & `copasi-petab-importer-1.0.5/copasi_petab_importer/convert_petab.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         all_ids = [x.getId() for x in doc.getListOfAllElements() if x.isSetId()]
 
         for i in range(observable_data.shape[0]):
             current = observable_data.iloc[i]
             id = current.observableId
 
             # ignore invalid ids
-            if not libsbml.SyntaxChecker_isValidSBMLSId(id):
+            if not libsbml.SyntaxChecker.isValidSBMLSId(id):
                 logger.warning(
                     'Invalid observableId {0} in observable table'.
                     format(id))
                 continue
 
             name = id
```

### Comparing `copasi-petab-importer-1.0.4/copasi_petab_importer/petab.ui` & `copasi-petab-importer-1.0.5/copasi_petab_importer/petab.ui`

 * *Files identical despite different names*

### Comparing `copasi-petab-importer-1.0.4/copasi_petab_importer.egg-info/SOURCES.txt` & `copasi-petab-importer-1.0.5/copasi_petab_importer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `copasi-petab-importer-1.0.4/setup.py` & `copasi-petab-importer-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `copasi-petab-importer-1.0.4/test/test_importer.py` & `copasi-petab-importer-1.0.5/test/test_importer.py`

 * *Files identical despite different names*

### Comparing `copasi-petab-importer-1.0.4/versioneer.py` & `copasi-petab-importer-1.0.5/versioneer.py`

 * *Files identical despite different names*

