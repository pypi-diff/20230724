# Comparing `tmp/plotly-extend-wrapper-0.0.1.tar.gz` & `tmp/plotly-extend-wrapper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotly-extend-wrapper-0.0.1.tar", last modified: Thu Jul  6 05:13:20 2023, max compression
+gzip compressed data, was "plotly-extend-wrapper-0.0.2.tar", last modified: Mon Jul 24 02:22:21 2023, max compression
```

## Comparing `plotly-extend-wrapper-0.0.1.tar` & `plotly-extend-wrapper-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-sr-x   0 sumi     (10014) pana     (10000)        0 2023-07-06 05:13:19.476178 plotly-extend-wrapper-0.0.1/
--rw-r--r--   0 sumi     (10014) pana     (10000)     1070 2023-07-06 04:24:37.000000 plotly-extend-wrapper-0.0.1/LICENSE
--rw-r--r--   0 sumi     (10014) pana     (10000)      465 2023-07-06 05:13:19.476178 plotly-extend-wrapper-0.0.1/PKG-INFO
--rw-r--r--   0 sumi     (10014) pana     (10000)      173 2023-07-06 05:11:49.000000 plotly-extend-wrapper-0.0.1/README.md
-drwxr-sr-x   0 sumi     (10014) pana     (10000)        0 2023-07-06 05:13:19.467178 plotly-extend-wrapper-0.0.1/plotly_extend_wrapper/
--rw-r--r--   0 sumi     (10014) pana     (10000)      206 2023-07-06 04:58:30.000000 plotly-extend-wrapper-0.0.1/plotly_extend_wrapper/__init__.py
--rw-r--r--   0 sumi     (10014) pana     (10000)      281 2023-07-06 04:59:17.000000 plotly-extend-wrapper-0.0.1/plotly_extend_wrapper/common.py
--rw-r--r--   0 sumi     (10014) pana     (10000)     2434 2023-07-06 04:59:54.000000 plotly-extend-wrapper-0.0.1/plotly_extend_wrapper/updater.py
--rw-r--r--   0 sumi     (10014) pana     (10000)     8841 2023-07-06 05:00:12.000000 plotly-extend-wrapper-0.0.1/plotly_extend_wrapper/wrapper.py
-drwxr-sr-x   0 sumi     (10014) pana     (10000)        0 2023-07-06 05:13:19.474178 plotly-extend-wrapper-0.0.1/plotly_extend_wrapper.egg-info/
--rw-r--r--   0 sumi     (10014) pana     (10000)      465 2023-07-06 05:13:19.000000 plotly-extend-wrapper-0.0.1/plotly_extend_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 sumi     (10014) pana     (10000)      397 2023-07-06 05:13:19.000000 plotly-extend-wrapper-0.0.1/plotly_extend_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 sumi     (10014) pana     (10000)        1 2023-07-06 05:13:19.000000 plotly-extend-wrapper-0.0.1/plotly_extend_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 sumi     (10014) pana     (10000)       43 2023-07-06 05:13:19.000000 plotly-extend-wrapper-0.0.1/plotly_extend_wrapper.egg-info/requires.txt
--rw-r--r--   0 sumi     (10014) pana     (10000)       22 2023-07-06 05:13:19.000000 plotly-extend-wrapper-0.0.1/plotly_extend_wrapper.egg-info/top_level.txt
--rw-r--r--   0 sumi     (10014) pana     (10000)      477 2023-07-06 05:11:09.000000 plotly-extend-wrapper-0.0.1/pyproject.toml
--rw-r--r--   0 sumi     (10014) pana     (10000)       38 2023-07-06 05:13:19.477178 plotly-extend-wrapper-0.0.1/setup.cfg
--rw-r--r--   0 sumi     (10014) pana     (10000)     1190 2023-07-06 05:13:13.000000 plotly-extend-wrapper-0.0.1/setup.py
+drwxr-sr-x   0 sumi     (10014) pana     (10000)        0 2023-07-24 02:22:21.415985 plotly-extend-wrapper-0.0.2/
+-rw-r--r--   0 sumi     (10014) pana     (10000)     1070 2023-07-06 04:24:37.000000 plotly-extend-wrapper-0.0.2/LICENSE
+-rw-r--r--   0 sumi     (10014) pana     (10000)     1080 2023-07-24 02:22:21.414985 plotly-extend-wrapper-0.0.2/PKG-INFO
+-rw-r--r--   0 sumi     (10014) pana     (10000)      574 2023-07-10 07:26:56.000000 plotly-extend-wrapper-0.0.2/README.md
+drwxr-sr-x   0 sumi     (10014) pana     (10000)        0 2023-07-24 02:22:21.406985 plotly-extend-wrapper-0.0.2/plotly_extend_wrapper/
+-rw-r--r--   0 sumi     (10014) pana     (10000)      154 2023-07-10 07:28:02.000000 plotly-extend-wrapper-0.0.2/plotly_extend_wrapper/__init__.py
+-rw-r--r--   0 sumi     (10014) pana     (10000)      262 2023-07-06 05:45:30.000000 plotly-extend-wrapper-0.0.2/plotly_extend_wrapper/common.py
+-rw-r--r--   0 sumi     (10014) pana     (10000)     2415 2023-07-06 05:45:46.000000 plotly-extend-wrapper-0.0.2/plotly_extend_wrapper/updater.py
+-rw-r--r--   0 sumi     (10014) pana     (10000)    10750 2023-07-24 02:15:08.000000 plotly-extend-wrapper-0.0.2/plotly_extend_wrapper/wrapper.py
+drwxr-sr-x   0 sumi     (10014) pana     (10000)        0 2023-07-24 02:22:21.412985 plotly-extend-wrapper-0.0.2/plotly_extend_wrapper.egg-info/
+-rw-r--r--   0 sumi     (10014) pana     (10000)     1080 2023-07-24 02:22:21.000000 plotly-extend-wrapper-0.0.2/plotly_extend_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 sumi     (10014) pana     (10000)      397 2023-07-24 02:22:21.000000 plotly-extend-wrapper-0.0.2/plotly_extend_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 sumi     (10014) pana     (10000)        1 2023-07-24 02:22:21.000000 plotly-extend-wrapper-0.0.2/plotly_extend_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 sumi     (10014) pana     (10000)       43 2023-07-24 02:22:21.000000 plotly-extend-wrapper-0.0.2/plotly_extend_wrapper.egg-info/requires.txt
+-rw-r--r--   0 sumi     (10014) pana     (10000)       22 2023-07-24 02:22:21.000000 plotly-extend-wrapper-0.0.2/plotly_extend_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 sumi     (10014) pana     (10000)      466 2023-07-10 07:27:32.000000 plotly-extend-wrapper-0.0.2/pyproject.toml
+-rw-r--r--   0 sumi     (10014) pana     (10000)       38 2023-07-24 02:22:21.415985 plotly-extend-wrapper-0.0.2/setup.cfg
+-rw-r--r--   0 sumi     (10014) pana     (10000)     1254 2023-07-24 02:22:02.000000 plotly-extend-wrapper-0.0.2/setup.py
```

### Comparing `plotly-extend-wrapper-0.0.1/LICENSE` & `plotly-extend-wrapper-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `plotly-extend-wrapper-0.0.1/plotly_extend_wrapper/updater.py` & `plotly-extend-wrapper-0.0.2/plotly_extend_wrapper/updater.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# encoding: utf-8
-
 from pathlib import Path
 from plotly import io as pio
 
 
 class Update_plotly_object:
     def __init__(self, po):
         self.po = po
```

