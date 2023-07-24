# Comparing `tmp/maud-metabolic-models-0.5.1.1.tar.gz` & `tmp/maud-metabolic-models-0.6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maud-metabolic-models-0.5.1.1.tar", last modified: Mon Jul 10 11:37:44 2023, max compression
+gzip compressed data, was "maud-metabolic-models-0.6.0.0.tar", last modified: Sun Jul 23 23:40:33 2023, max compression
```

## Comparing `maud-metabolic-models-0.5.1.1.tar` & `maud-metabolic-models-0.6.0.0.tar`

### file list

```diff
@@ -1,79 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:37:44.901083 maud-metabolic-models-0.5.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    32473 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-07-10 11:37:44.901083 maud-metabolic-models-0.5.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-10 11:37:44.901083 maud-metabolic-models-0.5.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:37:44.893082 maud-metabolic-models-0.5.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:37:44.897083 maud-metabolic-models-0.5.1.1/src/maud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    14310 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:37:44.893082 maud-metabolic-models-0.5.1.1/src/maud/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:37:44.893082 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:37:44.897083 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/example_ode/
--rw-r--r--   0 runner    (1001) docker     (123)    12765 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/example_ode/ODE_solution.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/example_ode/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/example_ode/experimental_setup.toml
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/example_ode/experiments.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/example_ode/inits.json
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/example_ode/input_data_train.json
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/example_ode/kinetic_model.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/example_ode/priors.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:37:44.897083 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/linear/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/linear/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/linear/expected_stan_input.json
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/linear/experiments.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/linear/kinetic_model.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/linear/parameters.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/linear/priors.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:37:44.897083 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/methionine/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/methionine/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)    13239 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/methionine/experiments.toml
--rw-r--r--   0 runner    (1001) docker     (123)    30701 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/methionine/inits.toml
--rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/methionine/methionine_cycle.toml
--rw-r--r--   0 runner    (1001) docker     (123)    36446 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/methionine/parameters.toml
--rw-r--r--   0 runner    (1001) docker     (123)    36103 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/methionine/priors.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:37:44.893082 maud-metabolic-models-0.5.1.1/src/maud/data/example_outputs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:37:44.893082 maud-metabolic-models-0.5.1.1/src/maud/data/example_outputs/linear/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:37:44.897083 maud-metabolic-models-0.5.1.1/src/maud/data/example_outputs/linear/user_input/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_outputs/linear/user_input/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_outputs/linear/user_input/experiments.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_outputs/linear/user_input/kinetic_model.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_outputs/linear/user_input/parameters.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data/example_outputs/linear/user_input/priors.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:37:44.901083 maud-metabolic-models-0.5.1.1/src/maud/data_model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data_model/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data_model/hardcoding.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data_model/id_component.py
--rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data_model/kinetic_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data_model/maud_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data_model/maud_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data_model/maud_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    20305 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data_model/maud_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data_model/prior.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/data_model/prior_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/getting_idatas.py
--rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/getting_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/getting_priors.py
--rw-r--r--   0 runner    (1001) docker     (123)    20455 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/getting_stan_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/loading_maud_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/parsing_kinetic_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/running_stan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:37:44.901083 maud-metabolic-models-0.5.1.1/src/maud/stan/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/stan/debug.stan
--rw-r--r--   0 runner    (1001) docker     (123)    20773 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/stan/functions.stan
--rw-r--r--   0 runner    (1001) docker     (123)    19183 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/stan/model.stan
--rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/stan/out_of_sample_model.stan
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-10 11:37:34.000000 maud-metabolic-models-0.5.1.1/src/maud/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:37:44.901083 maud-metabolic-models-0.5.1.1/src/maud_metabolic_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-07-10 11:37:44.000000 maud-metabolic-models-0.5.1.1/src/maud_metabolic_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-10 11:37:44.000000 maud-metabolic-models-0.5.1.1/src/maud_metabolic_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 11:37:44.000000 maud-metabolic-models-0.5.1.1/src/maud_metabolic_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-10 11:37:44.000000 maud-metabolic-models-0.5.1.1/src/maud_metabolic_models.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-10 11:37:44.000000 maud-metabolic-models-0.5.1.1/src/maud_metabolic_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 11:37:44.000000 maud-metabolic-models-0.5.1.1/src/maud_metabolic_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 11:37:44.000000 maud-metabolic-models-0.5.1.1/src/maud_metabolic_models.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:40:33.403416 maud-metabolic-models-0.6.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    32473 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-23 23:40:33.403416 maud-metabolic-models-0.6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:40:33.395416 maud-metabolic-models-0.6.0.0/maud/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14864 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:40:33.395416 maud-metabolic-models-0.6.0.0/maud/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:40:33.395416 maud-metabolic-models-0.6.0.0/maud/data/example_inputs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:40:33.399416 maud-metabolic-models-0.6.0.0/maud/data/example_inputs/example_ode/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data/example_inputs/example_ode/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data/example_inputs/example_ode/experimental_setup.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data/example_inputs/example_ode/experiments.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data/example_inputs/example_ode/inits.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data/example_inputs/example_ode/input_data_train.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data/example_inputs/example_ode/kinetic_model.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data/example_inputs/example_ode/priors.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:40:33.399416 maud-metabolic-models-0.6.0.0/maud/data/example_inputs/linear/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data/example_inputs/linear/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data/example_inputs/linear/expected_stan_input.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data/example_inputs/linear/experiments.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data/example_inputs/linear/kinetic_model.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data/example_inputs/linear/parameters.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data/example_inputs/linear/priors.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:40:33.395416 maud-metabolic-models-0.6.0.0/maud/data/example_outputs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:40:33.395416 maud-metabolic-models-0.6.0.0/maud/data/example_outputs/linear/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:40:33.399416 maud-metabolic-models-0.6.0.0/maud/data/example_outputs/linear/user_input/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data/example_outputs/linear/user_input/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data/example_outputs/linear/user_input/experiments.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data/example_outputs/linear/user_input/kinetic_model.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data/example_outputs/linear/user_input/parameters.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data/example_outputs/linear/user_input/priors.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:40:33.403416 maud-metabolic-models-0.6.0.0/maud/data_model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data_model/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data_model/hardcoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data_model/id_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data_model/kinetic_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data_model/maud_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data_model/maud_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data_model/maud_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20305 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data_model/maud_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data_model/parameter_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data_model/prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/data_model/prior_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/getting_idatas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/getting_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/getting_priors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20455 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/getting_stan_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/loading_maud_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/parsing_kinetic_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/running_stan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:40:33.403416 maud-metabolic-models-0.6.0.0/maud/stan/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/stan/debug.stan
+-rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/stan/functions.stan
+-rw-r--r--   0 runner    (1001) docker     (123)    19181 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/stan/model.stan
+-rw-r--r--   0 runner    (1001) docker     (123)    12663 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/stan/out_of_sample_model.stan
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/maud/utility_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:40:33.403416 maud-metabolic-models-0.6.0.0/maud_metabolic_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-23 23:40:33.000000 maud-metabolic-models-0.6.0.0/maud_metabolic_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-23 23:40:33.000000 maud-metabolic-models-0.6.0.0/maud_metabolic_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 23:40:33.000000 maud-metabolic-models-0.6.0.0/maud_metabolic_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 23:40:33.000000 maud-metabolic-models-0.6.0.0/maud_metabolic_models.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-23 23:40:33.000000 maud-metabolic-models-0.6.0.0/maud_metabolic_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-23 23:40:33.000000 maud-metabolic-models-0.6.0.0/maud_metabolic_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 23:40:33.403416 maud-metabolic-models-0.6.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-07-23 23:40:17.000000 maud-metabolic-models-0.6.0.0/setup.py
```

### Comparing `maud-metabolic-models-0.5.1.1/LICENSE` & `maud-metabolic-models-0.6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.1.1/README.rst` & `maud-metabolic-models-0.6.0.0/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -14,24 +14,24 @@
    :target: https://www.contributor-covenant.org/
    :alt: Contributor Covenant Version 1.4
 
 .. image:: https://readthedocs.org/projects/maud-metabolic-models/badge/?version=latest
    :target: https://maud-metabolic-models.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 
