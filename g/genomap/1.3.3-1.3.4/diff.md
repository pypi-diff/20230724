# Comparing `tmp/genomap-1.3.3.tar.gz` & `tmp/genomap-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genomap-1.3.3.tar", last modified: Mon Jul 24 20:07:25 2023, max compression
+gzip compressed data, was "genomap-1.3.4.tar", last modified: Mon Jul 24 20:37:36 2023, max compression
```

## Comparing `genomap-1.3.3.tar` & `genomap-1.3.4.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:07:25.653547 genomap-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-24 20:02:37.000000 genomap-1.3.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-24 20:02:37.000000 genomap-1.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13646 2023-07-24 20:07:25.653547 genomap-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13212 2023-07-24 20:02:37.000000 genomap-1.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:07:25.617547 genomap-1.3.3/data/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-24 20:02:37.000000 genomap-1.3.3/data/TM_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:07:25.617547 genomap-1.3.3/genomap/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:07:25.621547 genomap-1.3.3/genomap/bregman_genomap/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/bregman_genomap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   125058 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/bregman_genomap/bregman_genomap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:07:25.621547 genomap-1.3.3/genomap/genoAnnotate/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoAnnotate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoAnnotate/genoAnnotate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:07:25.625547 genomap-1.3.3/genomap/genoClassification/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoClassification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoClassification/genoClassification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:07:25.625547 genomap-1.3.3/genomap/genoDR/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoDR/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoDR/genoDimReduction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:07:25.625547 genomap-1.3.3/genomap/genoMOI/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoMOI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoMOI/genoMOI.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:07:25.629547 genomap-1.3.3/genomap/genoNet/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoNet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoNet/genoNet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:07:25.629547 genomap-1.3.3/genomap/genoNetRegression/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoNetRegression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoNetRegression/genoNet_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:07:25.633547 genomap-1.3.3/genomap/genoNetus/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoNetus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoNetus/genoNetus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:07:25.633547 genomap-1.3.3/genomap/genoRegression/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoRegression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoRegression/genoRegression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:07:25.633547 genomap-1.3.3/genomap/genoSig/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoSig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoSig/genoSig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:07:25.637547 genomap-1.3.3/genomap/genoTraj/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoTraj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoTraj/genoTraj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:07:25.641547 genomap-1.3.3/genomap/genoVis/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoVis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoVis/genoVis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genomap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:07:25.641547 genomap-1.3.3/genomap/genomapOPT/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genomapOPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genomapOPT/genomapOPT.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:07:25.641547 genomap-1.3.3/genomap/genomapT/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genomapT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genomapT/genomapT.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:07:25.645547 genomap-1.3.3/genomap/genotype/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genotype/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9775 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genotype/genotype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:07:25.653547 genomap-1.3.3/genomap/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/utils/ConvDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/utils/ConvIDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/utils/FcDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/utils/FcIDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/utils/class_discriminative_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/utils/gTraj_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/utils/group_centroid_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/utils/util_Sig.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/utils/util_genoClassReg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/utils/utils_MOI.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:07:25.621547 genomap-1.3.3/genomap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13646 2023-07-24 20:07:25.000000 genomap-1.3.3/genomap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-24 20:07:25.000000 genomap-1.3.3/genomap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 20:07:25.000000 genomap-1.3.3/genomap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-24 20:07:25.000000 genomap-1.3.3/genomap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 20:07:25.000000 genomap-1.3.3/genomap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-24 20:02:37.000000 genomap-1.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 20:07:25.653547 genomap-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-24 20:02:37.000000 genomap-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:37:36.674315 genomap-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-24 20:33:40.000000 genomap-1.3.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-24 20:33:40.000000 genomap-1.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13688 2023-07-24 20:37:36.674315 genomap-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13254 2023-07-24 20:33:40.000000 genomap-1.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:37:36.658315 genomap-1.3.4/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-24 20:33:40.000000 genomap-1.3.4/data/TM_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:37:36.658315 genomap-1.3.4/genomap/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:37:36.662315 genomap-1.3.4/genomap/bregman_genomap/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/bregman_genomap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125058 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/bregman_genomap/bregman_genomap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:37:36.662315 genomap-1.3.4/genomap/genoAnnotate/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoAnnotate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoAnnotate/genoAnnotate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:37:36.662315 genomap-1.3.4/genomap/genoClassification/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoClassification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoClassification/genoClassification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:37:36.662315 genomap-1.3.4/genomap/genoDR/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoDR/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoDR/genoDimReduction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:37:36.662315 genomap-1.3.4/genomap/genoMOI/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoMOI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoMOI/genoMOI.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:37:36.666315 genomap-1.3.4/genomap/genoNet/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoNet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoNet/genoNet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:37:36.666315 genomap-1.3.4/genomap/genoNetRegression/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoNetRegression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoNetRegression/genoNet_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:37:36.666315 genomap-1.3.4/genomap/genoNetus/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoNetus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoNetus/genoNetus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:37:36.666315 genomap-1.3.4/genomap/genoRegression/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoRegression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoRegression/genoRegression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:37:36.666315 genomap-1.3.4/genomap/genoSig/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoSig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoSig/genoSig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:37:36.666315 genomap-1.3.4/genomap/genoTraj/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoTraj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoTraj/genoTraj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:37:36.666315 genomap-1.3.4/genomap/genoVis/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoVis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoVis/genoVis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genomap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:37:36.670315 genomap-1.3.4/genomap/genomapOPT/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genomapOPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genomapOPT/genomapOPT.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:37:36.670315 genomap-1.3.4/genomap/genomapT/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genomapT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genomapT/genomapT.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:37:36.670315 genomap-1.3.4/genomap/genotype/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genotype/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9775 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genotype/genotype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:37:36.674315 genomap-1.3.4/genomap/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/utils/ConvDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/utils/ConvIDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/utils/FcDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/utils/FcIDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/utils/class_discriminative_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/utils/gTraj_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/utils/group_centroid_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/utils/util_Sig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/utils/util_genoClassReg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/utils/utils_MOI.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:37:36.662315 genomap-1.3.4/genomap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13688 2023-07-24 20:37:36.000000 genomap-1.3.4/genomap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-24 20:37:36.000000 genomap-1.3.4/genomap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 20:37:36.000000 genomap-1.3.4/genomap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-24 20:37:36.000000 genomap-1.3.4/genomap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 20:37:36.000000 genomap-1.3.4/genomap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-24 20:33:40.000000 genomap-1.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 20:37:36.674315 genomap-1.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-24 20:33:40.000000 genomap-1.3.4/setup.py
```

### Comparing `genomap-1.3.3/LICENSE.txt` & `genomap-1.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `genomap-1.3.3/PKG-INFO` & `genomap-1.3.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: genomap
-Version: 1.3.3
-Summary: Genomap converts tabular gene expression data into spatially meaningful images.
-Home-page: https://github.com/xinglab-ai/genomap
-Author: Md Tauhidul Islam
-Author-email: tauhid@stanford.edu
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # Genomap creates images from gene expression data and offers high-performance dimensionality reduction and visualization, data clustering, classification and regression, gene signature extraction, multi-omics data integration, and trajectory analysis 
 
 Genomap is an entropy-based cartography strategy to contrive the high dimensional gene expression data into a configured image format with explicit integration of the genomic interactions. This unique cartography casts the gene-gene interactions into a spatial configuration and enables us to extract the deep genomic interaction features and discover underlying discriminative patterns of the data. For a wide variety of applications (cell clustering and recognition, gene signature extraction, single-cell data integration, cellular trajectory analysis, dimensionality reduction, and visualization), genomap drastically improves the accuracy of data analyses as compared to state-of-the-art techniques.
 
 ## How to use genomap
 
 The easiest way to start with genomap is to install it from pypi using 
@@ -65,15 +52,15 @@
 import numpy as np
 import pandas as pd
 import genomap.genoVis as gp
 import matplotlib.pyplot as plt
 from sklearn.cluster import KMeans
 from sklearn.decomposition import PCA
 import phate
-import umap
+import umap.umap_ as umap
 
 data = pd.read_csv('TM_data.csv', header=None,
                    delim_whitespace=False)
 data=data.values
 gt_data = sio.loadmat('GT_TM.mat')
 y = np.squeeze(gt_data['GT'])
 n_clusters = len(np.unique(y))
@@ -102,15 +89,15 @@
 ### Example 3 - Try genoDR for dimensionality reduction
 
 ```python
 import scipy.io as sio
 import numpy as np
 import genomap.genoDR as gp
 import matplotlib.pyplot as plt
