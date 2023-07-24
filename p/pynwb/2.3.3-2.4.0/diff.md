# Comparing `tmp/pynwb-2.3.3.tar.gz` & `tmp/pynwb-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynwb-2.3.3.tar", last modified: Mon Jun 26 21:00:02 2023, max compression
+gzip compressed data, was "pynwb-2.4.0.tar", last modified: Mon Jul 24 14:38:46 2023, max compression
```

## Comparing `pynwb-2.3.3.tar` & `pynwb-2.4.0.tar`

### file list

```diff
@@ -1,186 +1,188 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:00:02.447686 pynwb-2.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-26 20:55:48.000000 pynwb-2.3.3/Legal.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-26 20:55:48.000000 pynwb-2.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-06-26 21:00:02.447686 pynwb-2.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-06-26 20:55:48.000000 pynwb-2.3.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-26 20:55:49.000000 pynwb-2.3.3/environment-ros3.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-06-26 20:55:49.000000 pynwb-2.3.3/license.txt
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-26 20:55:49.000000 pynwb-2.3.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-26 20:55:49.000000 pynwb-2.3.3/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-26 20:55:49.000000 pynwb-2.3.3/requirements-min.txt
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-26 20:55:49.000000 pynwb-2.3.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-26 21:00:02.451686 pynwb-2.3.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2402 2023-06-26 20:55:49.000000 pynwb-2.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:00:02.387685 pynwb-2.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:00:02.451686 pynwb-2.3.3/src/pynwb/
--rw-r--r--   0 runner    (1001) docker     (123)    17453 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/_due.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-26 21:00:02.451686 pynwb-2.3.3/src/pynwb/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    28433 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/behavior.py
--rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    18125 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/ecephys.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/epoch.py
--rw-r--r--   0 runner    (1001) docker     (123)    57672 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/file.py
--rw-r--r--   0 runner    (1001) docker     (123)    45643 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/icephys.py
--rw-r--r--   0 runner    (1001) docker     (123)    17740 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:00:02.407686 pynwb-2.3.3/src/pynwb/io/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/io/base.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/io/behavior.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/io/core.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/io/ecephys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/io/epoch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10002 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/io/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/io/icephys.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/io/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/io/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/io/ogen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/io/ophys.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/io/retinotopy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:00:02.407686 pynwb-2.3.3/src/pynwb/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:00:02.411686 pynwb-2.3.3/src/pynwb/legacy/io/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/legacy/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/legacy/io/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/legacy/io/behavior.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/legacy/io/ecephys.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/legacy/io/epoch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/legacy/io/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/legacy/io/icephys.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/legacy/io/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/legacy/io/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/legacy/io/ogen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/legacy/io/ophys.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/legacy/io/retinotopy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/legacy/map.py
--rw-r--r--   0 runner    (1001) docker     (123)    17449 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:00:02.387685 pynwb-2.3.3/src/pynwb/nwb-schema/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:00:02.415686 pynwb-2.3.3/src/pynwb/nwb-schema/core/
--rw-r--r--   0 runner    (1001) docker     (123)     9437 2023-06-26 20:55:51.000000 pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.base.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-06-26 20:55:51.000000 pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.behavior.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-26 20:55:51.000000 pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.device.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12064 2023-06-26 20:55:51.000000 pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.ecephys.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-26 20:55:51.000000 pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.epoch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    21539 2023-06-26 20:55:51.000000 pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.file.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    16212 2023-06-26 20:55:51.000000 pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.icephys.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-06-26 20:55:51.000000 pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.image.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11642 2023-06-26 20:55:51.000000 pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.misc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-26 20:55:51.000000 pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.namespace.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-26 20:55:51.000000 pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.ogen.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12714 2023-06-26 20:55:51.000000 pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.ophys.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-06-26 20:55:51.000000 pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.retinotopy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/ogen.py
--rw-r--r--   0 runner    (1001) docker     (123)    22692 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/ophys.py
--rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/retinotopy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:00:02.419686 pynwb-2.3.3/src/pynwb/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9160 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/testing/icephys_testutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/testing/make_test_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:00:02.423686 pynwb-2.3.3/src/pynwb/testing/mock/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/testing/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/testing/mock/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/testing/mock/behavior.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/testing/mock/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/testing/mock/ecephys.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/testing/mock/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/testing/mock/icephys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/testing/mock/ogen.py
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/testing/mock/ophys.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/testing/mock/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15790 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/testing/testh5io.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/testing/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-06-26 20:55:49.000000 pynwb-2.3.3/src/pynwb/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:00:02.403685 pynwb-2.3.3/src/pynwb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-06-26 21:00:02.000000 pynwb-2.3.3/src/pynwb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-06-26 21:00:02.000000 pynwb-2.3.3/src/pynwb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 21:00:02.000000 pynwb-2.3.3/src/pynwb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:56:09.000000 pynwb-2.3.3/src/pynwb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-26 21:00:02.000000 pynwb-2.3.3/src/pynwb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-26 21:00:02.000000 pynwb-2.3.3/src/pynwb.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    14813 2023-06-26 20:55:49.000000 pynwb-2.3.3/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:00:02.423686 pynwb-2.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:00:02.431686 pynwb-2.3.3/tests/back_compat/
--rw-r--r--   0 runner    (1001) docker     (123)    13056 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/1.0.2_nwbfile.nwb
--rw-r--r--   0 runner    (1001) docker     (123)    15632 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/1.0.2_str_experimenter.nwb
--rw-r--r--   0 runner    (1001) docker     (123)    15632 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/1.0.2_str_pub.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   143504 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/1.0.3_nwbfile.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   144096 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/1.0.3_str_experimenter.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   144096 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/1.0.3_str_pub.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   142512 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/1.1.0_nwbfile.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   143104 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/1.1.0_str_experimenter.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   143104 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/1.1.0_str_pub.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   148288 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/1.1.2_nwbfile.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   148880 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/1.1.2_str_experimenter.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   148880 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/1.1.2_str_pub.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   169624 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/1.5.1_imageseries_no_data.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   169408 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/1.5.1_imageseries_no_unit.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   169120 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/1.5.1_timeseries_no_data.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   169408 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/1.5.1_timeseries_no_unit.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   182272 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/2.1.0_imageseries_no_data.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   182272 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/2.1.0_imageseries_non_external_format.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   182272 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/2.1.0_imageseries_nonmatch_starting_frame.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   184152 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/2.1.0_nwbfile_with_extension.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   181616 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/2.2.0_subject_no_age__reference.nwb
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/test_import_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/back_compat/test_read.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:00:02.435686 pynwb-2.3.3/tests/coverage/
--rwxr-xr-x   0 runner    (1001) docker     (123)      295 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/coverage/runCoverage
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:00:02.435686 pynwb-2.3.3/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:00:02.439686 pynwb-2.3.3/tests/integration/hdf5/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/integration/hdf5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/integration/hdf5/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/integration/hdf5/test_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    11609 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/integration/hdf5/test_ecephys.py
--rw-r--r--   0 runner    (1001) docker     (123)    13771 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/integration/hdf5/test_icephys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/integration/hdf5/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    25147 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/integration/hdf5/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     8609 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/integration/hdf5/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/integration/hdf5/test_modular_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    26419 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/integration/hdf5/test_nwbfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/integration/hdf5/test_ogen.py
--rw-r--r--   0 runner    (1001) docker     (123)    13921 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/integration/hdf5/test_ophys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/integration/hdf5/test_retinotopy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/integration/hdf5/test_scratch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:00:02.439686 pynwb-2.3.3/tests/integration/ros3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/integration/ros3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/integration/ros3/test_ros3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:00:02.439686 pynwb-2.3.3/tests/integration/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/integration/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/integration/utils/test_io_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:00:02.439686 pynwb-2.3.3/tests/read_dandi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/read_dandi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/read_dandi/test_read_dandi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:00:02.447686 pynwb-2.3.3/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31128 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/unit/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/unit/test_behavior.py
--rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/unit/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/unit/test_core_NWBContainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/unit/test_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    14154 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/unit/test_ecephys.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/unit/test_epoch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/unit/test_epoch_legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/unit/test_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)    27739 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/unit/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    14961 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/unit/test_icephys.py
--rw-r--r--   0 runner    (1001) docker     (123)    66716 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/unit/test_icephys_metadata_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)    16176 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/unit/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/unit/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/unit/test_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/unit/test_ogen.py
--rw-r--r--   0 runner    (1001) docker     (123)    19248 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/unit/test_ophys.py
--rw-r--r--   0 runner    (1001) docker     (123)     8025 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/unit/test_retinotopy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/unit/test_scratch.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/unit/test_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:00:02.447686 pynwb-2.3.3/tests/validation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15661 2023-06-26 20:55:49.000000 pynwb-2.3.3/tests/validation/test_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-06-26 20:55:49.000000 pynwb-2.3.3/tox.ini
--rw-r--r--   0 runner    (1001) docker     (123)    83021 2023-06-26 20:55:49.000000 pynwb-2.3.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:38:46.830415 pynwb-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-24 14:33:53.000000 pynwb-2.4.0/Legal.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-24 14:33:53.000000 pynwb-2.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-07-24 14:38:46.830415 pynwb-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-07-24 14:33:53.000000 pynwb-2.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-24 14:33:53.000000 pynwb-2.4.0/environment-ros3.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-24 14:33:53.000000 pynwb-2.4.0/license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-24 14:33:53.000000 pynwb-2.4.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-24 14:33:53.000000 pynwb-2.4.0/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-24 14:33:53.000000 pynwb-2.4.0/requirements-min.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-24 14:33:53.000000 pynwb-2.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-24 14:38:46.830415 pynwb-2.4.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2353 2023-07-24 14:33:53.000000 pynwb-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:38:46.790414 pynwb-2.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:38:46.830415 pynwb-2.4.0/src/pynwb/
+-rw-r--r--   0 runner    (1001) docker     (123)    17755 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/_due.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-24 14:38:46.830415 pynwb-2.4.0/src/pynwb/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28433 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/behavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18125 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/ecephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/epoch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57750 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45643 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/icephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17740 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:38:46.806414 pynwb-2.4.0/src/pynwb/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/io/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/io/behavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/io/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/io/ecephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/io/epoch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10002 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/io/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/io/icephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/io/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/io/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/io/ogen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/io/ophys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/io/retinotopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:38:46.806414 pynwb-2.4.0/src/pynwb/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:38:46.810415 pynwb-2.4.0/src/pynwb/legacy/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/legacy/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/legacy/io/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/legacy/io/behavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/legacy/io/ecephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/legacy/io/epoch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/legacy/io/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/legacy/io/icephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/legacy/io/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/legacy/io/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/legacy/io/ogen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/legacy/io/ophys.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/legacy/io/retinotopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/legacy/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17449 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:38:46.790414 pynwb-2.4.0/src/pynwb/nwb-schema/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:38:46.814415 pynwb-2.4.0/src/pynwb/nwb-schema/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     9437 2023-07-24 14:33:59.000000 pynwb-2.4.0/src/pynwb/nwb-schema/core/nwb.base.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-07-24 14:33:59.000000 pynwb-2.4.0/src/pynwb/nwb-schema/core/nwb.behavior.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-24 14:33:59.000000 pynwb-2.4.0/src/pynwb/nwb-schema/core/nwb.device.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12064 2023-07-24 14:33:59.000000 pynwb-2.4.0/src/pynwb/nwb-schema/core/nwb.ecephys.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-24 14:33:59.000000 pynwb-2.4.0/src/pynwb/nwb-schema/core/nwb.epoch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    21539 2023-07-24 14:33:59.000000 pynwb-2.4.0/src/pynwb/nwb-schema/core/nwb.file.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    16212 2023-07-24 14:33:59.000000 pynwb-2.4.0/src/pynwb/nwb-schema/core/nwb.icephys.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-07-24 14:33:59.000000 pynwb-2.4.0/src/pynwb/nwb-schema/core/nwb.image.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11642 2023-07-24 14:33:59.000000 pynwb-2.4.0/src/pynwb/nwb-schema/core/nwb.misc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-07-24 14:33:59.000000 pynwb-2.4.0/src/pynwb/nwb-schema/core/nwb.namespace.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-24 14:33:59.000000 pynwb-2.4.0/src/pynwb/nwb-schema/core/nwb.ogen.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12714 2023-07-24 14:33:59.000000 pynwb-2.4.0/src/pynwb/nwb-schema/core/nwb.ophys.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-07-24 14:33:59.000000 pynwb-2.4.0/src/pynwb/nwb-schema/core/nwb.retinotopy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/ogen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22692 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/ophys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/retinotopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:38:46.814415 pynwb-2.4.0/src/pynwb/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9160 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/testing/icephys_testutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/testing/make_test_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:38:46.814415 pynwb-2.4.0/src/pynwb/testing/mock/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/testing/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/testing/mock/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/testing/mock/behavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/testing/mock/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/testing/mock/ecephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/testing/mock/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/testing/mock/icephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/testing/mock/ogen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/testing/mock/ophys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/testing/mock/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15790 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/testing/testh5io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/testing/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-07-24 14:33:53.000000 pynwb-2.4.0/src/pynwb/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:38:46.806414 pynwb-2.4.0/src/pynwb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-07-24 14:38:46.000000 pynwb-2.4.0/src/pynwb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-07-24 14:38:46.000000 pynwb-2.4.0/src/pynwb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 14:38:46.000000 pynwb-2.4.0/src/pynwb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 14:34:26.000000 pynwb-2.4.0/src/pynwb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-24 14:38:46.000000 pynwb-2.4.0/src/pynwb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 14:38:46.000000 pynwb-2.4.0/src/pynwb.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14813 2023-07-24 14:33:53.000000 pynwb-2.4.0/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:38:46.814415 pynwb-2.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:38:46.826415 pynwb-2.4.0/tests/back_compat/
+-rw-r--r--   0 runner    (1001) docker     (123)    13056 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/back_compat/1.0.2_nwbfile.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)    15632 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/back_compat/1.0.2_str_experimenter.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)    15632 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/back_compat/1.0.2_str_pub.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   143504 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/back_compat/1.0.3_nwbfile.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   144096 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/back_compat/1.0.3_str_experimenter.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   144096 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/back_compat/1.0.3_str_pub.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   142512 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/back_compat/1.1.0_nwbfile.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   143104 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/back_compat/1.1.0_str_experimenter.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   143104 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/back_compat/1.1.0_str_pub.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   148288 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/back_compat/1.1.2_nwbfile.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   148880 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/back_compat/1.1.2_str_experimenter.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   148880 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/back_compat/1.1.2_str_pub.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   169624 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/back_compat/1.5.1_imageseries_no_data.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   169408 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/back_compat/1.5.1_imageseries_no_unit.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   169120 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/back_compat/1.5.1_timeseries_no_data.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   169408 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/back_compat/1.5.1_timeseries_no_unit.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   182272 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/back_compat/2.1.0_imageseries_no_data.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   182272 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/back_compat/2.1.0_imageseries_non_external_format.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   182272 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/back_compat/2.1.0_imageseries_nonmatch_starting_frame.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   184152 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/back_compat/2.1.0_nwbfile_with_extension.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   181616 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/back_compat/2.2.0_subject_no_age__reference.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/back_compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/back_compat/test_import_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/back_compat/test_read.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:38:46.826415 pynwb-2.4.0/tests/coverage/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      295 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/coverage/runCoverage
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:38:46.826415 pynwb-2.4.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:38:46.826415 pynwb-2.4.0/tests/integration/hdf5/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/integration/hdf5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/integration/hdf5/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/integration/hdf5/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11609 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/integration/hdf5/test_ecephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13771 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/integration/hdf5/test_icephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/integration/hdf5/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25147 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/integration/hdf5/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8609 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/integration/hdf5/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/integration/hdf5/test_modular_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26419 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/integration/hdf5/test_nwbfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/integration/hdf5/test_ogen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13921 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/integration/hdf5/test_ophys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/integration/hdf5/test_retinotopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/integration/hdf5/test_scratch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:38:46.826415 pynwb-2.4.0/tests/integration/ros3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/integration/ros3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/integration/ros3/test_ros3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:38:46.826415 pynwb-2.4.0/tests/integration/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/integration/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/integration/utils/test_io_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:38:46.826415 pynwb-2.4.0/tests/read_dandi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/read_dandi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/read_dandi/test_read_dandi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:38:46.830415 pynwb-2.4.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31128 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/unit/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/unit/test_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/unit/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/unit/test_core_NWBContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/unit/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14154 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/unit/test_ecephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/unit/test_epoch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/unit/test_epoch_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/unit/test_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27739 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/unit/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14961 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/unit/test_icephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66716 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/unit/test_icephys_metadata_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16176 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/unit/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/unit/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/unit/test_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/unit/test_ogen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19248 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/unit/test_ophys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/unit/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8025 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/unit/test_retinotopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/unit/test_scratch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/unit/test_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:38:46.830415 pynwb-2.4.0/tests/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15661 2023-07-24 14:33:53.000000 pynwb-2.4.0/tests/validation/test_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-07-24 14:33:53.000000 pynwb-2.4.0/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    83021 2023-07-24 14:33:53.000000 pynwb-2.4.0/versioneer.py
```

### Comparing `pynwb-2.3.3/Legal.txt` & `pynwb-2.4.0/Legal.txt`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/PKG-INFO` & `pynwb-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: pynwb
-Version: 2.3.3
+Version: 2.4.0
 Summary: Package for working with Neurodata stored in the NWB format
 Home-page: https://github.com/NeurodataWithoutBorders/pynwb
 Author: Andrew Tritt
 Author-email: ajtritt@lbl.gov
 License: BSD
 Keywords: Neuroscience python HDF HDF5 cross-platform open-data data-format open-source open-science reproducible-research PyNWB NWB NWB:N NeurodataWithoutBorders
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst; charset=UTF-8
 
 .. image:: docs/source/figures/logo_pynwb.png
     :width: 200px
 
 PyNWB is a Python package for working with NWB files. The PyNWB
 documentation can be found at https://pynwb.readthedocs.io
```

