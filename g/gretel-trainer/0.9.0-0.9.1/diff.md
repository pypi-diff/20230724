# Comparing `tmp/gretel-trainer-0.9.0.tar.gz` & `tmp/gretel-trainer-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gretel-trainer-0.9.0.tar", last modified: Tue Jun 20 17:56:26 2023, max compression
+gzip compressed data, was "gretel-trainer-0.9.1.tar", last modified: Mon Jul 24 18:03:46 2023, max compression
```

## Comparing `gretel-trainer-0.9.0.tar` & `gretel-trainer-0.9.1.tar`

### file list

```diff
@@ -1,144 +1,145 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:26.988721 gretel-trainer-0.9.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:26.956721 gretel-trainer-0.9.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:26.964721 gretel-trainer-0.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11950 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-20 17:56:26.988721 gretel-trainer-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:26.964721 gretel-trainer-0.9.0/data/
--rw-r--r--   0 runner    (1001) docker     (123)   108190 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/data/cpu_states.csv
--rw-r--r--   0 runner    (1001) docker     (123)   629637 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/data/mitre-synthea-health.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:26.968721 gretel-trainer-0.9.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:26.968721 gretel-trainer-0.9.0/docs/img/
--rw-r--r--   0 runner    (1001) docker     (123)    22313 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/docs/img/gretel-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/docs/img/gretel_logo_white.png
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/docs/models.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/docs/relational.rst
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/docs/trainer.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:26.972721 gretel-trainer-0.9.0/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/notebooks/benchmark.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/notebooks/conditional-generation.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/notebooks/custom-example.py
--rw-r--r--   0 runner    (1001) docker     (123)    19041 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/notebooks/relational.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/notebooks/simple-conditional-generation.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/notebooks/simple-example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/notebooks/table_extraction_with_subsetting.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/notebooks/trainer-examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 17:56:26.988721 gretel-trainer-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:26.960721 gretel-trainer-0.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:26.972721 gretel-trainer-0.9.0/src/gretel_trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:26.976721 gretel-trainer-0.9.0/src/gretel_trainer/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/benchmark/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/benchmark/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:26.976721 gretel-trainer-0.9.0/src/gretel_trainer/benchmark/custom/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/benchmark/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/benchmark/custom/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/benchmark/custom/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:26.976721 gretel-trainer-0.9.0/src/gretel_trainer/benchmark/gretel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/benchmark/gretel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/benchmark/gretel/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/benchmark/gretel/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/benchmark/gretel/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/benchmark/gretel/sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/benchmark/gretel/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:26.980721 gretel-trainer-0.9.0/src/gretel_trainer/relational/
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/ancestry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/connectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    29056 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/drawing.py
--rw-r--r--   0 runner    (1001) docker     (123)    21916 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13734 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/model_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    51127 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/multi_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:26.980721 gretel-trainer-0.9.0/src/gretel_trainer/relational/report/
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/report/figures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/report/key_highlight.js
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/report/report.css
--rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/report/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/report/report_privacy_protection.css
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/report/report_synthetic_quality.css
--rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/report/report_template.html
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/sdk_extras.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:26.980721 gretel-trainer-0.9.0/src/gretel_trainer/relational/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)    14319 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/strategies/ancestral.py
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/strategies/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/strategies/independent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/table_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/task_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:26.980721 gretel-trainer-0.9.0/src/gretel_trainer/relational/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/tasks/classify.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/tasks/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/tasks/synthetics_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/tasks/synthetics_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/tasks/synthetics_train.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/tasks/transforms_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/tasks/transforms_train.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/workflow_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    29826 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:26.976721 gretel-trainer-0.9.0/src/gretel_trainer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-20 17:56:26.000000 gretel-trainer-0.9.0/src/gretel_trainer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-06-20 17:56:26.000000 gretel-trainer-0.9.0/src/gretel_trainer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 17:56:26.000000 gretel-trainer-0.9.0/src/gretel_trainer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-20 17:56:26.000000 gretel-trainer-0.9.0/src/gretel_trainer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 17:56:26.000000 gretel-trainer-0.9.0/src/gretel_trainer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:26.984721 gretel-trainer-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:26.984721 gretel-trainer-0.9.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)  2927798 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/data/core-221-train.csv
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/example_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/mocks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:26.988721 gretel-trainer-0.9.0/tests/relational/
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:26.988721 gretel-trainer-0.9.0/tests/relational/example_dbs/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/example_dbs/art.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/example_dbs/documents.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/example_dbs/ecom.sql
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/example_dbs/mutagenesis.sql
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/example_dbs/pets.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/example_dbs/tpch.sql
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/example_dbs/trips.sql
--rw-r--r--   0 runner    (1001) docker     (123)    22755 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/test_ancestral_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/test_ancestry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/test_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/test_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/test_common_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/test_connectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/test_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/test_independent_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/test_model_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/test_multi_table_config_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    25838 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/test_multi_table_restore.py
--rw-r--r--   0 runner    (1001) docker     (123)    12055 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/test_relational_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    30572 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/test_relational_data_with_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/test_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/test_synthetics_run_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/test_task_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/test_train_synthetics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/test_train_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/test_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/test_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:03:46.487912 gretel-trainer-0.9.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:03:46.471912 gretel-trainer-0.9.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:03:46.471912 gretel-trainer-0.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11950 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-24 18:03:46.487912 gretel-trainer-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:03:46.471912 gretel-trainer-0.9.1/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   108190 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/data/cpu_states.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   629637 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/data/mitre-synthea-health.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:03:46.475912 gretel-trainer-0.9.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:03:46.475912 gretel-trainer-0.9.1/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    22313 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/docs/img/gretel-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/docs/img/gretel_logo_white.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/docs/models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/docs/relational.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/docs/trainer.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:03:46.475912 gretel-trainer-0.9.1/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/notebooks/benchmark.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/notebooks/conditional-generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/notebooks/custom-example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19041 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/notebooks/relational.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/notebooks/simple-conditional-generation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/notebooks/simple-example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/notebooks/table_extraction_with_subsetting.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/notebooks/trainer-examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 18:03:46.487912 gretel-trainer-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:03:46.471912 gretel-trainer-0.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:03:46.475912 gretel-trainer-0.9.1/src/gretel_trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:03:46.475912 gretel-trainer-0.9.1/src/gretel_trainer/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/benchmark/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/benchmark/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:03:46.475912 gretel-trainer-0.9.1/src/gretel_trainer/benchmark/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/benchmark/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/benchmark/custom/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/benchmark/custom/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:03:46.475912 gretel-trainer-0.9.1/src/gretel_trainer/benchmark/gretel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/benchmark/gretel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/benchmark/gretel/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/benchmark/gretel/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/benchmark/gretel/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/benchmark/gretel/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/benchmark/gretel/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:03:46.479912 gretel-trainer-0.9.1/src/gretel_trainer/relational/
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/relational/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/relational/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/relational/ancestry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/relational/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/relational/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/relational/connectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31961 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/relational/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/relational/drawing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21969 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/relational/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14044 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/relational/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/relational/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/relational/model_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49807 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/relational/multi_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:03:46.479912 gretel-trainer-0.9.1/src/gretel_trainer/relational/report/
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/relational/report/figures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/relational/report/key_highlight.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/relational/report/report.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/relational/report/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/relational/report/report_privacy_protection.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/relational/report/report_synthetic_quality.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/relational/report/report_template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/relational/sdk_extras.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:03:46.479912 gretel-trainer-0.9.1/src/gretel_trainer/relational/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)    14594 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/relational/strategies/ancestral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/relational/strategies/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/relational/strategies/independent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/relational/table_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/relational/task_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:03:46.479912 gretel-trainer-0.9.1/src/gretel_trainer/relational/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/relational/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/relational/tasks/classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/relational/tasks/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/relational/tasks/synthetics_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/relational/tasks/synthetics_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/relational/tasks/synthetics_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/relational/tasks/transforms_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/relational/tasks/transforms_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/relational/workflow_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29826 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/src/gretel_trainer/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:03:46.475912 gretel-trainer-0.9.1/src/gretel_trainer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-24 18:03:46.000000 gretel-trainer-0.9.1/src/gretel_trainer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-24 18:03:46.000000 gretel-trainer-0.9.1/src/gretel_trainer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:03:46.000000 gretel-trainer-0.9.1/src/gretel_trainer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-24 18:03:46.000000 gretel-trainer-0.9.1/src/gretel_trainer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-24 18:03:46.000000 gretel-trainer-0.9.1/src/gretel_trainer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:03:46.479912 gretel-trainer-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:03:46.479912 gretel-trainer-0.9.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  2927798 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/tests/data/core-221-train.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/tests/example_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/tests/mocks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:03:46.487912 gretel-trainer-0.9.1/tests/relational/
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/tests/relational/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:03:46.487912 gretel-trainer-0.9.1/tests/relational/example_dbs/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/tests/relational/example_dbs/art.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/tests/relational/example_dbs/documents.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/tests/relational/example_dbs/ecom.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/tests/relational/example_dbs/mutagenesis.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/tests/relational/example_dbs/pets.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/tests/relational/example_dbs/tpch.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/tests/relational/example_dbs/trips.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    25932 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/tests/relational/test_ancestral_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8597 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/tests/relational/test_ancestry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/tests/relational/test_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/tests/relational/test_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/tests/relational/test_common_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/tests/relational/test_connectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/tests/relational/test_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/tests/relational/test_independent_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/tests/relational/test_model_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/tests/relational/test_multi_table_config_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25838 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/tests/relational/test_multi_table_restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11646 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/tests/relational/test_relational_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36946 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/tests/relational/test_relational_data_with_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/tests/relational/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/tests/relational/test_synthetics_run_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/tests/relational/test_task_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9524 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/tests/relational/test_train_synthetics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/tests/relational/test_train_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/tests/test_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-24 18:03:40.000000 gretel-trainer-0.9.1/tests/test_strategy.py
```

### Comparing `gretel-trainer-0.9.0/.github/workflows/python-publish.yml` & `gretel-trainer-0.9.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/.gitignore` & `gretel-trainer-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/LICENSE` & `gretel-trainer-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/PKG-INFO` & `gretel-trainer-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gretel-trainer
-Version: 0.9.0
+Version: 0.9.1
 Summary: Synthetic Data Generation with optional Differential Privacy
 Home-page: https://github.com/gretelai/gretel-trainer
 License: https://gretel.ai/license/source-available-license
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Free To Use But Restricted
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `gretel-trainer-0.9.0/README.md` & `gretel-trainer-0.9.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -60,13 +60,22 @@
 ## 3. Generate synthetic data!
 ```python3
 df = model.generate()
 ```
 
 ## Development
 
+Setup environment and install dependencies.
+
+```sh
+python -m venv venv
+source venv/bin/activate
+pip install -r requirements-dev.txt
+pip install -e .
+```
+
 - Run tests via `make test`
 - Run type-checking (limited coverage) via `make type`
 
 ## TODOs / Roadmap
 
 - [ ] Enable conditional generation via SDK interface (supported in Notebooks currently).
```

### Comparing `gretel-trainer-0.9.0/data/cpu_states.csv` & `gretel-trainer-0.9.1/data/cpu_states.csv`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/data/mitre-synthea-health.csv` & `gretel-trainer-0.9.1/data/mitre-synthea-health.csv`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/docs/Makefile` & `gretel-trainer-0.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/docs/conf.py` & `gretel-trainer-0.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/docs/img/gretel-logo.png` & `gretel-trainer-0.9.1/docs/img/gretel-logo.png`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/docs/img/gretel_logo_white.png` & `gretel-trainer-0.9.1/docs/img/gretel_logo_white.png`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/docs/index.rst` & `gretel-trainer-0.9.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/docs/make.bat` & `gretel-trainer-0.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/docs/quickstart.rst` & `gretel-trainer-0.9.1/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/docs/relational.rst` & `gretel-trainer-0.9.1/docs/relational.rst`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/notebooks/benchmark.ipynb` & `gretel-trainer-0.9.1/notebooks/benchmark.ipynb`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/notebooks/conditional-generation.py` & `gretel-trainer-0.9.1/notebooks/conditional-generation.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/notebooks/custom-example.py` & `gretel-trainer-0.9.1/notebooks/custom-example.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/notebooks/relational.ipynb` & `gretel-trainer-0.9.1/notebooks/relational.ipynb`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/notebooks/simple-conditional-generation.ipynb` & `gretel-trainer-0.9.1/notebooks/simple-conditional-generation.ipynb`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/notebooks/table_extraction_with_subsetting.ipynb` & `gretel-trainer-0.9.1/notebooks/table_extraction_with_subsetting.ipynb`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/notebooks/trainer-examples.ipynb` & `gretel-trainer-0.9.1/notebooks/trainer-examples.ipynb`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/setup.py` & `gretel-trainer-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/benchmark/__init__.py` & `gretel-trainer-0.9.1/src/gretel_trainer/benchmark/__init__.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/benchmark/compare.py` & `gretel-trainer-0.9.1/src/gretel_trainer/benchmark/compare.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/benchmark/core.py` & `gretel-trainer-0.9.1/src/gretel_trainer/benchmark/core.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/benchmark/custom/datasets.py` & `gretel-trainer-0.9.1/src/gretel_trainer/benchmark/custom/datasets.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/benchmark/custom/executor.py` & `gretel-trainer-0.9.1/src/gretel_trainer/benchmark/custom/executor.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/benchmark/gretel/datasets.py` & `gretel-trainer-0.9.1/src/gretel_trainer/benchmark/gretel/datasets.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/benchmark/gretel/executor.py` & `gretel-trainer-0.9.1/src/gretel_trainer/benchmark/gretel/executor.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/benchmark/gretel/models.py` & `gretel-trainer-0.9.1/src/gretel_trainer/benchmark/gretel/models.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/benchmark/gretel/sdk.py` & `gretel-trainer-0.9.1/src/gretel_trainer/benchmark/gretel/sdk.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/models.py` & `gretel-trainer-0.9.1/src/gretel_trainer/models.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/relational/README.md` & `gretel-trainer-0.9.1/src/gretel_trainer/relational/README.md`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/relational/ancestry.py` & `gretel-trainer-0.9.1/src/gretel_trainer/relational/ancestry.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/relational/artifacts.py` & `gretel-trainer-0.9.1/src/gretel_trainer/relational/artifacts.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/relational/backup.py` & `gretel-trainer-0.9.1/src/gretel_trainer/relational/backup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from __future__ import annotations
 
 from dataclasses import asdict, dataclass
-from typing import Any, Optional
+from typing import Any, Optional, Union
 
 from gretel_trainer.relational.artifacts import ArtifactCollection
-from gretel_trainer.relational.core import ForeignKey, RelationalData
+from gretel_trainer.relational.core import ForeignKey, RelationalData, Scope
+from gretel_trainer.relational.json import InventedTableMetadata, ProducerMetadata
 
 
 @dataclass
 class BackupRelationalDataTable:
     primary_key: list[str]
     invented_table_metadata: Optional[dict[str, Any]] = None
+    producer_metadata: Optional[dict[str, Any]] = None
 
 
 @dataclass
 class BackupForeignKey:
     table: str
     constrained_columns: list[str]
     referred_table: str
@@ -27,57 +29,52 @@
             constrained_columns=fk.columns,
             referred_table=fk.parent_table_name,
             referred_columns=fk.parent_columns,
         )
 
 
 @dataclass
-class BackupRelationalJson:
-    original_table_name: str
-    original_primary_key: list[str]
-    original_columns: list[str]
-    table_name_mappings: dict[str, str]
-
-
-@dataclass
 class BackupRelationalData:
     tables: dict[str, BackupRelationalDataTable]
     foreign_keys: list[BackupForeignKey]
-    relational_jsons: dict[str, BackupRelationalJson]
 
     @classmethod
     def from_relational_data(cls, rel_data: RelationalData) -> BackupRelationalData:
         tables = {}
         foreign_keys = []
-        relational_jsons = {}
-        for table in rel_data.list_all_tables():
-            backup_table = BackupRelationalDataTable(
+        for table in rel_data.list_all_tables(Scope.ALL):
+            tables[table] = BackupRelationalDataTable(
                 primary_key=rel_data.get_primary_key(table),
+                invented_table_metadata=_optionally_as_dict(
+                    rel_data.get_invented_table_metadata(table)
+                ),
+                producer_metadata=_optionally_as_dict(
+                    rel_data.get_producer_metadata(table)
+                ),
             )
-            if (
-                invented_table_metadata := rel_data.get_invented_table_metadata(table)
-            ) is not None:
-                backup_table.invented_table_metadata = asdict(invented_table_metadata)
-            tables[table] = backup_table
-            foreign_keys.extend(
-                [
-                    BackupForeignKey.from_fk(key)
-                    for key in rel_data.get_foreign_keys(table)
-                ]
-            )
-        for key, rel_json in rel_data.relational_jsons.items():
-            relational_jsons[key] = BackupRelationalJson(
-                original_table_name=rel_json.original_table_name,
-                original_primary_key=rel_json.original_primary_key,
-                original_columns=rel_json.original_columns,
-                table_name_mappings=rel_json.table_name_mappings,
-            )
-        return BackupRelationalData(
-            tables=tables, foreign_keys=foreign_keys, relational_jsons=relational_jsons
-        )
+
+            # Producer tables delegate their foreign keys to root invented tables.
+            # We exclude producers here to avoid adding duplicate foreign keys.
+            if not rel_data.is_producer_of_invented_tables(table):
+                foreign_keys.extend(
+                    [
+                        BackupForeignKey.from_fk(key)
+                        for key in rel_data.get_foreign_keys(table)
+                    ]
+                )
+        return BackupRelationalData(tables=tables, foreign_keys=foreign_keys)
+
+
+def _optionally_as_dict(
+    metadata: Optional[Union[InventedTableMetadata, ProducerMetadata]]
+) -> Optional[dict[str, Any]]:
+    if metadata is None:
+        return None
+
+    return asdict(metadata)
 
 
 @dataclass
 class BackupClassify:
     model_ids: dict[str, str]
 
 
@@ -133,18 +130,14 @@
                     table=fk["table"],
                     constrained_columns=fk["constrained_columns"],
                     referred_table=fk["referred_table"],
                     referred_columns=fk["referred_columns"],
                 )
                 for fk in relational_data.get("foreign_keys", [])
             ],
