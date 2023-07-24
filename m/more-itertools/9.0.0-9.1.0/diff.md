# Comparing `tmp/more-itertools-9.0.0.tar.gz` & `tmp/more-itertools-9.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "more-itertools-9.0.0.tar", last modified: Tue Oct 18 13:38:38 2022, max compression
+gzip compressed data, was "more-itertools-9.1.0.tar", last modified: Mon Feb 27 14:42:05 2023, max compression
```

## Comparing `more-itertools-9.0.0.tar` & `more-itertools-9.1.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0       81 2022-10-18 13:37:02.101069 more-itertools-9.0.0/.gitattributes
--rw-r--r--   0        0        0       88 2022-10-18 13:37:02.101069 more-itertools-9.0.0/.github/ISSUE_TEMPLATE/other-issues.md
--rw-r--r--   0        0        0      589 2022-10-18 13:37:02.101069 more-itertools-9.0.0/.github/ISSUE_TEMPLATE/propose-a-new-itertool.md
--rw-r--r--   0        0        0      368 2022-10-18 13:37:02.101069 more-itertools-9.0.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0     1695 2022-10-18 13:38:19.069835 more-itertools-9.0.0/.github/workflows/python-app.yml
--rw-r--r--   0        0        0      328 2022-10-18 13:37:02.101069 more-itertools-9.0.0/.gitignore
--rw-r--r--   0        0        0     1053 2022-10-18 13:37:02.101069 more-itertools-9.0.0/LICENSE
--rw-r--r--   0        0        0      196 2022-10-18 13:37:02.101069 more-itertools-9.0.0/MANIFEST.in
--rw-r--r--   0        0        0    30136 2022-10-18 13:38:19.069835 more-itertools-9.0.0/README.rst
--rw-r--r--   0        0        0     5596 2022-10-18 13:37:02.101069 more-itertools-9.0.0/docs/Makefile
--rw-r--r--   0        0        0      437 2022-10-18 13:37:02.101069 more-itertools-9.0.0/docs/_static/theme_overrides.css
--rw-r--r--   0        0        0     6133 2022-10-18 13:37:02.101069 more-itertools-9.0.0/docs/api.rst
--rw-r--r--   0        0        0     9150 2022-10-18 13:37:02.101069 more-itertools-9.0.0/docs/conf.py
--rw-r--r--   0        0        0      163 2022-10-18 13:37:02.101069 more-itertools-9.0.0/docs/index.rst
--rw-r--r--   0        0        0      646 2022-10-18 13:37:02.101069 more-itertools-9.0.0/docs/license.rst
--rw-r--r--   0        0        0     5112 2022-10-18 13:37:02.101069 more-itertools-9.0.0/docs/make.bat
--rw-r--r--   0        0        0        7 2022-10-18 13:37:02.101069 more-itertools-9.0.0/docs/requirements.txt
--rw-r--r--   0        0        0      302 2022-10-18 13:37:02.101069 more-itertools-9.0.0/docs/testing.rst
--rw-r--r--   0        0        0    22215 2022-10-18 13:38:19.069835 more-itertools-9.0.0/docs/versions.rst
--rw-r--r--   0        0        0      148 2022-10-18 13:38:19.069835 more-itertools-9.0.0/more_itertools/__init__.py
--rw-r--r--   0        0        0       43 2022-10-18 13:37:02.101069 more-itertools-9.0.0/more_itertools/__init__.pyi
--rwxr-xr-x   0        0        0   133336 2022-10-18 13:38:19.073834 more-itertools-9.0.0/more_itertools/more.py
--rw-r--r--   0        0        0    20297 2022-10-18 13:38:19.073834 more-itertools-9.0.0/more_itertools/more.pyi
--rw-r--r--   0        0        0        0 2022-10-18 13:37:02.101069 more-itertools-9.0.0/more_itertools/py.typed
--rw-r--r--   0        0        0    22975 2022-10-18 13:38:19.073834 more-itertools-9.0.0/more_itertools/recipes.py
--rw-r--r--   0        0        0     3851 2022-10-18 13:38:19.073834 more-itertools-9.0.0/more_itertools/recipes.pyi
--rw-r--r--   0        0        0     1344 2022-10-18 13:38:19.073834 more-itertools-9.0.0/pyproject.toml
--rw-r--r--   0        0        0      681 2022-10-18 13:38:19.073834 more-itertools-9.0.0/setup.cfg
--rw-r--r--   0        0        0       38 2022-10-18 13:37:02.101069 more-itertools-9.0.0/setup.py
--rw-r--r--   0        0        0        0 2022-10-18 13:37:02.101069 more-itertools-9.0.0/tests/__init__.py
--rw-r--r--   0        0        0   175595 2022-10-18 13:38:19.073834 more-itertools-9.0.0/tests/test_more.py
--rw-r--r--   0        0        0    30719 2022-10-18 13:38:19.073834 more-itertools-9.0.0/tests/test_recipes.py
--rw-r--r--   0        0        0      113 2022-10-18 13:37:02.101069 more-itertools-9.0.0/tox.ini
--rw-r--r--   0        0        0    31266 1970-01-01 00:00:00.000000 more-itertools-9.0.0/PKG-INFO
+-rw-r--r--   0        0        0       81 2021-11-04 16:55:44.181025 more-itertools-9.1.0/.gitattributes
+-rw-r--r--   0        0        0       88 2021-11-04 16:55:44.181558 more-itertools-9.1.0/.github/ISSUE_TEMPLATE/other-issues.md
+-rw-r--r--   0        0        0      589 2021-11-04 16:55:44.181762 more-itertools-9.1.0/.github/ISSUE_TEMPLATE/propose-a-new-itertool.md
+-rw-r--r--   0        0        0      368 2021-11-04 16:55:44.181974 more-itertools-9.1.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0     1706 2023-02-21 17:00:55.991196 more-itertools-9.1.0/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0      328 2021-11-04 16:55:44.182514 more-itertools-9.1.0/.gitignore
+-rw-r--r--   0        0        0     1053 2021-11-04 16:55:44.182692 more-itertools-9.1.0/LICENSE
+-rw-r--r--   0        0        0      196 2021-11-04 16:55:44.182945 more-itertools-9.1.0/MANIFEST.in
+-rw-r--r--   0        0        0    31141 2023-02-27 14:41:12.542422 more-itertools-9.1.0/README.rst
+-rw-r--r--   0        0        0     5596 2021-11-04 16:55:44.183643 more-itertools-9.1.0/docs/Makefile
+-rw-r--r--   0        0        0      437 2021-11-04 16:55:44.183953 more-itertools-9.1.0/docs/_static/theme_overrides.css
+-rw-r--r--   0        0        0     6271 2023-02-21 15:06:20.592258 more-itertools-9.1.0/docs/api.rst
+-rw-r--r--   0        0        0     9150 2022-08-23 13:45:26.468085 more-itertools-9.1.0/docs/conf.py
+-rw-r--r--   0        0        0      163 2022-08-23 13:45:26.469220 more-itertools-9.1.0/docs/index.rst
+-rw-r--r--   0        0        0      646 2021-11-04 16:55:44.185598 more-itertools-9.1.0/docs/license.rst
+-rw-r--r--   0        0        0     5112 2021-11-04 16:55:44.185850 more-itertools-9.1.0/docs/make.bat
+-rw-r--r--   0        0        0        7 2022-04-29 14:09:30.635338 more-itertools-9.1.0/docs/requirements.txt
+-rw-r--r--   0        0        0      302 2021-11-04 16:55:44.186089 more-itertools-9.1.0/docs/testing.rst
+-rw-r--r--   0        0        0    23217 2023-02-27 14:41:12.546871 more-itertools-9.1.0/docs/versions.rst
+-rw-r--r--   0        0        0      148 2023-02-27 14:41:12.550684 more-itertools-9.1.0/more_itertools/__init__.py
+-rw-r--r--   0        0        0       43 2021-11-04 16:55:44.187494 more-itertools-9.1.0/more_itertools/__init__.pyi
+-rwxr-xr-x   0        0        0   134968 2023-02-21 15:05:46.935729 more-itertools-9.1.0/more_itertools/more.py
+-rw-r--r--   0        0        0    20105 2023-02-21 15:05:46.938101 more-itertools-9.1.0/more_itertools/more.pyi
+-rw-r--r--   0        0        0        0 2021-11-04 16:55:44.189144 more-itertools-9.1.0/more_itertools/py.typed
+-rw-r--r--   0        0        0    25416 2023-02-21 15:05:46.940384 more-itertools-9.1.0/more_itertools/recipes.py
+-rw-r--r--   0        0        0     4056 2023-02-21 15:05:46.943320 more-itertools-9.1.0/more_itertools/recipes.pyi
+-rw-r--r--   0        0        0     1344 2022-11-03 19:57:28.417051 more-itertools-9.1.0/pyproject.toml
+-rw-r--r--   0        0        0      681 2023-02-27 14:41:12.554733 more-itertools-9.1.0/setup.cfg
+-rw-r--r--   0        0        0       38 2022-04-29 14:09:30.654483 more-itertools-9.1.0/setup.py
+-rw-r--r--   0        0        0        0 2021-11-04 16:55:44.191193 more-itertools-9.1.0/tests/__init__.py
+-rw-r--r--   0        0        0   177305 2023-01-13 20:05:28.316245 more-itertools-9.1.0/tests/test_more.py
+-rw-r--r--   0        0        0    33876 2023-02-21 15:05:46.945628 more-itertools-9.1.0/tests/test_recipes.py
+-rw-r--r--   0        0        0      113 2022-03-09 19:55:14.109171 more-itertools-9.1.0/tox.ini
+-rw-r--r--   0        0        0    32271 1970-01-01 00:00:00.000000 more-itertools-9.1.0/PKG-INFO
```

### Comparing `more-itertools-9.0.0/.github/ISSUE_TEMPLATE/propose-a-new-itertool.md` & `more-itertools-9.1.0/.github/ISSUE_TEMPLATE/propose-a-new-itertool.md`

 * *Files identical despite different names*

### Comparing `more-itertools-9.0.0/.github/workflows/python-app.yml` & `more-itertools-9.1.0/.github/workflows/python-app.yml`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11.0-rc.2", "pypy-3.8"]
+        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11", "3.12.0-alpha.1", "pypy-3.8"]
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install .
         pip install -U coverage flake8 wheel
```