### Comparing `pynwb-2.3.3/README.rst` & `pynwb-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/license.txt` & `pynwb-2.4.0/license.txt`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/requirements-doc.txt` & `pynwb-2.4.0/requirements-doc.txt`

 * *Files 10% similar despite different names*

```diff
@@ -7,9 +7,8 @@
 # allensdk>=2.13.2  # allensdk reinstalls pynwb and hdmf. TODO set up a separate workflow to test allensdk
 # MarkupSafe==2.0.1  # resolve incompatibility between jinja2 and markupsafe: https://github.com/AllenInstitute/AllenSDK/issues/2308
 Pillow
 sphinx-copybutton
 dataframe_image   # used to render large dataframe as image in the sphinx gallery to improve html display
 lxml  # used by dataframe_image when using the matplotlib backend
 hdf5plugin
-importlib-metadata<4.3; python_version < "3.8"  # TODO: remove when minimum python version is 3.8
```

### Comparing `pynwb-2.3.3/setup.cfg` & `pynwb-2.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/setup.py` & `pynwb-2.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 pkgs = find_packages('src', exclude=['data'])
 print('found these packages:', pkgs)
 
 schema_dir = 'nwb-schema/core'
 
 reqs = [
     'h5py>=2.10',
-    'hdmf>=3.5.4',
+    'hdmf>=3.8.0',
     'numpy>=1.16',
     'pandas>=1.1.5',
     'python-dateutil>=2.7.3',
     'setuptools'
 ]
 
 print(reqs)