-            relational_jsons={
-                k: BackupRelationalJson(**v)
-                for k, v in relational_data.get("relational_jsons", {}).items()
-            },
         )
 
         backup = Backup(
             project_name=b["project_name"],
             strategy=b["strategy"],
             gretel_model=b["gretel_model"],
             working_dir=b["working_dir"],
```

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/relational/connectors.py` & `gretel-trainer-0.9.1/src/gretel_trainer/relational/connectors.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,24 +5,27 @@
 the "Connector.extract" method, a "RelationalData" instance is provided
 which you can then use with the "MultiTable" class to process data with
 Gretel Transforms, Classify, Synthetics, or a combination of both.
 """
 from __future__ import annotations
 
 import logging
-import tempfile
 from pathlib import Path
 from typing import Optional
 
 import pandas as pd
 from sqlalchemy import create_engine
 from sqlalchemy.engine.base import Engine
 from sqlalchemy.exc import OperationalError
 
-from gretel_trainer.relational.core import MultiTableException, RelationalData
+from gretel_trainer.relational.core import (
+    DEFAULT_RELATIONAL_SOURCE_DIR,
+    MultiTableException,
+    RelationalData,
+)
 from gretel_trainer.relational.extractor import ExtractorConfig, TableExtractor
 
 logger = logging.getLogger(__name__)
 
 
 class Connector:
     """
@@ -64,48 +67,52 @@
 
     def extract(
         self,
         only: Optional[set[str]] = None,
         ignore: Optional[set[str]] = None,
         schema: Optional[str] = None,
         config: Optional[ExtractorConfig] = None,
+        storage_dir: str = DEFAULT_RELATIONAL_SOURCE_DIR,
     ) -> RelationalData:
         """
         Extracts table data and relationships from the database. Optional args include:
 
         Args:
             only: Only extract these table names, cannot be used with `ignore`
             ignore: Skip extracting these table names, cannot be used with `only`
             schema: An optional schema name that is passed through to SQLAlchemy, may only
                 be used with certain dialects.
             config: An optional extraction config. This config can be used to only include
                 specific tables, ignore specific tables, and configure subsetting. Please
                 see the `ExtractorConfig` docs for more details.
+            storage_dir: The output directory where extracted data is stored.
         """
         if only is not None and ignore is not None:
             raise MultiTableException("Cannot specify both `only` and `ignore`.")
 
         if config is None:
             config = ExtractorConfig(
                 only=only, ignore=ignore, schema=schema  # pyright: ignore
             )
 
-        with tempfile.TemporaryDirectory() as tmpdir:
-            extractor = TableExtractor(
-                config=config, connector=self, storage_dir=Path(tmpdir)
-            )
-            extractor.sample_tables()
+        storage_dir_path = Path(storage_dir)
+        storage_dir_path.mkdir(parents=True, exist_ok=True)
 
-            # We ensure to re-create RelationalData after extraction so
-            # we can account for any embedded JSON. This also loads
-            # each table as a DF in the object which is currently
-            # the expected behavior for later operations.
-            extractor._relational_data = extractor._create_rel_data(
-                extracted_tables=extractor.table_order
-            )
+        extractor = TableExtractor(
+            config=config, connector=self, storage_dir=storage_dir_path
+        )
+        extractor.sample_tables()
+
+        # We ensure to re-create RelationalData after extraction so
+        # we can account for any embedded JSON. This also loads
+        # each table as a DF in the object which is currently
+        # the expected behavior for later operations.
+        extractor._relational_data = extractor._create_rel_data(
+            extracted_tables=extractor.table_order
+        )
 
         return extractor.relational_data
 
     def save(self, tables: dict[str, pd.DataFrame], prefix: str = "") -> None:
         for name, data in tables.items():
             data.to_sql(
                 f"{prefix}{name}", con=self.engine, if_exists="replace", index=False
```

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/relational/core.py` & `gretel-trainer-0.9.1/src/gretel_trainer/relational/core.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,33 +11,38 @@
 
 Please see the specific docs for the "RelationalData" class on how to do this.
 """
 
 from __future__ import annotations
 
 import logging
+import shutil
+import tempfile
 from dataclasses import dataclass, replace
 from enum import Enum
 from pathlib import Path
 from typing import Any, Optional, Union
 
 import networkx
 import pandas as pd
 from networkx.algorithms.dag import dag_longest_path_length, topological_sort
 from pandas.api.types import is_string_dtype
 
+import gretel_trainer.relational.json as relational_json
 from gretel_trainer.relational.json import (
     IngestResponseT,
     InventedTableMetadata,
-    RelationalJson,
-    get_json_columns,
+    ProducerMetadata,
 )
 
 logger = logging.getLogger(__name__)
 
+DEFAULT_RELATIONAL_SOURCE_DIR = "relational_source"
+PREVIEW_ROW_COUNT = 5
+
 
 class MultiTableException(Exception):
     pass
 
 
 GretelModelConfig = Union[str, Path, dict]
 
@@ -46,14 +51,15 @@
 class ForeignKey:
     table_name: str
     columns: list[str]
     parent_table_name: str
     parent_columns: list[str]
 
 
+UserFriendlyDataT = Union[pd.DataFrame, str, Path]
 UserFriendlyPrimaryKeyT = Optional[Union[str, list[str]]]
 
 
 class Scope(str, Enum):
     """
     Various non-mutually-exclusive sets of tables known to the system
     """
@@ -83,20 +89,29 @@
     Includes all tables invented from un-modelable user source tables
     """
 
 
 @dataclass
 class TableMetadata:
     primary_key: list[str]
-    data: pd.DataFrame
+    source: Path
     columns: list[str]
     invented_table_metadata: Optional[InventedTableMetadata] = None
+    producer_metadata: Optional[ProducerMetadata] = None
     safe_ancestral_seed_columns: Optional[set[str]] = None
 
 
+@dataclass
+class _RemovedTableMetadata:
+    source: Path
+    primary_key: list[str]
+    fks_to_parents: list[ForeignKey]
+    fks_from_children: list[ForeignKey]
+
+
 class RelationalData:
     """
     Stores information about multiple tables and their relationships. When
     using this object you could create it without any arguments and rely
     on the instance methods for adding tables and key relationships.
 
     Example::
@@ -105,17 +120,18 @@
         rel_data.add_table(...)
         rel_data.add_table(...)
         rel_data.add_foreign_key_constraint(...)
 
     See the specific method docstrings for details on each method.
     """
 
-    def __init__(self):
+    def __init__(self, directory: Optional[Union[str, Path]] = None):
+        self.dir = Path(directory or DEFAULT_RELATIONAL_SOURCE_DIR)
+        self.dir.mkdir(parents=True, exist_ok=True)
         self.graph = networkx.DiGraph()
-        self.relational_jsons: dict[str, RelationalJson] = {}
 
     @property
     def is_empty(self) -> bool:
         """
         Return a bool to indicate if the `RelationalData` contains
         any table information.
         """
@@ -129,93 +145,163 @@
         Users should rely on MultiTable calling this internally when appropriate and not
         need to do so themselves.
         """
         restored = {}
         discarded = set()
 
         # Restore any invented tables to nested-JSON format
-        for table_name, rel_json in self.relational_jsons.items():
+        producers = {
+            table: pmeta
+            for table in self.list_all_tables(Scope.ALL)
+            if (pmeta := self.get_producer_metadata(table)) is not None
+        }
+        for table_name, producer_metadata in producers.items():
             tables = {
                 table: data
                 for table, data in tableset.items()
-                if table in rel_json.table_names
+                if table in producer_metadata.table_names
             }
-            data = rel_json.restore(tables, self)
+            data = relational_json.restore(
+                tables=tables,
+                rel_data=self,
+                root_table_name=producer_metadata.invented_root_table_name,
+                original_columns=self.get_table_columns(table_name),
+                table_name_mappings=producer_metadata.table_name_mappings,
+                original_table_name=table_name,
+            )
             if data is not None:
                 restored[table_name] = data
-            discarded.update(rel_json.table_names)
+            discarded.update(producer_metadata.table_names)
 
         # Add remaining tables
         for table, data in tableset.items():
             if table not in discarded:
                 restored[table] = data
 
         return restored
 
     def add_table(
         self,
         *,
         name: str,
         primary_key: UserFriendlyPrimaryKeyT,
-        data: pd.DataFrame,
+        data: UserFriendlyDataT,
     ) -> None:
         """
         Add a table. The primary key can be None (if one is not defined on the table),
         a string column name (most common), or a list of multiple string column names (composite key).
 
         This call MAY result in multiple tables getting "registered," specifically if
         the table includes nested JSON data.
         """
         primary_key = self._format_key_column(primary_key)
-        if (rj_ingest := self._check_for_json(name, primary_key, data)) is not None:
-            self._add_rel_json_and_tables(name, rj_ingest)
-        else:
-            self._add_single_table(name=name, primary_key=primary_key, data=data)
+        source_path = Path(f"{self.dir}/{name}.csv")
 
-    def _check_for_json(
-        self,
-        table: str,
-        primary_key: list[str],
-        data: pd.DataFrame,
-    ) -> Optional[IngestResponseT]:
-        json_cols = get_json_columns(data)
+        # Preview data to get list of columns and determine if there is any JSON
+        if isinstance(data, pd.DataFrame):
+            preview_df = data.head(PREVIEW_ROW_COUNT)
+        elif isinstance(data, (str, Path)):
+            preview_df = pd.read_csv(data, nrows=PREVIEW_ROW_COUNT)
+        columns = list(preview_df.columns)
+        json_cols = relational_json.get_json_columns(preview_df)
+
+        # Write/copy source to preferred internal location
+        if isinstance(data, pd.DataFrame):
+            relational_json.jsonencode(data, json_cols).to_csv(source_path, index=False)
+        elif isinstance(data, (str, Path)):
+            shutil.copyfile(data, source_path)
+
+        # If we found JSON in preview above, run JSON ingestion on full data
+        rj_ingest = None
         if len(json_cols) > 0:
             logger.info(
-                f"Detected JSON data in table `{table}`. Running JSON normalization."
+                f"Detected JSON data in table `{name}`. Running JSON normalization."
+            )
+            if isinstance(data, pd.DataFrame):
+                df = data
+            elif isinstance(data, (str, Path)):
+                df = pd.read_csv(data)
+            rj_ingest = relational_json.ingest(name, primary_key, df, json_cols)
+
+        # Add the table(s)
+        if rj_ingest is not None:
+            self._add_producer_and_invented_tables(
+                name, primary_key, source_path, columns, rj_ingest
+            )
+        else:
+            self._add_single_table(
+                name=name,
+                primary_key=primary_key,
+                source=source_path,
+                columns=columns,
             )
-            return RelationalJson.ingest(table, primary_key, data, json_cols)
 
-    def _add_rel_json_and_tables(self, table: str, rj_ingest: IngestResponseT) -> None:
-        rel_json, commands = rj_ingest
+    def _add_producer_and_invented_tables(
+        self,
+        table: str,
+        primary_key: list[str],
+        source: Path,
+        columns: list[str],
+        rj_ingest: IngestResponseT,
+    ) -> None:
+        commands, producer_metadata = rj_ingest
         tables, foreign_keys = commands
 
-        self.relational_jsons[table] = rel_json
+        # Add the producer table
+        self._add_single_table(
+            name=table,
+            primary_key=primary_key,
+            source=source,
+            columns=columns,
+            producer_metadata=producer_metadata,
+        )
 
+        # Add the invented tables
         for tbl in tables:
-            self._add_single_table(**tbl)
+            name = tbl["name"]
+            source_path = Path(f"{self.dir}/{name}.csv")
+            df = tbl["data"]
+            df.to_csv(source_path, index=False)
+            self._add_single_table(
+                name=name,
+                primary_key=tbl["primary_key"],
+                source=source_path,
+                columns=list(df.columns),
+                invented_table_metadata=tbl["invented_table_metadata"],
+            )
         for foreign_key in foreign_keys:
             self.add_foreign_key_constraint(**foreign_key)
 
     def _add_single_table(
         self,
         *,
         name: str,
         primary_key: UserFriendlyPrimaryKeyT,
-        data: pd.DataFrame,
+        source: Path,
+        columns: Optional[list[str]] = None,
         invented_table_metadata: Optional[InventedTableMetadata] = None,
+        producer_metadata: Optional[ProducerMetadata] = None,
     ) -> None:
         primary_key = self._format_key_column(primary_key)
+        columns = columns or list(pd.read_csv(source, nrows=1).columns)
         metadata = TableMetadata(
             primary_key=primary_key,
-            data=data,
-            columns=list(data.columns),
+            source=source,
+            columns=columns,
             invented_table_metadata=invented_table_metadata,
+            producer_metadata=producer_metadata,
         )
         self.graph.add_node(name, metadata=metadata)
 
+    def _get_table_metadata(self, table: str) -> TableMetadata:
+        try:
+            return self.graph.nodes[table]["metadata"]
+        except KeyError:
+            raise MultiTableException(f"Unrecognized table: `{table}`")
+
     def set_primary_key(
         self, *, table: str, primary_key: UserFriendlyPrimaryKeyT
     ) -> None:
         """
         (Re)set the primary key on an existing table.
         If the table does not yet exist in the instance's collection, add it via `add_table`.
         """
@@ -225,67 +311,94 @@
         primary_key = self._format_key_column(primary_key)
 
         known_columns = self.get_table_columns(table)
         for col in primary_key:
             if col not in known_columns:
                 raise MultiTableException(f"Unrecognized column name: `{col}`")
 
-        if self.relational_jsons.get(table) is not None:
-            original_data, _, original_fks = self._remove_relational_json(table)
-            if original_data is None:
-                raise MultiTableException("Original data with JSON is lost.")
-
-            new_rj_ingest = RelationalJson.ingest(table, primary_key, original_data)
-            if new_rj_ingest is None:
-                raise MultiTableException(
-                    "Failed to change primary key on tables invented from JSON data"
-                )
+        # Prevent interfering with manually invented tables
+        if self._is_invented(table):
+            raise MultiTableException("Cannot change primary key on invented tables")
+
+        # If `table` is a producer of invented tables, we redo JSON ingestion
+        # to ensure primary keys are set properly on invented tables
+        elif self.is_producer_of_invented_tables(table):
+            source = self.get_table_source(table)
+            with tempfile.TemporaryDirectory() as tmpdir:
+                tmpfile = Path(tmpdir) / f"{table}.csv"
+                shutil.move(source, tmpfile)
+                removal_metadata = self._remove_producer(table)
+                self.add_table(name=table, primary_key=primary_key, data=tmpfile)
+            self._restore_fks_in_both_directions(table, removal_metadata)
 
-            self._add_rel_json_and_tables(table, new_rj_ingest)
-            for fk in original_fks:
-                self.add_foreign_key_constraint(
-                    table=fk.table_name,
-                    constrained_columns=fk.columns,
-                    referred_table=fk.parent_table_name,
-                    referred_columns=fk.parent_columns,
-                )
+        # At this point we are working with a "normal" table
         else:
-            self.graph.nodes[table]["metadata"].primary_key = primary_key
+            self._get_table_metadata(table).primary_key = primary_key
             self._clear_safe_ancestral_seed_columns(table)
 
+    def _restore_fks_in_both_directions(
+        self, table: str, removal_metadata: _RemovedTableMetadata
+    ) -> None:
+        for fk in removal_metadata.fks_to_parents:
+            self.add_foreign_key_constraint(
+                table=table,
+                constrained_columns=fk.columns,
+                referred_table=fk.parent_table_name,
+                referred_columns=fk.parent_columns,
+            )
+
+        for fk in removal_metadata.fks_from_children:
+            self.add_foreign_key_constraint(
+                table=fk.table_name,
+                constrained_columns=fk.columns,
+                referred_table=table,
+                referred_columns=fk.parent_columns,
+            )
+
     def _get_user_defined_fks_to_table(self, table: str) -> list[ForeignKey]:
         return [
             fk
             for child in self.graph.predecessors(table)
             for fk in self.get_foreign_keys(child)
             if fk.parent_table_name == table and not self._is_invented(fk.table_name)
         ]
 
-    def _remove_relational_json(
-        self, table: str
-    ) -> tuple[Optional[pd.DataFrame], list[str], list[ForeignKey]]:
+    def _remove_producer(self, table: str) -> _RemovedTableMetadata:
         """
-        Removes the RelationalJson instance and removes all invented tables from the graph.
+        Removes the producer table and all its invented tables from the graph
+        (which in turn removes all edges (foreign keys) to/from other tables).
 
-        Returns the original data, primary key, and foreign keys.
+        Returns a _RemovedTableMetadata object for restoring metadata in broader "update" contexts.
         """
-        rel_json = self.relational_jsons[table]
+        table_metadata = self._get_table_metadata(table)
+        producer_metadata = table_metadata.producer_metadata
+
+        if producer_metadata is None:
+            raise MultiTableException(
+                "Cannot remove invented tables from non-producer table"
+            )
 
-        original_data = rel_json.original_data
-        original_primary_key = rel_json.original_primary_key
-        original_foreign_keys = self._get_user_defined_fks_to_table(
-            rel_json.root_table_name
+        removal_metadata = _RemovedTableMetadata(
+            source=table_metadata.source,
+            primary_key=table_metadata.primary_key,
+            fks_to_parents=self.get_foreign_keys(table),
+            fks_from_children=self._get_user_defined_fks_to_table(
+                self._get_fk_delegate_table(table)
+            ),
         )
 
-        for invented_table_name in rel_json.table_names:
+        for invented_table_name in producer_metadata.table_names:
             if invented_table_name in self.graph.nodes:
-                self.graph.remove_node(invented_table_name)
-        del self.relational_jsons[table]
+                self._remove_node(invented_table_name)
+        self._remove_node(table)
 
-        return original_data, original_primary_key, original_foreign_keys
+        return removal_metadata
+
+    def _remove_node(self, table: str) -> None:
+        self.graph.remove_node(table)
 
     def _format_key_column(self, key: Optional[Union[str, list[str]]]) -> list[str]:
         if key is None:
             return []
         elif isinstance(key, str):
             return [key]
         else:
@@ -336,17 +449,14 @@
         if referred_table not in known_tables:
             logger.warning(f"Unrecognized table name: `{referred_table}`")
             abort = True
 
         if abort:
             raise MultiTableException("Unrecognized table(s) in foreign key arguments")
 
-        table = self._get_table_in_graph(table)
-        referred_table = self._get_table_in_graph(referred_table)
-
         if len(constrained_columns) != len(referred_columns):
             logger.warning(
                 "Constrained and referred columns must be of the same length"
             )
             raise MultiTableException(
                 "Invalid column constraints in foreign key arguments"
             )
@@ -365,26 +475,30 @@
                     f"Referred column `{col}` does not exist on table `{referred_table}`"
                 )
                 abort = True
 
         if abort:
             raise MultiTableException("Unrecognized column(s) in foreign key arguments")
 
-        self.graph.add_edge(table, referred_table)
-        edge = self.graph.edges[table, referred_table]
+        fk_delegate_table = self._get_fk_delegate_table(table)
+        fk_delegate_referred_table = self._get_fk_delegate_table(referred_table)
+
+        self.graph.add_edge(fk_delegate_table, fk_delegate_referred_table)
+        edge = self.graph.edges[fk_delegate_table, fk_delegate_referred_table]
         via = edge.get("via", [])
         via.append(
             ForeignKey(
-                table_name=table,
+                table_name=fk_delegate_table,
                 columns=constrained_columns,
-                parent_table_name=referred_table,
+                parent_table_name=fk_delegate_referred_table,
                 parent_columns=referred_columns,
             )
         )
         edge["via"] = via
+        self._clear_safe_ancestral_seed_columns(fk_delegate_table)
         self._clear_safe_ancestral_seed_columns(table)
 
     def remove_foreign_key(self, foreign_key: str) -> None:
         """
         DEPRECATED: Please use `remove_foreign_key_constraint` instead.
         """
         logger.warning(
@@ -401,171 +515,139 @@
     ) -> None:
         """
         Remove an existing foreign key.
         """
         if table not in self.list_all_tables(Scope.ALL):
             raise MultiTableException(f"Unrecognized table name: `{table}`")
 
-        table = self._get_table_in_graph(table)
-
         key_to_remove = None
         for fk in self.get_foreign_keys(table):
             if fk.columns == constrained_columns:
                 key_to_remove = fk
 
         if key_to_remove is None:
             raise MultiTableException(
                 f"`{table} does not have a foreign key with constrained columns {constrained_columns}`"
             )
 
-        edge = self.graph.edges[table, key_to_remove.parent_table_name]
+        fk_delegate_table = self._get_fk_delegate_table(table)
+
+        edge = self.graph.edges[fk_delegate_table, key_to_remove.parent_table_name]
         via = edge.get("via")
         via.remove(key_to_remove)
         if len(via) == 0:
-            self.graph.remove_edge(table, key_to_remove.parent_table_name)
+            self.graph.remove_edge(fk_delegate_table, key_to_remove.parent_table_name)
         else:
             edge["via"] = via
+        self._clear_safe_ancestral_seed_columns(fk_delegate_table)
         self._clear_safe_ancestral_seed_columns(table)
 
-    def update_table_data(self, table: str, data: pd.DataFrame) -> None:
+    def update_table_data(self, table: str, data: UserFriendlyDataT) -> None:
         """
         Set a DataFrame as the table data for a given table name.
         """
-        if table in self.relational_jsons:
-            _, original_pk, original_fks = self._remove_relational_json(table)
-            if (
-                new_rj_ingest := self._check_for_json(table, original_pk, data)
-            ) is not None:
-                self._add_rel_json_and_tables(table, new_rj_ingest)
-                parent_table_name = new_rj_ingest[0].root_table_name
-            else:
-                self._add_single_table(
-                    name=table,
-                    primary_key=original_pk,
-                    data=data,
-                )
-                parent_table_name = table
-            for fk in original_fks:
-                self.add_foreign_key_constraint(
-                    table=fk.table_name,
-                    constrained_columns=fk.columns,
-                    referred_table=parent_table_name,
-                    referred_columns=fk.parent_columns,
-                )
+        if self._is_invented(table):
+            raise MultiTableException("Cannot modify invented tables' data")
+        elif self.is_producer_of_invented_tables(table):
+            removal_metadata = self._remove_producer(table)
         else:
-            try:
-                metadata = self.graph.nodes[table]["metadata"]
-            except KeyError:
-                raise MultiTableException(
-                    f"Unrecognized table name: {table}. If this is a new table to add, use `add_table`."
-                )
+            removal_metadata = _RemovedTableMetadata(
+                source=Path(),  # we don't care about the old data
+                primary_key=self.get_primary_key(table),
+                fks_to_parents=self.get_foreign_keys(table),
+                fks_from_children=self._get_user_defined_fks_to_table(table),
+            )
+            self._remove_node(table)
 
-            if (
-                new_rj_ingest := self._check_for_json(table, metadata.primary_key, data)
-            ) is not None:
-                original_foreign_keys = self._get_user_defined_fks_to_table(table)
-                self.graph.remove_node(table)
-                self._add_rel_json_and_tables(table, new_rj_ingest)
-                for fk in original_foreign_keys:
-                    self.add_foreign_key_constraint(
-                        table=fk.table_name,
-                        constrained_columns=fk.columns,
-                        referred_table=new_rj_ingest[0].root_table_name,
-                        referred_columns=fk.parent_columns,
-                    )
-            else:
-                metadata.data = data
-                metadata.columns = list(data.columns)
-                self._clear_safe_ancestral_seed_columns(table)
+        self.add_table(name=table, primary_key=removal_metadata.primary_key, data=data)
+        self._restore_fks_in_both_directions(table, removal_metadata)
 
     def list_all_tables(self, scope: Scope = Scope.MODELABLE) -> list[str]:
         """
         Returns a list of table names belonging to the provided Scope.
         See "Scope" enum documentation for details.
         By default, returns tables that can be submitted as jobs to Gretel
         (i.e. that are MODELABLE).
         """
         graph_nodes = list(self.graph.nodes)
 
-        json_source_tables = [
-            rel_json.original_table_name
-            for _, rel_json in self.relational_jsons.items()
+        producer_tables = [
+            t for t in graph_nodes if self.is_producer_of_invented_tables(t)
         ]
 
-        all_tables = graph_nodes + json_source_tables
-
         modelable_tables = []
         evaluatable_tables = []
         invented_tables: list[str] = []
 
         for n in graph_nodes:
-            meta = self.graph.nodes[n]["metadata"]
+            meta = self._get_table_metadata(n)
             if (invented_meta := meta.invented_table_metadata) is not None:
                 invented_tables.append(n)
                 if invented_meta.invented_root_table_name == n:
                     evaluatable_tables.append(n)
                 if not invented_meta.empty:
                     modelable_tables.append(n)
             else:
-                modelable_tables.append(n)
-                evaluatable_tables.append(n)
+                if n not in producer_tables:
+                    modelable_tables.append(n)
+                    evaluatable_tables.append(n)
 
         if scope == Scope.MODELABLE:
             return modelable_tables
         elif scope == Scope.EVALUATABLE:
             return evaluatable_tables
         elif scope == Scope.INVENTED:
             return invented_tables
         elif scope == Scope.ALL:
-            return all_tables
+            return graph_nodes
         elif scope == Scope.PUBLIC:
-            return [t for t in all_tables if t not in invented_tables]
+            return [t for t in graph_nodes if t not in invented_tables]
 
     def _is_invented(self, table: str) -> bool:
-        return (
-            table in self.graph.nodes
-            and self.graph.nodes[table]["metadata"].invented_table_metadata is not None
-        )
+        return self.get_invented_table_metadata(table) is not None
+
+    def is_producer_of_invented_tables(self, table: str) -> bool:
+        return self.get_producer_metadata(table) is not None
 
     def get_modelable_table_names(self, table: str) -> list[str]:
         """
         Returns a list of MODELABLE table names connected to the provided table.
         If the provided table is the source of invented tables, returns the modelable invented tables created from it.
         If the provided table is itself modelable, returns that table name back.
         Otherwise returns an empty list.
         """
-        if (rel_json := self.relational_jsons.get(table)) is not None:
+        try:
+            table_metadata = self._get_table_metadata(table)
+        except MultiTableException:
+            return []
+
+        if (pmeta := table_metadata.producer_metadata) is not None:
             return [
                 t
-                for t in rel_json.table_names
+                for t in pmeta.table_names
                 if t in self.list_all_tables(Scope.MODELABLE)
             ]
         elif table in self.list_all_tables(Scope.MODELABLE):
             return [table]
         else:
             return []
 
     def get_public_name(self, table: str) -> Optional[str]:
-        if table in self.relational_jsons:
-            return table
-
-        if (
-            imeta := self.graph.nodes[table]["metadata"].invented_table_metadata
-        ) is not None:
+        if (imeta := self.get_invented_table_metadata(table)) is not None:
             return imeta.original_table_name
 
         return table
 
     def get_invented_table_metadata(
         self, table: str
     ) -> Optional[InventedTableMetadata]:
-        if table in self.relational_jsons:
-            return None
+        return self._get_table_metadata(table).invented_table_metadata
 
-        return self.graph.nodes[table]["metadata"].invented_table_metadata
+    def get_producer_metadata(self, table: str) -> Optional[ProducerMetadata]:
+        return self._get_table_metadata(table).producer_metadata
 
     def get_parents(self, table: str) -> list[str]:
         """
         Given a table name, return the table names that are referred to
         by the foreign keys in this table.
         """
         return list(self.graph.successors(table))
@@ -617,53 +699,37 @@
         return list(reversed(list(topological_sort(self.graph))))
 
     def get_primary_key(self, table: str) -> list[str]:
         """
         Return the list of columns defining the primary key for a table.
         It may be a single column or multiple columns (composite key).
         """
-        try:
-            return self.graph.nodes[table]["metadata"].primary_key
-        except KeyError:
-            if table in self.relational_jsons:
-                return self.relational_jsons[table].original_primary_key
-            else:
-                raise MultiTableException(f"Unrecognized table: `{table}`")
+        return self._get_table_metadata(table).primary_key
+
+    def get_table_source(self, table: str) -> Path:
+        return self._get_table_metadata(table).source
 
     def get_table_data(
         self, table: str, usecols: Optional[list[str]] = None
     ) -> pd.DataFrame:
         """
         Return the table contents for a given table name as a DataFrame.
         """
+        source = self.get_table_source(table)
         usecols = usecols or self.get_table_columns(table)
-        try:
-            return self.graph.nodes[table]["metadata"].data[usecols]
-        except KeyError:
-            if table in self.relational_jsons:
-                if (df := self.relational_jsons[table].original_data) is None:
-                    raise MultiTableException("Original data with JSON is lost.")
-                return df
-            else:
-                raise MultiTableException(f"Unrecognized table: `{table}`")
+        return pd.read_csv(source, usecols=usecols)
 
     def get_table_columns(self, table: str) -> list[str]:
         """
         Return the column names for a provided table name.
         """
-        try:
-            return self.graph.nodes[table]["metadata"].columns
-        except KeyError:
-            if table in self.relational_jsons:
-                return self.relational_jsons[table].original_columns
-            else:
-                raise MultiTableException(f"Unrecognized table: `{table}`")
+        return self._get_table_metadata(table).columns
 
     def get_safe_ancestral_seed_columns(self, table: str) -> set[str]:
-        safe_columns = self.graph.nodes[table]["metadata"].safe_ancestral_seed_columns
+        safe_columns = self._get_table_metadata(table).safe_ancestral_seed_columns
         if safe_columns is None:
             safe_columns = self._set_safe_ancestral_seed_columns(table)
         return safe_columns
 
     def _set_safe_ancestral_seed_columns(self, table: str) -> set[str]:
         cols = set()
 
@@ -675,44 +741,37 @@
         data = self.get_table_data(table)
         for col in self.get_table_columns(table):
             if col in cols:
                 continue
             if _ok_for_train_and_seed(col, data):
                 cols.add(col)
 
-        self.graph.nodes[table]["metadata"].safe_ancestral_seed_columns = cols
+        self._get_table_metadata(table).safe_ancestral_seed_columns = cols
         return cols
 
     def _clear_safe_ancestral_seed_columns(self, table: str) -> None:
-        self.graph.nodes[table]["metadata"].safe_ancestral_seed_columns = None
+        self._get_table_metadata(table).safe_ancestral_seed_columns = None
+
+    def _get_fk_delegate_table(self, table: str) -> str:
+        if (pmeta := self.get_producer_metadata(table)) is not None:
+            return pmeta.invented_root_table_name
 
-    def _get_table_in_graph(self, table: str) -> str:
-        if table in self.relational_jsons:
-            table = self.relational_jsons[table].root_table_name
         return table
 
     def get_foreign_keys(
         self, table: str, rename_invented_tables: bool = False
     ) -> list[ForeignKey]:
         def _rename_invented(fk: ForeignKey) -> ForeignKey:
-            table_name = fk.table_name
-            parent_table_name = fk.parent_table_name
-            if self._is_invented(table_name):
-                table_name = self.graph.nodes[table_name][
-                    "metadata"
-                ].invented_table_metadata.original_table_name
-            if self._is_invented(parent_table_name):
-                parent_table_name = self.graph.nodes[parent_table_name][
-                    "metadata"
-                ].invented_table_metadata.original_table_name
+            table_name = self.get_public_name(fk.table_name)
+            parent_table_name = self.get_public_name(fk.parent_table_name)
             return replace(
                 fk, table_name=table_name, parent_table_name=parent_table_name
             )
 
-        table = self._get_table_in_graph(table)
+        table = self._get_fk_delegate_table(table)
         foreign_keys = []
         for parent in self.get_parents(table):
             fks = self.graph.edges[table, parent]["via"]
             foreign_keys.extend(fks)
 
         if rename_invented_tables:
             return [_rename_invented(fk) for fk in foreign_keys]
@@ -733,32 +792,45 @@
 
         all_tables = self.list_all_tables(Scope.ALL)
         total_foreign_key_count = 0
         tables = {}
         for table in all_tables:
             this_table_foreign_key_count = 0
             foreign_keys = []
-            fk_lookup_table_name = self._get_table_in_graph(table)
-            for key in self.get_foreign_keys(fk_lookup_table_name):
+            for key in self.get_foreign_keys(table):
                 total_foreign_key_count = total_foreign_key_count + 1
                 this_table_foreign_key_count = this_table_foreign_key_count + 1
                 foreign_keys.append(
                     {
                         "columns": key.columns,
                         "parent_table_name": key.parent_table_name,
                         "parent_columns": key.parent_columns,
                     }
                 )
-            tables[table] = {
+            table_metadata = {
                 "column_count": len(self.get_table_columns(table)),
                 "primary_key": self.get_primary_key(table),
                 "foreign_key_count": this_table_foreign_key_count,
                 "foreign_keys": foreign_keys,
                 "is_invented_table": self._is_invented(table),
             }
+            if (producer_metadata := self.get_producer_metadata(table)) is not None:
+                table_metadata["invented_table_details"] = {
+                    "table_type": "producer",
+                    "json_to_table_mappings": producer_metadata.table_name_mappings,
+                }
+            elif (
+                invented_table_metadata := self.get_invented_table_metadata(table)
+            ) is not None:
+                table_metadata["invented_table_details"] = {
+                    "table_type": "invented",
+                    "json_breadcrumb_path": invented_table_metadata.json_breadcrumb_path,
+                }
+            tables[table] = table_metadata
+
         return {
             "foreign_key_count": total_foreign_key_count,
             "max_depth": max_depth,
             "tables": tables,
             "public_table_count": public_table_count,
             "invented_table_count": invented_table_count,
         }
```

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/relational/extractor.py` & `gretel-trainer-0.9.1/src/gretel_trainer/relational/extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     """
     Configuration class for extracting tables from a remote database. An instance
     of this class should be passed as a param to the "TableExtractor" constructor.
     """
 
     target_row_count: float = -1.0
     """
-    The target number of rows (or ratio of rows) to sample. This will be used as the sample target for "leaf" tables, 
+    The target number of rows (or ratio of rows) to sample. This will be used as the sample target for "leaf" tables,
     or tables that do not have any references to their primary keys. If this number is >= 1 then
     that number of rows will be used, if the value is between 0..1 then it is considered to be a percetange
     of the total number of rows. A 0 value will just extract headers and -1 will extract entire tables.
 
     The default value, -1, implies that full tables should be extracted.
     """
 
@@ -232,15 +232,15 @@
         self._config = config
 
         if not storage_dir.is_dir():
             raise ValueError("The `storage_dir` must be a directory!")
 
         self._storage_dir = storage_dir
 
-        self._relational_data = RelationalData()
+        self._relational_data = RelationalData(directory=self._storage_dir)
         self.table_order = []
         self._chunk_size = 50_000
 
     def _get_table_session(self, table_name: str) -> _TableSession:
         metadata = MetaData()
         metadata.reflect(only=[table_name], bind=self._connector.engine)
         table = metadata.tables[table_name]
@@ -264,15 +264,15 @@
 
         NOTE: If `extracted_tables` are provided, then these tables must have already been
         extracted!
         """
         if extracted_tables is None:
             extracted_tables = []
 
-        rel_data = RelationalData()
+        rel_data = RelationalData(directory=self._storage_dir)
         inspector = inspect(self._connector.engine)
         foreign_keys: list[tuple[str, dict]] = []
 
         for table_name in inspector.get_table_names(schema=self._config.schema):
             if self._config._should_skip_table(table_name):
                 continue
```

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/relational/json.py` & `gretel-trainer-0.9.1/src/gretel_trainer/relational/json.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from __future__ import annotations
 
-import hashlib
 import logging
 import re
 from dataclasses import dataclass
-from json import JSONDecodeError, loads
+from json import JSONDecodeError, dumps, loads
 from typing import Any, Optional, Protocol, Union
+from uuid import uuid4
 
 import numpy as np
 import pandas as pd
 from unflatten import unflatten
 
 logger = logging.getLogger(__name__)
 
-PREVIEW_ROW_COUNT = 5
-
 # JSON dict to multi-column and list to multi-table
 
 FIELD_SEPARATOR = ">"
 TABLE_SEPARATOR = "^"
 ID_SUFFIX = "~id"
 ORDER_COLUMN = "array~order"
 CONTENT_COLUMN = "content"
@@ -114,23 +112,67 @@
 
 
 def _is_invented_child_table(table: str, rel_data: _RelationalData) -> bool:
     imeta = rel_data.get_invented_table_metadata(table)
     return imeta is not None and imeta.invented_root_table_name != table
 
 
-def sanitize_str(s):
+def generate_unique_table_name(s: str):
     sanitized_str = "-".join(re.findall(r"[a-zA-Z_0-9]+", s))
-    # Generate suffix from original string, in case of sanitized_str collision
-    unique_suffix = make_suffix(s)
-    return f"{sanitized_str}-{unique_suffix}"
+    # Generate unique suffix to prevent collisions
+    unique_suffix = make_suffix()
+    # Max length for a table/filename is 128 chars
+    return f"{sanitized_str[:80]}_invented_{unique_suffix}"
+
+
+def make_suffix():
+    return uuid4().hex
+
+
+def jsonencode(df: pd.DataFrame, cols: list[str]) -> pd.DataFrame:
+    """
+    Returns a dataframe with the specified columns transformed such that their JSON-like
+    values can be written to CSV and later re-read back to Pandas from CSV.
+    """
+    # Save memory and return the *original dataframe* (not a copy!) if no columns to transform
+    if len(cols) == 0:
+        return df
 
+    def _jsonencode(x):
+        if isinstance(x, str):
+            return x
+        elif isinstance(x, (dict, list)):
+            return dumps(x)
 
-def make_suffix(s):
-    return hashlib.sha256(s.encode("utf-8")).hexdigest()[:10]
+    copy = df.copy()
+    for col in cols:
+        copy[col] = copy[col].map(_jsonencode)
+
+    return copy
+
+
+def jsondecode(df: pd.DataFrame, cols: list[str]) -> pd.DataFrame:
+    """
+    Returns a dataframe with the specified columns parsed from JSON to Python objects.
+    """
+    # Save memory and return the *original dataframe* (not a copy!) if no columns to transform
+    if len(cols) == 0:
+        return df
+
+    def _jsondecode(obj):
+        try:
+            return loads(obj)
+        except (ValueError, TypeError, JSONDecodeError):
+            return obj
+
+    copy = df.copy()
+    for col in cols:
+        copy[col] = copy[col].map(_jsondecode)
+
+    return copy
 
 
 class _RelationalData(Protocol):
     def get_foreign_keys(
         self, table: str
     ) -> list:  # can't specify element type (ForeignKey) without cyclic dependency
         ...
@@ -144,231 +186,228 @@
         ...
 
 
 @dataclass
 class InventedTableMetadata:
     invented_root_table_name: str
     original_table_name: str
+    json_breadcrumb_path: str
     empty: bool
 
 
-class RelationalJson:
-    def __init__(
-        self,
-        original_table_name: str,
-        original_primary_key: list[str],
-        original_columns: list[str],
-        original_data: Optional[pd.DataFrame],
-        table_name_mappings: dict[str, str],
-    ):
-        self.original_table_name = original_table_name
-        self.original_primary_key = original_primary_key
-        self.original_columns = original_columns
-        self.original_data = original_data
-        self.table_name_mappings = table_name_mappings
-
-    @classmethod
-    def ingest(
-        cls,
-        table_name: str,
-        primary_key: list[str],
-        df: pd.DataFrame,
-        json_columns: Optional[list[str]] = None,
-    ) -> Optional[IngestResponseT]:
-        tables = _normalize_json([(table_name, df.copy())], [], json_columns)
-        # If we created additional tables (from JSON lists) or added columns (from JSON dicts)
-        if len(tables) > 1 or len(tables[0][1].columns) > len(df.columns):
-            mappings = {name: sanitize_str(name) for name, _ in tables}
-            logger.info(f"Transformed JSON into {len(mappings)} tables for modeling.")
-            logger.debug(f"Invented table names: {list(mappings.values())}")
-            rel_json = RelationalJson(
-                original_table_name=table_name,
-                original_primary_key=primary_key,
-                original_data=df,
-                original_columns=list(df.columns),
-                table_name_mappings=mappings,
-            )
-            commands = _generate_commands(rel_json, tables)
-            return (rel_json, commands)
-
-    @property
-    def root_table_name(self) -> str:
-        return self.table_name_mappings[self.original_table_name]
+@dataclass
+class ProducerMetadata:
+    invented_root_table_name: str
+    table_name_mappings: dict[str, str]
 
     @property
     def table_names(self) -> list[str]:
-        """Returns sanitized, model-friendly table names, *including* those of empty invented tables."""
         return list(self.table_name_mappings.values())
 
-    @property
-    def inverse_table_name_mappings(self) -> dict[str, str]:
-        # Keys are sanitized, model-friendly names
-        # Values are "provenance" names (a^b>c) or the original table name
-        return {value: key for key, value in self.table_name_mappings.items()}
-
-    def restore(
-        self, tables: dict[str, pd.DataFrame], rel_data: _RelationalData
-    ) -> Optional[pd.DataFrame]:
-        """Reduces a set of tables (assumed to match the shapes created on initialization)
-        to a single table matching the shape of the original source table
-        """
-        # If the root invented table failed, we are completely out of luck
-        # (Missing invented child tables can be replaced with empty lists so we at least provide _something_)
-        if self.root_table_name not in tables:
-            logger.warning(
-                f"Cannot restore nested JSON data: root invented table `{self.root_table_name}` is missing from output tables."
-            )
-            return None
-
-        return self._denormalize_json(tables, rel_data)[self.original_columns]
 
-    def _denormalize_json(
-        self, tables: dict[str, pd.DataFrame], rel_data: _RelationalData
-    ) -> pd.DataFrame:
-        table_dict: dict = {
-            self.inverse_table_name_mappings[k]: v for k, v in tables.items()
-        }
-        for table_name in list(reversed(self.table_names)):
-            table_provenance_name = self.inverse_table_name_mappings[table_name]
-            empty_fallback = pd.DataFrame(
-                data={col: [] for col in rel_data.get_table_columns(table_name)},
-            )
-            table_df = table_dict.get(table_provenance_name, empty_fallback)
-
-            if table_df.empty and _is_invented_child_table(table_name, rel_data):
-                p_name = rel_data.get_foreign_keys(table_name)[0].parent_table_name
-                parent_name = self.inverse_table_name_mappings[p_name]
-                col_name = get_parent_column_name_from_child_table_name(
-                    table_provenance_name
-                )
-                kwargs = {col_name: table_dict[parent_name].apply(lambda x: [], axis=1)}
-                table_dict[parent_name] = table_dict[parent_name].assign(**kwargs)
-            else:
-                col_names = [col for col in table_df.columns if FIELD_SEPARATOR in col]
-                new_col_names = [col.replace(FIELD_SEPARATOR, ".") for col in col_names]
-                flat_df = table_df[col_names].rename(
-                    columns=dict(zip(col_names, new_col_names))
-                )
-                flat_dict = {
-                    k: {
-                        k1: v1
-                        for k1, v1 in v.items()
-                        if v1 is not np.nan and v1 is not None
-                    }
-                    for k, v in flat_df.to_dict("index").items()
-                }
-                dict_df = nulls_to_empty_dicts(
-                    pd.DataFrame.from_dict(
-                        {k: unflatten(v) for k, v in flat_dict.items()}, orient="index"
-                    )
-                )
-                nested_df = table_df.join(dict_df).drop(columns=col_names)
-                if _is_invented_child_table(table_name, rel_data):
-                    # we know there is exactly one foreign key on invented child tables...
-                    fk = rel_data.get_foreign_keys(table_name)[0]
-                    # ...with exactly one column
-                    fk_col = fk.columns[0]
-                    p_name = fk.parent_table_name
-                    parent_name = self.inverse_table_name_mappings[p_name]
-                    nested_df = (
-                        nested_df.sort_values(ORDER_COLUMN)
-                        .groupby(fk_col)[CONTENT_COLUMN]
-                        .agg(list)
-                    )
-                    col_name = get_parent_column_name_from_child_table_name(
-                        table_provenance_name
-                    )
-                    table_dict[parent_name] = table_dict[parent_name].join(
-                        nested_df.rename(col_name)
-                    )
-                    table_dict[parent_name][col_name] = nulls_to_empty_lists(
-                        table_dict[parent_name][col_name]
-                    )
-                table_dict[table_provenance_name] = nested_df
-        return table_dict[self.original_table_name]
+def ingest(
+    table_name: str,
+    primary_key: list[str],
+    df: pd.DataFrame,
+    json_columns: list[str],
+) -> Optional[IngestResponseT]:
+    json_decoded = jsondecode(df, json_columns)
+    tables = _normalize_json([(table_name, json_decoded)], [], json_columns)
+
+    # If we created additional tables (from JSON lists) or added columns (from JSON dicts)
+    if len(tables) > 1 or len(tables[0][1].columns) > len(df.columns):
+        # Map json breadcrumbs to uniquely generated table name
+        mappings = {name: generate_unique_table_name(table_name) for name, _ in tables}
+        logger.info(f"Transformed JSON into {len(mappings)} tables for modeling.")
+        logger.debug(f"Invented table names: {list(mappings.values())}")
+        commands = _generate_commands(
+            tables=tables,
+            table_name_mappings=mappings,
+            original_table_name=table_name,
+            original_primary_key=primary_key,
+        )
+        producer_metadata = ProducerMetadata(
+            invented_root_table_name=mappings[table_name],
+            table_name_mappings=mappings,
+        )
+        return (commands, producer_metadata)
 
 
 def _generate_commands(
-    rel_json: RelationalJson, tables: list[tuple[str, pd.DataFrame]]
+    tables: list[tuple[str, pd.DataFrame]],
+    table_name_mappings: dict[str, str],
+    original_table_name: str,
+    original_primary_key: list[str],
 ) -> CommandsT:
     """
     Returns lists of keyword arguments designed to be passed to a
     RelationalData instance's _add_single_table and add_foreign_key methods
     """
-    tables_to_add = {rel_json.table_name_mappings[name]: df for name, df in tables}
+    root_table_name = table_name_mappings[original_table_name]
 
     _add_single_table = []
     add_foreign_key = []
 
-    for table_name, table_df in tables_to_add.items():
-        if table_name == rel_json.root_table_name:
-            table_pk = rel_json.original_primary_key + [PRIMARY_KEY_COLUMN]
+    for table_breadcrumb_name, table_df in tables:
+        table_name = table_name_mappings[table_breadcrumb_name]
+        if table_name == root_table_name:
+            table_pk = original_primary_key + [PRIMARY_KEY_COLUMN]
         else:
             table_pk = [PRIMARY_KEY_COLUMN]
         table_df.index.rename(PRIMARY_KEY_COLUMN, inplace=True)
         table_df.reset_index(inplace=True)
-        invented_root_table_name = rel_json.table_name_mappings[
-            rel_json.original_table_name
-        ]
         metadata = InventedTableMetadata(
-            invented_root_table_name=invented_root_table_name,
-            original_table_name=rel_json.original_table_name,
+            invented_root_table_name=root_table_name,
+            original_table_name=original_table_name,
+            json_breadcrumb_path=table_breadcrumb_name,
             empty=table_df.empty,
         )
         _add_single_table.append(
             {
                 "name": table_name,
                 "primary_key": table_pk,
                 "data": table_df,
                 "invented_table_metadata": metadata,
             }
         )
 
-    for table_name, table_df in tables_to_add.items():
+    for table_breadcrumb_name, table_df in tables:
+        table_name = table_name_mappings[table_breadcrumb_name]
         for column in get_id_columns(table_df):
-            referred_table = rel_json.table_name_mappings[
+            referred_table = table_name_mappings[
                 get_parent_table_name_from_child_id_column(column)
             ]
             add_foreign_key.append(
                 {
                     "table": table_name,
                     "constrained_columns": [column],
                     "referred_table": referred_table,
                     "referred_columns": [PRIMARY_KEY_COLUMN],
                 }
             )
     return (_add_single_table, add_foreign_key)
 
 
+def restore(
+    tables: dict[str, pd.DataFrame],
+    rel_data: _RelationalData,
+    root_table_name: str,
+    original_columns: list[str],
+    table_name_mappings: dict[str, str],
+    original_table_name: str,
+) -> Optional[pd.DataFrame]:
+    # If the root invented table is not present, we are completely out of luck
+    # (Missing invented child tables can be replaced with empty lists so we at least provide _something_)
+    if root_table_name not in tables:
+        logger.warning(
+            f"Cannot restore nested JSON data: root invented table `{root_table_name}` is missing from output tables."
+        )
+        return None
+
+    return _denormalize_json(
+        tables, rel_data, table_name_mappings, original_table_name
+    )[original_columns]
+
+
+def _denormalize_json(
+    tables: dict[str, pd.DataFrame],
+    rel_data: _RelationalData,
+    table_name_mappings: dict[str, str],
+    original_table_name: str,
+) -> pd.DataFrame:
+    table_names = list(table_name_mappings.values())
+    inverse_table_name_mappings = {v: k for k, v in table_name_mappings.items()}
+    table_dict: dict = {inverse_table_name_mappings[k]: v for k, v in tables.items()}
+    for table_name in list(reversed(table_names)):
+        table_provenance_name = inverse_table_name_mappings[table_name]
+        empty_fallback = pd.DataFrame(
+            data={col: [] for col in rel_data.get_table_columns(table_name)},
+        )
+        table_df = table_dict.get(table_provenance_name, empty_fallback)
+
+        if table_df.empty and _is_invented_child_table(table_name, rel_data):
+            p_name = rel_data.get_foreign_keys(table_name)[0].parent_table_name
+            parent_name = inverse_table_name_mappings[p_name]
+            col_name = get_parent_column_name_from_child_table_name(
+                table_provenance_name
+            )
+            kwargs = {col_name: table_dict[parent_name].apply(lambda x: [], axis=1)}
+            table_dict[parent_name] = table_dict[parent_name].assign(**kwargs)
+        else:
+            col_names = [col for col in table_df.columns if FIELD_SEPARATOR in col]
+            new_col_names = [col.replace(FIELD_SEPARATOR, ".") for col in col_names]
+            flat_df = table_df[col_names].rename(
+                columns=dict(zip(col_names, new_col_names))
+            )
+            flat_dict = {
+                k: {
+                    k1: v1
+                    for k1, v1 in v.items()
+                    if v1 is not np.nan and v1 is not None
+                }
+                for k, v in flat_df.to_dict("index").items()
+            }
+            dict_df = nulls_to_empty_dicts(
+                pd.DataFrame.from_dict(
+                    {k: unflatten(v) for k, v in flat_dict.items()}, orient="index"
+                )
+            )
+            nested_df = table_df.join(dict_df).drop(columns=col_names)
+            if _is_invented_child_table(table_name, rel_data):
+                # we know there is exactly one foreign key on invented child tables...
+                fk = rel_data.get_foreign_keys(table_name)[0]
+                # ...with exactly one column
+                fk_col = fk.columns[0]
+                p_name = fk.parent_table_name
+                parent_name = inverse_table_name_mappings[p_name]
+                nested_df = (
+                    nested_df.sort_values(ORDER_COLUMN)
+                    .groupby(fk_col)[CONTENT_COLUMN]
+                    .agg(list)
+                )
+                col_name = get_parent_column_name_from_child_table_name(
+                    table_provenance_name
+                )
+                table_dict[parent_name] = table_dict[parent_name].join(
+                    nested_df.rename(col_name)
+                )
+                table_dict[parent_name][col_name] = nulls_to_empty_lists(
+                    table_dict[parent_name][col_name]
+                )
+            table_dict[table_provenance_name] = nested_df
+    return table_dict[original_table_name]
+
+
 def get_json_columns(df: pd.DataFrame) -> list[str]:
     """
     Samples non-null values from all columns and returns those that contain
     valid JSON dicts or lists.
 
     Raises an error if *all* columns are lists, as that is not currently supported.
     """
-    column_previews = {
-        col: preview_data
+    object_cols = {
+        col: data
         for col in df.columns
-        if df.dtypes[col] == "object"
-        and len(preview_data := df[col].dropna().head(PREVIEW_ROW_COUNT)) > 0
+        if df.dtypes[col] == "object" and len(data := df[col].dropna()) > 0
     }
 
-    if len(column_previews) == 0:
+    if len(object_cols) == 0:
         return []
 
     list_cols = [
-        col for col, series in column_previews.items() if series.apply(is_list).all()
+        col for col, series in object_cols.items() if series.apply(is_list).all()
     ]
 
     if len(list_cols) == len(df.columns):
         raise ValueError("Cannot accept tables with JSON lists in all columns")
 
     dict_cols = [
-        col for col, series in column_previews.items() if series.apply(is_dict).all()
+        col
+        for col, series in object_cols.items()
+        if col not in list_cols and series.apply(is_dict).all()
     ]
 
     return dict_cols + list_cols
 
 
 CommandsT = tuple[list[dict], list[dict]]
-IngestResponseT = tuple[RelationalJson, CommandsT]
+IngestResponseT = tuple[CommandsT, ProducerMetadata]
```

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/relational/log.py` & `gretel-trainer-0.9.1/src/gretel_trainer/relational/log.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/relational/model_config.py` & `gretel-trainer-0.9.1/src/gretel_trainer/relational/model_config.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/relational/multi_table.py` & `gretel-trainer-0.9.1/src/gretel_trainer/relational/multi_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,17 +39,18 @@
     BackupTransformsTrain,
 )
 from gretel_trainer.relational.core import (
     GretelModelConfig,
     MultiTableException,
     RelationalData,
     Scope,
+    UserFriendlyDataT,
     skip_table,
 )
