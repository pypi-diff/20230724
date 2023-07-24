# Comparing `tmp/autora-theorist-toolkit-0.2.3.tar.gz` & `tmp/autora-theorist-toolkit-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-theorist-toolkit-0.2.3.tar", last modified: Sat Jul 22 00:09:02 2023, max compression
+gzip compressed data, was "autora-theorist-toolkit-0.2.4.tar", last modified: Mon Jul 24 18:24:03 2023, max compression
```

## Comparing `autora-theorist-toolkit-0.2.3.tar` & `autora-theorist-toolkit-0.2.4.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 00:09:02.232451 autora-theorist-toolkit-0.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 00:09:02.228451 autora-theorist-toolkit-0.2.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 00:09:02.228451 autora-theorist-toolkit-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 00:09:02.228451 autora-theorist-toolkit-0.2.3/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/.idea/autora-theorist-toolkit.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 00:09:02.228451 autora-theorist-toolkit-0.2.3/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-07-22 00:09:02.232451 autora-theorist-toolkit-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 00:09:02.228451 autora-theorist-toolkit-0.2.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/docs/Additional Example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/docs/Basic Usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 00:09:02.228451 autora-theorist-toolkit-0.2.3/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 00:09:02.228451 autora-theorist-toolkit-0.2.3/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 00:09:02.232451 autora-theorist-toolkit-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 00:09:02.228451 autora-theorist-toolkit-0.2.3/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 00:09:02.228451 autora-theorist-toolkit-0.2.3/src/autora/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 00:09:02.228451 autora-theorist-toolkit-0.2.3/src/autora/theorist/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 00:09:02.228451 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 00:09:02.232451 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/components/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/components/primitives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 00:09:02.232451 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/methods/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/methods/fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/methods/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/methods/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/methods/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 00:09:02.232451 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/models/bayesian_machine_scientist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/models/bayesian_symbolic_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/models/ddm_bms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/models/hierarchical_bayesian_symbolic_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/models/hierarchical_symbolic_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/models/hybrid_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/models/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/models/parallel_symbolic_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/models/symbolic_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/models/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 00:09:02.232451 autora-theorist-toolkit-0.2.3/src/autora_theorist_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-07-22 00:09:02.000000 autora-theorist-toolkit-0.2.3/src/autora_theorist_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-22 00:09:02.000000 autora-theorist-toolkit-0.2.3/src/autora_theorist_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 00:09:02.000000 autora-theorist-toolkit-0.2.3/src/autora_theorist_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-22 00:09:02.000000 autora-theorist-toolkit-0.2.3/src/autora_theorist_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-22 00:09:02.000000 autora-theorist-toolkit-0.2.3/src/autora_theorist_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 00:09:02.232451 autora-theorist-toolkit-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/tests/test_toolkit.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/tests/test_visual.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:24:03.759158 autora-theorist-toolkit-0.2.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:24:03.751158 autora-theorist-toolkit-0.2.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:24:03.751158 autora-theorist-toolkit-0.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:24:03.751158 autora-theorist-toolkit-0.2.4/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/.idea/autora-theorist-toolkit.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:24:03.751158 autora-theorist-toolkit-0.2.4/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-07-24 18:24:03.759158 autora-theorist-toolkit-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:24:03.751158 autora-theorist-toolkit-0.2.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/docs/Additional Example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/docs/Basic Usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:24:03.751158 autora-theorist-toolkit-0.2.4/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:24:03.751158 autora-theorist-toolkit-0.2.4/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 18:24:03.759158 autora-theorist-toolkit-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:24:03.751158 autora-theorist-toolkit-0.2.4/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:24:03.751158 autora-theorist-toolkit-0.2.4/src/autora/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:24:03.755158 autora-theorist-toolkit-0.2.4/src/autora/theorist/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:24:03.755158 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:24:03.755158 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/components/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/components/primitives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:24:03.755158 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/methods/fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/methods/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/methods/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/methods/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:24:03.755158 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/models/bayesian_machine_scientist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/models/bayesian_symbolic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/models/ddm_bms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/models/hierarchical_bayesian_symbolic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/models/hierarchical_symbolic_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/models/hybrid_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/models/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/models/parallel_symbolic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/models/symbolic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/models/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:24:03.759158 autora-theorist-toolkit-0.2.4/src/autora_theorist_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-07-24 18:24:03.000000 autora-theorist-toolkit-0.2.4/src/autora_theorist_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-24 18:24:03.000000 autora-theorist-toolkit-0.2.4/src/autora_theorist_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:24:03.000000 autora-theorist-toolkit-0.2.4/src/autora_theorist_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-24 18:24:03.000000 autora-theorist-toolkit-0.2.4/src/autora_theorist_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 18:24:03.000000 autora-theorist-toolkit-0.2.4/src/autora_theorist_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:24:03.759158 autora-theorist-toolkit-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/tests/test_toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/tests/test_visual.py
```

### Comparing `autora-theorist-toolkit-0.2.3/.github/pull_request_template.md` & `autora-theorist-toolkit-0.2.4/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.3/.github/workflows/python-publish.yml` & `autora-theorist-toolkit-0.2.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.3/.gitignore` & `autora-theorist-toolkit-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.3/.idea/inspectionProfiles/Project_Default.xml` & `autora-theorist-toolkit-0.2.4/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.3/.pre-commit-config.yaml` & `autora-theorist-toolkit-0.2.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.3/PKG-INFO` & `autora-theorist-toolkit-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-theorist-toolkit
-Version: 0.2.3
+Version: 0.2.4
 Summary: Toolkit to build algorithms for model recovery
 Author-email: "Joshua T. S. Hewson" <joshua_hewson@brown.edu>
 License: MIT license
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/TheLemonPig/autora-theorist-toolkit
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `autora-theorist-toolkit-0.2.3/README.md` & `autora-theorist-toolkit-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.3/docs/Additional Example.ipynb` & `autora-theorist-toolkit-0.2.4/docs/Additional Example.ipynb`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.3/docs/Basic Usage.ipynb` & `autora-theorist-toolkit-0.2.4/docs/Basic Usage.ipynb`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.3/docs/index.md` & `autora-theorist-toolkit-0.2.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.3/mkdocs/base.yml` & `autora-theorist-toolkit-0.2.4/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.3/pyproject.toml` & `autora-theorist-toolkit-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/components/nodes.py` & `autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/components/nodes.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/components/primitives.py` & `autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/components/primitives.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/methods/fitting.py` & `autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/methods/fitting.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/methods/metrics.py` & `autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/methods/metrics.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/methods/regression.py` & `autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/methods/regression.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/methods/rules.py` & `autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/methods/rules.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/models/bayesian_machine_scientist.py` & `autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/models/bayesian_machine_scientist.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/models/bayesian_symbolic_regression.py` & `autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/models/bayesian_symbolic_regression.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/models/hierarchical_bayesian_symbolic_regression.py` & `autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/models/hierarchical_bayesian_symbolic_regression.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/models/hierarchical_symbolic_regressor.py` & `autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/models/hierarchical_symbolic_regressor.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         super().cache()
 
     def back_step(self):
         self.id_parameters = self.parameter_cache.pop()
         super().back_step()
 
     def get_id_data(self, g, id, x, y=None):
-        id_x = x[g == id]
+        id_x = x[(g == id)[:, 0], :]
         if len(id_x.shape) == 1:
             id_x = id_x.reshape((-1, 1))
         if y is None:
             id_y = None
         else:
             id_y = y[g == id]
             if len(id_y.shape) == 1:
```