-import umap
+import umap.umap_ as umap
 
 dx = sio.loadmat('reducedData_divseq.mat')
 data=dx['X']
 gt_data = sio.loadmat('GT_divseq.mat')
 y = np.squeeze(gt_data['GT'])
 n_clusters = len(np.unique(y))
 
@@ -136,15 +123,15 @@
 import scipy.io as sio
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 from sklearn.cluster import KMeans
 from sklearn.decomposition import PCA
 import phate
-import umap
+import umap.umap_ as umap
 import genomap.genoTraj as gp
 
 # Load data
 dx = sio.loadmat('organoidData.mat')
 data=dx['X3']
 gt_data = sio.loadmat('cellsPsudo.mat')
 Y_time = np.squeeze(gt_data['newGT'])
```

### Comparing `genomap-1.3.3/README.md` & `genomap-1.3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: genomap
+Version: 1.3.4
+Summary: Genomap converts tabular gene expression data into spatially meaningful images.
+Home-page: https://github.com/xinglab-ai/genomap
+Author: Md Tauhidul Islam
+Author-email: tauhid@stanford.edu
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # Genomap creates images from gene expression data and offers high-performance dimensionality reduction and visualization, data clustering, classification and regression, gene signature extraction, multi-omics data integration, and trajectory analysis 
 
 Genomap is an entropy-based cartography strategy to contrive the high dimensional gene expression data into a configured image format with explicit integration of the genomic interactions. This unique cartography casts the gene-gene interactions into a spatial configuration and enables us to extract the deep genomic interaction features and discover underlying discriminative patterns of the data. For a wide variety of applications (cell clustering and recognition, gene signature extraction, single-cell data integration, cellular trajectory analysis, dimensionality reduction, and visualization), genomap drastically improves the accuracy of data analyses as compared to state-of-the-art techniques.
 
 ## How to use genomap
 
 The easiest way to start with genomap is to install it from pypi using 
