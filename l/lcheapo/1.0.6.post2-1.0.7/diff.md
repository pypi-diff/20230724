# Comparing `tmp/lcheapo-1.0.6.post2.tar.gz` & `tmp/lcheapo-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lcheapo-1.0.6.post2.tar", last modified: Wed Dec  7 09:36:06 2022, max compression
+gzip compressed data, was "lcheapo-1.0.7.tar", last modified: Mon Jul 24 13:00:57 2023, max compression
```

## Comparing `lcheapo-1.0.6.post2.tar` & `lcheapo-1.0.7.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2022-12-07 09:36:06.485369 lcheapo-1.0.6.post2/
--rw-r--r--   0 crawford   (501) admin       (80)    35150 2019-02-11 14:51:26.000000 lcheapo-1.0.6.post2/LICENSE.txt
--rw-r--r--   0 crawford   (501) admin       (80)      100 2021-09-22 12:30:41.000000 lcheapo-1.0.6.post2/MANIFEST.in
--rw-r--r--   0 crawford   (501) admin       (80)     7894 2022-12-07 09:36:06.485078 lcheapo-1.0.6.post2/PKG-INFO
--rw-r--r--   0 crawford   (501) admin       (80)     7091 2022-06-22 18:23:03.000000 lcheapo-1.0.6.post2/README.md
--rw-r--r--   0 crawford   (501) admin       (80)      270 2021-09-27 09:46:39.000000 lcheapo-1.0.6.post2/ToDo.rst
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2022-12-07 09:36:06.477680 lcheapo-1.0.6.post2/lcheapo/
--rw-r--r--   0 crawford   (501) admin       (80)     2767 2020-03-12 01:05:36.000000 lcheapo-1.0.6.post2/lcheapo/Peterson_noise_model.py
--rw-r--r--   0 crawford   (501) admin       (80)      122 2021-09-23 11:48:54.000000 lcheapo-1.0.6.post2/lcheapo/__init__.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2022-12-07 09:36:06.480852 lcheapo-1.0.6.post2/lcheapo/_examples/
--rw-r--r--   0 crawford   (501) admin       (80)     1570 2021-09-22 13:11:02.000000 lcheapo-1.0.6.post2/lcheapo/_examples/BBOBS.lctest.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     1797 2019-09-05 15:51:08.000000 lcheapo-1.0.6.post2/lcheapo/_examples/calc_spectral.py
--rwxr-xr-x   0 crawford   (501) admin       (80)     1513 2020-02-05 21:01:47.000000 lcheapo-1.0.6.post2/lcheapo/_examples/lc_print_bad_times.py
--rw-r--r--   0 crawford   (501) admin       (80)     1879 2021-09-22 13:10:53.000000 lcheapo-1.0.6.post2/lcheapo/_examples/stations.lctest.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     7792 2021-09-22 13:10:38.000000 lcheapo-1.0.6.post2/lcheapo/_examples/tests.lctest.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      241 2021-03-24 16:42:41.000000 lcheapo-1.0.6.post2/lcheapo/chan_maps.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2022-12-07 09:36:06.482862 lcheapo-1.0.6.post2/lcheapo/data/
--rw-r--r--   0 crawford   (501) admin       (80)   239680 2021-04-08 15:15:36.000000 lcheapo-1.0.6.post2/lcheapo/data/BBOBS1.station.xml
--rw-r--r--   0 crawford   (501) admin       (80)   309388 2020-10-30 11:33:58.000000 lcheapo-1.0.6.post2/lcheapo/data/HYDROCT.station.xml
--rw-r--r--   0 crawford   (501) admin       (80)   310464 2020-03-12 17:51:52.000000 lcheapo-1.0.6.post2/lcheapo/data/SPOBS2.station.xml
--rw-r--r--   0 crawford   (501) admin       (80)    11426 2022-06-24 13:21:51.000000 lcheapo-1.0.6.post2/lcheapo/data/lctest.schema.json
--rw-r--r--   0 crawford   (501) admin       (80)    10166 2022-09-14 09:01:32.000000 lcheapo-1.0.6.post2/lcheapo/lc2SDS.py
--rw-r--r--   0 crawford   (501) admin       (80)     3477 2021-09-27 09:42:22.000000 lcheapo-1.0.6.post2/lcheapo/lc2ms.py
--rwxr-xr-x   0 crawford   (501) admin       (80)     4931 2022-12-06 17:20:31.000000 lcheapo-1.0.6.post2/lcheapo/lccut.py
--rwxr-xr-x   0 crawford   (501) admin       (80)     5568 2022-09-14 09:01:56.000000 lcheapo-1.0.6.post2/lcheapo/lcdump.py
--rwxr-xr-x   0 crawford   (501) admin       (80)    34614 2022-09-14 09:01:21.000000 lcheapo-1.0.6.post2/lcheapo/lcfix.py
--rwxr-xr-x   0 crawford   (501) admin       (80)    13157 2022-12-06 22:13:37.000000 lcheapo-1.0.6.post2/lcheapo/lcheader.py
--rwxr-xr-x   0 crawford   (501) admin       (80)    17009 2022-09-14 09:01:51.000000 lcheapo-1.0.6.post2/lcheapo/lcheapo_utils.py
--rwxr-xr-x   0 crawford   (501) admin       (80)     4168 2022-09-14 09:05:31.000000 lcheapo-1.0.6.post2/lcheapo/lcinfo.py
--rw-r--r--   0 crawford   (501) admin       (80)     5821 2022-09-14 09:01:44.000000 lcheapo-1.0.6.post2/lcheapo/lcplot.py
--rw-r--r--   0 crawford   (501) admin       (80)     1219 2022-09-14 09:05:47.000000 lcheapo-1.0.6.post2/lcheapo/lcputexamples.py
--rw-r--r--   0 crawford   (501) admin       (80)    19759 2022-09-14 09:01:39.000000 lcheapo-1.0.6.post2/lcheapo/lcread.py
--rw-r--r--   0 crawford   (501) admin       (80)    22164 2022-12-07 09:33:51.000000 lcheapo-1.0.6.post2/lcheapo/lctest.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2022-12-07 09:36:06.484638 lcheapo-1.0.6.post2/lcheapo/sdpchain/
--rw-r--r--   0 crawford   (501) admin       (80)     1783 2021-09-23 12:05:17.000000 lcheapo-1.0.6.post2/lcheapo/sdpchain/__init__.py
--rwxr-xr-x   0 crawford   (501) admin       (80)     5954 2021-09-13 14:11:22.000000 lcheapo-1.0.6.post2/lcheapo/sdpchain/argument_parser.py
--rwxr-xr-x   0 crawford   (501) admin       (80)     8222 2022-12-06 17:17:43.000000 lcheapo-1.0.6.post2/lcheapo/sdpchain/process_steps.py
--rwxr-xr-x   0 crawford   (501) admin       (80)     2571 2021-09-23 11:04:59.000000 lcheapo-1.0.6.post2/lcheapo/sdpchain/sdpcat.py
--rwxr--r--   0 crawford   (501) admin       (80)     6727 2021-09-23 11:04:42.000000 lcheapo-1.0.6.post2/lcheapo/sdpchain/sdpstep.py
--rw-r--r--   0 crawford   (501) admin       (80)       26 2021-06-16 16:43:57.000000 lcheapo-1.0.6.post2/lcheapo/sdpchain/version.py
--rw-r--r--   0 crawford   (501) admin       (80)    18555 2020-03-13 22:37:03.000000 lcheapo-1.0.6.post2/lcheapo/spectral.py
--rw-r--r--   0 crawford   (501) admin       (80)       26 2022-12-07 09:34:47.000000 lcheapo-1.0.6.post2/lcheapo/version.py
--rw-r--r--   0 crawford   (501) admin       (80)     8273 2021-07-19 20:52:06.000000 lcheapo-1.0.6.post2/lcheapo/yaml_json.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2022-12-07 09:36:06.479413 lcheapo-1.0.6.post2/lcheapo.egg-info/
--rw-r--r--   0 crawford   (501) admin       (80)     7894 2022-12-07 09:36:06.000000 lcheapo-1.0.6.post2/lcheapo.egg-info/PKG-INFO
--rw-r--r--   0 crawford   (501) admin       (80)     1098 2022-12-07 09:36:06.000000 lcheapo-1.0.6.post2/lcheapo.egg-info/SOURCES.txt
--rw-r--r--   0 crawford   (501) admin       (80)        1 2022-12-07 09:36:06.000000 lcheapo-1.0.6.post2/lcheapo.egg-info/dependency_links.txt
--rw-r--r--   0 crawford   (501) admin       (80)      399 2022-12-07 09:36:06.000000 lcheapo-1.0.6.post2/lcheapo.egg-info/entry_points.txt
--rw-r--r--   0 crawford   (501) admin       (80)       81 2022-12-07 09:36:06.000000 lcheapo-1.0.6.post2/lcheapo.egg-info/requires.txt
--rw-r--r--   0 crawford   (501) admin       (80)        8 2022-12-07 09:36:06.000000 lcheapo-1.0.6.post2/lcheapo.egg-info/top_level.txt
--rw-r--r--   0 crawford   (501) admin       (80)       38 2022-12-07 09:36:06.485459 lcheapo-1.0.6.post2/setup.cfg
--rw-r--r--   0 crawford   (501) admin       (80)     2150 2022-12-07 09:12:56.000000 lcheapo-1.0.6.post2/setup.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-07-24 13:00:57.992000 lcheapo-1.0.7/
+-rw-r--r--   0 crawford   (501) admin       (80)    35150 2019-02-11 14:51:26.000000 lcheapo-1.0.7/LICENSE.txt
+-rw-r--r--   0 crawford   (501) admin       (80)      100 2021-09-22 12:30:41.000000 lcheapo-1.0.7/MANIFEST.in
+-rw-r--r--   0 crawford   (501) admin       (80)     7888 2023-07-24 13:00:57.991691 lcheapo-1.0.7/PKG-INFO
+-rw-r--r--   0 crawford   (501) admin       (80)     7091 2022-06-22 18:23:03.000000 lcheapo-1.0.7/README.md
+-rw-r--r--   0 crawford   (501) admin       (80)      270 2021-09-27 09:46:39.000000 lcheapo-1.0.7/ToDo.rst
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-07-24 13:00:57.983890 lcheapo-1.0.7/lcheapo/
+-rw-r--r--   0 crawford   (501) admin       (80)     2767 2020-03-12 01:05:36.000000 lcheapo-1.0.7/lcheapo/Peterson_noise_model.py
+-rw-r--r--   0 crawford   (501) admin       (80)      122 2021-09-23 11:48:54.000000 lcheapo-1.0.7/lcheapo/__init__.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-07-24 13:00:57.987125 lcheapo-1.0.7/lcheapo/_examples/
+-rw-r--r--   0 crawford   (501) admin       (80)     1570 2021-09-22 13:11:02.000000 lcheapo-1.0.7/lcheapo/_examples/BBOBS.lctest.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1797 2019-09-05 15:51:08.000000 lcheapo-1.0.7/lcheapo/_examples/calc_spectral.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)     1513 2020-02-05 21:01:47.000000 lcheapo-1.0.7/lcheapo/_examples/lc_print_bad_times.py
+-rw-r--r--   0 crawford   (501) admin       (80)     1879 2021-09-22 13:10:53.000000 lcheapo-1.0.7/lcheapo/_examples/stations.lctest.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     7792 2021-09-22 13:10:38.000000 lcheapo-1.0.7/lcheapo/_examples/tests.lctest.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      241 2021-03-24 16:42:41.000000 lcheapo-1.0.7/lcheapo/chan_maps.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-07-24 13:00:57.989266 lcheapo-1.0.7/lcheapo/data/
+-rw-r--r--   0 crawford   (501) admin       (80)   239680 2021-04-08 15:15:36.000000 lcheapo-1.0.7/lcheapo/data/BBOBS1.station.xml
+-rw-r--r--   0 crawford   (501) admin       (80)   309388 2020-10-30 11:33:58.000000 lcheapo-1.0.7/lcheapo/data/HYDROCT.station.xml
+-rw-r--r--   0 crawford   (501) admin       (80)   310464 2020-03-12 17:51:52.000000 lcheapo-1.0.7/lcheapo/data/SPOBS2.station.xml
+-rw-r--r--   0 crawford   (501) admin       (80)    11426 2022-06-24 13:21:51.000000 lcheapo-1.0.7/lcheapo/data/lctest.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)    10166 2022-09-14 09:01:32.000000 lcheapo-1.0.7/lcheapo/lc2SDS.py
+-rw-r--r--   0 crawford   (501) admin       (80)     3620 2023-07-24 12:59:04.000000 lcheapo-1.0.7/lcheapo/lc2ms.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)     4931 2022-12-06 17:20:31.000000 lcheapo-1.0.7/lcheapo/lccut.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)     5568 2022-09-14 09:01:56.000000 lcheapo-1.0.7/lcheapo/lcdump.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)    34614 2022-09-14 09:01:21.000000 lcheapo-1.0.7/lcheapo/lcfix.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)    13157 2022-12-06 22:13:37.000000 lcheapo-1.0.7/lcheapo/lcheader.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)    17009 2022-09-14 09:01:51.000000 lcheapo-1.0.7/lcheapo/lcheapo_utils.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)     4168 2022-09-14 09:05:31.000000 lcheapo-1.0.7/lcheapo/lcinfo.py
+-rw-r--r--   0 crawford   (501) admin       (80)     5821 2022-09-14 09:01:44.000000 lcheapo-1.0.7/lcheapo/lcplot.py
+-rw-r--r--   0 crawford   (501) admin       (80)     1219 2022-09-14 09:05:47.000000 lcheapo-1.0.7/lcheapo/lcputexamples.py
+-rw-r--r--   0 crawford   (501) admin       (80)    19759 2022-09-14 09:01:39.000000 lcheapo-1.0.7/lcheapo/lcread.py
+-rw-r--r--   0 crawford   (501) admin       (80)    22166 2023-07-24 12:59:04.000000 lcheapo-1.0.7/lcheapo/lctest.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-07-24 13:00:57.991312 lcheapo-1.0.7/lcheapo/sdpchain/
+-rw-r--r--   0 crawford   (501) admin       (80)     1783 2021-09-23 12:05:17.000000 lcheapo-1.0.7/lcheapo/sdpchain/__init__.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)     5954 2021-09-13 14:11:22.000000 lcheapo-1.0.7/lcheapo/sdpchain/argument_parser.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)     8222 2023-07-24 12:59:04.000000 lcheapo-1.0.7/lcheapo/sdpchain/process_steps.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)     2574 2023-07-24 12:59:04.000000 lcheapo-1.0.7/lcheapo/sdpchain/sdpcat.py
+-rwxr--r--   0 crawford   (501) admin       (80)     6727 2021-09-23 11:04:42.000000 lcheapo-1.0.7/lcheapo/sdpchain/sdpstep.py
+-rw-r--r--   0 crawford   (501) admin       (80)       26 2021-06-16 16:43:57.000000 lcheapo-1.0.7/lcheapo/sdpchain/version.py
+-rw-r--r--   0 crawford   (501) admin       (80)    18555 2020-03-13 22:37:03.000000 lcheapo-1.0.7/lcheapo/spectral.py
+-rw-r--r--   0 crawford   (501) admin       (80)       20 2023-07-24 12:59:04.000000 lcheapo-1.0.7/lcheapo/version.py
+-rw-r--r--   0 crawford   (501) admin       (80)     8273 2021-07-19 20:52:06.000000 lcheapo-1.0.7/lcheapo/yaml_json.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-07-24 13:00:57.985556 lcheapo-1.0.7/lcheapo.egg-info/
+-rw-r--r--   0 crawford   (501) admin       (80)     7888 2023-07-24 13:00:57.000000 lcheapo-1.0.7/lcheapo.egg-info/PKG-INFO
+-rw-r--r--   0 crawford   (501) admin       (80)     1098 2023-07-24 13:00:57.000000 lcheapo-1.0.7/lcheapo.egg-info/SOURCES.txt
+-rw-r--r--   0 crawford   (501) admin       (80)        1 2023-07-24 13:00:57.000000 lcheapo-1.0.7/lcheapo.egg-info/dependency_links.txt
+-rw-r--r--   0 crawford   (501) admin       (80)      399 2023-07-24 13:00:57.000000 lcheapo-1.0.7/lcheapo.egg-info/entry_points.txt
+-rw-r--r--   0 crawford   (501) admin       (80)       79 2023-07-24 13:00:57.000000 lcheapo-1.0.7/lcheapo.egg-info/requires.txt
+-rw-r--r--   0 crawford   (501) admin       (80)        8 2023-07-24 13:00:57.000000 lcheapo-1.0.7/lcheapo.egg-info/top_level.txt
+-rw-r--r--   0 crawford   (501) admin       (80)       38 2023-07-24 13:00:57.992153 lcheapo-1.0.7/setup.cfg
+-rw-r--r--   0 crawford   (501) admin       (80)     2148 2023-07-24 13:00:49.000000 lcheapo-1.0.7/setup.py
```

### Comparing `lcheapo-1.0.6.post2/LICENSE.txt` & `lcheapo-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lcheapo-1.0.6.post2/PKG-INFO` & `lcheapo-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcheapo
-Version: 1.0.6.post2
+Version: 1.0.7
 Summary: LCHEAPO data routines
 Home-page: https://github.com/WayneCrawford/lcheapo
 Author: Wayne Crawford
 Author-email: crawford@ipgp.fr
 Keywords: oceanography,marine,OBS
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `lcheapo-1.0.6.post2/README.md` & `lcheapo-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `lcheapo-1.0.6.post2/lcheapo/Peterson_noise_model.py` & `lcheapo-1.0.7/lcheapo/Peterson_noise_model.py`

 * *Files identical despite different names*

### Comparing `lcheapo-1.0.6.post2/lcheapo/_examples/BBOBS.lctest.yaml` & `lcheapo-1.0.7/lcheapo/_examples/BBOBS.lctest.yaml`

 * *Files identical despite different names*

### Comparing `lcheapo-1.0.6.post2/lcheapo/_examples/calc_spectral.py` & `lcheapo-1.0.7/lcheapo/_examples/calc_spectral.py`

 * *Files identical despite different names*

### Comparing `lcheapo-1.0.6.post2/lcheapo/_examples/lc_print_bad_times.py` & `lcheapo-1.0.7/lcheapo/_examples/lc_print_bad_times.py`

 * *Files identical despite different names*

### Comparing `lcheapo-1.0.6.post2/lcheapo/_examples/stations.lctest.yaml` & `lcheapo-1.0.7/lcheapo/_examples/stations.lctest.yaml`

 * *Files identical despite different names*

### Comparing `lcheapo-1.0.6.post2/lcheapo/_examples/tests.lctest.yaml` & `lcheapo-1.0.7/lcheapo/_examples/tests.lctest.yaml`

 * *Files identical despite different names*

### Comparing `lcheapo-1.0.6.post2/lcheapo/data/BBOBS1.station.xml` & `lcheapo-1.0.7/lcheapo/data/BBOBS1.station.xml`

 * *Files identical despite different names*

### Comparing `lcheapo-1.0.6.post2/lcheapo/data/HYDROCT.station.xml` & `lcheapo-1.0.7/lcheapo/data/HYDROCT.station.xml`

 * *Files identical despite different names*

### Comparing `lcheapo-1.0.6.post2/lcheapo/data/SPOBS2.station.xml` & `lcheapo-1.0.7/lcheapo/data/SPOBS2.station.xml`

 * *Files identical despite different names*

### Comparing `lcheapo-1.0.6.post2/lcheapo/data/lctest.schema.json` & `lcheapo-1.0.7/lcheapo/data/lctest.schema.json`

 * *Files identical despite different names*

### Comparing `lcheapo-1.0.6.post2/lcheapo/lc2SDS.py` & `lcheapo-1.0.7/lcheapo/lc2SDS.py`

 * *Files identical despite different names*

### Comparing `lcheapo-1.0.6.post2/lcheapo/lc2ms.py` & `lcheapo-1.0.7/lcheapo/lc2ms.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,26 +50,29 @@
     args = parser.parse_args()
     parameters = vars(args).copy()
     if args.version is True:
         print(f"Version {__version__}")
         sys.exit(0)
 
     # ADJUST INPUT PARAMETERS
