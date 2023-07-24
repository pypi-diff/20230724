# Comparing `tmp/adafruit-circuitpython-dash-display-1.1.9.tar.gz` & `tmp/adafruit-circuitpython-dash-display-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-dash-display-1.1.9.tar", last modified: Fri Jul 22 16:48:46 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-dash-display-2.0.0.tar", last modified: Mon Jul 24 14:21:10 2023, max compression
```

## Comparing `adafruit-circuitpython-dash-display-1.1.9.tar` & `adafruit-circuitpython-dash-display-2.0.0.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:48:46.906015 adafruit-circuitpython-dash-display-1.1.9/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:48:46.882013 adafruit-circuitpython-dash-display-1.1.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:48:46.890014 adafruit-circuitpython-dash-display-1.1.9/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:48:46.894014 adafruit-circuitpython-dash-display-1.1.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2725 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16292 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:48:46.894014 adafruit-circuitpython-dash-display-1.1.9/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5162 2022-07-22 16:48:46.906015 adafruit-circuitpython-dash-display-1.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4419 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:48:46.894014 adafruit-circuitpython-dash-display-1.1.9/adafruit_circuitpython_dash_display.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5162 2022-07-22 16:48:46.000000 adafruit-circuitpython-dash-display-1.1.9/adafruit_circuitpython_dash_display.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1453 2022-07-22 16:48:46.000000 adafruit-circuitpython-dash-display-1.1.9/adafruit_circuitpython_dash_display.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-22 16:48:46.000000 adafruit-circuitpython-dash-display-1.1.9/adafruit_circuitpython_dash_display.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-07-22 16:48:46.000000 adafruit-circuitpython-dash-display-1.1.9/adafruit_circuitpython_dash_display.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-07-22 16:48:46.000000 adafruit-circuitpython-dash-display-1.1.9/adafruit_circuitpython_dash_display.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     9775 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/adafruit_dash_display.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:48:46.898014 adafruit-circuitpython-dash-display-1.1.9/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:48:46.902014 adafruit-circuitpython-dash-display-1.1.9/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      298 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5846 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      408 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1206 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:48:46.902014 adafruit-circuitpython-dash-display-1.1.9/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     5484 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/examples/dash_display_advancedtest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:48:46.906015 adafruit-circuitpython-dash-display-1.1.9/examples/dash_display_client_examples/
--rw-r--r--   0 runner    (1001) docker     (121)     3289 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/examples/dash_display_client_examples/battery_daughter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2099 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/examples/dash_display_client_examples/door_daughter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2478 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/examples/dash_display_client_examples/neopixel_daughter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1852 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/examples/dash_display_client_examples/neopixel_setter.py
--rw-r--r--   0 runner    (1001) docker     (121)     3674 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/examples/dash_display_client_examples/neopixel_setter_daughter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2384 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/examples/dash_display_client_examples/relay_daughter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2429 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/examples/dash_display_client_examples/relay_hi_daughter.py
--rw-r--r--   0 runner    (1001) docker     (121)     4048 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/examples/dash_display_client_examples/temp_humid_daughter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2324 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/examples/dash_display_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-22 16:48:46.906015 adafruit-circuitpython-dash-display-1.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1944 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:21:10.462317 adafruit-circuitpython-dash-display-2.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:21:10.454317 adafruit-circuitpython-dash-display-2.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:21:10.458317 adafruit-circuitpython-dash-display-2.0.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-24 14:20:50.000000 adafruit-circuitpython-dash-display-2.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:21:10.458317 adafruit-circuitpython-dash-display-2.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-24 14:20:50.000000 adafruit-circuitpython-dash-display-2.0.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-24 14:20:50.000000 adafruit-circuitpython-dash-display-2.0.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-24 14:20:50.000000 adafruit-circuitpython-dash-display-2.0.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-24 14:20:50.000000 adafruit-circuitpython-dash-display-2.0.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-24 14:20:50.000000 adafruit-circuitpython-dash-display-2.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-24 14:20:50.000000 adafruit-circuitpython-dash-display-2.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-07-24 14:20:50.000000 adafruit-circuitpython-dash-display-2.0.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-24 14:20:50.000000 adafruit-circuitpython-dash-display-2.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-07-24 14:20:50.000000 adafruit-circuitpython-dash-display-2.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-24 14:20:50.000000 adafruit-circuitpython-dash-display-2.0.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:21:10.458317 adafruit-circuitpython-dash-display-2.0.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-07-24 14:20:50.000000 adafruit-circuitpython-dash-display-2.0.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-24 14:20:50.000000 adafruit-circuitpython-dash-display-2.0.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-24 14:20:50.000000 adafruit-circuitpython-dash-display-2.0.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-07-24 14:21:10.462317 adafruit-circuitpython-dash-display-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-07-24 14:20:50.000000 adafruit-circuitpython-dash-display-2.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-24 14:20:50.000000 adafruit-circuitpython-dash-display-2.0.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:21:10.458317 adafruit-circuitpython-dash-display-2.0.0/adafruit_circuitpython_dash_display.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-07-24 14:21:10.000000 adafruit-circuitpython-dash-display-2.0.0/adafruit_circuitpython_dash_display.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-24 14:21:10.000000 adafruit-circuitpython-dash-display-2.0.0/adafruit_circuitpython_dash_display.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 14:21:10.000000 adafruit-circuitpython-dash-display-2.0.0/adafruit_circuitpython_dash_display.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 14:21:10.000000 adafruit-circuitpython-dash-display-2.0.0/adafruit_circuitpython_dash_display.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 14:21:10.000000 adafruit-circuitpython-dash-display-2.0.0/adafruit_circuitpython_dash_display.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10637 2023-07-24 14:21:02.000000 adafruit-circuitpython-dash-display-2.0.0/adafruit_dash_display.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:21:10.462317 adafruit-circuitpython-dash-display-2.0.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:21:10.462317 adafruit-circuitpython-dash-display-2.0.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-24 14:20:50.000000 adafruit-circuitpython-dash-display-2.0.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-24 14:20:50.000000 adafruit-circuitpython-dash-display-2.0.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-24 14:20:50.000000 adafruit-circuitpython-dash-display-2.0.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-24 14:20:50.000000 adafruit-circuitpython-dash-display-2.0.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-07-24 14:20:50.000000 adafruit-circuitpython-dash-display-2.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-24 14:20:50.000000 adafruit-circuitpython-dash-display-2.0.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-24 14:20:50.000000 adafruit-circuitpython-dash-display-2.0.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-24 14:20:50.000000 adafruit-circuitpython-dash-display-2.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-24 14:20:50.000000 adafruit-circuitpython-dash-display-2.0.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-24 14:20:50.000000 adafruit-circuitpython-dash-display-2.0.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:21:10.462317 adafruit-circuitpython-dash-display-2.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-07-24 14:21:02.000000 adafruit-circuitpython-dash-display-2.0.0/examples/dash_display_advancedtest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:21:10.462317 adafruit-circuitpython-dash-display-2.0.0/examples/dash_display_client_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-07-24 14:21:02.000000 adafruit-circuitpython-dash-display-2.0.0/examples/dash_display_client_examples/battery_daughter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-24 14:21:02.000000 adafruit-circuitpython-dash-display-2.0.0/examples/dash_display_client_examples/door_daughter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-07-24 14:21:02.000000 adafruit-circuitpython-dash-display-2.0.0/examples/dash_display_client_examples/neopixel_daughter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-24 14:21:02.000000 adafruit-circuitpython-dash-display-2.0.0/examples/dash_display_client_examples/neopixel_setter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-07-24 14:21:02.000000 adafruit-circuitpython-dash-display-2.0.0/examples/dash_display_client_examples/neopixel_setter_daughter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-07-24 14:21:02.000000 adafruit-circuitpython-dash-display-2.0.0/examples/dash_display_client_examples/relay_daughter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-24 14:21:02.000000 adafruit-circuitpython-dash-display-2.0.0/examples/dash_display_client_examples/relay_hi_daughter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-07-24 14:21:02.000000 adafruit-circuitpython-dash-display-2.0.0/examples/dash_display_client_examples/temp_humid_daughter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-07-24 14:21:02.000000 adafruit-circuitpython-dash-display-2.0.0/examples/dash_display_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-24 14:20:50.000000 adafruit-circuitpython-dash-display-2.0.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-24 14:21:02.000000 adafruit-circuitpython-dash-display-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-24 14:20:50.000000 adafruit-circuitpython-dash-display-2.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 14:21:10.462317 adafruit-circuitpython-dash-display-2.0.0/setup.cfg
```

### Comparing `adafruit-circuitpython-dash-display-1.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-dash-display-2.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dash-display-1.1.9/.gitignore` & `adafruit-circuitpython-dash-display-2.0.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 _build
 
 # This file results from running `pip -e install .` in a local repository
 *.egg-info
 
 # Virtual environment-specific files
 .env
