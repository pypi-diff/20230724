# Comparing `tmp/solo_epd_loader-0.3.3.tar.gz` & `tmp/solo_epd_loader-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solo_epd_loader-0.3.3.tar", last modified: Fri Jul 21 14:04:30 2023, max compression
+gzip compressed data, was "/home/gieseler/uni/solo/solo-epd-loader/dist/.tmp-kdtqsuqj/solo_epd_loader-0.3.4.tar", last modified: Mon Jul 24 13:34:24 2023, max compression
```

## Comparing `solo_epd_loader-0.3.3.tar` & `solo_epd_loader-0.3.4.tar`

### file list

```diff
@@ -1,36 +1,47 @@
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-21 14:04:30.466758 solo_epd_loader-0.3.3/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.3.3/LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      457 2022-03-01 17:04:02.000000 solo_epd_loader-0.3.3/MANIFEST.in
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16842 2023-07-21 14:04:30.466758 solo_epd_loader-0.3.3/PKG-INFO
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    15894 2023-07-20 13:53:21.000000 solo_epd_loader-0.3.3/README.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3370 2022-03-30 15:49:33.000000 solo_epd_loader-0.3.3/code_of_conduct.md
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-21 14:04:30.462758 solo_epd_loader-0.3.3/docs/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      634 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.3/docs/Makefile
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2312 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.3/docs/conf.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      379 2022-01-11 15:35:29.000000 solo_epd_loader-0.3.3/docs/index.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      760 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.3/docs/make.bat
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-21 14:04:30.466758 solo_epd_loader-0.3.3/examples/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-01-18 13:16:32.000000 solo_epd_loader-0.3.3/examples/gh2021_fig_2.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    72237 2021-05-19 13:25:57.000000 solo_epd_loader-0.3.3/examples/ws2021_fig_2d.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-28 12:32:34.000000 solo_epd_loader-0.3.3/gh2021_fig_2.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-25 16:10:07.000000 solo_epd_loader-0.3.3/gh2021_fig_2a.png
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-21 14:04:30.466758 solo_epd_loader-0.3.3/licenses/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.3.3/licenses/LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1308 2023-07-05 12:35:18.000000 solo_epd_loader-0.3.3/licenses/SUNPY_LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1659 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.3/licenses/TEMPLATE_LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      134 2022-03-01 17:04:02.000000 solo_epd_loader-0.3.3/pyproject.toml
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2309 2023-07-21 14:04:30.466758 solo_epd_loader-0.3.3/setup.cfg
--rwxrwxr-x   0 gieseler  (1000) gieseler  (1000)      666 2022-03-01 17:04:02.000000 solo_epd_loader-0.3.3/setup.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-21 14:04:30.466758 solo_epd_loader-0.3.3/solo_epd_loader/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    81547 2023-07-21 14:00:54.000000 solo_epd_loader-0.3.3/solo_epd_loader/__init__.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-21 14:04:30.466758 solo_epd_loader-0.3.3/solo_epd_loader/tests/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      108 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.3/solo_epd_loader/tests/__init__.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      345 2023-07-21 14:04:30.000000 solo_epd_loader-0.3.3/solo_epd_loader/version.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-21 14:04:30.466758 solo_epd_loader-0.3.3/solo_epd_loader.egg-info/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16842 2023-07-21 14:04:30.000000 solo_epd_loader-0.3.3/solo_epd_loader.egg-info/PKG-INFO
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      638 2023-07-21 14:04:30.000000 solo_epd_loader-0.3.3/solo_epd_loader.egg-info/SOURCES.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2023-07-21 14:04:30.000000 solo_epd_loader-0.3.3/solo_epd_loader.egg-info/dependency_links.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2022-01-12 15:20:36.000000 solo_epd_loader-0.3.3/solo_epd_loader.egg-info/not-zip-safe
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      194 2023-07-21 14:04:30.000000 solo_epd_loader-0.3.3/solo_epd_loader.egg-info/requires.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       16 2023-07-21 14:04:30.000000 solo_epd_loader-0.3.3/solo_epd_loader.egg-info/top_level.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1308 2022-06-28 13:22:42.000000 solo_epd_loader-0.3.3/tox.ini
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-24 13:34:24.894011 solo_epd_loader-0.3.4/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.3.4/LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      457 2022-03-01 17:04:02.000000 solo_epd_loader-0.3.4/MANIFEST.in
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16742 2023-07-24 13:34:24.898011 solo_epd_loader-0.3.4/PKG-INFO
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    15894 2023-07-20 13:53:21.000000 solo_epd_loader-0.3.4/README.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3370 2022-03-30 15:49:33.000000 solo_epd_loader-0.3.4/code_of_conduct.md
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-24 13:34:24.882011 solo_epd_loader-0.3.4/docs/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      634 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.4/docs/Makefile
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2312 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.4/docs/conf.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      379 2022-01-11 15:35:29.000000 solo_epd_loader-0.3.4/docs/index.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      760 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.4/docs/make.bat
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-24 13:34:24.886011 solo_epd_loader-0.3.4/examples/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-01-18 13:16:32.000000 solo_epd_loader-0.3.4/examples/gh2021_fig_2.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    72237 2021-05-19 13:25:57.000000 solo_epd_loader-0.3.4/examples/ws2021_fig_2d.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-28 12:32:34.000000 solo_epd_loader-0.3.4/gh2021_fig_2.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-25 16:10:07.000000 solo_epd_loader-0.3.4/gh2021_fig_2a.png
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-24 13:34:24.886011 solo_epd_loader-0.3.4/licenses/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.3.4/licenses/LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1308 2023-07-05 12:35:18.000000 solo_epd_loader-0.3.4/licenses/SUNPY_LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1659 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.4/licenses/TEMPLATE_LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      134 2022-03-01 17:04:02.000000 solo_epd_loader-0.3.4/pyproject.toml
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       89 2023-07-24 13:24:35.000000 solo_epd_loader-0.3.4/requirements.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2209 2023-07-24 13:34:24.898011 solo_epd_loader-0.3.4/setup.cfg
+-rwxrwxr-x   0 gieseler  (1000) gieseler  (1000)      666 2022-03-01 17:04:02.000000 solo_epd_loader-0.3.4/setup.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-24 13:34:24.890011 solo_epd_loader-0.3.4/solo_epd_loader/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    83025 2023-07-24 12:55:49.000000 solo_epd_loader-0.3.4/solo_epd_loader/__init__.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-24 13:34:24.874011 solo_epd_loader-0.3.4/solo_epd_loader/data/
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-24 13:34:24.874011 solo_epd_loader-0.3.4/solo_epd_loader/data/test/
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-24 13:34:24.874011 solo_epd_loader-0.3.4/solo_epd_loader/data/test/l2/
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-24 13:34:24.874011 solo_epd_loader-0.3.4/solo_epd_loader/data/test/l2/epd/
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-24 13:34:24.894011 solo_epd_loader-0.3.4/solo_epd_loader/data/test/l2/epd/ept/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   104579 2022-06-20 13:33:16.000000 solo_epd_loader-0.3.4/solo_epd_loader/data/test/l2/epd/ept/solo_L2_epd-ept-asun-rates_20200603_V02.cdf
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   107761 2022-06-20 13:33:23.000000 solo_epd_loader-0.3.4/solo_epd_loader/data/test/l2/epd/ept/solo_L2_epd-ept-north-rates_20200603_V02.cdf
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   104907 2022-06-20 13:33:32.000000 solo_epd_loader-0.3.4/solo_epd_loader/data/test/l2/epd/ept/solo_L2_epd-ept-south-rates_20200603_V02.cdf
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   103697 2022-06-20 13:33:39.000000 solo_epd_loader-0.3.4/solo_epd_loader/data/test/l2/epd/ept/solo_L2_epd-ept-sun-rates_20200603_V02.cdf
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-24 13:34:24.894011 solo_epd_loader-0.3.4/solo_epd_loader/tests/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      108 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.4/solo_epd_loader/tests/__init__.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     9850 2023-07-24 13:16:47.000000 solo_epd_loader-0.3.4/solo_epd_loader/tests/tests.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      345 2023-07-24 13:34:24.000000 solo_epd_loader-0.3.4/solo_epd_loader/version.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-24 13:34:24.890011 solo_epd_loader-0.3.4/solo_epd_loader.egg-info/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16742 2023-07-24 13:34:24.000000 solo_epd_loader-0.3.4/solo_epd_loader.egg-info/PKG-INFO
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1011 2023-07-24 13:34:24.000000 solo_epd_loader-0.3.4/solo_epd_loader.egg-info/SOURCES.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2023-07-24 13:34:24.000000 solo_epd_loader-0.3.4/solo_epd_loader.egg-info/dependency_links.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2022-01-12 15:20:36.000000 solo_epd_loader-0.3.4/solo_epd_loader.egg-info/not-zip-safe
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      175 2023-07-24 13:34:24.000000 solo_epd_loader-0.3.4/solo_epd_loader.egg-info/requires.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       16 2023-07-24 13:34:24.000000 solo_epd_loader-0.3.4/solo_epd_loader.egg-info/top_level.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1308 2022-06-28 13:22:42.000000 solo_epd_loader-0.3.4/tox.ini
```

### Comparing `solo_epd_loader-0.3.3/LICENSE.rst` & `solo_epd_loader-0.3.4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.3/PKG-INFO` & `solo_epd_loader-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: solo_epd_loader
-Version: 0.3.3
+Version: 0.3.4
 Summary: Data loader for Solar Orbiter/EPD energetic charged particle sensors EPT, HET, and STEP.
 Home-page: https://github.com/jgieseler/solo-epd-loader
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Provides-Extra: all
 Provides-Extra: test
 Provides-Extra: docs
 License-File: licenses/LICENSE.rst
 
 solo-epd-loader
 ===============