-from gretel_trainer.relational.json import InventedTableMetadata, RelationalJson
+from gretel_trainer.relational.json import InventedTableMetadata, ProducerMetadata
 from gretel_trainer.relational.log import silent_logs
 from gretel_trainer.relational.model_config import (
     get_model_key,
     ingest,
     make_classify_config,
     make_evaluate_config,
     make_synthetics_config,
@@ -167,44 +168,35 @@
         if not source_archive_path.exists():
             raise MultiTableException(
                 "Cannot restore from backup: source archive is missing."
             )
         with tarfile.open(source_archive_path, "r:gz") as tar:
             tar.extractall(path=self._working_dir)
         for table_name, table_backup in backup.relational_data.tables.items():
-            source_data = pd.read_csv(self._working_dir / f"source_{table_name}.csv")
+            source_data = self._working_dir / f"source_{table_name}.csv"
             invented_table_metadata = None
+            producer_metadata = None
             if (imeta := table_backup.invented_table_metadata) is not None:
-                invented_table_metadata = InventedTableMetadata(
-                    invented_root_table_name=imeta["invented_root_table_name"],
-                    original_table_name=imeta["original_table_name"],
-                    empty=imeta["empty"],
-                )
+                invented_table_metadata = InventedTableMetadata(**imeta)
+            if (pmeta := table_backup.producer_metadata) is not None:
+                producer_metadata = ProducerMetadata(**pmeta)
             self.relational_data._add_single_table(
                 name=table_name,
                 primary_key=table_backup.primary_key,
-                data=source_data,
+                source=source_data,
                 invented_table_metadata=invented_table_metadata,
+                producer_metadata=producer_metadata,
             )
         for fk_backup in backup.relational_data.foreign_keys:
             self.relational_data.add_foreign_key_constraint(
                 table=fk_backup.table,
                 constrained_columns=fk_backup.constrained_columns,
                 referred_table=fk_backup.referred_table,
                 referred_columns=fk_backup.referred_columns,
             )
-        for key, rel_json_backup in backup.relational_data.relational_jsons.items():
-            relational_json = RelationalJson(
-                original_table_name=rel_json_backup.original_table_name,
-                original_primary_key=rel_json_backup.original_primary_key,
-                original_columns=rel_json_backup.original_columns,
-                original_data=None,
-                table_name_mappings=rel_json_backup.table_name_mappings,
-            )
-            self.relational_data.relational_jsons[key] = relational_json
 
         # Debug summary
         debug_summary_id = backup.artifact_collection.gretel_debug_summary
         if debug_summary_id is not None:
             self._extended_sdk.download_file_artifact(
                 self._project,
                 debug_summary_id,
@@ -389,15 +381,15 @@
                 try:
                     self._attach_existing_reports(latest_run_id, table)
                 except FileNotFoundError:
                     logger.info(
                         f"Could not find report data for table `{table}` in run outputs."
                     )
             logger.info(
-                f"All tasks for generation run `{latest_run_id}` finished prior to backup. From here, you can access your synthetic data as Pandas DataFrames via `synthetic_output_tables`, or review them in CSV format along with the relational report in the local working directory."
+                f"All tasks for generation run `{latest_run_id}` finished prior to backup. From here, you can review your synthetic data in CSV format along with the relational report in the local working directory."
             )
             return None
         else:
             # Latest run was still in progress. Download any seeds we may have previously created.
             for table, rh in record_handlers.items():
                 data_source = rh.data_source
                 if data_source is not None:
@@ -424,15 +416,15 @@
         Create a `MultiTable` instance from a backup file.
         """
         logger.info(f"Restoring from backup file `{backup_file}`.")
         with open(backup_file, "r") as b:
             backup = Backup.from_dict(json.load(b))
 
         return MultiTable(
-            relational_data=RelationalData(),
+            relational_data=RelationalData(directory=backup.working_dir),
             strategy=backup.strategy,
             gretel_model=backup.gretel_model,
             refresh_interval=backup.refresh_interval,
             backup=backup,
         )
 
     def _backup(self) -> None:
@@ -546,30 +538,23 @@
             self._project, str(debug_summary_path)
         )
 
     def classify(self, config: GretelModelConfig, all_rows: bool = False) -> None:
         classify_data_sources = {}
         for table in self.relational_data.list_all_tables():
             classify_config = make_classify_config(table, config)
-
-            # Ensure consistent, friendly data source names in Console
-            table_data = self.relational_data.get_table_data(table)
-            classify_data_source_path = str(
-                self._working_dir / f"classify_data_source_{table}.csv"
-            )
-            table_data.to_csv(classify_data_source_path, index=False)
-
-            classify_data_sources[table] = classify_data_source_path
+            data_source = str(self.relational_data.get_table_source(table))
+            classify_data_sources[table] = data_source
 
             # Create model if necessary
             if self._classify.models.get(table) is not None:
                 continue
 
             model = self._project.create_model_obj(
-                model_config=classify_config, data_source=classify_data_source_path
+                model_config=classify_config, data_source=data_source
             )
             self._classify.models[table] = model
 
         self._backup()
 
         task = ClassifyTask(
             classify=self._classify,
@@ -586,26 +571,17 @@
             self._project, str(archive_path)
         )
 
     def _setup_transforms_train_state(
         self, configs: dict[str, GretelModelConfig]
     ) -> None:
         for table, config in configs.items():
-            transform_config = make_transform_config(
-                self.relational_data, table, config
-            )
-
-            # Ensure consistent, friendly data source names in Console
-            table_data = self.relational_data.get_table_data(table)
-            transforms_train_path = self._working_dir / f"transforms_train_{table}.csv"
-            table_data.to_csv(transforms_train_path, index=False)
-
-            # Create model
             model = self._project.create_model_obj(
-                model_config=transform_config, data_source=str(transforms_train_path)
+                model_config=make_transform_config(self.relational_data, table, config),
+                data_source=str(self.relational_data.get_table_source(table)),
             )
             self._transforms_train.models[table] = model
 
         self._backup()
 
     def train_transform_models(self, configs: dict[str, GretelModelConfig]) -> None:
         """
@@ -649,15 +625,15 @@
         )
         run_task(task, self._extended_sdk)
 
     def run_transforms(
         self,
         identifier: Optional[str] = None,
         in_place: bool = False,
-        data: Optional[dict[str, pd.DataFrame]] = None,
+        data: Optional[dict[str, UserFriendlyDataT]] = None,
         encode_keys: bool = False,
     ) -> None:
         """
         Run pre-trained Gretel Transform models on Relational table data:
 
         Args:
             identifier: Unique string identifying a specific call to this method. Defaults to `transforms_` + current timestamp
@@ -682,23 +658,26 @@
                 )
 
         identifier = identifier or f"transforms_{_timestamp()}"
         logger.info(f"Starting transforms run `{identifier}`")
         run_dir = _mkdir(str(self._working_dir / identifier))
         transforms_run_paths = {}
 
-        data = data or {
-            table: self.relational_data.get_table_data(table)
+        data_sources = data or {
+            table: str(self.relational_data.get_table_source(table))
             for table in self._transforms_train.models
             if _table_trained_successfully(self._transforms_train, table)
         }
 
-        for table, df in data.items():
+        for table, data_source in data_sources.items():
             transforms_run_path = run_dir / f"transforms_input_{table}.csv"
-            df.to_csv(transforms_run_path, index=False)
+            if isinstance(data_source, pd.DataFrame):
+                data_source.to_csv(transforms_run_path, index=False)
+            else:
+                shutil.copyfile(data_source, transforms_run_path)
             transforms_run_paths[table] = transforms_run_path
 
         transforms_record_handlers: dict[str, RecordHandler] = {}
 
         for table_name, transforms_run_path in transforms_run_paths.items():
             model = self._transforms_train.models[table_name]
             record_handler = model.create_record_handler_obj(
@@ -911,15 +890,15 @@
         configs = {
             table: table_specific_config_dicts.get(table, default_config_dict)
             for table in include_tables
         }
 
         self._train_synthetics_models(configs)
 
-    def retrain_tables(self, tables: dict[str, pd.DataFrame]) -> None:
+    def retrain_tables(self, tables: dict[str, UserFriendlyDataT]) -> None:
         """
         Provide updated table data and retrain. This method overwrites the table data in the
         `RelationalData` instance. It should be used when initial training fails and source data
         needs to be altered, but progress on other tables can be left as-is.
         """
         for table_name, table_data in tables.items():
             self.relational_data.update_table_data(table_name, table_data)
@@ -939,23 +918,17 @@
 
         self._train_synthetics_models(configs)
 
     def _upload_sources_to_project(self) -> None:
         archive_path = self._working_dir / "source_tables.tar.gz"
         with tarfile.open(archive_path, "w:gz") as tar:
             for table in self.relational_data.list_all_tables(Scope.ALL):
-                filename = f"source_{table}.csv"
-                out_path = self._working_dir / filename
-                df = self.relational_data.get_table_data(table)
-                df.to_csv(
-                    out_path,
-                    index=False,
-                    columns=self.relational_data.get_table_columns(table),
-                )
-                tar.add(out_path, arcname=filename)
+                source_path = Path(self.relational_data.get_table_source(table))
+                filename = source_path.name
+                tar.add(source_path, arcname=f"source_{filename}")
         self._artifact_collection.upload_source_archive(
             self._project, str(archive_path)
         )
         self._backup()
 
     def generate(
         self,
@@ -971,17 +944,14 @@
         joining to parent tables (which may have been synthesized) continues to work properly.
 
         Args:
             record_size_ratio (float, optional): Ratio to upsample real world data size with. Defaults to 1.
             preserve_tables (list[str], optional): List of tables to skip sampling and leave (mostly) identical to source.
             identifier (str, optional): Unique string identifying a specific call to this method. Defaults to `synthetics_` + current timestamp.
             resume (bool, optional): Set to True when restoring from a backup to complete a previous, interrupted run.
-
-        Returns:
-            dict[str, pd.DataFrame]: Return a dictionary of table names and output data.
         """
         if resume:
             if identifier is not None:
                 logger.warning(
                     "Cannot set identifier when resuming previous generation. Ignoring."
                 )
             if record_size_ratio is not None:
@@ -1212,15 +1182,15 @@
         return False
     else:
         return model.status == Status.COMPLETED
 
 
 def _mkdir(name: str) -> Path:
     d = Path(name)
-    os.makedirs(d, exist_ok=True)
+    d.mkdir(parents=True, exist_ok=True)
     return d
 
 
 def _upload_gretel_backup(project: Project, path: str, hybrid: bool) -> None:
     if hybrid:
         return None
     latest = project.upload_artifact(path)
```

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/relational/report/figures.py` & `gretel-trainer-0.9.1/src/gretel_trainer/relational/report/figures.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/relational/report/key_highlight.js` & `gretel-trainer-0.9.1/src/gretel_trainer/relational/report/key_highlight.js`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/relational/report/report.css` & `gretel-trainer-0.9.1/src/gretel_trainer/relational/report/report.css`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/relational/report/report.py` & `gretel-trainer-0.9.1/src/gretel_trainer/relational/report/report.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/relational/report/report_privacy_protection.css` & `gretel-trainer-0.9.1/src/gretel_trainer/relational/report/report_privacy_protection.css`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/relational/report/report_synthetic_quality.css` & `gretel-trainer-0.9.1/src/gretel_trainer/relational/report/report_synthetic_quality.css`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/relational/report/report_template.html` & `gretel-trainer-0.9.1/src/gretel_trainer/relational/report/report_template.html`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/relational/sdk_extras.py` & `gretel-trainer-0.9.1/src/gretel_trainer/relational/sdk_extras.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/relational/strategies/ancestral.py` & `gretel-trainer-0.9.1/src/gretel_trainer/relational/strategies/ancestral.py`

 * *Files 2% similar despite different names*

```diff
@@ -238,35 +238,43 @@
     ) -> pd.DataFrame:
         """
         Replaces primary key values with a new, contiguous set of values.
         Replaces synthesized foreign keys with seed primary keys.
         """
         processed = synthetic_table
 
