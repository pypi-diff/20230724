# Comparing `tmp/rattr-0.1.6.tar.gz` & `tmp/rattr-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rattr-0.1.6.tar", last modified: Fri May 26 08:32:07 2023, max compression
+gzip compressed data, was "rattr-0.1.7.tar", last modified: Mon Jul 24 10:06:34 2023, max compression
```

## Comparing `rattr-0.1.6.tar` & `rattr-0.1.7.tar`

### file list

```diff
@@ -1,98 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:32:07.730930 rattr-0.1.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:32:07.718930 rattr-0.1.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:32:07.722930 rattr-0.1.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-26 08:31:47.000000 rattr-0.1.6/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-26 08:31:47.000000 rattr-0.1.6/.github/workflows/staticanalysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-26 08:31:47.000000 rattr-0.1.6/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-26 08:31:47.000000 rattr-0.1.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-26 08:31:47.000000 rattr-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 08:31:47.000000 rattr-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-05-26 08:32:07.730930 rattr-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13848 2023-05-26 08:31:47.000000 rattr-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:32:07.722930 rattr-0.1.6/rattr/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-26 08:32:07.000000 rattr-0.1.6/rattr/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:32:07.726930 rattr-0.1.6/rattr/analyser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/analyser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/analyser/annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/analyser/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/analyser/cls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:32:07.726930 rattr-0.1.6/rattr/analyser/context/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/analyser/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20909 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/analyser/context/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/analyser/context/symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/analyser/context/symbol_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/analyser/file.py
--rw-r--r--   0 runner    (1001) docker     (123)    17963 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/analyser/function.py
--rw-r--r--   0 runner    (1001) docker     (123)    10901 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/analyser/ir_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/analyser/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/analyser/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    33184 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/analyser/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:32:07.726930 rattr-0.1.6/rattr/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/cli/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    23959 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/cli/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/cli/toml_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/cli/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:32:07.726930 rattr-0.1.6/rattr/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:32:07.726930 rattr-0.1.6/rattr/error/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/error/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/error/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:32:07.726930 rattr-0.1.6/rattr/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:32:07.726930 rattr-0.1.6/rattr/plugins/analysers/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/plugins/analysers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/plugins/analysers/builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/plugins/analysers/collections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:32:07.726930 rattr-0.1.6/rattr/plugins/assertors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/plugins/assertors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/plugins/assertors/import_clobbering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:32:07.722930 rattr-0.1.6/rattr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-05-26 08:32:07.000000 rattr-0.1.6/rattr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-26 08:32:07.000000 rattr-0.1.6/rattr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 08:32:07.000000 rattr-0.1.6/rattr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-26 08:32:07.000000 rattr-0.1.6/rattr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-26 08:32:07.000000 rattr-0.1.6/rattr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 08:32:07.000000 rattr-0.1.6/rattr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-26 08:31:47.000000 rattr-0.1.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-26 08:32:07.730930 rattr-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-26 08:31:47.000000 rattr-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:32:07.730930 rattr-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21080 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:32:07.730930 rattr-0.1.6/tests/context/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28992 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/context/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/context/test_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/context/test_symbol_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:32:07.730930 rattr-0.1.6/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/data/config_1.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:32:07.730930 rattr-0.1.6/tests/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:32:07.730930 rattr-0.1.6/tests/plugins/analysers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/plugins/analysers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/plugins/analysers/test_builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/plugins/analysers/test_collections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:32:07.730930 rattr-0.1.6/tests/plugins/assertors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/plugins/assertors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15049 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/plugins/assertors/test_import_clobbering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:32:07.730930 rattr-0.1.6/tests/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/snippets/not_a_py.file
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/snippets/rattr_full_one.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/snippets/rattr_results_one.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/snippets/rattr_results_two.py
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/test_analysers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/test_bin.py
--rw-r--r--   0 runner    (1001) docker     (123)    13583 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/test_cls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/test_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    23253 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/test_function.py
--rw-r--r--   0 runner    (1001) docker     (123)    17199 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/test_ir_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     9440 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/test_rattr.py
--rw-r--r--   0 runner    (1001) docker     (123)    14967 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/test_regressions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14122 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    43225 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:34.547995 rattr-0.1.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:34.515995 rattr-0.1.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:34.527995 rattr-0.1.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-24 10:06:13.000000 rattr-0.1.7/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-24 10:06:13.000000 rattr-0.1.7/.github/workflows/staticanalysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-24 10:06:13.000000 rattr-0.1.7/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-24 10:06:13.000000 rattr-0.1.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-24 10:06:13.000000 rattr-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-24 10:06:13.000000 rattr-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-07-24 10:06:34.547995 rattr-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13848 2023-07-24 10:06:13.000000 rattr-0.1.7/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      230 2023-07-24 10:06:13.000000 rattr-0.1.7/mkvenv
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-24 10:06:13.000000 rattr-0.1.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:34.527995 rattr-0.1.7/rattr/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-24 10:06:34.000000 rattr-0.1.7/rattr/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:34.535995 rattr-0.1.7/rattr/analyser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/analyser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/analyser/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/analyser/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/analyser/cls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:34.539995 rattr-0.1.7/rattr/analyser/context/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/analyser/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21307 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/analyser/context/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/analyser/context/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/analyser/context/symbol_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/analyser/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18606 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/analyser/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10936 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/analyser/ir_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/analyser/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/analyser/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35612 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/analyser/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:34.539995 rattr-0.1.7/rattr/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/cli/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23983 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/cli/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/cli/toml_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/cli/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:34.539995 rattr-0.1.7/rattr/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:34.539995 rattr-0.1.7/rattr/error/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/error/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/error/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:34.539995 rattr-0.1.7/rattr/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:34.539995 rattr-0.1.7/rattr/plugins/analysers/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/plugins/analysers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/plugins/analysers/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/plugins/analysers/collections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:34.539995 rattr-0.1.7/rattr/plugins/assertors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/plugins/assertors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-07-24 10:06:13.000000 rattr-0.1.7/rattr/plugins/assertors/import_clobbering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:34.531995 rattr-0.1.7/rattr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-07-24 10:06:34.000000 rattr-0.1.7/rattr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-24 10:06:34.000000 rattr-0.1.7/rattr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 10:06:34.000000 rattr-0.1.7/rattr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-24 10:06:34.000000 rattr-0.1.7/rattr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-24 10:06:34.000000 rattr-0.1.7/rattr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-24 10:06:34.000000 rattr-0.1.7/rattr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-24 10:06:13.000000 rattr-0.1.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 10:06:34.547995 rattr-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-24 10:06:13.000000 rattr-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:34.543995 rattr-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21130 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:34.543995 rattr-0.1.7/tests/context/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29028 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/context/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/context/test_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/context/test_symbol_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:34.543995 rattr-0.1.7/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/data/config_1.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:34.543995 rattr-0.1.7/tests/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:34.543995 rattr-0.1.7/tests/plugins/analysers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/plugins/analysers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/plugins/analysers/test_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/plugins/analysers/test_collections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:34.547995 rattr-0.1.7/tests/plugins/assertors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/plugins/assertors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15085 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/plugins/assertors/test_import_clobbering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:34.547995 rattr-0.1.7/tests/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/snippets/not_a_py.file
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/snippets/rattr_full_one.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/snippets/rattr_results_one.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/snippets/rattr_results_two.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/test_analysers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/test_bin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13619 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/test_cls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23289 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/test_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17235 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/test_ir_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/test_rattr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24797 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/test_regressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46573 2023-07-24 10:06:13.000000 rattr-0.1.7/tests/test_util.py
```

### Comparing `rattr-0.1.6/.github/workflows/publish.yml` & `rattr-0.1.7/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `rattr-0.1.6/.github/workflows/staticanalysis.yml` & `rattr-0.1.7/.github/workflows/staticanalysis.yml`

 * *Files 10% similar despite different names*