```

### Comparing `solo_epd_loader-0.3.3/README.rst` & `solo_epd_loader-0.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.3/code_of_conduct.md` & `solo_epd_loader-0.3.4/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.3/docs/Makefile` & `solo_epd_loader-0.3.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.3/docs/conf.py` & `solo_epd_loader-0.3.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.3/docs/make.bat` & `solo_epd_loader-0.3.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.3/examples/gh2021_fig_2.png` & `solo_epd_loader-0.3.4/examples/gh2021_fig_2.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.3/examples/ws2021_fig_2d.png` & `solo_epd_loader-0.3.4/examples/ws2021_fig_2d.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.3/gh2021_fig_2.png` & `solo_epd_loader-0.3.4/gh2021_fig_2.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.3/gh2021_fig_2a.png` & `solo_epd_loader-0.3.4/gh2021_fig_2a.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.3/licenses/LICENSE.rst` & `solo_epd_loader-0.3.4/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.3/licenses/SUNPY_LICENSE.rst` & `solo_epd_loader-0.3.4/licenses/SUNPY_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.3/licenses/TEMPLATE_LICENSE.rst` & `solo_epd_loader-0.3.4/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.3/setup.cfg` & `solo_epd_loader-0.3.4/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -9,40 +9,35 @@
 long_description = file: README.rst
 classifiers = 
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: BSD License
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: Scientific/Engineering :: Physics
 
 [options]
 zip_safe = False
 packages = find:
 include_package_data = True
