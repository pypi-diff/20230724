# Comparing `tmp/maestral-1.8.0.dev0.tar.gz` & `tmp/maestral-1.8.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maestral-1.8.0.dev0.tar", last modified: Sat Jul 22 15:24:25 2023, max compression
+gzip compressed data, was "maestral-1.8.0.dev1.tar", last modified: Mon Jul 24 18:51:27 2023, max compression
```

## Comparing `maestral-1.8.0.dev0.tar` & `maestral-1.8.0.dev1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:24:25.877261 maestral-1.8.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-07-22 15:24:25.877261 maestral-1.8.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 15:24:25.877261 maestral-1.8.0.dev0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:24:25.873261 maestral-1.8.0.dev0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:24:25.873261 maestral-1.8.0.dev0/src/maestral/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12863 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/autostart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:24:25.877261 maestral-1.8.0.dev0/src/maestral/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14787 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/cli/cli_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    10518 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/cli/cli_info.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1867 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/cli/cli_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    15396 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/cli/cli_maintenance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/cli/cli_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/cli/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/cli/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/cli/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/cli/output.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    69736 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:24:25.877261 maestral-1.8.0.dev0/src/maestral/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/config/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    17864 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/config/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    21989 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/daemon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:24:25.877261 maestral-1.8.0.dev0/src/maestral/database/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/database/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    17337 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/database/orm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/database/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/database/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    33650 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/errorhandling.py
--rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:24:25.877261 maestral-1.8.0.dev0/src/maestral/fsevents/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/fsevents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/fsevents/polling.py
--rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/keyring.py
--rw-r--r--   0 runner    (1001) docker     (123)     8819 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    63443 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    28502 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    18270 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/notify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:24:25.877261 maestral-1.8.0.dev0/src/maestral/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   137001 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/resources/maestral.png
--rw-r--r--   0 runner    (1001) docker     (123)   150874 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:24:25.877261 maestral-1.8.0.dev0/src/maestral/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/utils/appdirs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/utils/caches.py
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/utils/hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/utils/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    19452 2023-07-22 15:24:09.000000 maestral-1.8.0.dev0/src/maestral/utils/path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:24:25.873261 maestral-1.8.0.dev0/src/maestral.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-07-22 15:24:25.000000 maestral-1.8.0.dev0/src/maestral.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-22 15:24:25.000000 maestral-1.8.0.dev0/src/maestral.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 15:24:25.000000 maestral-1.8.0.dev0/src/maestral.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-22 15:24:25.000000 maestral-1.8.0.dev0/src/maestral.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-22 15:24:25.000000 maestral-1.8.0.dev0/src/maestral.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-22 15:24:25.000000 maestral-1.8.0.dev0/src/maestral.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:51:27.483572 maestral-1.8.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-07-24 18:51:27.483572 maestral-1.8.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 18:51:27.483572 maestral-1.8.0.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:51:27.467572 maestral-1.8.0.dev1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:51:27.475572 maestral-1.8.0.dev1/src/maestral/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12863 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/autostart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:51:27.479572 maestral-1.8.0.dev1/src/maestral/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14787 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/cli/cli_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10518 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/cli/cli_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1867 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/cli/cli_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15396 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/cli/cli_maintenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/cli/cli_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/cli/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/cli/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/cli/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/cli/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69736 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:51:27.479572 maestral-1.8.0.dev1/src/maestral/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/config/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17864 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/config/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21989 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/daemon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:51:27.479572 maestral-1.8.0.dev1/src/maestral/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/database/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17337 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/database/orm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/database/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/database/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33650 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/errorhandling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:51:27.479572 maestral-1.8.0.dev1/src/maestral/fsevents/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/fsevents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/fsevents/polling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/keyring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8819 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63443 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28502 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18270 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/notify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:51:27.479572 maestral-1.8.0.dev1/src/maestral/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   137001 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/resources/maestral.png
+-rw-r--r--   0 runner    (1001) docker     (123)   150874 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:51:27.483572 maestral-1.8.0.dev1/src/maestral/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/utils/appdirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/utils/caches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/utils/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/utils/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19452 2023-07-24 18:51:02.000000 maestral-1.8.0.dev1/src/maestral/utils/path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:51:27.475572 maestral-1.8.0.dev1/src/maestral.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-07-24 18:51:27.000000 maestral-1.8.0.dev1/src/maestral.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-24 18:51:27.000000 maestral-1.8.0.dev1/src/maestral.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:51:27.000000 maestral-1.8.0.dev1/src/maestral.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-24 18:51:27.000000 maestral-1.8.0.dev1/src/maestral.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-24 18:51:27.000000 maestral-1.8.0.dev1/src/maestral.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-24 18:51:27.000000 maestral-1.8.0.dev1/src/maestral.egg-info/top_level.txt
```

### Comparing `maestral-1.8.0.dev0/LICENSE.txt` & `maestral-1.8.0.dev1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maestral-1.8.0.dev0/PKG-INFO` & `maestral-1.8.0.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maestral
-Version: 1.8.0.dev0
+Version: 1.8.0.dev1
 Summary: Open-source Dropbox client for macOS and Linux.
 Author-email: Sam Schott <sam.schott@outlook.com>
 License: MIT
 Project-URL: Homepage, https://maestral.app
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
```

### Comparing `maestral-1.8.0.dev0/README.md` & `maestral-1.8.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `maestral-1.8.0.dev0/pyproject.toml` & `maestral-1.8.0.dev1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2", "build"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "maestral"
-version = "1.8.0.dev0"
+version = "1.8.0.dev1"
 authors = [{name = "Sam Schott", email = "sam.schott@outlook.com"}]
 license = {text = "MIT"}
 description = "Open-source Dropbox client for macOS and Linux."
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Operating System :: Unix",
     "Programming Language :: Python",
@@ -44,16 +44,16 @@
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
 [project.optional-dependencies]
 gui = [
-    "maestral-qt>=1.8.0.dev0;sys_platform=='linux'",
-    "maestral-cocoa>=1.8.0.dev0;sys_platform=='darwin'",
+    "maestral-qt>=1.8.0.dev1;sys_platform=='linux'",
+    "maestral-cocoa>=1.8.0.dev1;sys_platform=='darwin'",
 ]
 syslog = ["systemd-python"]
 lint = [
     "black",
     "flake8",
     "flake8-pyproject",
     "mypy",
```