@@ -52,15 +65,15 @@
 import numpy as np
 import pandas as pd
 import genomap.genoVis as gp
 import matplotlib.pyplot as plt
 from sklearn.cluster import KMeans
 from sklearn.decomposition import PCA
 import phate
-import umap
+import umap.umap_ as umap
 
 data = pd.read_csv('TM_data.csv', header=None,
                    delim_whitespace=False)
 data=data.values
 gt_data = sio.loadmat('GT_TM.mat')
 y = np.squeeze(gt_data['GT'])
 n_clusters = len(np.unique(y))
@@ -89,15 +102,15 @@
 ### Example 3 - Try genoDR for dimensionality reduction
 
 ```python
 import scipy.io as sio
 import numpy as np
 import genomap.genoDR as gp
 import matplotlib.pyplot as plt
-import umap
+import umap.umap_ as umap
 
 dx = sio.loadmat('reducedData_divseq.mat')
 data=dx['X']
 gt_data = sio.loadmat('GT_divseq.mat')
 y = np.squeeze(gt_data['GT'])
 n_clusters = len(np.unique(y))
 
@@ -123,15 +136,15 @@
 import scipy.io as sio
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 from sklearn.cluster import KMeans
 from sklearn.decomposition import PCA
 import phate
-import umap
+import umap.umap_ as umap
 import genomap.genoTraj as gp
 
 # Load data
 dx = sio.loadmat('organoidData.mat')
 data=dx['X3']
 gt_data = sio.loadmat('cellsPsudo.mat')
 Y_time = np.squeeze(gt_data['newGT'])
```