-        primary_key = rel_data.get_primary_key(table_name)
         multigenerational_primary_key = ancestry.get_multigenerational_primary_key(
             rel_data, table_name
         )
 
         if len(multigenerational_primary_key) == 0:
             pass
         elif len(multigenerational_primary_key) == 1:
             processed[multigenerational_primary_key[0]] = [
                 i for i in range(len(synthetic_table))
             ]
         else:
-            synthetic_pk_columns = common.make_composite_pk_columns(
+            synthetic_pk_columns = common.make_composite_pks(
                 table_name=table_name,
                 rel_data=rel_data,
-                primary_key=primary_key,
+                primary_key=multigenerational_primary_key,
                 synth_row_count=len(synthetic_table),
-                record_size_ratio=record_size_ratio,
             )
-            for index, col in enumerate(multigenerational_primary_key):
-                processed[col] = synthetic_pk_columns[index]
+
+            # make_composite_pks may not have created as many unique keys as we have
+            # synthetic rows, so we truncate the table to avoid inserting NaN PKs.
+            processed = pd.concat(
+                [
+                    pd.DataFrame.from_records(synthetic_pk_columns),
+                    processed.drop(multigenerational_primary_key, axis="columns").head(
+                        len(synthetic_pk_columns)
+                    ),
+                ],
+                axis=1,
+            )
 
         for fk_map in ancestry.get_ancestral_foreign_key_maps(rel_data, table_name):
             fk_col, parent_pk_col = fk_map
             processed[fk_col] = processed[parent_pk_col]
 
         return processed
```

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/relational/strategies/independent.py` & `gretel-trainer-0.9.1/src/gretel_trainer/relational/strategies/independent.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,17 +46,20 @@
             columns_to_drop.update(rel_data.get_primary_key(table))
             for foreign_key in rel_data.get_foreign_keys(table):
                 columns_to_drop.update(foreign_key.columns)
 
             all_columns = rel_data.get_table_columns(table)
             use_columns = [col for col in all_columns if col not in columns_to_drop]
 
-            rel_data.get_table_data(table, usecols=use_columns).to_csv(
-                path, index=False
-            )
+            pd.DataFrame(columns=use_columns).to_csv(path, index=False)
+            source_path = rel_data.get_table_source(table)
+            for chunk in pd.read_csv(
+                source_path, usecols=use_columns, chunksize=10_000
+            ):
+                chunk.to_csv(path, index=False, mode="a", header=False)
 
         return table_paths
 
     def tables_to_retrain(
         self, tables: list[str], rel_data: RelationalData
     ) -> list[str]:
         """
@@ -224,23 +227,30 @@
         synth_row_count = len(synth_data)
 
         if len(primary_key) == 0:
             continue
         elif len(primary_key) == 1:
             processed[table_name][primary_key[0]] = [i for i in range(synth_row_count)]
         else:
-            synthetic_pk_columns = common.make_composite_pk_columns(
+            synthetic_pk_columns = common.make_composite_pks(
                 table_name=table_name,
                 rel_data=rel_data,
                 primary_key=primary_key,
                 synth_row_count=synth_row_count,
-                record_size_ratio=record_size_ratio,
             )
-            for index, col in enumerate(primary_key):
-                processed[table_name][col] = synthetic_pk_columns[index]
+
+            # make_composite_pks may not have created as many unique keys as we have
+            # synthetic rows, so we truncate the table to avoid inserting NaN PKs.
+            processed[table_name] = pd.concat(
+                [
+                    processed[table_name].head(len(synthetic_pk_columns)),
+                    pd.DataFrame.from_records(synthetic_pk_columns),
+                ],
+                axis=1,
+            )
 
     return processed
 
 
 def _synthesize_foreign_keys(
     synth_tables: dict[str, pd.DataFrame], rel_data: RelationalData
 ) -> dict[str, pd.DataFrame]:
```

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/relational/table_evaluation.py` & `gretel-trainer-0.9.1/src/gretel_trainer/relational/table_evaluation.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/relational/task_runner.py` & `gretel-trainer-0.9.1/src/gretel_trainer/relational/task_runner.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/relational/tasks/classify.py` & `gretel-trainer-0.9.1/src/gretel_trainer/relational/tasks/classify.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/relational/tasks/common.py` & `gretel-trainer-0.9.1/src/gretel_trainer/relational/tasks/common.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/relational/tasks/synthetics_evaluate.py` & `gretel-trainer-0.9.1/src/gretel_trainer/relational/tasks/synthetics_evaluate.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/relational/tasks/synthetics_run.py` & `gretel-trainer-0.9.1/src/gretel_trainer/relational/tasks/synthetics_run.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/relational/tasks/synthetics_train.py` & `gretel-trainer-0.9.1/src/gretel_trainer/relational/tasks/synthetics_train.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/relational/tasks/transforms_run.py` & `gretel-trainer-0.9.1/src/gretel_trainer/relational/tasks/transforms_run.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/relational/tasks/transforms_train.py` & `gretel-trainer-0.9.1/src/gretel_trainer/relational/tasks/transforms_train.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/relational/workflow_state.py` & `gretel-trainer-0.9.1/src/gretel_trainer/relational/workflow_state.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/runner.py` & `gretel-trainer-0.9.1/src/gretel_trainer/runner.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/strategy.py` & `gretel-trainer-0.9.1/src/gretel_trainer/strategy.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer/trainer.py` & `gretel-trainer-0.9.1/src/gretel_trainer/trainer.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer.egg-info/PKG-INFO` & `gretel-trainer-0.9.1/src/gretel_trainer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gretel-trainer
-Version: 0.9.0
+Version: 0.9.1
 Summary: Synthetic Data Generation with optional Differential Privacy
 Home-page: https://github.com/gretelai/gretel-trainer
 License: https://gretel.ai/license/source-available-license
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Free To Use But Restricted
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `gretel-trainer-0.9.0/src/gretel_trainer.egg-info/SOURCES.txt` & `gretel-trainer-0.9.1/src/gretel_trainer.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 .gitignore
 .readthedocs.yaml
 LICENSE
 Makefile
 README.md
+pyproject.toml
 requirements-dev.txt
 requirements.txt
 setup.py
 .github/workflows/build.yml
 .github/workflows/python-publish.yml
 data/cpu_states.csv
 data/mitre-synthea-health.csv
```

### Comparing `gretel-trainer-0.9.0/tests/data/core-221-train.csv` & `gretel-trainer-0.9.1/tests/data/core-221-train.csv`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/tests/mocks.py` & `gretel-trainer-0.9.1/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/tests/relational/example_dbs/art.sql` & `gretel-trainer-0.9.1/tests/relational/example_dbs/art.sql`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/tests/relational/example_dbs/documents.sql` & `gretel-trainer-0.9.1/tests/relational/example_dbs/documents.sql`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/tests/relational/example_dbs/ecom.sql` & `gretel-trainer-0.9.1/tests/relational/example_dbs/ecom.sql`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/tests/relational/example_dbs/mutagenesis.sql` & `gretel-trainer-0.9.1/tests/relational/example_dbs/mutagenesis.sql`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/tests/relational/example_dbs/pets.sql` & `gretel-trainer-0.9.1/tests/relational/example_dbs/pets.sql`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/tests/relational/example_dbs/tpch.sql` & `gretel-trainer-0.9.1/tests/relational/example_dbs/tpch.sql`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/tests/relational/test_ancestral_strategy.py` & `gretel-trainer-0.9.1/tests/relational/test_ancestral_strategy.py`

 * *Files 17% similar despite different names*

```diff
@@ -63,33 +63,31 @@
         train_pets = pd.read_csv(training_data["pets"])
 
     for expected_column in ["self|id", "self|name", "self.human_id|id"]:
         assert expected_column in train_pets
 
 
 def test_prepare_training_data_drops_highly_unique_categorical_ancestor_fields(art):
-    art.update_table_data(
-        table="artists",
-        data=pd.DataFrame(
+    with tempfile.NamedTemporaryFile() as artists_csv, tempfile.NamedTemporaryFile() as paintings_csv:
+        pd.DataFrame(
             data={
                 "id": [f"A{i}" for i in range(100)],
-                "name": [str(i) for i in range(100)],
+                "name": [f"artist_name_{i}" for i in range(100)],
             }
-        ),
-    )
-    art.update_table_data(
-        table="paintings",
-        data=pd.DataFrame(
+        ).to_csv(artists_csv.name, index=False)
+        art.update_table_data(table="artists", data=artists_csv.name)
+
+        pd.DataFrame(
             data={
                 "id": [f"P{i}" for i in range(100)],
                 "artist_id": [f"A{i}" for i in range(100)],
-                "name": [str(i) for i in range(100)],
+                "name": [f"painting_name_{i}" for i in range(100)],
             }
-        ),
-    )
+        ).to_csv(paintings_csv.name, index=False)
+        art.update_table_data(table="paintings", data=paintings_csv.name)
 
     strategy = AncestralStrategy()
 
     with tempfile.NamedTemporaryFile() as artists_dest, tempfile.NamedTemporaryFile() as paintings_dest:
         training_data = strategy.prepare_training_data(
             art,
             {
@@ -111,33 +109,32 @@
 def test_prepare_training_data_drops_highly_nan_ancestor_fields(art):
     highly_nan_names = []
     for i in range(100):
         if i > 70:
             highly_nan_names.append(None)
         else:
             highly_nan_names.append("some name")
-    art.update_table_data(
-        table="artists",
-        data=pd.DataFrame(
+
+    with tempfile.NamedTemporaryFile() as artists_csv, tempfile.NamedTemporaryFile() as paintings_csv:
+        pd.DataFrame(
             data={
                 "id": [f"A{i}" for i in range(100)],
                 "name": highly_nan_names,
             }
-        ),
-    )
-    art.update_table_data(
-        table="paintings",
-        data=pd.DataFrame(
+        ).to_csv(artists_csv.name, index=False)
+        art.update_table_data(table="artists", data=artists_csv.name)
+
+        pd.DataFrame(
             data={
                 "id": [f"P{i}" for i in range(100)],
                 "artist_id": [f"A{i}" for i in range(100)],
                 "name": [str(i) for i in range(100)],
             }
-        ),
-    )
+        ).to_csv(paintings_csv.name, index=False)
+        art.update_table_data(table="paintings", data=paintings_csv.name)
 
     strategy = AncestralStrategy()
 
     with tempfile.NamedTemporaryFile() as artists_dest, tempfile.NamedTemporaryFile() as paintings_dest:
         training_data = strategy.prepare_training_data(
             art,
             {
@@ -527,33 +524,87 @@
     pdtest.assert_frame_equal(expected_post_processing, processed_events)
 
 
 def test_post_processing_individual_synthetic_result_composite_keys(tpch):
     strategy = AncestralStrategy()
     synth_lineitem = pd.DataFrame(
         data={
-            "self|l_partkey": [10, 20, 30, 40],
-            "self|l_suppkey": [10, 20, 30, 40],
-            "self|l_quantity": [42, 42, 42, 42],
-            "self.l_partkey+l_suppkey|ps_partkey": [2, 3, 4, 5],
-            "self.l_partkey+l_suppkey|ps_suppkey": [6, 7, 8, 9],
-            "self.l_partkey+l_suppkey|ps_availqty": [80, 80, 80, 80],
-            "self.l_partkey+l_suppkey.ps_partkey|p_partkey": [2, 3, 4, 5],
-            "self.l_partkey+l_suppkey.ps_partkey|p_name": ["a", "b", "c", "d"],
-            "self.l_partkey+l_suppkey.ps_suppkey|s_suppkey": [6, 7, 8, 9],
-            "self.l_partkey+l_suppkey.ps_suppkey|s_name": ["e", "f", "g", "h"],
+            "self|l_partkey": [10, 20, 30, 40] * 3,
+            "self|l_suppkey": [10, 20, 30, 40] * 3,
+            "self|l_quantity": [42, 42, 42, 42] * 3,
+            "self.l_partkey+l_suppkey|ps_partkey": [2, 3, 4, 5] * 3,
+            "self.l_partkey+l_suppkey|ps_suppkey": [6, 7, 8, 9] * 3,
+            "self.l_partkey+l_suppkey|ps_availqty": [80, 80, 80, 80] * 3,
+            "self.l_partkey+l_suppkey.ps_partkey|p_partkey": [2, 3, 4, 5] * 3,
+            "self.l_partkey+l_suppkey.ps_partkey|p_name": ["a", "b", "c", "d"] * 3,
+            "self.l_partkey+l_suppkey.ps_suppkey|s_suppkey": [6, 7, 8, 9] * 3,
+            "self.l_partkey+l_suppkey.ps_suppkey|s_name": ["e", "f", "g", "h"] * 3,
         }
     )
 
     processed_lineitem = strategy.post_process_individual_synthetic_result(
         "lineitem", tpch, synth_lineitem, 1
     )
 
     expected_post_processing = pd.DataFrame(
         data={
+            "self|l_partkey": [2, 3, 4, 5] * 3,
+            "self|l_suppkey": [6, 7, 8, 9] * 3,
+            "self|l_quantity": [42, 42, 42, 42] * 3,
+            "self.l_partkey+l_suppkey|ps_partkey": [2, 3, 4, 5] * 3,
+            "self.l_partkey+l_suppkey|ps_suppkey": [6, 7, 8, 9] * 3,
+            "self.l_partkey+l_suppkey|ps_availqty": [80, 80, 80, 80] * 3,
+            "self.l_partkey+l_suppkey.ps_partkey|p_partkey": [2, 3, 4, 5] * 3,
+            "self.l_partkey+l_suppkey.ps_partkey|p_name": ["a", "b", "c", "d"] * 3,
+            "self.l_partkey+l_suppkey.ps_suppkey|s_suppkey": [6, 7, 8, 9] * 3,
+            "self.l_partkey+l_suppkey.ps_suppkey|s_name": ["e", "f", "g", "h"] * 3,
+        }
+    )
+
+    pdtest.assert_frame_equal(expected_post_processing, processed_lineitem)
+
+
+def test_post_processing_individual_composite_too_few_keys_created(tpch):
+    strategy = AncestralStrategy()
+    synth_lineitem = pd.DataFrame(
+        data={
+            "self|l_partkey": [10, 20, 30, 40] * 3,
+            "self|l_suppkey": [10, 20, 30, 40] * 3,
+            "self|l_quantity": [42, 42, 42, 42] * 3,
+            "self.l_partkey+l_suppkey|ps_partkey": [2, 3, 4, 5] * 3,
+            "self.l_partkey+l_suppkey|ps_suppkey": [6, 7, 8, 9] * 3,
+            "self.l_partkey+l_suppkey|ps_availqty": [80, 80, 80, 80] * 3,
+            "self.l_partkey+l_suppkey.ps_partkey|p_partkey": [2, 3, 4, 5] * 3,
+            "self.l_partkey+l_suppkey.ps_partkey|p_name": ["a", "b", "c", "d"] * 3,
+            "self.l_partkey+l_suppkey.ps_suppkey|s_suppkey": [6, 7, 8, 9] * 3,
+            "self.l_partkey+l_suppkey.ps_suppkey|s_name": ["e", "f", "g", "h"] * 3,
+        }
+    )
+
+    # Given inherent randomness, make_composite_pks can fail to produce enough
+    # unique composite keys to fill the entire synthetic dataframe. In such situations,
+    # the client drops records from the raw record handler output and the resulting
+    # synthetic table only has as many records as keys produced.
+    with patch(
+        "gretel_trainer.relational.strategies.ancestral.common.make_composite_pks"
+    ) as make_keys:
+        make_keys.return_value = [
+            {"self|l_partkey": 55, "self|l_suppkey": 55},
+            {"self|l_partkey": 66, "self|l_suppkey": 66},
+            {"self|l_partkey": 77, "self|l_suppkey": 77},
+            {"self|l_partkey": 88, "self|l_suppkey": 88},
+        ]
+        processed_lineitem = strategy.post_process_individual_synthetic_result(
+            "lineitem", tpch, synth_lineitem, 1
+        )
+
+    # make_composite_pks only created 4 unique keys, so the table is truncated.
+    # The values (2-5 and 6-9) come from the subsequent foreign key step.
+    expected_post_processing = pd.DataFrame(
+        data={
             "self|l_partkey": [2, 3, 4, 5],
             "self|l_suppkey": [6, 7, 8, 9],
             "self|l_quantity": [42, 42, 42, 42],
             "self.l_partkey+l_suppkey|ps_partkey": [2, 3, 4, 5],
             "self.l_partkey+l_suppkey|ps_suppkey": [6, 7, 8, 9],
             "self.l_partkey+l_suppkey|ps_availqty": [80, 80, 80, 80],
             "self.l_partkey+l_suppkey.ps_partkey|p_partkey": [2, 3, 4, 5],
```

### Comparing `gretel-trainer-0.9.0/tests/relational/test_ancestry.py` & `gretel-trainer-0.9.1/tests/relational/test_ancestry.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         "self.l_partkey+l_suppkey.ps_suppkey|s_name",
     }
     restored_lineitem = ancestry.drop_ancestral_data(lineitem_with_ancestors)
     assert set(restored_lineitem.columns) == {"l_partkey", "l_suppkey", "l_quantity"}
 
 
 def test_ancestral_data_from_different_tablesets(source_nba, synthetic_nba):
