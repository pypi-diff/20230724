# Comparing `tmp/cchdo.hydro-1.0.2.2.tar.gz` & `tmp/cchdo.hydro-1.0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cchdo.hydro-1.0.2.2.tar", last modified: Fri Aug 19 20:03:48 2022, max compression
+gzip compressed data, was "cchdo.hydro-1.0.2.3.tar", last modified: Mon Jul 24 19:29:52 2023, max compression
```

## Comparing `cchdo.hydro-1.0.2.2.tar` & `cchdo.hydro-1.0.2.3.tar`

### file list

```diff
@@ -1,68 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 20:03:48.912712 cchdo.hydro-1.0.2.2/
--rw-r--r--   0 runner    (1001) docker     (121)      167 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 20:03:48.908712 cchdo.hydro-1.0.2.2/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (121)     1353 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)     2005 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 20:03:48.908712 cchdo.hydro-1.0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 20:03:48.908712 cchdo.hydro-1.0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/.github/workflows/do-release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1365 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/.github/workflows/python-app.yml
--rw-r--r--   0 runner    (1001) docker     (121)      538 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      531 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      210 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 20:03:48.908712 cchdo.hydro-1.0.2.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (121)     4850 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (121)     1504 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2319 2022-08-19 20:03:48.912712 cchdo.hydro-1.0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      490 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 20:03:48.908712 cchdo.hydro-1.0.2.2/cchdo/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 20:03:48.912712 cchdo.hydro-1.0.2.2/cchdo/hydro/
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/cchdo/hydro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7694 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/cchdo/hydro/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1813 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/cchdo/hydro/__main_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-08-19 20:03:48.000000 cchdo.hydro-1.0.2.2/cchdo/hydro/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    19290 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/cchdo/hydro/accessors.py
--rw-r--r--   0 runner    (1001) docker     (121)     2087 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/cchdo/hydro/conformance.py
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/cchdo/hydro/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 20:03:48.912712 cchdo.hydro-1.0.2.2/cchdo/hydro/exchange/
--rw-r--r--   0 runner    (1001) docker     (121)    55604 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/cchdo/hydro/exchange/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4741 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/cchdo/hydro/exchange/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3810 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/cchdo/hydro/exchange/flags.py
--rw-r--r--   0 runner    (1001) docker     (121)     2638 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/cchdo/hydro/exchange/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1606 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/cchdo/hydro/rename.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 20:03:48.912712 cchdo.hydro-1.0.2.2/cchdo/hydro/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/cchdo/hydro/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      462 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/cchdo/hydro/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 20:03:48.912712 cchdo.hydro-1.0.2.2/cchdo/hydro/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)    62896 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/cchdo/hydro/tests/data/33RR20080204_mini_hy1.csv
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/cchdo/hydro/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4307 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/cchdo/hydro/tests/data/btl_time_span.csv
--rw-r--r--   0 runner    (1001) docker     (121)     5384 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/cchdo/hydro/tests/test_exchange.py
--rw-r--r--   0 runner    (1001) docker     (121)      436 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/cchdo/hydro/tests/test_merge.py
--rw-r--r--   0 runner    (1001) docker     (121)     1038 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/cchdo/hydro/tests/test_rename.py
--rw-r--r--   0 runner    (1001) docker     (121)     1429 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/cchdo/hydro/tutorial.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 20:03:48.908712 cchdo.hydro-1.0.2.2/cchdo.hydro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2319 2022-08-19 20:03:48.000000 cchdo.hydro-1.0.2.2/cchdo.hydro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1333 2022-08-19 20:03:48.000000 cchdo.hydro-1.0.2.2/cchdo.hydro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-19 20:03:48.000000 cchdo.hydro-1.0.2.2/cchdo.hydro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-08-19 20:03:48.000000 cchdo.hydro-1.0.2.2/cchdo.hydro.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-19 20:03:48.000000 cchdo.hydro-1.0.2.2/cchdo.hydro.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      505 2022-08-19 20:03:48.000000 cchdo.hydro-1.0.2.2/cchdo.hydro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-08-19 20:03:48.000000 cchdo.hydro-1.0.2.2/cchdo.hydro.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 20:03:48.912712 cchdo.hydro-1.0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      580 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9245 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/docs/attributes.rst
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5780 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      465 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      787 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 20:03:48.912712 cchdo.hydro-1.0.2.2/examples/
--rw-r--r--   0 runner    (1001) docker     (121)    89583 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/examples/simple.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)      352 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      986 2022-08-19 20:03:48.912712 cchdo.hydro-1.0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-08-19 20:03:36.000000 cchdo.hydro-1.0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:29:52.285889 cchdo.hydro-1.0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:29:52.277888 cchdo.hydro-1.0.2.3/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:29:52.273888 cchdo.hydro-1.0.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:29:52.277888 cchdo.hydro-1.0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/.github/workflows/do-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/.github/workflows/python-app.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:29:52.277888 cchdo.hydro-1.0.2.3/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-07-24 19:29:52.285889 cchdo.hydro-1.0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:29:52.273888 cchdo.hydro-1.0.2.3/cchdo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:29:52.277888 cchdo.hydro-1.0.2.3/cchdo/hydro/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/cchdo/hydro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/cchdo/hydro/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/cchdo/hydro/__main_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-24 19:29:52.000000 cchdo.hydro-1.0.2.3/cchdo/hydro/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28219 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/cchdo/hydro/accessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/cchdo/hydro/conformance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/cchdo/hydro/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/cchdo/hydro/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:29:52.281888 cchdo.hydro-1.0.2.3/cchdo/hydro/exchange/
+-rw-r--r--   0 runner    (1001) docker     (123)    59612 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/cchdo/hydro/exchange/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/cchdo/hydro/exchange/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/cchdo/hydro/exchange/flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/cchdo/hydro/exchange/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:29:52.281888 cchdo.hydro-1.0.2.3/cchdo/hydro/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/cchdo/hydro/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:29:52.281888 cchdo.hydro-1.0.2.3/cchdo/hydro/legacy/coards/
+-rw-r--r--   0 runner    (1001) docker     (123)    17887 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/cchdo/hydro/legacy/coards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7204 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/cchdo/hydro/legacy/coards/name_netcdf.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:29:52.281888 cchdo.hydro-1.0.2.3/cchdo/hydro/legacy/woce/
+-rw-r--r--   0 runner    (1001) docker     (123)    13897 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/cchdo/hydro/legacy/woce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/cchdo/hydro/legacy/woce/woce_params_for_exchange_to_woce.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/cchdo/hydro/migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/cchdo/hydro/rename.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:29:52.281888 cchdo.hydro-1.0.2.3/cchdo/hydro/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/cchdo/hydro/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/cchdo/hydro/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:29:52.281888 cchdo.hydro-1.0.2.3/cchdo/hydro/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    62896 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/cchdo/hydro/tests/data/33RR20080204_mini_hy1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/cchdo/hydro/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/cchdo/hydro/tests/data/btl_csv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/cchdo/hydro/tests/data/btl_time_span.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/cchdo/hydro/tests/data/stns_test_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/cchdo/hydro/tests/test_accessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/cchdo/hydro/tests/test_core_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/cchdo/hydro/tests/test_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/cchdo/hydro/tests/test_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/cchdo/hydro/tests/test_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/cchdo/hydro/tests/test_rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/cchdo/hydro/tutorial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:29:52.277888 cchdo.hydro-1.0.2.3/cchdo.hydro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-07-24 19:29:52.000000 cchdo.hydro-1.0.2.3/cchdo.hydro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-24 19:29:52.000000 cchdo.hydro-1.0.2.3/cchdo.hydro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 19:29:52.000000 cchdo.hydro-1.0.2.3/cchdo.hydro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 19:29:52.000000 cchdo.hydro-1.0.2.3/cchdo.hydro.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 19:29:52.000000 cchdo.hydro-1.0.2.3/cchdo.hydro.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-24 19:29:52.000000 cchdo.hydro-1.0.2.3/cchdo.hydro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-24 19:29:52.000000 cchdo.hydro-1.0.2.3/cchdo.hydro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:29:52.285889 cchdo.hydro-1.0.2.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7702 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/docs/ODF_CCHDO_netCDF_ops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/docs/_erddap_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20207 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/docs/_erddap_table.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11108 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/docs/attributes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/docs/erddap.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15384 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/docs/format_spec.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:29:52.285889 cchdo.hydro-1.0.2.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)  1417293 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/examples/round_trip.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    89583 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/examples/simple.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-24 19:29:52.285889 cchdo.hydro-1.0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-24 19:29:33.000000 cchdo.hydro-1.0.2.3/setup.py
```

### Comparing `cchdo.hydro-1.0.2.2/.github/workflows/do-release.yml` & `cchdo.hydro-1.0.2.3/.github/workflows/do-release.yml`

 * *Files 25% similar despite different names*

```diff
@@ -8,27 +8,27 @@
     types: [published]
 
 jobs:
   publish:
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v2
-    - name: Set up Python 3.8
-      uses: actions/setup-python@v2
+    - uses: actions/checkout@v3
+    - name: Set up Python 3.10
+      uses: actions/setup-python@v4
       with:
-        python-version: 3.8
+        python-version: '3.10'
     - name: Install Bundling dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install twine pep517
+        pip install twine build
     - name: Build Dists
       run: |
-        python -m pep517.build --source --binary . --out-dir dist
+        python -m build --sdist --wheel --outdir dist/
     - name: Test Wheel
       run: |
         cd dist && pip install $(ls *.whl)'[selftest]' && python -m pytest --pyargs cchdo.hydro && twine check *
     - name: Publish Python distribution to PyPI
-      uses: pypa/gh-action-pypi-publish@master
+      uses: pypa/gh-action-pypi-publish@release/v1
       with:
         user: __token__
         password: ${{ secrets.PYPI_PASSWORD }}
```

### Comparing `cchdo.hydro-1.0.2.2/.github/workflows/python-app.yml` & `cchdo.hydro-1.0.2.3/.github/workflows/python-app.yml`

 * *Files 24% similar despite different names*

```diff
@@ -11,19 +11,21 @@
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v2
-    - name: Set up Python 3.8
-      uses: actions/setup-python@v2
+    - uses: actions/checkout@v3
+    - name: Set up Python 3.10
+      uses: actions/setup-python@v4
       with:
-        python-version: 3.8
+        python-version: '3.10'
+        cache: 'pip'
+        cache-dependency-path: setup.py
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install .[complete]
     - name: Lint with flake8
       run: |
         # stop the build if there are Python syntax errors or undefined names
@@ -34,12 +36,12 @@
       run: |
         pytest --cov-report xml --cov=cchdo
     - name: Test code style with black
       run: |
         black --check .
     - name: Test typing
       run: |
-        mypy -v cchdo
+        mypy --namespace-packages --explicit-package-bases cchdo
     - name: Upload coverage to Codecov
       uses: codecov/codecov-action@v1
       with:
         file: ./coverage.xml
```

### Comparing `cchdo.hydro-1.0.2.2/.gitignore` & `cchdo.hydro-1.0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `cchdo.hydro-1.0.2.2/.pre-commit-config.yaml` & `cchdo.hydro-1.0.2.3/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
 # https://github.com/python/black#version-control-integration
 repos:
   - repo: https://github.com/python/black
-    rev: 22.6.0
+    rev: 23.1.0
     hooks:
       - id: black
         language_version: python3.9
   - repo: https://github.com/pycqa/flake8
-    rev:  5.0.4
+    rev:  6.0.0
     hooks:
       - id: flake8
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.971
+    rev: v1.0.0
     hooks:
       - id: mypy
         additional_dependencies: [types-requests]
```

### Comparing `cchdo.hydro-1.0.2.2/CHANGELOG` & `cchdo.hydro-1.0.2.3/CHANGELOG`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,39 @@
-v1.0.2.3 (unreleased)
+v1.0.2.3 (2023-07-24)
 =====================