-Maud is a work-in-progress application that fits Bayesian statistical models of
+Maud is an application that fits Bayesian statistical models of
 metabolic networks using `Python <https://www.python.org/>`_ and `Stan
 <https://mc-stan.org>`_.
 
 Maud aims to take into account allosteric effects, ensure that the laws of
 thermodynamics are obeyed and to synthesise information from both steady state
 experiments and the existing literature.
 
-Install
-=======
+Installation
+============
 First create a fresh Python virtual environment and then activate it:
 
 .. code-block:: console
 
     python -m venv .venv --prompt=maud
     source .venv/bin/activate
 
@@ -39,52 +39,27 @@
 this command:
 
 .. code-block:: console
 
     pip install maud-metabolic-models
 
 Cmdstanpy depends on `cmdstan <https://github.com/stan-dev/cmdstan>`_, 
-which in turn requires a c++ toolchain. Fortunately, cmdstanpy comes with
-commands that can install these for you. On windows the necessary dependencies 
-can be installed with the following powershell commands:
+which in turn requires a c++ toolchain. On some computers you will have to 
+install these in order to use Maud. You will hit an error at the next step if 
+this applies to your computer. Luckily cmdstanpy comes with commands that
+can do the necessary installing for you. On windows the c++ toolchain can be installed with 
+the following powershell commands:
 
