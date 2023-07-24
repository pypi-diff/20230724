# Comparing `tmp/rattr-0.1.7.tar.gz` & `tmp/rattr-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rattr-0.1.7.tar", last modified: Mon Jul 24 10:06:34 2023, max compression
+gzip compressed data, was "rattr-0.1.8.tar", last modified: Mon Jul 24 13:36:50 2023, max compression
```

## Comparing `rattr-0.1.7.tar` & `rattr-0.1.8.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:34.547995 rattr-0.1.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:34.515995 rattr-0.1.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:34.527995 rattr-0.1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-24 10:06:13.000000 rattr-0.1.7/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-24 10:06:13.000000 rattr-0.1.7/.github/workflows/staticanalysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-24 10:06:13.000000 rattr-0.1.7/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-24 10:06:13.000000 rattr-0.1.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-24 10:06:13.000000 rattr-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-24 10:06:13.000000 rattr-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-07-24 10:06:34.547995 rattr-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13848 2023-07-24 10:06:13.000000 rattr-0.1.7/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      230 2023-07-24 10:06:13.000000 rattr-0.1.7/mkvenv
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-24 10:06:13.000000 rattr-0.1.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:34.527995 rattr-0.1.7/rattr/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-24 10:06:34.000000 rattr-0.1.7/rattr/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:34.535995 rattr-0.1.7/rattr/analyser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/analyser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/analyser/annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/analyser/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/analyser/cls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:34.539995 rattr-0.1.7/rattr/analyser/context/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/analyser/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21307 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/analyser/context/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/analyser/context/symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/analyser/context/symbol_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/analyser/file.py
--rw-r--r--   0 runner    (1001) docker     (123)    18606 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/analyser/function.py
--rw-r--r--   0 runner    (1001) docker     (123)    10936 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/analyser/ir_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/analyser/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/analyser/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    35612 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/analyser/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:34.539995 rattr-0.1.7/rattr/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/cli/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    23983 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/cli/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/cli/toml_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/cli/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:34.539995 rattr-0.1.7/rattr/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:34.539995 rattr-0.1.7/rattr/error/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/error/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/error/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:34.539995 rattr-0.1.7/rattr/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:34.539995 rattr-0.1.7/rattr/plugins/analysers/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/plugins/analysers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/plugins/analysers/builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/plugins/analysers/collections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:34.539995 rattr-0.1.7/rattr/plugins/assertors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/plugins/assertors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/plugins/assertors/import_clobbering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:34.531995 rattr-0.1.7/rattr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-07-24 10:06:34.000000 rattr-0.1.7/rattr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-24 10:06:34.000000 rattr-0.1.7/rattr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 10:06:34.000000 rattr-0.1.7/rattr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-24 10:06:34.000000 rattr-0.1.7/rattr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-24 10:06:34.000000 rattr-0.1.7/rattr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-24 10:06:34.000000 rattr-0.1.7/rattr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-24 10:06:13.000000 rattr-0.1.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 10:06:34.547995 rattr-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-24 10:06:13.000000 rattr-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:34.543995 rattr-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21130 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:34.543995 rattr-0.1.7/tests/context/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29028 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/context/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/context/test_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/context/test_symbol_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:34.543995 rattr-0.1.7/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/data/config_1.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:34.543995 rattr-0.1.7/tests/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:34.543995 rattr-0.1.7/tests/plugins/analysers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/plugins/analysers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/plugins/analysers/test_builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/plugins/analysers/test_collections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:34.547995 rattr-0.1.7/tests/plugins/assertors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/plugins/assertors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15085 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/plugins/assertors/test_import_clobbering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:34.547995 rattr-0.1.7/tests/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/snippets/not_a_py.file
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/snippets/rattr_full_one.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/snippets/rattr_results_one.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/snippets/rattr_results_two.py
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/test_analysers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/test_bin.py
--rw-r--r--   0 runner    (1001) docker     (123)    13619 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/test_cls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/test_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    23289 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/test_function.py
--rw-r--r--   0 runner    (1001) docker     (123)    17235 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/test_ir_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/test_rattr.py
--rw-r--r--   0 runner    (1001) docker     (123)    24797 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/test_regressions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    46573 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:36:50.723884 rattr-0.1.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:36:50.707883 rattr-0.1.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:36:50.711883 rattr-0.1.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-24 13:36:27.000000 rattr-0.1.8/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-24 13:36:27.000000 rattr-0.1.8/.github/workflows/staticanalysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-24 13:36:27.000000 rattr-0.1.8/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-24 13:36:27.000000 rattr-0.1.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-24 13:36:27.000000 rattr-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-24 13:36:27.000000 rattr-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-07-24 13:36:50.723884 rattr-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13848 2023-07-24 13:36:27.000000 rattr-0.1.8/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      230 2023-07-24 13:36:27.000000 rattr-0.1.8/mkvenv
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-24 13:36:27.000000 rattr-0.1.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:36:50.711883 rattr-0.1.8/rattr/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-24 13:36:27.000000 rattr-0.1.8/rattr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-07-24 13:36:27.000000 rattr-0.1.8/rattr/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-24 13:36:50.000000 rattr-0.1.8/rattr/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:36:50.715884 rattr-0.1.8/rattr/analyser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:36:27.000000 rattr-0.1.8/rattr/analyser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-24 13:36:27.000000 rattr-0.1.8/rattr/analyser/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-07-24 13:36:27.000000 rattr-0.1.8/rattr/analyser/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-07-24 13:36:27.000000 rattr-0.1.8/rattr/analyser/cls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:36:50.715884 rattr-0.1.8/rattr/analyser/context/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-24 13:36:27.000000 rattr-0.1.8/rattr/analyser/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21315 2023-07-24 13:36:27.000000 rattr-0.1.8/rattr/analyser/context/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-07-24 13:36:27.000000 rattr-0.1.8/rattr/analyser/context/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-24 13:36:27.000000 rattr-0.1.8/rattr/analyser/context/symbol_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-07-24 13:36:27.000000 rattr-0.1.8/rattr/analyser/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18614 2023-07-24 13:36:27.000000 rattr-0.1.8/rattr/analyser/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10936 2023-07-24 13:36:27.000000 rattr-0.1.8/rattr/analyser/ir_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-24 13:36:27.000000 rattr-0.1.8/rattr/analyser/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-07-24 13:36:27.000000 rattr-0.1.8/rattr/analyser/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36450 2023-07-24 13:36:27.000000 rattr-0.1.8/rattr/analyser/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:36:50.715884 rattr-0.1.8/rattr/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-24 13:36:27.000000 rattr-0.1.8/rattr/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-07-24 13:36:27.000000 rattr-0.1.8/rattr/cli/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23983 2023-07-24 13:36:27.000000 rattr-0.1.8/rattr/cli/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-24 13:36:27.000000 rattr-0.1.8/rattr/cli/toml_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-24 13:36:27.000000 rattr-0.1.8/rattr/cli/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:36:50.715884 rattr-0.1.8/rattr/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-24 13:36:27.000000 rattr-0.1.8/rattr/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:36:50.715884 rattr-0.1.8/rattr/error/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-24 13:36:27.000000 rattr-0.1.8/rattr/error/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-07-24 13:36:27.000000 rattr-0.1.8/rattr/error/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:36:50.715884 rattr-0.1.8/rattr/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-24 13:36:27.000000 rattr-0.1.8/rattr/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:36:50.719884 rattr-0.1.8/rattr/plugins/analysers/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-24 13:36:27.000000 rattr-0.1.8/rattr/plugins/analysers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-07-24 13:36:27.000000 rattr-0.1.8/rattr/plugins/analysers/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-24 13:36:27.000000 rattr-0.1.8/rattr/plugins/analysers/collections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:36:50.719884 rattr-0.1.8/rattr/plugins/assertors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:36:27.000000 rattr-0.1.8/rattr/plugins/assertors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-07-24 13:36:27.000000 rattr-0.1.8/rattr/plugins/assertors/import_clobbering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:36:50.711883 rattr-0.1.8/rattr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-07-24 13:36:50.000000 rattr-0.1.8/rattr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-24 13:36:50.000000 rattr-0.1.8/rattr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:36:50.000000 rattr-0.1.8/rattr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-24 13:36:50.000000 rattr-0.1.8/rattr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-24 13:36:50.000000 rattr-0.1.8/rattr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-24 13:36:50.000000 rattr-0.1.8/rattr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-24 13:36:27.000000 rattr-0.1.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 13:36:50.723884 rattr-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-24 13:36:27.000000 rattr-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:36:50.719884 rattr-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:36:27.000000 rattr-0.1.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21130 2023-07-24 13:36:27.000000 rattr-0.1.8/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:36:50.723884 rattr-0.1.8/tests/context/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:36:27.000000 rattr-0.1.8/tests/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29028 2023-07-24 13:36:27.000000 rattr-0.1.8/tests/context/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-07-24 13:36:27.000000 rattr-0.1.8/tests/context/test_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-24 13:36:27.000000 rattr-0.1.8/tests/context/test_symbol_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:36:50.723884 rattr-0.1.8/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-24 13:36:27.000000 rattr-0.1.8/tests/data/config_1.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:36:50.723884 rattr-0.1.8/tests/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:36:27.000000 rattr-0.1.8/tests/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:36:50.723884 rattr-0.1.8/tests/plugins/analysers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:36:27.000000 rattr-0.1.8/tests/plugins/analysers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-07-24 13:36:27.000000 rattr-0.1.8/tests/plugins/analysers/test_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-24 13:36:27.000000 rattr-0.1.8/tests/plugins/analysers/test_collections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:36:50.723884 rattr-0.1.8/tests/plugins/assertors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:36:27.000000 rattr-0.1.8/tests/plugins/assertors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15085 2023-07-24 13:36:27.000000 rattr-0.1.8/tests/plugins/assertors/test_import_clobbering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:36:50.723884 rattr-0.1.8/tests/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:36:27.000000 rattr-0.1.8/tests/snippets/not_a_py.file
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-24 13:36:27.000000 rattr-0.1.8/tests/snippets/rattr_full_one.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-24 13:36:27.000000 rattr-0.1.8/tests/snippets/rattr_results_one.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-24 13:36:27.000000 rattr-0.1.8/tests/snippets/rattr_results_two.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-07-24 13:36:27.000000 rattr-0.1.8/tests/test_analysers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-07-24 13:36:27.000000 rattr-0.1.8/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-24 13:36:27.000000 rattr-0.1.8/tests/test_bin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13619 2023-07-24 13:36:27.000000 rattr-0.1.8/tests/test_cls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-07-24 13:36:27.000000 rattr-0.1.8/tests/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-07-24 13:36:27.000000 rattr-0.1.8/tests/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23289 2023-07-24 13:36:27.000000 rattr-0.1.8/tests/test_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17235 2023-07-24 13:36:27.000000 rattr-0.1.8/tests/test_ir_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-07-24 13:36:27.000000 rattr-0.1.8/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-07-24 13:36:27.000000 rattr-0.1.8/tests/test_rattr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27374 2023-07-24 13:36:27.000000 rattr-0.1.8/tests/test_regressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-07-24 13:36:27.000000 rattr-0.1.8/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46573 2023-07-24 13:36:27.000000 rattr-0.1.8/tests/test_util.py
```

### Comparing `rattr-0.1.7/.github/workflows/publish.yml` & `rattr-0.1.8/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/.github/workflows/staticanalysis.yml` & `rattr-0.1.8/.github/workflows/staticanalysis.yml`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/.github/workflows/tests.yml` & `rattr-0.1.8/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/.gitignore` & `rattr-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/LICENSE` & `rattr-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/PKG-INFO` & `rattr-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rattr
-Version: 0.1.7
+Version: 0.1.8
 Summary: Rattr rats on your attrs.
 Home-page: https://github.com/SuadeLabs/rattr
 Author: Suade Labs
 License: MIT
 Keywords: automation linting type-checking attributes rats
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `rattr-0.1.7/README.md` & `rattr-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/pyproject.toml` & `rattr-0.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/rattr/__main__.py` & `rattr-0.1.8/rattr/__main__.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/rattr/analyser/annotations.py` & `rattr-0.1.8/rattr/analyser/annotations.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/rattr/analyser/base.py` & `rattr-0.1.8/rattr/analyser/base.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/rattr/analyser/cls.py` & `rattr-0.1.8/rattr/analyser/cls.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/rattr/analyser/context/context.py` & `rattr-0.1.8/rattr/analyser/context/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -471,15 +471,15 @@
             else:
                 name = get_fullname(targets[0])
                 self.add(Func(name, *get_function_def_args(node.value)))
             return
 
         if namedtuple_in_rhs(node):
             if not assignment_is_one_to_one(node):
