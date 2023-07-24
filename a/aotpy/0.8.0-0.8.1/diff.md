# Comparing `tmp/aotpy-0.8.0.tar.gz` & `tmp/aotpy-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aotpy-0.8.0.tar", last modified: Mon Jul 17 15:39:51 2023, max compression
+gzip compressed data, was "aotpy-0.8.1.tar", last modified: Mon Jul 24 13:09:45 2023, max compression
```

## Comparing `aotpy-0.8.0.tar` & `aotpy-0.8.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 15:39:51.578629 aotpy-0.8.0/
--rw-rw-rw-   0        0        0     1592 2022-07-17 01:57:35.000000 aotpy-0.8.0/LICENSE
--rw-rw-rw-   0        0        0     2997 2023-07-17 15:39:51.578629 aotpy-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     2198 2023-05-02 22:45:22.000000 aotpy-0.8.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 15:39:51.527659 aotpy-0.8.0/aotpy/
--rw-rw-rw-   0        0        0      521 2023-05-03 10:25:00.000000 aotpy-0.8.0/aotpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 15:39:51.545372 aotpy-0.8.0/aotpy/core/
--rw-rw-rw-   0        0        0      555 2023-05-08 11:52:45.000000 aotpy-0.8.0/aotpy/core/__init__.py
--rw-rw-rw-   0        0        0     1073 2023-05-02 09:36:00.000000 aotpy-0.8.0/aotpy/core/aberration.py
--rw-rw-rw-   0        0        0     5304 2023-07-17 15:34:04.000000 aotpy-0.8.0/aotpy/core/ao_system.py
--rw-rw-rw-   0        0        0     3050 2023-07-17 15:15:05.000000 aotpy-0.8.0/aotpy/core/atmosphere.py
--rw-rw-rw-   0        0        0     1162 2023-07-17 10:40:27.000000 aotpy-0.8.0/aotpy/core/base.py
--rw-rw-rw-   0        0        0     1338 2023-07-17 12:24:43.000000 aotpy-0.8.0/aotpy/core/image.py
--rw-rw-rw-   0        0        0     5293 2023-07-17 15:13:26.000000 aotpy-0.8.0/aotpy/core/loop.py
--rw-rw-rw-   0        0        0    11452 2023-05-08 11:39:26.000000 aotpy-0.8.0/aotpy/core/optical_sensor.py
--rw-rw-rw-   0        0        0     2863 2023-05-22 10:44:57.000000 aotpy-0.8.0/aotpy/core/source.py
--rw-rw-rw-   0        0        0     4887 2023-06-19 16:50:55.000000 aotpy-0.8.0/aotpy/core/telescope.py
--rw-rw-rw-   0        0        0      706 2023-06-19 16:50:55.000000 aotpy-0.8.0/aotpy/core/time.py
--rw-rw-rw-   0        0        0     3552 2023-07-17 10:39:59.000000 aotpy-0.8.0/aotpy/core/wavefront_corrector.py
-drwxrwxrwx   0        0        0        0 2023-07-17 15:39:51.546372 aotpy-0.8.0/aotpy/data/
-drwxrwxrwx   0        0        0        0 2023-07-17 15:39:51.548372 aotpy-0.8.0/aotpy/data/ERIS/
--rw-rw-rw-   0        0        0    11520 2023-04-03 16:42:38.000000 aotpy-0.8.0/aotpy/data/ERIS/ho_subap.fits
--rw-rw-rw-   0        0        0     5760 2023-06-19 12:38:42.000000 aotpy-0.8.0/aotpy/data/ERIS/lo_subap.fits
-drwxrwxrwx   0        0        0        0 2023-07-17 15:39:51.549372 aotpy-0.8.0/aotpy/data/GALACSI/
--rw-rw-rw-   0        0        0    11520 2023-04-03 16:42:38.000000 aotpy-0.8.0/aotpy/data/GALACSI/subap.fits
-drwxrwxrwx   0        0        0        0 2023-07-17 15:39:51.550372 aotpy-0.8.0/aotpy/data/NAOMI/
--rw-rw-rw-   0        0        0  7344000 2023-05-03 14:12:48.000000 aotpy-0.8.0/aotpy/data/NAOMI/zernike_control_modes.fits
-drwxrwxrwx   0        0        0        0 2023-07-17 15:39:51.559459 aotpy-0.8.0/aotpy/data/PAPYRUS/
--rw-rw-rw-   0        0        0  1013760 2023-06-19 15:05:10.000000 aotpy-0.8.0/aotpy/data/PAPYRUS/T152_pupil.fits
--rw-rw-rw-   0        0        0      105 2023-05-02 18:50:46.000000 aotpy-0.8.0/aotpy/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 15:39:51.563459 aotpy-0.8.0/aotpy/io/
--rw-rw-rw-   0        0        0      436 2023-06-19 16:50:12.000000 aotpy-0.8.0/aotpy/io/__init__.py
--rw-rw-rw-   0        0        0     2789 2023-06-19 16:50:12.000000 aotpy-0.8.0/aotpy/io/base.py
-drwxrwxrwx   0        0        0        0 2023-07-17 15:39:51.568543 aotpy-0.8.0/aotpy/io/fits/
--rw-rw-rw-   0        0        0      200 2023-05-02 13:23:11.000000 aotpy-0.8.0/aotpy/io/fits/__init__.py
--rw-rw-rw-   0        0        0    26755 2023-07-17 08:56:36.000000 aotpy-0.8.0/aotpy/io/fits/_keywords.py
--rw-rw-rw-   0        0        0    41933 2023-07-06 15:43:11.000000 aotpy-0.8.0/aotpy/io/fits/reader.py
--rw-rw-rw-   0        0        0     9284 2023-06-28 16:40:48.000000 aotpy-0.8.0/aotpy/io/fits/utils.py
--rw-rw-rw-   0        0        0    31367 2023-07-17 09:16:43.000000 aotpy-0.8.0/aotpy/io/fits/writer.py
-drwxrwxrwx   0        0        0        0 2023-07-17 15:39:51.577633 aotpy-0.8.0/aotpy/translators/
--rw-rw-rw-   0        0        0      440 2023-06-28 16:02:08.000000 aotpy-0.8.0/aotpy/translators/__init__.py
--rw-rw-rw-   0        0        0      981 2023-06-19 16:46:11.000000 aotpy-0.8.0/aotpy/translators/base.py
--rw-rw-rw-   0        0        0     7087 2023-07-06 15:43:34.000000 aotpy-0.8.0/aotpy/translators/ciao.py
--rw-rw-rw-   0        0        0    18377 2023-07-06 15:47:56.000000 aotpy-0.8.0/aotpy/translators/eris.py
--rw-rw-rw-   0        0        0    10376 2023-06-28 16:36:06.000000 aotpy-0.8.0/aotpy/translators/eso.py
--rw-rw-rw-   0        0        0    11408 2023-07-06 15:45:27.000000 aotpy-0.8.0/aotpy/translators/galacsi.py
--rw-rw-rw-   0        0        0     7494 2023-07-06 15:45:40.000000 aotpy-0.8.0/aotpy/translators/naomi.py
--rw-rw-rw-   0        0        0     3658 2023-07-17 15:15:43.000000 aotpy-0.8.0/aotpy/translators/papyrus.py
-drwxrwxrwx   0        0        0        0 2023-07-17 15:39:51.532658 aotpy-0.8.0/aotpy.egg-info/
--rw-rw-rw-   0        0        0     2997 2023-07-17 15:39:51.000000 aotpy-0.8.0/aotpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1058 2023-07-17 15:39:51.000000 aotpy-0.8.0/aotpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 15:39:51.000000 aotpy-0.8.0/aotpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      138 2023-07-17 15:39:51.000000 aotpy-0.8.0/aotpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-17 15:39:51.000000 aotpy-0.8.0/aotpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2021-11-05 13:42:41.000000 aotpy-0.8.0/pyproject.toml
--rw-rw-rw-   0        0        0     1029 2023-07-17 15:39:51.579630 aotpy-0.8.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-24 13:09:45.002474 aotpy-0.8.1/
+-rw-rw-rw-   0        0        0     1592 2022-07-17 01:57:35.000000 aotpy-0.8.1/LICENSE
+-rw-rw-rw-   0        0        0     2997 2023-07-24 13:09:45.002474 aotpy-0.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2198 2023-05-02 22:45:22.000000 aotpy-0.8.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 13:09:44.938486 aotpy-0.8.1/aotpy/
+-rw-rw-rw-   0        0        0      521 2023-05-03 10:25:00.000000 aotpy-0.8.1/aotpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 13:09:44.958016 aotpy-0.8.1/aotpy/core/
+-rw-rw-rw-   0        0        0      555 2023-05-08 11:52:45.000000 aotpy-0.8.1/aotpy/core/__init__.py
+-rw-rw-rw-   0        0        0     1073 2023-05-02 09:36:00.000000 aotpy-0.8.1/aotpy/core/aberration.py
+-rw-rw-rw-   0        0        0     5304 2023-07-24 12:45:59.000000 aotpy-0.8.1/aotpy/core/ao_system.py
+-rw-rw-rw-   0        0        0     3050 2023-07-17 15:15:05.000000 aotpy-0.8.1/aotpy/core/atmosphere.py
+-rw-rw-rw-   0        0        0     1162 2023-07-24 12:45:59.000000 aotpy-0.8.1/aotpy/core/base.py
+-rw-rw-rw-   0        0        0     1338 2023-07-24 12:45:59.000000 aotpy-0.8.1/aotpy/core/image.py
+-rw-rw-rw-   0        0        0     5293 2023-07-17 15:13:26.000000 aotpy-0.8.1/aotpy/core/loop.py
+-rw-rw-rw-   0        0        0    11452 2023-05-08 11:39:26.000000 aotpy-0.8.1/aotpy/core/optical_sensor.py
+-rw-rw-rw-   0        0        0     2863 2023-05-22 10:44:57.000000 aotpy-0.8.1/aotpy/core/source.py
+-rw-rw-rw-   0        0        0     4887 2023-06-19 16:50:55.000000 aotpy-0.8.1/aotpy/core/telescope.py
+-rw-rw-rw-   0        0        0      706 2023-06-19 16:50:55.000000 aotpy-0.8.1/aotpy/core/time.py
+-rw-rw-rw-   0        0        0     3552 2023-07-17 10:39:59.000000 aotpy-0.8.1/aotpy/core/wavefront_corrector.py
+drwxrwxrwx   0        0        0        0 2023-07-24 13:09:44.958994 aotpy-0.8.1/aotpy/data/
+drwxrwxrwx   0        0        0        0 2023-07-24 13:09:44.961924 aotpy-0.8.1/aotpy/data/ERIS/
+-rw-rw-rw-   0        0        0    11520 2023-04-03 16:42:38.000000 aotpy-0.8.1/aotpy/data/ERIS/ho_subap.fits
+-rw-rw-rw-   0        0        0     5760 2023-06-19 12:38:42.000000 aotpy-0.8.1/aotpy/data/ERIS/lo_subap.fits
+drwxrwxrwx   0        0        0        0 2023-07-24 13:09:44.963876 aotpy-0.8.1/aotpy/data/GALACSI/
+-rw-rw-rw-   0        0        0    11520 2023-07-24 12:45:59.000000 aotpy-0.8.1/aotpy/data/GALACSI/subap.fits
+drwxrwxrwx   0        0        0        0 2023-07-24 13:09:44.964852 aotpy-0.8.1/aotpy/data/NAOMI/
+-rw-rw-rw-   0        0        0  7344000 2023-05-03 14:12:48.000000 aotpy-0.8.1/aotpy/data/NAOMI/zernike_control_modes.fits
+drwxrwxrwx   0        0        0        0 2023-07-24 13:09:44.980988 aotpy-0.8.1/aotpy/data/PAPYRUS/
+-rw-rw-rw-   0        0        0  1013760 2023-06-19 15:05:10.000000 aotpy-0.8.1/aotpy/data/PAPYRUS/T152_pupil.fits
+-rw-rw-rw-   0        0        0      105 2023-05-02 18:50:46.000000 aotpy-0.8.1/aotpy/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 13:09:44.984893 aotpy-0.8.1/aotpy/io/
+-rw-rw-rw-   0        0        0      436 2023-06-19 16:50:12.000000 aotpy-0.8.1/aotpy/io/__init__.py
+-rw-rw-rw-   0        0        0     2789 2023-06-19 16:50:12.000000 aotpy-0.8.1/aotpy/io/base.py
+drwxrwxrwx   0        0        0        0 2023-07-24 13:09:44.991728 aotpy-0.8.1/aotpy/io/fits/
+-rw-rw-rw-   0        0        0      200 2023-05-02 13:23:11.000000 aotpy-0.8.1/aotpy/io/fits/__init__.py
+-rw-rw-rw-   0        0        0    26755 2023-07-24 12:45:59.000000 aotpy-0.8.1/aotpy/io/fits/_keywords.py
+-rw-rw-rw-   0        0        0    41933 2023-07-24 12:45:59.000000 aotpy-0.8.1/aotpy/io/fits/reader.py
+-rw-rw-rw-   0        0        0     9313 2023-07-24 13:06:09.000000 aotpy-0.8.1/aotpy/io/fits/utils.py
+-rw-rw-rw-   0        0        0    31367 2023-07-24 12:45:59.000000 aotpy-0.8.1/aotpy/io/fits/writer.py
+drwxrwxrwx   0        0        0        0 2023-07-24 13:09:45.000517 aotpy-0.8.1/aotpy/translators/
+-rw-rw-rw-   0        0        0      440 2023-07-24 12:45:59.000000 aotpy-0.8.1/aotpy/translators/__init__.py
+-rw-rw-rw-   0        0        0      981 2023-06-19 16:46:11.000000 aotpy-0.8.1/aotpy/translators/base.py
+-rw-rw-rw-   0        0        0     7087 2023-07-24 12:45:59.000000 aotpy-0.8.1/aotpy/translators/ciao.py
+-rw-rw-rw-   0        0        0    18377 2023-07-24 12:45:59.000000 aotpy-0.8.1/aotpy/translators/eris.py
+-rw-rw-rw-   0        0        0    10376 2023-07-24 12:45:59.000000 aotpy-0.8.1/aotpy/translators/eso.py
+-rw-rw-rw-   0        0        0    11408 2023-07-24 12:45:59.000000 aotpy-0.8.1/aotpy/translators/galacsi.py
+-rw-rw-rw-   0        0        0     7494 2023-07-24 12:45:59.000000 aotpy-0.8.1/aotpy/translators/naomi.py
+-rw-rw-rw-   0        0        0    12582 2023-07-24 13:05:57.000000 aotpy-0.8.1/aotpy/translators/papyrus.py
+drwxrwxrwx   0        0        0        0 2023-07-24 13:09:44.944345 aotpy-0.8.1/aotpy.egg-info/
+-rw-rw-rw-   0        0        0     2997 2023-07-24 13:09:44.000000 aotpy-0.8.1/aotpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1058 2023-07-24 13:09:44.000000 aotpy-0.8.1/aotpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 13:09:44.000000 aotpy-0.8.1/aotpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      138 2023-07-24 13:09:44.000000 aotpy-0.8.1/aotpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-24 13:09:44.000000 aotpy-0.8.1/aotpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2021-11-05 13:42:41.000000 aotpy-0.8.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1029 2023-07-24 13:09:45.003452 aotpy-0.8.1/setup.cfg
```

### Comparing `aotpy-0.8.0/LICENSE` & `aotpy-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.0/PKG-INFO` & `aotpy-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aotpy
-Version: 0.8.0
+Version: 0.8.1
 Summary: Helper package for handling Adaptive Optics Telemetry (AOT) standard files
 Home-page: https://github.com/STAR-PORT/aotpy
 Author: Tiago Gomes
 Author-email: tiagogomes@fe.up.pt
 Project-URL: Bug Tracker, https://github.com/STAR-PORT/aotpy/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aotpy-0.8.0/README.md` & `aotpy-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.0/aotpy/__init__.py` & `aotpy-0.8.1/aotpy/__init__.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.0/aotpy/core/__init__.py` & `aotpy-0.8.1/aotpy/core/__init__.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.0/aotpy/core/aberration.py` & `aotpy-0.8.1/aotpy/core/aberration.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.0/aotpy/core/ao_system.py` & `aotpy-0.8.1/aotpy/core/ao_system.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.0/aotpy/core/atmosphere.py` & `aotpy-0.8.1/aotpy/core/atmosphere.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.0/aotpy/core/base.py` & `aotpy-0.8.1/aotpy/core/base.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.0/aotpy/core/image.py` & `aotpy-0.8.1/aotpy/core/image.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.0/aotpy/core/loop.py` & `aotpy-0.8.1/aotpy/core/loop.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.0/aotpy/core/optical_sensor.py` & `aotpy-0.8.1/aotpy/core/optical_sensor.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.0/aotpy/core/source.py` & `aotpy-0.8.1/aotpy/core/source.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.0/aotpy/core/telescope.py` & `aotpy-0.8.1/aotpy/core/telescope.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.0/aotpy/core/time.py` & `aotpy-0.8.1/aotpy/core/time.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.0/aotpy/core/wavefront_corrector.py` & `aotpy-0.8.1/aotpy/core/wavefront_corrector.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.0/aotpy/data/ERIS/ho_subap.fits` & `aotpy-0.8.1/aotpy/data/ERIS/ho_subap.fits`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.0/aotpy/data/ERIS/lo_subap.fits` & `aotpy-0.8.1/aotpy/data/ERIS/lo_subap.fits`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.0/aotpy/data/GALACSI/subap.fits` & `aotpy-0.8.1/aotpy/data/GALACSI/subap.fits`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.0/aotpy/data/NAOMI/zernike_control_modes.fits` & `aotpy-0.8.1/aotpy/data/NAOMI/zernike_control_modes.fits`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.0/aotpy/data/PAPYRUS/T152_pupil.fits` & `aotpy-0.8.1/aotpy/data/PAPYRUS/T152_pupil.fits`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.0/aotpy/io/base.py` & `aotpy-0.8.1/aotpy/io/base.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.0/aotpy/io/fits/_keywords.py` & `aotpy-0.8.1/aotpy/io/fits/_keywords.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.0/aotpy/io/fits/reader.py` & `aotpy-0.8.1/aotpy/io/fits/reader.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.0/aotpy/io/fits/utils.py` & `aotpy-0.8.1/aotpy/io/fits/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,14 +186,15 @@
 
 
 def _get_image_fields_from_hdu(hdu) -> tuple[str, np.ndarray, str, str, list[aotpy.Metadatum]]:
     metadata = metadata_from_hdu(hdu)
     unit = None
     if (md := next((x for x in metadata if x.key == kw.IMAGE_UNIT), None)) is not None:
         unit = md.value