### Comparing `plotly-extend-wrapper-0.0.1/plotly_extend_wrapper/wrapper.py` & `plotly-extend-wrapper-0.0.2/plotly_extend_wrapper/wrapper.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,93 @@
-# encoding: utf-8
-
 from plotly import express as px
 from plotly.subplots import make_subplots
 import pandas as pd
 from plotly_extend_wrapper.common import check_directory
 
 
 def Plot_pie(data: pd.DataFrame, target: str, **kwargs):
+    """Make pie plot
+
+    Parameters
+    ----------
+    data : pd.DataFrame
+        pandas.DataFrame included data to make pie chart
+    target : str
+        String which column you would like to use for pie chart
+
+    Returns
+    -------
+    plotly.graph_objects
+        Object of pie chart
+    """
     vc = data[target].value_counts().reset_index(name="count")
     return px.pie(
         vc,
         names="index",
         values="count",
         **kwargs
     )
 
 
 def Plot_sunburst(data: pd.DataFrame, groups: list, **kwargs):
+    """Make sunburst plot
+
+    Parameters
+    ----------
+    data : pd.DataFrame
+        pandas.DataFrame included data to make sunburst chart
+    groups : list
+        Strings list of group
+        Changed when you replace the order
+
+    Returns
+    -------
+    plotly.graph_objects
+        Object of sunburst chart
+    """
     vc = data.value_counts(subset=groups).reset_index(name="count")
     return px.sunburst(
         vc,
         path=groups,
         values="count",
         **kwargs
     )
 
 