-                error.fatal("namedtuple assignment must be one-to-one", node)
+                error.fatal("namedtuple assignment must be one-to-one", culprit=node)
 
             name = get_fullname(targets[0])
             self.add(Class(name, args=get_namedtuple_attrs_from_call(node)))
             return
 
         # Walrus operator in the right-hand side of containing assignment
         for walrus in get_contained_walruses(node):
```

### Comparing `rattr-0.1.7/rattr/analyser/context/symbol.py` & `rattr-0.1.8/rattr/analyser/context/symbol.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/rattr/analyser/context/symbol_table.py` & `rattr-0.1.8/rattr/analyser/context/symbol_table.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/rattr/analyser/file.py` & `rattr-0.1.8/rattr/analyser/file.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/rattr/analyser/function.py` & `rattr-0.1.8/rattr/analyser/function.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,15 +226,15 @@
         self.context.add(func)
 
     def visit_NamedTupleAssign(self, node: AnyAssign, targets: List[ast.expr]) -> None:
         """Helper method for handling non-anonymous lambdas."""
         target = targets[0]
 
         if not assignment_is_one_to_one(node):
-            error.fatal("namedtuple assignment must be one-to-one", node)
+            error.fatal("namedtuple assignment must be one-to-one", culprit=node)
 
         name = get_fullname(target)
         cls = Class(name, args=get_namedtuple_attrs_from_call(node))
 
         self.context.add(cls)
 
     def visit_ClassAssign(self, node: AnyAssign, targets: List[ast.expr]) -> None:
```

### Comparing `rattr-0.1.7/rattr/analyser/ir_dag.py` & `rattr-0.1.8/rattr/analyser/ir_dag.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/rattr/analyser/results.py` & `rattr-0.1.8/rattr/analyser/results.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/rattr/analyser/types.py` & `rattr-0.1.8/rattr/analyser/types.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/rattr/analyser/util.py` & `rattr-0.1.8/rattr/analyser/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -815,27 +815,65 @@
     _iterable = (ast.Tuple, ast.List)
 
     def _target_is_namedtuple(call: ast.Call) -> bool:
         # HACK
         #   This is a naive approach, when enum / class-namedtuple / etc detection is
         #   refactored we can do this a bit better.
         #   See: cls.py::is_enum, cls.py::is_namedtuple
-        name = get_fullname(call.func)
+        name = get_fullname(call.func, safe=True)
         return name == "namedtuple" or name.endswith(".namedtuple")
 
     if isinstance(node.value, ast.Call):
         return _target_is_namedtuple(node.value)
     elif isinstance(node.value, _iterable):
         return any(
-            _target_is_namedtuple(v) for v in node.value.elts if isinstance(v, ast.Call)
+            _target_is_namedtuple(value)
+            for value in node.value.elts
+            if isinstance(value, ast.Call)
         )
     else:
         return False
 
 
