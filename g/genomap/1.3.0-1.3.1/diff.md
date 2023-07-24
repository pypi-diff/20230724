# Comparing `tmp/genomap-1.3.0.tar.gz` & `tmp/genomap-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genomap-1.3.0.tar", last modified: Mon Jul 24 17:34:48 2023, max compression
+gzip compressed data, was "genomap-1.3.1.tar", last modified: Mon Jul 24 18:10:50 2023, max compression
```

## Comparing `genomap-1.3.0.tar` & `genomap-1.3.1.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:48.483265 genomap-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-24 17:30:15.000000 genomap-1.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-24 17:30:15.000000 genomap-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13593 2023-07-24 17:34:48.483265 genomap-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-07-24 17:30:15.000000 genomap-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:48.451264 genomap-1.3.0/data/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-24 17:30:15.000000 genomap-1.3.0/data/TM_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:48.455264 genomap-1.3.0/genomap/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:48.455264 genomap-1.3.0/genomap/bregman_genomap/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/bregman_genomap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   125058 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/bregman_genomap/bregman_genomap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:48.459264 genomap-1.3.0/genomap/genoAnnotate/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoAnnotate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoAnnotate/genoAnnotate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:48.459264 genomap-1.3.0/genomap/genoClassification/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoClassification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoClassification/genoClassification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:48.459264 genomap-1.3.0/genomap/genoDR/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoDR/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoDR/genoDimReduction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:48.463264 genomap-1.3.0/genomap/genoMOI/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoMOI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoMOI/genoMOI.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:48.463264 genomap-1.3.0/genomap/genoNet/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoNet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoNet/genoNet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:48.463264 genomap-1.3.0/genomap/genoNetRegression/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoNetRegression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoNetRegression/genoNet_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:48.467265 genomap-1.3.0/genomap/genoNetus/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoNetus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoNetus/genoNetus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:48.467265 genomap-1.3.0/genomap/genoRegression/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoRegression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoRegression/genoRegression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:48.467265 genomap-1.3.0/genomap/genoSig/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoSig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoSig/genoSig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:48.467265 genomap-1.3.0/genomap/genoTraj/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoTraj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoTraj/genoTraj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:48.471264 genomap-1.3.0/genomap/genoVis/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoVis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoVis/genoVis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genomap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:48.471264 genomap-1.3.0/genomap/genomapOPT/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genomapOPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genomapOPT/genomapOPT.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:48.471264 genomap-1.3.0/genomap/genomapT/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genomapT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genomapT/genomapT.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:48.475265 genomap-1.3.0/genomap/genotype/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genotype/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genotype/genotype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:48.479265 genomap-1.3.0/genomap/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/utils/ConvDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/utils/ConvIDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/utils/FcDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/utils/FcIDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/utils/class_discriminative_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/utils/gTraj_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/utils/group_centroid_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/utils/util_Sig.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/utils/util_genoClassReg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/utils/utils_MOI.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:48.455264 genomap-1.3.0/genomap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13593 2023-07-24 17:34:48.000000 genomap-1.3.0/genomap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-24 17:34:48.000000 genomap-1.3.0/genomap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 17:34:48.000000 genomap-1.3.0/genomap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-24 17:34:48.000000 genomap-1.3.0/genomap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 17:34:48.000000 genomap-1.3.0/genomap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-24 17:30:15.000000 genomap-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 17:34:48.483265 genomap-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-24 17:30:15.000000 genomap-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:10:50.137690 genomap-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-24 18:06:15.000000 genomap-1.3.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-24 18:06:15.000000 genomap-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13593 2023-07-24 18:10:50.137690 genomap-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-07-24 18:06:15.000000 genomap-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:10:50.109690 genomap-1.3.1/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-24 18:06:15.000000 genomap-1.3.1/data/TM_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:10:50.109690 genomap-1.3.1/genomap/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:10:50.113690 genomap-1.3.1/genomap/bregman_genomap/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/bregman_genomap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125058 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/bregman_genomap/bregman_genomap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:10:50.113690 genomap-1.3.1/genomap/genoAnnotate/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoAnnotate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoAnnotate/genoAnnotate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:10:50.113690 genomap-1.3.1/genomap/genoClassification/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoClassification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoClassification/genoClassification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:10:50.113690 genomap-1.3.1/genomap/genoDR/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoDR/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoDR/genoDimReduction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:10:50.117690 genomap-1.3.1/genomap/genoMOI/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoMOI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoMOI/genoMOI.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:10:50.117690 genomap-1.3.1/genomap/genoNet/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoNet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoNet/genoNet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:10:50.117690 genomap-1.3.1/genomap/genoNetRegression/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoNetRegression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoNetRegression/genoNet_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:10:50.117690 genomap-1.3.1/genomap/genoNetus/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoNetus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoNetus/genoNetus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:10:50.121690 genomap-1.3.1/genomap/genoRegression/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoRegression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoRegression/genoRegression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:10:50.121690 genomap-1.3.1/genomap/genoSig/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoSig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoSig/genoSig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:10:50.121690 genomap-1.3.1/genomap/genoTraj/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoTraj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoTraj/genoTraj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:10:50.125690 genomap-1.3.1/genomap/genoVis/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoVis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoVis/genoVis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genomap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:10:50.125690 genomap-1.3.1/genomap/genomapOPT/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genomapOPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genomapOPT/genomapOPT.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:10:50.125690 genomap-1.3.1/genomap/genomapT/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genomapT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genomapT/genomapT.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:10:50.133690 genomap-1.3.1/genomap/genotype/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genotype/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genotype/genotype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:10:50.137690 genomap-1.3.1/genomap/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/utils/ConvDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/utils/ConvIDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/utils/FcDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/utils/FcIDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/utils/class_discriminative_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/utils/gTraj_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/utils/group_centroid_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/utils/util_Sig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/utils/util_genoClassReg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/utils/utils_MOI.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:10:50.109690 genomap-1.3.1/genomap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13593 2023-07-24 18:10:50.000000 genomap-1.3.1/genomap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-24 18:10:50.000000 genomap-1.3.1/genomap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:10:50.000000 genomap-1.3.1/genomap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-24 18:10:50.000000 genomap-1.3.1/genomap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 18:10:50.000000 genomap-1.3.1/genomap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-24 18:06:15.000000 genomap-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 18:10:50.137690 genomap-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-24 18:06:15.000000 genomap-1.3.1/setup.py
```

### Comparing `genomap-1.3.0/LICENSE.txt` & `genomap-1.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `genomap-1.3.0/PKG-INFO` & `genomap-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomap
-Version: 1.3.0
+Version: 1.3.1
 Summary: Genomap converts tabular gene expression data into spatially meaningful images.
 Home-page: https://github.com/xinglab-ai/genomap
 Author: Md Tauhidul Islam
 Author-email: tauhid@stanford.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `genomap-1.3.0/README.md` & `genomap-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `genomap-1.3.0/genomap/bregman_genomap/bregman_genomap.py` & `genomap-1.3.1/genomap/bregman_genomap/bregman_genomap.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.0/genomap/genoAnnotate/genoAnnotate.py` & `genomap-1.3.1/genomap/genoAnnotate/genoAnnotate.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.0/genomap/genoClassification/genoClassification.py` & `genomap-1.3.1/genomap/genoClassification/genoClassification.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.0/genomap/genoDR/genoDimReduction.py` & `genomap-1.3.1/genomap/genoDR/genoDimReduction.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.0/genomap/genoMOI/genoMOI.py` & `genomap-1.3.1/genomap/genoMOI/genoMOI.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.0/genomap/genoNet/genoNet.py` & `genomap-1.3.1/genomap/genoNet/genoNet.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.0/genomap/genoNetRegression/genoNet_regression.py` & `genomap-1.3.1/genomap/genoNetRegression/genoNet_regression.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.0/genomap/genoNetus/genoNetus.py` & `genomap-1.3.1/genomap/genoNetus/genoNetus.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.0/genomap/genoRegression/genoRegression.py` & `genomap-1.3.1/genomap/genoRegression/genoRegression.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.0/genomap/genoSig/genoSig.py` & `genomap-1.3.1/genomap/genoSig/genoSig.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.0/genomap/genoTraj/genoTraj.py` & `genomap-1.3.1/genomap/genoTraj/genoTraj.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.0/genomap/genoVis/genoVis.py` & `genomap-1.3.1/genomap/genoVis/genoVis.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.0/genomap/genomap.py` & `genomap-1.3.1/genomap/genomap.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.0/genomap/genomapOPT/genomapOPT.py` & `genomap-1.3.1/genomap/genomapOPT/genomapOPT.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.0/genomap/genomapT/genomapT.py` & `genomap-1.3.1/genomap/genomapT/genomapT.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.0/genomap/genotype/genotype.py` & `genomap-1.3.1/genomap/genotype/genotype.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.0/genomap/utils/ConvDEC.py` & `genomap-1.3.1/genomap/utils/ConvDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.0/genomap/utils/ConvIDEC.py` & `genomap-1.3.1/genomap/utils/ConvIDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.0/genomap/utils/FcDEC.py` & `genomap-1.3.1/genomap/utils/FcDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.0/genomap/utils/FcIDEC.py` & `genomap-1.3.1/genomap/utils/FcIDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.0/genomap/utils/class_discriminative_opt.py` & `genomap-1.3.1/genomap/utils/class_discriminative_opt.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.0/genomap/utils/gTraj_utils.py` & `genomap-1.3.1/genomap/utils/gTraj_utils.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.0/genomap/utils/group_centroid_opt.py` & `genomap-1.3.1/genomap/utils/group_centroid_opt.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.0/genomap/utils/metrics.py` & `genomap-1.3.1/genomap/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.0/genomap/utils/util_Sig.py` & `genomap-1.3.1/genomap/utils/util_Sig.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.0/genomap/utils/utils_MOI.py` & `genomap-1.3.1/genomap/utils/utils_MOI.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.0/genomap.egg-info/PKG-INFO` & `genomap-1.3.1/genomap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomap
-Version: 1.3.0
+Version: 1.3.1
 Summary: Genomap converts tabular gene expression data into spatially meaningful images.
 Home-page: https://github.com/xinglab-ai/genomap
 Author: Md Tauhidul Islam
 Author-email: tauhid@stanford.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `genomap-1.3.0/genomap.egg-info/SOURCES.txt` & `genomap-1.3.1/genomap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `genomap-1.3.0/setup.py` & `genomap-1.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="genomap",
-    version="1.3.0",
+    version="1.3.1",
     author="Md Tauhidul Islam",
     author_email="tauhid@stanford.edu",
     description="Genomap converts tabular gene expression data into spatially meaningful images.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xinglab-ai/genomap",
     classifiers=[
```