+        metadata.remove(md)
 
     _time = None
     if (md := next((x for x in metadata if x.key == kw.TIME_REFERENCE), None)) is not None:
         _time = md.value
         metadata.remove(md)
     return hdu.name, hdu.data, unit, _time, metadata
```

### Comparing `aotpy-0.8.0/aotpy/io/fits/writer.py` & `aotpy-0.8.1/aotpy/io/fits/writer.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.0/aotpy/translators/base.py` & `aotpy-0.8.1/aotpy/translators/base.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.0/aotpy/translators/ciao.py` & `aotpy-0.8.1/aotpy/translators/ciao.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.0/aotpy/translators/eris.py` & `aotpy-0.8.1/aotpy/translators/eris.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.0/aotpy/translators/eso.py` & `aotpy-0.8.1/aotpy/translators/eso.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.0/aotpy/translators/galacsi.py` & `aotpy-0.8.1/aotpy/translators/galacsi.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.0/aotpy/translators/naomi.py` & `aotpy-0.8.1/aotpy/translators/naomi.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.0/aotpy.egg-info/PKG-INFO` & `aotpy-0.8.1/aotpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aotpy
-Version: 0.8.0
+Version: 0.8.1
 Summary: Helper package for handling Adaptive Optics Telemetry (AOT) standard files
 Home-page: https://github.com/STAR-PORT/aotpy
 Author: Tiago Gomes
 Author-email: tiagogomes@fe.up.pt
 Project-URL: Bug Tracker, https://github.com/STAR-PORT/aotpy/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aotpy-0.8.0/aotpy.egg-info/SOURCES.txt` & `aotpy-0.8.1/aotpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.0/setup.cfg` & `aotpy-0.8.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 6f74 7079 0d0a 7665 7273 696f   = aotpy..versio
-00000020: 6e20 3d20 302e 382e 300d 0a61 7574 686f  n = 0.8.0..autho
+00000020: 6e20 3d20 302e 382e 310d 0a61 7574 686f  n = 0.8.1..autho
 00000030: 7220 3d20 5469 6167 6f20 476f 6d65 730d  r = Tiago Gomes.
 00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000050: 7469 6167 6f67 6f6d 6573 4066 652e 7570  tiagogomes@fe.up
 00000060: 2e70 740d 0a64 6573 6372 6970 7469 6f6e  .pt..description
 00000070: 203d 2048 656c 7065 7220 7061 636b 6167   = Helper packag
 00000080: 6520 666f 7220 6861 6e64 6c69 6e67 2041  e for handling A
 00000090: 6461 7074 6976 6520 4f70 7469 6373 2054  daptive Optics T
```

