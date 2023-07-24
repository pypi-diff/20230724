# Comparing `tmp/pyspm-0.3.2.tar.gz` & `tmp/pyspm-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspm-0.3.2.tar", max compression
+gzip compressed data, was "pyspm-0.3.3.tar", max compression
```

## Comparing `pyspm-0.3.2.tar` & `pyspm-0.3.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0    11547 2023-03-05 18:27:01.179302 pyspm-0.3.2/LICENSE
--rw-r--r--   0        0        0      966 2023-07-06 13:25:08.071581 pyspm-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      542 2023-07-06 12:37:08.199861 pyspm-0.3.2/pySPM/__init__.py
--rw-r--r--   0        0        0     1766 2023-07-06 12:37:08.200862 pyspm-0.3.2/pySPM/__main__.py
--rw-r--r--   0        0        0    10876 2023-07-06 12:37:08.201864 pyspm-0.3.2/pySPM/align.py
--rw-r--r--   0        0        0    34297 2023-07-06 12:37:08.188862 pyspm-0.3.2/pySPM/Block.py
--rw-r--r--   0        0        0     8097 2023-07-06 13:11:30.075518 pyspm-0.3.2/pySPM/Bruker.py
--rw-r--r--   0        0        0    10014 2023-07-06 12:37:08.202862 pyspm-0.3.2/pySPM/collection.py
--rw-r--r--   0        0        0   376832 2023-03-05 18:27:01.395335 pyspm-0.3.2/pySPM/data/elements.db
--rw-r--r--   0        0        0    43286 2023-07-06 12:37:08.190863 pyspm-0.3.2/pySPM/ITA.py
--rw-r--r--   0        0        0     6920 2023-07-06 12:37:08.192862 pyspm-0.3.2/pySPM/ITAslicer.py
--rw-r--r--   0        0        0     4051 2023-07-06 12:37:08.191862 pyspm-0.3.2/pySPM/ITAX.py
--rw-r--r--   0        0        0    61097 2023-07-06 12:37:08.193862 pyspm-0.3.2/pySPM/ITM.py
--rw-r--r--   0        0        0      746 2023-07-06 12:37:08.194863 pyspm-0.3.2/pySPM/ITS.py
--rw-r--r--   0        0        0     1181 2023-07-06 12:37:08.203863 pyspm-0.3.2/pySPM/mplwidget.py
--rw-r--r--   0        0        0     8664 2023-07-06 12:37:08.204862 pyspm-0.3.2/pySPM/nanoscan.py
--rw-r--r--   0        0        0     8314 2023-07-06 12:37:08.195862 pyspm-0.3.2/pySPM/PCA.py
--rw-r--r--   0        0        0     5200 2023-07-06 12:37:08.205863 pyspm-0.3.2/pySPM/slicer.py
--rw-r--r--   0        0        0    73601 2023-07-06 12:37:08.197862 pyspm-0.3.2/pySPM/SPM.py
--rw-r--r--   0        0        0     3020 2023-07-06 12:37:08.198862 pyspm-0.3.2/pySPM/SXM.py
--rw-r--r--   0        0        0     7907 2023-07-06 12:37:08.199861 pyspm-0.3.2/pySPM/ToF.py
--rw-r--r--   0        0        0        0 2023-03-05 18:27:01.410967 pyspm-0.3.2/pySPM/tools/__init__.py
--rw-r--r--   0        0        0     2012 2023-07-06 12:37:08.206862 pyspm-0.3.2/pySPM/tools/emission_current_plotter.py
--rw-r--r--   0        0        0     3116 2023-07-06 12:37:08.208863 pyspm-0.3.2/pySPM/tools/fpanel.py
--rw-r--r--   0        0        0     1096 2023-07-06 12:37:08.209865 pyspm-0.3.2/pySPM/tools/mplwidget.py
--rw-r--r--   0        0        0    12419 2023-07-06 12:37:08.210862 pyspm-0.3.2/pySPM/tools/spectra.py
--rw-r--r--   0        0        0     5713 2023-07-06 12:37:08.211862 pyspm-0.3.2/pySPM/tools/spectraviewer.py
--rw-r--r--   0        0        0     6920 2023-07-06 12:37:08.212863 pyspm-0.3.2/pySPM/tools/spectraviewer.ui
--rw-r--r--   0        0        0     2623 2023-07-06 12:37:08.214874 pyspm-0.3.2/pySPM/tools/stability.py
--rw-r--r--   0        0        0     2014 2023-07-06 12:37:08.215866 pyspm-0.3.2/pySPM/tools/timer_display.py
--rw-r--r--   0        0        0     1882 2023-07-06 12:37:08.216867 pyspm-0.3.2/pySPM/tools/timer_display.ui
--rw-r--r--   0        0        0     1847 2023-07-06 12:37:08.217863 pyspm-0.3.2/pySPM/tools/tof_timer.py
--rw-r--r--   0        0        0     1218 2023-03-05 18:27:01.410967 pyspm-0.3.2/pySPM/tools/values_display.py
--rw-r--r--   0        0        0     8319 2023-07-06 12:37:08.218863 pyspm-0.3.2/pySPM/tools/win32_helper.py
--rw-r--r--   0        0        0     7572 2023-07-06 12:37:08.219863 pyspm-0.3.2/pySPM/utils/__init__.py
--rw-r--r--   0        0        0      270 2023-07-06 12:37:08.219863 pyspm-0.3.2/pySPM/utils/colors.py
--rw-r--r--   0        0        0      385 2023-07-06 12:37:08.220863 pyspm-0.3.2/pySPM/utils/constants.py
--rw-r--r--   0        0        0    14280 2023-07-06 12:37:08.221863 pyspm-0.3.2/pySPM/utils/elts.py
--rw-r--r--   0        0        0    11678 2023-07-06 12:37:08.222862 pyspm-0.3.2/pySPM/utils/fit.py
--rw-r--r--   0        0        0     2924 2023-07-06 12:37:08.223861 pyspm-0.3.2/pySPM/utils/geometry.py
--rw-r--r--   0        0        0     1619 2023-07-06 12:37:08.223861 pyspm-0.3.2/pySPM/utils/haar.py
--rw-r--r--   0        0        0    10455 2023-07-06 12:37:08.224862 pyspm-0.3.2/pySPM/utils/math.py
--rw-r--r--   0        0        0     5317 2023-07-06 12:37:08.225862 pyspm-0.3.2/pySPM/utils/misc.py
--rw-r--r--   0        0        0    15478 2023-07-06 12:37:08.226863 pyspm-0.3.2/pySPM/utils/plot.py
--rw-r--r--   0        0        0      909 2023-07-06 12:37:08.227863 pyspm-0.3.2/pySPM/utils/progressbar.py
--rw-r--r--   0        0        0     7138 2023-07-06 12:37:08.228862 pyspm-0.3.2/pySPM/utils/restoration.py
--rw-r--r--   0        0        0     6459 2023-07-06 12:37:08.229864 pyspm-0.3.2/pySPM/utils/save.py
--rw-r--r--   0        0        0    16833 2023-07-06 12:37:08.230863 pyspm-0.3.2/pySPM/utils/spectra.py
--rw-r--r--   0        0        0     7071 2023-07-06 12:37:08.231862 pyspm-0.3.2/pySPM/utils/units.py
--rw-r--r--   0        0        0     5478 2023-07-06 12:37:08.181863 pyspm-0.3.2/README.md
--rw-r--r--   0        0        0     6441 1970-01-01 00:00:00.000000 pyspm-0.3.2/setup.py
--rw-r--r--   0        0        0     6649 1970-01-01 00:00:00.000000 pyspm-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    11547 2023-03-05 18:27:01.179302 pyspm-0.3.3/LICENSE
+-rw-r--r--   0        0        0      966 2023-07-24 18:07:25.592157 pyspm-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      542 2023-07-22 15:32:02.734470 pyspm-0.3.3/pySPM/__init__.py
+-rw-r--r--   0        0        0     1766 2023-07-06 12:37:08.200862 pyspm-0.3.3/pySPM/__main__.py
+-rw-r--r--   0        0        0    10876 2023-07-06 12:37:08.201864 pyspm-0.3.3/pySPM/align.py
+-rw-r--r--   0        0        0    34297 2023-07-06 12:37:08.188862 pyspm-0.3.3/pySPM/Block.py
+-rw-r--r--   0        0        0     8097 2023-07-06 13:11:30.075518 pyspm-0.3.3/pySPM/Bruker.py
+-rw-r--r--   0        0        0    10014 2023-07-06 12:37:08.202862 pyspm-0.3.3/pySPM/collection.py
+-rw-r--r--   0        0        0   376832 2023-03-05 18:27:01.395335 pyspm-0.3.3/pySPM/data/elements.db
+-rw-r--r--   0        0        0    43286 2023-07-06 12:37:08.190863 pyspm-0.3.3/pySPM/ITA.py
+-rw-r--r--   0        0        0     6920 2023-07-06 12:37:08.192862 pyspm-0.3.3/pySPM/ITAslicer.py
+-rw-r--r--   0        0        0     4051 2023-07-06 12:37:08.191862 pyspm-0.3.3/pySPM/ITAX.py
+-rw-r--r--   0        0        0    61097 2023-07-06 12:37:08.193862 pyspm-0.3.3/pySPM/ITM.py
+-rw-r--r--   0        0        0      746 2023-07-06 12:37:08.194863 pyspm-0.3.3/pySPM/ITS.py
+-rw-r--r--   0        0        0     1181 2023-07-06 12:37:08.203863 pyspm-0.3.3/pySPM/mplwidget.py
+-rw-r--r--   0        0        0     8664 2023-07-06 12:37:08.204862 pyspm-0.3.3/pySPM/nanoscan.py
+-rw-r--r--   0        0        0     8314 2023-07-06 12:37:08.195862 pyspm-0.3.3/pySPM/PCA.py
+-rw-r--r--   0        0        0     5200 2023-07-06 12:37:08.205863 pyspm-0.3.3/pySPM/slicer.py
+-rw-r--r--   0        0        0    73601 2023-07-06 12:37:08.197862 pyspm-0.3.3/pySPM/SPM.py
+-rw-r--r--   0        0        0     3185 2023-07-24 18:04:50.416978 pyspm-0.3.3/pySPM/SXM.py
+-rw-r--r--   0        0        0     7907 2023-07-06 12:37:08.199861 pyspm-0.3.3/pySPM/ToF.py
+-rw-r--r--   0        0        0        0 2023-03-05 18:27:01.410967 pyspm-0.3.3/pySPM/tools/__init__.py
+-rw-r--r--   0        0        0     2012 2023-07-06 12:37:08.206862 pyspm-0.3.3/pySPM/tools/emission_current_plotter.py
+-rw-r--r--   0        0        0     3116 2023-07-06 12:37:08.208863 pyspm-0.3.3/pySPM/tools/fpanel.py
+-rw-r--r--   0        0        0     1096 2023-07-06 12:37:08.209865 pyspm-0.3.3/pySPM/tools/mplwidget.py
+-rw-r--r--   0        0        0    12419 2023-07-06 12:37:08.210862 pyspm-0.3.3/pySPM/tools/spectra.py
+-rw-r--r--   0        0        0     5713 2023-07-06 12:37:08.211862 pyspm-0.3.3/pySPM/tools/spectraviewer.py
+-rw-r--r--   0        0        0     6920 2023-07-06 12:37:08.212863 pyspm-0.3.3/pySPM/tools/spectraviewer.ui
+-rw-r--r--   0        0        0     2623 2023-07-06 12:37:08.214874 pyspm-0.3.3/pySPM/tools/stability.py
+-rw-r--r--   0        0        0     2014 2023-07-06 12:37:08.215866 pyspm-0.3.3/pySPM/tools/timer_display.py
+-rw-r--r--   0        0        0     1882 2023-07-06 12:37:08.216867 pyspm-0.3.3/pySPM/tools/timer_display.ui
+-rw-r--r--   0        0        0     1847 2023-07-06 12:37:08.217863 pyspm-0.3.3/pySPM/tools/tof_timer.py
+-rw-r--r--   0        0        0     1218 2023-03-05 18:27:01.410967 pyspm-0.3.3/pySPM/tools/values_display.py
+-rw-r--r--   0        0        0     8319 2023-07-06 12:37:08.218863 pyspm-0.3.3/pySPM/tools/win32_helper.py
+-rw-r--r--   0        0        0     7572 2023-07-06 12:37:08.219863 pyspm-0.3.3/pySPM/utils/__init__.py
+-rw-r--r--   0        0        0      270 2023-07-06 12:37:08.219863 pyspm-0.3.3/pySPM/utils/colors.py
+-rw-r--r--   0        0        0      385 2023-07-06 12:37:08.220863 pyspm-0.3.3/pySPM/utils/constants.py
+-rw-r--r--   0        0        0    14280 2023-07-06 12:37:08.221863 pyspm-0.3.3/pySPM/utils/elts.py
+-rw-r--r--   0        0        0    11678 2023-07-06 12:37:08.222862 pyspm-0.3.3/pySPM/utils/fit.py
+-rw-r--r--   0        0        0     2924 2023-07-06 12:37:08.223861 pyspm-0.3.3/pySPM/utils/geometry.py
+-rw-r--r--   0        0        0     1619 2023-07-06 12:37:08.223861 pyspm-0.3.3/pySPM/utils/haar.py
+-rw-r--r--   0        0        0    10455 2023-07-06 12:37:08.224862 pyspm-0.3.3/pySPM/utils/math.py
+-rw-r--r--   0        0        0     5317 2023-07-06 12:37:08.225862 pyspm-0.3.3/pySPM/utils/misc.py
+-rw-r--r--   0        0        0    15478 2023-07-06 12:37:08.226863 pyspm-0.3.3/pySPM/utils/plot.py
+-rw-r--r--   0        0        0      909 2023-07-06 12:37:08.227863 pyspm-0.3.3/pySPM/utils/progressbar.py
+-rw-r--r--   0        0        0     7138 2023-07-06 12:37:08.228862 pyspm-0.3.3/pySPM/utils/restoration.py
+-rw-r--r--   0        0        0     6459 2023-07-06 12:37:08.229864 pyspm-0.3.3/pySPM/utils/save.py
+-rw-r--r--   0        0        0    16833 2023-07-06 12:37:08.230863 pyspm-0.3.3/pySPM/utils/spectra.py
+-rw-r--r--   0        0        0     7071 2023-07-06 12:37:08.231862 pyspm-0.3.3/pySPM/utils/units.py
+-rw-r--r--   0        0        0     5478 2023-07-06 12:37:08.181863 pyspm-0.3.3/README.md
+-rw-r--r--   0        0        0     6441 1970-01-01 00:00:00.000000 pyspm-0.3.3/setup.py
+-rw-r--r--   0        0        0     6649 1970-01-01 00:00:00.000000 pyspm-0.3.3/PKG-INFO
```

### Comparing `pyspm-0.3.2/LICENSE` & `pyspm-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/pyproject.toml` & `pyspm-0.3.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyspm"
-version = "0.3.2"
+version = "0.3.3"
 description = "Library to handle SPM and ToF-SIMS data"
 authors = ["Olivier Scholder <o.scholder@gmail.com>"]
 maintainers = ["Dinesh Pinto <annual.fallout_0z@icloud.com>"]
 homepage = "https://github.com/scholi/pySPM"
 repository = "https://github.com/scholi/pySPM"
 license = "Apache-2.0"
 readme = "README.md"