### Comparing `autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/models/hybrid_regression.py` & `autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/models/hybrid_regression.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/models/memory.py` & `autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/models/memory.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/models/parallel_symbolic_regression.py` & `autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/models/parallel_symbolic_regression.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/models/symbolic_regression.py` & `autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/models/symbolic_regression.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/models/tree.py` & `autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/models/tree.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/utils.py` & `autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/utils.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.3/src/autora_theorist_toolkit.egg-info/PKG-INFO` & `autora-theorist-toolkit-0.2.4/src/autora_theorist_toolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-theorist-toolkit
-Version: 0.2.3
+Version: 0.2.4
 Summary: Toolkit to build algorithms for model recovery
 Author-email: "Joshua T. S. Hewson" <joshua_hewson@brown.edu>
 License: MIT license
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/TheLemonPig/autora-theorist-toolkit
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `autora-theorist-toolkit-0.2.3/src/autora_theorist_toolkit.egg-info/SOURCES.txt` & `autora-theorist-toolkit-0.2.4/src/autora_theorist_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.3/tests/README.md` & `autora-theorist-toolkit-0.2.4/tests/README.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.3/tests/test_toolkit.py` & `autora-theorist-toolkit-0.2.4/tests/test_toolkit.py`

 * *Files 18% similar despite different names*

