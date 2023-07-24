# Comparing `tmp/f311-18.3.1.0.tar.gz` & `tmp/f311-23.7.21.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/f311-18.3.1.0.tar", last modified: Tue Mar  6 17:19:54 2018, max compression
+gzip compressed data, was "f311-23.7.21.0.tar", last modified: Mon Jul 24 12:53:25 2023, max compression
```

## Comparing `f311-18.3.1.0.tar` & `f311-23.7.21.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2018-03-06 17:19:54.000000 f311-18.3.1.0/
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2018-03-06 17:19:54.000000 f311-18.3.1.0/f311/
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2018-03-06 17:19:54.000000 f311-18.3.1.0/f311/explorer/
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2018-03-06 17:19:54.000000 f311-18.3.1.0/f311/explorer/gui/
--rw-r--r--   0 j         (1000) j         (1000)     1367 2017-12-21 21:45:50.000000 f311-18.3.1.0/f311/explorer/gui/a_XText.py
--rw-r--r--   0 j         (1000) j         (1000)    15613 2017-12-21 21:45:50.000000 f311-18.3.1.0/f311/explorer/gui/a_XFileMainWindow.py
--rw-r--r--   0 j         (1000) j         (1000)      197 2017-12-21 21:45:50.000000 f311-18.3.1.0/f311/explorer/gui/__init__.py
--rw-r--r--   0 j         (1000) j         (1000)     3426 2017-12-21 21:45:50.000000 f311-18.3.1.0/f311/explorer/gui/a_XSelectDataFile.py
--rw-r--r--   0 j         (1000) j         (1000)    26066 2017-12-21 21:45:50.000000 f311-18.3.1.0/f311/explorer/gui/a_XExplorer.py
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2018-03-06 17:19:54.000000 f311-18.3.1.0/f311/explorer/vis/
--rw-r--r--   0 j         (1000) j         (1000)      211 2017-12-21 21:45:50.000000 f311-18.3.1.0/f311/explorer/vis/__init__.py
--rw-r--r--   0 j         (1000) j         (1000)      228 2017-12-21 21:45:50.000000 f311-18.3.1.0/f311/explorer/vis/visprint.py
--rw-r--r--   0 j         (1000) j         (1000)     9903 2017-12-21 21:45:50.000000 f311-18.3.1.0/f311/explorer/vis/plotsp.py
--rw-r--r--   0 j         (1000) j         (1000)     1459 2017-12-21 21:45:50.000000 f311-18.3.1.0/f311/explorer/vis/basic.py
--rw-r--r--   0 j         (1000) j         (1000)      552 2017-12-21 21:45:50.000000 f311-18.3.1.0/f311/explorer/vis/visspectrum.py
--rw-r--r--   0 j         (1000) j         (1000)      595 2017-12-21 21:45:50.000000 f311-18.3.1.0/f311/explorer/__init__.py
--rw-r--r--   0 j         (1000) j         (1000)      712 2017-12-21 21:45:50.000000 f311-18.3.1.0/f311/explorer/util.py
--rw-r--r--   0 j         (1000) j         (1000)   561633 2017-12-21 21:45:50.000000 f311-18.3.1.0/f311/hapi.py
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2018-03-06 17:19:54.000000 f311-18.3.1.0/f311/scripts/
--rwxr-xr-x   0 j         (1000) j         (1000)     5010 2017-12-21 21:45:50.000000 f311-18.3.1.0/f311/scripts/plot-spectra.py
--rwxr-xr-x   0 j         (1000) j         (1000)     3461 2017-12-21 21:45:50.000000 f311-18.3.1.0/f311/scripts/programs.py
--rwxr-xr-x   0 j         (1000) j         (1000)     1362 2017-12-21 21:45:50.000000 f311-18.3.1.0/f311/scripts/cut-spectrum.py
--rwxr-xr-x   0 j         (1000) j         (1000)      645 2017-12-21 21:45:50.000000 f311-18.3.1.0/f311/scripts/explorer.py
--rw-r--r--   0 j         (1000) j         (1000)      144 2017-12-21 21:45:50.000000 f311-18.3.1.0/f311/__init__.py
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2018-03-06 17:19:54.000000 f311-18.3.1.0/f311/filetypes/
--rw-r--r--   0 j         (1000) j         (1000)    13438 2017-12-21 21:45:50.000000 f311-18.3.1.0/f311/filetypes/spectrum.py
--rw-r--r--   0 j         (1000) j         (1000)     3677 2017-12-21 21:45:50.000000 f311-18.3.1.0/f311/filetypes/datafile.py
--rw-r--r--   0 j         (1000) j         (1000)     1460 2017-12-21 21:45:50.000000 f311-18.3.1.0/f311/filetypes/filefits.py
--rw-r--r--   0 j         (1000) j         (1000)      233 2017-12-21 21:45:50.000000 f311-18.3.1.0/f311/filetypes/__init__.py
--rw-r--r--   0 j         (1000) j         (1000)     2610 2018-03-01 22:06:12.000000 f311-18.3.1.0/f311/filetypes/filespectrum.py
--rw-r--r--   0 j         (1000) j         (1000)     3034 2017-12-21 21:45:50.000000 f311-18.3.1.0/f311/filetypes/filepy.py
--rw-r--r--   0 j         (1000) j         (1000)     6276 2018-03-01 16:22:28.000000 f311-18.3.1.0/f311/filetypes/filesqlitedb.py
--rw-r--r--   0 j         (1000) j         (1000)     8609 2018-03-01 16:52:11.000000 f311-18.3.1.0/f311/collaboration.py
--rw-r--r--   0 j         (1000) j         (1000)     2097 2017-12-21 21:45:50.000000 f311-18.3.1.0/f311/pathfinder.py
--rw-r--r--   0 j         (1000) j         (1000)     8708 2017-12-21 21:45:50.000000 f311-18.3.1.0/f311/util.py
--rw-r--r--   0 j         (1000) j         (1000)       40 2017-12-21 21:45:50.000000 f311-18.3.1.0/MANIFEST.in
--rw-r--r--   0 j         (1000) j         (1000)      463 2018-03-06 17:19:54.000000 f311-18.3.1.0/PKG-INFO
--rw-r--r--   0 j         (1000) j         (1000)      152 2017-12-21 21:45:50.000000 f311-18.3.1.0/README.md
--rw-r--r--   0 j         (1000) j         (1000)       38 2018-03-06 17:19:54.000000 f311-18.3.1.0/setup.cfg
--rw-r--r--   0 j         (1000) j         (1000)     1567 2018-03-01 16:52:51.000000 f311-18.3.1.0/setup.py
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2018-03-06 17:19:54.000000 f311-18.3.1.0/f311.egg-info/
--rw-r--r--   0 j         (1000) j         (1000)        1 2018-03-06 17:19:54.000000 f311-18.3.1.0/f311.egg-info/dependency_links.txt
--rw-r--r--   0 j         (1000) j         (1000)      133 2018-03-06 17:19:54.000000 f311-18.3.1.0/f311.egg-info/requires.txt
--rw-r--r--   0 j         (1000) j         (1000)        5 2018-03-06 17:19:54.000000 f311-18.3.1.0/f311.egg-info/top_level.txt
--rw-r--r--   0 j         (1000) j         (1000)      463 2018-03-06 17:19:54.000000 f311-18.3.1.0/f311.egg-info/PKG-INFO
--rw-r--r--   0 j         (1000) j         (1000)      922 2018-03-06 17:19:54.000000 f311-18.3.1.0/f311.egg-info/SOURCES.txt
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-24 12:53:25.108945 f311-23.7.21.0/
+-rw-rw-r--   0 j         (1000) j         (1000)       40 2020-07-20 14:21:24.000000 f311-23.7.21.0/MANIFEST.in
+-rw-rw-r--   0 j         (1000) j         (1000)      430 2023-07-24 12:53:25.108945 f311-23.7.21.0/PKG-INFO
+-rw-rw-r--   0 j         (1000) j         (1000)      152 2020-07-20 14:21:24.000000 f311-23.7.21.0/README.md
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-24 12:53:25.092944 f311-23.7.21.0/f311/
+-rw-rw-r--   0 j         (1000) j         (1000)      144 2020-07-20 14:21:24.000000 f311-23.7.21.0/f311/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)     8609 2020-07-20 14:21:24.000000 f311-23.7.21.0/f311/collaboration.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-24 12:53:25.096945 f311-23.7.21.0/f311/explorer/
+-rw-rw-r--   0 j         (1000) j         (1000)      595 2020-07-20 14:21:24.000000 f311-23.7.21.0/f311/explorer/__init__.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-24 12:53:25.096945 f311-23.7.21.0/f311/explorer/gui/
+-rw-rw-r--   0 j         (1000) j         (1000)      197 2020-07-20 14:21:24.000000 f311-23.7.21.0/f311/explorer/gui/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)    26066 2020-07-20 14:21:24.000000 f311-23.7.21.0/f311/explorer/gui/a_XExplorer.py
+-rw-rw-r--   0 j         (1000) j         (1000)    15613 2020-07-20 14:21:24.000000 f311-23.7.21.0/f311/explorer/gui/a_XFileMainWindow.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3426 2020-07-20 14:21:24.000000 f311-23.7.21.0/f311/explorer/gui/a_XSelectDataFile.py
+-rw-rw-r--   0 j         (1000) j         (1000)     1367 2020-07-20 14:21:24.000000 f311-23.7.21.0/f311/explorer/gui/a_XText.py
+-rw-rw-r--   0 j         (1000) j         (1000)      712 2020-07-20 14:21:24.000000 f311-23.7.21.0/f311/explorer/util.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-24 12:53:25.100945 f311-23.7.21.0/f311/explorer/vis/
+-rw-rw-r--   0 j         (1000) j         (1000)      211 2020-07-20 14:21:24.000000 f311-23.7.21.0/f311/explorer/vis/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)     1459 2020-07-20 14:21:24.000000 f311-23.7.21.0/f311/explorer/vis/basic.py
+-rw-rw-r--   0 j         (1000) j         (1000)    10719 2023-07-21 16:35:57.000000 f311-23.7.21.0/f311/explorer/vis/plotsp.py
+-rw-rw-r--   0 j         (1000) j         (1000)      228 2020-07-20 14:21:24.000000 f311-23.7.21.0/f311/explorer/vis/visprint.py
+-rw-rw-r--   0 j         (1000) j         (1000)      552 2020-07-20 14:21:24.000000 f311-23.7.21.0/f311/explorer/vis/visspectrum.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-24 12:53:25.104945 f311-23.7.21.0/f311/filetypes/
+-rw-rw-r--   0 j         (1000) j         (1000)      233 2020-07-20 14:21:24.000000 f311-23.7.21.0/f311/filetypes/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3677 2020-07-20 14:21:24.000000 f311-23.7.21.0/f311/filetypes/datafile.py
+-rw-rw-r--   0 j         (1000) j         (1000)     1460 2020-07-20 14:21:24.000000 f311-23.7.21.0/f311/filetypes/filefits.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3034 2020-07-20 14:21:24.000000 f311-23.7.21.0/f311/filetypes/filepy.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3020 2023-07-21 15:37:16.000000 f311-23.7.21.0/f311/filetypes/filespectrum.py
+-rw-rw-r--   0 j         (1000) j         (1000)     6276 2020-07-20 14:21:24.000000 f311-23.7.21.0/f311/filetypes/filesqlitedb.py
+-rw-rw-r--   0 j         (1000) j         (1000)    13438 2020-07-20 14:21:24.000000 f311-23.7.21.0/f311/filetypes/spectrum.py
+-rw-rw-r--   0 j         (1000) j         (1000)   561633 2020-07-20 14:21:24.000000 f311-23.7.21.0/f311/hapi.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2097 2020-07-20 14:21:24.000000 f311-23.7.21.0/f311/pathfinder.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-24 12:53:25.104945 f311-23.7.21.0/f311/scripts/
+-rwxrwxr-x   0 j         (1000) j         (1000)     1362 2020-07-20 14:21:24.000000 f311-23.7.21.0/f311/scripts/cut-spectrum.py
+-rwxrwxr-x   0 j         (1000) j         (1000)      645 2020-07-20 14:21:24.000000 f311-23.7.21.0/f311/scripts/explorer.py
+-rwxrwxr-x   0 j         (1000) j         (1000)     5010 2020-07-20 14:21:24.000000 f311-23.7.21.0/f311/scripts/plot-spectra.py
+-rwxrwxr-x   0 j         (1000) j         (1000)     3461 2020-07-20 14:21:24.000000 f311-23.7.21.0/f311/scripts/programs.py
+-rw-rw-r--   0 j         (1000) j         (1000)     8708 2020-07-20 14:21:24.000000 f311-23.7.21.0/f311/util.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-24 12:53:25.096945 f311-23.7.21.0/f311.egg-info/
+-rw-rw-r--   0 j         (1000) j         (1000)      430 2023-07-24 12:53:25.000000 f311-23.7.21.0/f311.egg-info/PKG-INFO
+-rw-rw-r--   0 j         (1000) j         (1000)      922 2023-07-24 12:53:25.000000 f311-23.7.21.0/f311.egg-info/SOURCES.txt
+-rw-rw-r--   0 j         (1000) j         (1000)        1 2023-07-24 12:53:25.000000 f311-23.7.21.0/f311.egg-info/dependency_links.txt
+-rw-rw-r--   0 j         (1000) j         (1000)      133 2023-07-24 12:53:25.000000 f311-23.7.21.0/f311.egg-info/requires.txt
+-rw-rw-r--   0 j         (1000) j         (1000)        5 2023-07-24 12:53:25.000000 f311-23.7.21.0/f311.egg-info/top_level.txt
+-rw-rw-r--   0 j         (1000) j         (1000)       38 2023-07-24 12:53:25.108945 f311-23.7.21.0/setup.cfg
+-rw-rw-r--   0 j         (1000) j         (1000)     1568 2023-07-21 15:30:00.000000 f311-23.7.21.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `f311-18.3.1.0/f311/explorer/gui/a_XText.py` & `f311-23.7.21.0/f311/explorer/gui/a_XText.py`

 * *Files identical despite different names*