```

### Comparing `pyspm-0.3.2/pySPM/__init__.py` & `pyspm-0.3.3/pySPM/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/pySPM/__main__.py` & `pyspm-0.3.3/pySPM/__main__.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/pySPM/align.py` & `pyspm-0.3.3/pySPM/align.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/pySPM/Block.py` & `pyspm-0.3.3/pySPM/Block.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/pySPM/Bruker.py` & `pyspm-0.3.3/pySPM/Bruker.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/pySPM/collection.py` & `pyspm-0.3.3/pySPM/collection.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/pySPM/data/elements.db` & `pyspm-0.3.3/pySPM/data/elements.db`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/pySPM/ITA.py` & `pyspm-0.3.3/pySPM/ITA.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/pySPM/ITAslicer.py` & `pyspm-0.3.3/pySPM/ITAslicer.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/pySPM/ITAX.py` & `pyspm-0.3.3/pySPM/ITAX.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/pySPM/ITM.py` & `pyspm-0.3.3/pySPM/ITM.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/pySPM/ITS.py` & `pyspm-0.3.3/pySPM/ITS.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/pySPM/mplwidget.py` & `pyspm-0.3.3/pySPM/mplwidget.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/pySPM/nanoscan.py` & `pyspm-0.3.3/pySPM/nanoscan.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/pySPM/PCA.py` & `pyspm-0.3.3/pySPM/PCA.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/pySPM/slicer.py` & `pyspm-0.3.3/pySPM/slicer.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/pySPM/SPM.py` & `pyspm-0.3.3/pySPM/SPM.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/pySPM/SXM.py` & `pyspm-0.3.3/pySPM/SXM.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,19 @@
         while l != b':SCANIT_END:':
             l = self.f.readline().rstrip()
             if l[:1] == b':':
                 key = l.split(b':')[1].decode('ascii')
                 self.header[key] = []
             else:
                 if l:  # remove empty lines
-                    self.header[key].append(l.decode('ascii').split())
+                    try:
+                        self.header[key].append(l.decode('ascii').split())
+                    except UnicodeDecodeError:
+                        self.header[key].append(l.decode('unicode_escape').split())
+
         while self.f.read(1) != b'\x1a':
             pass
         assert self.f.read(1) == b'\x04'
         assert self.header['SCANIT_TYPE'][0][0] in ['FLOAT', 'INT', 'UINT', 'DOUBLE']
         self.data_offset = self.f.tell()
         self.f.close()
         self.size = dict(pixels={
```