-* None yet
+* Add `read_csv` method
+* (bug) Remove the `C_format` and `C_format_source` attributes for non floating point variables. Integer and string values are exact so do not need any sort of format hint. Including a format string for non floating point values is undefined behavior in the netCDF-C Library and can result in crashing.
+* (new) Add `to_coards()` and `to_woce()` accessors to maintain legacy formats at CCHDO.
+* (new) All the `to_*` accessors now support a path argument that will accept a writeable binary mode file like object or a filesystem path to write to.
+* (new) Add a `compact_profile()` accessor that drops the trailing fill values from a profile
+* (new) Add the a `file_seperator` and `keep_seperator` to `cchdo.hydro.exchange.read_exchange()`.
+  The `keep_seperator` argument defualts to True.
+  This is specifically to allow the reading of CTD exchange files that have been concatenated together (rather than zipped).
+  Assuming there is nothing after "END_DATA" and you cat a bunch of _ct1.csv files together, they should be readable if "END_DATA" is passed into the `file_seperator` argument.
+* (new) Add `--dump-data-counts` option to the exchange status generator which will dump a json document containing a object with nc_var name strings to count integers of how many 
+  variables with this name actually contain any data (i.e. are not just entirely fill value).
+* Add a `--version` option to the cli interface
+* (changed) Export `read_exchange` from the top level `cchdo.hydro` namespace.
+* (changed) Bump min `cchdo.params` version to 0.1.21
+* (changed) Dropped netCDF4 as requried for installation, if netCDF4 isn't installed already you can install with the `cchdo.hydro[netcdf4]` optional.
+
+  * While this might seem like an odd choice for a library that started as one to convert WHP Exchange files to netCDf, netCDF 
+    itself is not called untill the very end of the conversion process. Internally, everything is an `xarray.Dataset`. This means you can
+    install this library to read exchange files in tricky enviornments like pyodide or jupyterlite which already tend to have pandas and numpy in them.
+
+* (bug) fix `pressure` variable not having a `_FillValue` attribute
 
 v1.0.2.2 (2022-08-18)
 =====================
 * Support for time values that are equal to 2400, when this is encountered, the date will be set to midnight of the next day.
 * `read_exchange()` will now accept bytes and bytearray objects as input, wrapping data in an `io.BytesIO` is not needed anymore.
 
 v1.0.2.1 (2022-07-08)
 =====================
-* (breaking) fix misspelling of ``convert_exchange``subcommand
+* (breaking) fix misspelling of ``convert_exchange`` subcommand
 * Will not rely on the python universal newlines for reading exchange data
 * Will now combine CDOM parameters into a single variable with a new wavelength dimmension in the last axis.
 * Update the WHP error name lookup to be compatable with cchdo.params v0.1.18, this is now the minimum version
 * Add an ``error_data`` attribute to ``ExchangeParameterUndefError`` that will contain a list of all the unknown ``(param, unit)`` pairs in an exchange file when attempting to read one.
 * Add an ``error_data`` attribute to ``ExchangeDataFlagPairError`` that will contain a list of all the found flag errors as an xarray.Dataset
 * Automatically attempt to use BTLNBR as a fallback if SAMPNO is not present in a bottle file.
 * Automatically reconstruct the date of a missing BTL_DATE param if only BTL_TIME is present.
```

### Comparing `cchdo.hydro-1.0.2.2/LICENSE.md` & `cchdo.hydro-1.0.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cchdo.hydro-1.0.2.2/PKG-INFO` & `cchdo.hydro-1.0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: cchdo.hydro
-Version: 1.0.2.2
+Version: 1.0.2.3
 Home-page: https://github.com/cchdo/hydro
 Author: CCHDO
 Author-email: cchdo@ucsd.edu
 License: BSD 3-clause
-Requires-Python: ~=3.8
+Requires-Python: ~=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: netcdf
+Provides-Extra: matlab
 Provides-Extra: selftest
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: cli
 Provides-Extra: complete
 License-File: LICENSE.md
```

### Comparing `cchdo.hydro-1.0.2.2/cchdo/hydro/__main__.py` & `cchdo.hydro-1.0.2.3/cchdo/hydro/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 import logging
 from pathlib import Path
 from multiprocessing import Pool
 from tempfile import TemporaryDirectory
 import shutil
 from html import escape
 import json
+from collections import Counter
+from typing import List
 
 import click
 from rich.logging import RichHandler
 from rich.progress import track
 
+import xarray as xr
+import numpy as np
+
 log = logging.getLogger(__name__)
 
+from . import __version__
+
 
 def setup_logging(level):
     FORMAT = "%(funcName)s: %(message)s"
     log_handler = RichHandler(level=level)
     logging.basicConfig(
         level="NOTSET", format=FORMAT, datefmt="[%X]", handlers=[log_handler]
     )
@@ -89,20 +96,32 @@
 
     return file_dest
 
 
 from . import __main_helpers as mh
 
 
+def vars_with_value(ds: xr.Dataset) -> List[str]:
+    vars_with_data: List[str] = []
+    for name, var in ds.variables.items():
+        if var.dtype.kind == "f":
+            if np.any(np.isfinite(var)).item():
+                vars_with_data.append(str(name))
+        else:
+            vars_with_data.append(str(name))
+    return vars_with_data
+
+
 @status.command()
 @click.argument("dtype")
 @click.argument("out_dir")
 @click.option("--dump-unknown-params", is_flag=True)
 @click.option("-v", "--verbose", count=True)
-def status_exchange(dtype, out_dir, dump_unknown_params, verbose):
+@click.option("--dump-data-counts", is_flag=True)
+def status_exchange(dtype, out_dir, dump_unknown_params, verbose, dump_data_counts):
     """Generate a bottle conversion status for all ex files of type type in the CCHDO Dataset"""
     from cchdo.hydro._version import version as hydro_version  # type: ignore
     from cchdo.params import _version as params_version  # type: ignore
 
     if verbose == 0:
         setup_logging("CRITICAL")
     if verbose == 1:
@@ -114,14 +133,15 @@
     cruises, files = cchdo_loader(dtype)
     file_paths = []
     for file in track(files, description="Loading data files"):
         file_paths.append((cached_file_loader(file), file))
 
     results = []
     all_unknown_params = {}