### Comparing `f311-18.3.1.0/f311/explorer/gui/a_XFileMainWindow.py` & `f311-23.7.21.0/f311/explorer/gui/a_XFileMainWindow.py`

 * *Files identical despite different names*

### Comparing `f311-18.3.1.0/f311/explorer/gui/a_XSelectDataFile.py` & `f311-23.7.21.0/f311/explorer/gui/a_XSelectDataFile.py`

 * *Files identical despite different names*

### Comparing `f311-18.3.1.0/f311/explorer/gui/a_XExplorer.py` & `f311-23.7.21.0/f311/explorer/gui/a_XExplorer.py`

 * *Files identical despite different names*

### Comparing `f311-18.3.1.0/f311/explorer/vis/plotsp.py` & `f311-23.7.21.0/f311/explorer/vis/plotsp.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,24 +35,32 @@
 
     Args:
         fmt_xlabel: format string for x-label
         fmt_ylabel: format string for y-label
         fmt_title: format string for title
         ymin: (optional) force mininum y-value
         flag_legend: Whether to show legend in plot
+        flag_xlabel:
+        flag_ylabel:
+        flag_ignore_units: if True, mismatching units [between spectra] will be ignored
+        stylespecs: dictionary with optional keys "c<i>", "lw<i>", "s<i>" (color, line width and line style), where <i>
+                    is the 0-based spectrum index
     """
     def __init__(self, fmt_xlabel="{.xunit}", fmt_ylabel="{.yunit}", fmt_title="{.title}",
-                 ymin=None, flag_legend=True, flag_xlabel=True, flag_ylabel=True):
+                 ymin=None, flag_legend=True, flag_xlabel=True, flag_ylabel=True,
+                 flag_ignore_units=True, stylespecs=None):
         self.flag_xlabel = flag_xlabel
         self.flag_ylabel = flag_ylabel
         self.fmt_xlabel = fmt_xlabel
         self.fmt_ylabel = fmt_ylabel
         self.fmt_title = fmt_title
         self.ymin = ymin
         self.flag_legend = flag_legend
+        self.flag_ignore_units=flag_ignore_units
+        self.stylespecs = stylespecs
 
     def __repr__(self):
         return "{}('{}', '{}', '{}', {}, {})".format(self.__class__.__name__,self.fmt_xlabel,
           self.fmt_ylabel, self.fmt_title, self.ymin, self.flag_legend)
 
 
 _default_setup = PlotSpectrumSetup()
@@ -96,26 +104,26 @@
     a99.format_BLB()
     if len(ss) > 0:
         xunit, yunit = None, None
         for i, s in enumerate(ss):
             if xunit is None:
                 xunit = s.xunit
             else:
-                if xunit != s.xunit:
+                if xunit != s.xunit and not setup.flag_ignore_units:
                     raise RuntimeError("Spectra x-units do not match")
 
             if yunit is None:
                 yunit = s.yunit
             else:
-                if yunit != s.yunit:
+                if yunit != s.yunit and not setup.flag_ignore_units:
                     raise RuntimeError("Spectra x-units do not match")
 
             ax = plt.gca()
             y = s.y
-            ax.plot(s.x, y, label=str(s.title))
+            _plot_with_styles(ax, s.x, y, str(s.title), setup.stylespecs, i)
 
         # plt.ylabel('({})'.format(yunit))
         # **Note** Takes last spectrum as reference to mount x-label
         if setup.flag_xlabel and setup.fmt_xlabel:
             _set_plot(plt.xlabel, setup.fmt_xlabel, s)
         xmin, xmax, ymin_, ymax, xspan, yspan = calc_max_min(ss)
         ymin = ymin_ if setup.ymin is None else setup.ymin
@@ -126,14 +134,21 @@
             a99.format_legend(leg)
         plt.tight_layout()
 
     if title is not None:
         plt.gcf().canvas.set_window_title(title)
 
 
+def _plot_with_styles(ax, x, y, label, stylespecs, i):
+    ax.plot(x, y, label=label,
+            c=stylespecs.get(f"c{i}"),
+            lw=stylespecs.get(f"lw{i}"),
+            linestyle=stylespecs.get(f"s{i}"))
+
+
 def plot_spectra_pieces_pdf(ss, aint=10, pdf_filename='pieces.pdf', setup=_default_setup):
     """
     Plots spectra, overlapped, in small wavelength intervals into a PDF file,
     one interval per page of the PDF file.
 
     Args:
       ss: list of Spectrum objects