+    args.input_files = [args.infile]
     process_step = ProcessStep('lc2ms_weak',
                                " ".join(sys.argv),
                                app_description=__doc__,
                                app_version=__version__,
                                parameters=parameters)
     args.in_dir, args.out_dir, args.infiles = ProcessStep.setup_paths(args)
     # Expand captured wildcards
     # args.infiles = [x.name for f in args.infiles
     #                 for x in Path(args.in_dir).glob(f)]
 
     stream = lcread(Path(args.in_dir) / args.infile, network=args.network,
-                    station=args.station, obs_type=args.obs_type)
+                    station=args.station, obs_type=args.obs_type,
+                    starttime=0,
+                    endtime = 1*86400*365.25) # For up to 1 year of data
     out_dir = Path(args.out_dir)
     out_dir.mkdir(parents=True, exist_ok=True)
     out_files = []
     for tr in stream:
         s = tr.stats
         out_files.append(f'{s.network}.{s.station}.{s.location}.{s.channel}.mseed')
         fname = str(out_dir / out_files[-1])
```

### Comparing `lcheapo-1.0.6.post2/lcheapo/lccut.py` & `lcheapo-1.0.7/lcheapo/lccut.py`

 * *Files identical despite different names*

### Comparing `lcheapo-1.0.6.post2/lcheapo/lcdump.py` & `lcheapo-1.0.7/lcheapo/lcdump.py`

 * *Files identical despite different names*

### Comparing `lcheapo-1.0.6.post2/lcheapo/lcfix.py` & `lcheapo-1.0.7/lcheapo/lcfix.py`

 * *Files identical despite different names*

### Comparing `lcheapo-1.0.6.post2/lcheapo/lcheader.py` & `lcheapo-1.0.7/lcheapo/lcheader.py`

 * *Files identical despite different names*

### Comparing `lcheapo-1.0.6.post2/lcheapo/lcheapo_utils.py` & `lcheapo-1.0.7/lcheapo/lcheapo_utils.py`

 * *Files identical despite different names*

### Comparing `lcheapo-1.0.6.post2/lcheapo/lcinfo.py` & `lcheapo-1.0.7/lcheapo/lcinfo.py`

 * *Files identical despite different names*

### Comparing `lcheapo-1.0.6.post2/lcheapo/lcplot.py` & `lcheapo-1.0.7/lcheapo/lcplot.py`

 * *Files identical despite different names*

### Comparing `lcheapo-1.0.6.post2/lcheapo/lcputexamples.py` & `lcheapo-1.0.7/lcheapo/lcputexamples.py`

 * *Files identical despite different names*

### Comparing `lcheapo-1.0.6.post2/lcheapo/lcread.py` & `lcheapo-1.0.7/lcheapo/lcread.py`

 * *Files identical despite different names*

### Comparing `lcheapo-1.0.6.post2/lcheapo/lctest.py` & `lcheapo-1.0.7/lcheapo/lctest.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
 import jsonref
 import jsonschema
 from matplotlib import pyplot as plt
 from obspy.core import UTCDateTime, Stream
 from obspy.signal import PPSD
 # from crawtools.spectral import SpectralDensity  # PSDs