+    variables_with_data = []
     with TemporaryDirectory() as temp_dir:
         with Pool() as pool:
             for result in track(
                 pool.imap_unordered(
                     mh.p_file, [(temp_dir, f[0], f[1]) for f in file_paths]
                 ),
                 total=len(file_paths),
@@ -176,14 +196,19 @@
                     log.critical(metadata["cruises"])
                     raise
                 fn = metadata["file_name"]
                 file_id = metadata["id"]
                 if status == 200:
                     tmp_nc = Path(path_or_err)
                     res_nc = nc_path / tmp_nc.name
+
+                    if dump_data_counts:
+                        ds = xr.load_dataset(tmp_nc)
+                        variables_with_data.extend(vars_with_value(ds))
+
                     shutil.copy(tmp_nc, res_nc)
                     f.write(
                         f"""<tr class='table-success'>
                             <td>{crs}</td>
                             <td>{file_id}</td>
                             <td><a href="https://cchdo.ucsd.edu/data/{file_id}/{fn}">{fn}</a></td>
                             <td><a href="nc/{res_nc.name}">{res_nc.name}</a></td>
@@ -210,14 +235,19 @@
                     f.write("""</tr>""")
             f.write("</tbody></table></div></body></html>")
 
     log.info(success_str)
     if dump_unknown_params:
         with open(out_path / f"unknown_params_{dtype}.json", "w") as f:
             json.dump(all_unknown_params, f)
+    if dump_data_counts:
+        with open(out_path / f"params_with_data_{dtype}.json", "w") as f:
+            json.dump(Counter(variables_with_data), f)
 
 
-cli = click.CommandCollection(sources=[convert, status])
+cli = click.version_option(__version__)(
+    click.CommandCollection(sources=[convert, status])
+)
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `cchdo.hydro-1.0.2.2/cchdo/hydro/__main_helpers.py` & `cchdo.hydro-1.0.2.3/cchdo/hydro/__main_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     unknown_params = []
 
     warnings.simplefilter("ignore")
     if ("OSNUM", None) not in WHPNames:
         WHPNames.add_alias(("OSNUM", None), ("EVENT_NUMBER", None))
 
     if file_metadata["data_type"] == "ctd" and ("NITRATE", "UMOL/KG") not in WHPNames:
-
         # HOT names that are a little dangerous to have in the real DB
         WHPNames.add_alias(("NITRATE", "UMOL/KG"), ("CTDNITRATE", "UMOL/KG"))
         WHPNames.add_alias(("CHLPIG", "uG/L"), ("CTDFLUOR", "MG/M^3"))
         WHPNames.add_alias(("CHLPIG", "UG/L"), ("CTDFLUOR", "MG/M^3"))
 
         # other one off things
         WHPNames.add_alias(("CTDFLUOR", "UG/L_UNCALIBRATED"), ("CTDFLUOR", "MG/M^3"))
```

### Comparing `cchdo.hydro-1.0.2.2/cchdo/hydro/accessors.py` & `cchdo.hydro-1.0.2.3/cchdo/hydro/accessors.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,155 @@
-from typing import List, Dict, Optional, Union
+from io import BytesIO, BufferedWriter
+import string
+import re
+import os
+from datetime import datetime, timezone
+from typing import List, Dict, Optional, Union, NamedTuple, Literal
+from zipfile import ZIP_DEFLATED, ZipFile
+from collections import defaultdict
+
 import xarray as xr
 import pandas as pd
 import numpy as np
-import string
-import re
 
 from cchdo.params import WHPNames, WHPName
 
 from .exchange import FileType, all_same, check_flags as _check_flags
+from .exchange import flatten_cdom_coordinate, extract_numeric_precisions
 
+FLAG_NAME = "cchdo.hydro._qc"
+ERROR_NAME = "cchdo.hydro._error"
 
-class CCHDOAccessorBase:
-    """Class base for CCHDO accessors
+PathType = Union[str, bytes, os.PathLike]
 
-    saves the xarray object to self._obj for all the subclasses
-    """
 
-    def __init__(self, xarray_obj: Union[xr.DataArray, xr.Dataset]):
-        self._obj = xarray_obj
+def write_or_return(
+    data: bytes, path_or_fobj: Optional[Union[PathType, BufferedWriter]] = None
+) -> Optional[bytes]:
+    # assume path_or_fobj is an open filelike
+    if path_or_fobj is None:
+        return data
+
+    if isinstance(path_or_fobj, BufferedWriter):
+        try:
+            path_or_fobj.write(data)
+        except TypeError as error:
+            raise TypeError("File must be open for bytes writing") from error
+    else:
+        with open(path_or_fobj, "wb") as f:
+            f.write(data)
+
+    return None
+
+
+# maybe temp location for FQ merge machinery
+class FQPointKey(NamedTuple):
+    expocode: str
+    station: str
+    cast: int
+    sample: str
+
+
+class FQProfileKey(NamedTuple):
+    expocode: str
+    station: str
+    cast: int
+
+
+class WHPIndxer:
+    def __init__(self, obj: xr.Dataset) -> None:
+        self.n_prof = pd.MultiIndex.from_arrays(
+            [
+                obj.expocode.data,
+                obj.station.data,
+                obj.cast.data,
+            ],
+            names=["expocode", "station", "cast"],
+        )
+        self.n_level = [
+            pd.MultiIndex.from_arrays([prof.sample.data], names=["sample"])
+            for _, prof in obj.groupby("N_PROF")
+        ]
 
+    def __getitem__(self, key: Union[FQProfileKey, FQPointKey]):
+        prof_idx = self.n_prof.get_loc((key.expocode, key.station, key.cast))
+        if isinstance(key, FQPointKey):
+            level_idx = self.n_level[prof_idx].get_loc((key.sample))
+        else:
+            level_idx = slice(None)
+
+        return prof_idx, level_idx
+
+
+NormalizedFQ = Dict[Union[FQProfileKey, FQPointKey], Dict[str, Union[str, float]]]
+
+
+def normalize_fq(
+    fq: List[Dict[str, Union[str, float]]], *, check_dupes=True
+) -> NormalizedFQ:
+    normalized: NormalizedFQ = defaultdict(dict)
+    key: Union[FQProfileKey, FQPointKey]
+    for line in fq:
+        expocode = str(line.pop("EXPOCODE"))
+        station = str(line.pop("STNNBR"))
+        cast = int(line.pop("CASTNO"))
+        try:
+            sample = str(line.pop("SAMPNO"))
+        except KeyError:
+            key = FQProfileKey(expocode, station, cast)
+        else:
+            key = FQPointKey(expocode, station, cast, sample)
+
+        if check_dupes is True:
+            shared_keys = normalized[key].keys() & line.keys()
+            if len(shared_keys) != 0:
+                raise ValueError(f"Duplicate input data found: {key}")
+
+        normalized[key].update(line)
+
+    return normalized
+
+
+def fq_get_precisions(fq: NormalizedFQ) -> Dict[str, int]:
+    collect: Dict[str, List[str]] = defaultdict(list)
+    for value in fq.values():
+        for param, data in value.items():
+            if isinstance(data, str):
+                collect[param].append(data)
+
+    return {
+        param: extract_numeric_precisions(data).item()
+        for param, data in collect.items()
+    }
 
-class MatlabAccessor(CCHDOAccessorBase):
-    """Accessor containing the experimental matlab machinery"""
+
+FTypeOptions = Literal["cf", "exchange"]
+
+
+class CCHDOAccessor:
+    def __init__(self, xarray_obj: xr.Dataset):
+        self._obj = xarray_obj
 
     def to_mat(self, fname):
         """Experimental Matlab .mat data file generator
 
         The support for netCDF files in Matlab is really bad.
         Matlab also has no built in support for the standards
         we are trying to follow (CF, ACDD), the most egregious
         lack of support is how to deal with times in netCDF files.
         This was an attempt to make a mat file which takes
         care of some of the things matlab won't do for you.
         It requires scipy to function.
 
         The file it produces is in no way stable.
         """
-        from scipy.io import savemat as scipy_savemat
+        try:
+            from scipy.io import savemat as scipy_savemat  # noqa
+        except ImportError as error:
+            raise ImportError("scipy is required for mat file saving") from error
 
         mat_dict = {}
         data = self._obj.to_dict()
 
         # flatten
         for coord, value in data["coords"].items():
             del value["dims"]
@@ -67,17 +176,23 @@
                     value["data"] = dt_list_to_str_list(value["data"])
 
             if "status_flag" in value.get("attrs", {}).get("standard_name", ""):
                 value["data"] = np.nan_to_num(value["data"], nan=9)
 
         scipy_savemat(fname, mat_dict)
 
+    def to_coards(self, path=None):
+        from .legacy.coards import to_coards
 
-class WoceAccessor(CCHDOAccessorBase):
-    """Accessor containing woce file output machinery"""
+        return write_or_return(to_coards(self._obj), path)
+
+    def to_woce(self, path=None):
+        from .legacy.woce import to_woce
+
+        return write_or_return(to_woce(self._obj), path)
 
     def to_sum(self, path=None):
         """netCDF to WOCE sumfile maker
 
         This is missing some information that is not included anymore (wire out, height above bottom).
         It is especially lacking in including woce parameter IDs
         """
@@ -140,47 +255,39 @@
             ">",  # wire out
             ">",  # pres
             ">",  # no bottles
             "<",  # params
             "<",  # comments
         ]
 
-        def sum_lat(deg_str):
-            deg_str = str(deg_str)
-            deg, dec = deg_str.split(".")
-            deg = int(deg)
-            if deg > 0:
+        def sum_lat(deg_float):
+            deg = abs(int(deg_float))
+            if deg_float >= 0:
                 hem = "N"
+                dec = deg_float % 1
             else:
                 hem = "S"
-            deg = abs(deg)
-
-            dec_len = len(dec)
-            dec = int(dec)
+                dec = -(deg_float % -1)
 
-            min = 60 * (dec / (10**dec_len))
+            mins = 60 * dec
 
-            return f"{deg:>2d} {min:05.2f} {hem}"
+            return f"{deg:>2d} {mins:05.2f} {hem}"
 
-        def sum_lon(deg_str):
-            deg_str = str(deg_str)
-            deg, dec = deg_str.split(".")
-            deg = int(deg)
-            if deg > 0:
+        def sum_lon(deg_float):
+            deg = abs(int(deg_float))
+            if deg_float >= 0:
                 hem = "E"
+                dec = deg_float % 1
             else:
                 hem = "W"
-            deg = abs(deg)
+                dec = -(deg_float % -1)
 
-            dec_len = len(dec)
-            dec = int(dec)
+            mins = 60 * dec
 
-            min = 60 * (dec / (10**dec_len))
-
-            return f"{deg:>3d} {min:05.2f} {hem}"
+            return f"{deg:>3d} {mins:05.2f} {hem}"
 
         col_widths = [len(s) for s in SUM_COLUMN_HEADERS_1]
         col_widths = [max(x, len(s)) for x, s in zip(col_widths, SUM_COLUMN_HEADERS_2)]
 
         sum_rows = []
         for _, prof in self._obj.groupby("N_PROF"):
             dt = pd.to_datetime(prof.time.values)
@@ -237,25 +344,18 @@
         HEADERS_1 = format_str.format(*SUM_COLUMN_HEADERS_1)
         HEADERS_2 = format_str.format(*SUM_COLUMN_HEADERS_2)
         SEP_LINE = "-" * (sum(col_widths) + len(col_widths))
         SUM_ROWS = []
         for row in sum_rows:
             SUM_ROWS.append(format_str.format(*row))
 
-        sum_file = "\n".join([COMMENTS, HEADERS_1, HEADERS_2, SEP_LINE, *SUM_ROWS])
-        if path is not None:
-            with open(path, "w", encoding="ascii") as f:
-                f.write(sum_file)
-                return
-
-        return sum_file
-
-
-class GeoAccessor(CCHDOAccessorBase):
-    """Accessor providing geo_interface machinery"""
+        sum_file = "\n".join(
+            [COMMENTS, HEADERS_1, HEADERS_2, SEP_LINE, *SUM_ROWS]
+        ).encode("ascii")
+        return write_or_return(sum_file, path)
 
     @property
     def __geo_interface__(self):
         """The station positions as a MultiPoint geo interface
 
         See https://gist.github.com/sgillies/2217756
         """
@@ -274,88 +374,127 @@
             # Website only supports LineString which must contain at least 2 points
             # They can be the same point though
             geo["coordinates"].append(geo["coordinates"][0])
 
         geo["type"] = "LineString"
         return geo
 
-
-class MiscAccessor(CCHDOAccessorBase):
-    """Accessor with misc functions that don't fit in some other category"""
-
-    def gen_fname(self, ftype="cf") -> str:
-        """Generate a human friendly netCDF filename for this object"""
-        ds = self._obj
+    @staticmethod
+    def _gen_fname(
+        expocode: str,
+        station: str,
+        cast: int,
+        profile_type: FileType,
+        profile_count: int = 1,
+        ftype: FTypeOptions = "cf",
+    ) -> str:
         allowed_chars = set(f"._{string.ascii_letters}{string.digits}")
 
         ctd_one = "ctd.nc"
         ctd_many = "ctd.nc"
         bottle = "bottle.nc"
 
         if ftype == "exchange":
             ctd_one = "ct1.csv"
             ctd_many = "ct1.zip"
             bottle = "hy1.csv"
 
-        expocode = np.atleast_1d(ds["expocode"])[0]
-        station = np.atleast_1d(ds["station"])[0]
-        cast = np.atleast_1d(ds["cast"])[0]
-
-        profile_type = np.atleast_1d(ds["profile_type"])[0]
-
-        if profile_type == FileType.BOTTLE.value:
+        if profile_type == FileType.BOTTLE:
             fname = f"{expocode}_{bottle}"
-        elif profile_type == FileType.CTD.value and len(ds.get("N_PROF", [])) > 1:
+        elif profile_type == FileType.CTD and profile_count > 1:
             fname = f"{expocode}_{ctd_many}"
         else:
             fname = f"{expocode}_{station}_{cast:.0f}_{ctd_one}"
 
         for char in set(fname) - allowed_chars:
             fname = fname.replace(char, "_")
 
         return fname
 
+    def gen_fname(self, ftype: FTypeOptions = "cf") -> str:
+        """Generate a human friendly netCDF filename for this object"""
+
+        expocode = np.atleast_1d(self._obj["expocode"])[0]
+        station = np.atleast_1d(self._obj["station"])[0]
+        cast = np.atleast_1d(self._obj["cast"])[0]
+
+        profile_type = FileType(np.atleast_1d(self._obj["profile_type"])[0])
+        profile_count = len(self._obj.get("N_PROF", []))
+
+        return self._gen_fname(
+            expocode, station, cast, profile_type, profile_count, ftype
+        )
+
+    def compact_profile(self):
+        """Drop the trailing empty data from a profile.
+
+        Because we use the incomplete multidimensional array representation of profiles
+        there is often "wasted space" at the end of any profile that is not the longest one.
+        This accessor drops that wasted space for xr.Dataset objects containing a single profile
+        """
+        if self._obj.dims["N_PROF"] != 1:
+            raise NotImplementedError(
+                "Cannot compact Dataset with more than one profile"
+            )
+        return self._obj.isel(N_LEVELS=(self._obj.sample != "")[0])
+
+    date_names = {WHPNames["DATE"], WHPNames["BTL_DATE"]}
+    time_names = {WHPNames["TIME"], WHPNames["BTL_TIME"]}
+
+    @property
+    def file_type(self):
+        # TODO profile_type is guaranteed to be present
+        # TODO profile_type must have C or D as the value
+        profile_type = self._obj.profile_type
+        if not all_same(profile_type.values):
+            raise NotImplementedError(
+                "Unable to convert a mix of ctd and bottle (or unknown) dtypes"
+            )
 
-class ExchangeAccessor(CCHDOAccessorBase):
-    """Class containing the to_exchange functionn"""
+        if profile_type[0] == FileType.CTD.value:
+            return FileType.CTD
+        elif profile_type[0] == FileType.BOTTLE.value:
+            return FileType.BOTTLE
+        else:
+            raise NotImplementedError("Unknown profile type encountered")
 
     @staticmethod
     def cchdo_c_format_precision(c_format: str) -> Optional[int]:
         if not c_format.endswith("f"):
             return None
 
         f_format = re.compile(r"\.(\d+)f")
         if (match := f_format.search(c_format)) is not None:
             return int(match.group(1))
         return match
 
-    @staticmethod
     def _make_params_units_line(
+        self,
         params: Dict[WHPName, xr.DataArray],
-        flags: Dict[WHPName, xr.DataArray],
-        errors: Dict[WHPName, xr.DataArray],
     ):
         plist = []
         ulist = []
-        for param in params:
+        for param, dataarray in sorted(params.items()):
+            if self.file_type == FileType.CTD and (
+                param.scope != "sample" or param.nc_name == "sample"
+            ):
+                continue
             plist.append(param.whp_name)
             unit = param.whp_unit
             if unit is None:
                 unit = ""
 
             ulist.append(unit)
 
-            if param in flags:
-                plist.append(f"{param.whp_name}_FLAG_W")
+            if (flag := dataarray.attrs.get(FLAG_NAME)) is not None:
+                plist.append(flag.attrs["whp_name"])
                 ulist.append("")
 
-            if param in errors:
-                if param.error_name is None:
-                    raise ValueError(f"No error name for {param}")
-                plist.append(param.error_name)
+            if (error := dataarray.attrs.get(ERROR_NAME)) is not None:
+                plist.append(error.attrs["whp_name"])
                 ulist.append(unit)
 
         return ",".join(plist), ",".join(ulist)
 
     @staticmethod
     def _whpname_from_attrs(attrs) -> List[WHPName]:
         params = []
@@ -366,110 +505,70 @@
                 params.append(WHPNames[(combined, unit)])
         else:
             if (param, unit) in WHPNames.error_cols:
                 return []
             params.append(WHPNames[(param, unit)])
         return params
 
-    def to_exchange(self):
-        """Convert a CCHDO CF netCDF dataset to exchange"""
-        # all of the todo comments are for documenting/writing validators
-
-        date_names = {WHPNames["DATE"], WHPNames["BTL_DATE"]}
-        time_names = {WHPNames["TIME"], WHPNames["BTL_TIME"]}
-
-        # TODO guarantee these coordinates
-        ds = self._obj.reset_coords(
-            [
-                "expocode",
-                "station",
-                "cast",
-                "sample",
-                "time",
-                "latitude",
-                "longitude",
-                "pressure",
-            ]
-        ).stack(ex=("N_PROF", "N_LEVELS"))
-
-        # TODO profile_type is guaranteed to be present
-        # TODO profile_type must have C or D as the value
-        profile_type = ds.profile_type
-        if not all_same(profile_type.values):
-            raise NotImplementedError(
-                "Unable to convert a mix of ctd and bottle dtypes"
-            )
-
-        if profile_type[0] != FileType.BOTTLE.value:
-            raise NotImplementedError("CTD conversion not implimentaed yet")
-
-        output = []
-        output.append("BOTTLE,date_initals")
-
-        if len(comments := ds.attrs.get("comments", "")) > 0:
-            for comment_line in comments.splitlines():
-                output.append(f"#{comment_line}")
-
-        # collect all the Exchange variables
-        # TODO, all things that appear in an exchange file, must have WHP name
-        exchange_vars = ds.filter_by_attrs(whp_name=lambda name: name is not None)
-        params: Dict[WHPName, xr.DataArray] = {}
-        flags = {}
-        errors = {}
-        for var in exchange_vars.values():
-            whp_params = self._whpname_from_attrs(var.attrs)
-            for param in whp_params:
-                params[param] = var
-
-            ancillary_vars_attr = var.attrs.get("ancillary_variables")
-            if ancillary_vars_attr is None:
+    def _make_ctd_headers(self, params) -> List[str]:
+        headers = {}
+        for param, da in params.items():
+            if param.scope != "profile":
                 continue
 
-            # CF says these need to be space seperated
-            ancillary_vars = ancillary_vars_attr.split(" ")
-            for ancillary_var in ancillary_vars:
-                ancillary = ds[ancillary_var]
-
-                standard_name = ancillary.attrs.get("standard_name")
-                if standard_name is None and ancillary.attrs.get("whp_name") is None:
-                    # TODO maybe raise...
-                    continue
-
-                # currently there are three types of ancillary: flags, errors, and analytical temps (e.g. for pH)
-                if standard_name == "temperature_of_analysis_of_sea_water":
-                    # this needs to get treated like a param
-                    for param in self._whpname_from_attrs(ancillary.attrs):
-                        params[param] = ancillary
-
-                if standard_name == "status_flag":
-                    for param in whp_params:
-                        flags[param] = ancillary
-
-                # TODO find a way to test this
-                if ancillary.attrs.get("whp_name") in WHPNames.error_cols:
-                    for param in whp_params:
-                        errors[param] = ancillary
+            date_or_time = None
+            if param in self.date_names:
+                date_or_time = "date"
+                value = da.dt.strftime("%Y%m%d").to_numpy()[0]
+            elif param in self.time_names:
+                date_or_time = "time"
+                value = da.dt.round("T").dt.strftime("%H%M").to_numpy()[0]
+            else:
+                try:
+                    data = da.values[0].item()
+                except AttributeError:
+                    data = da.values[0]
 
-        # add the params and units line
-        output.extend(self._make_params_units_line(params, flags, errors))
+                numeric_precision_override = self.cchdo_c_format_precision(
+                    da.attrs.get("C_format", "")
+                )
+                value = param.strfex(
+                    data,
+                    date_or_time=date_or_time,
+                    numeric_precision_override=numeric_precision_override,
+                )
+            headers[param.whp_name] = value.strip()
+        return [
+            f"NUMBER_HEADERS = {len(headers) + 1}",
+            *[f"{key} = {value}" for key, value in headers.items()],
+        ]
 
+    def _make_data_block(self, params) -> List[str]:
         # TODO N_PROF is guaranteed
-        # for _, prof in ds.groupby("N_PROF"):
-        #    # TODO sample is empty/null string for... non samples
-        #    valid_levels = prof.sample != ""
         valid_levels = params[WHPNames["SAMPNO"]] != ""
         data_block = []
-        for param, da in params.items():
+        for param, da in sorted(params.items()):
+            if self.file_type == FileType.CTD and (
+                param.scope != "sample" or param.nc_name == "sample"
+            ):
+                continue
             date_or_time = None
-            if param in date_names:
+            # TODO, deal with missing time in BTL_DATE
+            if param in self.date_names:
                 date_or_time = "date"
                 values = da[valid_levels].dt.strftime("%Y%m%d").to_numpy().tolist()
-            elif param in time_names:
+            elif param in self.time_names:
                 date_or_time = "time"
-                values = da[valid_levels].dt.strftime("%H%M").to_numpy().tolist()
+                values = (
+                    da[valid_levels]
+                    .dt.round("T")
+                    .dt.strftime("%H%M")
+                    .to_numpy()
+                    .tolist()
+                )
             else:
                 data = np.nditer(da[valid_levels], flags=["refs_ok"])
                 numeric_precision_override = self.cchdo_c_format_precision(
                     da.attrs.get("C_format", "")
                 )
                 values = [
                     param.strfex(
@@ -478,103 +577,219 @@
                         numeric_precision_override=numeric_precision_override,
                     )
                     for v in data
                 ]
 
             data_block.append(values)
 
-            if param in flags:
-                data = np.nditer(flags[param][valid_levels])
+            if (flags := da.attrs.get(FLAG_NAME)) is not None:
+                data = np.nditer(flags[valid_levels])
                 flag = [param.strfex(v, flag=True) for v in data]
                 data_block.append(flag)
 
-            if param in errors:
-                data = np.nditer(errors[param][valid_levels])
-                numeric_precision_override = (
-                    self.cchdo_c_format_precision(da.attrs.get("C_format", "")),
+            if (errors := da.attrs.get(ERROR_NAME)) is not None:
+                data = np.nditer(errors[valid_levels])
+                numeric_precision_override = self.cchdo_c_format_precision(
+                    da.attrs.get("C_format", "")
                 )
                 error = [
                     param.strfex(
                         v,
                         date_or_time=date_or_time,
                         numeric_precision_override=numeric_precision_override,
                     )
                     for v in data
                 ]
                 data_block.append(error)
+        return data_block
 
-        for row in zip(*data_block):
-            output.append(",".join(str(cell) for cell in row))
-
-        output.append("END_DATA\n")
-
-        return "\n".join(output)
+    def _get_comments(self):
+        output = []
+        if len(comments := self._obj.attrs.get("comments", "")) > 0:
+            for comment_line in comments.splitlines():
+                output.append(f"#{comment_line}")
+        return output
 
+    def to_whp_columns(self, compact=False):
+        # collect all the Exchange variables
+        # TODO, all things that appear in an exchange file, must have WHP name
+        ds = flatten_cdom_coordinate(self._obj)
 
-class WHPIndxer:
-    def __init__(self, obj: xr.Dataset) -> None:
-        self.n_prof = pd.MultiIndex.from_arrays(
+        ds = self._obj.reset_coords(
             [
-                obj.expocode.data,
-                obj.station.data,
-                obj.cast.data,
-            ],
-            names=["expocode", "station", "cast"],
+                "expocode",
+                "station",
+                "cast",
+                "sample",
+                "time",
+                "latitude",
+                "longitude",
+                "pressure",
+            ]
         )
-        self.n_level = [
-            pd.MultiIndex.from_arrays([prof.sample.data], names=["sample"])
-            for _, prof in obj.groupby("N_PROF")
-        ]
 
-    def __getitem__(self, key):
-        expocode = str(key.pop("EXPOCODE"))
-        station = str(key.pop("STNNBR"))
-        cast = int(key.pop("CASTNO"))
-        sample = str(key.pop("SAMPNO"))
-        prof_idx = self.n_prof.get_loc((expocode, station, cast))
-        level_idx = self.n_level[prof_idx].get_loc((sample))
+        ds = ds.stack(ex=("N_PROF", "N_LEVELS"))
+        if compact:
+            ds = ds.isel(ex=(ds.sample != ""))
 
-        return prof_idx, level_idx
+        exchange_vars = ds.filter_by_attrs(whp_name=lambda name: name is not None)
+        params: Dict[WHPName, xr.DataArray] = {}
+        for var in exchange_vars.values():
+            whp_params = self._whpname_from_attrs(var.attrs)
+            for param in whp_params:
+                params[param] = var
+
+            ancillary_vars_attr = var.attrs.get("ancillary_variables")
+            if ancillary_vars_attr is None:
+                continue
+
+            # CF says these need to be space seperated
+            ancillary_vars = ancillary_vars_attr.split(" ")
+            for ancillary_var in ancillary_vars:
+                ancillary = ds[ancillary_var]
+
+                standard_name = ancillary.attrs.get("standard_name")
+                if standard_name is None and ancillary.attrs.get("whp_name") is None:
+                    # TODO maybe raise...
+                    continue
+
+                # TODO find a way to test this
+                if (
+                    ancillary.attrs.get("whp_name"),
+                    ancillary.attrs.get("whp_unit"),
+                ) in WHPNames.error_cols:
+                    for param in whp_params:
+                        if param.error_name is None:
+                            raise ValueError(f"No error name for {param}")
+                        ancillary.attrs["whp_name"] = param.error_name
+                        params[param].attrs[ERROR_NAME] = ancillary
+
+                # currently there are three types of ancillary: flags, errors, and analytical temps (e.g. for pH)
+                elif standard_name == "temperature_of_analysis_of_sea_water":
+                    # this needs to get treated like a param
+                    for param in self._whpname_from_attrs(ancillary.attrs):
+                        params[param] = ancillary
+
+                elif standard_name == "status_flag":
+                    for param in whp_params:
+                        ancillary.attrs["whp_name"] = f"{param.whp_name}_FLAG_W"
+                        params[param].attrs[FLAG_NAME] = ancillary
+
+        return params
+
+    def to_exchange(self, path=None):
+        """Convert a CCHDO CF netCDF dataset to exchange"""
+        # all of the todo comments are for documenting/writing validators
+        output_files = {}
+        if self.file_type == FileType.CTD:
+            for _, ds1 in self._obj.groupby("N_PROF", squeeze=False):
+                fname = ds1.cchdo.gen_fname(ftype="exchange")
+
+                output = []
+                output.append(f"CTD,{datetime.now(timezone.utc):%Y%m%d}CCHHYDRO")
+                output.extend(self._get_comments())
+
+                params = ds1.cchdo.to_whp_columns()
+                output.extend(self._make_ctd_headers(params))
+                output.extend(self._make_params_units_line(params))
+
+                data_block = self._make_data_block(params)
+                for row in zip(*data_block):
+                    output.append(",".join(str(cell) for cell in row))
+
+                output.append("END_DATA\n")
+                output_files[fname] = "\n".join(output).encode("utf8")
+
+        if self.file_type == FileType.BOTTLE:
+            fname = self._obj.cchdo.gen_fname(ftype="exchange")
+
+            output = []
+            output.append(f"BOTTLE,{datetime.now(timezone.utc):%Y%m%d}CCHHYDRO")
+            output.extend(self._get_comments())
+            params = self._obj.cchdo.to_whp_columns()
+
+            # add the params and units line
+            output.extend(self._make_params_units_line(params))
+
+            data_block = self._make_data_block(params)
+
+            for row in zip(*data_block):
+                output.append(",".join(str(cell) for cell in row))
+
+            output.append("END_DATA\n")
+            output_files[fname] = "\n".join(output).encode("utf8")
+
+        if len(output_files) == 1:
+            return write_or_return(list(output_files.values())[0], path)
+        output_zip = BytesIO()
+        with ZipFile(output_zip, "w", compression=ZIP_DEFLATED) as zipfile:
+            for fname, data in output_files.items():
+                zipfile.writestr(fname, data)
 
+        output_zip.seek(0)
+        return write_or_return(output_zip.read(), path)
 
-class MergeFQAccessor(CCHDOAccessorBase):
     # Until I figure out how to use the pandas machinery (or the explict index project of xarray pays off)
     # I will use a "custom" indexer here to index into the variables
     # This will rely on the N_PROF and N_LEVELS (with extra at some point)
     # * N_PROF will be indexed with (expocode, station, cast)
     # * N_LEVELS will be subindexd with (sample)
-    def merge_fq(self, fq, check_flags=True):
+    def merge_fq(self, fq: List[Dict[str, Union[str, float]]], *, check_flags=True):
+        # TODOs...
+        # * (default True) restrict to open "slots" of non flag 9s
+        # * Vectorize updates
+        # * Update history attribute...
+        now = datetime.now(timezone.utc)
         new_obj = self._obj.copy(deep=True)
         idxer = WHPIndxer(new_obj)
 
-        for line in fq:
-            prof, level = idxer[line]
-            for param, value in line.items():
+        normalized_fq = normalize_fq(fq)
+        input_precisions = fq_get_precisions(normalized_fq)
+
+        for key, values in normalized_fq.items():
+            prof, level = idxer[key]
+            for param, value in values.items():
                 if param in WHPNames.error_cols:
                     whpname = WHPNames.error_cols[param]
-                    new_obj[whpname.nc_name_error][prof, level] = value
-                if param.endswith("_FLAG_W"):
-                    whpname = WHPNames[param[:-7]]
+                    col_ref = new_obj[whpname.nc_name_error]
+                    col_ref[prof, level] = value
+                    col_ref.attrs["date_modified"] = now.isoformat(timespec="seconds")
+                    if param in input_precisions and whpname.dtype == "decimal":
+                        new_c_format = f"%.{input_precisions[param]}f"
+                        new_c_format_source = "input_file"
+                        if (
+                            col_ref.attrs.get("C_format") != new_c_format
+                            or col_ref.attrs.get("C_format_source")
+                            != new_c_format_source
+                        ):
+                            col_ref.attrs["C_format"] = new_c_format
+                            col_ref.attrs["C_format_source"] = new_c_format_source
+                            col_ref.attrs["date_metadata_modified"] = now.isoformat(
+                                timespec="seconds"
+                            )
+                elif (whpname := param.removesuffix("_FLAG_W")) != param:
+                    whpname = WHPNames[whpname]
                     new_obj[whpname.nc_name_flag][prof, level] = value
                 else:
                     whpname = WHPNames[param]
-                    new_obj[whpname.nc_name][prof, level] = value
-
+                    col_ref = new_obj[whpname.nc_name]
+                    col_ref[prof, level] = value
+                    col_ref.attrs["date_modified"] = now.isoformat(timespec="seconds")
+                    if param in input_precisions and whpname.dtype == "decimal":
+                        new_c_format = f"%.{input_precisions[param]}f"
+                        new_c_format_source = "input_file"
+                        if (
+                            col_ref.attrs.get("C_format") != new_c_format
+                            or col_ref.attrs.get("C_format_source")
+                            != new_c_format_source
+                        ):
+                            col_ref.attrs["C_format"] = new_c_format
+                            col_ref.attrs["C_format_source"] = new_c_format_source
+                            col_ref.attrs["date_metadata_modified"] = now.isoformat(
+                                timespec="seconds"
+                            )
         if check_flags:
             _check_flags(new_obj)
         return new_obj
 
 
-class CCHDOAccessor(
-    ExchangeAccessor,
-    GeoAccessor,
-    WoceAccessor,
-    MatlabAccessor,
-    MiscAccessor,
-    MergeFQAccessor,
-):
-    """Collect all the accessors into a single class"""
-
-    ...
-
-
 xr.register_dataset_accessor("cchdo")(CCHDOAccessor)
```

### Comparing `cchdo.hydro-1.0.2.2/cchdo/hydro/conformance.py` & `cchdo.hydro-1.0.2.3/cchdo/hydro/conformance.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 
     @property
     def ok(self) -> bool:
         return self.error is None and self.warning is None
 
 
 class CCHDOnetCDF10:
-
     __cchdo_version__ = "1.0"
 
     def check_cf_version(self, ds):
         cf_version = "CF-1.8"
         try:
             conventions = ds.attrs["Conventions"]
         except AttributeError:
```

### Comparing `cchdo.hydro-1.0.2.2/cchdo/hydro/exchange/__init__.py` & `cchdo.hydro-1.0.2.3/cchdo/hydro/exchange/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,16 +48,14 @@
 
     CCHDO_VERSION = ".".join(hydro_version.split(".")[:2])
     if "dev" in hydro_version:
         CCHDO_VERSION = hydro_version
 except ImportError:
     hydro_version = CCHDO_VERSION = "unknown"
 
-__all__ = ["read_exchange"]
-
 log = logging.getLogger(__name__)
 
 DIMS = ("N_PROF", "N_LEVELS")
 
 EXPOCODE = WHPNames["EXPOCODE"]
 STNNBR = WHPNames["STNNBR"]
 CASTNO = WHPNames["CASTNO"]
@@ -171,26 +169,30 @@
     :returns: Mapping of :py:class:`~hydro.data.WHPName` to column indicies for the status flag column
     :rtype: dict with keys of :py:class:`~hydro.data.WHPName` and values of int
     :raises ExchangeFlagUnitError: if the flag column has units other than None
     :raises ExchangeFlaglessParameterError: if the flag column is for a parameter not allowed to have status flags
     :raises ExchangeOrphanFlagError: if the flag column is for a parameter not in the passed in mapping of whp_params
     """
     param_flags = {}
-    whp_params_names = {x.whp_name: x for x in whp_params.keys()}
+    whp_params_names = whp_params.keys()
 
     for index, (param, unit) in enumerate(params_units):
         if not param.endswith("_FLAG_W"):
             continue
 
         if unit is not None:
             raise ExchangeFlagUnitError
 
         data_col = param.replace("_FLAG_W", "")
         try:
-            whpname = whp_params_names[data_col]
+            whpname = WHPNames[data_col]
+
+            if whpname not in whp_params_names:
+                raise KeyError
+
             if whpname.flag_w is None:
                 raise ExchangeFlaglessParameterError(f"{data_col}")
             param_flags[whpname] = index
         except KeyError as error:
             # we might have an alias...
             for name in whp_params:
                 potential = [k[0] for k, v in WHPNames.items() if v == name]
@@ -242,14 +244,48 @@
     return header, dtype(value)
 
 
 def _is_all_dataarray(val: List[Any]) -> TypeGuard[List[xr.DataArray]]:
     return all(isinstance(obj, xr.DataArray) for obj in val)
 
 
+def flatten_cdom_coordinate(dataset: xr.Dataset) -> xr.Dataset:
+    """Takes the a dataset with a CDOM wavelength and explocdes it back into individual variables"""
+    if "cdom" not in dataset:
+        return dataset
+
+    keys = ["cdom"]
+    if "cdom_qc" in dataset:
+        keys.append("cdom_qc")
+
+    ds = dataset.copy()
+    cdom_var = ds[keys]
+    for cdom_wavelength, arr in cdom_var.groupby("CDOM_WAVELENGTHS"):
+        cdom = arr["cdom"].copy()
+
+        cdom_qc = arr.get("cdom_qc")
+        if cdom_qc is not None:
+            cdom_qc = cdom_qc.copy()
+
+        cdom.attrs["whp_name"] = cdom.attrs["whp_name"].format(
+            CDOM_WAVELENGTHS=cdom_wavelength
+        )
+
+        whp_name = WHPNames[f'{cdom.attrs["whp_name"]} [{cdom.attrs["whp_unit"]}]']
+
+        if cdom_qc is not None:
+            cdom.attrs["ancillary_variables"] = whp_name.nc_name_flag
+
+        ds[whp_name.nc_name] = cdom
+        if cdom_qc is not None:
+            ds[whp_name.nc_name_flag] = cdom_qc
+
+    return ds.drop(keys)
+
+
 def add_cdom_coordinate(dataset: xr.Dataset) -> xr.Dataset:
     """Find all the paraters in the cdom group and add their wavelength in a new coordinate"""
 
     # this needs to be a set to deal with the potential for aliasesd names
     cdom_names = {
         name.nc_name
         for name in filter(lambda x: x.nc_group == "cdom", WHPNames.values())
@@ -509,15 +545,14 @@
         if "status_flag" in data.attrs["standard_name"]:
             flag_vars.append(var_name)
 
     # match flags with their data vars
     # it is legal in CF for one set of flags to apply to multiple vars
     flag_errors = {}
     for flag_var in flag_vars:
-
         # get the flag and check attrs for defs
         flag_da = dataset[flag_var]
         conventions = None
         for flag in woce_flags:
             if flag_da.attrs.get("conventions", "").startswith(flag):
                 conventions = flag
                 break
@@ -916,17 +951,19 @@
         whp_error_precisions = {}
 
         for param, idx in self.whp_params.items():
             param_col = np_db[:, idx]
             fill_spaces = _get_fill_locs(param_col, fill_values)
             if param.dtype in ("decimal", "integer"):
                 if not _is_valid_exchange_numeric(param_col):
-                    raise ValueError("exchange numeric data has bad chars")
+                    raise ValueError(
+                        f"exchange numeric data for {param.whp_name} has bad chars"
+                    )
                 if precision_source == "file":
-                    whp_param_precisions[param] = _extract_numeric_precisions(param_col)
+                    whp_param_precisions[param] = extract_numeric_precisions(param_col)
                 param_col[fill_spaces] = "nan"
             if param.dtype == "string":
                 param_col[fill_spaces] = ""
             whp_param_cols[param] = param_col.astype(dtype_map[param.dtype])
 
         for param, idx in self.whp_flags.items():
             param_col = np_db[:, idx]
@@ -939,15 +976,15 @@
             fill_spaces = _get_fill_locs(param_col, fill_values)
             if param.dtype in ("decimal", "integer"):
                 if not _is_valid_exchange_numeric(param_col):
                     raise ValueError(
                         f"{param} error col exchange numeric data has bad chars"
                     )
                 if precision_source == "file":
-                    whp_error_precisions[param] = _extract_numeric_precisions(param_col)
+                    whp_error_precisions[param] = extract_numeric_precisions(param_col)
                 param_col[fill_spaces] = "nan"
             whp_error_cols[param] = param_col.astype(dtype_map[param.dtype])
 
         comments = "\n".join([*self.stamp, *self.comments])
         del self._raw_lines
 
         return _ExchangeData(
@@ -1048,15 +1085,17 @@
             units_idx=units,
             data_slice=slice(data_start, data_end),
             post_data_slice=slice(post_data_start, post_data_end),
             _raw_lines=lines,
         )
 
 
-def _extract_numeric_precisions(data: npt.NDArray[np.str_]) -> npt.NDArray[np.int_]:
+def extract_numeric_precisions(
+    data: Union[List[str], npt.NDArray[np.str_]]
+) -> npt.NDArray[np.int_]:
     """Get the numeric precision of a printed decimal number"""
     # magic number explain: np.char.partition expands each element into a 3-tuple
     # of (pre, sep, post) of some sep, in our case a "." char.
     # We only want the post bits [idx 2] (the number of chars after a decimal seperator)
     # of the last axis.
     numeric_parts = np.char.partition(data, ".")[..., 2]
     str_lens = np.char.str_len(numeric_parts)
@@ -1077,15 +1116,14 @@
 
 
 def _combine_dt_ndarray(
     date_arr: npt.NDArray[np.str_],
     time_arr: Optional[npt.NDArray[np.str_]] = None,
     time_pad=False,
 ) -> np.ndarray:
-
     # TODO: When min pyver is 3.10, maybe consider pattern matching here
     def _parse_date(date_val: str) -> np.datetime64:
         if date_val == "":
             return np.datetime64("nat")
         return np.datetime64(datetime.strptime(date_val, "%Y%m%d"))
 
     def _parse_datetime(date_val: str) -> np.datetime64:
@@ -1142,15 +1180,15 @@
             )
 
     # now we can just use the xarray sorting, which only supports 1D
     return dataset.sortby(["time", "latitude", "longitude"])
 
 
 def check_sorted(dataset: xr.Dataset) -> bool:
-    """Check that the dataset is sorted by the rules in :py:`sort_ds`"""
+    """Check that the dataset is sorted by the rules in :func:`sort_ds`"""
     sorted_ds = sort_ds(dataset.copy(deep=True))
 
     return all(
         [
             np.allclose(sorted_ds.pressure, dataset.pressure, equal_nan=True),
             np.all(
                 (sorted_ds.time == dataset.time)
@@ -1199,15 +1237,15 @@
 
     precision = 1 / 24 / 60  # minute as day fraction
     if dt_arr.dtype.name == "datetime64[D]":
         precision = 1
         whp_name = date_name.whp_name
 
     time_var = xr.DataArray(
-        dt_arr,
+        dt_arr.astype("datetime64[ns]"),
         dims=date.dims,
         attrs={
             "standard_name": "time",
             "whp_name": whp_name,
             "resolution": precision,
         },
     )
@@ -1254,15 +1292,20 @@
             continue
         if len(dataset[coord.nc_name].dims) == 1:
             dataset[coord.nc_name].encoding["_FillValue"] = None
 
     return dataset
 
 
-def _load_raw_exchange(filename_or_obj: ExchangeIO) -> List[str]:
+def _load_raw_exchange(
+    filename_or_obj: ExchangeIO,
+    *,
+    file_seperator: Optional[str] = None,
+    keep_seperator=True,
+) -> List[str]:
     if isinstance(filename_or_obj, str) and filename_or_obj.startswith("http"):
         log.info("Loading object over http")
         data_raw = io.BytesIO(requests.get(filename_or_obj).content)
 
     elif isinstance(filename_or_obj, (str, Path)) and Path(filename_or_obj).exists():
         log.info("Loading object from local file path")
         with open(filename_or_obj, "rb") as local_file:
@@ -1274,17 +1317,26 @@
         # https://github.com/python/mypy/issues/1424
         data_raw = io.BytesIO(filename_or_obj.read())  # type: ignore
 
     elif isinstance(filename_or_obj, (bytes, bytearray)):
         log.info("Loading raw data bytes")
         data_raw = io.BytesIO(filename_or_obj)
 
-    data = []
-    if is_zipfile(data_raw):
+    data: List[str] = []
+
+    if file_seperator is not None:
+        data = data_raw.read().decode("utf8").strip().split(file_seperator)
+        data = list(filter(lambda x: x != "", data))
+
+        if keep_seperator:
+            data = [(datum + file_seperator).strip() for datum in data]
+
+        data = [datum.strip() for datum in data]
 
+    elif is_zipfile(data_raw):
         data_raw.seek(0)  # is_zipfile moves the "tell" position
         with ZipFile(data_raw) as zipfile:
             for zipinfo in zipfile.infolist():
                 log.debug("Reading %s", zipinfo)
                 try:
                     data.append(zipfile.read(zipinfo).decode("utf8"))
                 except UnicodeDecodeError as error:
@@ -1308,30 +1360,95 @@
     return np.all(ndarr == ndarr.flat[0])
 
 
 class CheckOptions(TypedDict, total=False):
     flags: bool
 
 
+def read_csv(
+    filename_or_obj: ExchangeIO,
+    *,
+    ftype: FileType = FileType.BOTTLE,
+    checks: Optional[CheckOptions] = None,
+) -> xr.Dataset:
+    @dataclasses.dataclass
+    class DummyParam:
+        whp_name: str
+        whp_unit: str
+
+    _checks: CheckOptions = {"flags": True}
+    if checks is not None:
+        _checks.update(checks)
+
+    data = _load_raw_exchange(
+        filename_or_obj,
+        file_seperator="something_very_unliekly~~~",
+        keep_seperator=False,
+    )
+
+    if len(data) != 1:
+        raise ValueError("read_csv can only read a single file")
+
+    splitdata = data[0].splitlines()
+
+    params_units = splitdata[0]
+    whp_params: list[WHPName | DummyParam] = []
+    for name in params_units.split(","):
+        try:
+            whp_params.append(WHPNames[name])
+        except KeyError:
+            try:
+                WHPNames.error_cols[name]
+            except KeyError:
+                whp_params.append(DummyParam(name, ""))
+
+    params = [name.whp_name for name in whp_params]
+    units = [
+        name.whp_unit if (name.whp_unit is not None) else "" for name in whp_params
+    ]
+
+    NONE_SLICE = slice(
+        0,
+        0,
+    )
+    new_data = tuple((",".join(params), ",".join(units), *splitdata[1:]))
+    exchange_data = _ExchangeInfo(
+        stamp_slice=NONE_SLICE,
+        comments_slice=NONE_SLICE,
+        ctd_headers_slice=NONE_SLICE,
+        params_idx=0,
+        units_idx=1,
+        data_slice=slice(2, None),
+        post_data_slice=NONE_SLICE,
+        _raw_lines=new_data,
+    ).finalize()
+    return _from_exchange_data([exchange_data], ftype=ftype, checks=_checks)
+
+
 def read_exchange(
     filename_or_obj: ExchangeIO,
+    *,
     fill_values=("-999",),
     checks: Optional[CheckOptions] = None,
     precision_source="file",
+    file_seperator=None,
+    keep_seperator=True,
 ) -> xr.Dataset:
     """Loads the data from filename_or_obj and returns a xr.Dataset with the CCHDO
     CF/netCDF structure"""
 
     _checks: CheckOptions = {"flags": True}
     if checks is not None:
         _checks.update(checks)
 
     log.debug(f"Check options: {_checks}")
 
-    data = _load_raw_exchange(filename_or_obj)
+    data = _load_raw_exchange(
+        filename_or_obj, file_seperator=file_seperator, keep_seperator=keep_seperator
+    )
 
     log.info("Checking for BOM")
     if any((df.startswith("\ufeff") for df in data)):
         raise ExchangeBOMError
 
     log.info("Detecting file type")
     if all((df.startswith("BOTTLE") for df in data)):
@@ -1350,14 +1467,27 @@
         _ExchangeInfo.from_lines(tuple(df.splitlines()), ftype=ftype).finalize(
             fill_values=fill_values,
             precision_source=precision_source,
         )
         for df in data
     ]
 
+    return _from_exchange_data(exchange_data, ftype=ftype, checks=_checks)
+
+
+def _from_exchange_data(
+    exchange_data: list[_ExchangeData],
+    *,
+    ftype=FileType.BOTTLE,
+    checks: Optional[CheckOptions] = None,
+) -> xr.Dataset:
+    _checks: CheckOptions = {"flags": True}
+    if checks is not None:
+        _checks.update(checks)
+
     if not all((fp.single_profile for fp in exchange_data)):
         exchange_data = list(chain(*[exd.split_profiles() for exd in exchange_data]))
 
     N_PROF = len(exchange_data)
     N_LEVELS = max((fp.shape[0] for fp in exchange_data))
 
     log.debug((N_PROF, N_LEVELS))
@@ -1416,22 +1546,32 @@
                 "flag_values": np.array(flag_values, dtype="int8"),
                 "flag_meanings": " ".join(flag_meanings),
                 "conventions": odv_conventions_map[param.flag_w],  # type: ignore
             }
 
         var_da = xr.DataArray(arr, dims=DIMS[: arr.ndim], attrs=attrs)
 
+        if param.dtype != "decimal":
+            try:
+                del var_da.attrs["C_format"]
+            except KeyError:
+                pass
+            try:
+                del var_da.attrs["C_format_source"]
+            except KeyError:
+                pass
+
         if param.dtype == "string":
             var_da.encoding["dtype"] = "S1"
 
         if param.dtype == "integer":
             var_da.encoding["dtype"] = "int32"
             var_da.encoding["_FillValue"] = -999  # classic
 
-        if param in COORDS:
+        if param in COORDS and param != CTDPRS:
             var_da.encoding["_FillValue"] = None
             if param.dtype == "integer":
                 var_da = var_da.fillna(-999).astype("int32")
 
         if ctype == "flag":
             var_da.encoding["dtype"] = "int8"
             var_da.encoding["_FillValue"] = 9
@@ -1468,20 +1608,20 @@
     log.debug("Put data in arrays")
     comments = exchange_data[0].comments
     for n_prof, exd in enumerate(exchange_data):
         if exd.comments != comments:
             comments = f"{comments}\n----file_break----\n{exd.comments}"
 
         for param in params:
-            if param in exd.param_precisions:
+            if param in exd.param_precisions and param.dtype == "decimal":
                 dataarrays[param.nc_name].attrs[
                     "C_format"
                 ] = f"%.{exd.param_precisions[param]}f"
                 dataarrays[param.nc_name].attrs["C_format_source"] = "input_file"
-            if param in exd.error_precisions:
+            if param in exd.error_precisions and param.dtype == "decimal":
                 dataarrays[f"{param.nc_name}_error"].attrs[
                     "C_format"
                 ] = f"%.{exd.error_precisions[param]}f"
                 dataarrays[f"{param.nc_name}_error"].attrs[
                     "C_format_source"
                 ] = "input_file"
```

### Comparing `cchdo.hydro-1.0.2.2/cchdo/hydro/exchange/exceptions.py` & `cchdo.hydro-1.0.2.3/cchdo/hydro/exchange/exceptions.py`

 * *Files identical despite different names*

### Comparing `cchdo.hydro-1.0.2.2/cchdo/hydro/exchange/flags.py` & `cchdo.hydro-1.0.2.3/cchdo/hydro/exchange/flags.py`

 * *Files identical despite different names*

### Comparing `cchdo.hydro-1.0.2.2/cchdo/hydro/exchange/helpers.py` & `cchdo.hydro-1.0.2.3/cchdo/hydro/exchange/helpers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import io
+from typing import Optional, Dict
 
 from cchdo.params import WHPNames
 
 
-def simple_bottle_exchange(params=None, units=None, data=None, comments: str = None):
+def simple_bottle_exchange(
+    params=None, units=None, data=None, comments: Optional[str] = None
+):
     stamp = "BOTTLE,test"
     min_params = [
         "EXPOCODE",
         "STNNBR",
         "CASTNO",
         "SAMPNO",
         "LATITUDE",
@@ -42,15 +45,20 @@
     else:
         simple = "\n".join(
             [stamp, ",".join(min_params), ",".join(min_units), ",".join(min_line), end]
         )
     return simple.encode("utf8")
 
 
-def gen_complete_bottle(ctd_params_only=False):
+def gen_complete_bottle(
+    ctd_params_only=False,
+    param_counts: Optional[Dict[str, int]] = None,
+    min_count=5,
+    filter_erddap=False,
+):
     from . import read_exchange
 
     exclude = set(
         [
             "EXPOCODE",
             "STNNBR",
             "CASTNO",
@@ -65,16 +73,21 @@
         ]
     )
 
     params = []
     units = []
     data = []
     for name in set(WHPNames.values()):
+        if filter_erddap and not name.in_erddap:
+            continue
         if name.whp_name in exclude:
             continue
+        if param_counts is not None:
+            if param_counts.get(name.nc_name, 0) < min_count:
+                continue
         if ctd_params_only is True and name.flag_w in {
             "woce_discrete",
             "woce_bottle",
             "no_flags",
         }:
             continue
         params.append(name.whp_name)
```

### Comparing `cchdo.hydro-1.0.2.2/cchdo/hydro/rename.py` & `cchdo.hydro-1.0.2.3/cchdo/hydro/rename.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,8 +45,8 @@
                         attr_values[idx] = attr_value.replace(key, value)
             renamed[var].attrs[attr] = " ".join(attr_values)
 
     return renamed
 
 
 def to_argo_variable_names(xarray_obj: Dataset) -> Dataset:
-    ...
+    return xarray_obj
```

### Comparing `cchdo.hydro-1.0.2.2/cchdo/hydro/tests/data/33RR20080204_mini_hy1.csv` & `cchdo.hydro-1.0.2.3/cchdo/hydro/tests/data/33RR20080204_mini_hy1.csv`

 * *Files identical despite different names*

### Comparing `cchdo.hydro-1.0.2.2/cchdo/hydro/tests/data/btl_time_span.csv` & `cchdo.hydro-1.0.2.3/cchdo/hydro/tests/data/btl_time_span.csv`

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 BOTTLE,HYDRO_TEST_SUITE
 # This bottle file contains no BTL_DATE column and a BTL_TIME column that goes across midnight
 # The BTL_TIME column does not have leading zeros
 EXPOCODE,SECT_ID,STNNBR,CASTNO,SAMPNO,BTLNBR,BTLNBR_FLAG_W,DATE,TIME,LATITUDE,LONGITUDE,DEPTH,CTDPRS,BTL_TIME
 ,,,,,,,,,,,METERS,DBAR,
-49UF20120826,KS1207,  3612,  1,     99,     99,2,20120904,2341, 24.2490, 133.9858, 5079,      0.0,      115
-49UF20120826,KS1207,  3612,  1,     36,  21995,2,20120904,2341, 24.2490, 133.9858, 5079,     11.4,      133
-49UF20120826,KS1207,  3612,  1,     35,  21994,2,20120904,2341, 24.2490, 133.9858, 5079,     27.1,      132
-49UF20120826,KS1207,  3612,  1,     34,  21993,2,20120904,2341, 24.2490, 133.9858, 5079,     51.7,      128
-49UF20120826,KS1207,  3612,  1,     33,  21992,2,20120904,2341, 24.2490, 133.9858, 5079,     75.4,      127
-49UF20120826,KS1207,  3612,  1,     32,  21991,2,20120904,2341, 24.2490, 133.9858, 5079,    102.9,      126
-49UF20120826,KS1207,  3612,  1,     31,  21990,2,20120904,2341, 24.2490, 133.9858, 5079,    126.8,      125
-49UF20120826,KS1207,  3612,  1,     30,  21989,2,20120904,2341, 24.2490, 133.9858, 5079,    152.2,      123
-49UF20120826,KS1207,  3612,  1,     29,  21988,2,20120904,2341, 24.2490, 133.9858, 5079,    203.1,      122
-49UF20120826,KS1207,  3612,  1,     28,  21987,2,20120904,2341, 24.2490, 133.9858, 5079,    253.4,      120
-49UF20120826,KS1207,  3612,  1,     27,  21986,2,20120904,2341, 24.2490, 133.9858, 5079,    303.1,      118
-49UF20120826,KS1207,  3612,  1,     26,  21985,2,20120904,2341, 24.2490, 133.9858, 5079,    404.4,      116
-49UF20120826,KS1207,  3612,  1,     25,  21984,2,20120904,2341, 24.2490, 133.9858, 5079,    505.0,      113
-49UF20120826,KS1207,  3612,  1,     24,  21983,2,20120904,2341, 24.2490, 133.9858, 5079,    607.5,      110
-49UF20120826,KS1207,  3612,  1,     23,  21982,2,20120904,2341, 24.2490, 133.9858, 5079,    708.5,      108
-49UF20120826,KS1207,  3612,  1,     22,  21981,2,20120904,2341, 24.2490, 133.9858, 5079,    809.1,      105
-49UF20120826,KS1207,  3612,  1,     21,  21980,2,20120904,2341, 24.2490, 133.9858, 5079,    909.9,      102
-49UF20120826,KS1207,  3612,  1,     20,  21979,2,20120904,2341, 24.2490, 133.9858, 5079,   1009.9,       59
-49UF20120826,KS1207,  3612,  1,     19,  21978,2,20120904,2341, 24.2490, 133.9858, 5079,   1211.8,       55
-49UF20120826,KS1207,  3612,  1,     18,  21977,2,20120904,2341, 24.2490, 133.9858, 5079,   1415.2,       50
-49UF20120826,KS1207,  3612,  1,     17,  21976,2,20120904,2341, 24.2490, 133.9858, 5079,   1617.6,       45
-49UF20120826,KS1207,  3612,  1,     16,  21975,2,20120904,2341, 24.2490, 133.9858, 5079,   1820.8,       41
-49UF20120826,KS1207,  3612,  1,     15,  21974,2,20120904,2341, 24.2490, 133.9858, 5079,   2023.7,       36
-49UF20120826,KS1207,  3612,  1,     14,  21973,2,20120904,2341, 24.2490, 133.9858, 5079,   2277.2,       31
-49UF20120826,KS1207,  3612,  1,     13,  21972,2,20120904,2341, 24.2490, 133.9858, 5079,   2532.8,       26
-49UF20120826,KS1207,  3612,  1,     12,  21971,2,20120904,2341, 24.2490, 133.9858, 5079,   2786.9,       20
-49UF20120826,KS1207,  3612,  1,     11,  21970,2,20120904,2341, 24.2490, 133.9858, 5079,   3041.5,       15
-49UF20120826,KS1207,  3612,  1,     10,  21969,2,20120904,2341, 24.2490, 133.9858, 5079,   3041.5,       15
-49UF20120826,KS1207,  3612,  1,      9,  21968,2,20120904,2341, 24.2490, 133.9858, 5079,   3297.0,       10
-49UF20120826,KS1207,  3612,  1,      8,  21967,2,20120904,2341, 24.2490, 133.9858, 5079,   3553.0,        4
-49UF20120826,KS1207,  3612,  1,      7,  21966,2,20120904,2341, 24.2490, 133.9858, 5079,   3553.0,        4
+49UF20120826,KS1207,  3612,  1,     99,     99,2,20120904,2341, 24.2490, 133.9858, 5079,      0.0,     0115
+49UF20120826,KS1207,  3612,  1,     36,  21995,2,20120904,2341, 24.2490, 133.9858, 5079,     11.4,     0133
+49UF20120826,KS1207,  3612,  1,     35,  21994,2,20120904,2341, 24.2490, 133.9858, 5079,     27.1,     0132
+49UF20120826,KS1207,  3612,  1,     34,  21993,2,20120904,2341, 24.2490, 133.9858, 5079,     51.7,     0128
+49UF20120826,KS1207,  3612,  1,     33,  21992,2,20120904,2341, 24.2490, 133.9858, 5079,     75.4,     0127
+49UF20120826,KS1207,  3612,  1,     32,  21991,2,20120904,2341, 24.2490, 133.9858, 5079,    102.9,     0126
+49UF20120826,KS1207,  3612,  1,     31,  21990,2,20120904,2341, 24.2490, 133.9858, 5079,    126.8,     0125
+49UF20120826,KS1207,  3612,  1,     30,  21989,2,20120904,2341, 24.2490, 133.9858, 5079,    152.2,     0123
+49UF20120826,KS1207,  3612,  1,     29,  21988,2,20120904,2341, 24.2490, 133.9858, 5079,    203.1,     0122
+49UF20120826,KS1207,  3612,  1,     28,  21987,2,20120904,2341, 24.2490, 133.9858, 5079,    253.4,     0120
+49UF20120826,KS1207,  3612,  1,     27,  21986,2,20120904,2341, 24.2490, 133.9858, 5079,    303.1,     0118
+49UF20120826,KS1207,  3612,  1,     26,  21985,2,20120904,2341, 24.2490, 133.9858, 5079,    404.4,     0116
+49UF20120826,KS1207,  3612,  1,     25,  21984,2,20120904,2341, 24.2490, 133.9858, 5079,    505.0,     0113
+49UF20120826,KS1207,  3612,  1,     24,  21983,2,20120904,2341, 24.2490, 133.9858, 5079,    607.5,     0110
+49UF20120826,KS1207,  3612,  1,     23,  21982,2,20120904,2341, 24.2490, 133.9858, 5079,    708.5,     0108
+49UF20120826,KS1207,  3612,  1,     22,  21981,2,20120904,2341, 24.2490, 133.9858, 5079,    809.1,     0105
+49UF20120826,KS1207,  3612,  1,     21,  21980,2,20120904,2341, 24.2490, 133.9858, 5079,    909.9,     0102
+49UF20120826,KS1207,  3612,  1,     20,  21979,2,20120904,2341, 24.2490, 133.9858, 5079,   1009.9,     0059
+49UF20120826,KS1207,  3612,  1,     19,  21978,2,20120904,2341, 24.2490, 133.9858, 5079,   1211.8,     0055
+49UF20120826,KS1207,  3612,  1,     18,  21977,2,20120904,2341, 24.2490, 133.9858, 5079,   1415.2,     0050
+49UF20120826,KS1207,  3612,  1,     17,  21976,2,20120904,2341, 24.2490, 133.9858, 5079,   1617.6,     0045
+49UF20120826,KS1207,  3612,  1,     16,  21975,2,20120904,2341, 24.2490, 133.9858, 5079,   1820.8,     0041
+49UF20120826,KS1207,  3612,  1,     15,  21974,2,20120904,2341, 24.2490, 133.9858, 5079,   2023.7,     0036
+49UF20120826,KS1207,  3612,  1,     14,  21973,2,20120904,2341, 24.2490, 133.9858, 5079,   2277.2,     0031
+49UF20120826,KS1207,  3612,  1,     13,  21972,2,20120904,2341, 24.2490, 133.9858, 5079,   2532.8,     0026
+49UF20120826,KS1207,  3612,  1,     12,  21971,2,20120904,2341, 24.2490, 133.9858, 5079,   2786.9,     0020
+49UF20120826,KS1207,  3612,  1,     11,  21970,2,20120904,2341, 24.2490, 133.9858, 5079,   3041.5,     0015
+49UF20120826,KS1207,  3612,  1,     10,  21969,2,20120904,2341, 24.2490, 133.9858, 5079,   3041.5,     0015
+49UF20120826,KS1207,  3612,  1,      9,  21968,2,20120904,2341, 24.2490, 133.9858, 5079,   3297.0,     0010
+49UF20120826,KS1207,  3612,  1,      8,  21967,2,20120904,2341, 24.2490, 133.9858, 5079,   3553.0,     0004
+49UF20120826,KS1207,  3612,  1,      7,  21966,2,20120904,2341, 24.2490, 133.9858, 5079,   3553.0,     0004
 49UF20120826,KS1207,  3612,  1,      6,  21965,2,20120904,2341, 24.2490, 133.9858, 5079,   3809.0,     2359
 49UF20120826,KS1207,  3612,  1,      5,  21964,2,20120904,2341, 24.2490, 133.9858, 5079,   4064.3,     2354
 49UF20120826,KS1207,  3612,  1,      4,  21963,2,20120904,2341, 24.2490, 133.9858, 5079,   4064.3,     2354
 49UF20120826,KS1207,  3612,  1,      3,  22079,2,20120904,2341, 24.2490, 133.9858, 5079,   4321.3,     2348
 49UF20120826,KS1207,  3612,  1,      2,  21961,2,20120904,2341, 24.2490, 133.9858, 5079,   4577.9,     2343
 49UF20120826,KS1207,  3612,  1,      1,  21960,2,20120904,2341, 24.2490, 133.9858, 5079,   4631.1,     2341
 END_DATA
```

### Comparing `cchdo.hydro-1.0.2.2/cchdo/hydro/tests/test_exchange.py` & `cchdo.hydro-1.0.2.3/cchdo/hydro/tests/test_exchange.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import io
-import pytest
 from importlib.resources import open_binary
 
+import pytest
+
 import numpy as np
 
-from hydro.exchange import read_exchange
+from ..exchange import read_exchange
 
-from hydro.exchange.exceptions import (
+from ..exchange.exceptions import (
     ExchangeBOMError,
     ExchangeEncodingError,
     ExchangeDuplicateParameterError,
     ExchangeParameterUndefError,
 )
 
-from hydro.exchange.helpers import simple_bottle_exchange
+from ..exchange.helpers import simple_bottle_exchange
 
 
 def test_btl_date_time():
     raw = simple_bottle_exchange(
         params=("BTL_DATE", "BTL_TIME"), units=("", ""), data=("20200101", "1234")
     )
     ex_xr = read_exchange(io.BytesIO(raw))
@@ -33,14 +34,54 @@
     )
     with pytest.warns(UserWarning):
         ex_xr = read_exchange(io.BytesIO(raw))
 
     assert ex_xr["bottle_time"].values == [[np.datetime64("2020-01-01T00:34")]]
 
 
+def test_ctd_nan():
+    test_data = b"""CTD,test
+# some comment
+NUMBER_HEADERS = 8
+EXPOCODE = TEST
+STNNBR = 1
+CASTNO = 1
+DATE = 20200101
+TIME = 0000
+LATITUDE = nan
+LONGITUDE = 0
+CTDPRS
+DBAR
+0
+END_DATA
+"""
+    with pytest.raises(ValueError):
+        read_exchange(test_data)
+
+
+def test_file_seperator():
+    test_data = b"""CTD,test
+# some comment
+NUMBER_HEADERS = 8
+EXPOCODE = TEST
+STNNBR = 1
+CASTNO = 1
+DATE = 20200101
+TIME = 0000
+LATITUDE = 0
+LONGITUDE = 0
+CTDPRS
+DBAR
+0
+END_DATA
+"""
+    ex = read_exchange(test_data + test_data, file_seperator="END_DATA")
+    assert ex.dims["N_PROF"] == 2
+
+
 @pytest.mark.parametrize(
     "data,error",
     [
         (io.BytesIO("À".encode("latin-1")), ExchangeEncodingError),
         (io.BytesIO("\ufeffBOTTLE".encode("utf8")), ExchangeBOMError),
     ],
 )
```

### Comparing `cchdo.hydro-1.0.2.2/cchdo/hydro/tests/test_rename.py` & `cchdo.hydro-1.0.2.3/cchdo/hydro/tests/test_rename.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import xarray as xr
 
-from hydro.rename import rename_with_bookkeeping, to_argo_variable_names
+from ..rename import rename_with_bookkeeping, to_argo_variable_names
 
 
 def is_not_none(a):
     return a is not None
 
 
 def test_rename():
```

### Comparing `cchdo.hydro-1.0.2.2/cchdo/hydro/tutorial.py` & `cchdo.hydro-1.0.2.3/cchdo/hydro/tutorial.py`

 * *Files identical despite different names*

### Comparing `cchdo.hydro-1.0.2.2/cchdo.hydro.egg-info/PKG-INFO` & `cchdo.hydro-1.0.2.3/cchdo.hydro.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: cchdo.hydro
-Version: 1.0.2.2
+Version: 1.0.2.3
 Home-page: https://github.com/cchdo/hydro
 Author: CCHDO
 Author-email: cchdo@ucsd.edu
 License: BSD 3-clause
-Requires-Python: ~=3.8
+Requires-Python: ~=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: netcdf
+Provides-Extra: matlab
 Provides-Extra: selftest
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: cli
 Provides-Extra: complete
 License-File: LICENSE.md
```

### Comparing `cchdo.hydro-1.0.2.2/cchdo.hydro.egg-info/SOURCES.txt` & `cchdo.hydro-1.0.2.3/cchdo.hydro.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 CHANGELOG
 LICENSE.md
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
-.devcontainer/Dockerfile
 .devcontainer/devcontainer.json
 .github/workflows/do-release.yml
 .github/workflows/python-app.yml
 .vscode/settings.json
 cchdo.hydro.egg-info/PKG-INFO
 cchdo.hydro.egg-info/SOURCES.txt
 cchdo.hydro.egg-info/dependency_links.txt
@@ -26,29 +25,46 @@
 cchdo/hydro/__init__.py
 cchdo/hydro/__main__.py
 cchdo/hydro/__main_helpers.py
 cchdo/hydro/_version.py
 cchdo/hydro/accessors.py
 cchdo/hydro/conformance.py
 cchdo/hydro/convert.py
+cchdo/hydro/core.py
+cchdo/hydro/migration.py
 cchdo/hydro/rename.py
 cchdo/hydro/tutorial.py
 cchdo/hydro/exchange/__init__.py
 cchdo/hydro/exchange/exceptions.py
 cchdo/hydro/exchange/flags.py
 cchdo/hydro/exchange/helpers.py
+cchdo/hydro/legacy/__init__.py
+cchdo/hydro/legacy/coards/__init__.py
+cchdo/hydro/legacy/coards/name_netcdf.csv
+cchdo/hydro/legacy/woce/__init__.py
+cchdo/hydro/legacy/woce/woce_params_for_exchange_to_woce.csv
 cchdo/hydro/tests/__init__.py
 cchdo/hydro/tests/conftest.py
+cchdo/hydro/tests/test_accessors.py
+cchdo/hydro/tests/test_core_ops.py
+cchdo/hydro/tests/test_csv.py
 cchdo/hydro/tests/test_exchange.py
 cchdo/hydro/tests/test_merge.py
 cchdo/hydro/tests/test_rename.py
 cchdo/hydro/tests/data/33RR20080204_mini_hy1.csv
 cchdo/hydro/tests/data/__init__.py
+cchdo/hydro/tests/data/btl_csv.csv
 cchdo/hydro/tests/data/btl_time_span.csv
+cchdo/hydro/tests/data/stns_test_data.json
 docs/Makefile
-docs/api.rst
+docs/ODF_CCHDO_netCDF_ops.rst
+docs/_erddap_table.py
+docs/_erddap_table.rst
 docs/attributes.rst
 docs/changelog.rst
 docs/conf.py
+docs/erddap.rst
+docs/format_spec.rst
 docs/index.rst
 docs/make.bat
+examples/round_trip.ipynb
 examples/simple.ipynb
```

### Comparing `cchdo.hydro-1.0.2.2/docs/Makefile` & `cchdo.hydro-1.0.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cchdo.hydro-1.0.2.2/docs/attributes.rst` & `cchdo.hydro-1.0.2.3/docs/attributes.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,21 @@
+.. _attributes:
+
 **********
 Attributes
 **********
 
 
 Variable Level Attributes
 =========================
 
 ``_FillValue``
 --------------
 
 :dtype:      same as the variable
-:usage:      variables
 :required:   only if there are missing data
 :reference:  CF-1.8, NUG
 
 CF Definiton
 ````````````
 A value used to represent missing or undefined data. Allowed for auxiliary coordinate variables but not allowed for coordinate variables.
 
@@ -25,18 +26,19 @@
 Some special coordinate variables are not allowed to have any ``_FillValue`` values in them
 
 The ``_FillValue`` attribute has special meaning to the netCDF4 libraries (C and Java).
 When the size of the variable is known (i.e. the variable does not have an "unlimited" dimmension) at the time the netCDF file is written, all of the space in the variable will be initalized with the value in ``_FillValue``.
 This is usually almost entirely transparent to you the user, some software will change the data type when a variable still contains ``_FillValue`` values.
 Matlab for example, will change byte (integers between 0 and 255) data into IEEE floating point values while replacing the fill value with NaNs.
 
+.. _whp_name:
+
 ``whp_name``
 ------------
 :dtype:      char or array of strings
-:usage:      variables
 :required:   conditionally (see CCHDO Usage)
 :reference:  CCHDO
 
 CF Definiton
 ````````````
 Not used or defined in the CF conventions.
 
@@ -46,62 +48,63 @@
 Forms a pair with :ref:`whp_unit`
 This attribute will only be on variables which are data, and not on flag variables or certain specal variables meant to be interpreted by CF compliant readers (e.g. ``geometry_container``).
 
 Some variables cannot be represented by a single column in the WHP Exchange format, when this occurs, the attribute will be an array of strings containing all the names needed to represent this variable in WHP Exchange format.
 The most frequent example will be the ``time`` variable, in WHP Exchange files, this may either be a pair of columns (DATE, TIME) or a single column (DATE) when time of day is not reported.
 This will very likly be used to represet ex and em wavelengths for optical sensors with multiple channels.
 
-There is no requiremnt that all variables in a netCDF file contain unique ``whp_name`` and ``whp_unit`` pairs.
+.. warning::
+
+  There is no requiremnt that all variables in a netCDF file contain unique ``whp_name`` and ``whp_unit`` pairs.
 
 
+.. _whp_unit:
+
 ``whp_unit``
 ------------
 :dtype:      char or array of strings
-:usage:      variables
 :required:   conditionally (see CCHDO Usage)
 :reference:  CCHDO
 
 CF Definiton
 ````````````
 Not used or defined in the CF conventions.
 
 CCHDO Usage
 ```````````
 For this variable, the value which would appear in the units line of the WHP Exchange or WOCE sea/ctd file.
-Forms a pair with :ref:``whp_name``
+Forms a pair with :ref:`whp_name`
 Usage is the same as ``whp_name``
 
 
 ``standard_name``
 -----------------
 :dtype:      char
-:usage:      variables
 :required:   conditionally (see CF Usage)
 :reference:  CF 1.8
 
 CF Definiton
 ````````````
 .. todo::
   get cf definiton
 
 CCHDO Usage
 ```````````
 The CF usage will be followed, if a CF standard name exists for physical quantity represeted by a variable, the most specific name MUST be used and appear in the ``standard_name`` attribute.
 The CF standard names table is updated frequently, as names are added they will be evaluated for including in the CCHDO netCDF files to both be more specific or to add a standard name to a variable that did not have one previously.
 Always check the param version attribute to see which version of the standard name table is in use for a particular file.
 
-It is important to understand that standard names represet the physical quantity of the variable and not how that physical quantity was made.
+It is important to understand that standard names represet the physical quantity of the variable and not how the data was made.
 Standard names cannot distinguish between salinity measured in situ with a CTD, salinity measured with an autosal, or even salinity from a model output.
 The names are meant to help with intercomparison of the values themselves, not methods of determing that value.
 
 
 ``units``
 -----------------
 :dtype:      char
-:usage:      variables
 :required:   conditionally
 :reference:  CF 1.8
 
 CF Definiton
 ````````````
 .. todo::
   get cf definiton
@@ -123,15 +126,14 @@
 * Practical salinity will have the units of "1", not variabtions on "PSU" or even "0.001" implying g/kg of actual salinity.
 * Tritium Units are really parts per 1e18, so the equivalent SI units are the recriprical: 1e-18
 
 
 ``reference_scale``
 -------------------
 :dtype:      char
-:usage:      variables
 :required:   conditionally
 :reference:  OceanSITES 1.4
 
 CF Definiton
 ````````````
 This attribute is not defined in CF. 
 
@@ -147,15 +149,14 @@
 .. todo::
   this is a controlled list internally, list which variables have a scale and what their value can be.
 
 
 ``C_format``
 ------------
 :dtype:      char
-:usage:      variables
 :required:   no
 :reference:  NUG
 
 CF Definiton
 ````````````
 ``C_format`` is not mentioned at all in the CF-1.8 docs.
 
@@ -183,43 +184,190 @@
   More recent measuremnets have started to include explicit uncertanties which will be reported along side the data values.
   Often, the cruise report will contain some charicterizaion of the uncertanty of a given measumrnet.
 
 
 ``C_format_source``
 -------------------
 :dtype:      char
-:usage:      variables
 :required:   yes if C_format is present
 :reference:  CCHDO
 
 CF Definiton
 ````````````
 This attribute is not used in CF.
 
 CCHDO Usage
 ```````````
 This attribute describes where the value in ``C_format`` came from.
 This attribute will only have the values of either ``"database"`` to indicate the ``C_format`` was taken from the internal parameters table, or ``"source_file"`` if the values was calcualted from input text.
 
+``geometry``
+------------
+:dtype:      dtype
+:required:   maybe
+:reference:  Ref
 
-.. todo::
-  Attrs:
+CF Definiton
+````````````
+
+CCHDO Usage
+```````````
+
+``_Encoding``
+-------------
+:dtype:      char
+:required:   no
+:reference:  ref?
+
+CF Definiton
+````````````
+This is not defined by CF, it is however a reserved attribute in `Appendix B`_ of the netCDF4-C manual.
+
+.. _Appendix B: https://docs.unidata.ucar.edu/netcdf-c/current/file_format_specifications.html
+
+CCHDO Usage
+```````````
+This attribute is set by the libraries we use to make our data.
+It will almost always be set on string or char array data with a value of "utf8".
+
+``coordinates``
+---------------
+:dtype:      char
+:required:   conditionally
+:reference:  CF 1.8
+
+CF Definiton
+````````````
+
+CCHDO Usage
+```````````
+
+``ancillary_variables``
+-----------------------
+:dtype:      dtype
+:required:   maybe
+:reference:  Ref
+
+CF Definiton
+````````````
+
+CCHDO Usage
+```````````
+
+``flag_values``
+---------------
+:dtype:      dtype
+:required:   maybe
+:reference:  Ref
+
+CF Definiton
+````````````
+
+CCHDO Usage
+```````````
+
+``flag_meanings``
+-----------------
+:dtype:      dtype
+:required:   maybe
+:reference:  Ref
+
+CF Definiton
+````````````
+
+CCHDO Usage
+```````````
+
+``conventions``
+---------------
+:dtype:      dtype
+:required:   maybe
+:reference:  Ref
+
+CF Definiton
+````````````
+
+CCHDO Usage
+```````````
+
+``resolution (time)``
+---------------------
+:dtype:      dtype
+:required:   maybe
+:reference:  Ref
+
+CF Definiton
+````````````
+
+CCHDO Usage
+```````````
+
+``axis``
+--------
+:dtype:      dtype
+:required:   maybe
+:reference:  Ref
+
+CF Definiton
+````````````
+
+CCHDO Usage
+```````````
+
+``calendar``
+------------
+:dtype:      dtype
+:required:   maybe
+:reference:  Ref
+
+CF Definiton
+````````````
 
-  Variable Level:
+CCHDO Usage
+```````````
+
+``positive``
+------------
+:dtype:      dtype
+:required:   maybe
+:reference:  Ref
+
+CF Definiton
+````````````
+
+CCHDO Usage
+```````````
+
+``geometry_type``
+------------------
+:dtype:      dtype
+:required:   maybe
+:reference:  Ref
+
+CF Definiton
+````````````
 
-  * ancillary_variables
-  * coordinates
-  * flag_values
-  * flag_meanings
-  * conventions
-  * _Encoding
-  * geometry_type
-  * node_coordinates
-  * axis
-  * geometry
+CCHDO Usage
+```````````
+
+``node_coordinates``
+--------------------
+:dtype:      dtype
+:required:   maybe
+:reference:  Ref
+
+CF Definiton
+````````````
+
+CCHDO Usage
+```````````
+
+
+.. todo::
+  Attrs:
 
   Global Level:
 
   * Conventions
   * cchdo_software_version
   * cchdo_parameters_version
   * comments
@@ -243,8 +391,8 @@
 
   Non ACDD global level?:
   
   * platform (ICES ship code)
   * start/end ports
   * actual start/end dates
 
-  Huge TODO... history at the var and global level, including seperation between metadata and data history.
+  Huge TODO... history at the var and global level, including seperation between metadata and data history.
```

### Comparing `cchdo.hydro-1.0.2.2/docs/conf.py` & `cchdo.hydro-1.0.2.3/docs/conf.py`

 * *Files 16% similar despite different names*

```diff
@@ -40,19 +40,22 @@
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
     "sphinx.ext.todo",
     "sphinx.ext.viewcode",
-    "sphinx.ext.autosummary",
+    "sphinx_design",
+    "autoapi.extension",
 ]
 
-autosummary_generate = True
-autodoc_typehints = "none"
+autoapi_dirs = ["../cchdo", "../cchdo/hydro"]
+autoapi_python_use_implicit_namespaces = True
+
+autodoc_typehints = "description"
 
 # Add any paths that contain templates here, relative to this directory.
 # templates_path = ['_templates']
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
@@ -63,15 +66,15 @@
 master_doc = "index"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # The name of the Pygments (syntax highlighting) style to use.
```

### Comparing `cchdo.hydro-1.0.2.2/docs/make.bat` & `cchdo.hydro-1.0.2.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cchdo.hydro-1.0.2.2/examples/simple.ipynb` & `cchdo.hydro-1.0.2.3/examples/simple.ipynb`

 * *Files identical despite different names*

### Comparing `cchdo.hydro-1.0.2.2/setup.cfg` & `cchdo.hydro-1.0.2.3/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -11,58 +11,67 @@
 exclude = 
 	docs
 	versioneer.py
 
 [metadata]
 name = cchdo.hydro
 author = CCHDO
-author-email = cchdo@ucsd.edu
-home-page = https://github.com/cchdo/hydro
+author_email = cchdo@ucsd.edu
+home_page = https://github.com/cchdo/hydro
 license = BSD 3-clause
 long_description = file: README.md, LICENSE.md
+long_description_content_type = text/markdown
 
 [options]
-python_requires = ~=3.8
+python_requires = ~=3.10
 zip_safe = False
 packages = find_namespace:
 namespace_packages = 
 	cchdo
 setup_requires = setuptools_scm
 include_package_data = True
 install_requires = 
-	cchdo.params >= 0.1.19
+	cchdo.params >= 0.1.21
 	xarray >= 0.18.0
 	requests >= 2.26.0
-	netCDF4 >= 1.5.7
 	numpy >= 1.20.0
 	pandas >= 1.3.3
 	appdirs
 	typing_extensions
 
 [options.extras_require]
+netcdf = 
+	netCDF4 >= 1.5.7
+matlab = 
+	scipy
 selftest = 
 	pytest==6.2.5
 	requests-mock==1.8.0
 dev = 
 	%(selftest)s
 	pytest-cov
 	pre-commit
-	black==22.6.0
+	black==23.1.0
 	codecov
-	mypy==0.971
-	flake8==5.0.4
+	mypy==1.0.0
+	flake8==6.0.0
 	types-requests
 docs = 
 	Sphinx
 	jupyter
 	furo
+	sphinx-design
+	sphinx-autoapi
 cli = 
+	%(netcdf)s
 	click
 	rich
 complete = 
+	%(netcdf)s
+	%(matlab)s
 	%(cli)s
 	%(dev)s
 	%(docs)s
 
 [tool:pytest]
 xfail_strict = true
```