+.venv
 
 # MacOS-specific files
 *.DS_Store
 
 # IDE-specific files
 .idea
 .vscode
```

### Comparing `adafruit-circuitpython-dash-display-1.1.9/.pre-commit-config.yaml` & `adafruit-circuitpython-dash-display-2.0.0/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
   - repo: https://github.com/python/black
-    rev: 22.3.0
+    rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/fsfe/reuse-tool
-    rev: v0.14.0
+    rev: v1.1.2
     hooks:
       - id: reuse
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.2.0
+    rev: v4.4.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/pylint
-    rev: v2.11.1
+    rev: v2.17.4
     hooks:
       - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
```

### Comparing `adafruit-circuitpython-dash-display-1.1.9/.pylintrc` & `adafruit-circuitpython-dash-display-2.0.0/.pylintrc`

 * *Files 24% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 #init-hook=
 
 # Use multiple processes to speed up Pylint.
 jobs=1
 
 # List of plugins (as comma separated values of python modules names) to load,
 # usually to register additional checkers.
-load-plugins=
+load-plugins=pylint.extensions.no_self_use
 
 # Pickle collected data for later comparisons.
 persistent=yes
 
 # Specify a configuration file.
 #rcfile=
 
@@ -50,16 +50,16 @@
 # option multiple times (only on the command line, not in the configuration
 # file where it should appear only once).You can also use "--disable=all" to
 # disable everything first and then reenable specific checks. For example, if
 # you want to run only the similarities checker, you can use "--disable=all
 # --enable=similarities". If you want to run only the classes checker, but have
 # no Warning level messages displayed, use"--disable=all --enable=classes
 # --disable=W"
-# disable=import-error,print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call
-disable=print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call,import-error,bad-continuation,pointless-string-statement,unspecified-encoding
+# disable=import-error,raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,deprecated-str-translate-call
+disable=raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,import-error,pointless-string-statement,unspecified-encoding
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where
 # it should appear only once). See also the "--disable" option for examples.
 enable=
 
@@ -221,20 +221,14 @@
 
 # Maximum number of characters on a single line.
 max-line-length=100
 
 # Maximum number of lines in a module
 max-module-lines=1000
 
-# List of optional constructs for which whitespace checking is disabled. `dict-
-# separator` is used to allow tabulation in dicts, etc.: {1  : 1,\n222: 2}.
-# `trailing-comma` allows a space between comma and closing bracket: (a, ).
-# `empty-line` allows space-only lines.
-no-space-check=trailing-comma,dict-separator
-
 # Allow the body of a class to be on the same line as the declaration if body
 # contains single statement.
 single-line-class-stmt=no
 
 # Allow the body of an if to be on the same line as the test if there is no
 # else.
 single-line-if-stmt=no