-from tiskit import SpectralDensity  # PSDs
+from tiskitpy import SpectralDensity  # PSDs
 
 from .lcread import read as lcread
 
 
 def main():
     """
     Read the yaml file and plot the specified tests
```

### Comparing `lcheapo-1.0.6.post2/lcheapo/sdpchain/__init__.py` & `lcheapo-1.0.7/lcheapo/sdpchain/__init__.py`

 * *Files identical despite different names*

### Comparing `lcheapo-1.0.6.post2/lcheapo/sdpchain/argument_parser.py` & `lcheapo-1.0.7/lcheapo/sdpchain/argument_parser.py`

 * *Files identical despite different names*

### Comparing `lcheapo-1.0.6.post2/lcheapo/sdpchain/process_steps.py` & `lcheapo-1.0.7/lcheapo/sdpchain/process_steps.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         tree = {}
         try:
             fp = open(in_file, "r")
         except FileNotFoundError:  # File not found
             pass
         else:   # File found
             if verbose is True:
-                write(f'\tFile exists, will append')
+                print(f'\tFile exists, will append')
             try:
                 tree = json.load(fp)
             except Exception:
                 # Couldn't read input file, don't overwrite it either
                 if in_file == out_file:
                     out_file = _unique_path(Path(out_dir),
                                                 'process-steps{:02d}.json')
```

### Comparing `lcheapo-1.0.6.post2/lcheapo/sdpchain/sdpcat.py` & `lcheapo-1.0.7/lcheapo/sdpchain/sdpcat.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     process_step = ProcessStep(
         'sdpcat',
         " ".join(sys.argv),
         app_description = __doc__,
         app_version = __version__,
         parameters=args)
 
-    args.in_dir, args.out_dir = ProcessStep.setup_paths(args)
+    args.in_dir, args.out_dir, _ = ProcessStep.setup_paths(args)
     # VERIFY THAT INPUT FILES EXIST AND OUTPUT FILE DOESN'T
     if len(args.input_files) < 2:
         print("You only provided 1 input file: this is just a copy!")
     for file in args.input_files:
         f = Path(args.in_dir) / file
         assert Path(f).is_file()
     assert (Path(args.out_dir) / args.output_file).exists() is False
```

### Comparing `lcheapo-1.0.6.post2/lcheapo/sdpchain/sdpstep.py` & `lcheapo-1.0.7/lcheapo/sdpchain/sdpstep.py`

 * *Files identical despite different names*

### Comparing `lcheapo-1.0.6.post2/lcheapo/spectral.py` & `lcheapo-1.0.7/lcheapo/spectral.py`

 * *Files identical despite different names*

### Comparing `lcheapo-1.0.6.post2/lcheapo/yaml_json.py` & `lcheapo-1.0.7/lcheapo/yaml_json.py`

 * *Files identical despite different names*

### Comparing `lcheapo-1.0.6.post2/lcheapo.egg-info/PKG-INFO` & `lcheapo-1.0.7/lcheapo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcheapo
-Version: 1.0.6.post2
+Version: 1.0.7
 Summary: LCHEAPO data routines
 Home-page: https://github.com/WayneCrawford/lcheapo
 Author: Wayne Crawford
 Author-email: crawford@ipgp.fr
 Keywords: oceanography,marine,OBS
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `lcheapo-1.0.6.post2/lcheapo.egg-info/SOURCES.txt` & `lcheapo-1.0.7/lcheapo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lcheapo-1.0.6.post2/setup.py` & `lcheapo-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,19 +20,19 @@
     include_package_data=True,
     # packages=['lcheapo'],
     # package_dir={'lcheapo': 'lcheapo'},
     # package_data={'lcheapo': ['data/*.xml', 'data/*.json',
     #                                 '_examples/*.py', '_examples/*.yaml']},
     install_requires=[
           'obspy>=1.1',
-          'pyyaml>5.0'
+          'pyyaml>5.0',
           'jsonschema>=2.6',
           'jsonref>=0.2',
           'progress>=1.5',
-          'tiskit-py>=0.3.1'
+          'tiskitpy>=0.4'
       ],
     entry_points={
          'console_scripts': [
              'sdpcat=lcheapo.sdpchain:sdpcat',
              'sdpstep=lcheapo.sdpchain:sdpstep',
              'lcfix=lcheapo.lcfix:main',
              'lcdump=lcheapo.lcdump:main',
```

