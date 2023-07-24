# Comparing `tmp/careless-0.3.4.tar.gz` & `tmp/careless-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "careless-0.3.4.tar", last modified: Fri Jul 14 01:42:47 2023, max compression
+gzip compressed data, was "careless-0.3.5.tar", last modified: Mon Jul 24 01:00:40 2023, max compression
```

## Comparing `careless-0.3.4.tar` & `careless-0.3.5.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:47.234871 careless-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-14 01:42:35.000000 careless-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-14 01:42:35.000000 careless-0.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-14 01:42:47.234871 careless-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-07-14 01:42:35.000000 careless-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:47.226871 careless-0.3.4/careless/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 01:42:35.000000 careless-0.3.4/careless/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-14 01:42:35.000000 careless-0.3.4/careless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:47.230871 careless-0.3.4/careless/args/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-14 01:42:35.000000 careless-0.3.4/careless/args/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-14 01:42:35.000000 careless-0.3.4/careless/args/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-14 01:42:35.000000 careless-0.3.4/careless/args/crossvalidation.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-14 01:42:35.000000 careless-0.3.4/careless/args/filtration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-14 01:42:35.000000 careless-0.3.4/careless/args/interpretation.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-14 01:42:35.000000 careless-0.3.4/careless/args/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-14 01:42:35.000000 careless-0.3.4/careless/args/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-14 01:42:35.000000 careless-0.3.4/careless/args/poly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-14 01:42:35.000000 careless-0.3.4/careless/args/positional_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-14 01:42:35.000000 careless-0.3.4/careless/args/prior.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-14 01:42:35.000000 careless-0.3.4/careless/args/required.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-14 01:42:35.000000 careless-0.3.4/careless/args/scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-14 01:42:35.000000 careless-0.3.4/careless/args/tf_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:47.230871 careless-0.3.4/careless/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:35.000000 careless-0.3.4/careless/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-14 01:42:35.000000 careless-0.3.4/careless/callbacks/progress_bar.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4677 2023-07-14 01:42:35.000000 careless-0.3.4/careless/careless.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:47.230871 careless-0.3.4/careless/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:35.000000 careless-0.3.4/careless/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-07-14 01:42:35.000000 careless-0.3.4/careless/io/asu.py
--rw-r--r--   0 runner    (1001) docker     (123)    22179 2023-07-14 01:42:35.000000 careless-0.3.4/careless/io/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-07-14 01:42:35.000000 careless-0.3.4/careless/io/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-07-14 01:42:35.000000 careless-0.3.4/careless/io/xds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:47.230871 careless-0.3.4/careless/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:35.000000 careless-0.3.4/careless/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-07-14 01:42:35.000000 careless-0.3.4/careless/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:47.230871 careless-0.3.4/careless/models/likelihoods/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 01:42:35.000000 careless-0.3.4/careless/models/likelihoods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-14 01:42:35.000000 careless-0.3.4/careless/models/likelihoods/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-07-14 01:42:35.000000 careless-0.3.4/careless/models/likelihoods/laue.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-14 01:42:35.000000 careless-0.3.4/careless/models/likelihoods/mono.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:47.230871 careless-0.3.4/careless/models/merging/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-14 01:42:35.000000 careless-0.3.4/careless/models/merging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-07-14 01:42:35.000000 careless-0.3.4/careless/models/merging/surrogate_posteriors.py
--rw-r--r--   0 runner    (1001) docker     (123)     9129 2023-07-14 01:42:35.000000 careless-0.3.4/careless/models/merging/variational.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:47.230871 careless-0.3.4/careless/models/priors/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-14 01:42:35.000000 careless-0.3.4/careless/models/priors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-14 01:42:35.000000 careless-0.3.4/careless/models/priors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-07-14 01:42:35.000000 careless-0.3.4/careless/models/priors/empirical.py
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-14 01:42:35.000000 careless-0.3.4/careless/models/priors/wilson.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:47.230871 careless-0.3.4/careless/models/scaling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:35.000000 careless-0.3.4/careless/models/scaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-14 01:42:35.000000 careless-0.3.4/careless/models/scaling/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-07-14 01:42:35.000000 careless-0.3.4/careless/models/scaling/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-07-14 01:42:35.000000 careless-0.3.4/careless/models/scaling/nn.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4389 2023-07-14 01:42:35.000000 careless-0.3.4/careless/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:47.230871 careless-0.3.4/careless/stats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:35.000000 careless-0.3.4/careless/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-07-14 01:42:35.000000 careless-0.3.4/careless/stats/ccanom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-14 01:42:35.000000 careless-0.3.4/careless/stats/cchalf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-07-14 01:42:35.000000 careless-0.3.4/careless/stats/ccpred.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-14 01:42:35.000000 careless-0.3.4/careless/stats/completeness.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-14 01:42:35.000000 careless-0.3.4/careless/stats/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-07-14 01:42:35.000000 careless-0.3.4/careless/stats/prior_b.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-14 01:42:35.000000 careless-0.3.4/careless/stats/rescale.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-14 01:42:35.000000 careless-0.3.4/careless/stats/rsplit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:47.230871 careless-0.3.4/careless/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:35.000000 careless-0.3.4/careless/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-14 01:42:35.000000 careless-0.3.4/careless/utils/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    12859 2023-07-14 01:42:35.000000 careless-0.3.4/careless/utils/distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-14 01:42:35.000000 careless-0.3.4/careless/utils/laue.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-14 01:42:35.000000 careless-0.3.4/careless/utils/positional_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-14 01:42:35.000000 careless-0.3.4/careless/utils/shame.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:47.226871 careless-0.3.4/careless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-14 01:42:47.000000 careless-0.3.4/careless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-14 01:42:47.000000 careless-0.3.4/careless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 01:42:47.000000 careless-0.3.4/careless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-14 01:42:47.000000 careless-0.3.4/careless.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-14 01:42:47.000000 careless-0.3.4/careless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-14 01:42:47.000000 careless-0.3.4/careless.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:47.230871 careless-0.3.4/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3872 2023-07-14 01:42:35.000000 careless-0.3.4/scripts/make_difference_map
--rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-07-14 01:42:35.000000 careless-0.3.4/scripts/stream2mtz
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-14 01:42:47.234871 careless-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-14 01:42:35.000000 careless-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:47.234871 careless-0.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:35.000000 careless-0.3.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-07-14 01:42:35.000000 careless-0.3.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-07-14 01:42:35.000000 careless-0.3.4/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:40.425135 careless-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-24 01:00:26.000000 careless-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 01:00:26.000000 careless-0.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-24 01:00:40.425135 careless-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9047 2023-07-24 01:00:26.000000 careless-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:40.421135 careless-0.3.5/careless/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 01:00:26.000000 careless-0.3.5/careless/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-24 01:00:26.000000 careless-0.3.5/careless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:40.421135 careless-0.3.5/careless/args/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-24 01:00:26.000000 careless-0.3.5/careless/args/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-24 01:00:26.000000 careless-0.3.5/careless/args/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-24 01:00:26.000000 careless-0.3.5/careless/args/crossvalidation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-24 01:00:26.000000 careless-0.3.5/careless/args/filtration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-24 01:00:26.000000 careless-0.3.5/careless/args/interpretation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-24 01:00:26.000000 careless-0.3.5/careless/args/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-24 01:00:26.000000 careless-0.3.5/careless/args/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-24 01:00:26.000000 careless-0.3.5/careless/args/poly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-24 01:00:26.000000 careless-0.3.5/careless/args/positional_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-24 01:00:26.000000 careless-0.3.5/careless/args/prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-24 01:00:26.000000 careless-0.3.5/careless/args/required.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-24 01:00:26.000000 careless-0.3.5/careless/args/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-24 01:00:26.000000 careless-0.3.5/careless/args/tf_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:40.421135 careless-0.3.5/careless/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:26.000000 careless-0.3.5/careless/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-24 01:00:26.000000 careless-0.3.5/careless/callbacks/progress_bar.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4677 2023-07-24 01:00:26.000000 careless-0.3.5/careless/careless.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:40.421135 careless-0.3.5/careless/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:26.000000 careless-0.3.5/careless/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-07-24 01:00:26.000000 careless-0.3.5/careless/io/asu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22179 2023-07-24 01:00:26.000000 careless-0.3.5/careless/io/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-07-24 01:00:26.000000 careless-0.3.5/careless/io/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-07-24 01:00:26.000000 careless-0.3.5/careless/io/xds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:40.421135 careless-0.3.5/careless/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:26.000000 careless-0.3.5/careless/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-07-24 01:00:26.000000 careless-0.3.5/careless/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:40.421135 careless-0.3.5/careless/models/likelihoods/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 01:00:26.000000 careless-0.3.5/careless/models/likelihoods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-24 01:00:26.000000 careless-0.3.5/careless/models/likelihoods/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-07-24 01:00:26.000000 careless-0.3.5/careless/models/likelihoods/laue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-24 01:00:26.000000 careless-0.3.5/careless/models/likelihoods/mono.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:40.421135 careless-0.3.5/careless/models/merging/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-24 01:00:26.000000 careless-0.3.5/careless/models/merging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-07-24 01:00:26.000000 careless-0.3.5/careless/models/merging/surrogate_posteriors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9129 2023-07-24 01:00:26.000000 careless-0.3.5/careless/models/merging/variational.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:40.421135 careless-0.3.5/careless/models/priors/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-24 01:00:26.000000 careless-0.3.5/careless/models/priors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-24 01:00:26.000000 careless-0.3.5/careless/models/priors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-07-24 01:00:26.000000 careless-0.3.5/careless/models/priors/empirical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-24 01:00:26.000000 careless-0.3.5/careless/models/priors/wilson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:40.425135 careless-0.3.5/careless/models/scaling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:26.000000 careless-0.3.5/careless/models/scaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-24 01:00:26.000000 careless-0.3.5/careless/models/scaling/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-07-24 01:00:26.000000 careless-0.3.5/careless/models/scaling/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-07-24 01:00:26.000000 careless-0.3.5/careless/models/scaling/nn.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4389 2023-07-24 01:00:26.000000 careless-0.3.5/careless/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:40.425135 careless-0.3.5/careless/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:26.000000 careless-0.3.5/careless/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-07-24 01:00:26.000000 careless-0.3.5/careless/stats/ccanom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-24 01:00:26.000000 careless-0.3.5/careless/stats/cchalf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-07-24 01:00:26.000000 careless-0.3.5/careless/stats/ccpred.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-24 01:00:26.000000 careless-0.3.5/careless/stats/completeness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-24 01:00:26.000000 careless-0.3.5/careless/stats/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-07-24 01:00:26.000000 careless-0.3.5/careless/stats/prior_b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-24 01:00:26.000000 careless-0.3.5/careless/stats/rescale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-24 01:00:26.000000 careless-0.3.5/careless/stats/rsplit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:40.425135 careless-0.3.5/careless/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:26.000000 careless-0.3.5/careless/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-24 01:00:26.000000 careless-0.3.5/careless/utils/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12859 2023-07-24 01:00:26.000000 careless-0.3.5/careless/utils/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-24 01:00:26.000000 careless-0.3.5/careless/utils/laue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-24 01:00:26.000000 careless-0.3.5/careless/utils/positional_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-24 01:00:26.000000 careless-0.3.5/careless/utils/shame.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:40.421135 careless-0.3.5/careless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-24 01:00:40.000000 careless-0.3.5/careless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-24 01:00:40.000000 careless-0.3.5/careless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 01:00:40.000000 careless-0.3.5/careless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-24 01:00:40.000000 careless-0.3.5/careless.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-24 01:00:40.000000 careless-0.3.5/careless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-24 01:00:40.000000 careless-0.3.5/careless.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:40.425135 careless-0.3.5/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3872 2023-07-24 01:00:26.000000 careless-0.3.5/scripts/make_difference_map
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-07-24 01:00:26.000000 careless-0.3.5/scripts/stream2mtz
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-24 01:00:40.425135 careless-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-24 01:00:26.000000 careless-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:40.425135 careless-0.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 01:00:26.000000 careless-0.3.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-07-24 01:00:26.000000 careless-0.3.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-07-24 01:00:26.000000 careless-0.3.5/tests/test_cli.py
```

### Comparing `careless-0.3.4/LICENSE` & `careless-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `careless-0.3.4/PKG-INFO` & `careless-0.3.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: careless
-Version: 0.3.4
+Version: 0.3.5
 Summary: Merging crystallography data without much physics.
 Home-page: https://github.com/rs-station/careless
 Author: Kevin M. Dalton
 Author-email: kmdalton@fas.harvard.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/rs-station/careless/issues
 Project-URL: Source Code, https://github.com/rs-station/careless
```