### Comparing `more-itertools-9.0.0/LICENSE` & `more-itertools-9.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `more-itertools-9.0.0/README.rst` & `more-itertools-9.1.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 |                        | `split_into <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.split_into>`_,                                                                         |
 |                        | `split_when <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.split_when>`_,                                                                         |
 |                        | `bucket <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.bucket>`_,                                                                                 |
 |                        | `unzip <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.unzip>`_,                                                                                   |
 |                        | `batched <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.batched>`_,                                                                               |
 |                        | `grouper <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.grouper>`_,                                                                               |
 |                        | `partition <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.partition>`_                                                                            |
+|                        | `transpose <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.transpose>`_                                                                            |
 +------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
 | Lookahead and lookback | `spy <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.spy>`_,                                                                                       |
 |                        | `peekable <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.peekable>`_,                                                                             |
 |                        | `seekable <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.seekable>`_                                                                              |
 +------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
 | Windowing              | `windowed <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.windowed>`_,                                                                             |
 |                        | `substrings <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.substrings>`_,                                                                         |
@@ -111,14 +112,15 @@
 |                        | `distinct_combinations <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.distinct_combinations>`_,                                                   |
 |                        | `circular_shifts <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.circular_shifts>`_,                                                               |
 |                        | `partitions <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.partitions>`_,                                                                         |
 |                        | `set_partitions <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.set_partitions>`_,                                                                 |
 |                        | `product_index <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.product_index>`_,                                                                   |
 |                        | `combination_index <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.combination_index>`_,                                                           |
 |                        | `permutation_index <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.permutation_index>`_,                                                           |
+|                        | `gray_product  <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.gray_product>`_,                                                                    |
 |                        | `powerset <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.powerset>`_,                                                                             |
 |                        | `random_product <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.random_product>`_,                                                                 |
 |                        | `random_permutation <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.random_permutation>`_,                                                         |
 |                        | `random_combination <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.random_combination>`_,                                                         |
 |                        | `random_combination_with_replacement <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.random_combination_with_replacement>`_,                       |
 |                        | `nth_product <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.nth_product>`_,                                                                       |
 |                        | `nth_permutation <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.nth_permutation>`_,                                                               |
@@ -138,19 +140,22 @@
 |                        | `side_effect <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.side_effect>`_,                                                                       |
 |                        | `iterate <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.iterate>`_,                                                                               |
 |                        | `difference <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.difference>`_,                                                                         |
 |                        | `make_decorator <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.make_decorator>`_,                                                                 |
 |                        | `SequenceView <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.SequenceView>`_,                                                                     |
 |                        | `time_limited <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.time_limited>`_,                                                                     |
 |                        | `map_if <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.map_if>`_,                                                                                 |
+|                        | `iter_index <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.iter_index>`_,                                                                         |
 |                        | `consume <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.consume>`_,                                                                               |
 |                        | `tabulate <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.tabulate>`_,                                                                             |
-|                        | `repeatfunc <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.repeatfunc>`_                                                                          |
-|                        | `polynomial_from_roots <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.polynomial_from_roots>`_                                                    |
+|                        | `repeatfunc <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.repeatfunc>`_,                                                                         |
+|                        | `polynomial_from_roots <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.polynomial_from_roots>`_,                                                   |
 |                        | `sieve <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.sieve>`_                                                                                    |
+|                        | `factor <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.factor>`_                                                                                  |
+|                        | `matmul <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.matmul>`_                                                                                  |
 +------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
 
 
 Getting started
 ===============
 
 To get started, install the library with `pip <https://pip.pypa.io/en/stable/>`_:
```

### Comparing `more-itertools-9.0.0/docs/Makefile` & `more-itertools-9.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `more-itertools-9.0.0/docs/api.rst` & `more-itertools-9.1.0/docs/api.rst`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 ----
 
 **Itertools recipes**
 
 .. autofunction:: batched
 .. autofunction:: grouper
 .. autofunction:: partition
+.. autofunction:: transpose
 
 
 Lookahead and lookback
 ======================
 
 These tools peek at an iterable's values without advancing it.
 
@@ -220,14 +221,15 @@
 .. autofunction:: distinct_combinations
 .. autofunction:: circular_shifts
 .. autofunction:: partitions
 .. autofunction:: set_partitions
 .. autofunction:: product_index
 .. autofunction:: combination_index
 .. autofunction:: permutation_index
+.. autofunction:: gray_product
 
 ----
 
 **Itertools recipes**
 
 .. autofunction:: powerset
 .. autofunction:: random_product
@@ -282,12 +284,15 @@
 .. autofunction:: time_limited
 .. autofunction:: map_if(iterable, pred, func, func_else=lambda x: x)
 
 ----
 
 **Itertools recipes**
 
+.. autofunction:: iter_index
 .. autofunction:: consume
 .. autofunction:: tabulate
 .. autofunction:: repeatfunc
 .. autofunction:: polynomial_from_roots
 .. autofunction:: sieve
+.. autofunction:: factor
+.. autofunction:: matmul
```

### Comparing `more-itertools-9.0.0/docs/conf.py` & `more-itertools-9.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `more-itertools-9.0.0/docs/license.rst` & `more-itertools-9.1.0/docs/license.rst`

 * *Files identical despite different names*

### Comparing `more-itertools-9.0.0/docs/make.bat` & `more-itertools-9.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `more-itertools-9.0.0/docs/versions.rst` & `more-itertools-9.1.0/docs/versions.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,35 @@
 ===============
 Version History
 ===============
 
 .. automodule:: more_itertools
    :noindex:
 
+8.14.0
+------
+
+* New functions
+    * :func:`iter_index` (from the Python itertools docs)
+    * :func:`transpose` (from the Python itertools docs)
+    * :func:`matmul` (from the Python itertools docs)
+    * :func:`factor` (from the Python itertools docs)
+    * :func:`gray_product` (thanks to haukex)
+
+* Changes to existing functions
+    * :func:`sieve` was updated to match the Python itertools docs
+    * :func:`maxsplit` was updated to fix a bug (thanks to abingham)
+    * :func:`sliced` had its `type hint <https://github.com/more-itertools/more-itertools/pull/667>`__ updated (thanks to ad-chaos)
+    
+
+* Other changes
+    * The ``batched`` function is marked as deprecated and will be removed in a future major release. For Python 3.12 and above, use ``itertools.batched`` instead. (thanks to neutrinoceros)
+    * The type hints now used postponed evaluation of annotations from PEP 563 (thanks to Isira-Seneviratne)
+    * Some documentation issues were fixed (thanks to Voskov and jdkandersson)
+
 9.0.0
 ------
 
 * Potentially breaking changes
     * :func:`grouper` no longer accepts an integer as its first argument. Previously this raised a ``DeprecationWarning``.
     * :func:`collate` has been removed. Use the built-in :func:`heapq.merge` instead.
     * :func:`windowed` now yields nothing when its iterable is empty.
```

### Comparing `more-itertools-9.0.0/more_itertools/more.py` & `more-itertools-9.1.0/more_itertools/more.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,14 +64,15 @@
     'distribute',
     'divide',
     'duplicates_everseen',
     'duplicates_justseen',
     'exactly_n',
     'filter_except',
     'first',
+    'gray_product',
     'groupby_transform',
     'ichunked',
     'iequals',
     'ilen',
     'interleave',
     'interleave_evenly',
     'interleave_longest',
@@ -654,14 +655,15 @@
 
         >>> sorted(distinct_permutations([1, 0, 1], r=2))
         [(0, 1), (1, 0), (1, 1)]
         >>> sorted(distinct_permutations(range(3), r=2))
         [(0, 1), (0, 2), (1, 0), (1, 2), (2, 0), (2, 1)]
 
     """
+
     # Algorithm: https://w.wiki/Qai
     def _full(A):
         while True:
             # Yield the permutation we have
             yield tuple(A)
 
             # Find the largest index i such that A[i] < A[i + 1]
@@ -1297,15 +1299,15 @@
     At most *maxsplit* splits are done. If *maxsplit* is not specified or -1,
     then there is no limit on the number of splits:
 
         >>> list(split_at(range(10), lambda n: n % 2 == 1, maxsplit=2))
         [[0], [2], [4, 5, 6, 7, 8, 9]]
 
     By default, the delimiting items are not included in the output.
-    The include them, set *keep_separator* to ``True``.
+    To include them, set *keep_separator* to ``True``.
 
         >>> list(split_at('abcdcba', lambda x: x == 'b', keep_separator=True))
         [['a'], ['b'], ['c', 'd', 'c'], ['b'], ['a']]
 
     """
     if maxsplit == 0:
         yield list(iterable)
@@ -1387,15 +1389,17 @@
     buf = []
     it = iter(iterable)
     for item in it:
         buf.append(item)
         if pred(item) and buf:
             yield buf
             if maxsplit == 1:
-                yield list(it)
+                buf = list(it)
+                if buf:
+                    yield buf
                 return
             buf = []
             maxsplit -= 1
     if buf:
         yield buf
 
 