-class scatter_with_size():
+class Plot_bubble_chart():
+    """Make bubble chart
+    """
     def __init__(self, df, x, y, color=None, facet_col=None, facet_row=None, rounded=None, decimals=None, normalize=False, smoothing=False, offset=0, **kwargs):
+        """Initialize function
+
+        Parameters
+        ----------
+        df : pandas.DataFrame
+            pandas.DataFrame included data to make plot
+        x : str
+            X-axis column's name
+        y : str
+            Y-axis column's name
+        color : str, optional
+            Column name you want colorize with data, by default None
+        facet_col : str, optional
+            Column name you want plot separeted vertically, by default None
+        facet_row : str, optional
+            Column name you want plot separeted horizontally, by default None
+        rounded : list, optional
+            Columns list which columns you want to round data, by default None
+        decimals : list, optional
+            Decimals list what level you want to round for each columns, by default None
+        normalize : bool, optional
+            If True, bubble size is calculated as normalized, by default False
+        smoothing : bool, optional
+            If True, bubble size were smoothed between each plot, by default False
+        offset : int, optional
+            Offset value for bubble size, by default 0
+        """
         self.df = df.copy()
         self.x = x
         self.y = y
         self.color = color
         self.facet_col = facet_col
         self.facet_row = facet_row
         self.rounded = rounded
@@ -107,16 +163,31 @@
             **self.kwargs
         )
 
     def __call__(self):
         return self.plot
 
 
-def plotly_line(df: pd.DataFrame, x, y, secondary_y, xtitle=None, ytitle=None, secondary_ytitle=None, save_html_path=None, vspan=None,
-                vspan_color_randomize=False, sort_column=True, sort_x=True, opacity=0.2, px_kwargs=dict(), **kwargs):
+def Plot_line(
+        df: pd.DataFrame,
+        x: str,
+        y: list,
+        secondary_y: list,
+        xtitle=None,
+        ytitle=None,
+        secondary_ytitle=None,
+        save_html_path=None,
+        vspan=None,
+        vspan_color_randomize=False,
+        sort_column=True,
+        sort_x=True,
+        opacity=0.2,
+        px_kwargs=dict(),
+        **kwargs
+    ):
     """Make line graph with secondary y using plotly.express
 
     Parameters
     ----------
     df : pd.DataFrame
         Original dataframe
     x : str
@@ -211,15 +282,15 @@
         output_p = check_directory(save_html_path)
         subfig.write_html(output_p)
         print(f"Ouput html file [{output_p}]")
 
     return subfig
 
 
-def bubble_chart_with_line(bubble_plot, line_info: dict, x1, x2, xtitle=None, ytitle=None, **kwargs):
+def Plot_bubble_chart_with_line(bubble_plot, line_info: dict, x1, x2, xtitle=None, ytitle=None, **kwargs):
     """Making bubble chart with linear plot
 
     Parameters
     ----------
     bubble_plot : Figure
         Bubble chart object
     line_info : dict
```

### Comparing `plotly-extend-wrapper-0.0.1/setup.py` & `plotly-extend-wrapper-0.0.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# encoding: utf-8
 # Author: Laplusdestiny <prayonshootingstars@gmail.com>
 # Copyright (c) 2023-2023 Laplusdestiny
 # License: MIT
 
 from setuptools import setup
 import plotly_extend_wrapper
 
@@ -35,15 +34,17 @@
 setup(
     name=NAME,
     author=AUTHOR,
     author_email=AUTHOR_EMAIL,
     maintainer=AUTHOR,
     maintainer_email=AUTHOR_EMAIL,
     description=DESCRIPTION,
-    README=readme,
+    # README=readme,
+    long_description_content_type="text/markdown",
+    long_description=readme,
     license=LICENSE,
     url=URL,
     version=VERSION,
     download_url=DOWNLOAD_URL,
     python_requires=PYTHON_REQUIRES,
     install_requires=INSTALL_REQUIRES,
     packages=PACKAGES,
```

