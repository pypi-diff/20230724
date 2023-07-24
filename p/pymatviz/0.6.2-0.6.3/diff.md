# Comparing `tmp/pymatviz-0.6.2.tar.gz` & `tmp/pymatviz-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymatviz-0.6.2.tar", last modified: Sat Apr 29 23:06:37 2023, max compression
+gzip compressed data, was "pymatviz-0.6.3.tar", last modified: Mon Jul 24 16:29:48 2023, max compression
```

## Comparing `pymatviz-0.6.2.tar` & `pymatviz-0.6.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 janosh     (501) wheel        (0)        0 2023-04-29 23:06:37.016901 pymatviz-0.6.2/
--rw-r--r--   0 janosh     (501) wheel        (0)    17362 2023-04-29 23:06:37.016698 pymatviz-0.6.2/PKG-INFO
--rw-r--r--   0 janosh     (501) wheel        (0)     1073 2021-08-04 10:50:41.000000 pymatviz-0.6.2/license
-drwxr-xr-x   0 janosh     (501) wheel        (0)        0 2023-04-29 23:06:37.012068 pymatviz-0.6.2/pymatviz/
--rw-r--r--   0 janosh     (501) wheel        (0)     2238 2023-03-27 18:51:03.000000 pymatviz-0.6.2/pymatviz/__init__.py
--rw-r--r--   0 janosh     (501) wheel        (0)     3675 2023-02-18 02:11:20.000000 pymatviz-0.6.2/pymatviz/correlation.py
--rw-r--r--   0 janosh     (501) wheel        (0)     2995 2023-02-20 20:13:42.000000 pymatviz-0.6.2/pymatviz/cumulative.py
--rw-r--r--   0 janosh     (501) wheel        (0)    19361 2022-12-30 20:51:55.000000 pymatviz-0.6.2/pymatviz/elements.csv
--rw-r--r--   0 janosh     (501) wheel        (0)    12350 2023-03-12 00:39:26.000000 pymatviz-0.6.2/pymatviz/histograms.py
--rw-r--r--   0 janosh     (501) wheel        (0)     9804 2023-03-27 18:51:03.000000 pymatviz-0.6.2/pymatviz/parity.py
--rw-r--r--   0 janosh     (501) wheel        (0)     1277 2023-02-20 19:27:21.000000 pymatviz-0.6.2/pymatviz/plot_defaults.py
--rw-r--r--   0 janosh     (501) wheel        (0)    28565 2023-04-16 23:28:04.000000 pymatviz-0.6.2/pymatviz/ptable.py
--rw-r--r--   0 janosh     (501) wheel        (0)     2795 2023-02-18 02:11:20.000000 pymatviz-0.6.2/pymatviz/relevance.py
--rw-r--r--   0 janosh     (501) wheel        (0)     2115 2023-03-27 18:51:03.000000 pymatviz-0.6.2/pymatviz/sankey.py
--rw-r--r--   0 janosh     (501) wheel        (0)    16624 2023-03-21 18:36:59.000000 pymatviz-0.6.2/pymatviz/structure_viz.py
--rw-r--r--   0 janosh     (501) wheel        (0)     2584 2023-04-16 23:28:04.000000 pymatviz-0.6.2/pymatviz/sunburst.py
--rw-r--r--   0 janosh     (501) wheel        (0)     9695 2023-02-18 02:11:20.000000 pymatviz-0.6.2/pymatviz/uncertainty.py
--rw-r--r--   0 janosh     (501) wheel        (0)    17038 2023-04-02 04:05:42.000000 pymatviz-0.6.2/pymatviz/utils.py
-drwxr-xr-x   0 janosh     (501) wheel        (0)        0 2023-04-29 23:06:37.013430 pymatviz-0.6.2/pymatviz.egg-info/
--rw-r--r--   0 janosh     (501) wheel        (0)    17362 2023-04-29 23:06:37.000000 pymatviz-0.6.2/pymatviz.egg-info/PKG-INFO
--rw-r--r--   0 janosh     (501) wheel        (0)      779 2023-04-29 23:06:37.000000 pymatviz-0.6.2/pymatviz.egg-info/SOURCES.txt
--rw-r--r--   0 janosh     (501) wheel        (0)        1 2023-04-29 23:06:37.000000 pymatviz-0.6.2/pymatviz.egg-info/dependency_links.txt
--rw-r--r--   0 janosh     (501) wheel        (0)      191 2023-04-29 23:06:37.000000 pymatviz-0.6.2/pymatviz.egg-info/requires.txt
--rw-r--r--   0 janosh     (501) wheel        (0)        9 2023-04-29 23:06:37.000000 pymatviz-0.6.2/pymatviz.egg-info/top_level.txt
--rw-r--r--   0 janosh     (501) wheel        (0)     2751 2023-04-29 23:04:24.000000 pymatviz-0.6.2/pyproject.toml
--rw-r--r--   0 janosh     (501) wheel        (0)    15353 2023-03-12 22:42:32.000000 pymatviz-0.6.2/readme.md
--rw-r--r--   0 janosh     (501) wheel        (0)       38 2023-04-29 23:06:37.016949 pymatviz-0.6.2/setup.cfg
-drwxr-xr-x   0 janosh     (501) wheel        (0)        0 2023-04-29 23:06:37.016436 pymatviz-0.6.2/tests/
--rw-r--r--   0 janosh     (501) wheel        (0)      464 2022-10-15 03:29:31.000000 pymatviz-0.6.2/tests/test_correlation.py
--rw-r--r--   0 janosh     (501) wheel        (0)      705 2022-12-24 23:29:33.000000 pymatviz-0.6.2/tests/test_cumulative.py
--rw-r--r--   0 janosh     (501) wheel        (0)     2370 2023-02-20 19:25:40.000000 pymatviz-0.6.2/tests/test_histograms.py
--rw-r--r--   0 janosh     (501) wheel        (0)     2575 2023-02-20 20:13:42.000000 pymatviz-0.6.2/tests/test_parity.py
--rw-r--r--   0 janosh     (501) wheel        (0)    10014 2023-04-16 23:28:04.000000 pymatviz-0.6.2/tests/test_ptable.py
--rw-r--r--   0 janosh     (501) wheel        (0)      496 2023-02-21 20:10:51.000000 pymatviz-0.6.2/tests/test_readme.py
--rw-r--r--   0 janosh     (501) wheel        (0)     1272 2022-10-14 17:22:38.000000 pymatviz-0.6.2/tests/test_relevance.py
--rw-r--r--   0 janosh     (501) wheel        (0)      589 2022-10-08 23:23:21.000000 pymatviz-0.6.2/tests/test_sankey.py
--rw-r--r--   0 janosh     (501) wheel        (0)     2124 2023-03-20 20:58:57.000000 pymatviz-0.6.2/tests/test_structure_viz.py
--rw-r--r--   0 janosh     (501) wheel        (0)      960 2022-10-08 23:23:21.000000 pymatviz-0.6.2/tests/test_sunburst.py
--rw-r--r--   0 janosh     (501) wheel        (0)     2006 2023-02-20 19:27:21.000000 pymatviz-0.6.2/tests/test_uncertainty.py
--rw-r--r--   0 janosh     (501) wheel        (0)     6038 2023-04-02 04:05:42.000000 pymatviz-0.6.2/tests/test_utils.py
+drwxr-xr-x   0 janosh     (501) wheel        (0)        0 2023-07-24 16:29:48.371163 pymatviz-0.6.3/
+-rw-r--r--   0 janosh     (501) wheel        (0)    17343 2023-07-24 16:29:48.370947 pymatviz-0.6.3/PKG-INFO
+-rw-r--r--   0 janosh     (501) wheel        (0)     1073 2021-08-04 10:50:41.000000 pymatviz-0.6.3/license
+drwxr-xr-x   0 janosh     (501) wheel        (0)        0 2023-07-24 16:29:48.368153 pymatviz-0.6.3/pymatviz/
+-rw-r--r--   0 janosh     (501) wheel        (0)     1233 2023-06-09 08:49:08.000000 pymatviz-0.6.3/pymatviz/__init__.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     3785 2023-07-13 00:18:14.000000 pymatviz-0.6.3/pymatviz/correlation.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     3105 2023-07-13 00:18:01.000000 pymatviz-0.6.3/pymatviz/cumulative.py
+-rw-r--r--   0 janosh     (501) wheel        (0)    19361 2022-12-30 20:51:55.000000 pymatviz-0.6.3/pymatviz/elements.csv
+-rw-r--r--   0 janosh     (501) wheel        (0)    12437 2023-06-23 02:50:53.000000 pymatviz-0.6.3/pymatviz/histograms.py
+-rw-r--r--   0 janosh     (501) wheel        (0)    10219 2023-06-23 02:50:53.000000 pymatviz-0.6.3/pymatviz/parity.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     1277 2023-05-19 14:05:47.000000 pymatviz-0.6.3/pymatviz/plot_defaults.py
+-rw-r--r--   0 janosh     (501) wheel        (0)    28940 2023-07-24 14:58:17.000000 pymatviz-0.6.3/pymatviz/ptable.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     2929 2023-06-23 02:50:53.000000 pymatviz-0.6.3/pymatviz/relevance.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     2144 2023-05-19 14:05:47.000000 pymatviz-0.6.3/pymatviz/sankey.py
+-rw-r--r--   0 janosh     (501) wheel        (0)    16767 2023-06-23 02:51:05.000000 pymatviz-0.6.3/pymatviz/structure_viz.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     2594 2023-05-19 14:10:31.000000 pymatviz-0.6.3/pymatviz/sunburst.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     9878 2023-06-23 02:50:53.000000 pymatviz-0.6.3/pymatviz/uncertainty.py
+-rw-r--r--   0 janosh     (501) wheel        (0)    18274 2023-06-23 02:50:53.000000 pymatviz-0.6.3/pymatviz/utils.py
+drwxr-xr-x   0 janosh     (501) wheel        (0)        0 2023-07-24 16:29:48.369048 pymatviz-0.6.3/pymatviz.egg-info/
+-rw-r--r--   0 janosh     (501) wheel        (0)    17343 2023-07-24 16:29:48.000000 pymatviz-0.6.3/pymatviz.egg-info/PKG-INFO
+-rw-r--r--   0 janosh     (501) wheel        (0)      779 2023-07-24 16:29:48.000000 pymatviz-0.6.3/pymatviz.egg-info/SOURCES.txt
+-rw-r--r--   0 janosh     (501) wheel        (0)        1 2023-07-24 16:29:48.000000 pymatviz-0.6.3/pymatviz.egg-info/dependency_links.txt
+-rw-r--r--   0 janosh     (501) wheel        (0)      191 2023-07-24 16:29:48.000000 pymatviz-0.6.3/pymatviz.egg-info/requires.txt
+-rw-r--r--   0 janosh     (501) wheel        (0)        9 2023-07-24 16:29:48.000000 pymatviz-0.6.3/pymatviz.egg-info/top_level.txt
+-rw-r--r--   0 janosh     (501) wheel        (0)     3506 2023-07-24 16:18:28.000000 pymatviz-0.6.3/pyproject.toml
+-rw-r--r--   0 janosh     (501) wheel        (0)    15334 2023-07-12 18:09:34.000000 pymatviz-0.6.3/readme.md
+-rw-r--r--   0 janosh     (501) wheel        (0)       38 2023-07-24 16:29:48.371222 pymatviz-0.6.3/setup.cfg
+drwxr-xr-x   0 janosh     (501) wheel        (0)        0 2023-07-24 16:29:48.370714 pymatviz-0.6.3/tests/
+-rw-r--r--   0 janosh     (501) wheel        (0)      464 2022-10-15 03:29:31.000000 pymatviz-0.6.3/tests/test_correlation.py
+-rw-r--r--   0 janosh     (501) wheel        (0)      705 2022-12-24 23:29:33.000000 pymatviz-0.6.3/tests/test_cumulative.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     2435 2023-05-24 19:03:25.000000 pymatviz-0.6.3/tests/test_histograms.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     2982 2023-07-13 00:17:35.000000 pymatviz-0.6.3/tests/test_parity.py
+-rw-r--r--   0 janosh     (501) wheel        (0)    11234 2023-07-24 16:09:09.000000 pymatviz-0.6.3/tests/test_ptable.py
+-rw-r--r--   0 janosh     (501) wheel        (0)      496 2023-02-21 20:10:51.000000 pymatviz-0.6.3/tests/test_readme.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     1378 2023-05-24 19:03:32.000000 pymatviz-0.6.3/tests/test_relevance.py
+-rw-r--r--   0 janosh     (501) wheel        (0)      589 2022-10-08 23:23:21.000000 pymatviz-0.6.3/tests/test_sankey.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     2106 2023-05-19 14:05:47.000000 pymatviz-0.6.3/tests/test_structure_viz.py
+-rw-r--r--   0 janosh     (501) wheel        (0)      999 2023-05-19 14:05:47.000000 pymatviz-0.6.3/tests/test_sunburst.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     2083 2023-05-24 19:03:14.000000 pymatviz-0.6.3/tests/test_uncertainty.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     7887 2023-07-22 13:56:32.000000 pymatviz-0.6.3/tests/test_utils.py
```

### Comparing `pymatviz-0.6.2/PKG-INFO` & `pymatviz-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymatviz
-Version: 0.6.2
+Version: 0.6.3
 Summary: A toolkit for visualizations in materials informatics
 Author-email: Janosh Riebesell <janosh.riebesell@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Janosh Riebesell
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,20 +22,20 @@
         fitness for a particular purpose and noninfringement. In no event shall the
         authors or copyright holders be liable for any claim, damages or other
         liability, whether in an action of contract, tort or otherwise, arising from,
         out of or in connection with the software or the use or other dealings in the
         software.
         
 Project-URL: Homepage, https://github.com/janosh/pymatviz