```diff
@@ -47,33 +47,43 @@
 
 
 def test_bayesian_machine_scientist_initialization():
     theorist = BayesianMachineScientist()
     assert theorist is not None
 
 
-def test_hsbr_prior_restriction_and_fitting():
+def test_hbsr_prior_restriction_and_fitting():
     prior_dict_ = {"+": 1.0, "expit": 1.0}
-    hsbr = HierarchicalBayesianSymbolicRegression(prior_dict=prior_dict_)
-    assert len(hsbr.theorists[-1]._primitives) > 0
+    hbsr = HierarchicalBayesianSymbolicRegression(prior_dict=prior_dict_)
+    assert len(hbsr.theorists[-1]._primitives) > 0
     x = scipy.special.expit(np.linspace(0, 1, 100)).reshape((-1, 1))
     y = 1 + x
     g = np.ones_like(x)
-    hsbr.fit(x, y, g, epochs=30)
-    assert "-" not in hsbr.theorists[-1].model_
-    assert "*" not in hsbr.theorists[-1].model_
-    assert "**" not in hsbr.theorists[-1].model_
-    assert "/" not in hsbr.theorists[-1].model_
-    assert "cos" not in hsbr.theorists[-1].model_
-    assert "exp" not in hsbr.theorists[-1].model_
-    assert "log" not in hsbr.theorists[-1].model_
-    assert "sin" not in hsbr.theorists[-1].model_
+    hbsr.fit(x, y, g, epochs=30)
+    assert "-" not in hbsr.theorists[-1].model_
+    assert "*" not in hbsr.theorists[-1].model_
+    assert "**" not in hbsr.theorists[-1].model_
+    assert "/" not in hbsr.theorists[-1].model_
+    assert "cos" not in hbsr.theorists[-1].model_
+    assert "exp" not in hbsr.theorists[-1].model_
+    assert "log" not in hbsr.theorists[-1].model_
+    assert "sin" not in hbsr.theorists[-1].model_
     assert (
-        np.sum(hsbr.theorists[-1].predict(x, g) - y) == 0
-    ), f"{hsbr.theorists[-1].model_} but should be 1+expit(x)"
+        np.sum(hbsr.theorists[-1].predict(x, g) - y) == 0
+    ), f"{hbsr.theorists[-1].model_} but should be 1+expit(x)"
+
+
+def test_hbsr_multi_x():
+    x = np.linspace(0, 1, 200).reshape((-1, 2))
+    y = 1 + x[:, 0] + x[:, 1]
+    y = y.reshape((-1, 1))
+    g = np.ones_like(y)
+    hbsr = HierarchicalBayesianSymbolicRegression()
+    hbsr.fit(x=x, y=y, g=g, epochs=30)
 
 
 if __name__ == "__main__":
     test_symbolic_regression_initialization()
     test_bayesian_symbolic_regression_initialization()
     test_parallel_symbolic_regression_initialization()
     test_bayesian_machine_scientist_initialization()
+    test_hbsr_multi_x()
```

### Comparing `autora-theorist-toolkit-0.2.3/tests/test_visual.py` & `autora-theorist-toolkit-0.2.4/tests/test_visual.py`

 * *Files identical despite different names*