```diff
@@ -28,31 +28,31 @@
       - name: Install dependencies
         run: |
           python -m pip install .[dev]
 
       - name: Run black on rattr
         run: black --check rattr/
 
-  lint:
+  ruff:
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v2
 
       - name: Setup Python
         uses: actions/setup-python@v2
         with:
           python-version: "3.8"
 
       - name: Install dependencies
         run: |
           python -m pip install .[dev]
 
-      - name: Run flake8 on rattr
-        run: flake8 rattr/
+      - name: Run ruff on rattr
+        run: ruff check .
 
   isort:
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v2
```

### Comparing `rattr-0.1.6/.github/workflows/tests.yml` & `rattr-0.1.7/.github/workflows/tests.yml`

 * *Files 11% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 #       installed -- thus they are included as a "faux"-dependency
 jobs:
   unittests:
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.7", "3.8", "3.9", "3.10", "pypy-3.7", "pypy-3.8"]
+        python-version: ["3.8", "3.9", "3.10", "pypy-3.8", "pypy-3.9"]
         os: [ubuntu-latest, macOS-latest, windows-latest]
 
     steps:
       - uses: actions/checkout@v2
 
       - name: Setup Python ${{ matrix.python-version }} on ${{ matrix.os }}
         uses: actions/setup-python@v2
@@ -37,8 +37,8 @@
           python-version: ${{ matrix.python-version }}
 
       - name: Install dependencies
         run: |
           python -m pip install .[dev]
 
       - name: Run unit tests
-        run: pytest tests/
+        run: python -m pytest tests/
```

### Comparing `rattr-0.1.6/.gitignore` & `rattr-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `rattr-0.1.6/LICENSE` & `rattr-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `rattr-0.1.6/PKG-INFO` & `rattr-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: rattr
-Version: 0.1.6
+Version: 0.1.7
 Summary: Rattr rats on your attrs.
-Home-page: https://github.com/SuadeLabs/ratter
+Home-page: https://github.com/SuadeLabs/rattr
 Author: Suade Labs
 License: MIT
 Keywords: automation linting type-checking attributes rats
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rattr-0.1.6/README.md` & `rattr-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `rattr-0.1.6/rattr/__main__.py` & `rattr-0.1.7/rattr/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python3
 """Rattr entry point."""
+from __future__ import annotations
 
 import json
 from math import log10
 from typing import Iterable, Set
 
 from rattr import config, error
 from rattr.analyser.context import Import, Symbol
```

### Comparing `rattr-0.1.6/rattr/analyser/annotations.py` & `rattr-0.1.7/rattr/analyser/annotations.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Annotations to be imported for use by Rattr analysed code."""
+from __future__ import annotations
 
 from typing import Dict, List, Optional, Set, Tuple
 
 # A set of names, e.g.: "@BinOp", "x.attr", "var_one"
 Names = Set[str]
 
 # LHS: positional args, RHS: named args
```

### Comparing `rattr-0.1.6/rattr/analyser/base.py` & `rattr-0.1.7/rattr/analyser/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Base classes for Rattr components."""
+from __future__ import annotations
 
 import ast
 from abc import ABCMeta, abstractmethod, abstractproperty
 from ast import NodeTransformer, NodeVisitor  # noqa: F401
 from itertools import product
 from typing import Dict, List, Optional
```

### Comparing `rattr-0.1.6/rattr/analyser/cls.py` & `rattr-0.1.7/rattr/analyser/cls.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """Rattr class analyser.
 
 Rattr is designed to be a function analyser and thus the class-based features
 are rather limited.
 
 """
+from __future__ import annotations
 
 import ast
 from typing import List
 
 from rattr.analyser.base import NodeVisitor
 from rattr.analyser.context import Context
 from rattr.analyser.context.symbol import Class, Func, Name, Symbol
 from rattr.analyser.function import FunctionAnalyser
 from rattr.analyser.types import (
     AnyAssign,
     AnyFunctionDef,
+    AstNamedExpr,
     ClassIR,
     FunctionIR,
-    ast_NamedExpr,
 )
 from rattr.analyser.util import (
     get_assignment_targets,
     get_fullname,
     get_function_def_args,
     has_annotation,
     unravel_names,
@@ -58,14 +59,20 @@
 
 
 def is_enum(cls: ast.ClassDef) -> bool:
     # NOTE Purely heuristic, though it does allow for user defined Enum bases
     return any(n == "Enum" or n.endswith(".Enum") for n in get_base_names(cls))
 
 
+def is_namedtuple(cls: ast.ClassDef) -> bool:
+    # NOTE Purely heuristic, though it does allow for user defined NamedTuple bases
+    bases = get_base_names(cls)
+    return any(b == "NamedTuple" or b.endswith(".NamedTuple") for b in bases)
+
+
 class ClassAnalyser(NodeVisitor):
     """Walk a class's AST to determine the accessed attributes.
 
 
     TODO
         - Inheritance, super
         - Class methods
@@ -122,14 +129,17 @@
         if init is not None:
             self.visit_initialiser(init)
 
         # NOTE TODO Handle with proper inheritance
         if init is None and is_enum(self._ast):
             self.visit_enum_initialiser()
 
+        if init is None and is_namedtuple(self._ast):
+            self.visit_named_tuple_initialiser()
+
         # Visit static methods
         for method in get_static_methods(methods):
             self.visit_static_method(method)
 
         return self.class_ir
 
     # ----------------------------------------------------------------------- #
@@ -149,22 +159,15 @@
         # See: context/context.py::RootContext.register_ClassDef
         cls.args, cls.vararg, cls.kwarg = get_function_def_args(init)
 
         self.class_ir[cls] = FunctionAnalyser(init, self.context).analyse()
 
     def visit_enum_initialiser(self) -> None:
         cls: Class = self.context.get(self.class_name)
-        cls.args, cls.vararg, cls.kwarg = (
-            [
-                "self",
-                "_id",
-            ],
-            None,
-            None,
-        )
+        cls.args, cls.vararg, cls.kwarg = ["self", "_id"], None, None
 
         # NOTE Can't determine result at compile-time, thus give every option
         symbols = self.context.symbol_table.symbols()
         names: List[Symbol] = list(filter(lambda s: isinstance(s, Name), symbols))
         enum_values = filter(lambda n: n.name.startswith(f"{self.class_name}."), names)
 
         ir: FunctionIR = {
@@ -172,14 +175,33 @@
             "gets": set(enum_values),
             "calls": set(),
             "dels": set(),
         }
 
         self.class_ir[cls] = ir
 