### Comparing `careless-0.3.4/README.md` & `careless-0.3.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -15,20 +15,39 @@
 conda create -yn careless python
 conda activate careless
 pip install --upgrade pip
 pip install careless
 ```
 
 ## Installation with GPU Support
-Careless supports GPU acceleration on NVIDIA GPUs. Prior to installing careless, install the 
+Careless supports GPU acceleration on NVIDIA GPUs. For users who would like to run `careless` in a cluster computing environment, requesting an interactive GPU node for the installation might be helpful. You may want to first follow the latest [Tensorflow installation instructions](https://www.tensorflow.org/install/pip#step-by-step_instructions) and then install `careless`. Specifically, 
+1) Create and activate a new environment with the appropriate Python version
+   ```bash
+   conda create -yn careless python=checktheversion
+   conda activate careless
+   pip install --upgrade pip
+   ```
+2) Install dependencies for GPU support (see the following paragraph)
+3) Install TensorFlow (and verify its GPU support)
+   ```bash
+   pip install tensorflow==checktheversion
+   #check that tensorflow sees the correct number of GPUs
+   python3 -c "import tensorflow as tf; print(len(tf.config.list_physical_devices('GPU')))"
+   ```
+4) Install `careless`
+   ```bash
+   pip install careless
+   ```
+
+The following dependencies are required for GPU support 
  - NVIDIA driver, 
  - CUDA Toolkit, and 
  - cuDNN. 
 
-For these dependencies, you can determine the versions required by the latest TensorFlow release from the [TensorFlow docs](https://www.tensorflow.org/install/pip#software_requirements). The driver is usually installed through the system package manager and will require root privileges. In a cluster computing environment, a suitable version of the NVIDIA driver will usually be provided by your system administrators. The two libraries, CUDA toolkit and cuDNN, may either be installed through the system package manager or using the Anaconda python distribution as described in the [TensorFlow docs](https://www.tensorflow.org/install/pip#step-by-step_instructions). 
+You can determine the versions required by the latest TensorFlow release from the [TensorFlow docs](https://www.tensorflow.org/install/pip#software_requirements). The driver is usually installed through the system package manager and will require root privileges. In a cluster computing environment, a suitable version of the NVIDIA driver will usually be provided by your system administrators. The two libraries, CUDA toolkit and cuDNN, may either be installed through the system package manager or using the Anaconda python distribution as described in the [TensorFlow docs](https://www.tensorflow.org/install/pip#step-by-step_instructions). 
 
 You may confirm GPU acceleration is active using the `nvidia-smi` command to monitor GPU usage during model training. If you are having trouble enabling GPU support, you may want to use the `--tf-debug` flag during training for verbose logging of TensorFlow issues. 
 
 ## Dependencies
 
 `careless` is likely to run on any operating system which is compatible with TensorFlow. 
 `careless` currently supports __Python 3.8 - 3.10__. 
@@ -37,15 +56,15 @@
  - optimization routines from [TensorFlow](https://www.tensorflow.org/)
  - statistical distributions from [Tensorflow-Probability](https://www.tensorflow.org/probability)
  - crystallographic computing resources from 
     - [ReciprocalSpaceship](https://rs-station.github.io/reciprocalspaceship/)
     - [GEMMI](https://gemmi.readthedocs.io/en/latest/)
 
 
-`careless` does not require but may take advantage of various accelator cards supported by TensorFlow. To 
+`careless` does not require but may take advantage of various accelator cards supported by TensorFlow.
 
 ## Get Help
 For help with command line arguments, type `careless mono --help` for monochromatic or `careless poly --help` for Laue processing options. 
 
 For usage examples and data from the [preprint](https://doi.org/10.1101/2021.01.05.425510), check out [careless-examples](https://github.com/rs-station/careless-examples)
 
 Still confused? File an [issue](https://github.com/rs-station/careless/issues/new/choose)! Issues help us improve our code base and leave a public record for other users.
```