@@ -253,81 +247,53 @@
 
 # Minimum lines number of a similarity.
 min-similarity-lines=12
 
 
 [BASIC]
 
-# Naming hint for argument names
-argument-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct argument names
 argument-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for attribute names
-attr-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct attribute names
 attr-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Bad variable names which should always be refused, separated by a comma
 bad-names=foo,bar,baz,toto,tutu,tata
 
-# Naming hint for class attribute names
-class-attribute-name-hint=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
-
 # Regular expression matching correct class attribute names
 class-attribute-rgx=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
 
-# Naming hint for class names
-# class-name-hint=[A-Z_][a-zA-Z0-9]+$
-class-name-hint=[A-Z_][a-zA-Z0-9_]+$
-
 # Regular expression matching correct class names
 # class-rgx=[A-Z_][a-zA-Z0-9]+$
 class-rgx=[A-Z_][a-zA-Z0-9_]+$
 
-# Naming hint for constant names
-const-name-hint=(([A-Z_][A-Z0-9_]*)|(__.*__))$
-
 # Regular expression matching correct constant names
 const-rgx=(([A-Z_][A-Z0-9_]*)|(__.*__))$
 
 # Minimum line length for functions/classes that require docstrings, shorter
 # ones are exempt.
 docstring-min-length=-1
 