+def _attrs_from_list_of_strings(attrs_argument: ast.List) -> list[str]:
+    attrs: list[str] = [
+        arg.value
+        for arg in attrs_argument.elts
+        if isinstance(arg, ast.Constant)
+        if isinstance(arg.value, str)
+    ]
+
+    if len(attrs) != len(attrs_argument.elts):
+        raise SyntaxError
+
+    return attrs
+
+
+def _attrs_from_space_delimited_string(attrs_argument: ast.Constant) -> list[str]:
+    if not isinstance(attrs_argument.value, str):
+        raise SyntaxError
+
+    attrs = attrs_argument.value.split(" ")
+
+    if not all(attr.isidentifier() for attr in attrs):
+        raise SyntaxError
+
+    return attrs
+
+
+def _namedtuple_attrs_from_second_argument(attrs_argument: ast.AST) -> list[str]:
+    if isinstance(attrs_argument, ast.List):
+        return _attrs_from_list_of_strings(attrs_argument)
+
+    if isinstance(attrs_argument, ast.Constant):
+        return _attrs_from_space_delimited_string(attrs_argument)
+
+    raise SyntaxError
+
+
 def get_namedtuple_attrs_from_call(node: AnyAssign) -> tuple[list[str], dict[str, str]]:
     """Return the args/attrs of the namedtuple constructed by this assignment by call.
 
     #### Note
     Assumes one-to-one assignment.
 
     #### Examples
@@ -849,42 +887,34 @@
     Returns:
         tuple[list[str], dict[str, str]]: The positional and keyword args of the init.
     """
     _invalid_signature_error = (
         "namedtuple expects exactly two positional arguments (i.e. name, attrs)"
     )
     _invalid_second_parameter_value_error = (
-        "namedtuple expects the second positional argument to be a list of "
-        "string-literals"
+        "namedtuple expects the second positional argument to be a list of valid "
+        "identifiers as either a list of string-literals or a space-delimited "
+        "string-literal"
     )
 
     # Parse call arguments
     if not isinstance(node.value, ast.Call):
         raise TypeError
 
     namedtuple_call_arguments = node.value.args
 
     if len(namedtuple_call_arguments) != 2:
-        error.fatal(_invalid_signature_error)
+        error.fatal(_invalid_signature_error, culprit=node.value)
 
     _, namedtuple_attrs_argument = namedtuple_call_arguments
 
-    if not isinstance(namedtuple_attrs_argument, ast.List):
-        error.fatal(_invalid_second_parameter_value_error)
-
-    # Get attribute names from second positional argument
-    attrs: list[str] = [
-        arg.value
-        for arg in namedtuple_attrs_argument.elts
-        if isinstance(arg, ast.Constant)
-        if isinstance(arg.value, str)
-    ]
-
-    if len(attrs) != len(namedtuple_attrs_argument.elts):
-        error.fatal(_invalid_second_parameter_value_error)
+    try:
+        attrs = _namedtuple_attrs_from_second_argument(namedtuple_attrs_argument)
+    except SyntaxError:
+        error.fatal(_invalid_second_parameter_value_error, culprit=node.value)
 
     return ["self", *attrs]
 
 
 def class_in_rhs(node: AnyAssign, context: Any) -> bool:
     """Return `True` if the RHS of the given assignment is a class init."""
     _iterable = (ast.Tuple, ast.List)
```

### Comparing `rattr-0.1.7/rattr/cli/argparse.py` & `rattr-0.1.8/rattr/cli/argparse.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/rattr/cli/parser.py` & `rattr-0.1.8/rattr/cli/parser.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/rattr/cli/toml_parser.py` & `rattr-0.1.8/rattr/cli/toml_parser.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/rattr/cli/util.py` & `rattr-0.1.8/rattr/cli/util.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/rattr/config/__init__.py` & `rattr-0.1.8/rattr/config/__init__.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/rattr/error/error.py` & `rattr-0.1.8/rattr/error/error.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/rattr/plugins/__init__.py` & `rattr-0.1.8/rattr/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/rattr/plugins/analysers/builtins.py` & `rattr-0.1.8/rattr/plugins/analysers/builtins.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/rattr/plugins/analysers/collections.py` & `rattr-0.1.8/rattr/plugins/analysers/collections.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/rattr/plugins/assertors/import_clobbering.py` & `rattr-0.1.8/rattr/plugins/assertors/import_clobbering.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/rattr.egg-info/PKG-INFO` & `rattr-0.1.8/rattr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rattr
-Version: 0.1.7
+Version: 0.1.8
 Summary: Rattr rats on your attrs.
 Home-page: https://github.com/SuadeLabs/rattr
 Author: Suade Labs
 License: MIT
 Keywords: automation linting type-checking attributes rats
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `rattr-0.1.7/rattr.egg-info/SOURCES.txt` & `rattr-0.1.8/rattr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/setup.py` & `rattr-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/tests/conftest.py` & `rattr-0.1.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/tests/context/test_context.py` & `rattr-0.1.8/tests/context/test_context.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/tests/context/test_symbol.py` & `rattr-0.1.8/tests/context/test_symbol.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/tests/context/test_symbol_table.py` & `rattr-0.1.8/tests/context/test_symbol_table.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/tests/plugins/analysers/test_builtins.py` & `rattr-0.1.8/tests/plugins/analysers/test_builtins.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/tests/plugins/analysers/test_collections.py` & `rattr-0.1.8/tests/plugins/analysers/test_collections.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/tests/plugins/assertors/test_import_clobbering.py` & `rattr-0.1.8/tests/plugins/assertors/test_import_clobbering.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/tests/snippets/rattr_full_one.py` & `rattr-0.1.8/tests/snippets/rattr_full_one.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/tests/test_analysers.py` & `rattr-0.1.8/tests/test_analysers.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/tests/test_base.py` & `rattr-0.1.8/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/tests/test_cls.py` & `rattr-0.1.8/tests/test_cls.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/tests/test_error.py` & `rattr-0.1.8/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/tests/test_file.py` & `rattr-0.1.8/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/tests/test_function.py` & `rattr-0.1.8/tests/test_function.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/tests/test_ir_dag.py` & `rattr-0.1.8/tests/test_ir_dag.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/tests/test_parser.py` & `rattr-0.1.8/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/tests/test_rattr.py` & `rattr-0.1.8/tests/test_rattr.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/tests/test_regressions.py` & `rattr-0.1.8/tests/test_regressions.py`

 * *Files 2% similar despite different names*