### Comparing `careless-0.3.4/careless/args/common.py` & `careless-0.3.5/careless/args/common.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.4/careless/args/crossvalidation.py` & `careless-0.3.5/careless/args/crossvalidation.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.4/careless/args/filtration.py` & `careless-0.3.5/careless/args/filtration.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.4/careless/args/interpretation.py` & `careless-0.3.5/careless/args/interpretation.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.4/careless/args/optimizer.py` & `careless-0.3.5/careless/args/optimizer.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.4/careless/args/poly.py` & `careless-0.3.5/careless/args/poly.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.4/careless/args/positional_encoding.py` & `careless-0.3.5/careless/args/positional_encoding.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.4/careless/args/prior.py` & `careless-0.3.5/careless/args/prior.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.4/careless/args/required.py` & `careless-0.3.5/careless/args/required.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.4/careless/args/scaling.py` & `careless-0.3.5/careless/args/scaling.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.4/careless/args/tf_options.py` & `careless-0.3.5/careless/args/tf_options.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.4/careless/callbacks/progress_bar.py` & `careless-0.3.5/careless/callbacks/progress_bar.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.4/careless/careless.py` & `careless-0.3.5/careless/careless.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.4/careless/io/asu.py` & `careless-0.3.5/careless/io/asu.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.4/careless/io/formatter.py` & `careless-0.3.5/careless/io/formatter.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.4/careless/io/manager.py` & `careless-0.3.5/careless/io/manager.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.4/careless/io/xds.py` & `careless-0.3.5/careless/io/xds.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.4/careless/models/base.py` & `careless-0.3.5/careless/models/base.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.4/careless/models/likelihoods/laue.py` & `careless-0.3.5/careless/models/likelihoods/laue.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.4/careless/models/likelihoods/mono.py` & `careless-0.3.5/careless/models/likelihoods/mono.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.4/careless/models/merging/surrogate_posteriors.py` & `careless-0.3.5/careless/models/merging/surrogate_posteriors.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -119,16 +119,16 @@
         loc   = tfp.util.TransformedVariable(
             loc,
             tfb.Exp(),
         )
         scale = tfp.util.TransformedVariable(
             scale,
             tfb.Chain([
-                tfb.Exp(),
                 tfb.Shift(scale_shift),
+                tfb.Exp(),
             ]),
         )
         return cls(loc, scale, low, high)
 
 class RiceWoolfson(tfd.Distribution):
     def __init__(self, loc, scale, centric):
         """
```

### Comparing `careless-0.3.4/careless/models/merging/variational.py` & `careless-0.3.5/careless/models/merging/variational.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.4/careless/models/priors/empirical.py` & `careless-0.3.5/careless/models/priors/empirical.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.4/careless/models/priors/wilson.py` & `careless-0.3.5/careless/models/priors/wilson.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.4/careless/models/scaling/image.py` & `careless-0.3.5/careless/models/scaling/image.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.4/careless/models/scaling/nn.py` & `careless-0.3.5/careless/models/scaling/nn.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.4/careless/parser.py` & `careless-0.3.5/careless/parser.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.4/careless/stats/ccanom.py` & `careless-0.3.5/careless/stats/ccanom.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.4/careless/stats/cchalf.py` & `careless-0.3.5/careless/stats/cchalf.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.4/careless/stats/ccpred.py` & `careless-0.3.5/careless/stats/ccpred.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.4/careless/stats/completeness.py` & `careless-0.3.5/careless/stats/completeness.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.4/careless/stats/parser.py` & `careless-0.3.5/careless/stats/parser.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.4/careless/stats/prior_b.py` & `careless-0.3.5/careless/stats/prior_b.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.4/careless/stats/rescale.py` & `careless-0.3.5/careless/stats/rescale.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.4/careless/stats/rsplit.py` & `careless-0.3.5/careless/stats/rsplit.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.4/careless/utils/distributions.py` & `careless-0.3.5/careless/utils/distributions.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.4/careless/utils/laue.py` & `careless-0.3.5/careless/utils/laue.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.4/careless/utils/positional_encoding.py` & `careless-0.3.5/careless/utils/positional_encoding.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.4/careless.egg-info/PKG-INFO` & `careless-0.3.5/careless.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: careless
-Version: 0.3.4
+Version: 0.3.5
 Summary: Merging crystallography data without much physics.
 Home-page: https://github.com/rs-station/careless
 Author: Kevin M. Dalton
 Author-email: kmdalton@fas.harvard.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/rs-station/careless/issues
 Project-URL: Source Code, https://github.com/rs-station/careless
```

### Comparing `careless-0.3.4/careless.egg-info/SOURCES.txt` & `careless-0.3.5/careless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `careless-0.3.4/scripts/make_difference_map` & `careless-0.3.5/scripts/make_difference_map`

 * *Files identical despite different names*

### Comparing `careless-0.3.4/scripts/stream2mtz` & `careless-0.3.5/scripts/stream2mtz`

 * *Files identical despite different names*

### Comparing `careless-0.3.4/setup.py` & `careless-0.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.4/tests/conftest.py` & `careless-0.3.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.4/tests/test_cli.py` & `careless-0.3.5/tests/test_cli.py`

 * *Files identical despite different names*