### Comparing `maestral-1.8.0.dev0/src/maestral/autostart.py` & `maestral-1.8.0.dev1/src/maestral/autostart.py`

 * *Files identical despite different names*

### Comparing `maestral-1.8.0.dev0/src/maestral/cli/cli_core.py` & `maestral-1.8.0.dev1/src/maestral/cli/cli_core.py`

 * *Files identical despite different names*

### Comparing `maestral-1.8.0.dev0/src/maestral/cli/cli_info.py` & `maestral-1.8.0.dev1/src/maestral/cli/cli_info.py`

 * *Files identical despite different names*

### Comparing `maestral-1.8.0.dev0/src/maestral/cli/cli_main.py` & `maestral-1.8.0.dev1/src/maestral/cli/cli_main.py`

 * *Files identical despite different names*

### Comparing `maestral-1.8.0.dev0/src/maestral/cli/cli_maintenance.py` & `maestral-1.8.0.dev1/src/maestral/cli/cli_maintenance.py`

 * *Files identical despite different names*

### Comparing `maestral-1.8.0.dev0/src/maestral/cli/cli_settings.py` & `maestral-1.8.0.dev1/src/maestral/cli/cli_settings.py`

 * *Files identical despite different names*

### Comparing `maestral-1.8.0.dev0/src/maestral/cli/common.py` & `maestral-1.8.0.dev1/src/maestral/cli/common.py`

 * *Files identical despite different names*

### Comparing `maestral-1.8.0.dev0/src/maestral/cli/core.py` & `maestral-1.8.0.dev1/src/maestral/cli/core.py`

 * *Files identical despite different names*