-python_requires = >=3.6
+python_requires = >=3.8
 setup_requires = setuptools_scm
 install_requires = 
 	astropy
-	bs4
 	cdflib
-	datetime
 	drms
 	h5netcdf
 	lxml
 	matplotlib
 	numpy
 	pandas
 	requests
-	seppy
 	sunpy>=4.1.0
 	tqdm
 	zeep
 
 [options.extras_require]
 all = 
 test =
```

### Comparing `solo_epd_loader-0.3.3/setup.py` & `solo_epd_loader-0.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.3/solo_epd_loader/__init__.py` & `solo_epd_loader-0.3.4/solo_epd_loader/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -513,22 +513,20 @@
         given, Exception is raised.
 
     Examples
     --------
     Load EPD/HET sun viewing direction low-latency data for Aug 20 to Aug 22,
     2020 from user-defined directory, downloading missing files from SOAR:
 
-    >>> df_protons, df_electrons, energies = epd_load('het', 'll', 20200820,
-    ...     20200822, 'sun', None, True)
+    > df_protons, df_electrons, energies = epd_load(sensor='het', level='ll', startdate=20200820, enddate=20200822, viewing='sun', path=None, autodownload=True)
 
     Load EPD/STEP level 2 data for Aug 20 to Aug 22, 2020 from user-defined
     directory, downloading missing files from SOAR:
 