+    def visit_named_tuple_initialiser(self) -> None:
+        prefix = f"{self.class_name}."
+        tuple_items = [
+            symbol.name[len(prefix) :]
+            for symbol in self.context.symbol_table.symbols()
+            if isinstance(symbol, Name)
+            if symbol.name.startswith(prefix)
+        ]
+
+        cls: Class = self.context.get(self.class_name)
+        cls.args, cls.vararg, cls.kwarg = ["self", *tuple_items], None, None
+
+        self.class_ir[cls] = {
+            "sets": set(),
+            "gets": set(),
+            "calls": set(),
+            "dels": set(),
+        }
+
     def visit_static_method(self, method: AnyFunctionDef) -> None:
         qualified_name = f"{self.class_name}.{method.name}"
         fn = Func(qualified_name, *get_function_def_args(method))
 
         self.class_ir[fn] = FunctionAnalyser(method, self.context).analyse()
 
     # ----------------------------------------------------------------------- #
@@ -208,9 +230,9 @@
 
     def visit_AnnAssign(self, node: ast.AnnAssign) -> None:
         self.visit_AnyAssign(node)
 
     def visit_AugAssign(self, node: ast.AugAssign) -> None:
         self.visit_AnyAssign(node)
 
-    def visit_NamedExpr(self, node: ast_NamedExpr) -> None:
+    def visit_NamedExpr(self, node: AstNamedExpr) -> None:
         self.visit_AnyAssign(node)
```

### Comparing `rattr-0.1.6/rattr/analyser/context/context.py` & `rattr-0.1.7/rattr/analyser/context/context.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 within a given file. All contexts for a file for a tree with unidirectional
 references from child context to parent context.
 
 The root context of a file contains, amongst other things, the Python builtin
 functions such as `print`, etc.
 
 """
+from __future__ import annotations
 
 import ast
 from contextlib import contextmanager
 from dataclasses import replace as copy_dataclass
 from typing import Any, Generator, Iterable, Optional, Set, TypeVar, Union
 
 from rattr import config, error
@@ -23,33 +24,35 @@
     Import,
     Name,
     Symbol,
     get_module_name_and_spec,
     get_possible_module_names,
 )
 from rattr.analyser.context.symbol_table import SymbolTable
-from rattr.analyser.types import AnyAssign, Constant, Literal, ast_NamedExpr
+from rattr.analyser.types import AnyAssign, AstNamedExpr, Constant, Literal
 from rattr.analyser.util import (
     PYTHON_BUILTINS,
     Changes,
     assignment_is_one_to_one,
     enter_file,
     get_absolute_module_name,
     get_assignment_targets,
     get_contained_walruses,
     get_fullname,
     get_function_def_args,
+    get_namedtuple_attrs_from_call,
     get_starred_imports,
     has_affect,
     is_blacklisted_module,
     is_method_on_primitive,
     is_relative_import,
     is_starred_import,
     lambda_in_rhs,
     module_name_from_file_path,
+    namedtuple_in_rhs,
     remove_call_brackets,
     unravel_names,
 )
 
 _Context = TypeVar("_Context", bound="Context")
 
 
@@ -325,15 +328,15 @@
         "__file__",
         "__loader__",
         "__name__",
         "__package__",
         "__spec__",
     ]
 
-    def __new__(self, module: ast.Module) -> Any:  # Context, make mypy happy
+    def __new__(cls, module: ast.Module) -> Any:  # Context, make mypy happy
         if not isinstance(module, ast.Module):
             raise TypeError("The root context can only exist for a module")
 
         context = Context(None)
 
         # Register Python module level attributes
         for attribute in RootContext.module_level_attributes:
@@ -466,14 +469,22 @@
             if not assignment_is_one_to_one(node):
                 error.fatal("lambda assignment must be one-to-one", node)
             else:
                 name = get_fullname(targets[0])
                 self.add(Func(name, *get_function_def_args(node.value)))
             return
 
+        if namedtuple_in_rhs(node):
+            if not assignment_is_one_to_one(node):
+                error.fatal("namedtuple assignment must be one-to-one", node)
+
+            name = get_fullname(targets[0])
+            self.add(Class(name, args=get_namedtuple_attrs_from_call(node)))
+            return
+
         # Walrus operator in the right-hand side of containing assignment
         for walrus in get_contained_walruses(node):
             with Changes(self.symbol_table, keys_fn=lambda t: t.values()) as diff:
                 RootContext.register_NamedExpr(self, walrus)
 
             # If we have "a = (b := lambda ...)" then "a" will have been registered as a
             # Name when it just be a Func with the same signature as the just-added "b"
@@ -505,15 +516,15 @@
         error.warning(
             "avoid 'del' at module-level, Rattr will assume the target has "
             "been removed before reaching any child context (functions, "
             "classes, etc)",
             node,
         )
 
-    def register_NamedExpr(self, node: ast_NamedExpr) -> None:
+    def register_NamedExpr(self, node: AstNamedExpr) -> None:
         RootContext.register_AnyAssign(self, node)
 
     # ----------------------------------------------------------------------- #
     # Functions, classes, etc
     # ----------------------------------------------------------------------- #
 
     def register_FunctionDef(self, node: ast.FunctionDef) -> None:
```

### Comparing `rattr-0.1.6/rattr/analyser/context/symbol.py` & `rattr-0.1.7/rattr/analyser/context/symbol.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 Symbol hash and equivalence only holds when the symbols are within the same
 context.
 
 Symbol `name` is the Python `_identifier` for the given symbol.
 
 """
+from __future__ import annotations
 
 from dataclasses import dataclass
 from importlib.machinery import ModuleSpec
 from importlib.util import find_spec
 from itertools import accumulate, chain, filterfalse
 from typing import Dict, List, Optional, Tuple, Union
 
@@ -64,16 +65,16 @@
     def __hash__(self) -> int:
         return hash(repr(self))
 
 
 @dataclass
 class Func(Symbol):
     args: List[str]
-    vararg: Optional[str]
-    kwarg: Optional[str]
+    vararg: Optional[str] = None
+    kwarg: Optional[str] = None
     is_async: bool = False
     defined_in: Optional[str] = None
 
     def __post_init__(self) -> None:
         self.defined_in = config.current_file
 
     def __hash__(self) -> int:
@@ -87,17 +88,17 @@
     NOTE
         If no initialiser is found; args, vararg, and kwarg will all be None
         If an initialiser is found; args will be an initialised list (could be
         empty), but vararg and kwarg may-or-may-not be None
 
     """
 
-    args: Optional[List[str]]
-    vararg: Optional[str]
-    kwarg: Optional[str]
+    args: Optional[List[str]] = None
+    vararg: Optional[str] = None
+    kwarg: Optional[str] = None
     defined_in: Optional[str] = None
 
     def __post_init__(self) -> None:
         self.defined_in = config.current_file
 
     def __hash__(self) -> int:
         return hash(repr(self))
```

### Comparing `rattr-0.1.6/rattr/analyser/context/symbol_table.py` & `rattr-0.1.7/rattr/analyser/context/symbol_table.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Rattr symbol table."""
+from __future__ import annotations
 
 from typing import KeysView, ValuesView
 
 from rattr.analyser.context.symbol import Import, Symbol
 
 
 class SymbolTable(dict):