### Comparing `genomap-1.3.3/genomap/bregman_genomap/bregman_genomap.py` & `genomap-1.3.4/genomap/bregman_genomap/bregman_genomap.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.3/genomap/genoAnnotate/genoAnnotate.py` & `genomap-1.3.4/genomap/genoAnnotate/genoAnnotate.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.3/genomap/genoClassification/genoClassification.py` & `genomap-1.3.4/genomap/genoClassification/genoClassification.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.3/genomap/genoDR/genoDimReduction.py` & `genomap-1.3.4/genomap/genoDR/genoDimReduction.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 @author: Md Tauhidul Islam, Ph.D., Dept. of Radiation Oncology, Stanford University
 """
 import numpy as np
 import pandas as pd
 import scanpy as sc
 from sklearn.feature_selection import VarianceThreshold
 from tensorflow.keras.optimizers import Adam
-import umap
+import umap.umap_ as umap
 
 from genomap.genomap import construct_genomap
 from genomap.utils.ConvIDEC import ConvIDEC
 from genomap.utils.gTraj_utils import nearest_divisible_by_four
 from genomap.utils.util_Sig import select_n_features
 
 def genoDR(data,n_dim=32, n_clusters=None, colNum=32,rowNum=32,batch_size=64,verbose=1,
```

### Comparing `genomap-1.3.3/genomap/genoMOI/genoMOI.py` & `genomap-1.3.4/genomap/genoMOI/genoMOI.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 Created on Wed Jul 12 16:11:15 2023
 
 @author: Md Tauhidul Islam, Ph.D., Dept. of Radiation Oncology, Stanford University
 """
 
 from tensorflow.keras.optimizers import Adam
-import umap
+import umap.umap_ as umap
 import numpy as np
 import scanorama
 import phate
 import scanpy as sc
 import scipy.io
 import pandas as pd
 import anndata as ad
