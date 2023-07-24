# Comparing `tmp/specification_curve-0.3.1.tar.gz` & `tmp/specification_curve-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specification_curve-0.3.1.tar", max compression
+gzip compressed data, was "specification_curve-0.3.2.tar", max compression
```

## Comparing `specification_curve-0.3.1.tar` & `specification_curve-0.3.2.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1072 2022-10-29 20:10:08.860342 specification_curve-0.3.1/LICENSE
--rw-r--r--   0        0        0     4694 2022-10-29 20:10:08.860342 specification_curve-0.3.1/README.md
--rw-r--r--   0        0        0     1693 2022-10-29 20:10:25.673691 specification_curve-0.3.1/pyproject.toml
--rw-r--r--   0        0        0    20216 2022-10-29 20:10:08.864343 specification_curve-0.3.1/src/specification_curve/__init__.py
--rw-r--r--   0        0        0       27 2022-10-29 20:10:08.864343 specification_curve-0.3.1/src/specification_curve/__main__.py
--rw-r--r--   0        0        0    57372 2022-10-29 20:10:08.864343 specification_curve-0.3.1/src/specification_curve/data/example_data.csv
--rw-r--r--   0        0        0     5757 1970-01-01 00:00:00.000000 specification_curve-0.3.1/setup.py
--rw-r--r--   0        0        0     5834 1970-01-01 00:00:00.000000 specification_curve-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-24 18:50:43.107216 specification_curve-0.3.2/LICENSE
+-rw-r--r--   0        0        0     5238 2023-07-24 18:50:43.107216 specification_curve-0.3.2/README.md
+-rw-r--r--   0        0        0     1940 2023-07-24 18:51:03.263249 specification_curve-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0    22827 2023-07-24 18:50:43.111216 specification_curve-0.3.2/src/specification_curve/__init__.py
+-rw-r--r--   0        0        0       27 2023-07-24 18:50:43.111216 specification_curve-0.3.2/src/specification_curve/__main__.py
+-rw-r--r--   0        0        0    57372 2023-07-24 18:50:43.111216 specification_curve-0.3.2/src/specification_curve/data/example_data.csv
+-rw-r--r--   0        0        0     6273 1970-01-01 00:00:00.000000 specification_curve-0.3.2/PKG-INFO
```

### Comparing `specification_curve-0.3.1/LICENSE` & `specification_curve-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `specification_curve-0.3.1/README.md` & `specification_curve-0.3.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 [![Codecov](https://codecov.io/gh/aeturrell/specification_curve/branch/main/graph/badge.svg)](https://codecov.io/gh/aeturrell/specification_curve)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/aeturrell/438fb066e4471312667268669cef2c11/specification_curve-examples.ipynb)
 [![DOI](https://zenodo.org/badge/282989537.svg)](https://zenodo.org/badge/latestdoi/282989537)
 [![Downloads](https://static.pepy.tech/badge/specification-curve)](https://pepy.tech/project/Specification_curve)
 
-[![Linux](https://svgshare.com/i/Zhy.svg)](https://svgshare.com/i/Zhy.svg)
-[![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)
-[![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)
+![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
+![macOS](https://img.shields.io/badge/mac%20os-000000?style=for-the-badge&logo=macos&logoColor=F0F0F0)
+![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)
 
 [![Source](https://img.shields.io/badge/source%20code-github-lightgrey?style=for-the-badge)](https://github.com/aeturrell/specification_curve)
 
 [Go to the full documentation for **Specification Curve**](https://aeturrell.github.io/specification_curve/).
 
 ## Quickstart
 
@@ -80,14 +80,31 @@
 
 To install the development version from git, use:
 
 ```bash
 $ pip install git+https://github.com/aeturrell/specification_curve.git
 ```
 
+## Citing Specification Curve
+
+```text
+@misc{aeturrell_2022_7264033,
+  author       = {Arthur Turrell},
+  title        = {Specification Curve: v0.3.1},
+  month        = oct,
+  year         = 2022,
+  publisher    = {Zenodo},
+  version      = {v0.3.1},
+  doi          = {10.5281/zenodo.7264033},
+  url          = {https://doi.org/10.5281/zenodo.7264033}
+}
+```
+
+Using **Specification Curve** in your paper? Let us know by raising an issue beginning with "citation".
+
 ## License
 
 Distributed under the terms of the [MIT license](https://opensource.org/licenses/MIT).
 
 ## Credits
 
 The package is built with [poetry](https://python-poetry.org/), while the documentation is built with [Jupyter Book](https://jupyterbook.org). Tests are run with [nox](https://nox.thea.codes/en/stable/).
```

### Comparing `specification_curve-0.3.1/pyproject.toml` & `specification_curve-0.3.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "specification_curve"
-version = "0.3.1"
+version = "0.3.2"
 description = "Specification_Curve"
 authors = ["aeturrell <mail@mail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://aeturrell.github.io/specification_curve/"
 repository = "https://github.com/aeturrell/specification_curve"
 documentation = "https://aeturrell.github.io/specification_curve/"
@@ -15,57 +15,67 @@
     "Programming Language :: Python :: 3.10",
 ]
 
 [tool.poetry.urls]
 Changelog = "https://github.com/aeturrell/specification_curve/releases"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0.0"
-pandas = "^1.5.1"
-statsmodels = "^0.13.2"
+python = ">=3.8,<3.12"
+pandas = "^2.0.3"
+statsmodels = "^0.14.0"
 matplotlib = "^3.6.1"
+types-setuptools = ">=67.6,<69.0"
 
 [tool.poetry.dev-dependencies]
-black = "^22.10.0"
-pre-commit = "^2.20.0"
+
+
+[tool.poetry.scripts]
+specification_curve = "specification_curve.__main__:main"
+
+
+[tool.poetry.group.dev.dependencies]
+coverage = "^7.2.7"
+black = "^23.7.0"
+pre-commit = "^3.3.3"
 Sphinx = "^4.0.0"
-typeguard = "^2.13.3"
-safety = "^2.3.1"
-coverage = "^6.5.0"
-pytest = "^7.2.0"
+typeguard = ">=3.0.2,<5.0.0"
+safety = "^2.3.4"
+pytest = "^7.4.0"
 flake8 = "^5.0.4"
-pre-commit-hooks = "^4.3.0"
-nox = "^2022.8.7"
-ipykernel = "^6.16.2"
+pre-commit-hooks = "^4.4.0"
+nox = ">=2022.11.21,<2024.0.0"
+ipykernel = "^6.22.0"
 nbstripout = "^0.6.1"
-jupyter-book = "^0.13.1"
+jupyter-book = "^0.15.1"
 furo = "^2022.9.29"
 ghp-import = "^2.1.0"
-xdoctest = "^1.1.0"
-mypy = "^0.982"
+xdoctest = "^1.1.1"
+mypy = "^1.2"
 reorder-python-imports = "^3.9.0"
 sphinxcontrib-bibtex = "^2.5.0"
-
-[tool.poetry.scripts]
-specification_curve = "specification_curve.__main__:main"
+types-pkg-resources = "^0.1.3"
+types-setuptools = ">=67.6,<69.0"
+pandas-stubs = "^2.0.2.230605"
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
 
 [tool.coverage.run]
 branch = true
 source = ["specification_curve"]
 
 [tool.coverage.report]
 show_missing = true
 fail_under = 98
 
 [tool.mypy]
-strict = true
+strict = false
 pretty = true
 show_column_numbers = true
 show_error_codes = true
 show_error_context = true
+ignore_missing_imports = true
+disallow_untyped_calls = false
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `specification_curve-0.3.1/src/specification_curve/__init__.py` & `specification_curve-0.3.2/src/specification_curve/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,19 +2,27 @@
 Specification Curve
 -------------------
 A package that produces specification curve analysis.
 """
 import copy
 import itertools
 import os
+import typing
 from collections import Counter
 from collections import defaultdict
 from itertools import combinations
 from math import floor
 from math import log10
+from typing import DefaultDict
+from typing import Dict
+from typing import List
+from typing import Optional
+from typing import Set
+from typing import Tuple
+from typing import Union
 
 import matplotlib.patches as patches
 import matplotlib.pyplot as plt
 import matplotlib.ticker as ticker
 import numpy as np
 import pandas as pd
 import pkg_resources
@@ -22,162 +30,203 @@
 
 
 EXAMPLE_FILE = pkg_resources.resource_filename(
     "specification_curve", os.path.join("data", "example_data.csv")
 )
 
 
-def _round_to_1(x):
-    """
-    Rounds numbers to 1 s.f.
+def _round_to_1(x: float) -> float:
+    """Rounds numbers to 1 s.f.
+    Args:
+        x (float): input number
+    Returns:
+        float: number rounded
     """
     return round(x, -int(floor(log10(abs(x)))) + 1)
 
 
-def _double_list_check(XX):
-    """
-    If a list, return as list of lists
+@typing.no_type_check
+def _double_list_check(XX: Union[List[str], List[List[str]]]) -> List[List[str]]:
+    """Ensures that input is returned as nested list.
+    Args:
+        XX (Union[list[str], list[list[str]]]): Input list of (list of) strings
+    Returns:
+        list[list[str]]: List of list of strings
     """
     if not (any(isinstance(el, list) for el in XX)):
         XX = [XX]
     return XX
 
 
-def _single_list_check_str(X):
-    """
-    If type is string, return string in list
+@typing.no_type_check
+def _single_list_check_str(X: Union[str, List[str]]) -> List[str]:
+    """Ensures a list of strings.
+    Args:
+        X (Union[str, list[str]]): input string of list of strings
+    Returns:
+        list[str]: List of strings.
     """
     if type(X) == str:
         X = [X]
     return X
 
 
-def _remove_overlapping_vars(list_to_check, includes_list):
-    """Checks, and removes, any variable in list_to_check that is also in
-    includes_list, returning list_to_check without overlapping variable
-    names.
+def _remove_overlapping_vars(
+    list_to_check: List[str], includes_list: List[str]
+) -> List[str]:
+    """Removes any variable in list_to_check that is also in includes_list.
+    Args:
+        list_to_check (list[str]): _description_
+        includes_listlist (List[str]): _description_
+    Returns:
+        list[str]: without overlapping variable names.
     """
     return [x for x in list_to_check if x not in includes_list]
 
 
-def _pretty_plots():
-    """
-    Uses specification curve package's pretty plot style.
-    Overrides existing style.
-    """
+def _pretty_plots() -> None:
+    """Uses specification curve package's pretty plot style."""
     json_plot_settings = {
         "ytick.labelsize": 16,
         "xtick.labelsize": 16,
         "font.size": 22,
         "figure.figsize": (10, 5),
         "axes.titlesize": 22,
         "axes.labelsize": 18,
         "lines.linewidth": 2,
         "lines.markersize": 3,
         "legend.fontsize": 11,
         "mathtext.fontset": "stix",
-        # "axes.grid": True,
-        # "grid.color": "gray",
-        # "grid.alpha": 0.5,
-        # "grid.linewidth": 0.3,
         "font.family": "STIXGeneral",
     }
     plt.style.use(json_plot_settings)
 
 
 def _excl_combs(lst, r, excludes):
-    """lst = [1, 2, 3, 4, 5, 6]
-    excludes = [{1, 3}]
-    gen = _excl_combs(lst, 2, excludes)
+    """From a given list of combinations, excludes those in `excludes`.
+    Args:
+        lst (list[str]): combinations
+        r (int): combination integer
+        excludes (list[str]): combinations to exclude
+    Returns:
+        list[str]: combinations with excluded combinations remove
     """
     if excludes != [[]]:
         return [
             comb
             for comb in combinations(lst, r)
             if not any(e.issubset(comb) for e in excludes)
         ]
     else:
         return list(combinations(lst, r))
 
 
-def _flatn_list(nested_list):
-    """Flattens nested list"""
+def _flatn_list(nested_list: Union[str, List[str], List[List[str]]]) -> List[str]:
+    """Flattens nested list.
+    Args:
+        nested_list (Union[List[str], List[List[str]]]): nested list
+    Returns:
+        List[str]: flattened list
+    """
     return list(itertools.chain.from_iterable(nested_list))
 
 
 class SpecificationCurve:
     """Specification curve object.
-
     Uses a model to perform all variants of a specification.
     Stores the results of those regressions in a tidy format pandas dataframe.
     Plots the regressions in chart that can optionally be saved.
     Will iterate over multiple inputs for exog. and endog. variables.
     Note that categorical variables that are expanded cannot be mutually
     excluded from other categorical variables that are expanded.
-
     """
 
     def __init__(
         self,
         df: pd.DataFrame,
-        y_endog,
-        x_exog,
-        controls,
-        exclu_grps=[[]],
-        cat_expand=[],
-        always_include=[],
-    ):
+        y_endog: Union[str, List[str]],
+        x_exog: Union[str, List[str]],
+        controls: List[str],
+        exclu_grps: List[List[None]] = [[]],
+        cat_expand: Union[str, List[None]] = [],
+        always_include: List[str] = [],
+    ) -> None:
         """Specification curve object constructor.
-
         Args:
-            df (pd.DataFrame): Data to perform regression on
-            y_endog (_type_): _description_
-            x_exog (_type_): _description_
-            controls (_type_): _description_
-            exclu_grps (list, optional): _description_. Defaults to [[]].
-            cat_expand (list, optional): _description_. Defaults to [].
-            always_include (list, optional): _description_. Defaults to [].
+            df (pd.DataFrame): Data for regressions
+            y_endog (Union[str, List[str]]): Endogeneous variables
+            x_exog (Union[str, List[str]]): Exogeneous variables
+            controls (List[str]): Conditioning variables
+            exclu_grps (List[List[None]], optional): Combinations to exclude. Defaults to [[]].
+            cat_expand (List[None], optional): Fixed effects whose categories to run separately. Defaults to [].
+            always_include (List[str], optional): Any controls to always include. Defaults to [].
         """
         self.df = df.copy()
-        self.y_endog = y_endog
-        self.x_exog = x_exog
-        self.controls = controls
-        self.exclu_grps = exclu_grps
-        self.cat_expand = cat_expand
-        self.always_include = always_include
+        self.y_endog = _single_list_check_str(y_endog)
+        self.x_exog = _single_list_check_str(x_exog)
+        self.controls = _single_list_check_str(controls)
+        self.exclu_grps = _double_list_check(exclu_grps)
+        self.cat_expand = _single_list_check_str(cat_expand)
+        self.always_include = _single_list_check_str(always_include)
 
     def fit(self, estimator=sm.OLS) -> None:
         """Fits a specification curve by performing regressions.
-
         Args:
             estimator (statsmodels.regression.linear_model or statsmodels.discrete.discrete_model, optional): statsmodels estimator. Defaults to sm.OLS.
         """
         self.estimator = estimator
-        self.controls = _single_list_check_str(self.controls)
-        self.cat_expand = _single_list_check_str(self.cat_expand)
-        self.exclu_grps = _double_list_check(self.exclu_grps)
-        self.always_include = _single_list_check_str(self.always_include)
-        self.y_endog = _single_list_check_str(self.y_endog)
-        self.x_exog = _single_list_check_str(self.x_exog)
+        # self.cat_expand = _single_list_check_str(self.cat_expand)
+        # self.exclu_grps = _double_list_check(self.exclu_grps)
+        # self.always_include = _single_list_check_str(self.always_include)
         # If any of always include in any other list, remove it from other list
         self.controls = _remove_overlapping_vars(self.controls, self.always_include)
         self.x_exog = _remove_overlapping_vars(self.x_exog, self.always_include)
         self.ctrl_combs = self._compute_combinations()
         self.df_r = self._spec_curve_regression()
         print("Fit complete")
 
-    def _reg_func(self, y_endog, x_exog, reg_vars):
+    def _reg_func(
+        self, y_endog: List[str], x_exog: str, reg_vars: List[str]
+    ) -> sm.regression.linear_model.RegressionResults:
+        """Performs the regression.
+        Args:
+            y_endog (List[str]): Endogeneous variables
+            x_exog (str): Exogeneous variables
+            reg_vars (List[str]): Controls
+        Returns:
+            sm.regression.linear_model.RegressionResults: coefficients from reg
+        """
         # NB: get dummies
         # transforms by default any col that is object or cat
         xf = pd.get_dummies(self.df, prefix_sep="=")
-        new_cols = [x for x in xf.columns if x not in self.df.columns]
-        gone_cols = [x for x in self.df.columns if x not in xf.columns]
+        new_cols = [str(x) for x in xf.columns if x not in self.df.columns]
+        gone_cols = [str(x) for x in self.df.columns if x not in xf.columns]
         reg_vars_here = copy.copy(reg_vars)
         reg_vars_here.extend(new_cols)
-        [reg_vars_here.remove(x) for x in gone_cols if x in reg_vars_here]
+        # mypy prefers this formulation to a list comprehension
+        for x in gone_cols:
+            if x in reg_vars_here:
+                reg_vars_here.remove(x)
+        # Ensure new cols are int so that statsmodels will run on them.
+        # This is because statsmodels requires all values to be of either int or float dtype.
+        # first get columns series with true or false depending on if not int or float stem to data type
+        non_int_or_float_cols = (
+            ~xf[reg_vars_here]
+            .dtypes.astype("string")
+            .str.split("[1-9][0-9]", regex=True)
+            .str[0]
+            .isin(["int", "float"])
+        )
+        # now take only the trues from
+        cols_to_convert_to_int = list(
+            non_int_or_float_cols[non_int_or_float_cols].index
+        )
+        # convert just these columns to int
+        for col_name in cols_to_convert_to_int:
+            xf[col_name] = xf[col_name].astype(int)
         return self.estimator(xf[y_endog], xf[[x_exog] + reg_vars_here]).fit()
 
     def _compute_combinations(self):
         """
         Finds all possible combinations of variables.
         Changes df to have dummies for cat expand columns.
         """
@@ -226,18 +275,16 @@
         ctrl_combs = [list(x) for x in ctrl_combs]
         # Add in always included regressors
         ctrl_combs = [x + self.always_include for x in ctrl_combs]
         return ctrl_combs
 
     def _spec_curve_regression(self):
         """Performs all regressions for a specification curve.
-
         Estimates model with estimator as given in fitting function.
         Assumes that all controls and fixed effects should be varied.
-
         :returns: pandas dataframe of results
         """
         # Regressions - order of loop matters here
         reg_results = [
             [
                 [self._reg_func(y, x, ctrl_vars) for ctrl_vars in self.ctrl_combs]
                 for x in self.x_exog
@@ -284,19 +331,20 @@
         df_r = df_r.drop([x for x in df_r.columns if x not in cols_to_keep], axis=1)
         df_r = df_r.reset_index().drop("index", axis=1)
         df_r.index.names = ["Specification No."]
         df_r["Specification"] = df_r["Specification"].apply(lambda x: sorted(x))
         df_r["SpecificationCounts"] = df_r["Specification"].apply(lambda x: Counter(x))
         return df_r
 
-    def plot(self, save_path=None, pretty_plots=True, preferred_spec=[]):
+    def plot(
+        self, save_path=None, pretty_plots: bool = True, preferred_spec: List[None] = []
+    ) -> None:
         """Makes plots of fitted specification curve.
-
         Args:
-            save_path (_type_, optional): Eexported fig filename. Defaults to None.
+            save_path (_type_, optional): Exported fig filename. Defaults to None.
             pretty_plots (bool, optional): whether to use this package's figure formatting. Defaults to True.
             preferred_spec (list, optional): preferred specification. Defaults to [].
         """
         if pretty_plots:
             _pretty_plots()
         # Set up blocks for showing what effects are included
         df_spec = self.df_r["SpecificationCounts"].apply(pd.Series).fillna(0.0)
@@ -441,21 +489,20 @@
         if len(self.df_r) > 160:
             wid = 0.01
             color_dict = {True: "k", False: "#FFFFFF"}
         # Define group names to put on RHS of plot
 
         def return_string():
             """Convenience function to setup default dict.
-
             Returns:
                 str: "subset"
             """
             return "subset"
 
-        block_name_dict = defaultdict(return_string)
+        block_name_dict: DefaultDict[str, str] = defaultdict(return_string)
         block_name_dict.update({"x_exog": "x", "y_endog": "y", "control": "controls"})
         for ax_num, ax in enumerate(axarr[1:]):
             block_index = block_df.loc[block_df["group_index"] == ax_num, :].index
             df_sp_sl = df_spec.loc[block_index, :].copy()
             for i, row_name in enumerate(df_sp_sl.index):
                 for j, col_name in enumerate(df_sp_sl.columns):
                     color = color_dict[df_sp_sl.iloc[i, j]]
@@ -491,15 +538,14 @@
         if save_path is not None:
             plt.savefig(save_path, dpi=300)
         plt.show()
 
 
 def load_example_data1() -> pd.DataFrame:
     """Retrieves example data from a file included with the package.
-
     Returns:
         pd.DataFrame: Example data suitable for regression.
     """
     # Example data
     df = pd.read_csv(EXAMPLE_FILE, index_col=0)
     num_cols = [x for x in df.columns if x not in ["group1", "group2"]]
     for col in num_cols:
@@ -508,15 +554,14 @@
     for col in cat_cols:
         df[col] = df[col].astype("category")
     return df
 
 
 def load_example_data2() -> pd.DataFrame:
     """Generates fake data.
-
     Returns:
         pd.DataFrame: Example data suitable for regression.
     """
     # Set seed for random numbers
     seed_for_prng = 78557
     # prng=probabilistic random number generator
     prng = np.random.default_rng(seed_for_prng)
```

### Comparing `specification_curve-0.3.1/src/specification_curve/data/example_data.csv` & `specification_curve-0.3.2/src/specification_curve/data/example_data.csv`

 * *Files identical despite different names*

### Comparing `specification_curve-0.3.1/setup.py` & `specification_curve-0.3.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,140 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: specification-curve
+Version: 0.3.2
+Summary: Specification_Curve
+Home-page: https://aeturrell.github.io/specification_curve/
+License: MIT
+Author: aeturrell
+Author-email: mail@mail.com
+Requires-Python: >=3.8,<3.12
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: matplotlib (>=3.6.1,<4.0.0)
+Requires-Dist: pandas (>=2.0.3,<3.0.0)
+Requires-Dist: statsmodels (>=0.14.0,<0.15.0)
+Requires-Dist: types-setuptools (>=67.6,<69.0)
+Project-URL: Changelog, https://github.com/aeturrell/specification_curve/releases
+Project-URL: Documentation, https://aeturrell.github.io/specification_curve/
+Project-URL: Repository, https://github.com/aeturrell/specification_curve
+Description-Content-Type: text/markdown
+
+# Specification Curve
+
+Specification Curve is a Python package that performs specification curve analysis; it helps with the problem of the "garden of forking paths" (many defensible choices) when doing analysis by running many regressions and summarising the effects in an easy to digest chart.
+
+[![PyPI](https://img.shields.io/pypi/v/specification_curve.svg)](https://pypi.org/project/specification_curve/)
+[![Status](https://img.shields.io/pypi/status/specification_curve.svg)](https://pypi.org/project/specification_curve/)
+[![Python Version](https://img.shields.io/pypi/pyversions/specification_curve)](https://pypi.org/project/specification_curve)
+[![License](https://img.shields.io/pypi/l/specification_curve)](https://opensource.org/licenses/MIT)
+[![Tests](https://github.com/aeturrell/specification_curve/workflows/Tests/badge.svg)](https://github.com/aeturrell/specification_curve/actions?workflow=Tests)
+[![Codecov](https://codecov.io/gh/aeturrell/specification_curve/branch/main/graph/badge.svg)](https://codecov.io/gh/aeturrell/specification_curve)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
+[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/aeturrell/438fb066e4471312667268669cef2c11/specification_curve-examples.ipynb)
+[![DOI](https://zenodo.org/badge/282989537.svg)](https://zenodo.org/badge/latestdoi/282989537)
+[![Downloads](https://static.pepy.tech/badge/specification-curve)](https://pepy.tech/project/Specification_curve)
+
+![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
+![macOS](https://img.shields.io/badge/mac%20os-000000?style=for-the-badge&logo=macos&logoColor=F0F0F0)
+![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)
+
+[![Source](https://img.shields.io/badge/source%20code-github-lightgrey?style=for-the-badge)](https://github.com/aeturrell/specification_curve)
+
+[Go to the full documentation for **Specification Curve**](https://aeturrell.github.io/specification_curve/).
+
+## Quickstart
+
+You can try out specification curve right now in [Google Colab](https://colab.research.google.com/gist/aeturrell/438fb066e4471312667268669cef2c11/specification_curve-examples.ipynb).
+
+Here's an example of using **Specification Curve**.
+
+```python
+# import specification curve
+import specification_curve as specy
+
+
+# Generate some fake data
+# ------------------------
+import numpy as np
+import pandas as pd
+# Set seed for random numbers
+seed_for_prng = 78557
+# prng=probabilistic random number generator
+prng = np.random.default_rng(seed_for_prng)
+n_samples = 400
+# Number of dimensions
+n_dim = 4
+c_rnd_vars = prng.random(size=(n_dim, n_samples))
+y_1 = (0.4*c_rnd_vars[0, :] -  # THIS IS THE TRUE VALUE OF THE COEFFICIENT
+       0.2*c_rnd_vars[1, :] +
+       0.3*prng.standard_normal(n_samples))
+# Next line causes y_2 ests to be much more noisy
+y_2 = y_1 - 0.5*np.abs(prng.standard_normal(n_samples))
+# Put data into dataframe
+df = pd.DataFrame([y_1, y_2], ['y1', 'y2']).T
+df["x_1"] = c_rnd_vars[0, :]
+df["c_1"] = c_rnd_vars[1, :]
+df["c_2"] = c_rnd_vars[2, :]
+df["c_3"] = c_rnd_vars[3, :]
+
+# Specification Curve Analysis
+#-----------------------------
+sc = specy.SpecificationCurve(
+    df,
+    y_endog=['y1', 'y2'],
+    x_exog="x_1",
+    controls=["c_1", "c_2", "c_3"])
+sc.fit()
+sc.plot()
+```
+
+Grey squares (black lines when there are many specifications) show whether a variable is included in a specification or not. Blue or red markers and error bars show whether the coefficient is positive and significant (at the 0.05 level) or red and significant, respectively.
+
+## Installation
+
+You can install **Specification Curve** via pip:
+
+```bash
+$ pip install specification-curve
+```
+
+To install the development version from git, use:
+
+```bash
+$ pip install git+https://github.com/aeturrell/specification_curve.git
+```
+
+## Citing Specification Curve
+
+```text
+@misc{aeturrell_2022_7264033,
+  author       = {Arthur Turrell},
+  title        = {Specification Curve: v0.3.1},
+  month        = oct,
+  year         = 2022,
+  publisher    = {Zenodo},
+  version      = {v0.3.1},
+  doi          = {10.5281/zenodo.7264033},
+  url          = {https://doi.org/10.5281/zenodo.7264033}
+}
+```
 
-package_dir = \
-{'': 'src'}
+Using **Specification Curve** in your paper? Let us know by raising an issue beginning with "citation".
 
-packages = \
-['specification_curve']
+## License
 
-package_data = \
-{'': ['*'], 'specification_curve': ['data/*']}
-
-install_requires = \
-['matplotlib>=3.6.1,<4.0.0',
- 'pandas>=1.5.1,<2.0.0',
- 'statsmodels>=0.13.2,<0.14.0']
-
-entry_points = \
-{'console_scripts': ['specification_curve = specification_curve.__main__:main']}
-
-setup_kwargs = {
-    'name': 'specification-curve',
-    'version': '0.3.1',
-    'description': 'Specification_Curve',
-    'long_description': '# Specification Curve\n\nSpecification Curve is a Python package that performs specification curve analysis; it helps with the problem of the "garden of forking paths" (many defensible choices) when doing analysis by running many regressions and summarising the effects in an easy to digest chart.\n\n[![PyPI](https://img.shields.io/pypi/v/specification_curve.svg)](https://pypi.org/project/specification_curve/)\n[![Status](https://img.shields.io/pypi/status/specification_curve.svg)](https://pypi.org/project/specification_curve/)\n[![Python Version](https://img.shields.io/pypi/pyversions/specification_curve)](https://pypi.org/project/specification_curve)\n[![License](https://img.shields.io/pypi/l/specification_curve)](https://opensource.org/licenses/MIT)\n[![Tests](https://github.com/aeturrell/specification_curve/workflows/Tests/badge.svg)](https://github.com/aeturrell/specification_curve/actions?workflow=Tests)\n[![Codecov](https://codecov.io/gh/aeturrell/specification_curve/branch/main/graph/badge.svg)](https://codecov.io/gh/aeturrell/specification_curve)\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/aeturrell/438fb066e4471312667268669cef2c11/specification_curve-examples.ipynb)\n[![DOI](https://zenodo.org/badge/282989537.svg)](https://zenodo.org/badge/latestdoi/282989537)\n[![Downloads](https://static.pepy.tech/badge/specification-curve)](https://pepy.tech/project/Specification_curve)\n\n[![Linux](https://svgshare.com/i/Zhy.svg)](https://svgshare.com/i/Zhy.svg)\n[![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)\n[![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)\n\n[![Source](https://img.shields.io/badge/source%20code-github-lightgrey?style=for-the-badge)](https://github.com/aeturrell/specification_curve)\n\n[Go to the full documentation for **Specification Curve**](https://aeturrell.github.io/specification_curve/).\n\n## Quickstart\n\nYou can try out specification curve right now in [Google Colab](https://colab.research.google.com/gist/aeturrell/438fb066e4471312667268669cef2c11/specification_curve-examples.ipynb).\n\nHere\'s an example of using **Specification Curve**.\n\n```python\n# import specification curve\nimport specification_curve as specy\n\n\n# Generate some fake data\n# ------------------------\nimport numpy as np\nimport pandas as pd\n# Set seed for random numbers\nseed_for_prng = 78557\n# prng=probabilistic random number generator\nprng = np.random.default_rng(seed_for_prng)\nn_samples = 400\n# Number of dimensions\nn_dim = 4\nc_rnd_vars = prng.random(size=(n_dim, n_samples))\ny_1 = (0.4*c_rnd_vars[0, :] -  # THIS IS THE TRUE VALUE OF THE COEFFICIENT\n       0.2*c_rnd_vars[1, :] +\n       0.3*prng.standard_normal(n_samples))\n# Next line causes y_2 ests to be much more noisy\ny_2 = y_1 - 0.5*np.abs(prng.standard_normal(n_samples))\n# Put data into dataframe\ndf = pd.DataFrame([y_1, y_2], [\'y1\', \'y2\']).T\ndf["x_1"] = c_rnd_vars[0, :]\ndf["c_1"] = c_rnd_vars[1, :]\ndf["c_2"] = c_rnd_vars[2, :]\ndf["c_3"] = c_rnd_vars[3, :]\n\n# Specification Curve Analysis\n#-----------------------------\nsc = specy.SpecificationCurve(\n    df,\n    y_endog=[\'y1\', \'y2\'],\n    x_exog="x_1",\n    controls=["c_1", "c_2", "c_3"])\nsc.fit()\nsc.plot()\n```\n\nGrey squares (black lines when there are many specifications) show whether a variable is included in a specification or not. Blue or red markers and error bars show whether the coefficient is positive and significant (at the 0.05 level) or red and significant, respectively.\n\n## Installation\n\nYou can install **Specification Curve** via pip:\n\n```bash\n$ pip install specification-curve\n```\n\nTo install the development version from git, use:\n\n```bash\n$ pip install git+https://github.com/aeturrell/specification_curve.git\n```\n\n## License\n\nDistributed under the terms of the [MIT license](https://opensource.org/licenses/MIT).\n\n## Credits\n\nThe package is built with [poetry](https://python-poetry.org/), while the documentation is built with [Jupyter Book](https://jupyterbook.org). Tests are run with [nox](https://nox.thea.codes/en/stable/).\n\n## Similar Packages\n\nIn RStats, there is [specr](https://github.com/masurp/specr) (which inspired many design choices in this package) and [spec_chart](https://github.com/ArielOrtizBobea/spec_chart). Some of the example data in this package is the same as in specr, but please note that results have not been cross-checked across packages.\n',
-    'author': 'aeturrell',
-    'author_email': 'mail@mail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://aeturrell.github.io/specification_curve/',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0.0',
-}
+Distributed under the terms of the [MIT license](https://opensource.org/licenses/MIT).
+
+## Credits
+
+The package is built with [poetry](https://python-poetry.org/), while the documentation is built with [Jupyter Book](https://jupyterbook.org). Tests are run with [nox](https://nox.thea.codes/en/stable/).
+
+## Similar Packages
 
+In RStats, there is [specr](https://github.com/masurp/specr) (which inspired many design choices in this package) and [spec_chart](https://github.com/ArielOrtizBobea/spec_chart). Some of the example data in this package is the same as in specr, but please note that results have not been cross-checked across packages.
 
-setup(**setup_kwargs)
```