-    source_nba, _, _, _ = source_nba
+    source_nba = source_nba[0]
     _, custom_states, custom_cities, custom_teams = synthetic_nba
 
     # By default, get data from source
     source_teams_with_ancestors = ancestry.get_table_data_with_ancestors(
         source_nba, "teams"
     )
     assert set(source_teams_with_ancestors["self|name"]) == {"Lakers", "Grizzlies"}
```

### Comparing `gretel-trainer-0.9.0/tests/relational/test_artifacts.py` & `gretel-trainer-0.9.1/tests/relational/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/tests/relational/test_backup.py` & `gretel-trainer-0.9.1/tests/relational/test_backup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from gretel_trainer.relational.backup import (
     Backup,
     BackupClassify,
     BackupForeignKey,
     BackupGenerate,
     BackupRelationalData,
     BackupRelationalDataTable,
-    BackupRelationalJson,
     BackupSyntheticsTrain,
     BackupTransformsTrain,
 )
+from tests.relational.conftest import get_invented_table_suffix
 
 
 def test_backup_relational_data(trips):
     expected = BackupRelationalData(
         tables={
             "vehicle_types": BackupRelationalDataTable(
                 primary_key=["id"],
@@ -28,73 +28,76 @@
             BackupForeignKey(
                 table="trips",
                 constrained_columns=["vehicle_type_id"],
                 referred_table="vehicle_types",
                 referred_columns=["id"],
             )
         ],
-        relational_jsons={},
     )
 
     assert BackupRelationalData.from_relational_data(trips) == expected
 
 
 def test_backup_relational_data_with_json(documents):
+    purchases_root_invented_table = f"purchases_{get_invented_table_suffix(1)}"
+    purchases_data_years_invented_table = f"purchases_{get_invented_table_suffix(2)}"
+
     expected = BackupRelationalData(
         tables={
             "users": BackupRelationalDataTable(primary_key=["id"]),
-            "purchases-sfx": BackupRelationalDataTable(
+            "purchases": BackupRelationalDataTable(
+                primary_key=["id"],
+                producer_metadata={
+                    "invented_root_table_name": purchases_root_invented_table,
+                    "table_name_mappings": {
+                        "purchases": purchases_root_invented_table,
+                        "purchases^data>years": purchases_data_years_invented_table,
+                    },
+                },
+            ),
+            purchases_root_invented_table: BackupRelationalDataTable(
                 primary_key=["id", "~PRIMARY_KEY_ID~"],
                 invented_table_metadata={
-                    "invented_root_table_name": "purchases-sfx",
+                    "invented_root_table_name": purchases_root_invented_table,
                     "original_table_name": "purchases",
+                    "json_breadcrumb_path": "purchases",
                     "empty": False,
                 },
             ),
-            "purchases-data-years-sfx": BackupRelationalDataTable(
+            purchases_data_years_invented_table: BackupRelationalDataTable(
                 primary_key=["~PRIMARY_KEY_ID~"],
                 invented_table_metadata={
-                    "invented_root_table_name": "purchases-sfx",
+                    "invented_root_table_name": purchases_root_invented_table,
                     "original_table_name": "purchases",
+                    "json_breadcrumb_path": "purchases^data>years",
                     "empty": False,
                 },
             ),
             "payments": BackupRelationalDataTable(primary_key=["id"]),
         },
         foreign_keys=[
             BackupForeignKey(
                 table="payments",
                 constrained_columns=["purchase_id"],
-                referred_table="purchases-sfx",
+                referred_table=purchases_root_invented_table,
                 referred_columns=["id"],
             ),
             BackupForeignKey(
-                table="purchases-sfx",
+                table=purchases_root_invented_table,
                 constrained_columns=["user_id"],
                 referred_table="users",
                 referred_columns=["id"],
             ),
             BackupForeignKey(
-                table="purchases-data-years-sfx",
+                table=purchases_data_years_invented_table,
                 constrained_columns=["purchases~id"],
-                referred_table="purchases-sfx",
+                referred_table=purchases_root_invented_table,
                 referred_columns=["~PRIMARY_KEY_ID~"],
             ),
         ],
-        relational_jsons={
-            "purchases": BackupRelationalJson(
-                original_table_name="purchases",
-                original_primary_key=["id"],
-                original_columns=["id", "user_id", "data"],
-                table_name_mappings={
-                    "purchases": "purchases-sfx",
-                    "purchases^data>years": "purchases-data-years-sfx",
-                },
-            ),
-        },
     )
 
     assert BackupRelationalData.from_relational_data(documents) == expected
 
 
 def test_backup():
     backup_relational = BackupRelationalData(
@@ -110,15 +113,14 @@
             BackupForeignKey(
                 table="address",
                 constrained_columns=["customer_id"],
                 referred_table="customer",
                 referred_columns=["id"],
             )
         ],
-        relational_jsons={},
     )
     backup_classify = BackupClassify(
         model_ids={
             "customer": "aaabbbccc",
             "address": "dddeeefff",
         },
     )
```

### Comparing `gretel-trainer-0.9.0/tests/relational/test_common_strategy.py` & `gretel-trainer-0.9.1/tests/relational/test_common_strategy.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,86 +1,84 @@
 import pandas as pd
 
 import gretel_trainer.relational.strategies.common as common
 from gretel_trainer.relational.core import RelationalData
 
 
-def test_composite_pk_columns():
-    table = pd.DataFrame(
+def test_composite_pk_columns(tmpdir):
+    df = pd.DataFrame(
         data={
             "letter": ["a", "a", "a", "a", "b", "b", "b", "b"],
             "number": [1, 2, 3, 4, 1, 2, 3, 4],
         }
     )
-    rel_data = RelationalData()
+    rel_data = RelationalData(directory=tmpdir)
     rel_data.add_table(
         name="table",
         primary_key=["letter", "number"],
-        data=table,
+        data=df,
     )
 
-    result = common.make_composite_pk_columns(
+    result = common.make_composite_pks(
         table_name="table",
         rel_data=rel_data,
         primary_key=["letter", "number"],
         synth_row_count=8,
-        record_size_ratio=1.0,
     )
 
-    # There is a tuple of values for each primary key column
-    assert len(result) == 2
+    # Label-encoding turns the keys into zero-indexed contiguous integers.
+    # It is absolutely required that all composite keys returned are unique.
+    # We also ideally recreate the original data frequencies (in this case,
+    # two unique letters and four unique numbers).
+    expected_keys = [
+        {"letter": 0, "number": 0},
+        {"letter": 0, "number": 1},
+        {"letter": 0, "number": 2},
+        {"letter": 0, "number": 3},
+        {"letter": 1, "number": 0},
+        {"letter": 1, "number": 1},
+        {"letter": 1, "number": 2},
+        {"letter": 1, "number": 3},
+    ]
 
-    # Each tuple has enough values for the synthetic result
-    for t in result:
-        assert len(t) == 8
+    for expected_key in expected_keys:
+        assert expected_key in result
 
-    # Each combination is unique
-    synthetic_pks = set(zip(*result))
-    assert len(synthetic_pks) == 8
-
-    # The set of unique values in each synthetic column roughly matches
-    # the set of unique values in the source columns.
-    # In this example they match exactly because there are no other possible combinations,
-    # but in practice it's possible to randomly not-select some values.
-    assert len(set(result[0])) == 2
-    assert len(set(result[1])) == 4
 
-
-def test_composite_pk_columns_2():
-    table = pd.DataFrame(
+def test_composite_pk_columns_2(tmpdir):
+    df = pd.DataFrame(
         data={
             "letter": ["a", "a", "a", "a", "b", "b", "b", "b"],
             "number": [1, 2, 3, 4, 5, 6, 7, 8],
         }
     )
-    rel_data = RelationalData()
+    rel_data = RelationalData(directory=tmpdir)
     rel_data.add_table(
         name="table",
         primary_key=["letter", "number"],
-        data=table,
+        data=df,
     )
 
-    result = common.make_composite_pk_columns(
+    result = common.make_composite_pks(
         table_name="table",
         rel_data=rel_data,
         primary_key=["letter", "number"],
         synth_row_count=8,
-        record_size_ratio=1.0,
     )
 
-    # There is a tuple of values for each primary key column
-    assert len(result) == 2
-
-    # Each tuple has enough values for the synthetic result
-    for t in result:
-        assert len(t) == 8
+    # We create as many keys as we need
+    assert len(result) == 8
 
     # Each combination is unique
-    synthetic_pks = set(zip(*result))
-    assert len(synthetic_pks) == 8
+    assert len(set([str(composite_key) for composite_key in result])) == 8
 
-    # The set of unique values in each synthetic column roughly matches
-    # the set of unique values in the source columns.
-    # In this example, there are more potential combinations than there are synthetic rows,
-    # so our assertions are not as strict.
-    assert len(set(result[0])) <= 2
-    assert len(set(result[1])) <= 8
+    # In this case, there are more potential unique combinations than there are synthetic rows,
+    # so we can't say for sure what the exact composite values will be. However, we do expect
+    # the original frequencies to be maintained.
+    synthetic_letters = [key["letter"] for key in result]
+    assert len(synthetic_letters) == 8
+    assert set(synthetic_letters) == {0, 1}
+    assert len([x for x in synthetic_letters if x != 0]) == 4
+
+    synthetic_numbers = [key["number"] for key in result]
+    assert len(synthetic_numbers) == 8
+    assert set(synthetic_numbers) == {0, 1, 2, 3, 4, 5, 6, 7}
```

### Comparing `gretel-trainer-0.9.0/tests/relational/test_connectors.py` & `gretel-trainer-0.9.1/tests/relational/test_connectors.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,29 +3,32 @@
 
 import pytest
 
 from gretel_trainer.relational.connectors import sqlite_conn
 from gretel_trainer.relational.core import MultiTableException, Scope
 
 
-def test_extract_subsets_of_relational_data(example_dbs):
+def test_extract_subsets_of_relational_data(example_dbs, tmpdir):
     with tempfile.NamedTemporaryFile() as f:
         con = sqlite3.connect(f.name)
         cur = con.cursor()
         with open(example_dbs / "ecom.sql") as sql_script:
             cur.executescript(sql_script.read())
 
         connector = sqlite_conn(f.name)
 
         with pytest.raises(MultiTableException):
-            connector.extract(only={"users"}, ignore={"events"})
+            connector.extract(only={"users"}, ignore={"events"}, storage_dir=tmpdir)
 
-        only = connector.extract(only={"users", "events", "products"})
+        only = connector.extract(
+            only={"users", "events", "products"}, storage_dir=tmpdir
+        )
         ignore = connector.extract(
-            ignore={"distribution_center", "order_items", "inventory_items"}
+            ignore={"distribution_center", "order_items", "inventory_items"},
+            storage_dir=tmpdir,
         )
 
     expected_tables = {"users", "events", "products"}
     assert set(only.list_all_tables(Scope.ALL)) == expected_tables
     assert set(ignore.list_all_tables(Scope.ALL)) == expected_tables
 
     # `products` has a foreign key to `distribution_center` in the source, but because the
```

### Comparing `gretel-trainer-0.9.0/tests/relational/test_extractor.py` & `gretel-trainer-0.9.1/tests/relational/test_extractor.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/tests/relational/test_independent_strategy.py` & `gretel-trainer-0.9.1/tests/relational/test_independent_strategy.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/tests/relational/test_model_config.py` & `gretel-trainer-0.9.1/tests/relational/test_model_config.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/tests/relational/test_multi_table_config_options.py` & `gretel-trainer-0.9.1/tests/relational/test_multi_table_config_options.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/tests/relational/test_multi_table_restore.py` & `gretel-trainer-0.9.1/tests/relational/test_multi_table_restore.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/tests/relational/test_relational_data.py` & `gretel-trainer-0.9.1/tests/relational/test_relational_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pandas as pd
 import pytest
 
-from gretel_trainer.relational.core import MultiTableException, RelationalData
+from gretel_trainer.relational.core import MultiTableException
 
 
 def test_ecommerce_relational_data(ecom):
     assert ecom.get_parents("users") == []
     assert ecom.get_parents("events") == ["users"]
     assert set(ecom.get_parents("inventory_items")) == {
         "products",
@@ -39,34 +39,36 @@
     assert mutagenesis.get_primary_key("bond") == ["atom1_id", "atom2_id"]
     assert mutagenesis.get_primary_key("atom") == ["atom_id"]
 
     assert set(mutagenesis.get_all_key_columns("bond")) == {"atom1_id", "atom2_id"}
     assert set(mutagenesis.get_all_key_columns("atom")) == {"atom_id", "molecule_id"}
 
 
-def test_column_metadata(pets):
+def test_column_metadata(pets, tmpfile):
     assert pets.get_table_columns("humans") == ["id", "name", "city"]
 
     # Name is a highly unique categorical field, so is excluded
     assert pets.get_safe_ancestral_seed_columns("humans") == {"id", "city"}
 
     # Update the table data such that:
-    # - id is highly unique categorical, but still the PK
+    # - id is highly unique categorical (_ to force string instead of int), but still the PK
     # - name is no longer highly unique
     # - city is highly NaN
+    pd.DataFrame(
+        data={
+            "id": ["1_", "2_", "3_"],
+            "name": ["n", "n", "n"],
+            "city": [None, None, "Chicago"],
+        }
+    ).to_csv(tmpfile.name, index=False)
     pets.update_table_data(
         "humans",
-        pd.DataFrame(
-            data={
-                "id": ["1", "2", "3"],
-                "name": ["n", "n", "n"],
-                "city": [None, None, "Chicago"],
-            }
-        ),
+        tmpfile.name,
     )
+
     assert pets.get_safe_ancestral_seed_columns("humans") == {"id", "name"}
 
     # Resetting the primary key refreshes the cache state
     # In this case, since id is no longer the PK and is highly unique, it is excluded
     pets.set_primary_key(table="humans", primary_key=None)
     assert pets.get_safe_ancestral_seed_columns("humans") == {"name"}
 
@@ -83,103 +85,85 @@
     assert pets.get_safe_ancestral_seed_columns("humans") == {"id", "name", "city"}
 
     # Removing a foreign key refreshes the cache state
     pets.remove_foreign_key_constraint("humans", ["city"])
     assert pets.get_safe_ancestral_seed_columns("humans") == {"id", "name"}
 
 
-def test_adding_and_removing_foreign_keys():
-    rel_data = RelationalData()
-    rel_data.add_table(
-        name="users", primary_key="id", data=pd.DataFrame(data={"id": [1, 2, 3]})
-    )
-    rel_data.add_table(
-        name="events",
-        primary_key="id",
-        data=pd.DataFrame(data={"id": [1, 2, 3], "user_id": [1, 2, 3]}),
+def test_adding_and_removing_foreign_keys(pets):
+    # pets has a foreign key defined out of the box.
+    # First lets successfully remove it and re-add it.
+    assert len(pets.get_foreign_keys("pets")) == 1
+
+    pets.remove_foreign_key_constraint(table="pets", constrained_columns=["human_id"])
+    assert len(pets.get_foreign_keys("pets")) == 0
+
+    pets.add_foreign_key_constraint(
+        table="pets",
+        constrained_columns=["human_id"],
+        referred_table="humans",
+        referred_columns=["id"],
     )
+    assert len(pets.get_foreign_keys("pets")) == 1
+
+    # Now we'll make some assertions about our defense
 
     # Cannot add to an unrecognized table
     with pytest.raises(MultiTableException):
-        rel_data.add_foreign_key_constraint(
+        pets.add_foreign_key_constraint(
             table="unrecognized",
             constrained_columns=["user_id"],
-            referred_table="users",
+            referred_table="humans",
             referred_columns=["id"],
         )
 
     # Cannot add to an unrecognized referred table
     with pytest.raises(MultiTableException):
-        rel_data.add_foreign_key_constraint(
-            table="events",
-            constrained_columns=["user_id"],
+        pets.add_foreign_key_constraint(
+            table="pets",
+            constrained_columns=["human_id"],
             referred_table="unrecognized",
             referred_columns=["id"],
         )
 
     # Cannot add unrecognized columns
     with pytest.raises(MultiTableException):
-        rel_data.add_foreign_key_constraint(
-            table="events",
-            constrained_columns=["user_id"],
-            referred_table="users",
+        pets.add_foreign_key_constraint(
+            table="pets",
+            constrained_columns=["human_id"],
+            referred_table="humans",
             referred_columns=["unrecognized"],
         )
     with pytest.raises(MultiTableException):
-        rel_data.add_foreign_key_constraint(
-            table="events",
+        pets.add_foreign_key_constraint(
+            table="pets",
             constrained_columns=["unrecognized"],
-            referred_table="users",
+            referred_table="humans",
             referred_columns=["id"],
         )
 
-    # Successful add
-    rel_data.add_foreign_key_constraint(
-        table="events",
-        constrained_columns=["user_id"],
-        referred_table="users",
-        referred_columns=["id"],
-    )
-    assert len(rel_data.get_foreign_keys("events")) == 1
-
     # Cannot remove from unrecognized table
     with pytest.raises(MultiTableException):
-        rel_data.remove_foreign_key_constraint(
+        pets.remove_foreign_key_constraint(
             table="unrecognized", constrained_columns=["id"]
         )
 
     # Cannot remove a non-existent key
     with pytest.raises(MultiTableException):
-        rel_data.remove_foreign_key_constraint(
-            table="events", constrained_columns=["id"]
-        )
-
-    # Successful remove
-    rel_data.remove_foreign_key_constraint(
-        table="events", constrained_columns=["user_id"]
-    )
-    assert len(rel_data.get_foreign_keys("events")) == 0
+        pets.remove_foreign_key_constraint(table="pets", constrained_columns=["id"])
 
 
-def test_add_remove_foreign_key_shorthand():
-    rel_data = RelationalData()
-    rel_data.add_table(
-        name="users", primary_key="id", data=pd.DataFrame(data={"id": [1, 2, 3]})
-    )
-    rel_data.add_table(
-        name="events",
-        primary_key="id",
-        data=pd.DataFrame(data={"id": [1, 2, 3], "user_id": [1, 2, 3]}),
-    )
+def test_add_remove_foreign_key_shorthand(pets):
+    assert len(pets.get_foreign_keys("pets")) == 1
 
-    rel_data.add_foreign_key(foreign_key="events.user_id", referencing="users.id")
-    assert len(rel_data.get_foreign_keys("events")) == 1
+    pets.remove_foreign_key("pets.human_id")
+    assert len(pets.get_foreign_keys("pets")) == 0
 
-    rel_data.remove_foreign_key("events.user_id")
-    assert len(rel_data.get_foreign_keys("events")) == 0
+    pets.add_foreign_key(foreign_key="pets.human_id", referencing="humans.id")
+    assert len(pets.get_foreign_keys("pets")) == 1
 
 
 def test_set_primary_key(ecom):
     assert ecom.get_primary_key("users") == ["id"]
 
     ecom.set_primary_key(table="users", primary_key=None)
     assert ecom.get_primary_key("users") == []
```

### Comparing `gretel-trainer-0.9.0/tests/relational/test_relational_data_with_json.py` & `gretel-trainer-0.9.1/tests/relational/test_relational_data_with_json.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,75 +1,99 @@
+import itertools
+import re
+import tempfile
+
 import pandas as pd
 import pandas.testing as pdtest
 import pytest
 
 from gretel_trainer.relational.core import ForeignKey, RelationalData, Scope
-from gretel_trainer.relational.json import get_json_columns
+from gretel_trainer.relational.json import generate_unique_table_name, get_json_columns
+from tests.relational.conftest import get_invented_table_suffix
+
+purchases_root_invented_table = f"purchases_{get_invented_table_suffix(1)}"
+purchases_data_years_invented_table = f"purchases_{get_invented_table_suffix(2)}"
+bball_root_invented_table = f"bball_{get_invented_table_suffix(1)}"
+bball_suspensions_invented_table = f"bball_{get_invented_table_suffix(2)}"
+bball_teams_invented_table = f"bball_{get_invented_table_suffix(3)}"
 
 
 @pytest.fixture
-def bball():
+def bball(tmpdir):
     bball_jsonl = """
     {"name": "LeBron James", "age": 38, "draft": {"year": 2003}, "teams": ["Cavaliers", "Heat", "Lakers"], "suspensions": []}
     {"name": "Steph Curry", "age": 35, "draft": {"year": 2009, "college": "Davidson"}, "teams": ["Warriors"], "suspensions": []}
     """
     bball_df = pd.read_json(bball_jsonl, lines=True)
 
-    rel_data = RelationalData()
+    rel_data = RelationalData(directory=tmpdir)
     rel_data.add_table(name="bball", primary_key=None, data=bball_df)
 
     return rel_data
 
 
+@pytest.fixture
+def deeply_nested(tmpdir):
+    jsonl = """
+    {"hello1":"world1","level1_long_property_name":[{"hello2":"world2","level2_long_property_name":[{"hello3":"world3","level3_long_property_name":[{"hello4":"world4","level4_long_property_name":[{"hello5":"world5","level5_long_property_name":[{"hello6":"world6","level6_long_property_name":[{"hello7":"world7","level7_long_property_name":[{"hello8":"world8","level8_long_property_name":[{"hello9":"world9"}]}]}]}]}]}]}]}]}
+    """
+    df = pd.read_json(jsonl, lines=True)
+
+    rel_data = RelationalData(directory=tmpdir)
+    rel_data.add_table(name="deeply_nested", primary_key=None, data=df)
+
+    return rel_data
+
+
 def test_list_json_cols(documents, bball):
     assert get_json_columns(documents.get_table_data("users")) == []
     assert get_json_columns(documents.get_table_data("purchases")) == ["data"]
 
     assert set(get_json_columns(bball.get_table_data("bball"))) == {
         "draft",
         "teams",
         "suspensions",
     }
 
 
 def test_json_columns_produce_invented_flattened_tables(documents):
     pdtest.assert_frame_equal(
-        documents.get_table_data("purchases-sfx"),
+        documents.get_table_data(purchases_root_invented_table),
         pd.DataFrame(
             data={
                 "~PRIMARY_KEY_ID~": [0, 1, 2, 3, 4, 5],
                 "id": [1, 2, 3, 4, 5, 6],
                 "user_id": [1, 2, 2, 3, 3, 3],
                 "data>item": ["pen", "paint", "ink", "pen", "paint", "ink"],
                 "data>cost": [100, 100, 100, 100, 100, 100],
                 "data>details>color": ["red", "red", "red", "blue", "blue", "blue"],
             }
         ),
         check_like=True,
     )
 
     pdtest.assert_frame_equal(
-        documents.get_table_data("purchases-data-years-sfx"),
+        documents.get_table_data(purchases_data_years_invented_table),
         pd.DataFrame(
             data={
                 "content": [2023, 2023, 2022, 2020, 2019, 2021],
                 "array~order": [0, 0, 1, 0, 1, 0],
                 "~PRIMARY_KEY_ID~": [0, 1, 2, 3, 4, 5],
                 "purchases~id": [0, 1, 1, 2, 2, 4],
             }
         ),
         check_like=True,
         check_dtype=False,  # Without this, test fails asserting dtype mismatch in `content` field (object vs. int)
     )
 
-    assert documents.get_foreign_keys("purchases-data-years-sfx") == [
+    assert documents.get_foreign_keys(purchases_data_years_invented_table) == [
         ForeignKey(
-            table_name="purchases-data-years-sfx",
+            table_name=purchases_data_years_invented_table,
             columns=["purchases~id"],
-            parent_table_name="purchases-sfx",
+            parent_table_name=purchases_root_invented_table,
             parent_columns=["~PRIMARY_KEY_ID~"],
         )
     ]
 
 
 def test_list_tables_accepts_various_scopes(documents):
     # PUBLIC reflects the user's source
@@ -79,186 +103,225 @@
         "payments",
     }
 
     # MODELABLE replaces any source tables containing JSON with the invented tables
     assert set(documents.list_all_tables(Scope.MODELABLE)) == {
         "users",
         "payments",
-        "purchases-sfx",
-        "purchases-data-years-sfx",
+        purchases_root_invented_table,
+        purchases_data_years_invented_table,
     }
 
     # EVALUATABLE is similar to MODELABLE, but omits invented child tables—we only evaluate the root invented table
     assert set(documents.list_all_tables(Scope.EVALUATABLE)) == {
         "users",
         "payments",
-        "purchases-sfx",
+        purchases_root_invented_table,
     }
 
     # INVENTED returns only tables invented from source tables with JSON
     assert set(documents.list_all_tables(Scope.INVENTED)) == {
-        "purchases-sfx",
-        "purchases-data-years-sfx",
+        purchases_root_invented_table,
+        purchases_data_years_invented_table,
     }
 
     # ALL returns every table name, including both source-with-JSON tables and those invented from such tables
     assert set(documents.list_all_tables(Scope.ALL)) == {
         "users",
         "purchases",
         "payments",
-        "purchases-sfx",
-        "purchases-data-years-sfx",
+        purchases_root_invented_table,
+        purchases_data_years_invented_table,
     }
 
     # Default scope is MODELABLE
     assert set(documents.list_all_tables()) == set(
         documents.list_all_tables(Scope.MODELABLE)
     )
 
 
 def test_get_modelable_table_names(documents):
     # Given a source-with-JSON name, returns the tables invented from that source
     assert set(documents.get_modelable_table_names("purchases")) == {
-        "purchases-sfx",
-        "purchases-data-years-sfx",
+        purchases_root_invented_table,
+        purchases_data_years_invented_table,
     }
 
     # Invented tables are modelable
-    assert documents.get_modelable_table_names("purchases-sfx") == ["purchases-sfx"]
-    assert documents.get_modelable_table_names("purchases-data-years-sfx") == [
-        "purchases-data-years-sfx"
+    assert documents.get_modelable_table_names(purchases_root_invented_table) == [
+        purchases_root_invented_table
+    ]
+    assert documents.get_modelable_table_names(purchases_data_years_invented_table) == [
+        purchases_data_years_invented_table
     ]
 
     # Unknown tables return empty list
     assert documents.get_modelable_table_names("nonsense") == []
 
 
 def test_get_modelable_names_ignores_empty_mapped_tables(bball):
     # The `suspensions` column in the source data contained empty lists for all records.
-    # We need to hold onto that table name on the RelationalJson instance to support
-    # denormalizing back to the original source data shape. It is therefore exposed
-    # in the `table_names` attribute on RelationalJson...
-    assert set(bball.relational_jsons["bball"].table_names) == {
-        "bball-sfx",
-        "bball-teams-sfx",
-        "bball-suspensions-sfx",
+    # The normalization process transforms that into a standalone, empty table.
+    # We need to hold onto that table name to support denormalizing back to the original
+    # source data shape. It is therefore present when listing ALL tables...
+    assert set(bball.list_all_tables(Scope.ALL)) == {
+        "bball",
+        bball_root_invented_table,
+        bball_suspensions_invented_table,
+        bball_teams_invented_table,
+    }
+
+    # ...and the producer metadata is aware of it...
+    assert set(bball.get_producer_metadata("bball").table_names) == {
+        bball_root_invented_table,
+        bball_suspensions_invented_table,
+        bball_teams_invented_table,
     }
 
-    # ...BUT clients of RelationalData only care about invented tables that can be modeled
-    # (i.e. that contain data), so that class does not expose the empty table.
+    # ...BUT most clients only care about invented tables that can be modeled
+    # (i.e. that contain data), so the empty table does not appear in these contexts:
     assert set(bball.get_modelable_table_names("bball")) == {
-        "bball-sfx",
-        "bball-teams-sfx",
+        bball_root_invented_table,
+        bball_teams_invented_table,
+    }
+    assert set(bball.list_all_tables()) == {
+        bball_root_invented_table,
+        bball_teams_invented_table,
     }
-    assert set(bball.list_all_tables()) == {"bball-sfx", "bball-teams-sfx"}
 
 
-def test_invented_json_column_names(documents, bball):
+def test_invented_json_column_names_documents(documents):
     # The root invented table adds columns for dictionary properties lifted from nested JSON objects
-    assert documents.get_table_columns("purchases-sfx") == [
+    assert documents.get_table_columns(purchases_root_invented_table) == [
         "~PRIMARY_KEY_ID~",
         "id",
         "user_id",
         "data>item",
         "data>cost",
         "data>details>color",
     ]
 
     # JSON lists lead to invented child tables. These tables store the original content,
     # a new primary key, a foreign key back to the parent, and the original array index
-    assert documents.get_table_columns("purchases-data-years-sfx") == [
+    assert documents.get_table_columns(purchases_data_years_invented_table) == [
         "~PRIMARY_KEY_ID~",
         "purchases~id",
         "content",
         "array~order",
     ]
 
+
+def test_invented_json_column_names_bball(bball):
     # If the source table does not have a primary key defined, one is created on the root invented table
-    assert bball.get_table_columns("bball-sfx") == [
+    assert bball.get_table_columns(bball_root_invented_table) == [
         "~PRIMARY_KEY_ID~",
         "name",
         "age",
         "draft>year",
         "draft>college",
     ]
 
 
-def test_primary_key(documents, bball):
-    # The root invented table's primary key is a composite key that includes the source PK and an invented column
+def test_set_some_primary_key_to_none(static_suffix, documents):
+    # The producer table has a single column primary key,
+    # so the root invented table has a composite key that includes the source PK and an invented column
     assert documents.get_primary_key("purchases") == ["id"]
-    assert documents.get_primary_key("purchases-sfx") == ["id", "~PRIMARY_KEY_ID~"]
-
-    assert bball.get_primary_key("bball") == []
-    assert bball.get_primary_key("bball-sfx") == ["~PRIMARY_KEY_ID~"]
+    assert documents.get_primary_key(purchases_root_invented_table) == [
+        "id",
+        "~PRIMARY_KEY_ID~",
+    ]
 
     # Setting an existing primary key to None puts us in the correct state
     assert len(documents.list_all_tables(Scope.ALL)) == 5
     original_payments_fks = documents.get_foreign_keys("payments")
+
+    # Reset the make_suffix iterator back to original count since set_primary_key will call it again
+    # once for each invented table.
+    static_suffix.side_effect = itertools.count(start=1)
+
+    # Setting the primary key causes json invented tables to be dropped and reingested
     documents.set_primary_key(table="purchases", primary_key=None)
     assert len(documents.list_all_tables(Scope.ALL)) == 5
     assert documents.get_primary_key("purchases") == []
-    assert documents.get_primary_key("purchases-sfx") == ["~PRIMARY_KEY_ID~"]
-    assert documents.get_foreign_keys("purchases-data-years-sfx") == [
+    assert documents.get_primary_key(purchases_root_invented_table) == [
+        "~PRIMARY_KEY_ID~"
+    ]
+    assert documents.get_foreign_keys(purchases_data_years_invented_table) == [
         ForeignKey(
-            table_name="purchases-data-years-sfx",
+            table_name=purchases_data_years_invented_table,
             columns=["purchases~id"],
-            parent_table_name="purchases-sfx",
+            parent_table_name=purchases_root_invented_table,
             parent_columns=["~PRIMARY_KEY_ID~"],
         )
     ]
     assert documents.get_foreign_keys("payments") == original_payments_fks
 
+
+def test_set_none_primary_key_to_some_value(static_suffix, bball):
+    # The producer table has no primary key,
+    # so the root invented table has a single invented key column
+    assert bball.get_primary_key("bball") == []
+    assert bball.get_primary_key(bball_root_invented_table) == ["~PRIMARY_KEY_ID~"]
+
     # Setting a None primary key to some column puts us in the correct state
     assert len(bball.list_all_tables(Scope.ALL)) == 4
+
+    # Reset the make_suffix iterator back to original count since set_primary_key will call it again
+    # once for each invented table.
+    static_suffix.side_effect = itertools.count(start=1)
+
     bball.set_primary_key(table="bball", primary_key="name")
     assert len(bball.list_all_tables(Scope.ALL)) == 4
     assert bball.get_primary_key("bball") == ["name"]
-    assert bball.get_primary_key("bball-sfx") == ["name", "~PRIMARY_KEY_ID~"]
-    assert bball.get_foreign_keys("bball-teams-sfx") == [
+    assert bball.get_primary_key(bball_root_invented_table) == [
+        "name",
+        "~PRIMARY_KEY_ID~",
+    ]
+    assert bball.get_foreign_keys(bball_suspensions_invented_table) == [
         ForeignKey(
-            table_name="bball-teams-sfx",
+            table_name=bball_suspensions_invented_table,
             columns=["bball~id"],
-            parent_table_name="bball-sfx",
+            parent_table_name=bball_root_invented_table,
             parent_columns=["~PRIMARY_KEY_ID~"],
         )
     ]
 
 
 def test_foreign_keys(documents):
     # Foreign keys from the source-with-JSON table are present on the root invented table
     assert documents.get_foreign_keys("purchases") == documents.get_foreign_keys(
-        "purchases-sfx"
+        purchases_root_invented_table
     )
 
     # The root invented table name is used in the ForeignKey
     assert documents.get_foreign_keys("purchases") == [
         ForeignKey(
-            table_name="purchases-sfx",
+            table_name=purchases_root_invented_table,
             columns=["user_id"],
             parent_table_name="users",
             parent_columns=["id"],
         )
     ]
 
     # Invented children point to invented parents
-    assert documents.get_foreign_keys("purchases-data-years-sfx") == [
+    assert documents.get_foreign_keys(purchases_data_years_invented_table) == [
         ForeignKey(
-            table_name="purchases-data-years-sfx",
+            table_name=purchases_data_years_invented_table,
             columns=["purchases~id"],
-            parent_table_name="purchases-sfx",
+            parent_table_name=purchases_root_invented_table,
             parent_columns=["~PRIMARY_KEY_ID~"],
         )
     ]
 
     # Source children of the source-with-JSON table point to the root invented table
     assert documents.get_foreign_keys("payments") == [
         ForeignKey(
             table_name="payments",
             columns=["purchase_id"],
-            parent_table_name="purchases-sfx",
+            parent_table_name=purchases_root_invented_table,
             parent_columns=["id"],
         )
     ]
 
     # You can request public/user-supplied names instead of the default invented table names
     assert documents.get_foreign_keys("payments", rename_invented_tables=True) == [
         ForeignKey(
@@ -278,35 +341,39 @@
     ]
 
     # Removing a foreign key from the source-with-JSON table updates the root invented table
     documents.remove_foreign_key_constraint(
         table="purchases", constrained_columns=["user_id"]
     )
     assert documents.get_foreign_keys("purchases") == []
-    assert documents.get_foreign_keys("purchases-sfx") == []
+    assert documents.get_foreign_keys(purchases_root_invented_table) == []
 
 
-def test_update_data_with_existing_json_to_new_json(documents):
+def test_update_data_with_existing_json_to_new_json(static_suffix, documents):
     new_purchases_jsonl = """
     {"id": 1, "user_id": 1, "data": {"item": "watercolor", "cost": 200, "details": {"color": "aquamarine"}, "years": [1999]}}
     {"id": 2, "user_id": 2, "data": {"item": "watercolor", "cost": 200, "details": {"color": "aquamarine"}, "years": [1999]}}
     {"id": 3, "user_id": 2, "data": {"item": "watercolor", "cost": 200, "details": {"color": "aquamarine"}, "years": [1999]}}
     {"id": 4, "user_id": 3, "data": {"item": "charcoal", "cost": 200, "details": {"color": "aquamarine"}, "years": [1998]}}
     {"id": 5, "user_id": 3, "data": {"item": "charcoal", "cost": 200, "details": {"color": "aquamarine"}, "years": [1998]}}
     {"id": 6, "user_id": 3, "data": {"item": "charcoal", "cost": 200, "details": {"color": "aquamarine"}, "years": [1998]}}
     """
     new_purchases_df = pd.read_json(new_purchases_jsonl, lines=True)
 
+    # Reset the make_suffix iterator back to original count since make_suffix will be called again
+    # once for each invented table.
+    static_suffix.side_effect = itertools.count(start=1)
+
     documents.update_table_data("purchases", data=new_purchases_df)
 
     assert len(documents.list_all_tables(Scope.ALL)) == 5
     assert len(documents.list_all_tables(Scope.MODELABLE)) == 4
 
     expected = {
-        "purchases-sfx": pd.DataFrame(
+        purchases_root_invented_table: pd.DataFrame(
             data={
                 "~PRIMARY_KEY_ID~": [0, 1, 2, 3, 4, 5],
                 "id": [1, 2, 3, 4, 5, 6],
                 "user_id": [1, 2, 2, 3, 3, 3],
                 "data>item": [
                     "watercolor",
                     "watercolor",
@@ -322,43 +389,43 @@
                     "aquamarine",
                     "aquamarine",
                     "aquamarine",
                     "aquamarine",
                 ],
             }
         ),
-        "purchases-data-years-sfx": pd.DataFrame(
+        purchases_data_years_invented_table: pd.DataFrame(
             data={
                 "content": [1999, 1999, 1999, 1998, 1998, 1998],
                 "array~order": [0, 0, 0, 0, 0, 0],
                 "~PRIMARY_KEY_ID~": [0, 1, 2, 3, 4, 5],
                 "purchases~id": [0, 1, 2, 3, 4, 5],
             }
         ),
     }
 
     pdtest.assert_frame_equal(
-        documents.get_table_data("purchases-sfx"),
-        expected["purchases-sfx"],
+        documents.get_table_data(purchases_root_invented_table),
+        expected[purchases_root_invented_table],
         check_like=True,
     )
 
     pdtest.assert_frame_equal(
-        documents.get_table_data("purchases-data-years-sfx"),
-        expected["purchases-data-years-sfx"],
+        documents.get_table_data(purchases_data_years_invented_table),
+        expected[purchases_data_years_invented_table],
         check_like=True,
         check_dtype=False,  # Without this, test fails asserting dtype mismatch in `content` field (object vs. int)
     )
 
     # User-supplied child table FK still exists
     assert documents.get_foreign_keys("payments") == [
         ForeignKey(
             table_name="payments",
             columns=["purchase_id"],
-            parent_table_name="purchases-sfx",
+            parent_table_name=purchases_root_invented_table,
             parent_columns=["id"],
         )
     ]
 
 
 def test_update_data_existing_json_to_no_json(documents):
     new_purchases_df = pd.DataFrame(
@@ -385,68 +452,72 @@
             columns=["purchase_id"],
             parent_table_name="purchases",
             parent_columns=["id"],
         )
     ]
 
 
-def test_update_data_existing_flat_to_json(documents):
+def test_update_data_existing_flat_to_json(static_suffix, documents):
     # Build up a RelationalData instance that basically mirrors documents,
     # but purchases is flat to start and thus there are no RelationalJson instances
     flat_purchases_df = pd.DataFrame(
         data={
             "id": [1, 2, 3, 4, 5, 6],
             "user_id": [1, 2, 2, 3, 3, 3],
             "data": ["pen", "paint", "ink", "pen", "paint", "ink"],
         }
     )
-    rel_data = RelationalData()
-    rel_data.add_table(
-        name="users", primary_key="id", data=documents.get_table_data("users")
-    )
-    rel_data.add_table(name="purchases", primary_key="id", data=flat_purchases_df)
-    rel_data.add_table(
-        name="payments", primary_key="id", data=documents.get_table_data("payments")
-    )
-    rel_data.add_foreign_key_constraint(
-        table="purchases",
-        constrained_columns=["user_id"],
-        referred_table="users",
-        referred_columns=["id"],
-    )
-    rel_data.add_foreign_key_constraint(
-        table="payments",
-        constrained_columns=["purchase_id"],
-        referred_table="purchases",
-        referred_columns=["id"],
-    )
-    assert len(rel_data.list_all_tables(Scope.ALL)) == 3
-    assert len(rel_data.list_all_tables(Scope.MODELABLE)) == 3
+    with tempfile.TemporaryDirectory() as tmpdir:
+        rel_data = RelationalData(directory=tmpdir)
+        rel_data.add_table(
+            name="users", primary_key="id", data=documents.get_table_data("users")
+        )
+        rel_data.add_table(name="purchases", primary_key="id", data=flat_purchases_df)
+        rel_data.add_table(
+            name="payments", primary_key="id", data=documents.get_table_data("payments")
+        )
+        rel_data.add_foreign_key_constraint(
+            table="purchases",
+            constrained_columns=["user_id"],
+            referred_table="users",
+            referred_columns=["id"],
+        )
+        rel_data.add_foreign_key_constraint(
+            table="payments",
+            constrained_columns=["purchase_id"],
+            referred_table="purchases",
+            referred_columns=["id"],
+        )
+        assert len(rel_data.list_all_tables(Scope.ALL)) == 3
+        assert len(rel_data.list_all_tables(Scope.MODELABLE)) == 3
 
-    rel_data.update_table_data("purchases", documents.get_table_data("purchases"))
+        # Reset the make_suffix iterator back to original count since make_suffix will be called again
+        # once for each invented table.
+        static_suffix.side_effect = itertools.count(start=1)
+        rel_data.update_table_data("purchases", documents.get_table_data("purchases"))
 
     assert set(rel_data.list_all_tables(Scope.ALL)) == {
         "users",
         "purchases",
-        "purchases-sfx",
-        "purchases-data-years-sfx",
+        purchases_root_invented_table,
+        purchases_data_years_invented_table,
         "payments",
     }
     # the original purchases table is no longer flat, nor (therefore) MODELABLE
     assert set(rel_data.list_all_tables(Scope.MODELABLE)) == {
         "users",
-        "purchases-sfx",
-        "purchases-data-years-sfx",
+        purchases_root_invented_table,
+        purchases_data_years_invented_table,
         "payments",
     }
     assert rel_data.get_foreign_keys("payments") == [
         ForeignKey(
             table_name="payments",
             columns=["purchase_id"],
-            parent_table_name="purchases-sfx",  # The foreign key now points to the root invented table
+            parent_table_name=purchases_root_invented_table,  # The foreign key now points to the root invented table
             parent_columns=["id"],
         )
     ]
 
 
 # Simulates output tables from MultiTable transforms or synthetics, which will only include the MODELABLE tables
 @pytest.fixture()
@@ -461,25 +532,25 @@
         "payments": pd.DataFrame(
             data={
                 "id": [1, 2, 3, 4],
                 "amount": [10, 10, 10, 10],
                 "purchase_id": [1, 2, 3, 4],
             }
         ),
-        "purchases-sfx": pd.DataFrame(
+        purchases_root_invented_table: pd.DataFrame(
             data={
                 "~PRIMARY_KEY_ID~": [0, 1, 2, 3],
                 "id": [1, 2, 3, 4],
                 "user_id": [1, 1, 2, 3],
                 "data>item": ["pen", "paint", "ink", "ink"],
                 "data>cost": [18, 19, 20, 21],
                 "data>details>color": ["blue", "yellow", "pink", "orange"],
             }
         ),
-        "purchases-data-years-sfx": pd.DataFrame(
+        purchases_data_years_invented_table: pd.DataFrame(
             data={
                 "content": [2000, 2001, 2002, 2003, 2004, 2005, 2006, 2007],
                 "~PRIMARY_KEY_ID~": [0, 1, 2, 3, 4, 5, 6, 7],
                 "purchases~id": [0, 0, 0, 1, 2, 2, 3, 3],
                 "array~order": [0, 1, 2, 0, 0, 1, 0, 1],
             }
         ),
@@ -530,19 +601,21 @@
 
     for t, df in restored_tables.items():
         pdtest.assert_frame_equal(df, expected[t])
 
 
 def test_restore_with_incomplete_tableset(documents, mt_output_tables):
     without_invented_root = {
-        k: v for k, v in mt_output_tables.items() if k != "purchases-sfx"
+        k: v for k, v in mt_output_tables.items() if k != purchases_root_invented_table
     }
 
     without_invented_child = {
-        k: v for k, v in mt_output_tables.items() if k != "purchases-data-years-sfx"
+        k: v
+        for k, v in mt_output_tables.items()
+        if k != purchases_data_years_invented_table
     }
 
     restored_without_invented_root = documents.restore(without_invented_root)
     restored_without_invented_child = documents.restore(without_invented_child)
 
     # non-JSON-related tables are fine/unaffected
     pdtest.assert_frame_equal(
@@ -597,24 +670,24 @@
             }
         ),
     )
 
 
 def test_restore_with_empty_tables(bball):
     synthetic_bball_output_tables = {
-        "bball-sfx": pd.DataFrame(
+        bball_root_invented_table: pd.DataFrame(
             data={
                 "name": ["Jimmy Butler"],
                 "age": [33],
                 "draft>year": [2011],
                 "draft>college": ["Marquette"],
                 "~PRIMARY_KEY_ID~": [0],
             }
         ),
-        "bball-teams-sfx": pd.DataFrame(
+        bball_teams_invented_table: pd.DataFrame(
             data={
                 "content": ["Bulls", "Timberwolves", "Sixers", "Heat"],
                 "array~order": [0, 1, 2, 3],
                 "~PRIMARY_KEY_ID~": [0, 1, 2, 3],
                 "bball~id": [0, 0, 0, 0],
             }
         ),
@@ -626,15 +699,15 @@
     assert jimmy["name"] == "Jimmy Butler"
     assert jimmy["age"] == 33
     assert jimmy["draft"] == {"year": 2011, "college": "Marquette"}
     assert jimmy["teams"] == ["Bulls", "Timberwolves", "Sixers", "Heat"]
     assert jimmy["suspensions"] == []
 
 
-def test_flatten_and_restore_all_sorts_of_json():
+def test_flatten_and_restore_all_sorts_of_json(tmpdir):
     json = """
 [
     {
         "a": 1,
         "b": {"bb": 1},
         "c": {"cc": {"ccc": 1}},
         "d": [1, 2, 3],
@@ -649,86 +722,92 @@
                     {"fff": 2}
                 ]
             }
         ],
     }
 ]
 """
+    demo_root_invented_table = f"demo_{get_invented_table_suffix(1)}"
+    demo_invented_f_table = f"demo_{get_invented_table_suffix(2)}"
+    demo_invented_f_content_ff_table = f"demo_{get_invented_table_suffix(3)}"
+    demo_invented_e_table = f"demo_{get_invented_table_suffix(4)}"
+    demo_invented_d_table = f"demo_{get_invented_table_suffix(5)}"
+
     json_df = pd.read_json(json, orient="records")
-    rel_data = RelationalData()
+    rel_data = RelationalData(directory=tmpdir)
     rel_data.add_table(name="demo", primary_key=None, data=json_df)
 
     assert set(rel_data.list_all_tables(Scope.ALL)) == {
         "demo",
-        "demo-sfx",
-        "demo-d-sfx",
-        "demo-e-sfx",
-        "demo-f-sfx",
-        "demo-f-content-ff-sfx",
+        demo_root_invented_table,
+        demo_invented_f_table,
+        demo_invented_f_content_ff_table,
+        demo_invented_e_table,
+        demo_invented_d_table,
     }
 
-    assert rel_data.get_table_columns("demo-sfx") == [
+    assert rel_data.get_table_columns(demo_root_invented_table) == [
         "~PRIMARY_KEY_ID~",
         "a",
         "b>bb",
         "c>cc>ccc",
     ]
-    assert rel_data.get_table_columns("demo-d-sfx") == [
+    assert rel_data.get_table_columns(demo_invented_d_table) == [
         "~PRIMARY_KEY_ID~",
         "demo~id",
         "content",
         "array~order",
     ]
-    assert rel_data.get_table_columns("demo-e-sfx") == [
+    assert rel_data.get_table_columns(demo_invented_e_table) == [
         "~PRIMARY_KEY_ID~",
         "demo~id",
         "array~order",
         "content>ee",
     ]
-    assert rel_data.get_table_columns("demo-f-sfx") == [
+    assert rel_data.get_table_columns(demo_invented_f_table) == [
         "~PRIMARY_KEY_ID~",
         "demo~id",
         "array~order",
     ]
-    assert rel_data.get_table_columns("demo-f-content-ff-sfx") == [
+    assert rel_data.get_table_columns(demo_invented_f_content_ff_table) == [
         "~PRIMARY_KEY_ID~",
         "demo^f~id",
         "array~order",
         "content>fff",
     ]
 
     output_tables = {
-        "demo-sfx": pd.DataFrame(
+        demo_root_invented_table: pd.DataFrame(
             data={
                 "a": [1, 2],
                 "b>bb": [3, 4],
                 "c>cc>ccc": [5, 6],
                 "~PRIMARY_KEY_ID~": [0, 1],
             }
         ),
-        "demo-d-sfx": pd.DataFrame(
+        demo_invented_d_table: pd.DataFrame(
             data={
                 "content": [10, 11, 12, 13],
                 "~PRIMARY_KEY_ID~": [0, 1, 2, 3],
                 "demo~id": [0, 0, 0, 1],
                 "array~order": [0, 1, 2, 0],
             }
         ),
-        "demo-e-sfx": pd.DataFrame(
+        demo_invented_e_table: pd.DataFrame(
             data={
                 "content>ee": [100, 200, 300],
                 "~PRIMARY_KEY_ID~": [0, 1, 2],
                 "demo~id": [0, 1, 1],
                 "array~order": [0, 0, 1],
             }
         ),
-        "demo-f-sfx": pd.DataFrame(
+        demo_invented_f_table: pd.DataFrame(
             data={"~PRIMARY_KEY_ID~": [0, 1], "demo~id": [0, 1], "array~order": [0, 0]}
         ),
-        "demo-f-content-ff-sfx": pd.DataFrame(
+        demo_invented_f_content_ff_table: pd.DataFrame(
             data={
                 "content>fff": [10, 11, 12],
                 "~PRIMARY_KEY_ID~": [0, 1, 2],
                 "demo^f~id": [0, 0, 0],
                 "array~order": [0, 1, 2],
             }
         ),
@@ -747,48 +826,54 @@
         }
     )
 
     assert len(restored) == 1
     pdtest.assert_frame_equal(restored["demo"], expected)
 
 
-def test_only_lists_edge_case():
+def test_only_lists_edge_case(tmpdir):
     # Smallest reproduction: a dataframe with just one row and one column, and the value is a list
     list_df = pd.DataFrame(data={"l": [[1, 2, 3, 4]]})
-    rel_data = RelationalData()
+    rel_data = RelationalData(directory=tmpdir)
 
     # Since there are no flat fields on the source, the invented root table would be empty.
     # The root table is what we use for evaluation, so we bail.
     with pytest.raises(ValueError):
         rel_data.add_table(name="list", primary_key=None, data=list_df)
 
     assert rel_data.list_all_tables(Scope.ALL) == []
 
 
-def test_lists_of_lists():
+def test_lists_of_lists(tmpdir):
     # Enough flat data in the source to create a root invented table.
     # Upping the complexity by making the special value a list of lists,
     # but not to fear: we can handle this correctly.
     lol_df = pd.DataFrame(data={"a": [1], "l": [[[1, 2], [3, 4]]]})
-    rel_data = RelationalData()
+    rel_data = RelationalData(directory=tmpdir)
     rel_data.add_table(name="lol", primary_key=None, data=lol_df)
 
+    lol_invented_root_table = f"lol_{get_invented_table_suffix(1)}"
+    lol_invented_l_table = f"lol_{get_invented_table_suffix(2)}"
+    lol_invented_l_content_table = f"lol_{get_invented_table_suffix(3)}"
+
     assert set(rel_data.list_all_tables(Scope.ALL)) == {
         "lol",
-        "lol-sfx",
-        "lol-l-sfx",
-        "lol-l-content-sfx",
+        lol_invented_root_table,
+        lol_invented_l_table,
+        lol_invented_l_content_table,
     }
 
     output = {
-        "lol-sfx": pd.DataFrame(data={"a": [1, 2], "~PRIMARY_KEY_ID~": [0, 1]}),
-        "lol-l-sfx": pd.DataFrame(
+        lol_invented_root_table: pd.DataFrame(
+            data={"a": [1, 2], "~PRIMARY_KEY_ID~": [0, 1]}
+        ),
+        lol_invented_l_table: pd.DataFrame(
             data={"~PRIMARY_KEY_ID~": [0, 1], "lol~id": [0, 0], "array~order": [0, 1]}
         ),
-        "lol-l-content-sfx": pd.DataFrame(
+        lol_invented_l_content_table: pd.DataFrame(
             data={
                 "content": [10, 20, 30, 40],
                 "~PRIMARY_KEY_ID~": [0, 1, 2, 3],
                 "lol^l~id": [0, 0, 1, 1],
                 "array~order": [0, 1, 0, 1],
             }
         ),
@@ -803,34 +888,37 @@
                 "a": [1, 2],
                 "l": [[[10, 20], [30, 40]], []],
             }
         ),
     )
 
 
-def test_mix_of_dict_and_list_cols():
+def test_mix_of_dict_and_list_cols(tmpdir):
     df = pd.DataFrame(
         data={
             "id": [1, 2],
             "dcol": [{"language": "english"}, {"language": "spanish"}],
             "lcol": [["a", "b"], ["c", "d"]],
         }
     )
-    rel_data = RelationalData()
+    mix_invented_root_table = f"mix_{get_invented_table_suffix(1)}"
+    mix_invented_lcol_table = f"mix_{get_invented_table_suffix(2)}"
+
+    rel_data = RelationalData(directory=tmpdir)
     rel_data.add_table(name="mix", primary_key=None, data=df)
     assert set(rel_data.list_all_tables()) == {
-        "mix-sfx",
-        "mix-lcol-sfx",
+        mix_invented_root_table,
+        mix_invented_lcol_table,
     }
-    assert rel_data.get_table_columns("mix-sfx") == [
+    assert rel_data.get_table_columns(mix_invented_root_table) == [
         "~PRIMARY_KEY_ID~",
         "id",
         "dcol>language",
     ]
-    assert rel_data.get_table_columns("mix-lcol-sfx") == [
+    assert rel_data.get_table_columns(mix_invented_lcol_table) == [
         "~PRIMARY_KEY_ID~",
         "mix~id",
         "content",
         "array~order",
     ]
 
 
@@ -851,15 +939,15 @@
             "payments": {
                 "column_count": 3,
                 "primary_key": ["id"],
                 "foreign_key_count": 1,
                 "foreign_keys": [
                     {
                         "columns": ["purchase_id"],
-                        "parent_table_name": "purchases-sfx",
+                        "parent_table_name": purchases_root_invented_table,
                         "parent_columns": ["id"],
                     }
                 ],
                 "is_invented_table": False,
             },
             "purchases": {
                 "column_count": 3,
@@ -869,36 +957,75 @@
                     {
                         "columns": ["user_id"],
                         "parent_table_name": "users",
                         "parent_columns": ["id"],
                     }
                 ],
                 "is_invented_table": False,
+                "invented_table_details": {
+                    "table_type": "producer",
+                    "json_to_table_mappings": {
+                        "purchases": purchases_root_invented_table,
+                        "purchases^data>years": purchases_data_years_invented_table,
+                    },
+                },
             },
-            "purchases-sfx": {
+            purchases_root_invented_table: {
                 "column_count": 6,
                 "primary_key": ["id", "~PRIMARY_KEY_ID~"],
                 "foreign_key_count": 1,
                 "foreign_keys": [
                     {
                         "columns": ["user_id"],
                         "parent_table_name": "users",
                         "parent_columns": ["id"],
                     }
                 ],
                 "is_invented_table": True,
+                "invented_table_details": {
+                    "table_type": "invented",
+                    "json_breadcrumb_path": "purchases",
+                },
             },
-            "purchases-data-years-sfx": {
+            purchases_data_years_invented_table: {
                 "column_count": 4,
                 "primary_key": ["~PRIMARY_KEY_ID~"],
                 "foreign_key_count": 1,
                 "foreign_keys": [
                     {
                         "columns": ["purchases~id"],
-                        "parent_table_name": "purchases-sfx",
+                        "parent_table_name": purchases_root_invented_table,
                         "parent_columns": ["~PRIMARY_KEY_ID~"],
                     }
                 ],
                 "is_invented_table": True,
+                "invented_table_details": {
+                    "table_type": "invented",
+                    "json_breadcrumb_path": "purchases^data>years",
+                },
             },
         },
     }
+
+
+@pytest.mark.no_mock_suffix
+def test_invented_table_names_contain_uuid(documents: RelationalData):
+    regex = re.compile(r"purchases_invented_[a-fA-F0-9]{32}")
+    tables = documents.list_all_tables(Scope.INVENTED)
+    assert len(tables) == 2
+    assert regex.match(tables[0])
+    assert regex.match(tables[1])
+
+
+@pytest.mark.no_mock_suffix
+def test_generate_unique_table_name_truncates_length():
+    table_name_128_chars = "loremipsumdolorsitametconsecteturadipiscingelitseddoeiusmodtemporincididuntutlaboreetdoloremagnaaliquautenimadminimveniamquisnos"
+    result = generate_unique_table_name(table_name_128_chars)
+    assert len(result) < 128
+
+
+@pytest.mark.no_mock_suffix
+def test_deeply_nested_json_truncates_length(deeply_nested):
+    tables = deeply_nested.list_all_tables(Scope.ALL)
+    assert len(tables) == 10
+    for table in tables:
+        assert len(table) < 128
```

### Comparing `gretel-trainer-0.9.0/tests/relational/test_report.py` & `gretel-trainer-0.9.1/tests/relational/test_report.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/tests/relational/test_synthetics_run_task.py` & `gretel-trainer-0.9.1/tests/relational/test_synthetics_run_task.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/tests/relational/test_task_runner.py` & `gretel-trainer-0.9.1/tests/relational/test_task_runner.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/tests/relational/test_train_synthetics.py` & `gretel-trainer-0.9.1/tests/relational/test_train_synthetics.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import tempfile
 from unittest.mock import ANY, patch
 
 import pytest
 
 from gretel_trainer.relational.core import MultiTableException
 from gretel_trainer.relational.multi_table import MultiTable
+from tests.relational.conftest import get_invented_table_suffix
 
 
 # The assertions in this file are concerned with setting up the synthetics train
 # workflow state properly, and stop short of kicking off the task.
 @pytest.fixture(autouse=True)
 def run_task():
     with patch("gretel_trainer.relational.multi_table.run_task"):
@@ -205,19 +206,22 @@
     assert set(mt._synthetics_train.models.keys()) == {"products", "users"}
 
 
 def test_train_synthetics_models_for_dbs_with_invented_tables(documents, tmpdir):
     mt = MultiTable(documents, project_display_name=tmpdir)
     mt.train_synthetics()
 
+    purchases_root_invented_table = f"purchases_{get_invented_table_suffix(1)}"
+    purchases_data_years_invented_table = f"purchases_{get_invented_table_suffix(2)}"
+
     assert set(mt._synthetics_train.models.keys()) == {
         "users",
         "payments",
-        "purchases-sfx",
-        "purchases-data-years-sfx",
+        purchases_root_invented_table,
+        purchases_data_years_invented_table,
     }
 
 
 def test_train_synthetics_table_filters_cascade_to_invented_tables(documents, tmpdir):
     # When a user provides the ("public") name of a table that contained JSON and led
     # to the creation of invented tables, we recognize that as implicitly applying to
     # all the tables internally created from that source table.
```

### Comparing `gretel-trainer-0.9.0/tests/relational/test_train_transforms.py` & `gretel-trainer-0.9.1/tests/relational/test_train_transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     mt = MultiTable(ecom, project_display_name=tmpdir)
     mt.train_transforms("transform/default", only={"users"})
     transforms_train = mt._transforms_train
 
     assert set(transforms_train.models.keys()) == {"users"}
     project.create_model_obj.assert_called_with(
         model_config=ANY,  # a tailored transforms config, in dict form
-        data_source=f"{tmpdir}/transforms_train_users.csv",
+        data_source=f"{tmpdir}/users.csv",
     )
 
 
 def test_train_transforms_ignore_excludes_specified_tables(ecom, tmpdir):
     mt = MultiTable(ecom, project_display_name=tmpdir)
     mt.train_transforms("transform/default", ignore={"distribution_center", "products"})
     transforms_train = mt._transforms_train
```

### Comparing `gretel-trainer-0.9.0/tests/test_benchmark.py` & `gretel-trainer-0.9.1/tests/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.9.0/tests/test_strategy.py` & `gretel-trainer-0.9.1/tests/test_strategy.py`

 * *Files identical despite different names*

