# Comparing `tmp/reaxpro-wrappers-1.0.0.tar.gz` & `tmp/reaxpro-wrappers-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reaxpro-wrappers-1.0.0.tar", last modified: Tue Jul 18 09:34:31 2023, max compression
+gzip compressed data, was "reaxpro-wrappers-1.0.1.tar", last modified: Mon Jul 24 18:47:12 2023, max compression
```

## Comparing `reaxpro-wrappers-1.0.0.tar` & `reaxpro-wrappers-1.0.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:31.810426 reaxpro-wrappers-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-18 09:34:15.000000 reaxpro-wrappers-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-18 09:34:31.810426 reaxpro-wrappers-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-07-18 09:34:15.000000 reaxpro-wrappers-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:31.806426 reaxpro-wrappers-1.0.0/osp/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-18 09:34:15.000000 reaxpro-wrappers-1.0.0/osp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:31.806426 reaxpro-wrappers-1.0.0/osp/dictionaries/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:15.000000 reaxpro-wrappers-1.0.0/osp/dictionaries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:31.806426 reaxpro-wrappers-1.0.0/osp/dictionaries/ams/
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-07-18 09:34:15.000000 reaxpro-wrappers-1.0.0/osp/dictionaries/ams/Ziff-Gulari-Barshad-model-variants.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:15.000000 reaxpro-wrappers-1.0.0/osp/dictionaries/ams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-18 09:34:15.000000 reaxpro-wrappers-1.0.0/osp/dictionaries/ams/energy_landscape.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:31.806426 reaxpro-wrappers-1.0.0/osp/dictionaries/defaults/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-18 09:34:15.000000 reaxpro-wrappers-1.0.0/osp/dictionaries/defaults/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-18 09:34:15.000000 reaxpro-wrappers-1.0.0/osp/dictionaries/defaults/defaults_AMS.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:31.806426 reaxpro-wrappers-1.0.0/osp/dictionaries/energies/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-18 09:34:15.000000 reaxpro-wrappers-1.0.0/osp/dictionaries/energies/gas_energies.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:31.806426 reaxpro-wrappers-1.0.0/osp/dictionaries/example_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:15.000000 reaxpro-wrappers-1.0.0/osp/dictionaries/example_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-18 09:34:15.000000 reaxpro-wrappers-1.0.0/osp/dictionaries/example_data/lattice_input.dat
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-18 09:34:15.000000 reaxpro-wrappers-1.0.0/osp/dictionaries/example_data/state1.xyz
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-18 09:34:15.000000 reaxpro-wrappers-1.0.0/osp/dictionaries/example_data/state2.xyz
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-18 09:34:15.000000 reaxpro-wrappers-1.0.0/osp/dictionaries/example_data/state3.xyz
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-18 09:34:15.000000 reaxpro-wrappers-1.0.0/osp/dictionaries/example_data/state4.xyz
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-18 09:34:15.000000 reaxpro-wrappers-1.0.0/osp/dictionaries/example_data/state5.xyz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:31.806426 reaxpro-wrappers-1.0.0/osp/models/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-18 09:34:15.000000 reaxpro-wrappers-1.0.0/osp/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:31.806426 reaxpro-wrappers-1.0.0/osp/models/ams/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-18 09:34:15.000000 reaxpro-wrappers-1.0.0/osp/models/ams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-07-18 09:34:15.000000 reaxpro-wrappers-1.0.0/osp/models/ams/energy_landscape_refinement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:31.806426 reaxpro-wrappers-1.0.0/osp/models/settings/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-18 09:34:15.000000 reaxpro-wrappers-1.0.0/osp/models/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-18 09:34:15.000000 reaxpro-wrappers-1.0.0/osp/models/settings/general.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:31.806426 reaxpro-wrappers-1.0.0/osp/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:15.000000 reaxpro-wrappers-1.0.0/osp/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-07-18 09:34:15.000000 reaxpro-wrappers-1.0.0/osp/models/utils/general.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:31.806426 reaxpro-wrappers-1.0.0/osp/models/zacros/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:15.000000 reaxpro-wrappers-1.0.0/osp/models/zacros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48929 2023-07-18 09:34:15.000000 reaxpro-wrappers-1.0.0/osp/models/zacros/co_pyzacros.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:31.810426 reaxpro-wrappers-1.0.0/osp/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-18 09:34:15.000000 reaxpro-wrappers-1.0.0/osp/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7283 2023-07-18 09:34:15.000000 reaxpro-wrappers-1.0.0/osp/tools/graph_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    27026 2023-07-18 09:34:15.000000 reaxpro-wrappers-1.0.0/osp/tools/io_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    74897 2023-07-18 09:34:15.000000 reaxpro-wrappers-1.0.0/osp/tools/mapping_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-07-18 09:34:15.000000 reaxpro-wrappers-1.0.0/osp/tools/set_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:31.810426 reaxpro-wrappers-1.0.0/osp/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-18 09:34:15.000000 reaxpro-wrappers-1.0.0/osp/wrappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:31.810426 reaxpro-wrappers-1.0.0/osp/wrappers/simams/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-18 09:34:15.000000 reaxpro-wrappers-1.0.0/osp/wrappers/simams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-07-18 09:34:15.000000 reaxpro-wrappers-1.0.0/osp/wrappers/simams/simams_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:31.810426 reaxpro-wrappers-1.0.0/osp/wrappers/simzacros/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-18 09:34:15.000000 reaxpro-wrappers-1.0.0/osp/wrappers/simzacros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-07-18 09:34:15.000000 reaxpro-wrappers-1.0.0/osp/wrappers/simzacros/simzacros_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:31.810426 reaxpro-wrappers-1.0.0/reaxpro_wrappers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-18 09:34:31.000000 reaxpro-wrappers-1.0.0/reaxpro_wrappers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-18 09:34:31.000000 reaxpro-wrappers-1.0.0/reaxpro_wrappers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 09:34:31.000000 reaxpro-wrappers-1.0.0/reaxpro_wrappers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-18 09:34:31.000000 reaxpro-wrappers-1.0.0/reaxpro_wrappers.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-18 09:34:31.000000 reaxpro-wrappers-1.0.0/reaxpro_wrappers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-18 09:34:31.000000 reaxpro-wrappers-1.0.0/reaxpro_wrappers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-18 09:34:31.810426 reaxpro-wrappers-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-18 09:34:15.000000 reaxpro-wrappers-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:31.810426 reaxpro-wrappers-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-07-18 09:34:15.000000 reaxpro-wrappers-1.0.0/tests/test_energy_landscape_refinement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-18 09:34:15.000000 reaxpro-wrappers-1.0.0/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-07-18 09:34:15.000000 reaxpro-wrappers-1.0.0/tests/test_pyzacros_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-07-18 09:34:15.000000 reaxpro-wrappers-1.0.0/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:47:12.369703 reaxpro-wrappers-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-24 18:47:12.369703 reaxpro-wrappers-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:47:12.361703 reaxpro-wrappers-1.0.1/osp/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:47:12.361703 reaxpro-wrappers-1.0.1/osp/dictionaries/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/dictionaries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:47:12.361703 reaxpro-wrappers-1.0.1/osp/dictionaries/ams/
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/dictionaries/ams/Ziff-Gulari-Barshad-model-variants.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/dictionaries/ams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/dictionaries/ams/energy_landscape.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:47:12.361703 reaxpro-wrappers-1.0.1/osp/dictionaries/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/dictionaries/defaults/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/dictionaries/defaults/defaults_AMS.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:47:12.365703 reaxpro-wrappers-1.0.1/osp/dictionaries/energies/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/dictionaries/energies/gas_energies.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:47:12.365703 reaxpro-wrappers-1.0.1/osp/dictionaries/example_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/dictionaries/example_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/dictionaries/example_data/lattice_input.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/dictionaries/example_data/state1.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/dictionaries/example_data/state2.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/dictionaries/example_data/state3.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/dictionaries/example_data/state4.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/dictionaries/example_data/state5.xyz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:47:12.365703 reaxpro-wrappers-1.0.1/osp/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:47:12.365703 reaxpro-wrappers-1.0.1/osp/models/ams/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/models/ams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/models/ams/energy_landscape_refinement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:47:12.365703 reaxpro-wrappers-1.0.1/osp/models/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/models/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/models/settings/general.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:47:12.365703 reaxpro-wrappers-1.0.1/osp/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/models/utils/general.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:47:12.365703 reaxpro-wrappers-1.0.1/osp/models/zacros/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/models/zacros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48929 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/models/zacros/co_pyzacros.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:47:12.365703 reaxpro-wrappers-1.0.1/osp/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7283 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/tools/graph_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27026 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/tools/io_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74897 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/tools/mapping_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/tools/set_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:47:12.365703 reaxpro-wrappers-1.0.1/osp/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/wrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:47:12.365703 reaxpro-wrappers-1.0.1/osp/wrappers/simams/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/wrappers/simams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/wrappers/simams/simams_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:47:12.365703 reaxpro-wrappers-1.0.1/osp/wrappers/simzacros/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/wrappers/simzacros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/wrappers/simzacros/simzacros_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:47:12.365703 reaxpro-wrappers-1.0.1/reaxpro_wrappers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-24 18:47:12.000000 reaxpro-wrappers-1.0.1/reaxpro_wrappers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-24 18:47:12.000000 reaxpro-wrappers-1.0.1/reaxpro_wrappers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:47:12.000000 reaxpro-wrappers-1.0.1/reaxpro_wrappers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-24 18:47:12.000000 reaxpro-wrappers-1.0.1/reaxpro_wrappers.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-24 18:47:12.000000 reaxpro-wrappers-1.0.1/reaxpro_wrappers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-24 18:47:12.000000 reaxpro-wrappers-1.0.1/reaxpro_wrappers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-24 18:47:12.369703 reaxpro-wrappers-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:47:12.369703 reaxpro-wrappers-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/tests/test_energy_landscape_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/tests/test_pyzacros_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/tests/test_tools.py
```

### Comparing `reaxpro-wrappers-1.0.0/LICENSE` & `reaxpro-wrappers-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.0/PKG-INFO` & `reaxpro-wrappers-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reaxpro-wrappers
-Version: 1.0.0
+Version: 1.0.1
 Summary: The wrapper of AMS and Zacros drivers for SimPhoNy
 Home-page: https://www.esciencecenter.nl/
 Author: Netherlands eScience Center, Fraunhofer IWM
 Keywords: simphony,cuds,AMS,zacros,SCM
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `reaxpro-wrappers-1.0.0/README.md` & `reaxpro-wrappers-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.0/osp/dictionaries/ams/Ziff-Gulari-Barshad-model-variants.json` & `reaxpro-wrappers-1.0.1/osp/dictionaries/ams/Ziff-Gulari-Barshad-model-variants.json`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.0/osp/dictionaries/ams/energy_landscape.json` & `reaxpro-wrappers-1.0.1/osp/dictionaries/ams/energy_landscape.json`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.0/osp/dictionaries/defaults/defaults_AMS.yaml` & `reaxpro-wrappers-1.0.1/osp/dictionaries/defaults/defaults_AMS.yaml`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.0/osp/dictionaries/example_data/lattice_input.dat` & `reaxpro-wrappers-1.0.1/osp/dictionaries/example_data/lattice_input.dat`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.0/osp/dictionaries/example_data/state1.xyz` & `reaxpro-wrappers-1.0.1/osp/dictionaries/example_data/state1.xyz`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.0/osp/dictionaries/example_data/state2.xyz` & `reaxpro-wrappers-1.0.1/osp/dictionaries/example_data/state2.xyz`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.0/osp/dictionaries/example_data/state3.xyz` & `reaxpro-wrappers-1.0.1/osp/dictionaries/example_data/state3.xyz`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.0/osp/dictionaries/example_data/state4.xyz` & `reaxpro-wrappers-1.0.1/osp/dictionaries/example_data/state4.xyz`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.0/osp/dictionaries/example_data/state5.xyz` & `reaxpro-wrappers-1.0.1/osp/dictionaries/example_data/state5.xyz`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.0/osp/models/ams/energy_landscape_refinement.py` & `reaxpro-wrappers-1.0.1/osp/models/ams/energy_landscape_refinement.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.0/osp/models/settings/general.py` & `reaxpro-wrappers-1.0.1/osp/models/settings/general.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.0/osp/models/utils/general.py` & `reaxpro-wrappers-1.0.1/osp/models/utils/general.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.0/osp/models/zacros/co_pyzacros.py` & `reaxpro-wrappers-1.0.1/osp/models/zacros/co_pyzacros.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.0/osp/tools/graph_functions.py` & `reaxpro-wrappers-1.0.1/osp/tools/graph_functions.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.0/osp/tools/io_functions.py` & `reaxpro-wrappers-1.0.1/osp/tools/io_functions.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.0/osp/tools/mapping_functions.py` & `reaxpro-wrappers-1.0.1/osp/tools/mapping_functions.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.0/osp/tools/set_functions.py` & `reaxpro-wrappers-1.0.1/osp/tools/set_functions.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.0/osp/wrappers/simams/simams_session.py` & `reaxpro-wrappers-1.0.1/osp/wrappers/simams/simams_session.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     """Describe AMS Session class."""
 
     def __init__(self, engine=None, **kwargs):
         """Initialise SimamsSession."""
         if engine is None:
             PlamsInit()
             self.engine = MultiJob()