-# Naming hint for function names
-function-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct function names
 function-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Good variable names which should always be accepted, separated by a comma
 # good-names=i,j,k,ex,Run,_
 good-names=r,g,b,w,i,j,k,n,x,y,z,ex,ok,Run,_
 
 # Include a hint for the correct naming format with invalid-name
 include-naming-hint=no
 
-# Naming hint for inline iteration names
-inlinevar-name-hint=[A-Za-z_][A-Za-z0-9_]*$
-
 # Regular expression matching correct inline iteration names
 inlinevar-rgx=[A-Za-z_][A-Za-z0-9_]*$
 
-# Naming hint for method names
-method-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct method names
 method-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for module names
-module-name-hint=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
-
 # Regular expression matching correct module names
 module-rgx=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
 
 # Colon-delimited sets of names that determine each other's naming style when
 # the name regexes allow several styles.
 name-group=
 
@@ -335,17 +301,14 @@
 # not require a docstring.
 no-docstring-rgx=^_
 
 # List of decorators that produce properties, such as abc.abstractproperty. Add
 # to this list to register other decorators that produce valid properties.
 property-classes=abc.abstractproperty
 
-# Naming hint for variable names
-variable-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct variable names
 variable-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 
 [IMPORTS]
 
 # Allow wildcard imports from modules that define __all__.
@@ -429,8 +392,8 @@
 min-public-methods=1
 
 
 [EXCEPTIONS]
 
 # Exceptions that will emit a warning when being caught. Defaults to
 # "Exception"
-overgeneral-exceptions=Exception
+overgeneral-exceptions=builtins.Exception
```

### Comparing `adafruit-circuitpython-dash-display-1.1.9/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-dash-display-2.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dash-display-1.1.9/LICENSE` & `adafruit-circuitpython-dash-display-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dash-display-1.1.9/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-dash-display-2.0.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dash-display-1.1.9/LICENSES/MIT.txt` & `adafruit-circuitpython-dash-display-2.0.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dash-display-1.1.9/LICENSES/Unlicense.txt` & `adafruit-circuitpython-dash-display-2.0.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dash-display-1.1.9/PKG-INFO` & `adafruit-circuitpython-dash-display-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-dash-display
-Version: 1.1.9
+Version: 2.0.0
 Summary: CircuitPython library for creating Adafruit IO dashboards.
-Home-page: https://github.com/adafruit/Adafruit_CircuitPython_Dash_Display
-Author: Adafruit Industries
-Author-email: circuitpython@adafruit.com
+Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
-Keywords: adafruit displays iot adafruitio hardware micropythoncircuitpython
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Dash_Display
+Keywords: adafruit,displays,iot,adafruitio,hardware,micropythoncircuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
+Provides-Extra: optional
 License-File: LICENSE
 
 Introduction
 ============
 
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-dash_display/badge/?version=latest
@@ -161,9 +160,7 @@
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_Dash_Display/blob/HEAD/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-
```

### Comparing `adafruit-circuitpython-dash-display-1.1.9/README.rst` & `adafruit-circuitpython-dash-display-2.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dash-display-1.1.9/adafruit_circuitpython_dash_display.egg-info/PKG-INFO` & `adafruit-circuitpython-dash-display-2.0.0/adafruit_circuitpython_dash_display.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-dash-display
-Version: 1.1.9
+Version: 2.0.0
 Summary: CircuitPython library for creating Adafruit IO dashboards.
-Home-page: https://github.com/adafruit/Adafruit_CircuitPython_Dash_Display
-Author: Adafruit Industries
-Author-email: circuitpython@adafruit.com
+Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
-Keywords: adafruit displays iot adafruitio hardware micropythoncircuitpython
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Dash_Display
+Keywords: adafruit,displays,iot,adafruitio,hardware,micropythoncircuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
+Provides-Extra: optional
 License-File: LICENSE
 
 Introduction
 ============
 
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-dash_display/badge/?version=latest
@@ -161,9 +160,7 @@
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_Dash_Display/blob/HEAD/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-
```

### Comparing `adafruit-circuitpython-dash-display-1.1.9/adafruit_circuitpython_dash_display.egg-info/SOURCES.txt` & `adafruit-circuitpython-dash-display-2.0.0/adafruit_circuitpython_dash_display.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 .pylintrc
 .readthedocs.yaml
 CODE_OF_CONDUCT.md
 LICENSE
 README.rst
 README.rst.license
 adafruit_dash_display.py