@@ -2910,14 +2914,15 @@
         ('1', '3', '5')
         >>> it.peek()
         '7'
         >>> next(it)
         '7'
 
     """
+
     # See https://sites.google.com/site/bbayles/index/decorator_factory for
     # notes on how this works.
     def decorator(*wrapping_args, **wrapping_kwargs):
         def outer_wrapper(f):
             def inner_wrapper(*args, **kwargs):
                 result = f(*args, **kwargs)
                 wrapping_args_ = list(wrapping_args)
@@ -3460,15 +3465,14 @@
     W = exp(log(random()) / k)
 
     # The number of elements to skip before changing the reservoir is a random
     # number with a geometric distribution. Sample it using random() and logs.
     next_index = k + floor(log(random()) / log(1 - W))
 
     for index, element in enumerate(iterable, k):
-
         if index == next_index:
             reservoir[randrange(k)] = element
             # The new W is the largest in a sample of k U(0, `old_W`) numbers
             W *= exp(log(random()) / k)
             next_index += floor(log(random()) / log(1 - W)) + 1
 
     return reservoir
@@ -4280,15 +4284,14 @@
             if hi < y:
                 hi = y
 
     else:
         lo_key = hi_key = key(lo)
 
         for x, y in zip_longest(it, it, fillvalue=lo):
-
             x_key, y_key = key(x), key(y)
 
             if y_key < x_key:
                 x, y, x_key, y_key = y, x, y_key, x_key
             if x_key < lo_key:
                 lo, lo_key = x, x_key
             if hi_key < y_key:
@@ -4341,7 +4344,49 @@
 
         batch.append(item)
         batch_size += item_len
         batch_count += 1
 
     if batch:
         yield tuple(batch)
+
+
+def gray_product(*iterables):
+    """Like :func:`itertools.product`, but return tuples in an order such
+    that only one element in the generated tuple changes from one iteration
+    to the next.
+
+        >>> list(gray_product('AB','CD'))
+        [('A', 'C'), ('B', 'C'), ('B', 'D'), ('A', 'D')]
+
+    This function consumes all of the input iterables before producing output.
+    If any of the input iterables have fewer than two items, ``ValueError``
+    is raised.
+
+    For information on the algorithm, see
+    `this section <https://www-cs-faculty.stanford.edu/~knuth/fasc2a.ps.gz>`__
+    of Donald Knuth's *The Art of Computer Programming*.
+    """
+    all_iterables = tuple(tuple(x) for x in iterables)
+    iterable_count = len(all_iterables)
+    for iterable in all_iterables:
+        if len(iterable) < 2:
+            raise ValueError("each iterable must have two or more items")
+
+    # This is based on "Algorithm H" from section 7.2.1.1, page 20.
+    # a holds the indexes of the source iterables for the n-tuple to be yielded
+    # f is the array of "focus pointers"
+    # o is the array of "directions"
+    a = [0] * iterable_count
+    f = list(range(iterable_count + 1))
+    o = [1] * iterable_count
+    while True:
+        yield tuple(all_iterables[i][a[i]] for i in range(iterable_count))
+        j = f[0]
+        f[0] = 0
+        if j == iterable_count:
+            break
+        a[j] = a[j] + o[j]
+        if a[j] == 0 or a[j] == len(all_iterables[j]) - 1:
+            o[j] = -o[j]
+            f[j] = f[j + 1]
+            f[j + 1] = j + 1
```

### Comparing `more-itertools-9.0.0/more_itertools/more.pyi` & `more-itertools-9.1.0/more_itertools/more.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,364 +1,359 @@
 """Stubs for more_itertools.more"""
+from __future__ import annotations
 
+from types import TracebackType
 from typing import (
     Any,
     Callable,
     Container,
-    Dict,
+    ContextManager,
     Generic,
     Hashable,
     Iterable,
     Iterator,
-    List,
-    Optional,
+    overload,
     Reversible,
     Sequence,
     Sized,
-    Tuple,
-    Union,
+    Type,
     TypeVar,
     type_check_only,
 )
-from types import TracebackType
-from typing_extensions import ContextManager, Protocol, Type, overload
+from typing_extensions import Protocol
 
 # Type and type variable definitions
 _T = TypeVar('_T')
 _T1 = TypeVar('_T1')
 _T2 = TypeVar('_T2')
 _U = TypeVar('_U')
 _V = TypeVar('_V')
 _W = TypeVar('_W')
 _T_co = TypeVar('_T_co', covariant=True)
 _GenFn = TypeVar('_GenFn', bound=Callable[..., Iterator[object]])
-_Raisable = Union[BaseException, 'Type[BaseException]']
+_Raisable = BaseException | Type[BaseException]
 
 @type_check_only
 class _SizedIterable(Protocol[_T_co], Sized, Iterable[_T_co]): ...
 
 @type_check_only
 class _SizedReversible(Protocol[_T_co], Sized, Reversible[_T_co]): ...
 
+@type_check_only
+class _SupportsSlicing(Protocol[_T_co]):
+    def __getitem__(self, __k: slice) -> _T_co: ...
+
 def chunked(
-    iterable: Iterable[_T], n: Optional[int], strict: bool = ...
-) -> Iterator[List[_T]]: ...
+    iterable: Iterable[_T], n: int | None, strict: bool = ...
+) -> Iterator[list[_T]]: ...
 @overload
 def first(iterable: Iterable[_T]) -> _T: ...
 @overload
-def first(iterable: Iterable[_T], default: _U) -> Union[_T, _U]: ...
+def first(iterable: Iterable[_T], default: _U) -> _T | _U: ...
 @overload
 def last(iterable: Iterable[_T]) -> _T: ...
 @overload
-def last(iterable: Iterable[_T], default: _U) -> Union[_T, _U]: ...
+def last(iterable: Iterable[_T], default: _U) -> _T | _U: ...
 @overload
 def nth_or_last(iterable: Iterable[_T], n: int) -> _T: ...
 @overload
-def nth_or_last(
-    iterable: Iterable[_T], n: int, default: _U
-) -> Union[_T, _U]: ...
+def nth_or_last(iterable: Iterable[_T], n: int, default: _U) -> _T | _U: ...
 
 class peekable(Generic[_T], Iterator[_T]):
     def __init__(self, iterable: Iterable[_T]) -> None: ...
     def __iter__(self) -> peekable[_T]: ...
     def __bool__(self) -> bool: ...
     @overload
     def peek(self) -> _T: ...
     @overload
-    def peek(self, default: _U) -> Union[_T, _U]: ...
+    def peek(self, default: _U) -> _T | _U: ...
     def prepend(self, *items: _T) -> None: ...
     def __next__(self) -> _T: ...
     @overload
     def __getitem__(self, index: int) -> _T: ...
     @overload
-    def __getitem__(self, index: slice) -> List[_T]: ...
+    def __getitem__(self, index: slice) -> list[_T]: ...
 
 def consumer(func: _GenFn) -> _GenFn: ...
 def ilen(iterable: Iterable[object]) -> int: ...
 def iterate(func: Callable[[_T], _T], start: _T) -> Iterator[_T]: ...
 def with_iter(
     context_manager: ContextManager[Iterable[_T]],
 ) -> Iterator[_T]: ...
 def one(
     iterable: Iterable[_T],
-    too_short: Optional[_Raisable] = ...,
-    too_long: Optional[_Raisable] = ...,
+    too_short: _Raisable | None = ...,
+    too_long: _Raisable | None = ...,
 ) -> _T: ...
 def raise_(exception: _Raisable, *args: Any) -> None: ...
 def strictly_n(
     iterable: Iterable[_T],
     n: int,
-    too_short: Optional[_GenFn] = ...,
-    too_long: Optional[_GenFn] = ...,
-) -> List[_T]: ...
+    too_short: _GenFn | None = ...,
+    too_long: _GenFn | None = ...,
+) -> list[_T]: ...
 def distinct_permutations(
-    iterable: Iterable[_T], r: Optional[int] = ...
-) -> Iterator[Tuple[_T, ...]]: ...
+    iterable: Iterable[_T], r: int | None = ...
+) -> Iterator[tuple[_T, ...]]: ...
 def intersperse(
     e: _U, iterable: Iterable[_T], n: int = ...
-) -> Iterator[Union[_T, _U]]: ...
-def unique_to_each(*iterables: Iterable[_T]) -> List[List[_T]]: ...
+) -> Iterator[_T | _U]: ...
+def unique_to_each(*iterables: Iterable[_T]) -> list[list[_T]]: ...
 @overload
 def windowed(
     seq: Iterable[_T], n: int, *, step: int = ...
-) -> Iterator[Tuple[Optional[_T], ...]]: ...
+) -> Iterator[tuple[_T | None, ...]]: ...
 @overload
 def windowed(
     seq: Iterable[_T], n: int, fillvalue: _U, step: int = ...
-) -> Iterator[Tuple[Union[_T, _U], ...]]: ...
-def substrings(iterable: Iterable[_T]) -> Iterator[Tuple[_T, ...]]: ...
+) -> Iterator[tuple[_T | _U, ...]]: ...
+def substrings(iterable: Iterable[_T]) -> Iterator[tuple[_T, ...]]: ...
 def substrings_indexes(
     seq: Sequence[_T], reverse: bool = ...
-) -> Iterator[Tuple[Sequence[_T], int, int]]: ...
+) -> Iterator[tuple[Sequence[_T], int, int]]: ...
 
 class bucket(Generic[_T, _U], Container[_U]):
     def __init__(
         self,
         iterable: Iterable[_T],
         key: Callable[[_T], _U],
-        validator: Optional[Callable[[object], object]] = ...,
+        validator: Callable[[object], object] | None = ...,
     ) -> None: ...
     def __contains__(self, value: object) -> bool: ...
     def __iter__(self) -> Iterator[_U]: ...
     def __getitem__(self, value: object) -> Iterator[_T]: ...
 
 def spy(
     iterable: Iterable[_T], n: int = ...
-) -> Tuple[List[_T], Iterator[_T]]: ...
+) -> tuple[list[_T], Iterator[_T]]: ...
 def interleave(*iterables: Iterable[_T]) -> Iterator[_T]: ...
 def interleave_longest(*iterables: Iterable[_T]) -> Iterator[_T]: ...
 def interleave_evenly(
-    iterables: List[Iterable[_T]], lengths: Optional[List[int]] = ...
+    iterables: list[Iterable[_T]], lengths: list[int] | None = ...
 ) -> Iterator[_T]: ...
 def collapse(
     iterable: Iterable[Any],
-    base_type: Optional[type] = ...,
-    levels: Optional[int] = ...,
+    base_type: type | None = ...,
+    levels: int | None = ...,
 ) -> Iterator[Any]: ...
 @overload
 def side_effect(
     func: Callable[[_T], object],
     iterable: Iterable[_T],
     chunk_size: None = ...,
-    before: Optional[Callable[[], object]] = ...,
-    after: Optional[Callable[[], object]] = ...,
+    before: Callable[[], object] | None = ...,
+    after: Callable[[], object] | None = ...,
 ) -> Iterator[_T]: ...
 @overload
 def side_effect(
-    func: Callable[[List[_T]], object],
+    func: Callable[[list[_T]], object],
     iterable: Iterable[_T],
     chunk_size: int,
-    before: Optional[Callable[[], object]] = ...,
-    after: Optional[Callable[[], object]] = ...,
+    before: Callable[[], object] | None = ...,
+    after: Callable[[], object] | None = ...,
 ) -> Iterator[_T]: ...
 def sliced(
-    seq: Sequence[_T], n: int, strict: bool = ...
-) -> Iterator[Sequence[_T]]: ...
+    seq: _SupportsSlicing[_T], n: int, strict: bool = ...
+) -> Iterator[_T]: ...
 def split_at(
     iterable: Iterable[_T],
     pred: Callable[[_T], object],
     maxsplit: int = ...,
     keep_separator: bool = ...,
-) -> Iterator[List[_T]]: ...
+) -> Iterator[list[_T]]: ...
 def split_before(
     iterable: Iterable[_T], pred: Callable[[_T], object], maxsplit: int = ...
-) -> Iterator[List[_T]]: ...
+) -> Iterator[list[_T]]: ...
 def split_after(
     iterable: Iterable[_T], pred: Callable[[_T], object], maxsplit: int = ...
-) -> Iterator[List[_T]]: ...
+) -> Iterator[list[_T]]: ...
 def split_when(
     iterable: Iterable[_T],
     pred: Callable[[_T, _T], object],
     maxsplit: int = ...,
-) -> Iterator[List[_T]]: ...
+) -> Iterator[list[_T]]: ...
 def split_into(
-    iterable: Iterable[_T], sizes: Iterable[Optional[int]]
-) -> Iterator[List[_T]]: ...
+    iterable: Iterable[_T], sizes: Iterable[int | None]
+) -> Iterator[list[_T]]: ...
 @overload
 def padded(
     iterable: Iterable[_T],
     *,
-    n: Optional[int] = ...,
+    n: int | None = ...,
     next_multiple: bool = ...,
-) -> Iterator[Optional[_T]]: ...
+) -> Iterator[_T | None]: ...
 @overload
 def padded(
     iterable: Iterable[_T],
     fillvalue: _U,
-    n: Optional[int] = ...,
+    n: int | None = ...,
     next_multiple: bool = ...,
-) -> Iterator[Union[_T, _U]]: ...
+) -> Iterator[_T | _U]: ...
 @overload
 def repeat_last(iterable: Iterable[_T]) -> Iterator[_T]: ...
 @overload
-def repeat_last(
-    iterable: Iterable[_T], default: _U
-) -> Iterator[Union[_T, _U]]: ...
-def distribute(n: int, iterable: Iterable[_T]) -> List[Iterator[_T]]: ...
+def repeat_last(iterable: Iterable[_T], default: _U) -> Iterator[_T | _U]: ...
+def distribute(n: int, iterable: Iterable[_T]) -> list[Iterator[_T]]: ...
 @overload
 def stagger(
     iterable: Iterable[_T],
     offsets: _SizedIterable[int] = ...,
     longest: bool = ...,
-) -> Iterator[Tuple[Optional[_T], ...]]: ...
+) -> Iterator[tuple[_T | None, ...]]: ...
 @overload
 def stagger(
     iterable: Iterable[_T],
     offsets: _SizedIterable[int] = ...,
     longest: bool = ...,
     fillvalue: _U = ...,
-) -> Iterator[Tuple[Union[_T, _U], ...]]: ...
+) -> Iterator[tuple[_T | _U, ...]]: ...
 
 class UnequalIterablesError(ValueError):
-    def __init__(
-        self, details: Optional[Tuple[int, int, int]] = ...
-    ) -> None: ...
+    def __init__(self, details: tuple[int, int, int] | None = ...) -> None: ...
 
 @overload
-def zip_equal(__iter1: Iterable[_T1]) -> Iterator[Tuple[_T1]]: ...
+def zip_equal(__iter1: Iterable[_T1]) -> Iterator[tuple[_T1]]: ...
 @overload
 def zip_equal(
     __iter1: Iterable[_T1], __iter2: Iterable[_T2]
-) -> Iterator[Tuple[_T1, _T2]]: ...
+) -> Iterator[tuple[_T1, _T2]]: ...
 @overload
 def zip_equal(
     __iter1: Iterable[_T],
     __iter2: Iterable[_T],
     __iter3: Iterable[_T],
     *iterables: Iterable[_T],
-) -> Iterator[Tuple[_T, ...]]: ...
+) -> Iterator[tuple[_T, ...]]: ...
 @overload
 def zip_offset(
     __iter1: Iterable[_T1],
     *,
     offsets: _SizedIterable[int],
     longest: bool = ...,
     fillvalue: None = None,
-) -> Iterator[Tuple[Optional[_T1]]]: ...
+) -> Iterator[tuple[_T1 | None]]: ...
 @overload
 def zip_offset(
     __iter1: Iterable[_T1],
     __iter2: Iterable[_T2],
     *,
     offsets: _SizedIterable[int],
     longest: bool = ...,
     fillvalue: None = None,
-) -> Iterator[Tuple[Optional[_T1], Optional[_T2]]]: ...
+) -> Iterator[tuple[_T1 | None, _T2 | None]]: ...
 @overload
 def zip_offset(
     __iter1: Iterable[_T],
     __iter2: Iterable[_T],
     __iter3: Iterable[_T],
     *iterables: Iterable[_T],
     offsets: _SizedIterable[int],
     longest: bool = ...,
     fillvalue: None = None,
-) -> Iterator[Tuple[Optional[_T], ...]]: ...
+) -> Iterator[tuple[_T | None, ...]]: ...
 @overload
 def zip_offset(
     __iter1: Iterable[_T1],
     *,
     offsets: _SizedIterable[int],
     longest: bool = ...,
     fillvalue: _U,
-) -> Iterator[Tuple[Union[_T1, _U]]]: ...
+) -> Iterator[tuple[_T1 | _U]]: ...
 @overload
 def zip_offset(
     __iter1: Iterable[_T1],
     __iter2: Iterable[_T2],
     *,
     offsets: _SizedIterable[int],
     longest: bool = ...,
     fillvalue: _U,
-) -> Iterator[Tuple[Union[_T1, _U], Union[_T2, _U]]]: ...
+) -> Iterator[tuple[_T1 | _U, _T2 | _U]]: ...
 @overload
 def zip_offset(
     __iter1: Iterable[_T],
     __iter2: Iterable[_T],
     __iter3: Iterable[_T],
     *iterables: Iterable[_T],
     offsets: _SizedIterable[int],
     longest: bool = ...,
     fillvalue: _U,
-) -> Iterator[Tuple[Union[_T, _U], ...]]: ...
+) -> Iterator[tuple[_T | _U, ...]]: ...
 def sort_together(
     iterables: Iterable[Iterable[_T]],
     key_list: Iterable[int] = ...,
-    key: Optional[Callable[..., Any]] = ...,
+    key: Callable[..., Any] | None = ...,
     reverse: bool = ...,
-) -> List[Tuple[_T, ...]]: ...
-def unzip(iterable: Iterable[Sequence[_T]]) -> Tuple[Iterator[_T], ...]: ...
-def divide(n: int, iterable: Iterable[_T]) -> List[Iterator[_T]]: ...
+) -> list[tuple[_T, ...]]: ...
+def unzip(iterable: Iterable[Sequence[_T]]) -> tuple[Iterator[_T], ...]: ...
+def divide(n: int, iterable: Iterable[_T]) -> list[Iterator[_T]]: ...
 def always_iterable(
     obj: object,
-    base_type: Union[
-        type, Tuple[Union[type, Tuple[Any, ...]], ...], None
-    ] = ...,
+    base_type: type | tuple[type | tuple[Any, ...], ...] | None = ...,
 ) -> Iterator[Any]: ...
 def adjacent(
     predicate: Callable[[_T], bool],
     iterable: Iterable[_T],
     distance: int = ...,
-) -> Iterator[Tuple[bool, _T]]: ...
+) -> Iterator[tuple[bool, _T]]: ...
 @overload
 def groupby_transform(
     iterable: Iterable[_T],
     keyfunc: None = None,
     valuefunc: None = None,
     reducefunc: None = None,
-) -> Iterator[Tuple[_T, Iterator[_T]]]: ...
+) -> Iterator[tuple[_T, Iterator[_T]]]: ...
 @overload
 def groupby_transform(
     iterable: Iterable[_T],
     keyfunc: Callable[[_T], _U],
     valuefunc: None,
     reducefunc: None,
-) -> Iterator[Tuple[_U, Iterator[_T]]]: ...
+) -> Iterator[tuple[_U, Iterator[_T]]]: ...
 @overload
 def groupby_transform(
     iterable: Iterable[_T],
     keyfunc: None,
     valuefunc: Callable[[_T], _V],
     reducefunc: None,
-) -> Iterable[Tuple[_T, Iterable[_V]]]: ...
+) -> Iterable[tuple[_T, Iterable[_V]]]: ...
 @overload
 def groupby_transform(
     iterable: Iterable[_T],
     keyfunc: Callable[[_T], _U],
     valuefunc: Callable[[_T], _V],
     reducefunc: None,
-) -> Iterable[Tuple[_U, Iterator[_V]]]: ...
+) -> Iterable[tuple[_U, Iterator[_V]]]: ...
 @overload
 def groupby_transform(
     iterable: Iterable[_T],
     keyfunc: None,
     valuefunc: None,
     reducefunc: Callable[[Iterator[_T]], _W],
-) -> Iterable[Tuple[_T, _W]]: ...
+) -> Iterable[tuple[_T, _W]]: ...
 @overload
 def groupby_transform(
     iterable: Iterable[_T],
     keyfunc: Callable[[_T], _U],
     valuefunc: None,
     reducefunc: Callable[[Iterator[_T]], _W],
-) -> Iterable[Tuple[_U, _W]]: ...
+) -> Iterable[tuple[_U, _W]]: ...
 @overload
 def groupby_transform(
     iterable: Iterable[_T],
     keyfunc: None,
     valuefunc: Callable[[_T], _V],
     reducefunc: Callable[[Iterable[_V]], _W],
-) -> Iterable[Tuple[_T, _W]]: ...
+) -> Iterable[tuple[_T, _W]]: ...
 @overload
 def groupby_transform(
     iterable: Iterable[_T],
     keyfunc: Callable[[_T], _U],
     valuefunc: Callable[[_T], _V],
     reducefunc: Callable[[Iterable[_V]], _W],
-) -> Iterable[Tuple[_U, _W]]: ...
+) -> Iterable[tuple[_U, _W]]: ...
 
 class numeric_range(Generic[_T, _U], Sequence[_T], Hashable, Reversible[_T]):
     @overload
     def __init__(self, __stop: _T) -> None: ...
     @overload
     def __init__(self, __start: _T, __stop: _T) -> None: ...
     @overload
@@ -371,60 +366,58 @@
     @overload
     def __getitem__(self, key: slice) -> numeric_range[_T, _U]: ...
     def __hash__(self) -> int: ...
     def __iter__(self) -> Iterator[_T]: ...
     def __len__(self) -> int: ...
     def __reduce__(
         self,
-    ) -> Tuple[Type[numeric_range[_T, _U]], Tuple[_T, _T, _U]]: ...
+    ) -> tuple[Type[numeric_range[_T, _U]], tuple[_T, _T, _U]]: ...
     def __repr__(self) -> str: ...
     def __reversed__(self) -> Iterator[_T]: ...
     def count(self, value: _T) -> int: ...
     def index(self, value: _T) -> int: ...  # type: ignore
 
 def count_cycle(
-    iterable: Iterable[_T], n: Optional[int] = ...
-) -> Iterable[Tuple[int, _T]]: ...
+    iterable: Iterable[_T], n: int | None = ...
+) -> Iterable[tuple[int, _T]]: ...
 def mark_ends(
     iterable: Iterable[_T],
-) -> Iterable[Tuple[bool, bool, _T]]: ...
+) -> Iterable[tuple[bool, bool, _T]]: ...
 def locate(
     iterable: Iterable[object],
     pred: Callable[..., Any] = ...,
-    window_size: Optional[int] = ...,
+    window_size: int | None = ...,
 ) -> Iterator[int]: ...
 def lstrip(
     iterable: Iterable[_T], pred: Callable[[_T], object]
 ) -> Iterator[_T]: ...
 def rstrip(
     iterable: Iterable[_T], pred: Callable[[_T], object]
 ) -> Iterator[_T]: ...
 def strip(
     iterable: Iterable[_T], pred: Callable[[_T], object]
 ) -> Iterator[_T]: ...
 
 class islice_extended(Generic[_T], Iterator[_T]):
-    def __init__(
-        self, iterable: Iterable[_T], *args: Optional[int]
-    ) -> None: ...
+    def __init__(self, iterable: Iterable[_T], *args: int | None) -> None: ...
     def __iter__(self) -> islice_extended[_T]: ...
     def __next__(self) -> _T: ...
     def __getitem__(self, index: slice) -> islice_extended[_T]: ...
 
 def always_reversible(iterable: Iterable[_T]) -> Iterator[_T]: ...
 def consecutive_groups(
     iterable: Iterable[_T], ordering: Callable[[_T], int] = ...
 ) -> Iterator[Iterator[_T]]: ...
 @overload
 def difference(
     iterable: Iterable[_T],
     func: Callable[[_T, _T], _U] = ...,
     *,
     initial: None = ...,
-) -> Iterator[Union[_T, _U]]: ...
+) -> Iterator[_T | _U]: ...
 @overload
 def difference(
     iterable: Iterable[_T], func: Callable[[_T, _T], _U] = ..., *, initial: _U
 ) -> Iterator[_U]: ...
 
 class SequenceView(Generic[_T], Sequence[_T]):
     def __init__(self, target: Sequence[_T]) -> None: ...
@@ -432,127 +425,127 @@
     def __getitem__(self, index: int) -> _T: ...
     @overload
     def __getitem__(self, index: slice) -> Sequence[_T]: ...
     def __len__(self) -> int: ...
 
 class seekable(Generic[_T], Iterator[_T]):
     def __init__(
-        self, iterable: Iterable[_T], maxlen: Optional[int] = ...
+        self, iterable: Iterable[_T], maxlen: int | None = ...
     ) -> None: ...
     def __iter__(self) -> seekable[_T]: ...
     def __next__(self) -> _T: ...
     def __bool__(self) -> bool: ...
     @overload
     def peek(self) -> _T: ...
     @overload
-    def peek(self, default: _U) -> Union[_T, _U]: ...
+    def peek(self, default: _U) -> _T | _U: ...
     def elements(self) -> SequenceView[_T]: ...
     def seek(self, index: int) -> None: ...
 
 class run_length:
     @staticmethod
-    def encode(iterable: Iterable[_T]) -> Iterator[Tuple[_T, int]]: ...
+    def encode(iterable: Iterable[_T]) -> Iterator[tuple[_T, int]]: ...
     @staticmethod
-    def decode(iterable: Iterable[Tuple[_T, int]]) -> Iterator[_T]: ...
+    def decode(iterable: Iterable[tuple[_T, int]]) -> Iterator[_T]: ...
 
 def exactly_n(
     iterable: Iterable[_T], n: int, predicate: Callable[[_T], object] = ...
 ) -> bool: ...
-def circular_shifts(iterable: Iterable[_T]) -> List[Tuple[_T, ...]]: ...
+def circular_shifts(iterable: Iterable[_T]) -> list[tuple[_T, ...]]: ...
 def make_decorator(
     wrapping_func: Callable[..., _U], result_index: int = ...
 ) -> Callable[..., Callable[[Callable[..., Any]], Callable[..., _U]]]: ...
 @overload
 def map_reduce(
     iterable: Iterable[_T],
     keyfunc: Callable[[_T], _U],
     valuefunc: None = ...,
     reducefunc: None = ...,
-) -> Dict[_U, List[_T]]: ...
+) -> dict[_U, list[_T]]: ...
 @overload
 def map_reduce(
     iterable: Iterable[_T],
     keyfunc: Callable[[_T], _U],
     valuefunc: Callable[[_T], _V],
     reducefunc: None = ...,
-) -> Dict[_U, List[_V]]: ...
+) -> dict[_U, list[_V]]: ...
 @overload
 def map_reduce(
     iterable: Iterable[_T],
     keyfunc: Callable[[_T], _U],
     valuefunc: None = ...,
-    reducefunc: Callable[[List[_T]], _W] = ...,
-) -> Dict[_U, _W]: ...
+    reducefunc: Callable[[list[_T]], _W] = ...,
+) -> dict[_U, _W]: ...
 @overload
 def map_reduce(
     iterable: Iterable[_T],
     keyfunc: Callable[[_T], _U],
     valuefunc: Callable[[_T], _V],
-    reducefunc: Callable[[List[_V]], _W],
-) -> Dict[_U, _W]: ...
+    reducefunc: Callable[[list[_V]], _W],
+) -> dict[_U, _W]: ...
 def rlocate(
     iterable: Iterable[_T],
     pred: Callable[..., object] = ...,
-    window_size: Optional[int] = ...,
+    window_size: int | None = ...,
 ) -> Iterator[int]: ...
 def replace(
     iterable: Iterable[_T],
     pred: Callable[..., object],
     substitutes: Iterable[_U],
-    count: Optional[int] = ...,
+    count: int | None = ...,
     window_size: int = ...,
-) -> Iterator[Union[_T, _U]]: ...
-def partitions(iterable: Iterable[_T]) -> Iterator[List[List[_T]]]: ...
+) -> Iterator[_T | _U]: ...
+def partitions(iterable: Iterable[_T]) -> Iterator[list[list[_T]]]: ...
 def set_partitions(
-    iterable: Iterable[_T], k: Optional[int] = ...
-) -> Iterator[List[List[_T]]]: ...
+    iterable: Iterable[_T], k: int | None = ...
+) -> Iterator[list[list[_T]]]: ...
 
 class time_limited(Generic[_T], Iterator[_T]):
     def __init__(
         self, limit_seconds: float, iterable: Iterable[_T]
     ) -> None: ...
     def __iter__(self) -> islice_extended[_T]: ...
     def __next__(self) -> _T: ...
 
 @overload
 def only(
-    iterable: Iterable[_T], *, too_long: Optional[_Raisable] = ...
-) -> Optional[_T]: ...
+    iterable: Iterable[_T], *, too_long: _Raisable | None = ...
+) -> _T | None: ...
 @overload
 def only(
-    iterable: Iterable[_T], default: _U, too_long: Optional[_Raisable] = ...
-) -> Union[_T, _U]: ...
+    iterable: Iterable[_T], default: _U, too_long: _Raisable | None = ...
+) -> _T | _U: ...
 def ichunked(iterable: Iterable[_T], n: int) -> Iterator[Iterator[_T]]: ...
 def distinct_combinations(
     iterable: Iterable[_T], r: int
-) -> Iterator[Tuple[_T, ...]]: ...
+) -> Iterator[tuple[_T, ...]]: ...
 def filter_except(
     validator: Callable[[Any], object],
     iterable: Iterable[_T],
     *exceptions: Type[BaseException],
 ) -> Iterator[_T]: ...
 def map_except(
     function: Callable[[Any], _U],
     iterable: Iterable[_T],
     *exceptions: Type[BaseException],
 ) -> Iterator[_U]: ...
 def map_if(
     iterable: Iterable[Any],
     pred: Callable[[Any], bool],
     func: Callable[[Any], Any],
-    func_else: Optional[Callable[[Any], Any]] = ...,
+    func_else: Callable[[Any], Any] | None = ...,
 ) -> Iterator[Any]: ...
 def sample(
     iterable: Iterable[_T],
     k: int,
-    weights: Optional[Iterable[float]] = ...,
-) -> List[_T]: ...
+    weights: Iterable[float] | None = ...,
+) -> list[_T]: ...
 def is_sorted(
     iterable: Iterable[_T],
-    key: Optional[Callable[[_T], _U]] = ...,
+    key: Callable[[_T], _U] | None = ...,
     reverse: bool = False,
     strict: bool = False,
 ) -> bool: ...
 
 class AbortThread(BaseException):
     pass
 
@@ -562,113 +555,112 @@
         func: Callable[..., Any],
         callback_kwd: str = ...,
         wait_seconds: float = ...,
     ) -> None: ...
     def __enter__(self) -> callback_iter[_T]: ...
     def __exit__(
         self,
-        exc_type: Optional[Type[BaseException]],
-        exc_value: Optional[BaseException],
-        traceback: Optional[TracebackType],
-    ) -> Optional[bool]: ...
+        exc_type: Type[BaseException] | None,
+        exc_value: BaseException | None,
+        traceback: TracebackType | None,
+    ) -> bool | None: ...
     def __iter__(self) -> callback_iter[_T]: ...
     def __next__(self) -> _T: ...
     def _reader(self) -> Iterator[_T]: ...
     @property
     def done(self) -> bool: ...
     @property
     def result(self) -> Any: ...
 
 def windowed_complete(
     iterable: Iterable[_T], n: int
-) -> Iterator[Tuple[_T, ...]]: ...
+) -> Iterator[tuple[_T, ...]]: ...
 def all_unique(
-    iterable: Iterable[_T], key: Optional[Callable[[_T], _U]] = ...
+    iterable: Iterable[_T], key: Callable[[_T], _U] | None = ...
 ) -> bool: ...
-def nth_product(index: int, *args: Iterable[_T]) -> Tuple[_T, ...]: ...
+def nth_product(index: int, *args: Iterable[_T]) -> tuple[_T, ...]: ...
 def nth_permutation(
     iterable: Iterable[_T], r: int, index: int
-) -> Tuple[_T, ...]: ...
-def value_chain(*args: Union[_T, Iterable[_T]]) -> Iterable[_T]: ...
+) -> tuple[_T, ...]: ...
+def value_chain(*args: _T | Iterable[_T]) -> Iterable[_T]: ...
 def product_index(element: Iterable[_T], *args: Iterable[_T]) -> int: ...
 def combination_index(
     element: Iterable[_T], iterable: Iterable[_T]
 ) -> int: ...
 def permutation_index(
     element: Iterable[_T], iterable: Iterable[_T]
 ) -> int: ...
 def repeat_each(iterable: Iterable[_T], n: int = ...) -> Iterator[_T]: ...
 
 class countable(Generic[_T], Iterator[_T]):
     def __init__(self, iterable: Iterable[_T]) -> None: ...
     def __iter__(self) -> countable[_T]: ...
     def __next__(self) -> _T: ...
 
-def chunked_even(iterable: Iterable[_T], n: int) -> Iterator[List[_T]]: ...
+def chunked_even(iterable: Iterable[_T], n: int) -> Iterator[list[_T]]: ...
 def zip_broadcast(
-    *objects: Union[_T, Iterable[_T]],
-    scalar_types: Union[
-        type, Tuple[Union[type, Tuple[Any, ...]], ...], None
-    ] = ...,
+    *objects: _T | Iterable[_T],
+    scalar_types: type | tuple[type | tuple[Any, ...], ...] | None = ...,
     strict: bool = ...,
-) -> Iterable[Tuple[_T, ...]]: ...
+) -> Iterable[tuple[_T, ...]]: ...
 def unique_in_window(
-    iterable: Iterable[_T], n: int, key: Optional[Callable[[_T], _U]] = ...
+    iterable: Iterable[_T], n: int, key: Callable[[_T], _U] | None = ...
 ) -> Iterator[_T]: ...
 def duplicates_everseen(
-    iterable: Iterable[_T], key: Optional[Callable[[_T], _U]] = ...
+    iterable: Iterable[_T], key: Callable[[_T], _U] | None = ...
 ) -> Iterator[_T]: ...
 def duplicates_justseen(
-    iterable: Iterable[_T], key: Optional[Callable[[_T], _U]] = ...
+    iterable: Iterable[_T], key: Callable[[_T], _U] | None = ...
 ) -> Iterator[_T]: ...
 
 class _SupportsLessThan(Protocol):
     def __lt__(self, __other: Any) -> bool: ...
 
 _SupportsLessThanT = TypeVar("_SupportsLessThanT", bound=_SupportsLessThan)
 
 @overload
 def minmax(
     iterable_or_value: Iterable[_SupportsLessThanT], *, key: None = None
-) -> Tuple[_SupportsLessThanT, _SupportsLessThanT]: ...
+) -> tuple[_SupportsLessThanT, _SupportsLessThanT]: ...
 @overload
 def minmax(
     iterable_or_value: Iterable[_T], *, key: Callable[[_T], _SupportsLessThan]
-) -> Tuple[_T, _T]: ...
+) -> tuple[_T, _T]: ...
 @overload
 def minmax(
     iterable_or_value: Iterable[_SupportsLessThanT],
     *,
     key: None = None,
     default: _U,
-) -> Union[_U, Tuple[_SupportsLessThanT, _SupportsLessThanT]]: ...
+) -> _U | tuple[_SupportsLessThanT, _SupportsLessThanT]: ...
 @overload
 def minmax(
     iterable_or_value: Iterable[_T],
     *,
     key: Callable[[_T], _SupportsLessThan],
     default: _U,
-) -> Union[_U, Tuple[_T, _T]]: ...
+) -> _U | tuple[_T, _T]: ...
 @overload
 def minmax(
     iterable_or_value: _SupportsLessThanT,
     __other: _SupportsLessThanT,
     *others: _SupportsLessThanT,
-) -> Tuple[_SupportsLessThanT, _SupportsLessThanT]: ...
+) -> tuple[_SupportsLessThanT, _SupportsLessThanT]: ...
 @overload
 def minmax(
     iterable_or_value: _T,
     __other: _T,
     *others: _T,
     key: Callable[[_T], _SupportsLessThan],
-) -> Tuple[_T, _T]: ...
+) -> tuple[_T, _T]: ...
 def longest_common_prefix(
     iterables: Iterable[Iterable[_T]],
 ) -> Iterator[_T]: ...
 def iequals(*iterables: Iterable[object]) -> bool: ...
 def constrained_batches(
     iterable: Iterable[object],
     max_size: int,
-    max_count: Optional[int] = ...,
+    max_count: int | None = ...,
     get_len: Callable[[_T], object] = ...,
     strict: bool = ...,
-) -> Iterator[Tuple[_T]]: ...
+) -> Iterator[tuple[_T]]: ...
+def gray_product(*iterables: Iterable[_T]) -> Iterator[tuple[_T, ...]]: ...
```

### Comparing `more-itertools-9.0.0/more_itertools/recipes.py` & `more-itertools-9.1.0/more_itertools/recipes.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,44 +5,50 @@
 Some backward-compatible usability improvements have been made.
 
 .. [1] http://docs.python.org/library/itertools.html#recipes
 
 """
 import math
 import operator