### Comparing `pyspm-0.3.2/pySPM/ToF.py` & `pyspm-0.3.3/pySPM/ToF.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/pySPM/tools/emission_current_plotter.py` & `pyspm-0.3.3/pySPM/tools/emission_current_plotter.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/pySPM/tools/fpanel.py` & `pyspm-0.3.3/pySPM/tools/fpanel.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/pySPM/tools/mplwidget.py` & `pyspm-0.3.3/pySPM/tools/mplwidget.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/pySPM/tools/spectra.py` & `pyspm-0.3.3/pySPM/tools/spectra.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/pySPM/tools/spectraviewer.py` & `pyspm-0.3.3/pySPM/tools/spectraviewer.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/pySPM/tools/spectraviewer.ui` & `pyspm-0.3.3/pySPM/tools/spectraviewer.ui`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/pySPM/tools/stability.py` & `pyspm-0.3.3/pySPM/tools/stability.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/pySPM/tools/timer_display.py` & `pyspm-0.3.3/pySPM/tools/timer_display.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/pySPM/tools/timer_display.ui` & `pyspm-0.3.3/pySPM/tools/timer_display.ui`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/pySPM/tools/tof_timer.py` & `pyspm-0.3.3/pySPM/tools/tof_timer.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/pySPM/tools/values_display.py` & `pyspm-0.3.3/pySPM/tools/values_display.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/pySPM/tools/win32_helper.py` & `pyspm-0.3.3/pySPM/tools/win32_helper.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/pySPM/utils/__init__.py` & `pyspm-0.3.3/pySPM/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/pySPM/utils/elts.py` & `pyspm-0.3.3/pySPM/utils/elts.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/pySPM/utils/fit.py` & `pyspm-0.3.3/pySPM/utils/fit.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/pySPM/utils/geometry.py` & `pyspm-0.3.3/pySPM/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/pySPM/utils/haar.py` & `pyspm-0.3.3/pySPM/utils/haar.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/pySPM/utils/math.py` & `pyspm-0.3.3/pySPM/utils/math.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/pySPM/utils/misc.py` & `pyspm-0.3.3/pySPM/utils/misc.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/pySPM/utils/plot.py` & `pyspm-0.3.3/pySPM/utils/plot.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/pySPM/utils/progressbar.py` & `pyspm-0.3.3/pySPM/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/pySPM/utils/restoration.py` & `pyspm-0.3.3/pySPM/utils/restoration.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/pySPM/utils/save.py` & `pyspm-0.3.3/pySPM/utils/save.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/pySPM/utils/spectra.py` & `pyspm-0.3.3/pySPM/utils/spectra.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/pySPM/utils/units.py` & `pyspm-0.3.3/pySPM/utils/units.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/README.md` & `pyspm-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pyspm-0.3.2/setup.py` & `pyspm-0.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'scikit-image>=0.20.0,<0.21.0',
  'scikit-learn>=1.2.2,<2.0.0',
  'seaborn>=0.12.2,<0.13.0',
  'tqdm>=4.65.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'pyspm',