@@ -40,18 +40,17 @@
     'author_email': 'ajtritt@lbl.gov',
     'url': 'https://github.com/NeurodataWithoutBorders/pynwb',
     'license': "BSD",
     'install_requires': reqs,
     'packages': pkgs,
     'package_dir': {'': 'src'},
     'package_data': {'pynwb': ["%s/*.yaml" % schema_dir, "%s/*.json" % schema_dir]},
-    'python_requires': '>=3.7',
+    'python_requires': '>=3.8',
     'classifiers': [
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: BSD License",
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
```

### Comparing `pynwb-2.3.3/src/pynwb/__init__.py` & `pynwb-2.4.0/src/pynwb/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -211,18 +211,21 @@
             {'name': 'manager', 'type': BuildManager, 'doc': 'the BuildManager to use for I/O', 'default': None},
             {'name': 'extensions', 'type': (str, TypeMap, list),
              'doc': 'a path to a namespace, a TypeMap, or a list consisting paths to namespaces and TypeMaps',
              'default': None},
             {'name': 'file', 'type': [h5py.File, 'S3File'], 'doc': 'a pre-existing h5py.File object', 'default': None},
             {'name': 'comm', 'type': "Intracomm", 'doc': 'the MPI communicator to use for parallel I/O',
              'default': None},
-            {'name': 'driver', 'type': str, 'doc': 'driver for h5py to use when opening HDF5 file', 'default': None})
+            {'name': 'driver', 'type': str, 'doc': 'driver for h5py to use when opening HDF5 file', 'default': None},
+            {'name': 'external_resources_path', 'type': str, 'doc': 'The path to the ExternalResources',
+             'default': None},)
     def __init__(self, **kwargs):