-        super().__init__(engine, **kwargs)
+        super().__init__(engine)
 
     def __str__(self):
         """To overwrite the private str method. Not advised, but here it is."""
         # TODO: Define the output of str(SomeSimulationSession())
         return "Some Wrapper Session"
 
     def _run(self, root_cuds_object: Cuds):
```

### Comparing `reaxpro-wrappers-1.0.0/osp/wrappers/simzacros/simzacros_session.py` & `reaxpro-wrappers-1.0.1/osp/wrappers/simzacros/simzacros_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     """Describe Zacros Session class."""
 
     def __init__(self, engine=None, **kwargs):
         """Initialise SimamsSession."""
         if engine is None:
             pz.init()
             self.engine = 'Zacros'
-        super().__init__(engine, **kwargs)
+        super().__init__(engine)
 
     def __str__(self):
         """To overwrite the private str method. Not advised, but here it is."""
         # TODO: Define the output of str(SomeSimulationSession())
         return "Some Wrapper Session"
 
     def _run(self, root_cuds_object: Cuds):
```

### Comparing `reaxpro-wrappers-1.0.0/reaxpro_wrappers.egg-info/PKG-INFO` & `reaxpro-wrappers-1.0.1/reaxpro_wrappers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reaxpro-wrappers
-Version: 1.0.0
+Version: 1.0.1
 Summary: The wrapper of AMS and Zacros drivers for SimPhoNy
 Home-page: https://www.esciencecenter.nl/
 Author: Netherlands eScience Center, Fraunhofer IWM
 Keywords: simphony,cuds,AMS,zacros,SCM
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `reaxpro-wrappers-1.0.0/reaxpro_wrappers.egg-info/SOURCES.txt` & `reaxpro-wrappers-1.0.1/reaxpro_wrappers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.0/setup.cfg` & `reaxpro-wrappers-1.0.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = reaxpro-wrappers
 author = Netherlands eScience Center, Fraunhofer IWM
 url = https://www.esciencecenter.nl/
-version = v1.0.0
+version = v1.0.1
 description = The wrapper of AMS and Zacros drivers for SimPhoNy
 keywords = simphony, cuds, AMS, zacros, SCM
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `reaxpro-wrappers-1.0.0/setup.py` & `reaxpro-wrappers-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.0/tests/test_energy_landscape_refinement.py` & `reaxpro-wrappers-1.0.1/tests/test_energy_landscape_refinement.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.0/tests/test_examples.py` & `reaxpro-wrappers-1.0.1/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.0/tests/test_pyzacros_model.py` & `reaxpro-wrappers-1.0.1/tests/test_pyzacros_model.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.0/tests/test_tools.py` & `reaxpro-wrappers-1.0.1/tests/test_tools.py`

 * *Files identical despite different names*