-    'version': '0.3.2',
+    'version': '0.3.3',
     'description': 'Library to handle SPM and ToF-SIMS data',
     'long_description': '[![Downloads](https://pepy.tech/badge/pyspm)](https://pepy.tech/project/pyspm)\n[![PyPi version](https://img.shields.io/pypi/v/pySPM)](https://pypi.python.org/pypi/pySPM/)\n[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)\n[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.998575.svg)](https://doi.org/10.5281/zenodo.998575)\n\n# pySPM\n\npySPM is a Python library in order to read, handle and plot Scanning Probe Microscopy (SPM) images as well as ToF-SIMS\ndata.\n\nSupported SPM file formats:\n\n* Nanoscan .xml file format\n* Bruker\n* Iontof ToF-SIMS fileformats:\n    * ITA\n    * ITM\n    * ITS\n* Nanonis SXM file\n\n## Important\n\nThis library is offered as it is and is still in development. Please note that reading the raw data was done by reverse\nengineering and guessing and not with a manual as the file format is proprietary. It seems to work well with the data\nused by the developer of this library, but there is **NO GUARANTEE** that this library will work correctly with your own\nspecific data.\n\nIf you find bugs and issues, please report them to the developer: https://github.com/scholi/pySPM/issues\n\n## Installation\n\n### From PyPI\n\n```bash\npip install pySPM\n```\n### From GitHub\n\n#### With poetry\n\n```bash\npoetry add git+https://github.com/scholi/pySPM.git\n```\n\n#### With pip\n\n```bash\npip install git+https://github.com/scholi/pySPM.git\n```\n\n### Optional dependencies\n\n`PyQT5` for GUI controls.\n\n## Documentation\n\nThe documentation is still in its early stage\n[read the documentation](https://nbviewer.jupyter.org/github/scholi/pySPM/blob/master/doc/pySPM%20Documentation.ipynb)\n\nThere is also\na [short introduction to pySPM for ToF-SIMS data](https://nbviewer.jupyter.org/github/scholi/pySPM/blob/master/doc/Introduction%20to%20pySPM%20for%20ToF-SIMS%20data.ipynb)\n\n## Citing\n\nIf you use this library for your work, please think about citing it.\n[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.998575.svg)](https://doi.org/10.5281/zenodo.998575)\n\nOlivier Scholder. (2018, November 28). scholi/pySPM: pySPM v0.2.16 (Version v0.2.16).\nZenodo. http://doi.org/10.5281/zenodo.998575\n\n## News\n\n### ITA files are writable\n\nFrom now on you can, not only view the ita files, but you can also write them by supplying the parameter\n_readable=False_ to _pySPM.ITA_ or _pySPM.ITM_. For the moment this is still a non-user-friendly procedure, but you can\nedit each ITStr Block with the ```edit_block()``` function. Be careful, because if the new data has a different size\nthan the old one, a new block is created, but the old one is also kept. This means that your ITA file size will grow.\nYou can also add new channels and images with the more user-friendly function ```pySPM.ITA.add_new_images()```.\n:warning: It is highly advised to copy the ita file before making any change. You can use the following code to copy the\nita in a temporary ita before making any change.\n\n```python\nfrom shutil import copyfile\nimport pySPM\n\nfilename = "scanfile.ita"\ncopyfile(src=filename, dst="temp.ita")\nA = pySPM.ITA("temp.ita", readonly=False)\n```\n\n### New tools\n\nThe library comes with three scripts to make your life easier. Those scripts are located in your python folder in the\nScripts directory. You can also run them from the command line.\n\n#### stability\n\nAllows you to select a measurement folder and display the Emission Current and Suppressor voltage in function of the\ntime/scan number.\nThis allows you to verify the stability of your source during your measurements.\n![stability_screenshot](doc/images/Capture_stability.png)\n\nsee the [wiki](../../wiki/stability) for more info\n\n#### plotter\n\nAllows you to plot the parameter logged by your logfile. If SurfaceLab is running this script will detect which logfile\nis beeing saved and will display the values live (the plot is refreshed every 3s in order add the new data). You can\nalso provide as first argument the logfile path (or in windows you can drag&drop the logfile over the plotter app).\n![plotter_screenshot](doc/images/Capture_plotter.png)\n\nsee the [wiki](../../wiki/plotter) for more info\n\n#### timer\n\nIf you are using SurfaceLab, this app will display a small progressbar of your measurement and will calculate the\nremaining time in function of the elapsed time, the total number of scans and the elapsed number of scan.\n![timer_screenshot](doc/images/Capture_timer.png)\n\nsee the [wiki](../../wiki/timer) for more info\n\n#### spectra\n\nThis tool can display spectra, visualize rapidly peaks assignment and perform fast mass calibration.\nYou can give an ITA filename as argument or if none a GUI filedialog will ask you for one. You will then see your\nspectrum.\nYou can navigate with the scroll of the mouse to zoom in & out. You can use the keyboard <kbd>+</kbd> and <kbd>-</kbd>\nto shift your spectra by ±1 Dalton. You can use left-mouse-button and drag to shift your spectra. You can perform very\nquick mass calibration by Right-Mouse-Click on one measurement peak (hold the mouse) the move to the element mark you\nwant to assign your peak and release the mouse. The mass calibration values should then be updated on the left table and\nthe mass calibration performed live so that you can see immediately the changes.\n![spectra_screenshot](doc/images/Capture_spectra.png)\n\nsee the [wiki](../../wiki/spectra) for more info\n',
     'author': 'Olivier Scholder',
     'author_email': 'o.scholder@gmail.com',
     'maintainer': 'Dinesh Pinto',
     'maintainer_email': 'annual.fallout_0z@icloud.com',
     'url': 'https://github.com/scholi/pySPM',
```

### Comparing `pyspm-0.3.2/PKG-INFO` & `pyspm-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspm
-Version: 0.3.2
+Version: 0.3.3
 Summary: Library to handle SPM and ToF-SIMS data
 Home-page: https://github.com/scholi/pySPM
 License: Apache-2.0
 Keywords: ToF,SIMS,ION-ToF,SPM,SFM,SXM,AFM,KPFM,PCA,ITA,imaging,ITM,Bruker,Nanonis
 Author: Olivier Scholder
 Author-email: o.scholder@gmail.com
 Maintainer: Dinesh Pinto
```

