# Comparing `tmp/casex-1.2.2.tar.gz` & `tmp/casex-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\casex-1.2.2.tar", last modified: Mon Jul 10 13:38:49 2023, max compression
+gzip compressed data, was "dist\casex-1.2.3.tar", last modified: Mon Jul 24 08:54:43 2023, max compression
```

## Comparing `casex-1.2.2.tar` & `casex-1.2.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 13:38:49.000000 casex-1.2.2/
-drwxrwxrwx   0        0        0        0 2023-07-10 13:38:49.000000 casex-1.2.2/casex/
--rw-rw-rw-   0        0        0    15514 2023-07-10 11:29:40.000000 casex-1.2.2/casex/aircraft_specs.py
--rw-rw-rw-   0        0        0    12292 2023-07-10 11:29:16.000000 casex-1.2.2/casex/annex_f_parms.py
--rw-rw-rw-   0        0        0    23506 2023-07-10 12:42:42.000000 casex-1.2.2/casex/annex_f_tables.py
--rw-rw-rw-   0        0        0    11320 2023-07-10 12:24:08.000000 casex-1.2.2/casex/ballistic_descent_models.py
--rw-rw-rw-   0        0        0      224 2023-07-10 09:35:41.000000 casex-1.2.2/casex/constants.py
--rw-rw-rw-   0        0        0     2163 2020-11-23 15:00:03.000000 casex-1.2.2/casex/conversion.py
--rw-rw-rw-   0        0        0    18061 2023-07-10 12:23:50.000000 casex-1.2.2/casex/critical_area_models.py
--rw-rw-rw-   0        0        0      974 2023-07-07 10:55:23.000000 casex-1.2.2/casex/enums.py
--rw-rw-rw-   0        0        0      494 2023-05-16 08:00:45.000000 casex-1.2.2/casex/exceptions.py
--rw-rw-rw-   0        0        0     9435 2020-12-18 07:43:14.000000 casex-1.2.2/casex/explosion_models.py
--rw-rw-rw-   0        0        0    27407 2023-07-10 13:12:13.000000 casex-1.2.2/casex/figures.py
--rw-rw-rw-   0        0        0     7941 2020-12-03 11:38:40.000000 casex-1.2.2/casex/friction_coefficient.py
--rw-rw-rw-   0        0        0     9778 2021-10-22 11:35:28.000000 casex-1.2.2/casex/ground_risk_buffer.py
--rw-rw-rw-   0        0        0     4617 2020-12-05 15:03:30.000000 casex-1.2.2/casex/misc.py
--rw-rw-rw-   0        0        0    40298 2021-02-05 12:05:45.000000 casex-1.2.2/casex/obstacles.py
--rw-rw-rw-   0        0        0     6993 2020-12-18 11:02:58.000000 casex-1.2.2/casex/obstacle_simulation.py
--rw-rw-rw-   0        0        0     1306 2021-02-23 22:47:23.000000 casex-1.2.2/casex/temporary_testing_figures.py
--rw-rw-rw-   0        0        0      472 2023-07-07 10:54:37.000000 casex-1.2.2/casex/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-10 13:38:49.000000 casex-1.2.2/casex.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-10 13:38:48.000000 casex-1.2.2/casex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2020-12-29 10:07:56.000000 casex-1.2.2/casex.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     2789 2023-07-10 13:38:48.000000 casex-1.2.2/casex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       41 2023-07-10 13:38:48.000000 casex-1.2.2/casex.egg-info/requires.txt
--rw-rw-rw-   0        0        0      627 2023-07-10 13:38:48.000000 casex-1.2.2/casex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        6 2023-07-10 13:38:48.000000 casex-1.2.2/casex.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      119 2020-10-20 09:11:26.000000 casex-1.2.2/LICENSE.txt
--rw-rw-rw-   0        0        0     2789 2023-07-10 13:38:49.000000 casex-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2175 2023-03-01 14:11:00.000000 casex-1.2.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-10 13:38:49.000000 casex-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0      946 2023-07-10 13:37:57.000000 casex-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 08:54:43.000000 casex-1.2.3/
+drwxrwxrwx   0        0        0        0 2023-07-24 08:54:43.000000 casex-1.2.3/casex/
+-rw-rw-rw-   0        0        0    15514 2023-07-10 11:29:40.000000 casex-1.2.3/casex/aircraft_specs.py
+-rw-rw-rw-   0        0        0    12292 2023-07-10 11:29:16.000000 casex-1.2.3/casex/annex_f_parms.py
+-rw-rw-rw-   0        0        0    23507 2023-07-10 13:41:06.000000 casex-1.2.3/casex/annex_f_tables.py
+-rw-rw-rw-   0        0        0    11320 2023-07-10 12:24:08.000000 casex-1.2.3/casex/ballistic_descent_models.py
+-rw-rw-rw-   0        0        0      224 2023-07-10 09:35:41.000000 casex-1.2.3/casex/constants.py
+-rw-rw-rw-   0        0        0     2163 2020-11-23 15:00:03.000000 casex-1.2.3/casex/conversion.py
+-rw-rw-rw-   0        0        0    18061 2023-07-10 13:43:04.000000 casex-1.2.3/casex/critical_area_models.py
+-rw-rw-rw-   0        0        0      974 2023-07-07 10:55:23.000000 casex-1.2.3/casex/enums.py
+-rw-rw-rw-   0        0        0      494 2023-05-16 08:00:45.000000 casex-1.2.3/casex/exceptions.py
+-rw-rw-rw-   0        0        0     9435 2020-12-18 07:43:14.000000 casex-1.2.3/casex/explosion_models.py
+-rw-rw-rw-   0        0        0    27407 2023-07-10 13:12:13.000000 casex-1.2.3/casex/figures.py
+-rw-rw-rw-   0        0        0     7941 2020-12-03 11:38:40.000000 casex-1.2.3/casex/friction_coefficient.py
+-rw-rw-rw-   0        0        0     9778 2021-10-22 11:35:28.000000 casex-1.2.3/casex/ground_risk_buffer.py
+-rw-rw-rw-   0        0        0     4617 2020-12-05 15:03:30.000000 casex-1.2.3/casex/misc.py
+-rw-rw-rw-   0        0        0    40298 2021-02-05 12:05:45.000000 casex-1.2.3/casex/obstacles.py
+-rw-rw-rw-   0        0        0     6993 2020-12-18 11:02:58.000000 casex-1.2.3/casex/obstacle_simulation.py
+-rw-rw-rw-   0        0        0     1306 2021-02-23 22:47:23.000000 casex-1.2.3/casex/temporary_testing_figures.py
+-rw-rw-rw-   0        0        0      472 2023-07-07 10:54:37.000000 casex-1.2.3/casex/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 08:54:43.000000 casex-1.2.3/casex.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-24 08:54:41.000000 casex-1.2.3/casex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2020-12-29 10:07:56.000000 casex-1.2.3/casex.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     2789 2023-07-24 08:54:41.000000 casex-1.2.3/casex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       41 2023-07-24 08:54:41.000000 casex-1.2.3/casex.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      627 2023-07-24 08:54:41.000000 casex-1.2.3/casex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        6 2023-07-24 08:54:41.000000 casex-1.2.3/casex.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      119 2020-10-20 09:11:26.000000 casex-1.2.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     2789 2023-07-24 08:54:43.000000 casex-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2175 2023-03-01 14:11:00.000000 casex-1.2.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-24 08:54:43.000000 casex-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      946 2023-07-11 11:59:09.000000 casex-1.2.3/setup.py
```

### Comparing `casex-1.2.2/casex/aircraft_specs.py` & `casex-1.2.3/casex/aircraft_specs.py`

 * *Files identical despite different names*

### Comparing `casex-1.2.2/casex/annex_f_parms.py` & `casex-1.2.3/casex/annex_f_parms.py`

 * *Files identical despite different names*

### Comparing `casex-1.2.2/casex/annex_f_tables.py` & `casex-1.2.3/casex/annex_f_tables.py`

 * *Files 0% similar despite different names*

```diff
@@ -462,15 +462,15 @@
         # This setup cannot use a single impact angle, so it will be adjusted below.
         AFP = AnnexFParms()
         
         impact_speed = [0, 0, 0, 0, 0]
         impact_angle = [0, 0, 0, 0, 0]
         for c in range(5):
             if scenario == 1:
-                impact_angle[c] = 10 if c > 0 else 35
+                impact_angle[c] = 10# if c > 0 else 35
                 impact_speed[c] = AFP.CA_parms[c].glide_speed
             elif scenario == 2:
                 impact_angle[c] = 35
                 impact_speed[c] = AFP.CA_parms[c].cruise_speed
             elif scenario == 3:
                 impact_angle[c] = AFP.CA_parms[c].ballistic_impact_angle
                 impact_speed[c] = AFP.CA_parms[c].ballistic_impact_velocity
```

### Comparing `casex-1.2.2/casex/ballistic_descent_models.py` & `casex-1.2.3/casex/ballistic_descent_models.py`

 * *Files identical despite different names*

### Comparing `casex-1.2.2/casex/conversion.py` & `casex-1.2.3/casex/conversion.py`

 * *Files identical despite different names*

### Comparing `casex-1.2.2/casex/critical_area_models.py` & `casex-1.2.3/casex/critical_area_models.py`

 * *Files identical despite different names*

### Comparing `casex-1.2.2/casex/enums.py` & `casex-1.2.3/casex/enums.py`

 * *Files identical despite different names*

### Comparing `casex-1.2.2/casex/explosion_models.py` & `casex-1.2.3/casex/explosion_models.py`

 * *Files identical despite different names*

### Comparing `casex-1.2.2/casex/figures.py` & `casex-1.2.3/casex/figures.py`

 * *Files identical despite different names*

### Comparing `casex-1.2.2/casex/friction_coefficient.py` & `casex-1.2.3/casex/friction_coefficient.py`

 * *Files identical despite different names*

### Comparing `casex-1.2.2/casex/ground_risk_buffer.py` & `casex-1.2.3/casex/ground_risk_buffer.py`

 * *Files identical despite different names*

### Comparing `casex-1.2.2/casex/misc.py` & `casex-1.2.3/casex/misc.py`

 * *Files identical despite different names*

### Comparing `casex-1.2.2/casex/obstacles.py` & `casex-1.2.3/casex/obstacles.py`

 * *Files identical despite different names*

### Comparing `casex-1.2.2/casex/obstacle_simulation.py` & `casex-1.2.3/casex/obstacle_simulation.py`

 * *Files identical despite different names*

### Comparing `casex-1.2.2/casex/temporary_testing_figures.py` & `casex-1.2.3/casex/temporary_testing_figures.py`

 * *Files identical despite different names*

### Comparing `casex-1.2.2/casex.egg-info/PKG-INFO` & `casex-1.2.3/casex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casex
-Version: 1.2.2
+Version: 1.2.3
 Summary: Casualty expectation toolbox
 Home-page: UNKNOWN
 Author: Anders la Cour-Harbo et al
 Author-email: anders@lacourfamily.dk
 License: CC-BY-4.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `casex-1.2.2/casex.egg-info/SOURCES.txt` & `casex-1.2.3/casex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `casex-1.2.2/PKG-INFO` & `casex-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casex
-Version: 1.2.2
+Version: 1.2.3
 Summary: Casualty expectation toolbox
 Home-page: UNKNOWN
 Author: Anders la Cour-Harbo et al
 Author-email: anders@lacourfamily.dk
 License: CC-BY-4.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `casex-1.2.2/README.md` & `casex-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `casex-1.2.2/setup.py` & `casex-1.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='casex',
-    version='1.2.2',
+    version='1.2.3',
     description='Casualty expectation toolbox',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'License :: Other/Proprietary License',
         'Programming Language :: Python :: 3.7',
```