```diff
@@ -732,14 +732,59 @@
         }
 
         # `point` is defined as a local callable, which is no yet supported, thus this
         # should fail in strict mode.
         assert file_ir._file_ir == expected
         assert _exit.call_count == 1
 
+    def test_call_with_space_delimited_string_argument(self, constant, parse):
+        _ast = parse(
+            """
+            from collections import namedtuple
+
+            point = namedtuple("point", "x y")
+
+            def my_function():
+                return point(1, y=2)
+            """
+        )
+
+        # This failed at analyse, but we should show that simplification also works
+        with mock.patch("sys.exit") as _exit:
+            file_ir = FileAnalyser(_ast, RootContext(_ast)).analyse()
+            _ = generate_results_from_ir(file_ir, imports_ir={})
+
+        point = Class("point", args=["self", "x", "y"])
+        point_call = Call(
+            name="point()",
+            args=["@ReturnValue", constant("Str")],
+            kwargs={"y": constant("Str")},
+            target=point,
+        )
+
+        my_function = Func("my_function", [])
+
+        expected = {
+            point: {
+                "gets": set(),
+                "sets": set(),
+                "dels": set(),
+                "calls": set(),
+            },
+            my_function: {
+                "gets": set(),
+                "sets": set(),
+                "dels": set(),
+                "calls": {point_call},
+            },
+        }
+
+        assert file_ir._file_ir == expected
+        assert _exit.call_count == 0
+
 
 class TestNamedTupleFromInheritance:
     # Test namedtuples constructed by inheriting from `typing.NamedTuple`.
     # This previously had a fatal error at simplification.
 
     @pytest.fixture(autouse=True)
     def _set_current_file(self, config) -> None:
@@ -873,7 +918,47 @@
                 "dels": set(),
                 "calls": {point_call},
             },
         }
 
         assert file_ir._file_ir == expected
         assert _exit.call_count == 0
+
+
+class TestRattrConstantInNameableOnCheckForNamedTuple:
+    """
+    Brief:
+    On checking if there is a named-tuple in the right-hand side of an expression,
+    when the right hand side is a non-safely nameable expression an error is given.
+
+    Introduced: 0.1.7
+    Fixed: 0.1.8
+    """
+
+    def test_safely_determine_rhs_name_on_namedtuple_check(self, parse, constant):
+        _ast = parse(
+            """
+            def my_function(foobar, info=None):
+                i_cause_the_error = "_".join(info.parts)
+            """
+        )
+
+        with mock.patch("sys.exit") as _exit:
+            file_ir = FileAnalyser(_ast, RootContext(_ast)).analyse()
+            _ = generate_results_from_ir(file_ir, imports_ir={})
+
+        my_function = Func("my_function", ["foobar", "info"])
+
+        string_join = f"{constant('@Str')}.join()"
+        string_join_call = Call(string_join, ["info.parts"], {})
+
+        expected_file_ir = {
+            my_function: {
+                "gets": {Name("info.parts", basename="info")},
+                "sets": {Name("i_cause_the_error")},
+                "dels": set(),
+                "calls": {string_join_call},
+            }
+        }
+
+        assert not _exit.called
+        assert file_ir._file_ir == expected_file_ir
```

### Comparing `rattr-0.1.7/tests/test_results.py` & `rattr-0.1.8/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.7/tests/test_util.py` & `rattr-0.1.8/tests/test_util.py`

 * *Files identical despite different names*