```

### Comparing `rattr-0.1.6/rattr/analyser/file.py` & `rattr-0.1.7/rattr/analyser/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Rattr file analyser."""
+from __future__ import annotations
 
 import ast
 from collections import namedtuple
 from copy import deepcopy
 from dataclasses import replace as copy_dataclass
 from typing import List, NamedTuple, Set, Tuple
 
@@ -10,31 +11,32 @@
 from rattr.analyser.base import NodeVisitor
 from rattr.analyser.cls import ClassAnalyser
 from rattr.analyser.context import Context, Func, Import, RootContext
 from rattr.analyser.function import FunctionAnalyser
 from rattr.analyser.types import (
     AnyAssign,
     AnyFunctionDef,
+    AstNamedExpr,
     FileIR,
     ImportsIR,
-    ast_NamedExpr,
 )
 from rattr.analyser.util import (
     Changes,
     assignment_is_one_to_one,
     enter_file,
     get_assignment_targets,
     get_contained_walruses,
     get_fullname,
     has_annotation,
     is_blacklisted_module,
     is_excluded_name,
     is_pip_module,
     is_stdlib_module,
     lambda_in_rhs,
+    namedtuple_in_rhs,
     parse_rattr_results_from_annotation,
     read,
     timer,
 )
 from rattr.plugins import plugins
 
 RattrStats = namedtuple(
@@ -235,18 +237,35 @@
 
         targets = get_assignment_targets(node)
         name = get_fullname(targets[0])
 
         fn, context = self.context.get(name), self.context
         self.file_ir[fn] = FunctionAnalyser(node.value, context).analyse()
 
+    def visit_NamedTupleAssign(self, node: AnyAssign) -> None:
+        if not assignment_is_one_to_one(node):
+            return error.fatal("namedtuple assignment must be one-to-one", node)
+
+        name = get_fullname(get_assignment_targets(node)[0])
+        cls = self.context.get(name)
+
+        self.file_ir[cls] = {
+            "gets": set(),
+            "sets": set(),
+            "dels": set(),
+            "calls": set(),
+        }
+
     def visit_AnyAssign(self, node: AnyAssign) -> None:
         if lambda_in_rhs(node):
             self.visit_LambdaAssign(node)
 
+        if namedtuple_in_rhs(node):
+            self.visit_NamedTupleAssign(node)
+
         # Walrus may obscure a lambda, so peek in and visit the nice walruses
         for walrus in get_contained_walruses(node):
             with Changes(self.file_ir) as diff:
                 self.visit_AnyAssign(walrus)
 
             # If the walrus is of the form "a = (b := lambda ...)" then "a" should have
             # the same result as "b" which would have just been registered
@@ -265,13 +284,13 @@
 
     def visit_AnnAssign(self, node: ast.AnnAssign) -> None:
         self.visit_AnyAssign(node)
 
     def visit_AugAssign(self, node: ast.AugAssign) -> None:
         self.visit_AnyAssign(node)
 
-    def visit_NamedExpr(self, node: ast_NamedExpr) -> None:
+    def visit_NamedExpr(self, node: AstNamedExpr) -> None:
         self.visit_AnyAssign(node)
 
     def visit_Lambda(self, node: ast.Lambda) -> None:
         # NOTE Only reached when the lambda is an anonymous function
         return error.fatal("module level lambdas unsupported", node)
```

### Comparing `rattr-0.1.6/rattr/analyser/function.py` & `rattr-0.1.7/rattr/analyser/function.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Rattr function analyser."""
+from __future__ import annotations
 
 import ast
 from itertools import accumulate
 from typing import List, Optional, Tuple
 
 from rattr import error
 from rattr.analyser.base import NodeVisitor
@@ -14,34 +15,36 @@
     Name,
     Symbol,
     new_context,
 )
 from rattr.analyser.types import (
     AnyAssign,
     AnyFunctionDef,
+    AstNamedExpr,
     CompoundStrictlyNameable,
     FunctionIR,
     Nameable,
     StrictlyNameable,
-    ast_NamedExpr,
 )
 from rattr.analyser.util import (
     LOCAL_VALUE_PREFIX,
     PYTHON_ATTR_BUILTINS,
     assignment_is_one_to_one,
     class_in_rhs,
     get_assignment_targets,
     get_basename,
     get_basename_fullname_pair,
     get_fullname,
     get_function_body,
     get_function_call_args,
     get_function_def_args,
+    get_namedtuple_attrs_from_call,
     is_call_to,
     lambda_in_rhs,
+    namedtuple_in_rhs,
     remove_call_brackets,
 )
 from rattr.plugins import plugins
 
 
 class FunctionAnalyser(NodeVisitor):
     """Walk a function's AST to determine the accessed attributes."""
@@ -50,16 +53,16 @@
         """Set configuration and initialise IR."""
         if not isinstance(_ast, AnyFunctionDef.__args__):
             raise TypeError("FunctionAnalyser expects `_ast` to be a function")
 
         self._ast: AnyFunctionDef = _ast
 
         self.func_ir: FunctionIR = {
-            "sets": set(),
             "gets": set(),
+            "sets": set(),
             "dels": set(),
             "calls": set(),
         }
 
         # NOTE Managed by `new_context` contextmanager -- do not manually set
         self.context: Context = context
 
@@ -218,14 +221,26 @@
         error.error("unable to unbind lambdas defined in functions", node)
 
         name = get_fullname(target)
         func = Func(name, *get_function_def_args(node.value))
 
         self.context.add(func)
 
+    def visit_NamedTupleAssign(self, node: AnyAssign, targets: List[ast.expr]) -> None:
+        """Helper method for handling non-anonymous lambdas."""
+        target = targets[0]
+
+        if not assignment_is_one_to_one(node):
+            error.fatal("namedtuple assignment must be one-to-one", node)
+
+        name = get_fullname(target)
+        cls = Class(name, args=get_namedtuple_attrs_from_call(node))
+
+        self.context.add(cls)
+
     def visit_ClassAssign(self, node: AnyAssign, targets: List[ast.expr]) -> None:
         """Helper method for assignments where RHS is a new class instance."""
         target = targets[0]
 
         if not assignment_is_one_to_one(node):
             error.fatal("class assignment must be one-to-one", node)
 
@@ -260,14 +275,18 @@
         targets = get_assignment_targets(node)
 
         # NOTE Handle special case, non-anonymous lambda
         if lambda_in_rhs(node):
             self.visit_LambdaAssign(node, targets)
             return
 
+        if namedtuple_in_rhs(node):
+            self.visit_NamedTupleAssign(node, targets)
+            return
+
         # NOTE Handle special case, rhs is class
         if class_in_rhs(node, self.context):
             self.visit_ClassAssign(node, targets)
             return
 
         for target in targets:
             self.context.add_identifiers_to_context(target)
@@ -279,15 +298,15 @@
 
     def visit_AnnAssign(self, node: ast.AnnAssign) -> None:
         self.visit_AnyAssign(node)
 
     def visit_AugAssign(self, node: ast.AugAssign) -> None:
         self.visit_AnyAssign(node)
 
-    def visit_NamedExpr(self, node: ast_NamedExpr) -> None:
+    def visit_NamedExpr(self, node: AstNamedExpr) -> None:
         self.func_ir["sets"].add(Name(*get_basename_fullname_pair(node.target)))
 
         if lambda_in_rhs(node):
             self.generic_visit(node.value)
 
         self.visit_AnyAssign(node)