-.. code-block:: console
-
-    python -m cmdstanpy.install_cxx_toolchain
-    python -m cmdstanpy.install_cmdstan --compiler
-
-On macos or Linux, you must install the c++ requirements manually 
-(see [here](https://cmdstanpy.readthedocs.io/en/v0.9.67/installation.html#install-cmdstan)) for instuctions. 
-Cmdstan can then be installed using this shell command:
-
-.. code-block:: console
-
-    install_cmdstan
 
 Usage
 =====
-To run the simple linear model, use the following command:
+Maud is used from the command line. To see all the available commands try running 
 
 .. code-block:: console
 
-    maud sample
-
-This will compile the Stan program at `src/maud/inference_model.stan
-<https://github.com/biosustain/Maud/blob/master/src/maud/inference_model.stan>`_, 
-then run the resulting binary file using the data at `src/maud/data/example_inputs/linear
-<https://github.com/biosustain/Maud/blob/master/src/maud/data/example_inputs/linear>`_, storing
-the results in a folder whose name starts with
-:code:`model_output_linear`.
-
-The `sample` command can be configured in a few ways - to check out all the
-options try running
-
-.. code-block:: console
-
-    maud sample --help
-
+    maud --help
 
 Copyright
 =========
 
-* Copyright (c) 2019, Novo Nordisk Foundation Center for Biosustainability, Technical University of Denmark.
+* Copyright (c) 2023, Novo Nordisk Foundation Center for Biosustainability, Technical University of Denmark.
 * Free software distributed under the `GNU General Public License 3.0 <https://www.gnu.org/licenses/>`_
```

### Comparing `maud-metabolic-models-0.5.1.1/src/maud/analysis.py` & `maud-metabolic-models-0.6.0.0/maud/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,15 @@
 
 def join_list_of_strings(l1, l2, sep="-"):
     """Join strings for use in infd coordinates."""
     return list(map(lambda a: f"{a[0]}{sep}{a[1]}", zip(l1, l2)))
 
 
 def load_infd_fit(fit, mi: MaudInput) -> az.InferenceData:
-    """Get an arviz InferenceData object from out-of-sample tmp generated csvs."""
-
+    """Get an InferenceData object from out-of-sample tmp generated csvs."""
     coords = {
         **mi.stan_coords.__dict__,
         **{
             "reactions": mi.stan_coords.reactions,
             "kms": join_list_of_strings(
                 mi.stan_coords.km_enzs, mi.stan_coords.km_mics
             ),
@@ -53,15 +52,14 @@
         },
         save_warmup=True,
     )
 
 
 def load_infd(csvs: List[str], mi: MaudInput) -> az.InferenceData:
     """Get an arviz InferenceData object from Maud csvs."""
-
     Numba.disable_numba()
     coords = {
         **mi.stan_coords.__dict__,
         **{
             "reactions": mi.stan_coords.reactions,
             "kms": join_list_of_strings(
                 mi.stan_coords.km_enzs, mi.stan_coords.km_mics
```

### Comparing `maud-metabolic-models-0.5.1.1/src/maud/cli.py` & `maud-metabolic-models-0.6.0.0/maud/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,36 +20,52 @@
 import shutil
 from datetime import datetime
 
 import arviz as az
 import click
 import importlib_resources
 
-from maud.data.example_inputs import linear
+from maud.data.example_inputs import linear, methionine
 from maud.getting_idatas import get_idata
 from maud.loading_maud_inputs import load_maud_input
 from maud.running_stan import optimize, predict, sample, simulate, variational
 
-
-EXAMPLE_INPUT_PATH = importlib_resources.files(linear)._paths[0]
+AVAILABLE_EXAMPLE_INPUTS = {"linear": linear, "methionine": methionine}
 
 
 @click.group()
 @click.help_option("--help", "-h")
 def cli():
     """Use Maud's command line interface."""
     pass
 
 
+@cli.command("load-input")
+@click.option("--output_dir", default=".", help="Where to save the folder.")
+@click.argument("input_name", type=click.STRING)
+def load_input_command(input_name, output_dir):
+    """Extract one of Maud's example inputs.
+
+    Available inputs: "linear", "methionine"
+    """
+    if input_name not in AVAILABLE_EXAMPLE_INPUTS.keys():
+        raise ValueError(
+            f"{input_name} not available."
+            " Available inputs:\n\t{'\n\t'.split(available)}"
+        )
+    data = AVAILABLE_EXAMPLE_INPUTS[input_name]
+    path = importlib_resources.files(data)._paths[0]
+    shutil.copytree(path, os.path.join(output_dir, input_name))
+
+
 @cli.command("sample")
 @click.option("--output_dir", default=".", help="Where to save Maud's output")
 @click.argument(
     "data_path",
     type=click.Path(exists=True, dir_okay=True, file_okay=False),
-    default=EXAMPLE_INPUT_PATH,
 )
 def sample_command(data_path, output_dir):
     """Generate MCMC samples given a user input directory.
 
     This function creates a new directory in output_dir with a name starting
     with "maud_output". It first copies the directory at data_path into the new
     this directory at new_dir/user_input, then runs the running_stan.sample
@@ -140,36 +156,33 @@
 
 @cli.command("simulate")
 @click.option("--output_dir", default=".", help="Where to save the output")
 @click.option("-n", default=1, type=int, help="Number of simulations")
 @click.argument(
     "data_path",
     type=click.Path(exists=True, dir_okay=True, file_okay=False),
-    default=EXAMPLE_INPUT_PATH,
 )
 def simulate_command(data_path, output_dir, n):
     """Generate draws from the initial values."""
     click.echo(do_simulate(data_path, output_dir, n))
 
 
 @cli.command("optimize")
 @click.option("--output_dir", default=".", help="Where to save the output")
 @click.argument(
     "data_path",
     type=click.Path(exists=True, dir_okay=True, file_okay=False),
-    default=EXAMPLE_INPUT_PATH,
 )
 def optimize_command(data_path, output_dir):
     """Optimize the model parameters."""
     click.echo(do_optimize(data_path, output_dir))
 
 
 def do_simulate(data_path, output_dir, n):
     """Generate draws from the initial values."""
-
     mi = load_maud_input(data_path=data_path)
     now = datetime.now().strftime("%Y%m%d%H%M%S")
     output_name = f"maud_output_sim-{mi.config.name}-{now}"
     output_path = os.path.join(output_dir, output_name)
     samples_path = os.path.join(output_path, "samples")
     ui_dir = os.path.join(output_path, "user_input")
     print("Creating output directory: " + output_path)
@@ -266,15 +279,14 @@
         idata.posterior["psi_train"].mean(dim=["chain", "draw"]).to_series().T
     )
     return output_path
 
 
 def do_optimize(data_path, output_dir):
     """Optimize the model parameters."""
-
     mi = load_maud_input(data_path=data_path)
     now = datetime.now().strftime("%Y%m%d%H%M%S")
     output_name = f"maud_output_opt-{mi.config.name}-{now}"
     output_path = os.path.join(output_dir, output_name)
     samples_path = os.path.join(output_path, "samples")
     ui_dir = os.path.join(output_path, "user_input")
     print("Creating output directory: " + output_path)
@@ -376,15 +388,14 @@
 
 
 @cli.command("variational")
 @click.option("--output_dir", default=".", help="Where to save Maud's output")
 @click.argument(
     "data_path",
     type=click.Path(exists=True, dir_okay=True, file_okay=False),
-    default=EXAMPLE_INPUT_PATH,
 )
 def variational_command(data_path, output_dir):
     """Generate MCMC samples given a user input directory.
 
     This function creates a new directory in output_dir with a name starting
     with "maud_output". It first copies the directory at data_path into the new
     this directory at new_dir/user_input, then runs the running_stan.sample
```

### Comparing `maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/example_ode/experiments.toml` & `maud-metabolic-models-0.6.0.0/maud/data/example_inputs/example_ode/experiments.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/example_ode/inits.json` & `maud-metabolic-models-0.6.0.0/maud/data/example_inputs/example_ode/inits.json`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/example_ode/input_data_train.json` & `maud-metabolic-models-0.6.0.0/maud/data/example_inputs/example_ode/input_data_train.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -240,8 +240,8 @@
 00000ef0: 6f6c 223a 2031 652d 3039 2c20 2261 6273  ol": 1e-09, "abs
 00000f00: 5f74 6f6c 223a 2031 652d 3039 2c20 2274  _tol": 1e-09, "t
 00000f10: 696d 6570 6f69 6e74 223a 2031 3030 302e  imepoint": 1000.
 00000f20: 302c 2022 6d61 785f 6e75 6d5f 7374 6570  0, "max_num_step
 00000f30: 7322 3a20 3130 3030 3030 3030 3030 2c20  s": 1000000000, 
 00000f40: 2263 6f6e 635f 696e 6974 223a 205b 5b30  "conc_init": [[0
 00000f50: 2e33 3233 3131 372c 2033 2e30 3231 3837  .323117, 3.02187
-00000f60: 5d5d 7d                                  ]]}
+00000f60: 5d5d 7d0a                                ]]}.
```

### Comparing `maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/example_ode/kinetic_model.toml` & `maud-metabolic-models-0.6.0.0/maud/data/example_inputs/example_ode/kinetic_model.toml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -89,8 +89,8 @@
 metabolite_id = "C"
 compartment_id = "c"
 
 [[allostery]]
 modification_type = "inhibition"
 enzyme_id = "r2B"
 metabolite_id = "C"
-compartment_id = "c"
+compartment_id = "c"
```

### Comparing `maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/example_ode/priors.toml` & `maud-metabolic-models-0.6.0.0/maud/data/example_inputs/example_ode/priors.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/linear/expected_stan_input.json` & `maud-metabolic-models-0.6.0.0/maud/data/example_inputs/linear/expected_stan_input.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -195,8 +195,8 @@
 00000c20: 2272 656c 5f74 6f6c 223a 2031 652d 3035  "rel_tol": 1e-05
 00000c30: 2c20 2261 6273 5f74 6f6c 223a 2031 652d  , "abs_tol": 1e-
 00000c40: 3035 2c20 2274 696d 6570 6f69 6e74 223a  05, "timepoint":
 00000c50: 2031 3030 302e 302c 2022 6d61 785f 6e75   1000.0, "max_nu
 00000c60: 6d5f 7374 6570 7322 3a20 3130 3030 3030  m_steps": 100000
 00000c70: 302c 2022 636f 6e63 5f69 6e69 7422 3a20  0, "conc_init": 
 00000c80: 5b5b 302e 3539 2c20 302e 3338 5d2c 205b  [[0.59, 0.38], [
-00000c90: 302e 3534 2c20 302e 3338 5d5d 7d         0.54, 0.38]]}
+00000c90: 302e 3534 2c20 302e 3338 5d5d 7d0a       0.54, 0.38]]}.
```

### Comparing `maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/linear/experiments.toml` & `maud-metabolic-models-0.6.0.0/maud/data/example_inputs/linear/experiments.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/linear/kinetic_model.toml` & `maud-metabolic-models-0.6.0.0/maud/data/example_inputs/linear/kinetic_model.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/linear/parameters.toml` & `maud-metabolic-models-0.6.0.0/maud/data/example_inputs/linear/parameters.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.1.1/src/maud/data/example_inputs/linear/priors.toml` & `maud-metabolic-models-0.6.0.0/maud/data/example_inputs/linear/priors.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.1.1/src/maud/data/example_outputs/linear/user_input/experiments.toml` & `maud-metabolic-models-0.6.0.0/maud/data/example_outputs/linear/user_input/experiments.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.1.1/src/maud/data/example_outputs/linear/user_input/kinetic_model.toml` & `maud-metabolic-models-0.6.0.0/maud/data/example_outputs/linear/user_input/kinetic_model.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.1.1/src/maud/data/example_outputs/linear/user_input/parameters.toml` & `maud-metabolic-models-0.6.0.0/maud/data/example_outputs/linear/user_input/parameters.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.1.1/src/maud/data/example_outputs/linear/user_input/priors.toml` & `maud-metabolic-models-0.6.0.0/maud/data/example_outputs/linear/user_input/priors.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.1.1/src/maud/data_model/experiment.py` & `maud-metabolic-models-0.6.0.0/maud/data_model/experiment.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.1.1/src/maud/data_model/kinetic_model.py` & `maud-metabolic-models-0.6.0.0/maud/data_model/kinetic_model.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.1.1/src/maud/data_model/maud_config.py` & `maud-metabolic-models-0.6.0.0/maud/data_model/maud_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,21 +22,21 @@
     :param kinetic_model_file: path to a valid kientic model file.
     :param priors_file: path to a valid priors file.
     :param experiments_file: path to a valid experiments file.
     :param likelihood: Whether or not to take measurements into account.
     :param cmdstanpy_config: Arguments to cmdstanpy.CmdStanModel.sample.
     :param reject_non_steady: Reject draws if a non-steady state is encountered.
     :param ode_config: Configuration for Stan's ode solver.
-    :param stanc_options: Valid choices for CmdStanModel argument `stanc_options`.
-    :param cpp_options: Valid choices for CmdStanModel `cpp_options`.
+    :param stanc_options: Options for CmdStanModel argument `stanc_options`.
+    :param cpp_options: Options for CmdStanModel `cpp_options`.
     :param variational_options: Arguments for CmdStanModel.variational.
     :param optimize_options: Arguments for CmdStanModel.optimize.
     :param user_inits_file: path to a csv file of initial values.
-    :param steady_state_threshold_abs: absolute threshold for Sv=0 be at steady state
-    :param steady_state_threshold_rel: relative threshold for Sv=0 be at steady state
+    :param steady_state_threshold_abs: abs threshold for Sv=0 be at steady state
+    :param steady_state_threshold_rel: rel threshold for Sv=0 be at steady state
     :param default_initial_concentration: in molecule_unit per volume_unit
     :param drain_small_conc_corrector: number for correcting small conc drains
     :param molecule_unit: A unit for counting molecules, like 'mol' or 'mmol'
     :param volume_unit: A unit for measuring volume, like 'L'
     :param energy_unit: A unit for measuring energy, like 'J' or 'kJ'
     """
```

### Comparing `maud-metabolic-models-0.5.1.1/src/maud/data_model/maud_init.py` & `maud-metabolic-models-0.6.0.0/maud/data_model/maud_init.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 
 
 def get_init_atom_input_ids(
     iai: InitAtomInput,
     id_components: List[List[IdComponent]],
 ) -> Tuple[str, ...]:
     """Get an init's id from a userinput."""
-
     return tuple(
         ID_SEPARATOR.join([getattr(iai, c) for c in idci])
         for idci in id_components
     )
 
 
 @dataclass(init=False)
```

### Comparing `maud-metabolic-models-0.5.1.1/src/maud/data_model/maud_input.py` & `maud-metabolic-models-0.6.0.0/maud/data_model/maud_input.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.1.1/src/maud/data_model/maud_parameter.py` & `maud-metabolic-models-0.6.0.0/maud/data_model/maud_parameter.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.1.1/src/maud/data_model/prior.py` & `maud-metabolic-models-0.6.0.0/maud/data_model/prior.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.1.1/src/maud/data_model/prior_input.py` & `maud-metabolic-models-0.6.0.0/maud/data_model/prior_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     scale: Optional[float] = None
     pct1: Optional[float] = None
     pct99: Optional[float] = None
 
     @validator("scale")
     def scale_is_positive(cls, v):
         """Check that scale is positive."""
-
         if v is not None and v <= 0:
             raise ValueError("scale must be a positive number.")
         return v
 
     @root_validator(pre=False, skip_on_failure=True)
     def prior_is_specified_correctly(cls, values):
         """Check that location, scale etc are correct."""
```

### Comparing `maud-metabolic-models-0.5.1.1/src/maud/getting_idatas.py` & `maud-metabolic-models-0.6.0.0/maud/getting_idatas.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from maud.data_model.experiment import MeasurementType
 from maud.data_model.hardcoding import ID_SEPARATOR
 from maud.data_model.maud_input import MaudInput
 
 
 def get_idata(csvs: List[str], mi: MaudInput, mode: str) -> az.InferenceData:
     """Get an arviz InferenceData object from Maud csvs."""
-
     experiments = (
         [e for e in mi.experiments if e.is_train]
         if mode == "train"
         else [e for e in mi.experiments if e.is_test]
     )
     yconc_coords, yflux_coords, yenz_coords = (
         [
```

### Comparing `maud-metabolic-models-0.5.1.1/src/maud/getting_parameters.py` & `maud-metabolic-models-0.6.0.0/maud/getting_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     ParameterSet,
     PsiTest,
     PsiTrain,
     TransferConstant,
 )
 from maud.data_model.prior_input import PriorInput
 
-
 AllostericCoords = Tuple[List[str], List[str], List[str], List[str], List[str]]
 KmCoords = Tuple[List[str], List[str], List[str], List[str]]
 KcatCoords = Tuple[List[str], List[str], List[str]]
 KiCoords = Tuple[List[str], List[str], List[str], List[str], List[str]]
 
 
 def get_km_coords(kinetic_model: KineticModel) -> KmCoords:
```

### Comparing `maud-metabolic-models-0.5.1.1/src/maud/getting_priors.py` & `maud-metabolic-models-0.6.0.0/maud/getting_priors.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import numpy as np
 import pandas as pd
 
 from maud.data_model.hardcoding import ID_SEPARATOR
 from maud.data_model.maud_parameter import IdComponent
 from maud.data_model.prior import IndPrior1d, IndPrior2d, PriorMVN
 from maud.data_model.prior_input import IndPriorAtomInput, PriorMVNInput
-from maud.utils import (
+from maud.utility_functions import (
     get_lognormal_parameters_from_quantiles,
     get_normal_parameters_from_quantiles,
 )
 
 
 def get_loc_and_scale(
     ipai: IndPriorAtomInput, non_negative: bool
```

### Comparing `maud-metabolic-models-0.5.1.1/src/maud/getting_stan_inputs.py` & `maud-metabolic-models-0.6.0.0/maud/getting_stan_inputs.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.5.1.1/src/maud/loading_maud_inputs.py` & `maud-metabolic-models-0.6.0.0/maud/loading_maud_inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 from maud.data_model.maud_init import InitInput
 from maud.data_model.maud_input import MaudInput
 from maud.data_model.prior_input import PriorInput
 from maud.parsing_kinetic_models import parse_kinetic_model
 
 
 def load_maud_input(data_path: str) -> MaudInput:
-    """
-    Load an MaudInput object from a data path.
+    """Load an MaudInput object from a data path.
 
     :param filepath: path to directory containing input toml file
     :param mode: determines which experiments will be included,
     defined in the `experimental_setup` as "sample" and/or "predict".
 
     """
     # get config
```

### Comparing `maud-metabolic-models-0.5.1.1/src/maud/parsing_kinetic_models.py` & `maud-metabolic-models-0.6.0.0/maud/parsing_kinetic_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     Metabolite,
     MetaboliteInCompartment,
     ModificationType,
     Phosphorylation,
     Reaction,
     ReactionMechanism,
 )
-from maud.utils import read_with_fallback
+from maud.utility_functions import read_with_fallback
 
 
 def parse_kinetic_model(raw: dict) -> KineticModel:
     """Turn the output of toml.load into a KineticModel object.
 
     :param raw: Result of running toml.load on a suitable toml file
```

### Comparing `maud-metabolic-models-0.5.1.1/src/maud/running_stan.py` & `maud-metabolic-models-0.6.0.0/maud/running_stan.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 """Code for sampling from a posterior distribution."""
 
 import os
+import shutil
+import warnings
+from pathlib import Path
 
 import arviz as az
 import cmdstanpy
 from cmdstanpy import CmdStanMLE
 from cmdstanpy.stanfit.mcmc import CmdStanMCMC
 from cmdstanpy.stanfit.vb import CmdStanVB
 
 from maud.data_model.maud_input import MaudInput
 
+CMDSTAN_VERSION = "2.32.2"
 
 HERE = os.path.dirname(os.path.abspath(__file__))
 DEFAULT_PRIOR_LOC_DRAIN = None
 DEFAULT_PRIOR_SCALE_DRAIN = None
+STAN_FILES_FOLDER = Path(__file__).parent / "stan"
 STAN_PROGRAM_RELATIVE_PATH = os.path.join("stan", "model.stan")
 STAN_PROGRAM_RELATIVE_PATH_PREDICT = os.path.join(
     "stan", "out_of_sample_model.stan"
 )
 PPC_PROGRAM_RELATIVE_PATH = "out_of_sample_model.stan"
 
 DEFAULT_SAMPLE_CONFIG = {
@@ -52,24 +57,55 @@
     "show_console": True,
     "refresh": 1,
     "save_profile": True,
     "save_iterations": True,
 }
 
 
+def load_stan_model(
+    name: str, cpp_options: dict, stanc_options: dict
+) -> cmdstanpy.CmdStanModel:
+    """Try to load precompiled Stan models.
+
+    If that fails, compile them.
+    """
+    try:
+        model = cmdstanpy.CmdStanModel(
+            exe_file=STAN_FILES_FOLDER / f"{name}.exe",
+            stan_file=STAN_FILES_FOLDER / f"{name}.stan",
+            cpp_options=cpp_options,
+            stanc_options=stanc_options,
+            compile=False,
+        )
+    except ValueError:
+        warnings.warn(
+            f"Failed to load pre-built model '{name}.exe', compiling",
+            stacklevel=2,
+        )
+        model = cmdstanpy.CmdStanModel(
+            stan_file=STAN_FILES_FOLDER / f"{name}.stan",
+            cpp_options=cpp_options,
+            stanc_options=stanc_options,
+        )
+        shutil.copy(
+            model.exe_file,  # type: ignore
+            STAN_FILES_FOLDER / f"{name}.exe",
+        )
+
+    return model
+
+
 def sample(mi: MaudInput, output_dir: str) -> CmdStanMCMC:
     """Sample from the posterior defined by mi.
 
     :param mi: a MaudInput object
     :param output_dir: a string specifying where to save the output.
     """
-    model = cmdstanpy.CmdStanModel(
-        stan_file=os.path.join(HERE, STAN_PROGRAM_RELATIVE_PATH),
-        cpp_options=mi.config.cpp_options,
-        stanc_options=mi.config.stanc_options,
+    model = load_stan_model(
+        "model", mi.config.cpp_options, mi.config.stanc_options
     )
     set_up_output_dir(output_dir, mi)
     sample_args: dict = {
         "data": os.path.join(output_dir, "input_data_train.json"),
         "inits": os.path.join(output_dir, "inits.json"),
         "output_dir": output_dir,
     }
@@ -86,18 +122,16 @@
     :param output_dir: a string specifying where to save the output.
     """
     mi_options = (
         {}
         if mi.config.variational_options is None
         else mi.config.variational_options
     )
-    model = cmdstanpy.CmdStanModel(
-        stan_file=os.path.join(HERE, STAN_PROGRAM_RELATIVE_PATH),
-        cpp_options=mi.config.cpp_options,
-        stanc_options=mi.config.stanc_options,
+    model = load_stan_model(
+        "model", mi.config.cpp_options, mi.config.stanc_options
     )
     set_up_output_dir(output_dir, mi)
     return model.variational(
         data=os.path.join(output_dir, "input_data_train.json"),
         inits=os.path.join(output_dir, "inits.json"),
         **{
             **DEFAULT_VARIATIONAL_CONFIG,
@@ -109,18 +143,16 @@
 
 def simulate(mi: MaudInput, output_dir: str, n: int) -> CmdStanMCMC:
     """Generate simulations from the prior mean.
 
     :param mi: a MaudInput object
     :param output_dir: a string specifying where to save the output.
     """
-    model = cmdstanpy.CmdStanModel(
-        stan_file=os.path.join(HERE, STAN_PROGRAM_RELATIVE_PATH),
-        cpp_options=mi.config.cpp_options,
-        stanc_options=mi.config.stanc_options,
+    model = load_stan_model(
+        "model", mi.config.cpp_options, mi.config.stanc_options
     )
     set_up_output_dir(output_dir, mi)
     return model.sample(
         output_dir=output_dir,
         iter_sampling=n,
         data=os.path.join(output_dir, "input_data_train.json"),
         inits=os.path.join(output_dir, "inits.json"),
@@ -133,18 +165,16 @@
 
     :param mi: a MaudInput object
     :param output_dir: a string specifying where to save the output.
     """
     mi_options = (
         {} if mi.config.optimize_options is None else mi.config.optimize_options
     )
-    model = cmdstanpy.CmdStanModel(
-        stan_file=os.path.join(HERE, STAN_PROGRAM_RELATIVE_PATH),
-        cpp_options=mi.config.cpp_options,
-        stanc_options=mi.config.stanc_options,
+    model = load_stan_model(
+        "model", mi.config.cpp_options, mi.config.stanc_options
     )
     set_up_output_dir(output_dir, mi)
     return model.optimize(
         data=os.path.join(output_dir, "input_data_train.json"),
         inits=os.path.join(output_dir, "inits.json"),
         output_dir=output_dir,
         **{
@@ -172,18 +202,16 @@
 ) -> az.InferenceData:
     """Call CmdStanModel.sample for out of sample predictions.
 
     :param mi: a MaudInput object
     :param output_dir: directory where output will be saved
     :param idata_train: InferenceData object with posterior draws
     """
-    model = cmdstanpy.CmdStanModel(
-        stan_file=os.path.join(HERE, STAN_PROGRAM_RELATIVE_PATH_PREDICT),
-        cpp_options=mi.config.cpp_options,
-        stanc_options=mi.config.stanc_options,
+    model = load_stan_model(
+        "out_of_sample_model", mi.config.cpp_options, mi.config.stanc_options
     )
     set_up_output_dir(output_dir, mi)
     kinetic_parameters = [
         "keq",
         "km",
         "kcat",
         "dissociation_constant",
```

### Comparing `maud-metabolic-models-0.5.1.1/src/maud/stan/functions.stan` & `maud-metabolic-models-0.6.0.0/maud/stan/functions.stan`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 functions {
   vector unz_1d(vector[] mnsd, vector z){
-    /* 
+    /*
       Recover a real-valued vector from a 1xn vector z of z scores and a 2xn
       array mnsd of vectors consisting of the mean and standard deviation of
-      each element. 
+      each element.
     */
     return mnsd[1] + mnsd[2] .* z;
   }
 
   vector unz_log_1d(vector[] mnsd, vector z){
-    /* 
+    /*
       Recover a positive-constrained vector from a 1xn vector z of z scores and
       a 2xn array mnsd of vectors consisting of the lognormal mean and standard
-      deviation of each element. 
+      deviation of each element.
     */
     return exp(mnsd[1] + mnsd[2] .* z);
   }
 
   vector[] unz_2d(vector[,] mnsd, vector[] z){
     /*
       Recover a mxn array of real-valued vectors from an mxn array z of vectors
```

### Comparing `maud-metabolic-models-0.5.1.1/src/maud/stan/model.stan` & `maud-metabolic-models-0.6.0.0/maud/stan/model.stan`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
   array[2] vector[N_experiment_train] priors_psi_train;
   array[2, N_experiment_train] vector[N_pme] priors_conc_pme_train;
   array[2, N_experiment_train] vector[N_unbalanced] priors_conc_unbalanced_train;
   array[2, N_experiment_train] vector[N_enzyme] priors_conc_enzyme_train;
   array[2, N_experiment_train] vector[N_drain] priors_drain_train;
   // configuration
   array[N_experiment_train] vector<lower=0>[N_mic-N_unbalanced] conc_init;
-  real rel_tol; 
+  real rel_tol;
   real abs_tol;
   real steady_state_threshold_abs;
   real steady_state_threshold_rel;
   int max_num_steps;
   int<lower=0,upper=1> likelihood;  // set to 0 for priors-only mode
   real drain_small_conc_corrector;
   real<lower=0> timepoint;
@@ -154,15 +154,15 @@
       conc_pme_experiment[pko_experiment] = rep_vector(0, N_pko_experiment);
     }
     conc_balanced_experiment =
       ode_bdf_tol(dbalanced_dt,
                   conc_init[e],
                   initial_time,
                   {timepoint},
-                  rel_tol, 
+                  rel_tol,
                   abs_tol,
                   max_num_steps,
                   conc_unbalanced_train[e],
                   balanced_mic_ix,
                   unbalanced_mic_ix,
                   conc_enzyme_experiment,
                   dgr_train[e],
```

### Comparing `maud-metabolic-models-0.5.1.1/src/maud/stan/out_of_sample_model.stan` & `maud-metabolic-models-0.6.0.0/maud/stan/out_of_sample_model.stan`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
   // hardcoded priors
   array[2, N_experiment_test] vector[N_pme] priors_conc_phos_test;
   array[2, N_experiment_test] vector[N_unbalanced] priors_conc_unbalanced_test;
   array[2, N_experiment_test] vector[N_enzyme] priors_conc_enzyme_test;
   array[2, N_experiment_test] vector[N_drain] priors_drain_test;
   // configuration
   array[N_experiment_test] vector<lower=0>[N_mic-N_unbalanced] conc_init;
-  real rel_tol; 
+  real rel_tol;
   real abs_tol;
   int max_num_steps;
   int<lower=0,upper=1> likelihood;  // set to 0 for priors-only mode
   real drain_small_conc_corrector;
   real<lower=0> timepoint;
 }
 transformed data {
@@ -95,15 +95,15 @@
   array[N_experiment_test] vector[N_edge] saturation_test;
   array[N_experiment_test] vector[N_edge] allostery_test;
   array[N_experiment_test] vector[N_edge] phosphorylation_test;
   array[N_experiment_test] vector[N_edge] reversibility_test;
   // Sampling experiment boundary conditions from priors
   for (e in 1:N_experiment_test){
     drain_test[e] = to_vector(normal_rng(priors_drain_test[1,e], priors_drain_test[2,e]));
-    conc_pme_test[e] = to_vector(lognormal_rng(log(priors_conc_pme_test[1,e]), priors_conc_pme_test[2,e]));
+    conc_pme_test[e] = to_vector(lognormal_rng(log(priors_conc_phos_test[1,e]), priors_conc_phos_test[2,e]));
     conc_unbalanced_test[e] = to_vector(lognormal_rng(log(priors_conc_unbalanced_test[1,e]), priors_conc_unbalanced_test[2,e]));
     conc_enzyme_test[e] = to_vector(lognormal_rng(log(priors_conc_enzyme_test[1,e]), priors_conc_enzyme_test[2,e]));
   }
   // Simulation of experiments
   for (e in 1:N_experiment_test){
     flux_test[e] = rep_vector(0, N_reaction);
     vector[N_enzyme] conc_enzyme_experiment = conc_enzyme_test[e];
@@ -122,15 +122,15 @@
       conc_pme_experiment[pko_experiment] = rep_vector(0, N_pko_experiment);
     }
     conc_balanced_experiment =
       ode_bdf_tol(dbalanced_dt,
                   conc_init[e, balanced_mic_ix],
                   initial_time,
                   {timepoint},
-                  rel_tol, 
+                  rel_tol,
                   abs_tol,
                   max_num_steps,
                   conc_unbalanced_test[e],
                   balanced_mic_ix,
                   unbalanced_mic_ix,
                   conc_enzyme_experiment,
                   dgr_test[e],
@@ -138,15 +138,15 @@
                   km,
                   ki,
                   transfer_constant,
                   dissociation_constant,
                   kcat_pme,
                   conc_pme_experiment,
                   drain_test[e],
-                  temperature_train[e],
+                  temperature_test[e],
                   drain_small_conc_corrector,
                   S,
                   subunits,
                   edge_type,
                   edge_to_enzyme,
                   edge_to_drain,
                   ci_mic_ix,
@@ -178,15 +178,15 @@
                                              km,
                                              ki,
                                              transfer_constant,
                                              dissociation_constant,
                                              kcat_pme,
                                              conc_pme_experiment,
                                              drain_test[e],
-                                             temperature_train[e],
+                                             temperature_test[e],
                                              drain_small_conc_corrector,
                                              S,
                                              subunits,
                                              edge_type,
                                              edge_to_enzyme,
                                              edge_to_drain,
                                              ci_mic_ix,
@@ -251,10 +251,10 @@
     phosphorylation_test[e] = get_phosphorylation(kcat_pme,
                                              conc_pme_test[e],
                                              phosphorylation_ix_long,
                                              phosphorylation_ix_bounds,
                                              phosphorylation_type,
                                              phosphorylation_pme,
                                              subunits);
-    reversibility_test[e] = get_reversibility(dgr_test[e], temperature_train[e], S, conc_test[e], edge_type);
+    reversibility_test[e] = get_reversibility(dgr_test[e], temperature_test[e], S, conc_test[e], edge_type);
   }
 }
```

### Comparing `maud-metabolic-models-0.5.1.1/src/maud/utils.py` & `maud-metabolic-models-0.6.0.0/maud/utility_functions.py`

 * *Files identical despite different names*