```

### Comparing `genomap-1.3.3/genomap/genoNet/genoNet.py` & `genomap-1.3.4/genomap/genoNet/genoNet.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.3/genomap/genoNetRegression/genoNet_regression.py` & `genomap-1.3.4/genomap/genoNetRegression/genoNet_regression.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.3/genomap/genoNetus/genoNetus.py` & `genomap-1.3.4/genomap/genoNetus/genoNetus.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.3/genomap/genoRegression/genoRegression.py` & `genomap-1.3.4/genomap/genoRegression/genoRegression.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.3/genomap/genoSig/genoSig.py` & `genomap-1.3.4/genomap/genoSig/genoSig.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.3/genomap/genoTraj/genoTraj.py` & `genomap-1.3.4/genomap/genoTraj/genoTraj.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.3/genomap/genoVis/genoVis.py` & `genomap-1.3.4/genomap/genoVis/genoVis.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 @author: Md Tauhidul Islam, Ph.D., Dept. of Radiation Oncology, Stanford University
 """
 
 from tensorflow.keras.optimizers import Adam
 from genomap.utils.ConvIDEC import ConvIDEC
 from sklearn.feature_selection import VarianceThreshold
 from genomap.genomap import construct_genomap
-import umap
+import umap.umap_ as umap
 from genomap.utils.gTraj_utils import nearest_divisible_by_four
 import scanpy as sc
 import numpy as np
 import pandas as pd
 from genomap.utils.util_Sig import select_n_features
 
 def genoVis(data,n_clusters=None, colNum=32,rowNum=32,batch_size=64,verbose=1,
```

### Comparing `genomap-1.3.3/genomap/genomap.py` & `genomap-1.3.4/genomap/genomap.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.3/genomap/genomapOPT/genomapOPT.py` & `genomap-1.3.4/genomap/genomapOPT/genomapOPT.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.3/genomap/genomapT/genomapT.py` & `genomap-1.3.4/genomap/genomapT/genomapT.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.3/genomap/genotype/genotype.py` & `genomap-1.3.4/genomap/genotype/genotype.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.3/genomap/utils/ConvDEC.py` & `genomap-1.3.4/genomap/utils/ConvDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.3/genomap/utils/ConvIDEC.py` & `genomap-1.3.4/genomap/utils/ConvIDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.3/genomap/utils/FcDEC.py` & `genomap-1.3.4/genomap/utils/FcDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.3/genomap/utils/FcIDEC.py` & `genomap-1.3.4/genomap/utils/FcIDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.3/genomap/utils/class_discriminative_opt.py` & `genomap-1.3.4/genomap/utils/class_discriminative_opt.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.3/genomap/utils/gTraj_utils.py` & `genomap-1.3.4/genomap/utils/gTraj_utils.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.3/genomap/utils/group_centroid_opt.py` & `genomap-1.3.4/genomap/utils/group_centroid_opt.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.3/genomap/utils/metrics.py` & `genomap-1.3.4/genomap/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.3/genomap/utils/util_Sig.py` & `genomap-1.3.4/genomap/utils/util_Sig.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.3/genomap/utils/utils_MOI.py` & `genomap-1.3.4/genomap/utils/utils_MOI.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.3/genomap.egg-info/PKG-INFO` & `genomap-1.3.4/genomap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomap
-Version: 1.3.3
+Version: 1.3.4
 Summary: Genomap converts tabular gene expression data into spatially meaningful images.
 Home-page: https://github.com/xinglab-ai/genomap
 Author: Md Tauhidul Islam
 Author-email: tauhid@stanford.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -65,15 +65,15 @@
 import numpy as np
 import pandas as pd
 import genomap.genoVis as gp
 import matplotlib.pyplot as plt
 from sklearn.cluster import KMeans
 from sklearn.decomposition import PCA
 import phate
-import umap
+import umap.umap_ as umap
 
 data = pd.read_csv('TM_data.csv', header=None,
                    delim_whitespace=False)
 data=data.values
 gt_data = sio.loadmat('GT_TM.mat')
 y = np.squeeze(gt_data['GT'])
 n_clusters = len(np.unique(y))
@@ -102,15 +102,15 @@
 ### Example 3 - Try genoDR for dimensionality reduction
 
 ```python
 import scipy.io as sio
 import numpy as np
 import genomap.genoDR as gp
 import matplotlib.pyplot as plt
-import umap
+import umap.umap_ as umap
 
 dx = sio.loadmat('reducedData_divseq.mat')
 data=dx['X']
 gt_data = sio.loadmat('GT_divseq.mat')
 y = np.squeeze(gt_data['GT'])
 n_clusters = len(np.unique(y))
 
@@ -136,15 +136,15 @@
 import scipy.io as sio
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 from sklearn.cluster import KMeans
 from sklearn.decomposition import PCA
 import phate
-import umap
+import umap.umap_ as umap
 import genomap.genoTraj as gp
 
 # Load data
 dx = sio.loadmat('organoidData.mat')
 data=dx['X3']
 gt_data = sio.loadmat('cellsPsudo.mat')
 Y_time = np.squeeze(gt_data['newGT'])
```

### Comparing `genomap-1.3.3/genomap.egg-info/SOURCES.txt` & `genomap-1.3.4/genomap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `genomap-1.3.3/setup.py` & `genomap-1.3.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="genomap",
-    version="1.3.3",
+    version="1.3.4",
     author="Md Tauhidul Islam",
     author_email="tauhid@stanford.edu",
     description="Genomap converts tabular gene expression data into spatially meaningful images.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xinglab-ai/genomap",
     classifiers=[
```