+import warnings
 
 from collections import deque
 from collections.abc import Sized
 from functools import reduce
 from itertools import (
     chain,
     combinations,
     compress,
     count,
     cycle,
     groupby,
     islice,
+    product,
     repeat,
     starmap,
     tee,
     zip_longest,
 )
 from random import randrange, sample, choice
+from sys import hexversion
 
 __all__ = [
     'all_equal',
     'batched',
     'before_and_after',
     'consume',
     'convolve',
     'dotproduct',
     'first_true',
+    'factor',
     'flatten',
     'grouper',
     'iter_except',
+    'iter_index',
+    'matmul',
     'ncycles',
     'nth',
     'nth_combination',
     'padnone',
     'pad_none',
     'pairwise',
     'partition',
@@ -58,14 +64,15 @@
     'roundrobin',
     'sieve',
     'sliding_window',
     'subslices',
     'tabulate',
     'tail',
     'take',
+    'transpose',
     'triplewise',
     'unique_everseen',
     'unique_justseen',
 ]
 
 _marker = object()
 
@@ -804,38 +811,120 @@
     prod = getattr(math, 'prod', lambda x: reduce(operator.mul, x, 1))
     roots = list(map(operator.neg, roots))
     return [
         sum(map(prod, combinations(roots, k))) for k in range(len(roots) + 1)
     ]
 
 