-    >>> df, energies = epd_load(sensor='step', level='l2', startdate=20200820,
-    ... enddate=20200822, autodownload=True)
+    > df, energies = epd_load(sensor='step', level='l2', startdate=20200820, enddate=20200822, autodownload=True)
     """
 
     # refuse string as date input:
     for d in [startdate, enddate]:
         if isinstance(d, str):
             raise SystemExit("startdate & enddate must be datetime objects or YYYYMMDD integer!")
 
@@ -916,14 +914,18 @@
         # check for duplicate files with different version numbers and remove them
         filelist = _check_duplicates(filelist, verbose=True)
 
         if len(filelist) == 0:
             warnings.warn('WARNING: No corresponding data files found! Try different settings, path or autodownload.')
             datadf = []
             energies_dict = []
+        elif level == 'll':
+            warnings.warn('WARNING: low-latency (ll) data not supported for STEP at the moment.')
+            datadf = []
+            energies_dict = []
         elif product == 'rates':
             if old_loading:
                 all_cdf = []
                 for file in filelist:
                     all_cdf.append(cdflib.CDF(file))
 
                 if level == 'l2':
@@ -1027,15 +1029,16 @@
         # if not only_averages:
         for i in range(1, 16):
             Electron_Flux_Mult['Electron_'+str(i).rjust(2, '0')+'_Flux_Mult'] = cdf['Electron_'+str(i).rjust(2, '0')+'_Flux_Mult']
         # df_Electron_Flux_Mult = pd.DataFrame(Electron_Flux_Mult)  # get dataframe from dict - not needed atm.
 
         meta['Electron_Flux_Mult'] = Electron_Flux_Mult
 
-    meta['df_rtn_desc'] = cdf.varattsget('RTN')['CATDESC']
+    if 'RTN' in cdf.cdf_info().zVariables:
+        meta['df_rtn_desc'] = cdf.varattsget('RTN')['CATDESC']
 
     del cdf
 
     df = pd.DataFrame()
     df_rtn = pd.DataFrame()
     df_hci = pd.DataFrame()
     for f in files:
@@ -1491,16 +1494,16 @@
         - Lowest EPT channels not supported because of overlapping energies.
 
     Examples
     --------
     Load EPT sun viewing direction level 2 data for Aug 20 to Aug 21, 2020, and
     combine electron channels 9 to 12 (i.e., 10th to 13th).
 
-    >>> df_p, df_e, meta = epd_load('ept', 20200820, 20200821, 'l2', 'sun')
-    >>> df_new, chan_new = combine_channels(df_p, meta, [9, 12], 'ept')
+    > df_p, df_e, meta = epd_load('ept', 20200820, 20200821, 'l2', 'sun')
+    > df_new, chan_new = combine_channels(df_p, meta, [9, 12], 'ept')
     """
     if sensor.lower() == 'step':
         raise Exception('STEP data not supported yet!')
         return pd.DataFrame(), ''
     # if species.lower() in ['e', 'electrons']:
     if 'Electron_Flux' in df.keys():
         en_str = energies['Electron_Bins_Text']
@@ -1553,18 +1556,47 @@
         en_channel_string = en_str[en_channel][0]
     return flux_out, en_channel_string
 
 
 calc_av_en_flux = copy.copy(combine_channels)  # define old name of the function for compatibility
 
 