-Keywords: science,materials informatics,materials discovery,chemistry,data visualization,plotly,matplotlib
-Classifier: Programming Language :: Python :: 3
+Keywords: chemistry,data visualization,materials discovery,materials informatics,matplotlib,plotly,science
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: data-src
 Provides-Extra: export-figs
 Provides-Extra: gh-pages
 
@@ -53,15 +53,15 @@
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/janosh/pymatviz/main.svg)](https://results.pre-commit.ci/latest/github/janosh/pymatviz/main)
 [![This project supports Python 3.8+](https://img.shields.io/badge/Python-3.8+-blue.svg?logo=python&logoColor=white)](https://python.org/downloads)
 [![PyPI](https://img.shields.io/pypi/v/pymatviz?logo=pypi&logoColor=white)](https://pypi.org/project/pymatviz)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/pymatviz?logo=icloud&logoColor=white)](https://pypistats.org/packages/pymatviz)
 
 </h4>
 
-**Note**: This project is not associated with or endorsed by [`pymatgen`](https://github.com/materialsproject/pymatgen), but aims to complement it with additional plotting functionality.
+**Note**: This project is not endorsed by [`pymatgen`](https://github.com/materialsproject/pymatgen), but aims to complement it with additional plotting functionality.
 
 ## Installation
 
 ```sh
 pip install pymatviz
 ```
```

### Comparing `pymatviz-0.6.2/license` & `pymatviz-0.6.3/license`

 * *Files identical despite different names*

### Comparing `pymatviz-0.6.2/pymatviz/correlation.py` & `pymatviz-0.6.3/pymatviz/correlation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,17 @@
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
 import numpy as np
 from matplotlib import pyplot as plt
 
-from pymatviz.utils import Array
+
+if TYPE_CHECKING:
+    from numpy.typing import ArrayLike
 
 
 def marchenko_pastur_pdf(x: float, gamma: float, sigma: float = 1) -> float:
     """Generate Marchenko-Pastur probability distribution which describes the density of
     singular values of large rectangular random matrices.
 
     See https://wikipedia.org/wiki/Marchenko-Pastur_distribution.
@@ -31,29 +37,29 @@
     root = np.sqrt((lambda_p - x) * (x - lambda_m))
     unit_step = x > lambda_p or x < lambda_m
 
     return prefac * root * (0 if unit_step else 1)
 
 
 def marchenko_pastur(
-    matrix: Array,
+    matrix: ArrayLike,
     gamma: float,
     sigma: float = 1,
     filter_high_evals: bool = False,
-    ax: plt.Axes = None,
+    ax: plt.Axes | None = None,
 ) -> plt.Axes:
     """Plot the eigenvalue distribution of a symmetric matrix (usually a correlation
     matrix) against the Marchenko Pastur distribution.
 
     The probability of a random matrix having eigenvalues >= (1 + sqrt(gamma))^2 in the
     absence of any signal is vanishingly small. Thus, if eigenvalues larger than that
     appear, they correspond to statistically significant signals.
 
     Args:
-        matrix (Array): 2d array
+        matrix (ArrayLike): 2d array
         gamma (float): The Marchenko-Pastur ratio of random variables to observation
             count. E.g. for N=1000 variables and p=500 observations of each,
             gamma = p/N = 1/2.
         sigma (float, optional): Standard deviation of random variables. Defaults to 1.
         filter_high_evals (bool, optional): Whether to filter out eigenvalues larger
             than theoretical random maximum. Useful for focusing the plot on the area
             of the MP PDF. Defaults to False.
```

### Comparing `pymatviz-0.6.2/pymatviz/cumulative.py` & `pymatviz-0.6.3/pymatviz/cumulative.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,22 @@
-from typing import Any
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, Any
 
 import matplotlib.pyplot as plt
 import numpy as np
 
-from pymatviz.utils import Array
+
+if TYPE_CHECKING:
+    from numpy.typing import ArrayLike
 
 
-def cumulative_residual(res: Array, ax: plt.Axes = None, **kwargs: Any) -> plt.Axes:
+def cumulative_residual(
+    res: ArrayLike, ax: plt.Axes | None = None, **kwargs: Any
+) -> plt.Axes:
     """Plot the empirical cumulative distribution for the residuals (y - mu).
 
     Args:
         res (array): Residuals between y_true and y_pred, i.e.
             targets - model predictions.
         ax (Axes, optional): matplotlib Axes on which to plot. Defaults to None.
         **kwargs: Additional keyword arguments passed to ax.fill_between().
@@ -51,15 +57,17 @@
 
     # Label the plot
     ax.set(xlabel="Residual", ylabel="Percentile", title="Cumulative Residual")
 
     return ax
 
 
-def cumulative_error(abs_err: Array, ax: plt.Axes = None, **kwargs: Any) -> plt.Axes:
+def cumulative_error(
+    abs_err: ArrayLike, ax: plt.Axes | None = None, **kwargs: Any
+) -> plt.Axes:
     """Plot the empirical cumulative distribution of the absolute errors.
 
     abs(y_true - y_pred).
 
     Args:
         abs_err (array): Absolute error between y_true and y_pred, i.e.
             abs(targets - model predictions).
```

### Comparing `pymatviz-0.6.2/pymatviz/elements.csv` & `pymatviz-0.6.3/pymatviz/elements.csv`

 * *Files identical despite different names*

### Comparing `pymatviz-0.6.2/pymatviz/histograms.py` & `pymatviz-0.6.3/pymatviz/histograms.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,24 +8,26 @@
 import scipy.stats
 from matplotlib import transforms
 from matplotlib.ticker import FixedLocator
 from pymatgen.core import Structure
 from pymatgen.symmetry.groups import SpaceGroup
 
 from pymatviz.ptable import count_elements
-from pymatviz.utils import Array, annotate_bars, df_to_arrays, get_crystal_sys
+from pymatviz.utils import annotate_bars, df_to_arrays, get_crystal_sys
 
 
 if TYPE_CHECKING:
+    from numpy.typing import ArrayLike
+
     from pymatviz.ptable import CountMode, ElemValues
 
 
 def residual_hist(
-    y_res: Array,
-    ax: plt.Axes = None,
+    y_res: ArrayLike,
+    ax: plt.Axes | None = None,
     xlabel: str | None = r"Residual ($y_\mathrm{true} - y_\mathrm{pred}$)",
     **kwargs: Any,
 ) -> plt.Axes:
     r"""Plot the residual distribution overlaid with a Gaussian kernel density estimate.
 
     Adapted from https://github.com/kaaiian/ML_figures (https://git.io/Jmb2O).
 
@@ -57,19 +59,19 @@
     ax.set(xlabel=xlabel)
     ax.legend(loc="upper left", framealpha=0.5, handlelength=1)
 
     return ax
 
 
 def true_pred_hist(
-    y_true: Array | str,
-    y_pred: Array | str,
-    y_std: Array | str,
-    df: pd.DataFrame = None,
-    ax: plt.Axes = None,
+    y_true: ArrayLike | str,
+    y_pred: ArrayLike | str,
+    y_std: ArrayLike | str,
+    df: pd.DataFrame | None = None,
+    ax: plt.Axes | None = None,
     cmap: str = "hot",
     truth_color: str = "blue",
     true_label: str = r"$y_\mathrm{true}$",
     pred_label: str = r"$y_\mathrm{pred}$",
     **kwargs: Any,
 ) -> plt.Axes:
     r"""Plot a histogram of model predictions with bars colored by the mean uncertainty
@@ -134,15 +136,15 @@
 
 
 def spacegroup_hist(
     data: Sequence[int | str | Structure] | pd.Series,
     show_counts: bool = True,
     xticks: Literal["all", "crys_sys_edges"] | int = 20,
     include_missing: bool = False,
-    ax: plt.Axes = None,
+    ax: plt.Axes | None = None,
     **kwargs: Any,
 ) -> plt.Axes:
     """Plot a histogram of spacegroups shaded by crystal system.
 
     Args:
         data (list[int | str | Structure] | pd.Series): Space group strings or numbers
             (from 1 - 230) or pymatgen structures.
@@ -277,18 +279,18 @@
     plt.xticks(rotation=90)
 
     return ax
 
 
 def hist_elemental_prevalence(
     formulas: ElemValues,
-    count_mode: CountMode = "element_composition",
+    count_mode: CountMode = "composition",
     log: bool = False,
-    keep_top: int = None,
-    ax: plt.Axes = None,
+    keep_top: int | None = None,
+    ax: plt.Axes | None = None,
     bar_values: Literal["percent", "count"] | None = "percent",
     h_offset: int = 0,
     v_offset: int = 10,
     rotation: int = 45,
     **kwargs: Any,
 ) -> plt.Axes:
     """Plot a histogram of the prevalence of each element in a materials dataset.
@@ -328,15 +330,15 @@
         ax.set(yscale="log", ylabel="log(Element Count)")
     else:
         ax.set(title="Element Count")
 
     if bar_values is not None:
         if bar_values == "percent":
             sum_elements = non_zero.sum()
-            labels = [f"{el / sum_elements:.1%}" for el in non_zero.values]
+            labels = [f"{el / sum_elements:.1%}" for el in non_zero.to_numpy()]
         else:
             labels = non_zero.astype(int).to_list()
         annotate_bars(
             ax, labels=labels, h_offset=h_offset, v_offset=v_offset, rotation=rotation
         )
 
     return ax
```

### Comparing `pymatviz-0.6.2/pymatviz/parity.py` & `pymatviz-0.6.3/pymatviz/parity.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 from __future__ import annotations
 
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
-import pandas as pd
 import scipy.interpolate
-from matplotlib.gridspec import GridSpec
 
-from pymatviz.utils import Array, annotate_metrics, df_to_arrays, with_hist
+from pymatviz.utils import annotate_metrics, df_to_arrays, with_hist
+
+
+if TYPE_CHECKING:
+    import pandas as pd
+    from matplotlib.gridspec import GridSpec
+    from numpy.typing import ArrayLike
 
 
 def hist_density(
-    x: Array | str,
-    y: Array | str,
-    df: pd.DataFrame = None,
+    x: ArrayLike | str,
+    y: ArrayLike | str,
+    df: pd.DataFrame | None = None,
     sort: bool = True,
     bins: int = 100,
-) -> tuple[Array, Array, Array]:
+) -> tuple[ArrayLike, ArrayLike, ArrayLike]:
     """Return an approximate density of 2d points.
 
     Args:
         x (array | str): x-values or dataframe column name.
         y (array | str): y-values or dataframe column name.
         df (pd.DataFrame, optional): DataFrame with x and y columns. Defaults to None.
         sort (bool, optional): Whether to sort points by density so that densest points
@@ -49,23 +53,23 @@
         idx = zs.argsort()
         x, y, zs = x[idx], y[idx], zs[idx]
 
     return x, y, zs
 
 
 def density_scatter(
-    x: Array | str,
-    y: Array | str,
-    df: pd.DataFrame = None,
-    ax: plt.Axes = None,
+    x: ArrayLike | str,
+    y: ArrayLike | str,
+    df: pd.DataFrame | None = None,
+    ax: plt.Axes | None = None,
     sort: bool = True,
     log_cmap: bool = True,
     density_bins: int = 100,
-    xlabel: str = None,
-    ylabel: str = None,
+    xlabel: str | None = None,
+    ylabel: str | None = None,
     identity: bool = True,
     stats: bool | dict[str, Any] = True,
     **kwargs: Any,
 ) -> plt.Axes:
     """Scatter plot colored (and optionally sorted) by density.
 
     Args:
@@ -86,14 +90,16 @@
             E.g. stats=dict(loc="upper left", prefix="Title", prop=dict(fontsize=16)).
         **kwargs: Additional keyword arguments to pass to ax.scatter(). E.g. cmap to
             change the color map.
 
     Returns:
         ax: The plot's matplotlib Axes.
     """
+    if not isinstance(stats, (bool, dict)):
+        raise TypeError(f"stats must be bool or dict, got {type(stats)} instead.")
     if xlabel is None:
         xlabel = getattr(x, "name", x if isinstance(x, str) else "Actual")
     if ylabel is None:
         ylabel = getattr(y, "name", y if isinstance(y, str) else "Predicted")
 
     x, y = df_to_arrays(df, x, y)
     ax = ax or plt.gca()
@@ -120,23 +126,23 @@
 
     ax.set(xlabel=xlabel, ylabel=ylabel)
 
     return ax
 
 
 def scatter_with_err_bar(
-    x: Array | str,
-    y: Array | str,
-    df: pd.DataFrame = None,
-    xerr: Array = None,
-    yerr: Array = None,
-    ax: plt.Axes = None,
+    x: ArrayLike | str,
+    y: ArrayLike | str,
+    df: pd.DataFrame | None = None,
+    xerr: ArrayLike | None = None,
+    yerr: ArrayLike | None = None,
+    ax: plt.Axes | None = None,
     xlabel: str = "Actual",
     ylabel: str = "Predicted",
-    title: str = None,
+    title: str | None = None,
     **kwargs: Any,
 ) -> plt.Axes:
     """Scatter plot with optional x- and/or y-error bars. Useful when passing model
     uncertainties as yerr=y_std for checking if uncertainty correlates with error, i.e.
     if points farther from the parity line have larger uncertainty.
 
     Args:
@@ -167,19 +173,19 @@
 
     ax.set(xlabel=xlabel, ylabel=ylabel, title=title)
 
     return ax
 
 
 def density_hexbin(
-    x: Array | str,
-    y: Array | str,
-    df: pd.DataFrame = None,
-    ax: plt.Axes = None,
-    weights: Array = None,
+    x: ArrayLike | str,
+    y: ArrayLike | str,
+    df: pd.DataFrame | None = None,
+    ax: plt.Axes | None = None,
+    weights: ArrayLike | None = None,
     xlabel: str = "Actual",
     ylabel: str = "Predicted",
     **kwargs: Any,
 ) -> plt.Axes:
     """Hexagonal-grid scatter plot colored by point density or by density in third
     dimension passed as weights.
 
@@ -215,50 +221,50 @@
 
     ax.set(xlabel=xlabel, ylabel=ylabel)
 
     return ax
 
 
 def density_scatter_with_hist(
-    x: Array | str,
-    y: Array | str,
-    df: pd.DataFrame = None,
-    cell: GridSpec = None,
+    x: ArrayLike | str,
+    y: ArrayLike | str,
+    df: pd.DataFrame | None = None,
+    cell: GridSpec | None = None,
     bins: int = 100,
     **kwargs: Any,
 ) -> plt.Axes:
     """Scatter plot colored (and optionally sorted) by density with histograms along
     each dimension.
     """
     x, y = df_to_arrays(df, x, y)
     ax_scatter = with_hist(x, y, cell, bins)
     return density_scatter(x, y, ax=ax_scatter, **kwargs)
 
 
 def density_hexbin_with_hist(
-    x: Array | str,
-    y: Array | str,
-    df: pd.DataFrame = None,
-    cell: GridSpec = None,
+    x: ArrayLike | str,
+    y: ArrayLike | str,
+    df: pd.DataFrame | None = None,
+    cell: GridSpec | None = None,
     bins: int = 100,
     **kwargs: Any,
 ) -> plt.Axes:
     """Hexagonal-grid scatter plot colored by density or by third dimension passed
     color_by with histograms along each dimension.
     """
     x, y = df_to_arrays(df, x, y)
     ax_scatter = with_hist(x, y, cell, bins)
     return density_hexbin(x, y, ax=ax_scatter, **kwargs)
 
 
 def residual_vs_actual(
-    y_true: Array | str,
-    y_pred: Array | str,
-    df: pd.DataFrame = None,
-    ax: plt.Axes = None,
+    y_true: ArrayLike | str,
+    y_pred: ArrayLike | str,
+    df: pd.DataFrame | None = None,
+    ax: plt.Axes | None = None,
     xlabel: str = r"Actual value",
     ylabel: str = r"Residual ($y_\mathrm{true} - y_\mathrm{pred}$)",
     **kwargs: Any,
 ) -> plt.Axes:
     r"""Plot targets on the x-axis vs residuals (y_err = y_true - y_pred) on the y-axis.
 
     Args:
```

### Comparing `pymatviz-0.6.2/pymatviz/plot_defaults.py` & `pymatviz-0.6.3/pymatviz/plot_defaults.py`

 * *Files identical despite different names*

### Comparing `pymatviz-0.6.2/pymatviz/ptable.py` & `pymatviz-0.6.3/pymatviz/ptable.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,40 +4,38 @@
 from typing import TYPE_CHECKING, Any, Literal, Sequence, get_args
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import plotly.express as px
 import plotly.figure_factory as ff
-import plotly.graph_objects as go
 from matplotlib.cm import get_cmap
 from matplotlib.colors import LogNorm, Normalize
 from matplotlib.patches import Rectangle
 from pandas.api.types import is_numeric_dtype, is_string_dtype
 from pymatgen.core import Composition
 
 from pymatviz.utils import df_ptable
 
 
 if TYPE_CHECKING:
     from typing import TypeAlias
 
+    import plotly.graph_objects as go
+
     ElemValues: TypeAlias = dict[str | int, int | float] | pd.Series | Sequence[str]
 
 CountMode = Literal[
-    "element_composition",
-    "fractional_composition",
-    "reduced_composition",
-    "occurrence",
+    "composition", "fractional_composition", "reduced_composition", "occurrence"
 ]
 
 
 def count_elements(
     elem_values: ElemValues,
-    count_mode: CountMode = "element_composition",
+    count_mode: CountMode = "composition",
     exclude_elements: Sequence[str] = (),
     fill_value: float | None = 0,
 ) -> pd.Series:
     """Count element occurrence in list of formula strings or dict-like compositions.
     If passed elem_values are already a map from element symbol to counts, ensure the
     data is a pd.Series filled with zero values for missing element symbols.
 
@@ -49,25 +47,25 @@
         ptable_heatmap(elem_counts) # fast, only rerun this line to update the plot
 
     Args:
         elem_values (dict[str, int | float] | pd.Series | list[str]): Iterable of
             composition strings/objects or map from element symbols to heatmap values.
         count_mode ('(element|fractional|reduced)_composition'):
             Only used when elem_values is a list of composition strings/objects.
-            - element_composition (default): Count elements in each composition as is,
+            - composition (default): Count elements in each composition as is,
                 i.e. without reduction or normalization.
             - fractional_composition: Convert to normalized compositions in which the
                 amounts of each species sum to before counting.
                 Example: Fe2 O3 -> Fe0.4 O0.6
             - reduced_composition: Convert to reduced compositions (i.e. amounts
                 normalized by greatest common denominator) before counting.
                 Example: Fe4 P4 O16 -> Fe P O4.
             - occurrence: Count the number of times each element occurs in a list of
                 formulas irrespective of compositions. E.g. [Fe2 O3, Fe O, Fe4 P4 O16]
-                counts to {Fe: 3, O: 3, P1}.
+                counts to {Fe: 3, O: 3, P: 1}.
         exclude_elements (Sequence[str]): Elements to exclude from the count. Defaults
             to ().
         fill_value (float | None): Value to fill in for missing elements. Defaults to 0.
 
     Returns:
         pd.Series: Map element symbols to heatmap values.
     """
@@ -83,16 +81,17 @@
         if count_mode == "occurrence":
             srs = pd.Series(
                 itertools.chain.from_iterable(
                     map(str, Composition(comp)) for comp in srs
                 )
             ).value_counts()
         else:
+            attr = "element_composition" if count_mode == "composition" else count_mode
             srs = pd.DataFrame(
-                getattr(Composition(formula), count_mode).as_dict() for formula in srs
+                getattr(Composition(formula), attr).as_dict() for formula in srs
             ).sum()  # sum up element occurrences
     else:
         raise ValueError(
             "Expected elem_values to be map from element symbols to heatmap values or "
             f"list of compositions (strings or Pymatgen objects), got {elem_values}"
         )
 
@@ -132,25 +131,25 @@
 
     return srs
 
 
 def ptable_heatmap(
     elem_values: ElemValues,
     log: bool = False,
-    ax: plt.Axes = None,
-    count_mode: CountMode = "element_composition",
+    ax: plt.Axes | None = None,
+    count_mode: CountMode = "composition",
     cbar_title: str = "Element Count",
     cbar_max: float | int | None = None,
     cmap: str = "summer_r",
     zero_color: str = "#DDD",  # light gray
     infty_color: str = "lightskyblue",
     na_color: str = "white",
     heat_mode: Literal["value", "fraction", "percent"] | None = "value",
-    precision: str = None,
-    cbar_precision: str = None,
+    precision: str | None = None,
+    cbar_precision: str | None = None,
     text_color: str | tuple[str, str] = "auto",
     exclude_elements: Sequence[str] = (),
     zero_symbol: str | float = "-",
 ) -> plt.Axes:
     """Plot a heatmap across the periodic table of elements.
 
     Args:
@@ -320,15 +319,15 @@
     plt.axis("off")
     return ax
 
 
 def ptable_heatmap_ratio(
     elem_values_num: ElemValues,
     elem_values_denom: ElemValues,
-    count_mode: CountMode = "element_composition",
+    count_mode: CountMode = "composition",
     normalize: bool = False,
     cbar_title: str = "Element Ratio",
     not_in_numerator: tuple[str, str] = ("#DDD", "gray: not in 1st list"),
     not_in_denominator: tuple[str, str] = ("lightskyblue", "blue: not in 2nd list"),
     not_in_either: tuple[str, str] = ("white", "white: not in either"),
     **kwargs: Any,
 ) -> plt.Axes:
@@ -385,30 +384,31 @@
         plt.text(0.8, y_pos, txt, fontsize=10, bbox=bbox)
 
     return ax
 
 
 def ptable_heatmap_plotly(
     elem_values: ElemValues,
-    count_mode: CountMode = "element_composition",
+    count_mode: CountMode = "composition",
     colorscale: str | Sequence[str] | Sequence[tuple[float, str]] = "viridis",
     showscale: bool = True,
     heat_mode: Literal["value", "fraction", "percent"] | None = "value",
-    precision: str = None,
+    precision: str | None = None,
     hover_props: Sequence[str] | dict[str, str] | None = None,
     hover_data: dict[str, str | int | float] | pd.Series | None = None,
     font_colors: Sequence[str] = ("#eee", "black"),
     gap: float = 5,
-    font_size: int = None,
-    bg_color: str = None,
-    color_bar: dict[str, Any] = None,
+    font_size: int | None = None,
+    bg_color: str | None = None,
+    color_bar: dict[str, Any] | None = None,
     cscale_range: tuple[float | None, float | None] = (None, None),
     exclude_elements: Sequence[str] = (),
     log: bool = False,
-    fill_value: float | None = 0,
+    fill_value: float | None = None,
+    label_map: dict[str, str] | Literal[False] | None = None,
     **kwargs: Any,
 ) -> go.Figure:
     """Create a Plotly figure with an interactive heatmap of the periodic table.
     Supports hover tooltips with custom data or atomic reference data like
     electronegativity, atomic_radius, etc. See kwargs hover_data and hover_props, resp.
 
     Args:
@@ -462,27 +462,42 @@
             (None, None) meaning the range is automatically determined from the data.
         exclude_elements (list[str]): Elements to exclude from the heatmap. E.g. if
             oxygen overpowers everything, you can do exclude_elements=['O'].
             Defaults to ().
         log (bool): Whether to use a logarithmic color scale. Defaults to False.
             Piece of advice: colorscale='viridis' and log=True go well together.
         fill_value (float | None): Value to fill in for missing elements. Defaults to 0.
+        label_map (dict[str, str] | None): Map heat values (after string formatting)
+            to target strings. Defaults to dict.fromkeys((np.nan, None, "nan"), " ")
+            so as not to display 'nan' for missing values. Set to False to disable.
         **kwargs: Additional keyword arguments passed to
             plotly.figure_factory.create_annotated_heatmap().
 
     Returns:
         Figure: Plotly Figure object.
     """
     if log and heat_mode in ("fraction", "percent"):
         raise ValueError(
             "Combining log color scale and heat_mode='fraction'/'percent' unsupported"
         )
     if len(cscale_range) != 2:
         raise ValueError(f"{cscale_range=} should have length 2")
 
+    if isinstance(colorscale, (str, type(None))):
+        colorscale = px.colors.get_colorscale(colorscale or "Pinkyl")
+    elif isinstance(colorscale, Sequence) and isinstance(
+        colorscale[0], (str, list, tuple)
+    ):
+        pass
+    else:
+        raise ValueError(
+            f"{colorscale = } should be string, list of strings or list of "
+            "tuples(float, str)"
+        )
+
     color_bar = color_bar or {}
     color_bar.setdefault("orientation", "h")
     # if elem_values is a series with a name, use it as the color bar title
     if isinstance(elem_values, pd.Series) and elem_values.name:
         color_bar.setdefault("title", elem_values.name)
 
     elem_values = count_elements(elem_values, count_mode, exclude_elements, fill_value)
@@ -500,15 +515,20 @@
         heat_value_element_map = elem_values / clean_vals.sum()
     else:
         heat_value_element_map = elem_values
 
     n_rows, n_columns = 10, 18
     # initialize tile text and hover tooltips to empty strings
     tile_texts, hover_texts = np.full([2, n_rows, n_columns], "", dtype=object)
-    heatmap_values = np.zeros([n_rows, n_columns])
+    heatmap_values = np.full([n_rows, n_columns], np.nan)
+
+    if label_map is None:
+        # default to space string for None, np.nan and "nan". space is needed
+        # for <br> in tile_text to work so all element symbols are vertically aligned
+        label_map = dict.fromkeys([np.nan, None, "nan"], " ")  # type: ignore
 
     for symbol, period, group, name, *_ in df_ptable.itertuples():
         # build table from bottom up so that period 1 becomes top row
         row = n_rows - period
         col = group - 1
 
         label = None  # label (if not None) is placed below the element symbol
@@ -521,17 +541,18 @@
             else:
                 default_prec = ".1f" if heat_value < 100 else ",.0f"
                 if heat_value > 1e5:
                     default_prec = ".2g"
                 label = f"{heat_value:{precision or default_prec}}".replace("e+0", "e")
 
         style = f"font-weight: bold; font-size: {1.5 * (font_size or 12)};"
-        tile_text = f"<span {style=}>{symbol}</span>"
-        if label is not None:
-            tile_text += f"<br>{label}"
+        tile_text = (
+            f"<span {style=}>{symbol}</span><br>"
+            f"{(label_map or {}).get(label, label)}"  # type: ignore
+        )
 
         tile_texts[row][col] = tile_text
 
         hover_text = name
 
         if hover_data is not None and symbol in hover_data:
             hover_text += f"<br>{hover_data[symbol]}"
@@ -564,55 +585,41 @@
 
         color_val = heat_value_element_map[symbol]
         if log and color_val > 0:
             color_val = np.log10(color_val)
         # until https://github.com/plotly/plotly.js/issues/975 is resolved, we need to
         # insert transparency (rgba0) at low end of colorscale (+1e-6) to not show any
         # colors on empty tiles of the periodic table
-        heatmap_values[row][col] = color_val + 1e-6
-
-    rgba0 = "rgba(0, 0, 0, 0)"
-    if colorscale is None:
-        colorscale = [rgba0] + px.colors.sequential.Pinkyl
-    elif isinstance(colorscale, str):
-        colorscale = [(0, rgba0)] + px.colors.get_colorscale(colorscale)
-        colorscale[1][0] = 1e-6  # type: ignore
-    elif isinstance(colorscale, Sequence) and isinstance(colorscale[0], str):
-        colorscale = [rgba0] + list(colorscale)  # type: ignore
-    elif isinstance(colorscale, Sequence) and isinstance(colorscale[0], (list, tuple)):
-        # list of tuples(float in [0, 1], color)
-        # make sure we're dealing with mutable lists
-        colorscale = [(0, rgba0), *map(list, colorscale)]  # type: ignore
-        colorscale[1][0] = 1e-6  # type: ignore
-    else:
-        raise ValueError(
-            f"{colorscale = } should be string, list of strings or list of "
-            "tuples(float, str)"
-        )
+        heatmap_values[row][col] = color_val
 
     # TODO: see if this ugly code can be handed off to plotly, looks like not atm
     # https://github.com/janosh/pymatviz/issues/52
     # https://github.com/plotly/documentation/issues/1611
     log_cbar = dict(
         tickvals=np.arange(int(np.log10(elem_values.max())) + 1),
         ticktext=10 ** np.arange(int(np.log10(elem_values.max())) + 1),
     )
+    if isinstance(font_colors, str):
+        font_colors = [font_colors]
+    if cscale_range == (None, None):
+        cscale_range = (elem_values.min(), elem_values.max())
+
     fig = ff.create_annotated_heatmap(
         heatmap_values,
         annotation_text=tile_texts,
         text=hover_texts,
         showscale=showscale,
         colorscale=colorscale,
         font_colors=font_colors,
         hoverinfo="text",
         xgap=gap,
         ygap=gap,
         colorbar=log_cbar if log else None,
-        zmax=cscale_range[1],
         zmin=cscale_range[0],
+        zmax=cscale_range[1],
         # https://github.com/plotly/plotly.py/issues/193
         zauto=cscale_range == (None, None),
         **kwargs,
     )
     fig.update_layout(
         margin=dict(l=10, r=10, t=10, b=10, pad=10),
         paper_bgcolor=bg_color,
```

### Comparing `pymatviz-0.6.2/pymatviz/relevance.py` & `pymatviz-0.6.3/pymatviz/relevance.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 from __future__ import annotations
 
+from typing import TYPE_CHECKING
+
 import matplotlib.pyplot as plt
-import pandas as pd
 import sklearn.metrics as skm
 
-from pymatviz.utils import Array, df_to_arrays
+from pymatviz.utils import df_to_arrays
+
+
+if TYPE_CHECKING:
+    import pandas as pd
+    from numpy.typing import ArrayLike
 
 
 def roc_curve(
-    targets: Array | str,
-    proba_pos: Array | str,
-    df: pd.DataFrame = None,
-    ax: plt.Axes = None,
+    targets: ArrayLike | str,
+    proba_pos: ArrayLike | str,
+    df: pd.DataFrame | None = None,
+    ax: plt.Axes | None = None,
 ) -> tuple[float, plt.Axes]:
     """Plot the receiver operating characteristic curve of a binary classifier given
     target labels and predicted probabilities for the positive class.
 
     Args:
         targets (array): Ground truth targets.
         proba_pos (array): predicted probabilities for the positive class.
@@ -39,18 +45,18 @@
     ax.set(xlim=(0, 1.05), ylim=(0, 1.05))
     ax.set(xlabel="False Positive Rate", ylabel="True Positive Rate", title="ROC Curve")
 
     return roc_auc, ax
 
 
 def precision_recall_curve(
-    targets: Array | str,
-    proba_pos: Array | str,
-    df: pd.DataFrame = None,
-    ax: plt.Axes = None,
+    targets: ArrayLike | str,
+    proba_pos: ArrayLike | str,
+    df: pd.DataFrame | None = None,
+    ax: plt.Axes | None = None,
 ) -> tuple[float, plt.Axes]:
     """Plot the precision recall curve of a binary classifier.
 
     Args:
         targets (array): Ground truth targets.
         proba_pos (array): predicted probabilities for the positive class.
         df (pd.DataFrame, optional): DataFrame with targets and proba_pos columns.
```

### Comparing `pymatviz-0.6.2/pymatviz/sankey.py` & `pymatviz-0.6.3/pymatviz/sankey.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from __future__ import annotations
 
-from typing import Any, Literal
+from typing import TYPE_CHECKING, Any, Literal
 
-import pandas as pd
 import plotly.graph_objects as go
 
 
+if TYPE_CHECKING:
+    import pandas as pd
+
+
 def sankey_from_2_df_cols(
     df: pd.DataFrame,
     cols: list[str],
     labels_with_counts: bool | Literal["percent"] = True,
     **kwargs: Any,
 ) -> go.Figure:
     """Plot two columns of a dataframe as a Plotly Sankey diagram.
@@ -30,15 +33,15 @@
     """
     if len(cols) != 2:
         raise ValueError(
             f"{cols=} should specify exactly two columns: (source_col, target_col)"
         )
 
     source, target, value = (
-        df[list(cols)].value_counts().reset_index().values.T.tolist()
+        df[list(cols)].value_counts().reset_index().to_numpy().T.tolist()
     )
 
     if labels_with_counts:
         as_percent = labels_with_counts == "percent"
         source_counts = df[cols[0]].value_counts(normalize=as_percent).to_dict()
         target_counts = df[cols[1]].value_counts(normalize=as_percent).to_dict()
         fmt = ".1%" if as_percent else "d"
@@ -60,9 +63,8 @@
             source=[source.index(x) for x in source],
             target=[len(source) + target.index(x) for x in target],
             value=value,
         ),
         **kwargs,
     )
 
-    fig = go.Figure(data=[sankey])
-    return fig
+    return go.Figure(data=[sankey])
```

### Comparing `pymatviz-0.6.2/pymatviz/structure_viz.py` & `pymatviz-0.6.3/pymatviz/structure_viz.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 from __future__ import annotations
 
 import math
 import warnings
 from itertools import product
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib.patches import PathPatch, Wedge
 from matplotlib.path import Path
 from pymatgen.analysis.local_env import CrystalNN, NearNeighbors
-from pymatgen.core import Structure
 
-from pymatviz.utils import Array, covalent_radii, jmol_colors
+from pymatviz.utils import covalent_radii, jmol_colors
+
+
+if TYPE_CHECKING:
+    from numpy.typing import ArrayLike
+    from pymatgen.core import Structure
 
 
 class ExperimentalWarning(Warning):
     """Used for experimental show_bonds feature."""
 
 
 warnings.simplefilter("once", ExperimentalWarning)
 
 
 # plot_structure_2d() and its helpers get_rot_matrix() and unit_cell_to_lines() were
 # inspired by ASE https://wiki.fysik.dtu.dk/ase/ase/visualize/visualize.html#matplotlib
 
 
-def _angles_to_rotation_matrix(angles: str, rotation: Array = None) -> Array:
+def _angles_to_rotation_matrix(
+    angles: str, rotation: ArrayLike | None = None
+) -> ArrayLike:
     """Convert Euler angles to a rotation matrix.
 
     Note the order of angles matters. 50x,40z != 40z,50x.
 
     Args:
         angles (str): Euler angles (in degrees) formatted as '-10y,50x,120z'
         rotation (np.array, optional): Initial rotation matrix. Use this if you already
@@ -57,15 +63,15 @@
         elif dim == 1:
             rotation = np.dot(rotation, [(cos, 0, -sin), (0, 1, 0), (sin, 0, cos)])
         else:
             rotation = np.dot(rotation, [(cos, sin, 0), (-sin, cos, 0), (0, 0, 1)])
     return rotation
 
 
-def unit_cell_to_lines(cell: Array) -> tuple[Array, Array, Array]:
+def unit_cell_to_lines(cell: ArrayLike) -> tuple[ArrayLike, ArrayLike, ArrayLike]:
     """Convert lattice vectors to plot lines.
 
     Args:
         cell (np.array): Lattice vectors.
 
     Returns:
         tuple[np.array, np.array, np.array]:
@@ -98,24 +104,24 @@
             n1 = n2
 
     return lines, z_indices, unit_cell_lines
 
 
 def plot_structure_2d(
     struct: Structure,
-    ax: plt.Axes = None,
+    ax: plt.Axes | None = None,
     rotation: str = "10x,10y,0z",
     atomic_radii: float | dict[str, float] | None = None,
-    colors: dict[str, str | list[float]] = None,
+    colors: dict[str, str | list[float]] | None = None,
     scale: float = 1,
     show_unit_cell: bool = True,
     show_bonds: bool | NearNeighbors = False,
     site_labels: bool | dict[str, str | float] | list[str | float] = True,
-    label_kwargs: dict[str, Any] = None,
-    bond_kwargs: dict[str, Any] = None,
+    label_kwargs: dict[str, Any] | None = None,
+    bond_kwargs: dict[str, Any] | None = None,
     standardize_struct: bool | None = None,
     axis: bool | str = "off",
 ) -> plt.Axes:
     """Plot pymatgen structure object in 2d. Uses matplotlib.
 
     Inspired by ASE's ase.visualize.plot.plot_atoms()
     https://wiki.fysik.dtu.dk/ase/ase/visualize/visualize.html#matplotlib
@@ -302,15 +308,15 @@
         xy = positions[idx, :2]
         start = 0
         if idx < n_atoms:
             # loop over all species on a site (usually just 1 for ordered sites)
             for elem, occupancy in struct[idx].species.items():
                 # strip oxidation state from element symbol (e.g. Ta5+ to Ta)
                 elem_symbol = elem.symbol
-                radius = atomic_radii[elem_symbol] * scale  # type: ignore
+                radius = atomic_radii[elem_symbol] * scale  # type: ignore[index]
                 face_color = colors[elem_symbol]
                 wedge = Wedge(
                     xy,
                     radius,
                     360 * start,
                     360 * (start + occupancy),
                     facecolor=face_color,
```

### Comparing `pymatviz-0.6.2/pymatviz/sunburst.py` & `pymatviz-0.6.3/pymatviz/sunburst.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from __future__ import annotations
 
-from typing import Any, Literal, Sequence, cast
+from typing import TYPE_CHECKING, Any, Literal, Sequence
 
 import pandas as pd
 import plotly.express as px
-import plotly.graph_objects as go
 from pymatgen.core import Structure
 from pymatgen.symmetry.groups import SpaceGroup
 
 from pymatviz.utils import get_crystal_sys
 
 
+if TYPE_CHECKING:
+    import plotly.graph_objects as go
+
+
 def spacegroup_sunburst(
     data: Sequence[int | str] | pd.Series,
     show_counts: Literal["value", "percent", False] = False,
     **kwargs: Any,
 ) -> go.Figure:
     """Generate a sunburst plot with crystal systems as the inner ring for a list of
     international space group numbers.
@@ -32,17 +35,17 @@
         **kwargs: Additional keyword arguments passed to plotly.express.sunburst.
 
     Returns:
         Figure: The Plotly figure.
     """
     if isinstance(next(iter(data)), Structure):
         # if 1st sequence item is structure, assume all are
-        data = cast(Sequence[Structure], data)
         series = pd.Series(
-            struct.get_space_group_info()[1] for struct in data  # type: ignore
+            struct.get_space_group_info()[1]  # type: ignore[union-attr]
+            for struct in data
         )
     else:
         series = pd.Series(data)
 
     df = pd.DataFrame(series.value_counts().reset_index())
     df.columns = ["spacegroup", "count"]
```

### Comparing `pymatviz-0.6.2/pymatviz/uncertainty.py` & `pymatviz-0.6.3/pymatviz/uncertainty.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 from __future__ import annotations
 
-from typing import Sequence
+from typing import TYPE_CHECKING, Sequence
 
 import matplotlib.pyplot as plt
 import numpy as np
-import pandas as pd
 from scipy.stats import norm
 
-from pymatviz.utils import Array, df_to_arrays
+from pymatviz.utils import df_to_arrays
+
+
+if TYPE_CHECKING:
+    import pandas as pd
+    from numpy.typing import ArrayLike
 
 
 def qq_gaussian(
-    y_true: Array | str,
-    y_pred: Array | str,
-    y_std: Array | dict[str, Array] | str | Sequence[str],
-    df: pd.DataFrame = None,
-    ax: plt.Axes = None,
+    y_true: ArrayLike | str,
+    y_pred: ArrayLike | str,
+    y_std: ArrayLike | dict[str, ArrayLike] | str | Sequence[str],
+    df: pd.DataFrame | None = None,
+    ax: plt.Axes | None = None,
 ) -> plt.Axes:
     """Plot the Gaussian quantile-quantile (Q-Q) plot of one (passed as array) or
     multiple (passed as dict) sets of uncertainty estimates for a single pair of ground
     truth targets `y_true` and model predictions `y_pred`.
 
     Overconfidence relative to a Gaussian distribution is visualized as shaded
     areas below the parity line, underconfidence (oversized uncertainties) as
@@ -104,16 +108,16 @@
             frameon=False,
         )
 
     return ax
 
 
 def get_err_decay(
-    y_true: Array, y_pred: Array, n_rand: int = 100
-) -> tuple[Array, Array]:
+    y_true: ArrayLike, y_pred: ArrayLike, n_rand: int = 100
+) -> tuple[ArrayLike, ArrayLike]:
     """Calculate the model's error curve as samples are excluded from the calculation
     based on their absolute error.
 
     Use in combination with get_std_decay to see what the error drop curve would look
     like if model error and uncertainty were perfectly rank-correlated.
 
     Args:
@@ -139,15 +143,15 @@
         np.random.shuffle(row)  # shuffle rows of ae_tile in place
 
     rand = ae_tile.cumsum(1) / n_inc
 
     return decay_by_err, rand.std(0)
 
 
-def get_std_decay(y_true: Array, y_pred: Array, y_std: Array) -> Array:
+def get_std_decay(y_true: ArrayLike, y_pred: ArrayLike, y_std: ArrayLike) -> ArrayLike:
     """Calculate the drop in model error as samples are excluded from the calculation
     based on the model's uncertainty.
 
     For model's able to estimate their own uncertainty well, meaning predictions of
     larger error are associated with larger uncertainty, the error curve should fall
     off sharply at first as the highest-error points are discarded and slowly towards
     the end where only small-error samples with little uncertainty remain.
@@ -174,35 +178,35 @@
     y_std_sort = np.argsort(y_std)
 
     # increasing count of the number of samples in each element of cumsum()
     n_inc = range(1, len(abs_err) + 1)
 
     decay_by_std = abs_err[y_std_sort].cumsum() / n_inc
 
-    return decay_by_std
+    return decay_by_std  # noqa: RET504
 
 
 def error_decay_with_uncert(
-    y_true: Array | str,
-    y_pred: Array | str,
-    y_std: Array | dict[str, Array] | str | Sequence[str],
-    df: pd.DataFrame = None,
+    y_true: ArrayLike | str,
+    y_pred: ArrayLike | str,
+    y_std: ArrayLike | dict[str, ArrayLike] | str | Sequence[str],
+    df: pd.DataFrame | None = None,
     n_rand: int = 100,
     percentiles: bool = True,
-    ax: plt.Axes = None,
+    ax: plt.Axes | None = None,
 ) -> plt.Axes:
     """Plot for assessing the quality of uncertainty estimates. If a model's uncertainty
     is well calibrated, i.e. strongly correlated with its error, removing the most
     uncertain predictions should make the mean error decay similarly to how it decays
     when removing the predictions of largest error.
 
     Args:
         y_true (array | str): Ground truth regression targets.
         y_pred (array | str): Model predictions.
-        y_std (array | dict[str, Array] | str | list[str]): Model uncertainties.
+        y_std (array | dict[str, ArrayLike] | str | list[str]): Model uncertainties.
             Can be single or multiple uncertainties (e.g. aleatoric/epistemic/total
             uncertainty) as dict.
         n_rand (int, optional): Number of shuffles from which to compute std.dev.
             of error decay by random ordering. Defaults to 100.
         df (pd.DataFrame, optional): DataFrame with y_true, y_pred and y_std columns.
         percentiles (bool, optional): Whether the x-axis shows percentiles or number
             of remaining samples in the MAE calculation. Defaults to True.
```

### Comparing `pymatviz-0.6.2/pymatviz/utils.py` & `pymatviz-0.6.3/pymatviz/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 from __future__ import annotations
 
 import ast
+import os
 import subprocess
 from os.path import dirname
 from shutil import which
-from typing import Any, Literal, Sequence, Union
+from time import sleep
+from typing import TYPE_CHECKING, Any, Literal, Sequence
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import plotly.graph_objects as go
 import sklearn
-from matplotlib.gridspec import GridSpec
 from matplotlib.offsetbox import AnchoredText
-from numpy.typing import NDArray
 from sklearn.metrics import mean_absolute_percentage_error as mape
 from sklearn.metrics import r2_score
 
 
+if TYPE_CHECKING:
+    from matplotlib.gridspec import GridSpec
+    from numpy.typing import ArrayLike
+
 ROOT = dirname(dirname(__file__))
 
-Array = NDArray[Union[np.float64, np.int_]]
 
 df_ptable = pd.read_csv(f"{ROOT}/pymatviz/elements.csv", comment="#").set_index(
     "symbol"
 )
 
 # http://jmol.sourceforge.net/jscolors
 jmol_colors = df_ptable.jmol_color.dropna().map(ast.literal_eval)
@@ -39,17 +42,17 @@
 
 for Z, symbol in enumerate(df_ptable.index, 1):
     atomic_numbers[symbol] = Z
     element_symbols[Z] = symbol
 
 
 def with_hist(
-    xs: NDArray[np.float64 | np.int_],
-    ys: NDArray[np.float64 | np.int_],
-    cell: GridSpec = None,
+    xs: ArrayLike,
+    ys: ArrayLike,
+    cell: GridSpec | None = None,
     bins: int = 100,
 ) -> plt.Axes:
     """Call before creating a plot and use the returned `ax_main` for all
     subsequent plotting ops to create a grid of plots with the main plot in the
     lower left and narrow histograms along its x- and/or y-axes displayed above
     and near the right edge.
 
@@ -81,18 +84,18 @@
     ax_histy.hist(ys, bins=bins, rwidth=0.8, orientation="horizontal")
     ax_histy.axis("off")
 
     return ax_main
 
 
 def annotate_bars(
-    ax: plt.Axes = None,
+    ax: plt.Axes | None = None,
     v_offset: int | float = 10,
     h_offset: int | float = 0,
-    labels: Sequence[str | int | float] = None,
+    labels: Sequence[str | int | float] | None = None,
     fontsize: int = 14,
     y_max_headroom: float = 1.2,
     **kwargs: Any,
 ) -> None:
     """Annotate each bar in bar plot with a label.
 
     Args:
@@ -131,18 +134,18 @@
         ax.annotate(txt, (x_pos, y_pos), ha="center", fontsize=fontsize, **kwargs)
 
     # ensure enough vertical space to display label above highest bar
     ax.set(ylim=(None, y_max * y_max_headroom))
 
 
 def annotate_metrics(
-    xs: NDArray[np.float64 | np.int_],
-    ys: NDArray[np.float64 | np.int_],
-    ax: plt.Axes = None,
-    metrics: dict[str, float] | Sequence[str] = ("MAE", "R2"),
+    xs: ArrayLike,
+    ys: ArrayLike,
+    ax: plt.Axes | None = None,
+    metrics: dict[str, float] | Sequence[str] = ("MAE", "$R^2$"),
     prefix: str = "",
     suffix: str = "",
     prec: int = 3,
     **kwargs: Any,
 ) -> AnchoredText:
     """Provide a set of x and y values of equal length and an optional Axes
     object on which to print the values' mean absolute error and R^2
@@ -166,20 +169,25 @@
         **kwargs: Additional arguments (rotation, arrowprops, frameon, loc, etc.) are
             passed to matplotlib.offsetbox.AnchoredText. Sets default loc="lower right"
             and frameon=False.
 
     Returns:
         AnchoredText: Instance containing the metrics.
     """
+    if isinstance(metrics, str):
+        metrics = [metrics]
+    if not isinstance(metrics, (dict, list, tuple, set)):
+        raise TypeError(f"metrics must be dict|list|tuple|set, not {type(metrics)}")
     funcs = {
         "MAE": lambda x, y: np.abs(x - y).mean(),
         "RMSE": lambda x, y: (((x - y) ** 2).mean()) ** 0.5,
         "MSE": lambda x, y: ((x - y) ** 2).mean(),
         "MAPE": mape,
         "R2": r2_score,
+        "$R^2$": r2_score,
         # TODO: check this for correctness
         "R2_adj": lambda x, y: 1 - (1 - r2_score(x, y)) * (len(x) - 1) / (len(x) - 2),
     }
     for key in set(metrics) - set(funcs):
         func = getattr(sklearn.metrics, key, None)
         if func:
             funcs[key] = func
@@ -236,15 +244,15 @@
         return "trigonal"
     if spg < 195:
         return "hexagonal"
     return "cubic"
 
 
 def add_identity_line(
-    fig: go.Figure, line_kwds: dict[str, Any] = None, trace_idx: int = 0
+    fig: go.Figure, line_kwds: dict[str, Any] | None = None, trace_idx: int = 0
 ) -> go.Figure:
     """Add a line shape to the background layer of a plotly figure spanning
     from smallest to largest x/y values in the trace specified by trace_idx.
 
     Args:
         fig (Figure): Plotly figure.
         line_kwds (dict[str, Any], optional): Keyword arguments for customizing the line
@@ -284,42 +292,53 @@
 
     return fig
 
 
 def save_fig(
     fig: go.Figure | plt.Figure | plt.Axes,
     path: str,
-    plotly_config: dict[str, Any] = None,
+    plotly_config: dict[str, Any] | None = None,
+    env_disable: Sequence[str] = ("CI",),
+    pdf_sleep: float = 0.6,
     **kwargs: Any,
 ) -> None:
     """Write a plotly figure to an HTML file. If the file is has .svelte
     extension, insert `{...$$props}` into the figure's top-level div so it can
     be styled by consuming Svelte code.
 
     Args:
         fig (go.Figure | plt.Figure | plt.Axes): Plotly or matplotlib Figure or
             matplotlib Axes object.
         path (str): Path to HTML file that will be created.
         plotly_config (dict, optional): Configuration options for fig.write_html().
         Defaults to dict(showTips=False, responsive=True, modeBarButtonsToRemove=
         ["lasso2d", "select2d", "autoScale2d", "toImage"]).
         See https://plotly.com/python/configuration-options.
+        env_disable (list[str], optional): Do nothing if any of these environment
+            variables are set. Defaults to ("CI",).
+        pdf_sleep (float, optional): Minimum time in seconds to wait before
+            writing a PDF file. Workaround for this plotly issue
+            https://github.com/plotly/plotly.py/issues/3469. Defaults to 0.6. Has no
+            effect on matplotlib figures.
 
         **kwargs: Keyword arguments passed to fig.write_html().
     """
+    if any(var in os.environ for var in env_disable):
+        return
     # handle matplotlib figures
     if isinstance(fig, (plt.Figure, plt.Axes)):
         if hasattr(fig, "figure"):
             fig = fig.figure  # unwrap Axes
         fig.savefig(path, **kwargs)
         return
     if not isinstance(fig, go.Figure):
         raise TypeError(
             f"Unsupported figure type {type(fig)}, expected plotly or matplotlib Figure"
         )
+    is_pdf = path.lower().endswith((".pdf", ".pdfa"))
     if path.lower().endswith((".svelte", ".html")):
         config = dict(
             showTips=False,
             modeBarButtonsToRemove=[
                 "lasso2d",
                 "select2d",
                 "autoScale2d",
@@ -339,25 +358,30 @@
             # insert {...$$props} into top-level div to be able to post-process and
             # style plotly figures from within Svelte files
             with open(path) as file:
                 text = file.read().replace("<div>", "<div {...$$props}>", 1)
             with open(path, "w") as file:
                 file.write(text + "\n")
     else:
-        if path.lower().endswith(".pdf"):
+        if is_pdf:
             orig_template = fig.layout.template
             fig.layout.template = "plotly_white"
         # hide click-to-show traces in PDF
         hidden_traces = []
         for trace in fig.data:
             if trace.visible == "legendonly":
                 trace.visible = False
                 hidden_traces.append(trace)
         fig.write_image(path, **kwargs)
-        if path.lower().endswith(".pdf"):
+        if is_pdf:
+            # write PDFs twice to get rid of "Loading [MathJax]/extensions/MathMenu.js"
+            # see https://github.com/plotly/plotly.py/issues/3469#issuecomment-994907721
+            sleep(pdf_sleep)
+            fig.write_image(path, **kwargs)
+
             fig.layout.template = orig_template
         for trace in hidden_traces:
             trace.visible = "legendonly"
 
 
 def save_and_compress_svg(
     fig: go.Figure | plt.Figure | plt.Axes, filename: str
@@ -384,37 +408,42 @@
 
     if (svgo := which("svgo")) is not None:
         subprocess.run([svgo, "--multipass", filepath])
 
 
 def df_to_arrays(
     df: pd.DataFrame | None,
-    *args: str | Sequence[str] | NDArray[np.float64 | np.int_],
-) -> list[NDArray[np.float64 | np.int_] | dict[str, NDArray[np.float64 | np.int_]]]:
+    *args: str | Sequence[str] | ArrayLike,
+    strict: bool = True,
+) -> list[ArrayLike | dict[str, ArrayLike]]:
     """If df is None, this is a no-op: args are returned as-is. If df is a
     dataframe, all following args are used as column names and the column data
     returned as arrays (after dropping rows with NaNs in any column).
 
     Args:
         df (pd.DataFrame | None): Optional pandas DataFrame.
-        *args (list[Array | str]): Arbitrary number of arrays or column names in df.
+        *args (list[ArrayLike | str]): Arbitrary number of arrays or column names in df.
+        strict (bool, optional): If True, raise TypeError if df is not pd.DataFrame
+            or None. If False, return args as-is. Defaults to True.
 
     Raises:
         ValueError: If df is not None and any of the args is not a df column name.
         TypeError: If df is not pd.DataFrame and not None.
 
     Returns:
-        tuple[Array, Array]: Input arrays or arrays from dataframe columns.
+        tuple[ArrayLike, ArrayLike]: Input arrays or arrays from dataframe columns.
     """
     if df is None:
         if cols := [arg for arg in args if isinstance(arg, str)]:
             raise ValueError(f"got column names but no df to get data from: {cols}")
         return args  # type: ignore[return-value]
 
     if not isinstance(df, pd.DataFrame):
+        if not strict:
+            return args  # type: ignore[return-value]
         raise TypeError(f"df should be pandas DataFrame or None, got {type(df)}")
 
     if arrays := [arg for arg in args if isinstance(arg, np.ndarray)]:
         raise ValueError(
             "don't pass dataframe and arrays to df_to_arrays(), should be either or, "
             f"got {arrays}"
         )
@@ -428,17 +457,17 @@
             flat_args.append(col_name)
         else:
             flat_args.extend(col_name)
 
     df_no_nan = df.dropna(subset=flat_args)
     for idx, col_name in enumerate(args):
         if isinstance(col_name, (str, int)):
-            args[idx] = df_no_nan[col_name].values  # type: ignore[index]
+            args[idx] = df_no_nan[col_name].to_numpy()  # type: ignore[index]
         else:
-            col_data = df_no_nan[[*col_name]].values.T
+            col_data = df_no_nan[[*col_name]].to_numpy().T
             args[idx] = dict(zip(col_name, col_data))  # type: ignore[index]
 
     return args  # type: ignore[return-value]
 
 
 def bin_df_cols(
     df: pd.DataFrame,
```

### Comparing `pymatviz-0.6.2/pymatviz.egg-info/PKG-INFO` & `pymatviz-0.6.3/pymatviz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymatviz
-Version: 0.6.2
+Version: 0.6.3
 Summary: A toolkit for visualizations in materials informatics
 Author-email: Janosh Riebesell <janosh.riebesell@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Janosh Riebesell
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,20 +22,20 @@
         fitness for a particular purpose and noninfringement. In no event shall the
         authors or copyright holders be liable for any claim, damages or other
         liability, whether in an action of contract, tort or otherwise, arising from,
         out of or in connection with the software or the use or other dealings in the
         software.
         
 Project-URL: Homepage, https://github.com/janosh/pymatviz
-Keywords: science,materials informatics,materials discovery,chemistry,data visualization,plotly,matplotlib
-Classifier: Programming Language :: Python :: 3
+Keywords: chemistry,data visualization,materials discovery,materials informatics,matplotlib,plotly,science
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: data-src
 Provides-Extra: export-figs
 Provides-Extra: gh-pages
 
@@ -53,15 +53,15 @@
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/janosh/pymatviz/main.svg)](https://results.pre-commit.ci/latest/github/janosh/pymatviz/main)
 [![This project supports Python 3.8+](https://img.shields.io/badge/Python-3.8+-blue.svg?logo=python&logoColor=white)](https://python.org/downloads)
 [![PyPI](https://img.shields.io/pypi/v/pymatviz?logo=pypi&logoColor=white)](https://pypi.org/project/pymatviz)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/pymatviz?logo=icloud&logoColor=white)](https://pypistats.org/packages/pymatviz)
 
 </h4>
 
-**Note**: This project is not associated with or endorsed by [`pymatgen`](https://github.com/materialsproject/pymatgen), but aims to complement it with additional plotting functionality.
+**Note**: This project is not endorsed by [`pymatgen`](https://github.com/materialsproject/pymatgen), but aims to complement it with additional plotting functionality.
 
 ## Installation
 
 ```sh
 pip install pymatviz
 ```
```

### Comparing `pymatviz-0.6.2/pymatviz.egg-info/SOURCES.txt` & `pymatviz-0.6.3/pymatviz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymatviz-0.6.2/pyproject.toml` & `pymatviz-0.6.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pymatviz"
-version = "0.6.2"
+version = "0.6.3"
 description = "A toolkit for visualizations in materials informatics"
 authors = [{ name = "Janosh Riebesell", email = "janosh.riebesell@gmail.com" }]
 readme = "readme.md"
 license = { file = "license" }
 keywords = [
-    "science",
-    "materials informatics",
-    "materials discovery",
     "chemistry",
     "data visualization",
-    "plotly",
+    "materials discovery",
+    "materials informatics",
     "matplotlib",
+    "plotly",
+    "science",
 ]
 classifiers = [
-    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
-    "License :: OSI Approved :: MIT License",
 ]
 urls = { Homepage = "https://github.com/janosh/pymatviz" }
 requires-python = ">=3.8"
 dependencies = [
     "matplotlib >= 3.6.2",
     "numpy >= 1.21.0",
     "pandas",
     "plotly",
     "pymatgen",
     "scikit-learn",
     "scipy",
 ]
 
 [project.optional-dependencies]
-test = ["pytest", "pytest-cov", "kaleido"]
+test = ["kaleido", "pytest", "pytest-cov"]
 data-src = ["matminer"]
 export-figs = ["kaleido"]
-gh-pages = ["lazydocs", "jupyter", "nbconvert"]
+gh-pages = ["jupyter", "lazydocs", "nbconvert"]
 
 [tool.setuptools.packages]
 find = { include = ["pymatviz*"], exclude = ["tests*"] }
 
 [tool.setuptools.package-data]
 pymatviz = ["*.csv"]
 
@@ -64,39 +64,60 @@
 warn_redundant_casts = true
 warn_unused_ignores = true
 show_error_codes = true
 no_implicit_optional = false
 
 [tool.ruff]
 target-version = "py38"
+include = ["**/pyproject.toml", "*.ipynb", "*.py", "*.pyi"]
 select = [
-    "B",   # flake8-bugbear
-    "D",   # pydocstyle
-    "E",   # pycodestyle
-    "F",   # pyflakes
-    "I",   # isort
-    "PLE", # pylint error
-    "PLW", # pylint warning
-    "PYI", # flakes8-pyi
-    "Q",   # flake8-quotes
-    "SIM", # flake8-simplify
-    "TID", # tidy imports
-    "UP",  # pyupgrade
-    "W",   # pycodestyle
-    "YTT", # flake8-2020
+    "B",    # flake8-bugbear
+    "C4",   # flake8-comprehensions
+    "D",    # pydocstyle
+    "E",    # pycodestyle error
+    "EXE",  # flake8-executable
+    "F",    # pyflakes
+    "FA",   # flake8-future-annotations
+    "FLY",  # flynt
+    "I",    # isort
+    "ICN",  # flake8-import-conventions
+    "ISC",  # flake8-implicit-str-concat
+    "PD",   # pandas-vet
+    "PERF", # perflint
+    "PIE",  # flake8-pie
+    "PL",   # pylint
+    "PT",   # flake8-pytest-style
+    "PYI",  # flakes8-pyi
+    "Q",    # flake8-quotes
+    "RET",  # flake8-return
+    "RSE",  # flake8-raise
+    "RUF",  # Ruff-specific rules
+    "SIM",  # flake8-simplify
+    "SLOT", # flake8-slots
+    "TCH",  # flake8-type-checking
+    "TID",  # tidy imports
+    "UP",   # pyupgrade
+    "W",    # pycodestyle warning
+    "YTT",  # flake8-2020
 ]
 ignore = [
     "B028",    # No explicit stacklevel keyword argument found
+    "C408",    # unnecessary-collection-call
     "D100",    # Missing docstring in public module
-    "D104",    # Missing docstring in public package
     "D205",    # 1 blank line required between summary line and description
-    "SIM105",  # Use contextlib.suppress(FileNotFoundError) instead of try-except-pass
-    "SIM115",  # Use context handler for opening files
+    "N806",    # non-lowercase-variable-in-function
+    "PD901",   # pandas-df-variable-name
+    "PLR",     # pylint refactor
     "PLW2901", # Outer for loop variable overwritten by inner assignment target
+    "PT006",   # pytest-parametrize-names-wrong-type
+    "PT011",   # pytest-raises-too-broad
+    "RUF001",  # ambiguous-unicode-character-string
+    "SIM105",  # Use contextlib.suppress(FileNotFoundError) instead of try-except-pass
 ]
 pydocstyle.convention = "google"
 isort.lines-after-imports = 2
 isort.split-on-trailing-comma = false
 
 [tool.ruff.per-file-ignores]
+"__init__.py" = ["F401"]
 "tests/*" = ["D103"]
-"examples/*" = ["E402"] # E402 Module level import not at top of file
+"examples/*" = ["E402"]  # E402 Module level import not at top of file
```

### Comparing `pymatviz-0.6.2/readme.md` & `pymatviz-0.6.3/readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/janosh/pymatviz/main.svg)](https://results.pre-commit.ci/latest/github/janosh/pymatviz/main)
 [![This project supports Python 3.8+](https://img.shields.io/badge/Python-3.8+-blue.svg?logo=python&logoColor=white)](https://python.org/downloads)
 [![PyPI](https://img.shields.io/pypi/v/pymatviz?logo=pypi&logoColor=white)](https://pypi.org/project/pymatviz)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/pymatviz?logo=icloud&logoColor=white)](https://pypistats.org/packages/pymatviz)
 
 </h4>
 
-**Note**: This project is not associated with or endorsed by [`pymatgen`](https://github.com/materialsproject/pymatgen), but aims to complement it with additional plotting functionality.
+**Note**: This project is not endorsed by [`pymatgen`](https://github.com/materialsproject/pymatgen), but aims to complement it with additional plotting functionality.
 
 ## Installation
 
 ```sh
 pip install pymatviz
 ```
```

### Comparing `pymatviz-0.6.2/tests/test_cumulative.py` & `pymatviz-0.6.3/tests/test_cumulative.py`

 * *Files identical despite different names*

### Comparing `pymatviz-0.6.2/tests/test_histograms.py` & `pymatviz-0.6.3/tests/test_histograms.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from __future__ import annotations
 
-from typing import Literal
+from typing import TYPE_CHECKING, Literal
 
 import matplotlib.pyplot as plt
-import pandas as pd
 import pytest
-from pymatgen.core import Structure
 
 from pymatviz import residual_hist, spacegroup_hist, true_pred_hist
-from pymatviz.utils import Array
 from tests.conftest import df, y_pred, y_true
 
 
+if TYPE_CHECKING:
+    import pandas as pd
+    from numpy.typing import ArrayLike
+    from pymatgen.core import Structure
+
+
 y_std_mock = y_true - y_pred
 
 
 @pytest.mark.parametrize("bins", [None, 1, 100])
 @pytest.mark.parametrize("xlabel", [None, "foo"])
 def test_residual_hist(bins: int | None, xlabel: str | None) -> None:
     ax = residual_hist(y_true - y_pred, bins=bins, xlabel=xlabel)
@@ -30,21 +33,21 @@
     assert legend._get_loc() == 2  # 2 meaning 'upper left'
 
 
 @pytest.mark.parametrize("bins", [None, 1, 100])
 @pytest.mark.parametrize("cmap", ["hot", "Blues"])
 @pytest.mark.parametrize(
     "df, y_true, y_pred, y_std",
-    [[None, y_true, y_pred, y_std_mock], [df, *df.columns[:2], df.columns[0]]],
+    [(None, y_true, y_pred, y_std_mock), (df, *df.columns[:2], df.columns[0])],
 )
 def test_true_pred_hist(
     df: pd.DataFrame | None,
-    y_true: Array | str,
-    y_pred: Array | str,
-    y_std: Array | dict[str, Array] | str | list[str],
+    y_true: ArrayLike | str,
+    y_pred: ArrayLike | str,
+    y_std: ArrayLike | dict[str, ArrayLike] | str | list[str],
     bins: int | None,
     cmap: str,
 ) -> None:
     ax = true_pred_hist(y_true, y_pred, y_std, df, bins=bins, cmap=cmap)
     assert isinstance(ax, plt.Axes)
```

### Comparing `pymatviz-0.6.2/tests/test_parity.py` & `pymatviz-0.6.3/tests/test_parity.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,90 +1,102 @@
 from __future__ import annotations
 
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import pytest
 
 from pymatviz import (
     density_hexbin,
     density_hexbin_with_hist,
     density_scatter,
     density_scatter_with_hist,
     residual_vs_actual,
     scatter_with_err_bar,
 )
-from pymatviz.utils import Array
 from tests.conftest import df_x_y
 
 
+if TYPE_CHECKING:
+    from numpy.typing import ArrayLike
+
+
 @pytest.mark.parametrize("log_cmap", [True, False])
 @pytest.mark.parametrize("sort", [True, False])
 @pytest.mark.parametrize("cmap", [None, "Greens"])
 @pytest.mark.parametrize(
     "stats",
     [False, True, dict(prefix="test", loc="lower right", prop=dict(fontsize=10))],
 )
 @pytest.mark.parametrize("df, x, y", df_x_y)
 def test_density_scatter(
     df: pd.DataFrame | None,
-    x: Array | str,
-    y: str | Array,
+    x: ArrayLike | str,
+    y: str | ArrayLike,
     log_cmap: bool,
     sort: bool,
     cmap: str | None,
     stats: bool | dict[str, Any],
 ) -> None:
     ax = density_scatter(
         df=df, x=x, y=y, log_cmap=log_cmap, sort=sort, cmap=cmap, stats=stats
     )
     assert isinstance(ax, plt.Axes)
     assert ax.get_xlabel() == x if isinstance(x, str) else "Actual"
     assert ax.get_ylabel() == y if isinstance(y, str) else "Predicted"
 
 
+@pytest.mark.parametrize("stats", [1, (1,), "foo"])
+def test_density_scatter_raises_on_bad_stats_type(stats: Any) -> None:
+    match = f"stats must be bool or dict, got {type(stats)} instead."
+
+    vals = [1, 2, 3]
+    with pytest.raises(TypeError, match=match):
+        density_scatter(x=vals, y=vals, stats=stats)
+
+
 def test_density_scatter_uses_series_name_as_label() -> None:
     x = pd.Series(np.random.rand(5), name="x")
     y = pd.Series(np.random.rand(5), name="y")
     ax = density_scatter(x=x, y=y)
 
     assert ax.get_xlabel() == "x"
     assert ax.get_ylabel() == "y"
 
 
 @pytest.mark.parametrize("df, x, y", df_x_y)
 def test_density_scatter_with_hist(
-    df: pd.DataFrame | None, x: str | Array, y: str | Array
+    df: pd.DataFrame | None, x: str | ArrayLike, y: str | ArrayLike
 ) -> None:
     density_scatter_with_hist(df=df, x=x, y=y)
 
 
 @pytest.mark.parametrize("df, x, y", df_x_y)
 def test_density_hexbin(
-    df: pd.DataFrame | None, x: str | Array, y: str | Array
+    df: pd.DataFrame | None, x: str | ArrayLike, y: str | ArrayLike
 ) -> None:
     density_hexbin(df=df, x=x, y=y)
 
 
 @pytest.mark.parametrize("df, x, y", df_x_y)
 def test_density_hexbin_with_hist(
-    df: pd.DataFrame | None, x: str | Array, y: str | Array
+    df: pd.DataFrame | None, x: str | ArrayLike, y: str | ArrayLike
 ) -> None:
     density_hexbin_with_hist(df=df, x=x, y=y)
 
 
 @pytest.mark.parametrize("df, x, y", df_x_y)
 def test_scatter_with_err_bar(
-    df: pd.DataFrame | None, x: str | Array, y: str | Array
+    df: pd.DataFrame | None, x: str | ArrayLike, y: str | ArrayLike
 ) -> None:
     err = abs(df[x] - df[y]) if df is not None else abs(x - y)  # type: ignore[operator]
     scatter_with_err_bar(df=df, x=x, y=y, yerr=err)
     scatter_with_err_bar(df=df, x=x, y=y, xerr=err)
 
 
 @pytest.mark.parametrize("df, x, y", df_x_y)
 def test_residual_vs_actual(
-    df: pd.DataFrame | None, x: str | Array, y: str | Array
+    df: pd.DataFrame | None, x: str | ArrayLike, y: str | ArrayLike
 ) -> None:
     residual_vs_actual(df=df, y_true=x, y_pred=y)
```

### Comparing `pymatviz-0.6.2/tests/test_ptable.py` & `pymatviz-0.6.3/tests/test_ptable.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,53 +1,55 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Literal, Sequence
 
 import matplotlib.pyplot as plt
+import numpy as np
 import pandas as pd
 import plotly.graph_objects as go
 import pytest
 from plotly.exceptions import PlotlyError
-from pymatgen.core import Composition
 
 from pymatviz import (
     count_elements,
     hist_elemental_prevalence,
     ptable_heatmap,
     ptable_heatmap_plotly,
     ptable_heatmap_ratio,
 )
 from pymatviz.utils import df_ptable
 
 
 if TYPE_CHECKING:
+    from pymatgen.core import Composition
+
     from pymatviz.ptable import CountMode
 
 
-@pytest.fixture
+@pytest.fixture()
 def glass_formulas() -> list[str]:
     """First 20 materials in the Matbench glass dataset.
 
     from matminer.datasets import load_dataset
 
     load_dataset("matbench_glass").composition.head(20)
     """
     return (
         "Al Al(NiB)2 Al10Co21B19 Al10Co23B17 Al10Co27B13 Al10Co29B11 Al10Co31B9 "
         "Al10Co33B7 Al10Cr3Si7 Al10Fe23B17 Al10Fe27B13 Al10Fe31B9 Al10Fe33B7 "
         "Al10Ni23B17 Al10Ni27B13 Al10Ni29B11 Al10Ni31B9 Al10Ni33B7 Al11(CrSi2)3"
     ).split()
 
 
-@pytest.fixture
+@pytest.fixture()
 def glass_elem_counts(glass_formulas: pd.Series[Composition]) -> pd.Series[int]:
     return count_elements(glass_formulas)
 
 
-@pytest.fixture
+@pytest.fixture()
 def steel_formulas() -> list[str]:
     """Unusually fractional compositions, good for testing edge cases.
 
     Output of:
     from matminer.datasets import load_dataset
 
     load_dataset("matbench_steels").composition.head(2)
@@ -56,23 +58,23 @@
         "Fe0.620C0.000953Mn0.000521Si0.00102Cr0.000110Ni0.192Mo0.0176V0.000112"
         "Nb0.0000616Co0.146Al0.00318Ti0.0185",
         "Fe0.623C0.00854Mn0.000104Si0.000203Cr0.147Ni0.0000971Mo0.0179V0.00515"
         "N0.00163Nb0.0000614Co0.188W0.00729Al0.000845",
     ]
 
 
-@pytest.fixture
+@pytest.fixture()
 def steel_elem_counts(steel_formulas: pd.Series[Composition]) -> pd.Series[int]:
     return count_elements(steel_formulas)
 
 
 @pytest.mark.parametrize(
     "count_mode, counts",
     [
-        ("element_composition", {"Fe": 22, "O": 63, "P": 12}),
+        ("composition", {"Fe": 22, "O": 63, "P": 12}),
         ("fractional_composition", {"Fe": 2.5, "O": 5, "P": 0.5}),
         ("reduced_composition", {"Fe": 13, "O": 27, "P": 3}),
         ("occurrence", {"Fe": 8, "O": 8, "P": 3}),
     ],
 )
 def test_count_elements(count_mode: CountMode, counts: dict[str, float]) -> None:
     series = count_elements(["Fe2 O3"] * 5 + ["Fe4 P4 O16"] * 3, count_mode=count_mode)
@@ -272,19 +274,48 @@
 )
 def test_ptable_heatmap_plotly_cscale_range(
     cscale_range: tuple[float | None, float | None]
 ) -> None:
     fig = ptable_heatmap_plotly(df_ptable.density, cscale_range=cscale_range)
     trace = fig.data[0]
     assert "colorbar" in trace
-    # check that color bar range is correct
-    assert trace["zmin"] == cscale_range[0]
-    assert trace["zmax"] == cscale_range[1]
+    # check for correct color bar range
+    if cscale_range == (None, None):
+        # if both None, range is dynamic based on plotted data
+        assert trace["zmin"] == pytest.approx(df_ptable.density.min())
+        assert trace["zmax"] == pytest.approx(df_ptable.density.max())
+    else:
+        assert cscale_range == (trace["zmin"], trace["zmax"])
 
 
 def test_ptable_heatmap_plotly_cscale_range_raises() -> None:
     cscale_range = (0, 10, 20)
-    with pytest.raises(ValueError) as excinfo:
+    with pytest.raises(ValueError) as exc:
         ptable_heatmap_plotly(
             df_ptable.density, cscale_range=cscale_range  # type: ignore[arg-type]
         )
-    assert f"{cscale_range=} should have length 2" in str(excinfo.value)
+    assert f"{cscale_range=} should have length 2" in str(exc.value)
+
+
+@pytest.mark.parametrize(
+    "label_map",
+    [None, False, {"1.0": "one", "2.0": "two", "3.0": "three", np.nan: "N/A"}],
+)
+def test_ptable_heatmap_plotly_label_map(
+    label_map: dict[str, str] | Literal[False] | None
+) -> None:
+    elem_vals = dict(Al=1.0, Cr=2.0, Fe=3.0, Ni=np.nan)
+    fig = ptable_heatmap_plotly(elem_vals, label_map=label_map)
+    assert isinstance(fig, go.Figure)
+
+    # if label_map is not False, ensure mapped labels appear in figure annotations
+    if label_map is not False:
+        if label_map is None:
+            # use default map
+            label_map = dict.fromkeys([np.nan, None, "nan"], " ")  # type: ignore
+        # check for non-empty intersection between label_map values and annotations
+        # we use `val in anno.text` cause the labels are wrapped in non-matching
+        # HTML <span> tags
+        assert sum(
+            any(val in anno.text for val in label_map.values())
+            for anno in fig.layout.annotations
+        )
```

### Comparing `pymatviz-0.6.2/tests/test_relevance.py` & `pymatviz-0.6.3/tests/test_relevance.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,46 @@
 from __future__ import annotations
 
+from typing import TYPE_CHECKING
+
 import matplotlib.pyplot as plt
-import pandas as pd
 import pytest
 
 from pymatviz import precision_recall_curve, roc_curve
-from pymatviz.utils import Array
 from tests.conftest import df_x_y_clf
 
 
+if TYPE_CHECKING:
+    import pandas as pd
+    from numpy.typing import ArrayLike
+
+
 @pytest.mark.parametrize("ax", [None, plt.gca()])
 @pytest.mark.parametrize("df, y_binary, y_proba", df_x_y_clf)
 def test_roc_curve(
-    df: pd.DataFrame | None, y_binary: str | Array, y_proba: str | Array, ax: plt.Axes
+    df: pd.DataFrame | None,
+    y_binary: str | ArrayLike,
+    y_proba: str | ArrayLike,
+    ax: plt.Axes,
 ) -> None:
     roc_auc, ax = roc_curve(y_binary, y_proba, df=df, ax=ax)
     assert isinstance(roc_auc, float)
     assert isinstance(ax, plt.Axes)
     assert ax.get_title() == "ROC Curve"
     assert ax.get_xlabel() == "False Positive Rate"
     assert ax.get_ylabel() == "True Positive Rate"
 
 
 @pytest.mark.parametrize("ax", [None, plt.gca()])
 @pytest.mark.parametrize("df, y_binary, y_proba", df_x_y_clf)
 def test_precision_recall_curve(
-    df: pd.DataFrame | None, y_binary: str | Array, y_proba: str | Array, ax: plt.Axes
+    df: pd.DataFrame | None,
+    y_binary: str | ArrayLike,
+    y_proba: str | ArrayLike,
+    ax: plt.Axes,
 ) -> None:
     precision, ax = precision_recall_curve(y_binary, y_proba, df=df, ax=ax)
     assert isinstance(precision, float)
     assert isinstance(ax, plt.Axes)
     assert ax.get_title() == "Precision-Recall Curve"
     assert ax.get_xlabel() == "Recall"
     assert ax.get_ylabel() == "Precision"
```

### Comparing `pymatviz-0.6.2/tests/test_sankey.py` & `pymatviz-0.6.3/tests/test_sankey.py`

 * *Files identical despite different names*

### Comparing `pymatviz-0.6.2/tests/test_structure_viz.py` & `pymatviz-0.6.3/tests/test_structure_viz.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,16 @@
         standardize_struct=standardize_struct,
     )
     assert isinstance(ax, plt.Axes)
 
     assert ax.get_aspect() == 1, "aspect ratio should be set to 'equal', i.e. 1:1"
     x_min, x_max, y_min, y_max = ax.axis()
     assert x_min == y_min == 0, "x/y_min should be 0"
-    assert x_max > 5 and y_max > 5, "x/y_max should be > 5"
+    assert x_max > 5
+    assert y_max > 5
 
     patch_counts = pd.Series(
         [type(patch).__name__ for patch in ax.patches]
     ).value_counts()
     assert patch_counts["Wedge"] == len(disordered_struct.composition)
 
     assert patch_counts["PathPatch"] > 182
```

### Comparing `pymatviz-0.6.2/tests/test_sunburst.py` & `pymatviz-0.6.3/tests/test_sunburst.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from __future__ import annotations
 
-from typing import Literal
+from typing import TYPE_CHECKING, Literal
 
 import plotly.graph_objects as go
 import pytest
-from pymatgen.core import Structure
 
 from pymatviz import spacegroup_sunburst
 
 
+if TYPE_CHECKING:
+    from pymatgen.core import Structure
+
+
 @pytest.mark.parametrize("show_counts", ["value", "percent", False])
 def test_spacegroup_sunburst(
     spg_symbols: list[str],
     structures: list[Structure],
     show_counts: Literal["value", "percent", False],
 ) -> None:
     # spg numbers
```

### Comparing `pymatviz-0.6.2/tests/test_uncertainty.py` & `pymatviz-0.6.3/tests/test_uncertainty.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 from __future__ import annotations
 
-from typing import Sequence
+from typing import TYPE_CHECKING, Sequence
 
 import matplotlib.pyplot as plt
-import pandas as pd
 import pytest
 
 from pymatviz import error_decay_with_uncert, qq_gaussian
-from pymatviz.utils import Array
 from tests.conftest import df, df_x_y, xs, y_pred, y_true
 
 
+if TYPE_CHECKING:
+    import pandas as pd
+    from numpy.typing import ArrayLike
+
+
 y_std_mock = y_true - y_pred
 
 
 assert len(df_x_y) == 2
 assert len(df_x_y[0]) == 3
 
 
 @pytest.mark.parametrize(
     "df, x, y, y_std",
     [
-        [None, y_true, y_pred, y_std_mock],
-        [None, y_true, y_pred, {"y_std_mock": y_std_mock}],
-        [df, *df.columns[:2], df.columns[0]],  # single std col
-        [df, *df.columns[:2], df.columns[:2]],  # multiple std cols
+        (None, y_true, y_pred, y_std_mock),
+        (None, y_true, y_pred, {"y_std_mock": y_std_mock}),
+        (df, *df.columns[:2], df.columns[0]),  # single std col
+        (df, *df.columns[:2], df.columns[:2]),  # multiple std cols
     ],
 )
 @pytest.mark.parametrize("n_rand", [10, 100, 1000])
 @pytest.mark.parametrize("percentiles", [True, False])
 def test_error_decay_with_uncert(
     df: pd.DataFrame,
-    x: Array | str,
-    y: Array | str,
-    y_std: Array | dict[str, Array] | str | Sequence[str],
+    x: ArrayLike | str,
+    y: ArrayLike | str,
+    y_std: ArrayLike | dict[str, ArrayLike] | str | Sequence[str],
     n_rand: int,
     percentiles: bool,
 ) -> None:
     ax = error_decay_with_uncert(
         x, y, y_std, df=df, n_rand=n_rand, percentiles=percentiles
     )
 
@@ -49,26 +52,26 @@
     else:
         assert ax.get_xlabel() == "Excluded samples"
 
 
 @pytest.mark.parametrize(
     "df, x, y, y_std",
     [
-        [*df_x_y[0], xs],
-        [*df_x_y[0], {"foo": xs, "bar": 0.1 * xs}],
-        [*df_x_y[1], df.columns[0]],
-        [*df_x_y[1], df.columns[:2]],
+        (*df_x_y[0], xs),
+        (*df_x_y[0], {"foo": xs, "bar": 0.1 * xs}),
+        (*df_x_y[1], df.columns[0]),
+        (*df_x_y[1], df.columns[:2]),
     ],
 )
 @pytest.mark.parametrize("ax", [None, plt.gca()])
 def test_qq_gaussian(
     df: pd.DataFrame,
-    x: Array | str,
-    y: Array | str,
-    y_std: Array | dict[str, Array],
+    x: ArrayLike | str,
+    y: ArrayLike | str,
+    y_std: ArrayLike | dict[str, ArrayLike],
     ax: plt.Axes,
 ) -> None:
     ax = qq_gaussian(x, y, y_std, df=df, ax=ax)
 
     assert isinstance(ax, plt.Axes)
     assert ax.get_xlabel() == "Theoretical Quantile"
     assert ax.get_ylabel() == "Observed Quantile"
```

### Comparing `pymatviz-0.6.2/tests/test_utils.py` & `pymatviz-0.6.3/tests/test_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from __future__ import annotations
 
-from pathlib import Path
-from typing import Any, Sequence
+import os
+from datetime import datetime
+from typing import TYPE_CHECKING, Any, Sequence
+from unittest.mock import patch
 
 import pandas as pd
 import plotly.graph_objects as go
 import pytest
 from matplotlib import pyplot as plt
 from matplotlib.offsetbox import AnchoredText
 
@@ -17,47 +19,60 @@
     df_to_arrays,
     get_crystal_sys,
     save_fig,
 )
 from tests.conftest import y_pred, y_true
 
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
+
 @pytest.mark.parametrize(
     "metrics, prec",
     [
-        [["RMSE"], 1],
-        [("MAPE", "MSE"), 2],
-        [{"MAE", "R2", "RMSE"}, 3],
-        [{"MAE": 1, "R2": 2, "RMSE": 3}, 0],
+        ("MSE", 1),
+        (["RMSE"], 1),
+        (("MAPE", "MSE"), 2),
+        ({"MAE", "R2", "RMSE"}, 3),
+        ({"MAE": 1, "$R^2$": 2, "RMSE": 3}, 0),
     ],
 )
 def test_annotate_metrics(metrics: dict[str, float] | Sequence[str], prec: int) -> None:
     text_box = annotate_metrics(y_pred, y_true, metrics=metrics, prec=prec)
 
     assert isinstance(text_box, AnchoredText)
 
     expected = dict(MAE=0.113, R2=0.765, RMSE=0.144, MAPE=0.5900, MSE=0.0206)
 
     txt = ""
     if isinstance(metrics, dict):
         for key, val in metrics.items():
             txt += f"{key} = {val:.{prec}f}\n"
     else:
-        for key in metrics:
+        for key in [metrics] if isinstance(metrics, str) else metrics:
             txt += f"{key} = {expected[key]:.{prec}f}\n"
 
     assert text_box.txt.get_text() == txt
 
     prefix, suffix = "Metrics:\n", "\nthe end"
     text_box = annotate_metrics(
         y_pred, y_true, metrics=metrics, prec=prec, prefix=prefix, suffix=suffix
     )
     assert text_box.txt.get_text() == prefix + txt + suffix
 
 
+@pytest.mark.parametrize("metrics", [42, datetime.now()])
+def test_annotate_metrics_raises(metrics: Any) -> None:
+    with pytest.raises(
+        TypeError, match=f"metrics must be dict|list|tuple|set, not {type(metrics)}"
+    ):
+        annotate_metrics(y_pred, y_true, metrics=metrics)
+
+
 @pytest.mark.parametrize(
     "spg_num, crystal_sys",
     [
         (1, "triclinic"),
         (15, "monoclinic"),
         (16, "orthorhombic"),
         (75, "tetragonal"),
@@ -80,15 +95,15 @@
 @pytest.mark.parametrize("line_kwds", [None, {"color": "blue"}])
 def test_add_identity_line(
     plotly_scatter: go.Figure, trace_idx: int, line_kwds: dict[str, str] | None
 ) -> None:
     fig = add_identity_line(plotly_scatter, line_kwds=line_kwds, trace_idx=trace_idx)
     assert isinstance(fig, go.Figure)
 
-    line = [shape for shape in fig.layout["shapes"] if shape["type"] == "line"][0]
+    line = next(shape for shape in fig.layout["shapes"] if shape["type"] == "line")
     assert line["x0"] == line["y0"]  # fails if we don't handle nan since nan != nan
     assert line["x1"] == line["y1"]
     assert line["layer"] == "below"
     assert line["line"]["color"] == line_kwds["color"] if line_kwds else "gray"
 
 
 def test_df_to_arrays() -> None:
@@ -102,36 +117,57 @@
     assert x1 == pytest.approx(y_true)
     assert y1 == pytest.approx(y_pred)
 
     with pytest.raises(TypeError, match="df should be pandas DataFrame or None"):
         df_to_arrays("foo", y_true, y_pred)
 
     bad_col_name = "not-real-col-name"
-    with pytest.raises(KeyError) as exc_info:
+    with pytest.raises(KeyError) as exc:
         df_to_arrays(df, bad_col_name, df.columns[0])
 
-    assert "not-real-col-name" in str(exc_info.value)
+    assert "not-real-col-name" in str(exc.value)
+
+
+@pytest.mark.parametrize("strict", [True, False])
+def test_df_to_arrays_strict(strict: bool) -> None:
+    try:
+        args = df_to_arrays(42, "foo", "bar", strict=strict)
+    except TypeError as exc:
+        if strict:
+            assert "df should be pandas DataFrame or None" in str(exc)  # noqa: PT017
+        else:
+            assert args == ("foo", "bar")
 
 
 @pytest.mark.parametrize("fig", [go.Figure(), plt.figure()])
 @pytest.mark.parametrize("ext", ["html", "svelte", "png", "svg", "pdf"])
 @pytest.mark.parametrize(
     "plotly_config", [None, {"showTips": True}, {"scrollZoom": True}]
 )
+@pytest.mark.parametrize("env_disable", [[], ["CI"]])
+@patch.dict(os.environ, {"CI": "1"})
 def test_save_fig(
     fig: go.Figure | plt.Figure | plt.Axes,
     ext: str,
     tmp_path: Path,
     plotly_config: dict[str, Any] | None,
+    env_disable: list[str],
 ) -> None:
     if isinstance(fig, plt.Figure) and ext in ("svelte", "html"):
-        pytest.skip("svelte not supported for matplotlib figures")
+        pytest.skip("saving to Svelte file not supported for matplotlib figures")
 
     path = f"{tmp_path}/fig.{ext}"
-    save_fig(fig, path, plotly_config=plotly_config)
+    save_fig(fig, path, plotly_config=plotly_config, env_disable=env_disable)
+
+    if any(var in os.environ for var in env_disable):
+        # if CI env var is set, we should not save the figure
+        assert not os.path.exists(path)
+        return
+
+    assert os.path.isfile(path)
 
     if ext in ("svelte", "html"):
         with open(path) as file:
             html = file.read()
         if plotly_config and plotly_config.get("showTips"):
             assert '"showTips": true' in html
         else:
@@ -186,9 +222,28 @@
     assert not df_binned.empty
 
 
 def test_bin_df_cols_raises_value_error() -> None:
     df = pd.DataFrame({"col1": [1, 2, 3, 4], "col2": [2, 3, 4, 5]})
     bin_by_cols = ["col1", "col2"]
 
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError) as exc:
         bin_df_cols(df, bin_by_cols, n_bins=[2])
+
+    assert "len(bin_by_cols)=2 != len(n_bins)=1" in str(exc.value)
+
+
+def test_plotly_pdf_no_mathjax_loading(tmp_path: Path) -> None:
+    # https://github.com/plotly/plotly.py/issues/3469
+    PyPDF2 = pytest.importorskip("PyPDF2")
+
+    fig = go.Figure()
+    fig.add_trace(go.Scatter(x=[1, 2], y=[3, 4]))
+    path = f"{tmp_path}/test.pdf"
+    save_fig(fig, path)
+
+    # check PDF doesn't contain "Loading [MathJax]/extensions/MathMenu.js"
+    with open(path, "rb") as f:
+        pdf = PyPDF2.PdfFileReader(f)
+        assert len(pdf.pages) == 1
+        text = pdf.pages[0].extract_text()
+        assert "Loading [MathJax]/extensions/MathMenu.js" not in text
```