+def iter_index(iterable, value, start=0):
+    """Yield the index of each place in *iterable* that *value* occurs,
+    beginning with index *start*.
+
+    See :func:`locate` for a more general means of finding the indexes
+    associated with particular values.
+
+    >>> list(iter_index('AABCADEAF', 'A'))
+    [0, 1, 4, 7]
+    """
+    try:
+        seq_index = iterable.index
+    except AttributeError:
+        # Slow path for general iterables
+        it = islice(iterable, start, None)
+        for i, element in enumerate(it, start):
+            if element is value or element == value:
+                yield i
+    else:
+        # Fast path for sequences
+        i = start - 1
+        try:
+            while True:
+                i = seq_index(value, i + 1)
+                yield i
+        except ValueError:
+            pass
+
+
 def sieve(n):
     """Yield the primes less than n.
 
     >>> list(sieve(30))
     [2, 3, 5, 7, 11, 13, 17, 19, 23, 29]
     """
     isqrt = getattr(math, 'isqrt', lambda x: int(math.sqrt(x)))
+    data = bytearray((0, 1)) * (n // 2)
+    data[:3] = 0, 0, 0
     limit = isqrt(n) + 1
-    data = bytearray([1]) * n
-    data[:2] = 0, 0
     for p in compress(range(limit), data):
-        data[p + p : n : p] = bytearray(len(range(p + p, n, p)))
-
-    return compress(count(), data)
+        data[p * p : n : p + p] = bytes(len(range(p * p, n, p + p)))
+    data[2] = 1
+    return iter_index(data, 1) if n > 2 else iter([])
 
 
 def batched(iterable, n):
     """Batch data into lists of length *n*. The last batch may be shorter.
 
     >>> list(batched('ABCDEFG', 3))
     [['A', 'B', 'C'], ['D', 'E', 'F'], ['G']]
 
     This recipe is from the ``itertools`` docs. This library also provides
     :func:`chunked`, which has a different implementation.
     """
+    if hexversion >= 0x30C00A0:  # Python 3.12.0a0
+        warnings.warn(
+            (
+                'batched will be removed in a future version of '
+                'more-itertools. Use the standard library '
+                'itertools.batched function instead'
+            ),
+            DeprecationWarning,
+        )
+
     it = iter(iterable)
     while True:
         batch = list(islice(it, n))
         if not batch:
             break
         yield batch
+
+
+def transpose(it):
+    """Swap the rows and columns of the input.
+
+    >>> list(transpose([(1, 2, 3), (11, 22, 33)]))
+    [(1, 11), (2, 22), (3, 33)]
+
+    The caller should ensure that the dimensions of the input are compatible.
+    """
+    # TODO: when 3.9 goes end-of-life, add stric=True to this.
+    return zip(*it)
+
+
+def matmul(m1, m2):
+    """Multiply two matrices.
+    >>> list(matmul([(7, 5), (3, 5)], [(2, 5), (7, 9)]))
+    [[49, 80], [41, 60]]
+
+    The caller should ensure that the dimensions of the input matrices are
+    compatible with each other.
+    """
+    n = len(m2[0])
+    return batched(starmap(dotproduct, product(m1, transpose(m2))), n)
+
+
+def factor(n):
+    """Yield the prime factors of n.
+    >>> list(factor(360))
+    [2, 2, 2, 3, 3, 5]
+    """
+    isqrt = getattr(math, 'isqrt', lambda x: int(math.sqrt(x)))
+    for prime in sieve(isqrt(n) + 1):
+        while True:
+            quotient, remainder = divmod(n, prime)
+            if remainder:
+                break
+            yield prime
+            n = quotient
+            if n == 1:
+                return
+    if n >= 2:
+        yield n
```

### Comparing `more-itertools-9.0.0/more_itertools/recipes.pyi` & `more-itertools-9.1.0/more_itertools/recipes.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,110 +1,119 @@
 """Stubs for more_itertools.recipes"""
+from __future__ import annotations
+
 from typing import (
     Any,
     Callable,
     Iterable,
     Iterator,
-    List,
-    Optional,
+    overload,
     Sequence,
-    Tuple,
+    Type,
     TypeVar,
-    Union,
 )
-from typing_extensions import overload, Type
 
 # Type and type variable definitions
 _T = TypeVar('_T')
 _U = TypeVar('_U')
 
-def take(n: int, iterable: Iterable[_T]) -> List[_T]: ...
+def take(n: int, iterable: Iterable[_T]) -> list[_T]: ...
 def tabulate(
     function: Callable[[int], _T], start: int = ...
 ) -> Iterator[_T]: ...
 def tail(n: int, iterable: Iterable[_T]) -> Iterator[_T]: ...
-def consume(iterator: Iterable[object], n: Optional[int] = ...) -> None: ...
+def consume(iterator: Iterable[object], n: int | None = ...) -> None: ...
 @overload
-def nth(iterable: Iterable[_T], n: int) -> Optional[_T]: ...
+def nth(iterable: Iterable[_T], n: int) -> _T | None: ...
 @overload
-def nth(iterable: Iterable[_T], n: int, default: _U) -> Union[_T, _U]: ...
+def nth(iterable: Iterable[_T], n: int, default: _U) -> _T | _U: ...
 def all_equal(iterable: Iterable[object]) -> bool: ...
 def quantify(
     iterable: Iterable[_T], pred: Callable[[_T], bool] = ...
 ) -> int: ...
-def pad_none(iterable: Iterable[_T]) -> Iterator[Optional[_T]]: ...
-def padnone(iterable: Iterable[_T]) -> Iterator[Optional[_T]]: ...
+def pad_none(iterable: Iterable[_T]) -> Iterator[_T | None]: ...
+def padnone(iterable: Iterable[_T]) -> Iterator[_T | None]: ...
 def ncycles(iterable: Iterable[_T], n: int) -> Iterator[_T]: ...
 def dotproduct(vec1: Iterable[object], vec2: Iterable[object]) -> object: ...
 def flatten(listOfLists: Iterable[Iterable[_T]]) -> Iterator[_T]: ...
 def repeatfunc(
-    func: Callable[..., _U], times: Optional[int] = ..., *args: Any
+    func: Callable[..., _U], times: int | None = ..., *args: Any
 ) -> Iterator[_U]: ...
-def pairwise(iterable: Iterable[_T]) -> Iterator[Tuple[_T, _T]]: ...
+def pairwise(iterable: Iterable[_T]) -> Iterator[tuple[_T, _T]]: ...
 def grouper(
     iterable: Iterable[_T],
     n: int,
     incomplete: str = ...,
     fillvalue: _U = ...,
-) -> Iterator[Tuple[Union[_T, _U], ...]]: ...
+) -> Iterator[tuple[_T | _U, ...]]: ...
 def roundrobin(*iterables: Iterable[_T]) -> Iterator[_T]: ...
 def partition(
-    pred: Optional[Callable[[_T], object]], iterable: Iterable[_T]
-) -> Tuple[Iterator[_T], Iterator[_T]]: ...
-def powerset(iterable: Iterable[_T]) -> Iterator[Tuple[_T, ...]]: ...
+    pred: Callable[[_T], object] | None, iterable: Iterable[_T]
+) -> tuple[Iterator[_T], Iterator[_T]]: ...
+def powerset(iterable: Iterable[_T]) -> Iterator[tuple[_T, ...]]: ...
 def unique_everseen(
-    iterable: Iterable[_T], key: Optional[Callable[[_T], _U]] = ...
+    iterable: Iterable[_T], key: Callable[[_T], _U] | None = ...
 ) -> Iterator[_T]: ...
 def unique_justseen(
-    iterable: Iterable[_T], key: Optional[Callable[[_T], object]] = ...
+    iterable: Iterable[_T], key: Callable[[_T], object] | None = ...
 ) -> Iterator[_T]: ...
 @overload
 def iter_except(
     func: Callable[[], _T],
-    exception: Union[Type[BaseException], Tuple[Type[BaseException], ...]],
+    exception: Type[BaseException] | tuple[Type[BaseException], ...],
     first: None = ...,
 ) -> Iterator[_T]: ...
 @overload
 def iter_except(
     func: Callable[[], _T],
-    exception: Union[Type[BaseException], Tuple[Type[BaseException], ...]],
+    exception: Type[BaseException] | tuple[Type[BaseException], ...],
     first: Callable[[], _U],
-) -> Iterator[Union[_T, _U]]: ...
+) -> Iterator[_T | _U]: ...
 @overload
 def first_true(
-    iterable: Iterable[_T], *, pred: Optional[Callable[[_T], object]] = ...
-) -> Optional[_T]: ...
+    iterable: Iterable[_T], *, pred: Callable[[_T], object] | None = ...
+) -> _T | None: ...
 @overload
 def first_true(
     iterable: Iterable[_T],
     default: _U,
-    pred: Optional[Callable[[_T], object]] = ...,
-) -> Union[_T, _U]: ...
+    pred: Callable[[_T], object] | None = ...,
+) -> _T | _U: ...
 def random_product(
     *args: Iterable[_T], repeat: int = ...
-) -> Tuple[_T, ...]: ...
+) -> tuple[_T, ...]: ...
 def random_permutation(
-    iterable: Iterable[_T], r: Optional[int] = ...
-) -> Tuple[_T, ...]: ...
-def random_combination(iterable: Iterable[_T], r: int) -> Tuple[_T, ...]: ...
+    iterable: Iterable[_T], r: int | None = ...
+) -> tuple[_T, ...]: ...
+def random_combination(iterable: Iterable[_T], r: int) -> tuple[_T, ...]: ...
 def random_combination_with_replacement(
     iterable: Iterable[_T], r: int
-) -> Tuple[_T, ...]: ...
+) -> tuple[_T, ...]: ...
 def nth_combination(
     iterable: Iterable[_T], r: int, index: int
-) -> Tuple[_T, ...]: ...
-def prepend(value: _T, iterator: Iterable[_U]) -> Iterator[Union[_T, _U]]: ...
+) -> tuple[_T, ...]: ...
+def prepend(value: _T, iterator: Iterable[_U]) -> Iterator[_T | _U]: ...
 def convolve(signal: Iterable[_T], kernel: Iterable[_T]) -> Iterator[_T]: ...
 def before_and_after(
     predicate: Callable[[_T], bool], it: Iterable[_T]
-) -> Tuple[Iterator[_T], Iterator[_T]]: ...
-def triplewise(iterable: Iterable[_T]) -> Iterator[Tuple[_T, _T, _T]]: ...
+) -> tuple[Iterator[_T], Iterator[_T]]: ...
+def triplewise(iterable: Iterable[_T]) -> Iterator[tuple[_T, _T, _T]]: ...
 def sliding_window(
     iterable: Iterable[_T], n: int
-) -> Iterator[Tuple[_T, ...]]: ...
-def subslices(iterable: Iterable[_T]) -> Iterator[List[_T]]: ...
-def polynomial_from_roots(roots: Sequence[int]) -> List[int]: ...
+) -> Iterator[tuple[_T, ...]]: ...
+def subslices(iterable: Iterable[_T]) -> Iterator[list[_T]]: ...
+def polynomial_from_roots(roots: Sequence[int]) -> list[int]: ...
+def iter_index(
+    iterable: Iterable[object],
+    value: Any,
+    start: int | None = ...,
+) -> Iterator[int]: ...
 def sieve(n: int) -> Iterator[int]: ...
 def batched(
     iterable: Iterable[_T],
     n: int,
-) -> Iterator[List[_T]]: ...
+) -> Iterator[list[_T]]: ...
+def transpose(
+    it: Iterable[Iterable[_T]],
+) -> tuple[Iterator[_T], ...]: ...
+def matmul(m1: Sequence[_T], m2: Sequence[_T]) -> Iterator[list[_T]]: ...
+def factor(n: int) -> Iterator[int]: ...
```

### Comparing `more-itertools-9.0.0/pyproject.toml` & `more-itertools-9.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `more-itertools-9.0.0/setup.cfg` & `more-itertools-9.1.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 9.0.0
+current_version = 9.1.0
 commit = True
 tag = False
 files = more_itertools/__init__.py
 
 [flake8]
 exclude = ./docs/conf.py, .eggs/
 ignore = E203, E731, E741, F999, W503
```