-        path, mode, manager, extensions, load_namespaces, file_obj, comm, driver =\
-            popargs('path', 'mode', 'manager', 'extensions', 'load_namespaces', 'file', 'comm', 'driver', kwargs)
+        path, mode, manager, extensions, load_namespaces, file_obj, comm, driver, external_resources_path =\
+            popargs('path', 'mode', 'manager', 'extensions', 'load_namespaces',
+                    'file', 'comm', 'driver', 'external_resources_path', kwargs)
         # Define the BuildManager to use
         if load_namespaces:
             if manager is not None:
                 warn("loading namespaces from file - ignoring 'manager'")
             if extensions is not None:
                 warn("loading namespaces from file - ignoring 'extensions' argument")
             # namespaces are not loaded when creating an NWBHDF5IO object in write mode
@@ -243,15 +246,16 @@
             if manager is not None and extensions is not None:
                 raise ValueError("'manager' and 'extensions' cannot be specified together")
             elif extensions is not None:
                 manager = get_manager(extensions=extensions)
             elif manager is None:
                 manager = get_manager()
         # Open the file
-        super().__init__(path, manager=manager, mode=mode, file=file_obj, comm=comm, driver=driver)
+        super().__init__(path, manager=manager, mode=mode, file=file_obj, comm=comm,
+                         driver=driver, external_resources_path=external_resources_path)
 
     @property
     def nwb_version(self):
         """
         Get the version of the NWB file opened via this NWBHDF5IO object.
 
         :returns: Tuple consisting of: 1) the original version string as stored in the file and
@@ -293,15 +297,16 @@
             file_version_str, file_version = self.nwb_version
             if file_version is None:
                 raise TypeError("Missing NWB version in file. The file is not a valid NWB file.")
             if file_version[0] < 2:
                 raise TypeError("NWB version %s not supported. PyNWB supports NWB files version 2 and above." %
                                 str(file_version_str))
         # read the file
-        return super().read(**kwargs)
+        file = super().read(**kwargs)
+        return file
 
     @docval({'name': 'src_io', 'type': HDMFIO,
              'doc': 'the HDMFIO object (such as NWBHDF5IO) that was used to read the data to export'},
             {'name': 'nwbfile', 'type': 'NWBFile',
              'doc': 'the NWBFile object to export. If None, then the entire contents of src_io will be exported',
              'default': None},
             {'name': 'write_args', 'type': dict, 'doc': 'arguments to pass to :py:meth:`write_builder`',
@@ -345,15 +350,14 @@
         super().export(**kwargs)
 
 
 from . import io as __io  # noqa: F401,E402
 from .core import NWBContainer, NWBData  # noqa: F401,E402
 from .base import TimeSeries, ProcessingModule  # noqa: F401,E402
 from .file import NWBFile  # noqa: F401,E402
-
 from . import behavior  # noqa: F401,E402
 from . import device  # noqa: F401,E402
 from . import ecephys  # noqa: F401,E402
 from . import epoch  # noqa: F401,E402
 from . import icephys  # noqa: F401,E402
 from . import image  # noqa: F401,E402
 from . import misc  # noqa: F401,E402
```

### Comparing `pynwb-2.3.3/src/pynwb/_due.py` & `pynwb-2.4.0/src/pynwb/_due.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/base.py` & `pynwb-2.4.0/src/pynwb/base.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/behavior.py` & `pynwb-2.4.0/src/pynwb/behavior.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/core.py` & `pynwb-2.4.0/src/pynwb/core.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/device.py` & `pynwb-2.4.0/src/pynwb/device.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/ecephys.py` & `pynwb-2.4.0/src/pynwb/ecephys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/epoch.py` & `pynwb-2.4.0/src/pynwb/epoch.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/file.py` & `pynwb-2.4.0/src/pynwb/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from warnings import warn
 import copy as _copy
 
 import numpy as np
 import pandas as pd
 
 from hdmf.common import DynamicTableRegion, DynamicTable
+from hdmf.container import ExternalResourcesManager
 from hdmf.utils import docval, getargs, get_docval, popargs, popargs_to_dict, AllowPositional
 
 from . import register_class, CORE_NAMESPACE
 from .base import TimeSeries, ProcessingModule
 from .device import Device
 from .epoch import TimeIntervals
 from .ecephys import ElectrodeGroup
@@ -145,15 +146,15 @@
             args_to_set['date_of_birth'] = _add_missing_timezone(date_of_birth)
 
         for key, val in args_to_set.items():
             setattr(self, key, val)
 
 
 @register_class('NWBFile', CORE_NAMESPACE)
-class NWBFile(MultiContainerInterface):
+class NWBFile(MultiContainerInterface, ExternalResourcesManager):
     """
     A representation of an NWB file.
     """
 
     __clsconf__ = [
         {
             'attr': 'acquisition',
```

### Comparing `pynwb-2.3.3/src/pynwb/icephys.py` & `pynwb-2.4.0/src/pynwb/icephys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/image.py` & `pynwb-2.4.0/src/pynwb/image.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/io/base.py` & `pynwb-2.4.0/src/pynwb/io/base.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/io/core.py` & `pynwb-2.4.0/src/pynwb/io/core.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/io/epoch.py` & `pynwb-2.4.0/src/pynwb/io/epoch.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/io/file.py` & `pynwb-2.4.0/src/pynwb/io/file.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/io/icephys.py` & `pynwb-2.4.0/src/pynwb/io/icephys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/io/misc.py` & `pynwb-2.4.0/src/pynwb/io/misc.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/io/ophys.py` & `pynwb-2.4.0/src/pynwb/io/ophys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/io/utils.py` & `pynwb-2.4.0/src/pynwb/io/utils.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/legacy/__init__.py` & `pynwb-2.4.0/src/pynwb/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/legacy/io/base.py` & `pynwb-2.4.0/src/pynwb/legacy/io/base.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/legacy/io/behavior.py` & `pynwb-2.4.0/src/pynwb/legacy/io/behavior.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/legacy/io/epoch.py` & `pynwb-2.4.0/src/pynwb/legacy/io/epoch.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/legacy/io/file.py` & `pynwb-2.4.0/src/pynwb/legacy/io/file.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/legacy/io/icephys.py` & `pynwb-2.4.0/src/pynwb/legacy/io/icephys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/legacy/io/ogen.py` & `pynwb-2.4.0/src/pynwb/legacy/io/ogen.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/legacy/io/ophys.py` & `pynwb-2.4.0/src/pynwb/legacy/io/ophys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/legacy/map.py` & `pynwb-2.4.0/src/pynwb/legacy/map.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/misc.py` & `pynwb-2.4.0/src/pynwb/misc.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.base.yaml` & `pynwb-2.4.0/src/pynwb/nwb-schema/core/nwb.base.yaml`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.behavior.yaml` & `pynwb-2.4.0/src/pynwb/nwb-schema/core/nwb.behavior.yaml`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.ecephys.yaml` & `pynwb-2.4.0/src/pynwb/nwb-schema/core/nwb.ecephys.yaml`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.epoch.yaml` & `pynwb-2.4.0/src/pynwb/nwb-schema/core/nwb.epoch.yaml`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.file.yaml` & `pynwb-2.4.0/src/pynwb/nwb-schema/core/nwb.file.yaml`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.icephys.yaml` & `pynwb-2.4.0/src/pynwb/nwb-schema/core/nwb.icephys.yaml`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.image.yaml` & `pynwb-2.4.0/src/pynwb/nwb-schema/core/nwb.image.yaml`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.misc.yaml` & `pynwb-2.4.0/src/pynwb/nwb-schema/core/nwb.misc.yaml`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.namespace.yaml` & `pynwb-2.4.0/src/pynwb/nwb-schema/core/nwb.namespace.yaml`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.ogen.yaml` & `pynwb-2.4.0/src/pynwb/nwb-schema/core/nwb.ogen.yaml`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.ophys.yaml` & `pynwb-2.4.0/src/pynwb/nwb-schema/core/nwb.ophys.yaml`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/nwb-schema/core/nwb.retinotopy.yaml` & `pynwb-2.4.0/src/pynwb/nwb-schema/core/nwb.retinotopy.yaml`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/ogen.py` & `pynwb-2.4.0/src/pynwb/ogen.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/ophys.py` & `pynwb-2.4.0/src/pynwb/ophys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/retinotopy.py` & `pynwb-2.4.0/src/pynwb/retinotopy.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/spec.py` & `pynwb-2.4.0/src/pynwb/spec.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/testing/icephys_testutils.py` & `pynwb-2.4.0/src/pynwb/testing/icephys_testutils.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/testing/make_test_files.py` & `pynwb-2.4.0/src/pynwb/testing/make_test_files.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/testing/mock/__init__.py` & `pynwb-2.4.0/src/pynwb/testing/mock/__init__.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/testing/mock/base.py` & `pynwb-2.4.0/src/pynwb/testing/mock/base.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/testing/mock/behavior.py` & `pynwb-2.4.0/src/pynwb/testing/mock/behavior.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/testing/mock/ecephys.py` & `pynwb-2.4.0/src/pynwb/testing/mock/ecephys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/testing/mock/file.py` & `pynwb-2.4.0/src/pynwb/testing/mock/file.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/testing/mock/icephys.py` & `pynwb-2.4.0/src/pynwb/testing/mock/icephys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/testing/mock/ogen.py` & `pynwb-2.4.0/src/pynwb/testing/mock/ogen.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/testing/mock/ophys.py` & `pynwb-2.4.0/src/pynwb/testing/mock/ophys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/testing/mock/utils.py` & `pynwb-2.4.0/src/pynwb/testing/mock/utils.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/testing/testh5io.py` & `pynwb-2.4.0/src/pynwb/testing/testh5io.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb/validate.py` & `pynwb-2.4.0/src/pynwb/validate.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/src/pynwb.egg-info/PKG-INFO` & `pynwb-2.4.0/src/pynwb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: pynwb
-Version: 2.3.3
+Version: 2.4.0
 Summary: Package for working with Neurodata stored in the NWB format
 Home-page: https://github.com/NeurodataWithoutBorders/pynwb
 Author: Andrew Tritt
 Author-email: ajtritt@lbl.gov
 License: BSD
 Keywords: Neuroscience python HDF HDF5 cross-platform open-data data-format open-source open-science reproducible-research PyNWB NWB NWB:N NeurodataWithoutBorders
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst; charset=UTF-8
 
 .. image:: docs/source/figures/logo_pynwb.png
     :width: 200px
 
 PyNWB is a Python package for working with NWB files. The PyNWB
 documentation can be found at https://pynwb.readthedocs.io
```

### Comparing `pynwb-2.3.3/src/pynwb.egg-info/SOURCES.txt` & `pynwb-2.4.0/src/pynwb.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 src/pynwb/epoch.py
 src/pynwb/file.py
 src/pynwb/icephys.py
 src/pynwb/image.py
 src/pynwb/misc.py
 src/pynwb/ogen.py
 src/pynwb/ophys.py
+src/pynwb/resources.py
 src/pynwb/retinotopy.py
 src/pynwb/spec.py
 src/pynwb/validate.py
 src/pynwb.egg-info/PKG-INFO
 src/pynwb.egg-info/SOURCES.txt
 src/pynwb.egg-info/dependency_links.txt
 src/pynwb.egg-info/not-zip-safe
@@ -153,12 +154,13 @@
 tests/unit/test_icephys.py
 tests/unit/test_icephys_metadata_tables.py
 tests/unit/test_image.py
 tests/unit/test_misc.py
 tests/unit/test_mock.py
 tests/unit/test_ogen.py
 tests/unit/test_ophys.py
+tests/unit/test_resources.py
 tests/unit/test_retinotopy.py
 tests/unit/test_scratch.py
 tests/unit/test_spec.py
 tests/validation/__init__.py
 tests/validation/test_validate.py
```

### Comparing `pynwb-2.3.3/test.py` & `pynwb-2.4.0/test.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/back_compat/1.0.2_nwbfile.nwb` & `pynwb-2.4.0/tests/back_compat/1.0.2_nwbfile.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/back_compat/1.0.2_str_experimenter.nwb` & `pynwb-2.4.0/tests/back_compat/1.0.2_str_experimenter.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/back_compat/1.0.2_str_pub.nwb` & `pynwb-2.4.0/tests/back_compat/1.0.2_str_pub.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/back_compat/1.0.3_nwbfile.nwb` & `pynwb-2.4.0/tests/back_compat/1.0.3_nwbfile.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/back_compat/1.0.3_str_experimenter.nwb` & `pynwb-2.4.0/tests/back_compat/1.0.3_str_experimenter.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/back_compat/1.0.3_str_pub.nwb` & `pynwb-2.4.0/tests/back_compat/1.0.3_str_pub.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/back_compat/1.1.0_nwbfile.nwb` & `pynwb-2.4.0/tests/back_compat/1.1.0_nwbfile.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/back_compat/1.1.0_str_experimenter.nwb` & `pynwb-2.4.0/tests/back_compat/1.1.0_str_experimenter.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/back_compat/1.1.0_str_pub.nwb` & `pynwb-2.4.0/tests/back_compat/1.1.0_str_pub.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/back_compat/1.1.2_nwbfile.nwb` & `pynwb-2.4.0/tests/back_compat/1.1.2_nwbfile.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/back_compat/1.1.2_str_experimenter.nwb` & `pynwb-2.4.0/tests/back_compat/1.1.2_str_experimenter.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/back_compat/1.1.2_str_pub.nwb` & `pynwb-2.4.0/tests/back_compat/1.1.2_str_pub.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/back_compat/1.5.1_imageseries_no_data.nwb` & `pynwb-2.4.0/tests/back_compat/1.5.1_imageseries_no_data.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/back_compat/1.5.1_imageseries_no_unit.nwb` & `pynwb-2.4.0/tests/back_compat/1.5.1_imageseries_no_unit.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/back_compat/1.5.1_timeseries_no_data.nwb` & `pynwb-2.4.0/tests/back_compat/1.5.1_timeseries_no_data.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/back_compat/1.5.1_timeseries_no_unit.nwb` & `pynwb-2.4.0/tests/back_compat/1.5.1_timeseries_no_unit.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/back_compat/2.1.0_imageseries_no_data.nwb` & `pynwb-2.4.0/tests/back_compat/2.1.0_imageseries_no_data.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/back_compat/2.1.0_imageseries_non_external_format.nwb` & `pynwb-2.4.0/tests/back_compat/2.1.0_imageseries_non_external_format.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/back_compat/2.1.0_imageseries_nonmatch_starting_frame.nwb` & `pynwb-2.4.0/tests/back_compat/2.1.0_imageseries_nonmatch_starting_frame.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/back_compat/2.1.0_nwbfile_with_extension.nwb` & `pynwb-2.4.0/tests/back_compat/2.1.0_nwbfile_with_extension.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/back_compat/2.2.0_subject_no_age__reference.nwb` & `pynwb-2.4.0/tests/back_compat/2.2.0_subject_no_age__reference.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/back_compat/test_import_structure.py` & `pynwb-2.4.0/tests/back_compat/test_import_structure.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/back_compat/test_read.py` & `pynwb-2.4.0/tests/back_compat/test_read.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/integration/hdf5/test_base.py` & `pynwb-2.4.0/tests/integration/hdf5/test_base.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/integration/hdf5/test_device.py` & `pynwb-2.4.0/tests/integration/hdf5/test_device.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/integration/hdf5/test_ecephys.py` & `pynwb-2.4.0/tests/integration/hdf5/test_ecephys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/integration/hdf5/test_icephys.py` & `pynwb-2.4.0/tests/integration/hdf5/test_icephys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/integration/hdf5/test_image.py` & `pynwb-2.4.0/tests/integration/hdf5/test_image.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/integration/hdf5/test_io.py` & `pynwb-2.4.0/tests/integration/hdf5/test_io.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/integration/hdf5/test_misc.py` & `pynwb-2.4.0/tests/integration/hdf5/test_misc.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/integration/hdf5/test_modular_storage.py` & `pynwb-2.4.0/tests/integration/hdf5/test_modular_storage.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/integration/hdf5/test_nwbfile.py` & `pynwb-2.4.0/tests/integration/hdf5/test_nwbfile.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/integration/hdf5/test_ogen.py` & `pynwb-2.4.0/tests/integration/hdf5/test_ogen.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/integration/hdf5/test_ophys.py` & `pynwb-2.4.0/tests/integration/hdf5/test_ophys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/integration/hdf5/test_retinotopy.py` & `pynwb-2.4.0/tests/integration/hdf5/test_retinotopy.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/integration/hdf5/test_scratch.py` & `pynwb-2.4.0/tests/integration/hdf5/test_scratch.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/integration/ros3/test_ros3.py` & `pynwb-2.4.0/tests/integration/ros3/test_ros3.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/integration/utils/test_io_utils.py` & `pynwb-2.4.0/tests/integration/utils/test_io_utils.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/read_dandi/test_read_dandi.py` & `pynwb-2.4.0/tests/read_dandi/test_read_dandi.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/unit/test_base.py` & `pynwb-2.4.0/tests/unit/test_base.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/unit/test_behavior.py` & `pynwb-2.4.0/tests/unit/test_behavior.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/unit/test_core.py` & `pynwb-2.4.0/tests/unit/test_core.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/unit/test_core_NWBContainer.py` & `pynwb-2.4.0/tests/unit/test_core_NWBContainer.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/unit/test_ecephys.py` & `pynwb-2.4.0/tests/unit/test_ecephys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/unit/test_epoch.py` & `pynwb-2.4.0/tests/unit/test_epoch.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/unit/test_epoch_legacy.py` & `pynwb-2.4.0/tests/unit/test_epoch_legacy.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/unit/test_extension.py` & `pynwb-2.4.0/tests/unit/test_extension.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/unit/test_file.py` & `pynwb-2.4.0/tests/unit/test_file.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/unit/test_icephys.py` & `pynwb-2.4.0/tests/unit/test_icephys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/unit/test_icephys_metadata_tables.py` & `pynwb-2.4.0/tests/unit/test_icephys_metadata_tables.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/unit/test_image.py` & `pynwb-2.4.0/tests/unit/test_image.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/unit/test_misc.py` & `pynwb-2.4.0/tests/unit/test_misc.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/unit/test_mock.py` & `pynwb-2.4.0/tests/unit/test_mock.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/unit/test_ogen.py` & `pynwb-2.4.0/tests/unit/test_ogen.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/unit/test_ophys.py` & `pynwb-2.4.0/tests/unit/test_ophys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/unit/test_retinotopy.py` & `pynwb-2.4.0/tests/unit/test_retinotopy.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/unit/test_scratch.py` & `pynwb-2.4.0/tests/unit/test_scratch.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/unit/test_spec.py` & `pynwb-2.4.0/tests/unit/test_spec.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tests/validation/test_validate.py` & `pynwb-2.4.0/tests/validation/test_validate.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.3/tox.ini` & `pynwb-2.4.0/tox.ini`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Tox (https://tox.readthedocs.io/) is a tool for running tests
 # in multiple virtualenvs. This configuration file will run the
 # test suite on all supported python versions. To use it, "pip install tox"
 # and then run "tox" from this directory.
 
 [tox]
-envlist = py37, py38, py39, py310, py311
+envlist = py38, py39, py310, py311
 requires = pip >= 22.0
 
 [testenv]
 download = True
 usedevelop = True
 setenv =
   PYTHONDONTWRITEBYTECODE = 1
@@ -57,32 +57,28 @@
 install_command =
     python -m pip install -U --pre {opts} {packages}
 deps =
     -rrequirements-dev.txt
     ; -rrequirements-opt.txt
 commands = {[testenv]commands}
 
-# Test with python 3.7; pinned dev reqs; minimum run reqs
-[testenv:py37-minimum]
-basepython = python3.7
+# Test with python 3.8; pinned dev reqs; minimum run reqs
+[testenv:py38-minimum]
+basepython = python3.8
 deps =
     -rrequirements-dev.txt
     -rrequirements-min.txt
 commands = {[testenv]commands}
 
 # Envs that builds wheels and source distribution
 [testenv:build]
 commands =
     python -m pip install --upgrade build
     python -m build
 
-[testenv:build-py37]
-basepython = python3.7
-commands = {[testenv:build]commands}
-
 [testenv:build-py38]
 basepython = python3.8
 commands = {[testenv:build]commands}
 
 [testenv:build-py39]
 basepython = python3.9
 commands = {[testenv:build]commands}
@@ -116,16 +112,16 @@
 install_command =
     python -m pip install -U --pre {opts} {packages}
 deps =
     -rrequirements-dev.txt
     ; -rrequirements-opt.txt
 commands = {[testenv:build]commands}
 
-[testenv:build-py37-minimum]
-basepython = python3.7
+[testenv:build-py38-minimum]
+basepython = python3.8
 deps =
     -rrequirements-dev.txt
     -rrequirements-min.txt
 commands = {[testenv:build]commands}
 
 # Envs that will test installation from a wheel
 [testenv:wheelinstall]
@@ -142,19 +138,14 @@
 commands =
     python -m pip install -e .
     python -m pip install -r requirements-doc.txt  # NOTE: allensdk (requirements-doc.txt) requires pynwb
     python -m pip check
     python -m pip list
     python test.py --example
 
-[testenv:gallery-py37]
-basepython = python3.7
-deps = {[testenv:gallery]deps}
-commands = {[testenv:gallery]commands}
-
 [testenv:gallery-py38]
 basepython = python3.8
 deps = {[testenv:gallery]deps}
 commands = {[testenv:gallery]commands}
 
 [testenv:gallery-py39]
 basepython = python3.9
@@ -191,13 +182,13 @@
 commands =
     python -m pip install -U --pre -e .
     python -m pip install -r requirements-doc.txt  # NOTE: allensdk (requirements-doc.txt) requires pynwb
     python -m pip check
     python -m pip list
     python test.py --example
 
-# Test with python 3.7; pinned dev and doc reqs; minimum run reqs
-[testenv:gallery-py37-minimum]
-basepython = python3.7
+# Test with python 3.8; pinned dev and doc reqs; minimum run reqs
+[testenv:gallery-py38-minimum]
+basepython = python3.8
 deps =
     -rrequirements-min.txt
-commands = {[testenv:gallery]commands}
+commands = {[testenv:gallery]commands}
```

### Comparing `pynwb-2.3.3/versioneer.py` & `pynwb-2.4.0/versioneer.py`

 * *Files identical despite different names*