```

### Comparing `rattr-0.1.6/rattr/analyser/ir_dag.py` & `rattr-0.1.7/rattr/analyser/ir_dag.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Represent the IR of functions as a DAG, for simplification."""
+from __future__ import annotations
 
 from copy import deepcopy
 from dataclasses import dataclass
 from typing import Dict, List, Optional, Set, Tuple, Union
 
 from rattr import config, error
 from rattr.analyser.context import (
```

### Comparing `rattr-0.1.6/rattr/analyser/results.py` & `rattr-0.1.7/rattr/analyser/results.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """Rattr functions for producing and displaying results."""
+from __future__ import annotations
+
 import json
 
 from rattr.analyser.context import Symbol
 from rattr.analyser.ir_dag import IrDagNode
 from rattr.analyser.types import FileIR, FileResults, ImportsIR
```

### Comparing `rattr-0.1.6/rattr/analyser/types.py` & `rattr-0.1.7/rattr/analyser/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Rattr types."""
+from __future__ import annotations
 
 import ast
 import json
 import sys
 from typing import (
     Dict,
     ItemsView,
@@ -102,18 +103,18 @@
 
 class _TypeNotInPythonVersion:
     pass
 
 
 # Walrus operator typing
 if sys.version_info.major == 3 and sys.version_info.minor >= 8:
-    ast_NamedExpr: Type[ast.NamedExpr] = ast.NamedExpr
+    AstNamedExpr: Type[ast.NamedExpr] = ast.NamedExpr
     AnyAssign = Union[ast.Assign, ast.AnnAssign, ast.AugAssign, ast.NamedExpr]
 else:
-    ast_NamedExpr = _TypeNotInPythonVersion
+    AstNamedExpr = _TypeNotInPythonVersion
 
 # --------------------------------------------------------------------------- #
 # Results and intermediate representation (IR)
 # --------------------------------------------------------------------------- #
 
 FuncOrClass = Union[Func, Class]
```

### Comparing `rattr-0.1.6/rattr/analyser/util.py` & `rattr-0.1.7/rattr/analyser/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Rattr analyser util functions."""
+from __future__ import annotations
 
 import ast
 import builtins
 import hashlib
 import json
 import re
 import sys
@@ -26,36 +27,35 @@
     Type,
     Union,
 )
 
 from isort.api import place_module
 
 from rattr import config, error
-from rattr.analyser.context.symbol import get_possible_module_names  # noqa
 from rattr.analyser.context.symbol import (
     Class,
     Import,
     Name,
     Symbol,
     parse_call,
     parse_name,
 )
 from rattr.analyser.types import (
     AnyAssign,
     AnyFunctionDef,
     AstDef,
+    AstNamedExpr,
     Comprehension,
     Constant,
     FileResults,
     FuncOrAsyncFunc,
     FunctionIR,
     Literal,
     Nameable,
     StrictlyNameable,
-    ast_NamedExpr,
 )
 
 # The prefix given to local constants, literals, etc to produce a name
 # E.g. "hi" -> get_basename_fullname_pair(.) = "@Str"
 # This must be a character that is not legal for standard Python _identifiers
 # or else code elsewhere may break
 LOCAL_VALUE_PREFIX = "@"
@@ -743,21 +743,21 @@
 
 
 def get_assignment_targets(node: AnyAssign) -> List[ast.expr]:
     """Return the given assignment's targets as a list."""
     if isinstance(node, ast.Assign):
         return node.targets
 
-    if isinstance(node, (ast.AnnAssign, ast.AugAssign, ast_NamedExpr)):
+    if isinstance(node, (ast.AnnAssign, ast.AugAssign, AstNamedExpr)):
         return [node.target]
 
     raise TypeError(f"line {node.lineno}: {ast.dump(node)}")
 
 
-def get_contained_walruses(node: AnyAssign) -> List[ast_NamedExpr]:
+def get_contained_walruses(node: AnyAssign) -> List[AstNamedExpr]:
     """Return the walruses in the RHS of the given assignment.
 
     >>> get_nested_walruses(ast.parse("a = (b := c)"))
     [NamedExpr(target=Name(id='b', ctx=Store()), value=Name(id='c', ctx=Load())), ]
 
     >>> get_nested_walruses(ast.parse("a = (b, c := d)"))
     [NamedExpr(target=Name(id='c', ctx=Store()), value=Name(id='d', ctx=Load())), ]
@@ -766,15 +766,15 @@
         return list()
 
     if isinstance(node.value, (ast.Tuple, ast.List)):
         rhs_values = node.value.elts
     else:
         rhs_values = [node.value]
 
-    return list(filter(lambda v: isinstance(v, ast_NamedExpr), rhs_values))
+    return list(filter(lambda v: isinstance(v, AstNamedExpr), rhs_values))
 
 
 def assignment_is_one_to_one(node: AnyAssign) -> bool:
     """Return `True` if the given assignment is one-to-one."""
     _iterable = (ast.Tuple, ast.List)
 
     targets = get_assignment_targets(node)
@@ -798,22 +798,97 @@
         return False
 
 
 def walrus_in_rhs(node: AnyAssign) -> bool:
     """Return `True` if the RHS contains a walrus operator."""
     _iterable = (ast.Tuple, ast.List)
 
-    if isinstance(node.value, ast_NamedExpr):
+    if isinstance(node.value, AstNamedExpr):
         return True
     elif isinstance(node.value, _iterable):
-        return any(isinstance(v, ast_NamedExpr) for v in node.value.elts)
+        return any(isinstance(v, AstNamedExpr) for v in node.value.elts)
     else:
         return False
 
 
+def namedtuple_in_rhs(node: AnyAssign) -> bool:
+    """Return `True` if the RHS contains a namedtuple creation."""
+    _iterable = (ast.Tuple, ast.List)
+
+    def _target_is_namedtuple(call: ast.Call) -> bool:
+        # HACK
+        #   This is a naive approach, when enum / class-namedtuple / etc detection is
+        #   refactored we can do this a bit better.
+        #   See: cls.py::is_enum, cls.py::is_namedtuple
+        name = get_fullname(call.func)
+        return name == "namedtuple" or name.endswith(".namedtuple")
+
+    if isinstance(node.value, ast.Call):
+        return _target_is_namedtuple(node.value)
+    elif isinstance(node.value, _iterable):
+        return any(
+            _target_is_namedtuple(v) for v in node.value.elts if isinstance(v, ast.Call)
+        )
+    else:
+        return False
+
+
+def get_namedtuple_attrs_from_call(node: AnyAssign) -> tuple[list[str], dict[str, str]]:
+    """Return the args/attrs of the namedtuple constructed by this assignment by call.
+
+    #### Note
+    Assumes one-to-one assignment.
+
+    #### Examples
+    >>> node = ast.parse("p = namedtuple('p', ['x', 'y'])").body[0].value
+    >>> get_namedtuple_init_signature_from_assignment(node)
+    ["self", "x", "y]
+
+    Raises:
+        TypeError: The node is not an assignment of a call.
+
+    Returns:
+        tuple[list[str], dict[str, str]]: The positional and keyword args of the init.
+    """
+    _invalid_signature_error = (
+        "namedtuple expects exactly two positional arguments (i.e. name, attrs)"
+    )
+    _invalid_second_parameter_value_error = (
+        "namedtuple expects the second positional argument to be a list of "
+        "string-literals"
+    )
+
+    # Parse call arguments
+    if not isinstance(node.value, ast.Call):
+        raise TypeError
+
+    namedtuple_call_arguments = node.value.args
+
+    if len(namedtuple_call_arguments) != 2:
+        error.fatal(_invalid_signature_error)
+
+    _, namedtuple_attrs_argument = namedtuple_call_arguments
+
+    if not isinstance(namedtuple_attrs_argument, ast.List):
+        error.fatal(_invalid_second_parameter_value_error)
+
+    # Get attribute names from second positional argument
+    attrs: list[str] = [
+        arg.value
+        for arg in namedtuple_attrs_argument.elts
+        if isinstance(arg, ast.Constant)
+        if isinstance(arg.value, str)
+    ]
+
+    if len(attrs) != len(namedtuple_attrs_argument.elts):
+        error.fatal(_invalid_second_parameter_value_error)
+
+    return ["self", *attrs]
+
+
 def class_in_rhs(node: AnyAssign, context: Any) -> bool:
     """Return `True` if the RHS of the given assignment is a class init."""
     _iterable = (ast.Tuple, ast.List)
 
     def expr_is_class(expr):
         full = get_fullname(expr, safe=True)
```

### Comparing `rattr-0.1.6/rattr/cli/argparse.py` & `rattr-0.1.7/rattr/cli/argparse.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import sys as _sys
 from argparse import (
     _UNRECOGNIZED_ARGS_ATTR,
     SUPPRESS,
     ArgumentError,
     ArgumentParser,
     Namespace,
```

### Comparing `rattr-0.1.6/rattr/cli/parser.py` & `rattr-0.1.7/rattr/cli/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from abc import ABC, abstractstaticmethod
 from argparse import ArgumentError, Namespace, RawTextHelpFormatter
 from os.path import isfile, splitext
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple
 
 from tomli import TOMLDecodeError
@@ -444,15 +446,15 @@
             choices=["none", "short", "full"],
             help=multi_paragraph_wrap(
                 """\
                 >show path level meaning:
                 >    none  - do not show the file path in errors/warnings
                 >    short - show an abbreviated path \033[1m(default)\033[0m
                 >    full  - show the full path
-                >E.g.: "/home/user/very/deep/dir/path/file" becomes "~/.../dir/path/file"  # noqa
+                >E.g.: "/home/user/very/deep/dir/to/file" becomes "~/.../dir/to/file"
                 >TOML example: show-path='short'
                 """
             ),
         )
 
         return parser
```

### Comparing `rattr-0.1.6/rattr/cli/toml_parser.py` & `rattr-0.1.7/rattr/cli/toml_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from pathlib import Path
 from typing import Any, Dict, Optional
 
 try:
     # python >= 3.11
     import tomllib
 except ImportError:
```

### Comparing `rattr-0.1.6/rattr/cli/util.py` & `rattr-0.1.7/rattr/cli/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Rattr CLI parser util functions."""
+from __future__ import annotations
 
 from argparse import Namespace
 from textwrap import dedent, fill
 from typing import Any, Dict
 
 
 def multi_paragraph_wrap(text: str, width: int = 80) -> str:
```

### Comparing `rattr-0.1.6/rattr/config/__init__.py` & `rattr-0.1.7/rattr/config/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from dataclasses import dataclass, field
 from typing import Optional, Set
 
 
 @dataclass
 class Config:
     """Hold Rattr run-time configuration.
```

### Comparing `rattr-0.1.6/rattr/error/error.py` & `rattr-0.1.7/rattr/error/error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Rattr error/logging functions."""
+from __future__ import annotations
 
 import ast
 import sys
 from enum import Enum
 from os.path import expanduser
-from typing import List, Optional, Tuple
+from typing import List, NoReturn, Optional, Tuple
 
 from rattr import config
 
 __ERROR = "{prefix}: {optional_file_info}{optional_line_info}{message}"
 __FILE_INFO = "\033[1m{}: \033[0m"
 __LINE_INFO = "\033[1mline {}:{}: \033[0m"
 
@@ -86,15 +87,15 @@
     __log(Level.ERROR, message, culprit)
 
 
 def fatal(
     message: str,
     culprit: Optional[ast.AST] = None,
     badness: int = 0,  # noqa
-) -> None:
+) -> NoReturn:
     """Log a fatal error and, if given, include culprit line and file info.
 
     NOTE
         A fatal error has no notion of badness as it will always cause an
         immediate EXIT_FAILURE, however, badness is provided in the function
         interface for consistency with the other errors.
```

### Comparing `rattr-0.1.6/rattr/plugins/__init__.py` & `rattr-0.1.7/rattr/plugins/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from dataclasses import dataclass
 from typing import List, Set, Union
 
 from rattr.analyser.base import (
     Assertor,
     CustomFunctionAnalyser,
     CustomFunctionHandler,
```

### Comparing `rattr-0.1.6/rattr/plugins/analysers/builtins.py` & `rattr-0.1.7/rattr/plugins/analysers/builtins.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """CustomFunctionAnalyser for Python's builtin functions."""
+from __future__ import annotations
 
 import ast
 
 from rattr.analyser.base import CustomFunctionAnalyser
 from rattr.analyser.context import Context
 from rattr.analyser.types import FuncOrAsyncFunc, FunctionIR
 from rattr.analyser.util import get_dynamic_name, get_fullname
```

### Comparing `rattr-0.1.6/rattr/plugins/analysers/collections.py` & `rattr-0.1.7/rattr/plugins/analysers/collections.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """CustomFunctionAnalyser for Python's collections."""
+from __future__ import annotations
 
 import ast
 
 from rattr.analyser.base import CustomFunctionAnalyser
 from rattr.analyser.context import Context
 from rattr.analyser.types import FuncOrAsyncFunc, FunctionIR
```

### Comparing `rattr-0.1.6/rattr/plugins/assertors/import_clobbering.py` & `rattr-0.1.7/rattr/plugins/assertors/import_clobbering.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Assert that there are no assignment to names that identify imports."""
+from __future__ import annotations
 
 import ast
 from typing import List, Union
 
 from rattr.analyser.base import Assertor
 from rattr.analyser.types import AnyAssign, AnyFunctionDef, Comprehension
 from rattr.analyser.util import (
```

### Comparing `rattr-0.1.6/rattr.egg-info/PKG-INFO` & `rattr-0.1.7/rattr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: rattr
-Version: 0.1.6
+Version: 0.1.7
 Summary: Rattr rats on your attrs.
-Home-page: https://github.com/SuadeLabs/ratter
+Home-page: https://github.com/SuadeLabs/rattr
 Author: Suade Labs
 License: MIT
 Keywords: automation linting type-checking attributes rats
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rattr-0.1.6/rattr.egg-info/SOURCES.txt` & `rattr-0.1.7/rattr.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 .gitignore
 LICENSE
 MANIFEST.in
 README.md
+mkvenv
+pyproject.toml
 requirements.txt
-setup.cfg
 setup.py
 .github/workflows/publish.yml
 .github/workflows/staticanalysis.yml
 .github/workflows/tests.yml
 rattr/__init__.py
 rattr/__main__.py
 rattr/_version.py
```

### Comparing `rattr-0.1.6/setup.py` & `rattr-0.1.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,45 @@
-import pathlib
+from __future__ import annotations
 
-from setuptools import find_packages, setup
-
-HERE = pathlib.Path(__file__).parent.resolve()
+from pathlib import Path
 
-# Copy description from README.md
-with open(HERE / "README.md") as f:
-    DESCRIPTION = f.read()
+from setuptools import find_packages, setup
 
-# Copy requirements from requirements.txt
-with open(HERE / "requirements.txt") as f:
-    INSTALL_REQUIRES = [line.strip() for line in f.readlines()]
+HERE = Path(__file__).parent.resolve()
+README = HERE / "README.md"
+REQUIREMENTS = HERE / "requirements.txt"
 
 
 setup(
     name="rattr",
     use_scm_version={
         "write_to": "rattr/_version.py",
         "write_to_template": (
             'version = "{version}"  # this should be overwritten by setuptools_scm\n'
         ),
     },
     setup_requires=["setuptools_scm"],
     author="Suade Labs",
     packages=find_packages(),
     description="Rattr rats on your attrs.",
-    long_description=DESCRIPTION,
+    long_description=README.read_text(),
     long_description_content_type="text/markdown",
-    install_requires=INSTALL_REQUIRES,
+    install_requires=[r.strip() for r in REQUIREMENTS.read_text().splitlines()],
     extras_require={
         "dev": [
             "black==22.1.0",
             "click==8.0.2",
-            "flake8-bugbear==22.1.11",
-            "flake8==4.0.1",
-            "flask==2.0.3",
+            "ruff==0.0.270",
             "isort==5.10.1",
             "pytest==7.0.1",
         ],
     },
     entry_points={"console_scripts": ["rattr = rattr.__main__:entry_point"]},
     keywords="automation linting type-checking attributes rats",
-    url="https://github.com/SuadeLabs/ratter",
+    url="https://github.com/SuadeLabs/rattr",
     license="MIT",
     python_requires=">=3.7",
     classifiers=[
         "Environment :: Console",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `rattr-0.1.6/tests/conftest.py` & `rattr-0.1.7/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import ast
 import sys
 from contextlib import contextmanager
 from os.path import dirname, join
 from pathlib import Path
 from typing import Iterable
 
@@ -54,15 +56,15 @@
     else:
         items[:] = unmarked
 
 
 def is_pypy():
     """Return `True` if running under pypy."""
     try:
-        import __pypy__
+        import __pypy__  # noqa: F401
 
         return True
     except ModuleNotFoundError:
         return False
 
 
 def is_python_3_8_plus():
```

### Comparing `rattr-0.1.6/tests/context/test_context.py` & `rattr-0.1.7/tests/context/test_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import ast
 from unittest import mock
 
 import pytest
 
 from rattr.analyser.context import (
     Builtin,
```

### Comparing `rattr-0.1.6/tests/context/test_symbol.py` & `rattr-0.1.7/tests/context/test_symbol.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from rattr.analyser.context.symbol import (
     Call,
     Class,
     Func,
     Import,
     Name,
     Symbol,
```

### Comparing `rattr-0.1.6/tests/context/test_symbol_table.py` & `rattr-0.1.7/tests/context/test_symbol_table.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from rattr.analyser.context import Name, SymbolTable
 
 
 class TestSymbolTable:
     def test_add(self):
         symbol_table = SymbolTable()
```

### Comparing `rattr-0.1.6/tests/plugins/analysers/test_builtins.py` & `rattr-0.1.7/tests/plugins/analysers/test_builtins.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import pytest
 
 from rattr.analyser.context import Call, Func, Name, RootContext
 from rattr.analyser.file import FileAnalyser
 from rattr.plugins import plugins
 from rattr.plugins.analysers.builtins import SortedAnalyser
```

### Comparing `rattr-0.1.6/tests/plugins/analysers/test_collections.py` & `rattr-0.1.7/tests/plugins/analysers/test_collections.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import pytest
 
 from rattr.analyser.context import Builtin, Call, Func, Name, RootContext
 from rattr.analyser.file import FileAnalyser
 from rattr.plugins import plugins
 from rattr.plugins.analysers.collections import DefaultDictAnalyser
```

### Comparing `rattr-0.1.6/tests/plugins/assertors/test_import_clobbering.py` & `rattr-0.1.7/tests/plugins/assertors/test_import_clobbering.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from unittest import mock
 
 from rattr.analyser.context import RootContext
 from rattr.plugins.assertors.import_clobbering import ImportClobberingAssertor
 
 
 class TestImportClobberingAssertor:
```

### Comparing `rattr-0.1.6/tests/snippets/rattr_full_one.py` & `rattr-0.1.7/tests/snippets/rattr_full_one.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.6/tests/test_analysers.py` & `rattr-0.1.7/tests/test_analysers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 """Tests shared across multiple analysers."""
-
-from unittest import mock
-
-import pytest
+from __future__ import annotations
 
 from rattr.analyser.context import RootContext
 from rattr.analyser.context.symbol import Call, Func, Name
 from rattr.analyser.file import FileAnalyser
 
 
 class TestAnnotations:
```

### Comparing `rattr-0.1.6/tests/test_base.py` & `rattr-0.1.7/tests/test_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 """Rattr Base class tests."""
+from __future__ import annotations
 
 from unittest import mock
 
 import pytest
 
-from rattr.analyser.base import (  # CustomFunctionAnalyser,
-    Assertor,
-    CustomFunctionHandler,
-)
+from rattr.analyser.base import Assertor, CustomFunctionHandler
 from rattr.analyser.context.symbol import Call, Import, Name
 
 
 class TestAssertor:
     def test_assertor_is_strict(self, capfd):
         assertor = Assertor(is_strict=True)
```

### Comparing `rattr-0.1.6/tests/test_cls.py` & `rattr-0.1.7/tests/test_cls.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import pytest
 
 from rattr.analyser.context import Call, Class, Func, Name, RootContext
 from rattr.analyser.file import FileAnalyser
 
 
 class TestClassAnalyser:
@@ -69,27 +71,27 @@
         )
         results = FileAnalyser(_ast, RootContext(_ast)).analyse()
 
         func = Func("func", ["arg"], None, None)
         cls = Class("SomeClass", ["self", "some_arg"], None, None)
         expected = {
             func: {
-                "sets": set(),
                 "gets": {Name("arg")},
+                "sets": set(),
                 "dels": set(),
                 "calls": {Call("SomeClass()", ["@ReturnValue", "arg"], {}, target=cls)},
             },
             cls: {
+                "gets": {
+                    Name("some_arg.whatever", "some_arg"),
+                },
                 "sets": {
                     Name("self.whatever", "self"),
                     Name("some_arg.good_number", "some_arg"),
                 },
-                "gets": {
-                    Name("some_arg.whatever", "some_arg"),
-                },
                 "dels": set(),
                 "calls": set(),
             },
         }
 
         # HACK This has to be a repr, can't just compare, idk why
         print(results)
```

### Comparing `rattr-0.1.6/tests/test_error.py` & `rattr-0.1.7/tests/test_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from unittest import mock
 
 from rattr import error
 from rattr.analyser.util import enter_file
 
 
 class TestError:
```

### Comparing `rattr-0.1.6/tests/test_file.py` & `rattr-0.1.7/tests/test_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Tests for module/file level features."""
+from __future__ import annotations
+
 from unittest import mock
 
 import pytest
 
 from rattr.analyser.context import RootContext
-from rattr.analyser.context.symbol import Call, Func, Name
+from rattr.analyser.context.symbol import Func, Name
 from rattr.analyser.file import FileAnalyser
 
 
 class TestModuleLevelStatements:
     def test_assignment(self, parse):
         _ast = parse(
             """
```

### Comparing `rattr-0.1.6/tests/test_function.py` & `rattr-0.1.7/tests/test_function.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import pytest
 
 from rattr.analyser.context import (
     Builtin,
     Call,
     Class,
     Func,
```

### Comparing `rattr-0.1.6/tests/test_ir_dag.py` & `rattr-0.1.7/tests/test_ir_dag.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from unittest import mock
 
 import pytest
 
 from rattr.analyser.context import Builtin, Call, Func, Import, Name
 from rattr.analyser.context.symbol import Class
 from rattr.analyser.ir_dag import (
```

### Comparing `rattr-0.1.6/tests/test_parser.py` & `rattr-0.1.7/tests/test_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from argparse import ArgumentError, Namespace
 from pathlib import Path
 
 import pytest
 
 from rattr.cli.parser import parse_arguments
```

### Comparing `rattr-0.1.6/tests/test_rattr.py` & `rattr-0.1.7/tests/test_rattr.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.6/tests/test_results.py` & `rattr-0.1.7/tests/test_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from unittest import mock
 
 from rattr.analyser.context import Call, Func, Import, Name
 from rattr.analyser.context.symbol import Class
 from rattr.analyser.results import generate_results_from_ir
```

### Comparing `rattr-0.1.6/tests/test_util.py` & `rattr-0.1.7/tests/test_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import ast
 import sys
 from unittest import mock
 
 import pytest
 
 from rattr import error
@@ -20,14 +22,15 @@
     get_dynamic_name,
     get_first_argument_name,
     get_fullname,
     get_function_body,
     get_function_call_args,
     get_function_def_args,
     get_function_form,
+    get_namedtuple_attrs_from_call,
     get_xattr_obj_name_pair,
     has_affect,
     has_annotation,
     is_args,
     is_blacklisted_module,
     is_call_to,
     is_excluded_name,
@@ -38,14 +41,15 @@
     is_name,
     is_pip_module,
     is_relative_import,
     is_set_of_names,
     is_starred_import,
     is_stdlib_module,
     lambda_in_rhs,
+    namedtuple_in_rhs,
     parse_annotation,
     parse_rattr_results_from_annotation,
     remove_call_brackets,
     unravel_names,
     walrus_in_rhs,
 )
 
@@ -837,15 +841,16 @@
     def test_is_pip_module(self):
         # NOTE
         #   This is not the best test ever as it assumes that "flask" are
         #   installed and that "numpy" and "pandas" are not.
         #   However, as this test is testing code that if checking for that
         #   exact property I see no better way of testing it -- a mock would
         #   mock away the tested feature.
-        assert is_pip_module("flask")
+        assert is_pip_module("isort")
+        assert is_pip_module("pytest")
 
         assert not is_pip_module("numpy")
         assert not is_pip_module("pandas")
 
         assert not is_pip_module("math")
         assert not is_pip_module("string")
 
@@ -1329,7 +1334,98 @@
         with Changes(ir) as diff:
             ir["x"] = 99
             del ir["a"]
             del ir["b"]
 
         assert diff.added == {"x"}
         assert diff.removed == {"a", "b"}
+
+
+class TestNamedTupleInRhs:
+    def test_namedtuple_in_rhs(self):
+        ast_ = ast.parse("point = namedtuple('point', ['x', 'y'])")
+        assignment = ast_.body[0]
+        assert namedtuple_in_rhs(assignment)
+
+    def test_user_namedtuple_in_rhs(self):
+        ast_ = ast.parse("point = user_extended.namedtuple('point', ['x', 'y'])")
+        assignment = ast_.body[0]
+        assert namedtuple_in_rhs(assignment)
+
+    def test_namedtuple_not_in_rhs(self):
+        ast_ = ast.parse("point = noomedtoople('point', ['x', 'y'])")
+        assignment = ast_.body[0]
+        assert not namedtuple_in_rhs(assignment)
+
+
+class TestGetNamedTupleAttrsFromCall:
+    def test_rhs_is_not_call(self):
+        ast_ = ast.parse("point = 'not_a_call'")
+        assignment = ast_.body[0]
+
+        with pytest.raises(TypeError):
+            get_namedtuple_attrs_from_call(assignment)
+
+    def test_too_few_arguments(self):
+        ast_ = ast.parse("point = namedtuple('point')")
+        assignment = ast_.body[0]
+
+        with pytest.raises(SystemExit):
+            get_namedtuple_attrs_from_call(assignment)
+
+    def test_too_many_arguments(self):
+        ast_ = ast.parse("point = namedtuple('point', 'x', 'y')")
+        assignment = ast_.body[0]
+
+        with pytest.raises(SystemExit):
+            get_namedtuple_attrs_from_call(assignment)
+
+    def test_second_argument_is_not_a_list(self):
+        ast_ = ast.parse("point = namedtuple('point', ('x', 'y'))")
+        assignment = ast_.body[0]
+
+        with pytest.raises(SystemExit):
+            get_namedtuple_attrs_from_call(assignment)
+
+    def test_second_argument_is_not_a_list_of_string_literals(self):
+        # Non-string literal
+        ast_ = ast.parse("point = namedtuple('point', ['x', 123])")
+        assignment = ast_.body[0]
+
+        with pytest.raises(SystemExit):
+            get_namedtuple_attrs_from_call(assignment)
+
+        # Non-literal
+        ast_ = ast.parse("point = namedtuple('point', ['x', some_variable])")
+        assignment = ast_.body[0]
+
+        with pytest.raises(SystemExit):
+            get_namedtuple_attrs_from_call(assignment)
+
+    def test_attrs_from_named_tuple_call_the_empty_list(self):
+        # Non-string literal
+        ast_ = ast.parse("point = namedtuple('point', [])")
+        assignment = ast_.body[0]
+
+        assert get_namedtuple_attrs_from_call(assignment) == ["self"]
+
+    def test_attrs_from_named_tuple_call_one_item(self):
+        # Non-string literal
+        ast_ = ast.parse("point = namedtuple('point', ['x'])")
+        assignment = ast_.body[0]
+
+        assert get_namedtuple_attrs_from_call(assignment) == ["self", "x"]
+
+    def test_attrs_from_named_tuple_call_two_items(self):
+        # Non-string literal
+        ast_ = ast.parse("point = namedtuple('point', ['x', 'y'])")
+        assignment = ast_.body[0]
+
+        assert get_namedtuple_attrs_from_call(assignment) == ["self", "x", "y"]
+
+    def test_attrs_from_named_tuple_call_multiple_items(self):
+        # Non-string literal
+        ast_ = ast.parse("vec4 = vec4('vector', ['a', 'b', 'c', 'd'])")
+        assignment = ast_.body[0]
+
+        expected = ["self", "a", "b", "c", "d"]
+        assert get_namedtuple_attrs_from_call(assignment) == expected
```