### Comparing `more-itertools-9.0.0/tests/test_more.py` & `more-itertools-9.1.0/tests/test_more.py`

 * *Files 1% similar despite different names*

```diff
@@ -1444,14 +1444,18 @@
                 ('a,b,c,d', lambda c: c == '@', 2),
                 [['a', ',', 'b', ',', 'c', ',', 'd']],
             ),
             (
                 ('a,b,c,d', lambda c: c != ',', 2),
                 [['a'], [',', 'b'], [',', 'c', ',', 'd']],
             ),
+            (
+                ([1], lambda x: x == 1, 1),
+                [[1]],
+            ),
         ]:
             actual = list(mi.split_after(*args))
             self.assertEqual(actual, expected)
 
 
 class SplitWhenTests(TestCase):
     """Tests for ``split_when()``"""
@@ -5170,7 +5174,57 @@
             list(
                 mi.constrained_batches(
                     iterable, 10, get_len=lambda x: x.total_size()
                 )
             ),
             [(record_3, record_5), (record_10,), (record_2,)],
         )
+
+
+class GrayProductTests(TestCase):
+    def test_basic(self):
+        self.assertEqual(
+            tuple(mi.gray_product(('a', 'b', 'c'), range(1, 3))),
+            (("a", 1), ("b", 1), ("c", 1), ("c", 2), ("b", 2), ("a", 2)),
+        )
+        out = mi.gray_product(('foo', 'bar'), (3, 4, 5, 6), ['quz', 'baz'])
+        self.assertEqual(next(out), ('foo', 3, 'quz'))
+        self.assertEqual(
+            list(out),
+            [
+                ('bar', 3, 'quz'),
+                ('bar', 4, 'quz'),
+                ('foo', 4, 'quz'),
+                ('foo', 5, 'quz'),
+                ('bar', 5, 'quz'),
+                ('bar', 6, 'quz'),
+                ('foo', 6, 'quz'),
+                ('foo', 6, 'baz'),
+                ('bar', 6, 'baz'),
+                ('bar', 5, 'baz'),
+                ('foo', 5, 'baz'),
+                ('foo', 4, 'baz'),
+                ('bar', 4, 'baz'),
+                ('bar', 3, 'baz'),
+                ('foo', 3, 'baz'),
+            ],
+        )
+        self.assertEqual(tuple(mi.gray_product()), ((),))
+        self.assertEqual(tuple(mi.gray_product((1, 2))), ((1,), (2,)))
+
+    def test_errors(self):
+        with self.assertRaises(ValueError):
+            list(mi.gray_product((1, 2), ()))
+        with self.assertRaises(ValueError):
+            list(mi.gray_product((1, 2), (2,)))
+
+    def test_vs_product(self):
+        iters = (
+            ("a", "b"),
+            range(3, 6),
+            [None, None],
+            {"i", "j", "k", "l"},
+            "XYZ",
+        )
+        self.assertEqual(
+            sorted(product(*iters)), sorted(mi.gray_product(*iters))
+        )
```