+optional_requirements.txt
 pyproject.toml
 requirements.txt
-setup.py
 .github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
 .github/workflows/failure-help-text.yml
-.github/workflows/release.yml
+.github/workflows/release_gh.yml
+.github/workflows/release_pypi.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
 adafruit_circuitpython_dash_display.egg-info/PKG-INFO
 adafruit_circuitpython_dash_display.egg-info/SOURCES.txt
 adafruit_circuitpython_dash_display.egg-info/dependency_links.txt
 adafruit_circuitpython_dash_display.egg-info/requires.txt
```

### Comparing `adafruit-circuitpython-dash-display-1.1.9/adafruit_dash_display.py` & `adafruit-circuitpython-dash-display-2.0.0/adafruit_dash_display.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,31 +18,44 @@
 
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 
 """
+try:
+    from typing import Tuple, Callable, Optional, Any
+    from adafruit_io.adafruit_io import IO_MQTT
+    from digitalio import DigitalInOut
+except ImportError:
+    pass
 
 import time
 from collections import OrderedDict
-from adafruit_display_shapes.rect import Rect
-from adafruit_display_text.label import Label
 import displayio
 import terminalio
+from adafruit_display_shapes.rect import Rect
+from adafruit_display_text.label import Label
 
-__version__ = "0.0.0-auto.0"
+__version__ = "2.0.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Dash_Display.git"
 
 
 class Feed:
     """Feed object to make getting and setting different feed properties easier"""
 
     def __init__(
-        self, key, default_text, formatted_text, callback, color, pub, index
+        self,
+        key: str,
+        default_text: str,
+        formatted_text: str,
+        callback: Optional[Callable],
+        color: Optional[int],
+        pub: Optional[Callable],
+        index: int,
     ):  # pylint: disable=too-many-arguments
         self._key = key
         self.default_text = default_text
         self._text = formatted_text
         self._callback = callback
         self._color = color
         self._pub = pub
@@ -52,146 +65,157 @@
 
     @property
     def key(self):
         """Getter for feed key. Will give the value of the feed key"""
         return self._key
 
     @key.setter
-    def key(self, value):
+    def key(self, value: str):
         """Setter for feed key. Sets a new value for the feed key property _key"""
         self._key = value
 
     @property
     def text(self):
         """Getter for text ready to be formatted. Will give the feed text"""
         return self._text
 
     @text.setter
-    def text(self, value):
+    def text(self, value: str):
         """Setter for text ready to be formatted. Allows to change the feed text"""
         self._text = value
 
     @property
     def callback(self):
         """Getter for callback function. Returns the feed callback"""
         return self._callback
 
     @callback.setter
-    def callback(self, value):
+    def callback(self, value: Callable):
         """Setter for callback function. Changes the feed callback"""
         self._callback = value
 
     @property
     def color(self):
         """Getter for text color callback function. Will return the color for the feed"""
         return self._color
 
     @color.setter
-    def color(self, value):
+    def color(self, value: int):
         """Setter for text color callback function"""
         self._color = value
 
     @property
     def pub(self):
         """Getter for publish function, called when a new value is published by this library."""
         return self._pub
 
     @pub.setter
-    def pub(self, value):
+    def pub(self, value: Callable):
         """Setter for publish function"""
         self._pub = value
 
     @property
     def last_val(self):
         """Getter for the last value received"""
         return self._last_val
 
     @last_val.setter
-    def last_val(self, value):
+    def last_val(self, value: str):
         """Setter for last received value"""
         self._last_val = value
 
 
 class Hub:  # pylint: disable=too-many-instance-attributes
-    """Object that lets you make an IOT dashboard"""
+    """
+    Object that lets you make an IOT dashboard
+
+    :param displayio.Display display: The display for the dashboard.
+    :param IO_MQTT io_mqtt: MQTT communications object.
+    :param Tuple[DigitalInOut, ...] nav: The navigation pushbuttons.
+    """
 
-    def __init__(self, display, io, nav):
+    def __init__(
+        self,
+        display: displayio.Display,
+        io_mqtt: IO_MQTT,
+        nav: Tuple[DigitalInOut, ...],
+    ):
         self.display = display
 
-        self.io = io  # pylint: disable=invalid-name
+        self.io_mqtt = io_mqtt
 
         self.up_btn, self.select, self.down, self.back, self.submit = nav
 
         self.length = 0
         self.selected = 1
 
         self.feeds = OrderedDict()
 
-        self.io.on_mqtt_connect = self.connected
-        self.io.on_mqtt_disconnect = self.disconnected
-        self.io.on_mqtt_subscribe = self.subscribe
-        self.io.on_message = self.message
+        self.io_mqtt.on_mqtt_connect = self.connected
+        self.io_mqtt.on_mqtt_disconnect = self.disconnected
+        self.io_mqtt.on_mqtt_subscribe = self.subscribe
+        self.io_mqtt.on_message = self.message
 
         print("Connecting to Adafruit IO...")
-        io.connect()
+        io_mqtt.connect()
 
         self.display.show(None)
 
         self.splash = displayio.Group()
 
         self.rect = Rect(0, 0, 240, 30, fill=0xFFFFFF)
         self.splash.append(self.rect)
 
         self.display.show(self.splash)
 
     def simple_text_callback(
-        self, client, feed_id, message
+        self, client: IO_MQTT, feed_id: str, message: str
     ):  # pylint: disable=unused-argument
         """Default callback function that uses the text in the Feed object and the color callback
         to set the text"""
         feed_id = feed_id.split("/")[-1]
         feed = self.feeds[feed_id]
         try:
             text = feed.text.format(message)
         except ValueError:
             text = feed.text.format(float(message))
         return text
 
-    def update_text(self, client, feed_id, message):
+    def update_text(self, client: IO_MQTT, feed_id: str, message: str):
         """Updates the text on the display"""
         feed = self.feeds[feed_id]
         feed.callback(client, feed_id, message)
         self.splash[feed.index + 1].text = feed.callback(client, feed_id, str(message))
         if feed.color:
             self.splash[feed.index + 1].color = feed.color(message)
 
-    def base_pub(self, var):
+    def base_pub(self, var: Any):
         """Default function called when a feed is published to"""
 
     def add_device(
         self,
-        feed_key,
-        default_text=None,
-        formatted_text=None,
-        color_callback=None,
-        callback=None,
-        pub_method=None,
+        feed_key: str,
+        default_text: Optional[str] = None,
+        formatted_text: Optional[str] = None,
+        color_callback: Optional[int] = None,
+        callback: Optional[Callable] = None,
+        pub_method: Optional[Callable] = None,
     ):  # pylint: disable=too-many-arguments
         """Adds a feed/device to the UI"""
         if not callback:
             callback = self.simple_text_callback
         if not pub_method:
             pub_method = self.base_pub
         if not formatted_text:
             formatted_text = f"{feed_key} : "
             formatted_text = formatted_text + "{}"
         if not default_text:
             default_text = feed_key
 
-        self.io.subscribe(feed_key)
+        self.io_mqtt.subscribe(feed_key)
         if len(self.splash) == 1:
             self.splash.append(
                 Label(
                     font=terminalio.FONT,
                     text=default_text,
                     x=3,
                     y=15,
@@ -223,50 +247,50 @@
             index=len(self.feeds),
         )
 
     def get(self):
         """Gets all the subscribed feeds"""
         for feed in self.feeds.keys():
             print(f"getting {feed}")
-            self.io.get(feed)
+            self.io_mqtt.get(feed)
             time.sleep(0.1)
-        self.io.loop()
+        self.io_mqtt.loop()
 
     # pylint: disable=unused-argument
     @staticmethod
-    def connected(client):
+    def connected(client: IO_MQTT):
         """Callback for when the device is connected to Adafruit IO"""
         print("Connected to Adafruit IO!")
 
     @staticmethod
-    def subscribe(client, userdata, topic, granted_qos):
+    def subscribe(client: IO_MQTT, userdata: Any, topic: str, granted_qos: str):
         """Callback for when a new feed is subscribed to"""
-        print("Subscribed to {0} with QOS level {1}".format(topic, granted_qos))
+        print(f"Subscribed to {topic} with QOS level {granted_qos}")
 
     @staticmethod
-    def disconnected(client):
+    def disconnected(client: IO_MQTT):
         """Callback for when the device disconnects from Adafruit IO"""
         print("Disconnected from Adafruit IO!")
 
-    def message(self, client, feed_id, message):
+    def message(self, client: IO_MQTT, feed_id: str, message: str):
         """Callback for whenever a new message is received"""
-        print("Feed {0} received new value: {1}".format(feed_id, message))
+        print(f"Feed {feed_id} received new value: {message}")
         feed_id = feed_id.split("/")[-1]
         feed = self.feeds[feed_id]
         feed.last_val = message
         self.update_text(client, feed_id, str(message))
 
-    def publish(self, feed, message):
+    def publish(self, feed: Feed, message: str):
         """Callback for publishing a message"""
         print(f"Publishing {message} to {feed}")
-        self.io.publish(feed, message)
+        self.io_mqtt.publish(feed, message)
 
     def loop(self):
         """Loops Adafruit IO and also checks to see if any buttons have been pressed"""
-        self.io.loop()
+        self.io_mqtt.loop()
         if self.select.value:
             feed = self.feeds[list(self.feeds.keys())[self.selected - 1]]
             if feed.pub:
                 feed.pub(feed.last_val)
                 self.display.show(self.splash)
             while self.select.value:
                 pass
```

### Comparing `adafruit-circuitpython-dash-display-1.1.9/docs/_static/favicon.ico` & `adafruit-circuitpython-dash-display-2.0.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dash-display-1.1.9/docs/conf.py` & `adafruit-circuitpython-dash-display-2.0.0/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 
 # SPDX-FileCopyrightText: 2017 Scott Shawcroft, written for Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import sys
+import datetime
 
 sys.path.insert(0, os.path.abspath(".."))
 
 # -- General configuration ------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx.ext.autodoc",
+    "sphinxcontrib.jquery",
     "sphinx.ext.intersphinx",
     "sphinx.ext.napoleon",
     "sphinx.ext.todo",
 ]
 
 # TODO: Please Read!
 # Uncomment the below if you use native CircuitPython modules such as
@@ -48,15 +50,22 @@
 source_suffix = ".rst"
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "Adafruit  CircuitPython Dash_Display Library"
-copyright = "2021 Eva Herrada for Adafruit Industries"
+creation_year = "2021"
+current_year = str(datetime.datetime.now().year)
+year_duration = (
+    current_year
+    if current_year == creation_year
+    else creation_year + " - " + current_year
+)
+copyright = year_duration + " Eva Herrada for Adafruit Industries"
 author = "Eva Herrada"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
```

### Comparing `adafruit-circuitpython-dash-display-1.1.9/docs/index.rst` & `adafruit-circuitpython-dash-display-2.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dash-display-1.1.9/examples/dash_display_advancedtest.py` & `adafruit-circuitpython-dash-display-2.0.0/examples/dash_display_advancedtest.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,15 +192,15 @@
     socket_pool=pool,
     ssl_context=ssl.create_default_context(),
 )
 
 # Initialize an Adafruit IO MQTT Client
 io = IO_MQTT(mqtt_client)
 
-iot = Hub(display=display, io=io, nav=(up, select, down, back, submit))
+iot = Hub(display=display, io_mqtt=io, nav=(up, select, down, back, submit))
 
 iot.add_device(
     feed_key="lamp",
     default_text="Lamp: ",
     formatted_text="Lamp: {}",
     pub_method=pub_lamp,
 )
```

### Comparing `adafruit-circuitpython-dash-display-1.1.9/examples/dash_display_client_examples/battery_daughter.py` & `adafruit-circuitpython-dash-display-2.0.0/examples/dash_display_client_examples/battery_daughter.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 esp = adafruit_esp32spi.ESP_SPIcontrol(spi, esp32_cs, esp32_ready, esp32_reset)
 """Use below for Most Boards"""
 status_light = neopixel.NeoPixel(
     board.NEOPIXEL, 1, brightness=0.2
 )  # Uncomment for Most Boards
 wifi = adafruit_esp32spi_wifimanager.ESPSPI_WiFiManager(esp, secrets, status_light)
 
+
 # Define callback functions which will be called when certain events happen.
 # pylint: disable=unused-argument
 def connected(client):
     client.subscribe("battery")
 
 
 def subscribe(client, userdata, topic, granted_qos):
```

### Comparing `adafruit-circuitpython-dash-display-1.1.9/examples/dash_display_client_examples/door_daughter.py` & `adafruit-circuitpython-dash-display-2.0.0/examples/dash_display_client_examples/door_daughter.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dash-display-1.1.9/examples/dash_display_client_examples/neopixel_daughter.py` & `adafruit-circuitpython-dash-display-2.0.0/examples/dash_display_client_examples/neopixel_daughter.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 esp = adafruit_esp32spi.ESP_SPIcontrol(spi, esp32_cs, esp32_ready, esp32_reset)
 """Use below for Most Boards"""
 status_light = neopixel.NeoPixel(
     board.NEOPIXEL, 1, brightness=0.2
 )  # Uncomment for Most Boards
 wifi = adafruit_esp32spi_wifimanager.ESPSPI_WiFiManager(esp, secrets, status_light)
 
+
 # Define callback functions which will be called when certain events happen.
 # pylint: disable=unused-argument
 def connected(client):
     client.subscribe("neopixel")
 
 
 def subscribe(client, userdata, topic, granted_qos):
```

### Comparing `adafruit-circuitpython-dash-display-1.1.9/examples/dash_display_client_examples/neopixel_setter.py` & `adafruit-circuitpython-dash-display-2.0.0/examples/dash_display_client_examples/neopixel_setter.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dash-display-1.1.9/examples/dash_display_client_examples/neopixel_setter_daughter.py` & `adafruit-circuitpython-dash-display-2.0.0/examples/dash_display_client_examples/neopixel_setter_daughter.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dash-display-1.1.9/examples/dash_display_client_examples/relay_daughter.py` & `adafruit-circuitpython-dash-display-2.0.0/examples/dash_display_client_examples/relay_daughter.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 esp = adafruit_esp32spi.ESP_SPIcontrol(spi, esp32_cs, esp32_ready, esp32_reset)
 """Use below for Most Boards"""
 status_light = neopixel.NeoPixel(
     board.NEOPIXEL, 1, brightness=0.2
 )  # Uncomment for Most Boards
 wifi = adafruit_esp32spi_wifimanager.ESPSPI_WiFiManager(esp, secrets, status_light)
 
+
 # Define callback functions which will be called when certain events happen.
 # pylint: disable=unused-argument
 def connected(client):
     client.subscribe("lamp")
 
 
 def subscribe(client, userdata, topic, granted_qos):
```

### Comparing `adafruit-circuitpython-dash-display-1.1.9/examples/dash_display_client_examples/relay_hi_daughter.py` & `adafruit-circuitpython-dash-display-2.0.0/examples/dash_display_client_examples/relay_hi_daughter.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 esp = adafruit_esp32spi.ESP_SPIcontrol(spi, esp32_cs, esp32_ready, esp32_reset)
 """Use below for Most Boards"""
 status_light = neopixel.NeoPixel(
     board.NEOPIXEL, 1, brightness=0.2
 )  # Uncomment for Most Boards
 wifi = adafruit_esp32spi_wifimanager.ESPSPI_WiFiManager(esp, secrets, status_light)
 
+
 # Define callback functions which will be called when certain events happen.
 # pylint: disable=unused-argument
 def connected(client):
     client.subscribe("heatindex")
 
 
 def subscribe(client, userdata, topic, granted_qos):
```

### Comparing `adafruit-circuitpython-dash-display-1.1.9/examples/dash_display_client_examples/temp_humid_daughter.py` & `adafruit-circuitpython-dash-display-2.0.0/examples/dash_display_client_examples/temp_humid_daughter.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dash-display-1.1.9/examples/dash_display_simpletest.py` & `adafruit-circuitpython-dash-display-2.0.0/examples/dash_display_simpletest.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     if isinstance(lamp, str):
         lamp = eval(lamp)  # pylint: disable=eval-used
     iot.publish("lamp", str(not lamp))
     # funhouse.set_text(f"Lamp: {not lamp}", 0)
     time.sleep(0.3)
 
 
-iot = Hub(display=display, io=io, nav=(up, select, down, back, submit))
+iot = Hub(display=display, io_mqtt=io, nav=(up, select, down, back, submit))
 
 iot.add_device(
     feed_key="lamp",
     default_text="Lamp: ",
     formatted_text="Lamp: {}",
     pub_method=pub_lamp,
 )
```