@@ -274,21 +289,21 @@
         if len(s.x) > 0:
             xmin, xmax = min(min(s.x), xmin), max(max(s.x), xmax)
             any_span = True
 
         if xunit is None:
             xunit = s.xunit
         else:
-            if xunit != s.xunit:
+            if xunit != s.xunit and not setup.flag_ignore_units:
                 raise RuntimeError("Spectra x-units do not match")
 
         if yunit is None:
             yunit = s.yunit
         else:
-            if yunit != s.yunit:
+            if yunit != s.yunit and not setup.flag_ignore_units:
                 raise RuntimeError("Spectra x-units do not match")
 
     if any_span:
         span = xmax - xmin
         ax.set_xlim([xmin - span * _T, xmax + span * _T])
     for j in range(num_cols):
         ax = axarr[num_rows - 1, j]
```

### Comparing `f311-18.3.1.0/f311/explorer/vis/basic.py` & `f311-23.7.21.0/f311/explorer/vis/basic.py`

 * *Files identical despite different names*

### Comparing `f311-18.3.1.0/f311/explorer/vis/visspectrum.py` & `f311-23.7.21.0/f311/explorer/vis/visspectrum.py`

 * *Files identical despite different names*

### Comparing `f311-18.3.1.0/f311/explorer/__init__.py` & `f311-23.7.21.0/f311/explorer/__init__.py`

 * *Files identical despite different names*

### Comparing `f311-18.3.1.0/f311/explorer/util.py` & `f311-23.7.21.0/f311/explorer/util.py`

 * *Files identical despite different names*

### Comparing `f311-18.3.1.0/f311/hapi.py` & `f311-23.7.21.0/f311/hapi.py`

 * *Files identical despite different names*

### Comparing `f311-18.3.1.0/f311/scripts/plot-spectra.py` & `f311-23.7.21.0/f311/scripts/plot-spectra.py`

 * *Files identical despite different names*

### Comparing `f311-18.3.1.0/f311/scripts/programs.py` & `f311-23.7.21.0/f311/scripts/programs.py`

 * *Files identical despite different names*

### Comparing `f311-18.3.1.0/f311/scripts/cut-spectrum.py` & `f311-23.7.21.0/f311/scripts/cut-spectrum.py`

 * *Files identical despite different names*

### Comparing `f311-18.3.1.0/f311/scripts/explorer.py` & `f311-23.7.21.0/f311/scripts/explorer.py`

 * *Files identical despite different names*

### Comparing `f311-18.3.1.0/f311/filetypes/spectrum.py` & `f311-23.7.21.0/f311/filetypes/spectrum.py`

 * *Files identical despite different names*

### Comparing `f311-18.3.1.0/f311/filetypes/datafile.py` & `f311-23.7.21.0/f311/filetypes/datafile.py`

 * *Files identical despite different names*

### Comparing `f311-18.3.1.0/f311/filetypes/filefits.py` & `f311-23.7.21.0/f311/filetypes/filefits.py`

 * *Files identical despite different names*

### Comparing `f311-18.3.1.0/f311/filetypes/filespectrum.py` & `f311-23.7.21.0/f311/filetypes/filespectrum.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,28 +33,41 @@
     "Lambda-flux" Spectrum (2-column text file)
 
     File may have comment lines; these will be ignored altogether, because the file
     is read with numpy.loadtxt()
     """
 
     def _do_load(self, filename):
+        sp = self.spectrum = Spectrum()
+
+        # Reads metadata first
+        with open(filename, "r") as f:
+            for line in f:
+                if not line.startswith("#"):
+                    break
+                if line.startswith("# Title:"):
+                    sp.title = line[8:].strip()
+
+        # Now leaves it to numpy
         A = np.loadtxt(filename)
         if len(A.shape) < 2:
             raise RuntimeError("File {0!s} does not contain 2D array".format(filename))
         if A.shape[1] < 2:
             raise RuntimeError("File {0!s} must contain at least two columns".format(filename))
         if A.shape[1] > 2:
             a99.get_python_logger().warning("File {0!s} has more than two columns, taking only first and second".format(filename))
-        sp = self.spectrum = Spectrum()
         sp.x = A[:, 0]
         sp.y = A[:, 1]
 
 
     def _do_save_as(self, filename):
         with open(filename, "w") as h:
+            title = self.spectrum.title
+            if title:
+                write_lf(h, f"# Title: {title}")
             for x, y in zip(self.spectrum.x, self.spectrum.y):
                 write_lf(h, "{0:.10g} {1:.10g}".format(x, y))
 
 
 class FileSpectrumFits(FileSpectrum):
     """FITS Spectrum"""
     flag_txt = False
```

### Comparing `f311-18.3.1.0/f311/filetypes/filepy.py` & `f311-23.7.21.0/f311/filetypes/filepy.py`

 * *Files identical despite different names*

### Comparing `f311-18.3.1.0/f311/filetypes/filesqlitedb.py` & `f311-23.7.21.0/f311/filetypes/filesqlitedb.py`

 * *Files identical despite different names*

### Comparing `f311-18.3.1.0/f311/collaboration.py` & `f311-23.7.21.0/f311/collaboration.py`

 * *Files identical despite different names*

### Comparing `f311-18.3.1.0/f311/pathfinder.py` & `f311-23.7.21.0/f311/pathfinder.py`

 * *Files identical despite different names*

### Comparing `f311-18.3.1.0/f311/util.py` & `f311-23.7.21.0/f311/util.py`

 * *Files identical despite different names*

### Comparing `f311-18.3.1.0/setup.py` & `f311-23.7.21.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 pkgs = find_packages()
 scripts = find_scripts([PACKAGE_NAME])
 
 setup(
     name=PACKAGE_NAME,
     packages=find_packages(),
     include_package_data=True,
-    version='18.3.1.0',
+    version='23.7.21.0',
     license='GNU GPLv3',
     platforms='any',
     description='Astronomy-related API, command-line tools, and windowed applications',
     author='Julio Trevisan',
     author_email='juliotrevisan@gmail.com',
     url='https://github.com/trevisanj/f311',
     keywords= ['astronomy', "fits", "spectroscopy", "spectral synthesis", "photometry",
```

### Comparing `f311-18.3.1.0/f311.egg-info/SOURCES.txt` & `f311-23.7.21.0/f311.egg-info/SOURCES.txt`

 * *Files identical despite different names*