### Comparing `more-itertools-9.0.0/tests/test_recipes.py` & `more-itertools-9.1.0/tests/test_recipes.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from doctest import DocTestSuite
 from functools import reduce
 from itertools import combinations, count, permutations
+from operator import mul
 from math import factorial
 from unittest import TestCase
 
 import more_itertools as mi
 
 
 def load_tests(loader, tests, ignore):
@@ -876,14 +877,43 @@
             ((2, 4, 1), [1, -7, 14, -8]),
         ]:
             with self.subTest(roots=roots):
                 actual = mi.polynomial_from_roots(roots)
                 self.assertEqual(actual, expected)
 
 
+class IterIndexTests(TestCase):
+    def test_basic(self):
+        iterable = 'AABCADEAF'
+        for wrapper in (list, iter):
+            with self.subTest(wrapper=wrapper):
+                actual = list(mi.iter_index(wrapper(iterable), 'A'))
+                expected = [0, 1, 4, 7]
+                self.assertEqual(actual, expected)
+
+    def test_start(self):
+        for wrapper in (list, iter):
+            with self.subTest(wrapper=wrapper):
+                iterable = 'AABCADEAF'
+                i = -1
+                actual = []
+                while True:
+                    try:
+                        i = next(
+                            mi.iter_index(wrapper(iterable), 'A', start=i + 1)
+                        )
+                    except StopIteration:
+                        break
+                    else:
+                        actual.append(i)
+
+                expected = [0, 1, 4, 7]
+                self.assertEqual(actual, expected)
+
+
 class SieveTests(TestCase):
     def test_basic(self):
         self.assertEqual(
             list(mi.sieve(67)),
             [
                 2,
                 3,
@@ -938,7 +968,76 @@
             (4, [[1, 2, 3, 4], [5]]),
             (5, [[1, 2, 3, 4, 5]]),
             (6, [[1, 2, 3, 4, 5]]),
         ):
             with self.subTest(n=n):
                 actual = list(mi.batched(iterable, n))
                 self.assertEqual(actual, expected)
+
+
+class TransposeTests(TestCase):
+    def test_empty(self):
+        it = []
+        actual = list(mi.transpose(it))
+        expected = []
+        self.assertEqual(actual, expected)
+
+    def test_basic(self):
+        it = [(10, 11, 12), (20, 21, 22), (30, 31, 32)]
+        actual = list(mi.transpose(it))
+        expected = [(10, 20, 30), (11, 21, 31), (12, 22, 32)]
+        self.assertEqual(actual, expected)
+
+    def test_incompatible(self):
+        it = [(10, 11, 12, 13), (20, 21, 22), (30, 31, 32)]
+        actual = list(mi.transpose(it))
+        expected = [(10, 20, 30), (11, 21, 31), (12, 22, 32)]
+        self.assertEqual(actual, expected)
+
+
+class MatMulTests(TestCase):
+    def test_n_by_n(self):
+        actual = list(mi.matmul([(7, 5), (3, 5)], [[2, 5], [7, 9]]))
+        expected = [[49, 80], [41, 60]]
+        self.assertEqual(actual, expected)
+
+    def test_m_by_n(self):
+        m1 = [[2, 5], [7, 9], [3, 4]]
+        m2 = [[7, 11, 5, 4, 9], [3, 5, 2, 6, 3]]
+        actual = list(mi.matmul(m1, m2))
+        expected = [
+            [29, 47, 20, 38, 33],
+            [76, 122, 53, 82, 90],
+            [33, 53, 23, 36, 39],
+        ]
+        self.assertEqual(actual, expected)
+
+
+class FactorTests(TestCase):
+    def test_basic(self):
+        for n, expected in (
+            (0, []),
+            (1, []),
+            (2, [2]),
+            (3, [3]),
+            (4, [2, 2]),
+            (6, [2, 3]),
+            (360, [2, 2, 2, 3, 3, 5]),
+            (128_884_753_939, [128_884_753_939]),
+            (999953 * 999983, [999953, 999983]),
+            (909_909_090_909, [3, 3, 7, 13, 13, 751, 113797]),
+        ):
+            with self.subTest(n=n):
+                actual = list(mi.factor(n))
+                self.assertEqual(actual, expected)
+
+    def test_cross_check(self):
+        prod = lambda x: reduce(mul, x, 1)
+        self.assertTrue(all(prod(mi.factor(n)) == n for n in range(1, 2000)))
+        self.assertTrue(
+            all(set(mi.factor(n)) <= set(mi.sieve(n + 1)) for n in range(2000))
+        )
+        self.assertTrue(
+            all(
+                list(mi.factor(n)) == sorted(mi.factor(n)) for n in range(2000)
+            )
+        )
```

### Comparing `more-itertools-9.0.0/PKG-INFO` & `more-itertools-9.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: more-itertools
-Version: 9.0.0
+Version: 9.1.0
 Summary: More routines for operating on iterables, beyond itertools
 Keywords: itertools,iterator,iteration,filter,peek,peekable,chunk,chunked
 Author-email: Erik Rose <erikrose@grinchcentral.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -48,14 +48,15 @@
 |                        | `split_into <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.split_into>`_,                                                                         |
 |                        | `split_when <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.split_when>`_,                                                                         |
 |                        | `bucket <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.bucket>`_,                                                                                 |
 |                        | `unzip <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.unzip>`_,                                                                                   |
 |                        | `batched <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.batched>`_,                                                                               |
 |                        | `grouper <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.grouper>`_,                                                                               |
 |                        | `partition <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.partition>`_                                                                            |
+|                        | `transpose <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.transpose>`_                                                                            |
 +------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
 | Lookahead and lookback | `spy <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.spy>`_,                                                                                       |
 |                        | `peekable <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.peekable>`_,                                                                             |
 |                        | `seekable <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.seekable>`_                                                                              |
 +------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
 | Windowing              | `windowed <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.windowed>`_,                                                                             |
 |                        | `substrings <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.substrings>`_,                                                                         |
@@ -135,14 +136,15 @@
 |                        | `distinct_combinations <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.distinct_combinations>`_,                                                   |
 |                        | `circular_shifts <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.circular_shifts>`_,                                                               |
 |                        | `partitions <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.partitions>`_,                                                                         |
 |                        | `set_partitions <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.set_partitions>`_,                                                                 |
 |                        | `product_index <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.product_index>`_,                                                                   |
 |                        | `combination_index <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.combination_index>`_,                                                           |
 |                        | `permutation_index <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.permutation_index>`_,                                                           |
+|                        | `gray_product  <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.gray_product>`_,                                                                    |
 |                        | `powerset <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.powerset>`_,                                                                             |
 |                        | `random_product <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.random_product>`_,                                                                 |
 |                        | `random_permutation <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.random_permutation>`_,                                                         |
 |                        | `random_combination <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.random_combination>`_,                                                         |
 |                        | `random_combination_with_replacement <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.random_combination_with_replacement>`_,                       |
 |                        | `nth_product <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.nth_product>`_,                                                                       |
 |                        | `nth_permutation <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.nth_permutation>`_,                                                               |
@@ -162,19 +164,22 @@
 |                        | `side_effect <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.side_effect>`_,                                                                       |
 |                        | `iterate <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.iterate>`_,                                                                               |
 |                        | `difference <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.difference>`_,                                                                         |
 |                        | `make_decorator <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.make_decorator>`_,                                                                 |
 |                        | `SequenceView <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.SequenceView>`_,                                                                     |
 |                        | `time_limited <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.time_limited>`_,                                                                     |
 |                        | `map_if <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.map_if>`_,                                                                                 |
+|                        | `iter_index <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.iter_index>`_,                                                                         |
 |                        | `consume <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.consume>`_,                                                                               |
 |                        | `tabulate <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.tabulate>`_,                                                                             |
-|                        | `repeatfunc <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.repeatfunc>`_                                                                          |
-|                        | `polynomial_from_roots <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.polynomial_from_roots>`_                                                    |
+|                        | `repeatfunc <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.repeatfunc>`_,                                                                         |
+|                        | `polynomial_from_roots <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.polynomial_from_roots>`_,                                                   |
 |                        | `sieve <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.sieve>`_                                                                                    |
+|                        | `factor <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.factor>`_                                                                                  |
+|                        | `matmul <https://more-itertools.readthedocs.io/en/stable/api.html#more_itertools.matmul>`_                                                                                  |
 +------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
 
 
 Getting started
 ===============
 
 To get started, install the library with `pip <https://pip.pypa.io/en/stable/>`_:
```