### Comparing `maestral-1.8.0.dev0/src/maestral/cli/dialogs.py` & `maestral-1.8.0.dev1/src/maestral/cli/dialogs.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 """
 This module provides interactive commandline dialogs which are based on the
 :mod:`survey` Python library.
 """
 from __future__ import annotations
 
+import os
 import functools
 from typing import Callable, Sequence, TypeVar
 from typing_extensions import ParamSpec
 
-import click
-
 
 P = ParamSpec("P")
 T = TypeVar("T")
 
 
 def _style_message(message: str) -> str:
     return f"{message} "
 
 
 def _style_hint(hint: str) -> str:
     return f"{hint} " if hint else ""
 
 
 def _style_error(message: str) -> str:
-    return click.style(message, fg="red")
+    import survey
+
+    return survey.utils.paint(survey.colors.basic("red"), message)
 
 
 def exit_on_keyboard_interrupt(func: Callable[P, T]) -> Callable[P, T]:
     @functools.wraps(func)
     def wrapper(*args: P.args, **kwargs: P.kwargs) -> T:
         import survey
 
@@ -48,40 +49,50 @@
     import survey
 
     def check(value: str) -> None:
         if validate is not None and not validate(value):
             raise survey.widgets.Abort(_style_error(f"'{value}' is not allowed"))
 
     return survey.routines.input(
-        _style_message(message), validate=check, escapable=True
+        _style_message(message),
+        validate=check,
+        escapable=True,
+        mark_color=survey.colors.basic("cyan"),
     )
 
 
 @exit_on_keyboard_interrupt
 def confirm(message: str, default: bool | None = True) -> bool:
     import survey
 
     default_to_str = {True: "y", False: "n", None: None}
 
     return survey.routines.inquire(
-        _style_message(message), default=default_to_str[default], escapable=True
+        _style_message(message),
+        default=default_to_str[default],
+        escapable=True,
+        mark_color=survey.colors.basic("cyan"),
     )
 
 
 @exit_on_keyboard_interrupt
 def select(message: str, options: Sequence[str], hint: str | None = "") -> int:
     import survey
 
     if hint is None:
         kwargs = {}
     else:
         kwargs = {"hint": _style_hint(hint)}
 
     return survey.routines.select(
-        _style_message(message), options=options, escapable=True, **kwargs
+        _style_message(message),
+        options=options,
+        escapable=True,
+        mark_color=survey.colors.basic("cyan"),
+        **kwargs,
     )
 
 
 @exit_on_keyboard_interrupt
 def select_multiple(
     message: str, options: Sequence[str], hint: str | None = None
 ) -> list[int]:
@@ -104,32 +115,29 @@
     return survey.routines.basket(
         _style_message(message),
         options=options,
         positive_mark="[✓] ",
         negative_mark="[ ] ",
         reply=reply,
         escapable=True,
+        mark_color=survey.colors.basic("cyan"),
         **kwargs,
     )
 
 
 @exit_on_keyboard_interrupt
 def select_path(
     message: str,
     default: str | None = None,
     validate: Callable[[str], bool] = lambda x: True,
     exists: bool = False,
     files_allowed: bool = True,
     dirs_allowed: bool = True,
 ) -> str:
-    import os
     import survey
-    import wrapio
-
-    track = wrapio.Track()
 
     styled_message = _style_message(message)
 
     def check(value: str) -> None:
         value = value.strip()
 
         if value == "" and default:
@@ -153,17 +161,17 @@
         return survey.utils.paint(survey.colors.basic("cyan"), value or default)
 
     kwargs = {"hint": f"[{default}] "} if default else {}
 
     result = survey.routines.input(
         styled_message,
         reply=reply,
-        callback=track.invoke,
         validate=check,
         escapable=True,
+        mark_color=survey.colors.basic("cyan"),
         **kwargs,
     )
 
     result = result.strip()
 
     if result == "" and default:
         return default
```

### Comparing `maestral-1.8.0.dev0/src/maestral/cli/output.py` & `maestral-1.8.0.dev1/src/maestral/cli/output.py`

 * *Files identical despite different names*

### Comparing `maestral-1.8.0.dev0/src/maestral/client.py` & `maestral-1.8.0.dev1/src/maestral/client.py`

 * *Files identical despite different names*

### Comparing `maestral-1.8.0.dev0/src/maestral/config/__init__.py` & `maestral-1.8.0.dev1/src/maestral/config/__init__.py`

 * *Files identical despite different names*

### Comparing `maestral-1.8.0.dev0/src/maestral/config/main.py` & `maestral-1.8.0.dev1/src/maestral/config/main.py`

 * *Files identical despite different names*

### Comparing `maestral-1.8.0.dev0/src/maestral/config/user.py` & `maestral-1.8.0.dev1/src/maestral/config/user.py`

 * *Files identical despite different names*

### Comparing `maestral-1.8.0.dev0/src/maestral/constants.py` & `maestral-1.8.0.dev1/src/maestral/constants.py`

 * *Files identical despite different names*

### Comparing `maestral-1.8.0.dev0/src/maestral/core.py` & `maestral-1.8.0.dev1/src/maestral/core.py`

 * *Files identical despite different names*

### Comparing `maestral-1.8.0.dev0/src/maestral/daemon.py` & `maestral-1.8.0.dev1/src/maestral/daemon.py`

 * *Files identical despite different names*

### Comparing `maestral-1.8.0.dev0/src/maestral/database/core.py` & `maestral-1.8.0.dev1/src/maestral/database/core.py`

 * *Files identical despite different names*

### Comparing `maestral-1.8.0.dev0/src/maestral/database/orm.py` & `maestral-1.8.0.dev1/src/maestral/database/orm.py`

 * *Files identical despite different names*

### Comparing `maestral-1.8.0.dev0/src/maestral/database/query.py` & `maestral-1.8.0.dev1/src/maestral/database/query.py`

 * *Files identical despite different names*

### Comparing `maestral-1.8.0.dev0/src/maestral/database/types.py` & `maestral-1.8.0.dev1/src/maestral/database/types.py`

 * *Files identical despite different names*

### Comparing `maestral-1.8.0.dev0/src/maestral/errorhandling.py` & `maestral-1.8.0.dev1/src/maestral/errorhandling.py`

 * *Files identical despite different names*

### Comparing `maestral-1.8.0.dev0/src/maestral/exceptions.py` & `maestral-1.8.0.dev1/src/maestral/exceptions.py`

 * *Files identical despite different names*

### Comparing `maestral-1.8.0.dev0/src/maestral/fsevents/__init__.py` & `maestral-1.8.0.dev1/src/maestral/fsevents/__init__.py`

 * *Files identical despite different names*

### Comparing `maestral-1.8.0.dev0/src/maestral/fsevents/polling.py` & `maestral-1.8.0.dev1/src/maestral/fsevents/polling.py`

 * *Files identical despite different names*

### Comparing `maestral-1.8.0.dev0/src/maestral/keyring.py` & `maestral-1.8.0.dev1/src/maestral/keyring.py`

 * *Files identical despite different names*

### Comparing `maestral-1.8.0.dev0/src/maestral/logging.py` & `maestral-1.8.0.dev1/src/maestral/logging.py`

 * *Files identical despite different names*

### Comparing `maestral-1.8.0.dev0/src/maestral/main.py` & `maestral-1.8.0.dev1/src/maestral/main.py`

 * *Files identical despite different names*

### Comparing `maestral-1.8.0.dev0/src/maestral/manager.py` & `maestral-1.8.0.dev1/src/maestral/manager.py`

 * *Files identical despite different names*

### Comparing `maestral-1.8.0.dev0/src/maestral/models.py` & `maestral-1.8.0.dev1/src/maestral/models.py`

 * *Files identical despite different names*

### Comparing `maestral-1.8.0.dev0/src/maestral/notify.py` & `maestral-1.8.0.dev1/src/maestral/notify.py`

 * *Files identical despite different names*

### Comparing `maestral-1.8.0.dev0/src/maestral/resources/maestral.png` & `maestral-1.8.0.dev1/src/maestral/resources/maestral.png`

 * *Files identical despite different names*

### Comparing `maestral-1.8.0.dev0/src/maestral/sync.py` & `maestral-1.8.0.dev1/src/maestral/sync.py`

 * *Files identical despite different names*

### Comparing `maestral-1.8.0.dev0/src/maestral/utils/__init__.py` & `maestral-1.8.0.dev1/src/maestral/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `maestral-1.8.0.dev0/src/maestral/utils/appdirs.py` & `maestral-1.8.0.dev1/src/maestral/utils/appdirs.py`

 * *Files identical despite different names*

### Comparing `maestral-1.8.0.dev0/src/maestral/utils/caches.py` & `maestral-1.8.0.dev1/src/maestral/utils/caches.py`

 * *Files identical despite different names*

### Comparing `maestral-1.8.0.dev0/src/maestral/utils/hashing.py` & `maestral-1.8.0.dev1/src/maestral/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `maestral-1.8.0.dev0/src/maestral/utils/integration.py` & `maestral-1.8.0.dev1/src/maestral/utils/integration.py`

 * *Files identical despite different names*

### Comparing `maestral-1.8.0.dev0/src/maestral/utils/path.py` & `maestral-1.8.0.dev1/src/maestral/utils/path.py`

 * *Files identical despite different names*

### Comparing `maestral-1.8.0.dev0/src/maestral.egg-info/PKG-INFO` & `maestral-1.8.0.dev1/src/maestral.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maestral
-Version: 1.8.0.dev0
+Version: 1.8.0.dev1
 Summary: Open-source Dropbox client for macOS and Linux.
 Author-email: Sam Schott <sam.schott@outlook.com>
 License: MIT
 Project-URL: Homepage, https://maestral.app
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
```

### Comparing `maestral-1.8.0.dev0/src/maestral.egg-info/SOURCES.txt` & `maestral-1.8.0.dev1/src/maestral.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `maestral-1.8.0.dev0/src/maestral.egg-info/requires.txt` & `maestral-1.8.0.dev1/src/maestral.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,18 @@
 sphinxext-opengraph==0.8.2
 sphinx-autoapi==2.1.1
 sphinx-mdinclude==0.5.3
 
 [gui]
 
 [gui:sys_platform == "darwin"]
-maestral-cocoa>=1.8.0.dev0
+maestral-cocoa>=1.8.0.dev1
 
 [gui:sys_platform == "linux"]
-maestral-qt>=1.8.0.dev0
+maestral-qt>=1.8.0.dev1
 
 [lint]
 black
 flake8
 flake8-pyproject
 mypy
 pyupgrade
```