-# import here to avoid circular import with seppy
-def resample_df(df, resample, pos_timestamp='center', origin='start'):
-    from seppy.tools import resample_df
-    return resample_df(df=df, resample=resample, pos_timestamp=pos_timestamp, origin=origin)
+def resample_df(df, resample, pos_timestamp="center", origin="start"):
+    """
+    Resamples a Pandas Dataframe or Series to a new frequency.
+
+    Parameters:
+    -----------
+    df : pd.DataFrame or pd.Series
+            The dataframe or series to resample
+    resample : str
+            pandas-compatible time string, e.g., '1min', '2H' or '25s'
+    pos_timestamp : str, default 'center'
+            Controls if the timestamp is at the center of the time bin, or at
+            the start of it
+    origin : str, default 'start'
+            Controls if the origin of resampling is at the start of the day
+            (midnight) or at the first entry of the input dataframe/series
+
+    Returns:
+    ----------
+    df : pd.DataFrame or Series, depending on the input
+    """
+    try:
+        df = df.resample(resample, origin=origin, label="left").mean()
+        if pos_timestamp == 'start':
+            df.index = df.index
+        else:
+            df.index = df.index + pd.tseries.frequencies.to_offset(pd.Timedelta(resample)/2)
+        # if pos_timestamp == 'stop' or pos_timestamp == 'end':
+        #     df.index = df.index + pd.tseries.frequencies.to_offset(pd.Timedelta(resample))
+    except ValueError:
+        raise ValueError(f"Your 'resample' option of [{resample}] doesn't seem to be a proper Pandas frequency!")
+
+    return df
 
 
 """
 Modification of sunpy's read_cdf function to allow skipping of reading variables from a cdf file.
 This function is copied from sunpy under the terms of the BSD 2-Clause licence. See licenses/SUNPY_LICENSE.rst
 """
 
@@ -1671,15 +1703,16 @@
                 warn_user(f'The variable "{var_key}" has been skipped because it has more than 3 dimensions, which is unsupported.')
             elif data.ndim == 3:
                 # Multiple columns, give each column a unique label.
                 # Numbering hard-corded to SolO/EPD/STEP (old) data!
                 if var_key.startswith('Sector_'):
                     for j in range(data.T.shape[0]):
                         for i, col in enumerate(data.T[j, :, :]):
-                            var_key_mod = var_key.removeprefix('Sector_')
+                            # var_key_mod = var_key.removeprefix('Sector_')
+                            var_key_mod = var_key[len('Sector_'):]  # alternative to .removeprefix() that is supported in python <3.9
                             var_key_mod = var_key_mod.replace('_', '_'+str(j+1).rjust(2, '0')+'_')  # j+1: numbering hard-corded to SolO/EPD/STEP (old) data!
                             df[var_key_mod + f'_{i}'] = col
                             units[var_key_mod + f'_{i}'] = unit
                 elif var_key == 'RTN_Sectors' or var_key == 'RTN_Pixels':
                     for j in range(data.T.shape[1]):
                         for i, col in enumerate(data.T[:, j, :]):
                             var_key_mod = var_key+'_'+str(j+1).rjust(2, '0')  # j+1: numbering hard-corded to SolO/EPD/STEP (old) data!
```

### Comparing `solo_epd_loader-0.3.3/solo_epd_loader.egg-info/PKG-INFO` & `solo_epd_loader-0.3.4/solo_epd_loader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: solo-epd-loader
-Version: 0.3.3
+Version: 0.3.4
 Summary: Data loader for Solar Orbiter/EPD energetic charged particle sensors EPT, HET, and STEP.
 Home-page: https://github.com/jgieseler/solo-epd-loader
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Provides-Extra: all
 Provides-Extra: test
 Provides-Extra: docs
 License-File: licenses/LICENSE.rst
 
 solo-epd-loader
 ===============
```

### Comparing `solo_epd_loader-0.3.3/tox.ini` & `solo_epd_loader-0.3.4/tox.ini`

 * *Files identical despite different names*

