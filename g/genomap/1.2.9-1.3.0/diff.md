# Comparing `tmp/genomap-1.2.9.tar.gz` & `tmp/genomap-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genomap-1.2.9.tar", last modified: Tue Jul 18 16:58:25 2023, max compression
+gzip compressed data, was "genomap-1.3.0.tar", last modified: Mon Jul 24 17:34:48 2023, max compression
```

## Comparing `genomap-1.2.9.tar` & `genomap-1.3.0.tar`

### file list

```diff
@@ -1,71 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:58:25.949687 genomap-1.2.9/
--rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-18 16:54:01.000000 genomap-1.2.9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-18 16:54:01.000000 genomap-1.2.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11667 2023-07-18 16:58:25.945687 genomap-1.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11233 2023-07-18 16:54:01.000000 genomap-1.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:58:25.929687 genomap-1.2.9/data/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-18 16:54:01.000000 genomap-1.2.9/data/TM_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:58:25.929687 genomap-1.2.9/genomap/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:58:25.929687 genomap-1.2.9/genomap/bregman_genomap/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/bregman_genomap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   125058 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/bregman_genomap/bregman_genomap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:58:25.933687 genomap-1.2.9/genomap/genoClassification/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genoClassification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genoClassification/genoClassification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:58:25.933687 genomap-1.2.9/genomap/genoDR/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genoDR/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genoDR/genoDimReduction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:58:25.933687 genomap-1.2.9/genomap/genoMOI/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genoMOI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genoMOI/genoMOI.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:58:25.933687 genomap-1.2.9/genomap/genoNet/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genoNet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genoNet/genoNet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:58:25.937687 genomap-1.2.9/genomap/genoNetRegression/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genoNetRegression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genoNetRegression/genoNet_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:58:25.937687 genomap-1.2.9/genomap/genoNetus/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genoNetus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genoNetus/genoNetus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:58:25.937687 genomap-1.2.9/genomap/genoRegression/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genoRegression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genoRegression/genoRegression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:58:25.937687 genomap-1.2.9/genomap/genoSig/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genoSig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genoSig/genoSig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:58:25.937687 genomap-1.2.9/genomap/genoTraj/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genoTraj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genoTraj/genoTraj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:58:25.941687 genomap-1.2.9/genomap/genoVis/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genoVis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genoVis/genoVis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genomap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:58:25.941687 genomap-1.2.9/genomap/genomapOPT/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genomapOPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genomapOPT/genomapOPT.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:58:25.941687 genomap-1.2.9/genomap/genomapT/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genomapT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genomapT/genomapT.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:58:25.945687 genomap-1.2.9/genomap/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/utils/ConvDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/utils/ConvIDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/utils/FcDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/utils/FcIDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/utils/class_discriminative_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/utils/gTraj_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/utils/group_centroid_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/utils/util_Sig.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/utils/util_genoClassReg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/utils/utils_MOI.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:58:25.929687 genomap-1.2.9/genomap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11667 2023-07-18 16:58:25.000000 genomap-1.2.9/genomap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-18 16:58:25.000000 genomap-1.2.9/genomap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 16:58:25.000000 genomap-1.2.9/genomap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-18 16:58:25.000000 genomap-1.2.9/genomap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-18 16:58:25.000000 genomap-1.2.9/genomap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-18 16:54:01.000000 genomap-1.2.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 16:58:25.949687 genomap-1.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-18 16:54:01.000000 genomap-1.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:48.483265 genomap-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-24 17:30:15.000000 genomap-1.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-24 17:30:15.000000 genomap-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13593 2023-07-24 17:34:48.483265 genomap-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-07-24 17:30:15.000000 genomap-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:48.451264 genomap-1.3.0/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-24 17:30:15.000000 genomap-1.3.0/data/TM_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:48.455264 genomap-1.3.0/genomap/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:48.455264 genomap-1.3.0/genomap/bregman_genomap/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/bregman_genomap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125058 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/bregman_genomap/bregman_genomap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:48.459264 genomap-1.3.0/genomap/genoAnnotate/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoAnnotate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoAnnotate/genoAnnotate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:48.459264 genomap-1.3.0/genomap/genoClassification/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoClassification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoClassification/genoClassification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:48.459264 genomap-1.3.0/genomap/genoDR/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoDR/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoDR/genoDimReduction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:48.463264 genomap-1.3.0/genomap/genoMOI/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoMOI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoMOI/genoMOI.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:48.463264 genomap-1.3.0/genomap/genoNet/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoNet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoNet/genoNet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:48.463264 genomap-1.3.0/genomap/genoNetRegression/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoNetRegression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoNetRegression/genoNet_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:48.467265 genomap-1.3.0/genomap/genoNetus/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoNetus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoNetus/genoNetus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:48.467265 genomap-1.3.0/genomap/genoRegression/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoRegression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoRegression/genoRegression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:48.467265 genomap-1.3.0/genomap/genoSig/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoSig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoSig/genoSig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:48.467265 genomap-1.3.0/genomap/genoTraj/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoTraj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoTraj/genoTraj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:48.471264 genomap-1.3.0/genomap/genoVis/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoVis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genoVis/genoVis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genomap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:48.471264 genomap-1.3.0/genomap/genomapOPT/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genomapOPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genomapOPT/genomapOPT.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:48.471264 genomap-1.3.0/genomap/genomapT/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genomapT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genomapT/genomapT.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:48.475265 genomap-1.3.0/genomap/genotype/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genotype/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/genotype/genotype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:48.479265 genomap-1.3.0/genomap/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/utils/ConvDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/utils/ConvIDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/utils/FcDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/utils/FcIDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/utils/class_discriminative_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/utils/gTraj_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/utils/group_centroid_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/utils/util_Sig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/utils/util_genoClassReg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-24 17:30:15.000000 genomap-1.3.0/genomap/utils/utils_MOI.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:34:48.455264 genomap-1.3.0/genomap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13593 2023-07-24 17:34:48.000000 genomap-1.3.0/genomap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-24 17:34:48.000000 genomap-1.3.0/genomap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 17:34:48.000000 genomap-1.3.0/genomap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-24 17:34:48.000000 genomap-1.3.0/genomap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 17:34:48.000000 genomap-1.3.0/genomap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-24 17:30:15.000000 genomap-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 17:34:48.483265 genomap-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-24 17:30:15.000000 genomap-1.3.0/setup.py
```

### Comparing `genomap-1.2.9/LICENSE.txt` & `genomap-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `genomap-1.2.9/PKG-INFO` & `genomap-1.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: genomap
-Version: 1.2.9
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
@@ -28,15 +15,15 @@
 
 ## Sample data
 
 To run the example codes below, you will need to download data files from [here](https://drive.google.com/drive/folders/1xq3bBgVP0NCMD7bGTXit0qRkL8fbutZ6?usp=drive_link).
 
 ## Example codes
 
-### Example 1 - Construct a genomap
+### Example 1 - Construct genomaps
 
 ```python
 import pandas as pd # Please install pandas and matplotlib before you run this example
 import matplotlib.pyplot as plt
 import numpy as np
 import scipy
 import genomap as gp
@@ -79,15 +66,15 @@
 n_clusters = len(np.unique(y))
 
 
 resVis=gp.genoVis(data,n_clusters=n_clusters, colNum=33,rowNum=33)
 # Use resVis=gp.genoVis(data, colNum=32,rowNum=32), if you dont know the number
 # of classes in the data
 
-resVisEmb=resVis[0] # Dimensionality reduction and visualization result
+resVisEmb=resVis[0] # Visualization result
 clusIndex=resVis[1] # Clustering result
 
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
 h1=plt.scatter(resVisEmb[:, 0], resVisEmb[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
 plt.xlabel('genoVis1')
 plt.ylabel('genoVis2')
@@ -180,20 +167,18 @@
 ```
 
 ### Example 5 - Try genoMOI for multi-omic data integration
 
 ```python
 import scanpy as sc
 import matplotlib.pyplot as plt
-import genomap.genoMOI as gp
 import scipy.io as sio
 import numpy as np
 import pandas as pd
-import umap
-
+from genomap.genoMOI import genoMOIvis, genoMOItraj
 
 # Load five different pancreatic datasets
 dx = sio.loadmat('dataBaronX.mat')
 data=dx['dataBaron']
 dx = sio.loadmat('dataMuraroX.mat')
 data2=dx['dataMuraro']
 dx = sio.loadmat('dataScapleX.mat')
@@ -205,31 +190,87 @@
 
 # Load class and batch labels
 dx = sio.loadmat('classLabel.mat')
 y = np.squeeze(dx['classLabel'])
 dx = sio.loadmat('batchLabel.mat')
 ybatch = np.squeeze(dx['batchLabel'])
 
-# Apply genoMOI with genomap size of 44x44 and dimension of 32 for the returned integrated data
-resVis=gp.genoMOI(data, data2, data3, data4, data5, colNum=44, rowNum=44, n_dim=32)
+# Apply genomap-based multi omic integration and visualize the integrated data with local structure for cluster analysis
+# returns 2D visualization, cluster labels, and intgerated data
+resVis,cli,int_data=genoMOIvis(data, data2, data3, data4, data5, colNum=12, rowNum=12, n_dim=32, epoch=10, prealign_method='scanorama')
 
-# Visualize the integrated data using UMAP
-embedding = umap.UMAP(n_neighbors=30,min_dist=0.3,n_epochs=200).fit_transform(resVis)
 
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
-h1=plt.scatter(embedding[:, 0], embedding[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
-plt.xlabel('UMAP1')
-plt.ylabel('UMAP2')
+h1=plt.scatter(resVis[:, 0], resVis[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
+plt.xlabel('genoVis1')
+plt.ylabel('genoVis2')
+plt.tight_layout()
+plt.colorbar(h1)
+plt.show()
+
+plt.figure(figsize=(15, 10))
+plt.rcParams.update({'font.size': 28})    
+h1=plt.scatter(resVis[:, 0], resVis[:, 1], c=ybatch,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
+plt.xlabel('genoVis1')
+plt.ylabel('genoVis2')
 plt.tight_layout()
 plt.colorbar(h1)
 plt.show()
 ```
 
-### Example 6 - Try genoSig for finding gene signatures for cell/data classes
+```python
+# Apply genomap-based multi omic integration and visualize the integrated data with global structure for trajectory analysis
+
+# returns 2D embedding, cluster labels, and intgerated data
+resTraj,cli,int_data=genoMOItraj(data, data2, data3, data4, data5, colNum=12, rowNum=12, n_dim=32, epoch=10, prealign_method='scanorama')
+
+
+plt.figure(figsize=(15, 10))
+plt.rcParams.update({'font.size': 28})    
+h1=plt.scatter(resTraj[:, 0], resTraj[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
+plt.xlabel('genoTraj1')
+plt.ylabel('genoTraj2')
+plt.tight_layout()
+plt.colorbar(h1)
+plt.show()
+
+plt.figure(figsize=(15, 10))
+plt.rcParams.update({'font.size': 28})    
+h1=plt.scatter(resTraj[:, 0], resTraj[:, 1], c=ybatch,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
+plt.xlabel('genoTraj1')
+plt.ylabel('genoTraj2')
+plt.tight_layout()
+plt.colorbar(h1)
+plt.show()
+```
+
+### Example 6 - Try genoAnnotate for cell annotation
+
+```python
+import scanpy as sc
+import pandas as pd
+import genomap.genoAnnotate as gp
+#Load the PBMC dataset
+adata = sc.read_10x_mtx("pbmc3k_filtered_gene_bc_matrices/")
+
+# Input: adata: annData containing the raw gene counts
+# tissue type: e.g. Immune system,Pancreas,Liver,Eye,Kidney,Brain,Lung,Adrenal,Heart,Intestine,Muscle,Placenta,Spleen,Stomach,Thymus 
+ 
+adataP = gp.genoAnnotate(adata,tissue_type="Immune system")
+
+
+# Compute UMAP (requires neighborhood graph, see the previous code for Louvain clustering)
+sc.tl.umap(adataP)
+# Create a UMAP plot colored by cell type labels
+cell_annotations=adataP.obs['cell_type']
+sc.pl.umap(adataP, color='cell_type')
+```
+
+### Example 7 - Try genoSig for finding gene signatures for cell/data classes
 
 ```python
 import numpy as np
 import scipy.io as sio
 from genomap.utils.util_Sig import createGenomap_for_sig
 import pandas as pd
 import genomap.genoSig as gp
@@ -253,15 +294,15 @@
 genoMaps,gene_namesRe,T=createGenomap_for_sig(data,gene_names,rowNum,colNum)
 # compute the gene signatures
 result=gp.genoSig(genoMaps,T,label,userPD,gene_namesRe, epochs=50)
 
 print(result.head())
 ```
 
-### Example 7 - Try genoClassification for tabular data classification
+### Example 8 - Try genoClassification for tabular data classification
 
 ```python
 import pandas as pd
 import numpy as np
 import scipy.io as sio
 import genomap.genoClassification as gp
 from genomap.utils.util_genoClassReg import select_random_values
@@ -290,16 +331,15 @@
 test_data=data.values[indxTest-1]
 
 est=gp.genoClassification(training_data, training_labels, test_data, rowNum=rowNum, colNum=colNum, epoch=150)
 
 print('Classification accuracy of genomap approach:'+str(np.sum(est==groundTruthTest) / est.shape[0]))  
 ```
 
-
-### Example 8 - Try genoRegression for tabular data regression
+### Example 9 - Try genoRegression for tabular data regression
 
 ```python
 import pandas as pd
 import numpy as np
 import scipy.io as sio
 import genomap.genoRegression as gp
 from sklearn.metrics import mean_squared_error
```

### Comparing `genomap-1.2.9/README.md` & `genomap-1.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: genomap
+Version: 1.3.0
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
@@ -15,15 +28,15 @@
 
 ## Sample data
 
 To run the example codes below, you will need to download data files from [here](https://drive.google.com/drive/folders/1xq3bBgVP0NCMD7bGTXit0qRkL8fbutZ6?usp=drive_link).
 
 ## Example codes
 
-### Example 1 - Construct a genomap
+### Example 1 - Construct genomaps
 
 ```python
 import pandas as pd # Please install pandas and matplotlib before you run this example
 import matplotlib.pyplot as plt
 import numpy as np
 import scipy
 import genomap as gp
@@ -66,15 +79,15 @@
 n_clusters = len(np.unique(y))
 
 
 resVis=gp.genoVis(data,n_clusters=n_clusters, colNum=33,rowNum=33)
 # Use resVis=gp.genoVis(data, colNum=32,rowNum=32), if you dont know the number
 # of classes in the data
 
-resVisEmb=resVis[0] # Dimensionality reduction and visualization result
+resVisEmb=resVis[0] # Visualization result
 clusIndex=resVis[1] # Clustering result
 
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
 h1=plt.scatter(resVisEmb[:, 0], resVisEmb[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
 plt.xlabel('genoVis1')
 plt.ylabel('genoVis2')
@@ -167,20 +180,18 @@
 ```
 
 ### Example 5 - Try genoMOI for multi-omic data integration
 
 ```python
 import scanpy as sc
 import matplotlib.pyplot as plt
-import genomap.genoMOI as gp
 import scipy.io as sio
 import numpy as np
 import pandas as pd
-import umap
-
+from genomap.genoMOI import genoMOIvis, genoMOItraj
 
 # Load five different pancreatic datasets
 dx = sio.loadmat('dataBaronX.mat')
 data=dx['dataBaron']
 dx = sio.loadmat('dataMuraroX.mat')
 data2=dx['dataMuraro']
 dx = sio.loadmat('dataScapleX.mat')
@@ -192,31 +203,87 @@
 
 # Load class and batch labels
 dx = sio.loadmat('classLabel.mat')
 y = np.squeeze(dx['classLabel'])
 dx = sio.loadmat('batchLabel.mat')
 ybatch = np.squeeze(dx['batchLabel'])
 
-# Apply genoMOI with genomap size of 44x44 and dimension of 32 for the returned integrated data
-resVis=gp.genoMOI(data, data2, data3, data4, data5, colNum=44, rowNum=44, n_dim=32)
+# Apply genomap-based multi omic integration and visualize the integrated data with local structure for cluster analysis
+# returns 2D visualization, cluster labels, and intgerated data
+resVis,cli,int_data=genoMOIvis(data, data2, data3, data4, data5, colNum=12, rowNum=12, n_dim=32, epoch=10, prealign_method='scanorama')
 
-# Visualize the integrated data using UMAP
-embedding = umap.UMAP(n_neighbors=30,min_dist=0.3,n_epochs=200).fit_transform(resVis)
 
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
-h1=plt.scatter(embedding[:, 0], embedding[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
-plt.xlabel('UMAP1')
-plt.ylabel('UMAP2')
+h1=plt.scatter(resVis[:, 0], resVis[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
+plt.xlabel('genoVis1')
+plt.ylabel('genoVis2')
+plt.tight_layout()
+plt.colorbar(h1)
+plt.show()
+
+plt.figure(figsize=(15, 10))
+plt.rcParams.update({'font.size': 28})    
+h1=plt.scatter(resVis[:, 0], resVis[:, 1], c=ybatch,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
+plt.xlabel('genoVis1')
+plt.ylabel('genoVis2')
 plt.tight_layout()
 plt.colorbar(h1)
 plt.show()
 ```
 
-### Example 6 - Try genoSig for finding gene signatures for cell/data classes
+```python
+# Apply genomap-based multi omic integration and visualize the integrated data with global structure for trajectory analysis
+
+# returns 2D embedding, cluster labels, and intgerated data
+resTraj,cli,int_data=genoMOItraj(data, data2, data3, data4, data5, colNum=12, rowNum=12, n_dim=32, epoch=10, prealign_method='scanorama')
+
+
+plt.figure(figsize=(15, 10))
+plt.rcParams.update({'font.size': 28})    
+h1=plt.scatter(resTraj[:, 0], resTraj[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
+plt.xlabel('genoTraj1')
+plt.ylabel('genoTraj2')
+plt.tight_layout()
+plt.colorbar(h1)
+plt.show()
+
+plt.figure(figsize=(15, 10))
+plt.rcParams.update({'font.size': 28})    
+h1=plt.scatter(resTraj[:, 0], resTraj[:, 1], c=ybatch,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
+plt.xlabel('genoTraj1')
+plt.ylabel('genoTraj2')
+plt.tight_layout()
+plt.colorbar(h1)
+plt.show()
+```
+
+### Example 6 - Try genoAnnotate for cell annotation
+
+```python
+import scanpy as sc
+import pandas as pd
+import genomap.genoAnnotate as gp
+#Load the PBMC dataset
+adata = sc.read_10x_mtx("pbmc3k_filtered_gene_bc_matrices/")
+
+# Input: adata: annData containing the raw gene counts
+# tissue type: e.g. Immune system,Pancreas,Liver,Eye,Kidney,Brain,Lung,Adrenal,Heart,Intestine,Muscle,Placenta,Spleen,Stomach,Thymus 
+ 
+adataP = gp.genoAnnotate(adata,tissue_type="Immune system")
+
+
+# Compute UMAP (requires neighborhood graph, see the previous code for Louvain clustering)
+sc.tl.umap(adataP)
+# Create a UMAP plot colored by cell type labels
+cell_annotations=adataP.obs['cell_type']
+sc.pl.umap(adataP, color='cell_type')
+```
+
+### Example 7 - Try genoSig for finding gene signatures for cell/data classes
 
 ```python
 import numpy as np
 import scipy.io as sio
 from genomap.utils.util_Sig import createGenomap_for_sig
 import pandas as pd
 import genomap.genoSig as gp
@@ -240,15 +307,15 @@
 genoMaps,gene_namesRe,T=createGenomap_for_sig(data,gene_names,rowNum,colNum)
 # compute the gene signatures
 result=gp.genoSig(genoMaps,T,label,userPD,gene_namesRe, epochs=50)
 
 print(result.head())
 ```
 
-### Example 7 - Try genoClassification for tabular data classification
+### Example 8 - Try genoClassification for tabular data classification
 
 ```python
 import pandas as pd
 import numpy as np
 import scipy.io as sio
 import genomap.genoClassification as gp
 from genomap.utils.util_genoClassReg import select_random_values
@@ -277,16 +344,15 @@
 test_data=data.values[indxTest-1]
 
 est=gp.genoClassification(training_data, training_labels, test_data, rowNum=rowNum, colNum=colNum, epoch=150)
 
 print('Classification accuracy of genomap approach:'+str(np.sum(est==groundTruthTest) / est.shape[0]))  
 ```
 
-
-### Example 8 - Try genoRegression for tabular data regression
+### Example 9 - Try genoRegression for tabular data regression
 
 ```python
 import pandas as pd
 import numpy as np
 import scipy.io as sio
 import genomap.genoRegression as gp
 from sklearn.metrics import mean_squared_error
```

### Comparing `genomap-1.2.9/genomap/bregman_genomap/bregman_genomap.py` & `genomap-1.3.0/genomap/bregman_genomap/bregman_genomap.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.9/genomap/genoClassification/genoClassification.py` & `genomap-1.3.0/genomap/genoClassification/genoClassification.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.9/genomap/genoDR/genoDimReduction.py` & `genomap-1.3.0/genomap/genoDR/genoDimReduction.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.9/genomap/genoMOI/genoMOI.py` & `genomap-1.3.0/genomap/genoVis/genoVis.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,71 +7,69 @@
 
 from tensorflow.keras.optimizers import Adam
 from genomap.utils.ConvIDEC import ConvIDEC
 from sklearn.feature_selection import VarianceThreshold
 from genomap.genomap import construct_genomap
 import umap
 from genomap.utils.gTraj_utils import nearest_divisible_by_four
-from genomap.utils.utils_MOI import * 
+import scanpy as sc
+import numpy as np
+import pandas as pd
 from genomap.utils.util_Sig import select_n_features
 
-def genoMOI(*arrays, n_clusters=None, n_dim=32, colNum=32, rowNum=32):
-
-# arrays: a number of arrays such as array1, array2 from different sources
-# n_clusters: number of data classes
-# n_dim: number of the dimension in returned integrated data
-# colNum and rowNum: column and row number of genomaps
-#
-# Pre-align data with bbknn
-    batch_corrected_data=apply_bbknn_and_return_batch_corrected(*arrays)
-    dataDX=scipy.stats.zscore(batch_corrected_data, axis=0, ddof=1) 
-    
-    if n_clusters==None:
-        array1=arrays[0]
-        adata = convertToAnnData(array1)
-        # Perform Louvain clustering
-        sc.pp.neighbors(adata)
-        sc.tl.louvain(adata, resolution=1.0)
-        # Access the cluster assignments
-        cluster_labels = adata.obs['louvain']
-        n_clusters = len(np.unique(cluster_labels))        
-    
-    resVis=extract_genoVis_features(dataDX, n_clusters=n_clusters, n_dim=n_dim, colNum=colNum,rowNum=rowNum)
-    return resVis
-
-
-def extract_genoVis_features(data,n_clusters=20, n_dim=32, colNum=32, rowNum=32, batch_size=64, verbose=1,
-                    pretrain_epochs=100, maxiter=300):
+def genoVis(data,n_clusters=None, colNum=32,rowNum=32,batch_size=64,verbose=1,
+                    pretrain_epochs=100,maxiter=300):
 # rowNum and colNum are the row and column numbers of constructed genomaps
 # n_clusters: number of data classes in the data
 # batch_size: number of samples in each mini batch while training the deep neural network
 # verbose: whether training progress will be shown or not
 # pretrain_epochs: number of epoch for pre-training the CNN
 # maxiter: number of epoch of fine-tuning training
 # Construction of genomap    
     colNum=nearest_divisible_by_four(colNum)
     rowNum=nearest_divisible_by_four(rowNum)
     nump=rowNum*colNum 
     if nump<data.shape[1]:
-        data,index=select_n_features(data,nump) 
+        data,index=select_n_features(data,nump)
     genoMaps=construct_genomap(data,rowNum,colNum,epsilon=0.0,num_iter=200)
+    
+    if n_clusters==None:
+        
+        adata = convertToAnnData(data)
+        # Perform Louvain clustering
+        sc.pp.neighbors(adata)
+        sc.tl.louvain(adata, resolution=1.0)
+        # Access the cluster assignments
+        cluster_labels = adata.obs['louvain']
+        n_clusters = len(np.unique(cluster_labels)) 
 
-# Deep learning-based dimensionality reduction and clustering
+    # Deep learning-based dimensionality reduction and clustering
     optimizer = Adam()    
-    model = ConvIDEC(input_shape=genoMaps.shape[1:], filters=[32, 64, 128, n_dim], n_clusters=n_clusters)
+    model = ConvIDEC(input_shape=genoMaps.shape[1:], filters=[32, 64, 128, 32], n_clusters=n_clusters)
     model.compile(optimizer=optimizer, loss=['kld', 'mse'], loss_weights=[0.1, 1.0])
     pretrain_optimizer ='adam'
     update_interval=50
     model.pretrain(genoMaps, y=None, optimizer=pretrain_optimizer, epochs=pretrain_epochs, batch_size=batch_size,
                         verbose=verbose)
 
     y_pred = model.fit(genoMaps, y=None, maxiter=maxiter, batch_size=batch_size, update_interval=update_interval,
                        )
+    # Perform clustering using genomap
     y_pred = model.predict_labels(genoMaps)
-    # Extract DNN features
+    # Extract the autoencoder features
     feat_DNN=model.extract_features(genoMaps)
-    #embedding2D = umap.UMAP(n_neighbors=30,min_dist=0.3,n_epochs=200).fit_transform(feat_DNN)
-    return feat_DNN
-
+    # Create embeddings from the extracted features
+    embedding2D = umap.UMAP(n_neighbors=30,min_dist=0.3,n_epochs=200).fit_transform(feat_DNN)
+    return embedding2D, y_pred
 
 
+def convertToAnnData(data):
+    # Convert numpy array to annData
+    # Create pseudo cell names
+    cell_names = ['Cell_' + str(i) for i in range(1, data.shape[0]+1)]
+    # Create pseudo gene names
+    gene_names = ['Gene_' + str(i) for i in range(1, data.shape[1]+1)]
+    # Create a pandas DataFrame
+    df = pd.DataFrame(data, index=cell_names, columns=gene_names)
+    adataMy=sc.AnnData(df)
+    return adataMy
```

### Comparing `genomap-1.2.9/genomap/genoNet/genoNet.py` & `genomap-1.3.0/genomap/genoNet/genoNet.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.9/genomap/genoNetRegression/genoNet_regression.py` & `genomap-1.3.0/genomap/genoNetRegression/genoNet_regression.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.9/genomap/genoNetus/genoNetus.py` & `genomap-1.3.0/genomap/genoNetus/genoNetus.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.9/genomap/genoRegression/genoRegression.py` & `genomap-1.3.0/genomap/genoRegression/genoRegression.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.9/genomap/genoSig/genoSig.py` & `genomap-1.3.0/genomap/genoSig/genoSig.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from keras.layers import Conv2D, MaxPooling2D, Flatten, Dense
 from lime import lime_image
 import numpy as np
 from tensorflow.keras.utils import to_categorical
 
 def compute_genoSig(imageset,label, sig_class, epochs=100):
     # imageset contains the genomaps in shape (cellNum, rowNum, colNum, 1)
-    # label: numpy array of shape (cellNum, 1) containing the cell labels
+    # label: dataframe of shape (cellNum, 1) containing the cell labels
     # sig_class: numpy array containing the cell classes for which gene signatures will be computed
 
     n_clusters = len(np.unique(label))
     # Create the deep learning model
     model = Sequential()
     model.add(Conv2D(32, kernel_size=(3, 3), activation='relu', input_shape=(imageset.shape[1], imageset.shape[2], imageset.shape[3])))
     model.add(MaxPooling2D(pool_size=(2, 2)))
```

### Comparing `genomap-1.2.9/genomap/genoTraj/genoTraj.py` & `genomap-1.3.0/genomap/genoTraj/genoTraj.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.9/genomap/genomap.py` & `genomap-1.3.0/genomap/genomap.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.9/genomap/genomapOPT/genomapOPT.py` & `genomap-1.3.0/genomap/genomapOPT/genomapOPT.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.9/genomap/genomapT/genomapT.py` & `genomap-1.3.0/genomap/genomapT/genomapT.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.9/genomap/utils/ConvDEC.py` & `genomap-1.3.0/genomap/utils/ConvDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.9/genomap/utils/ConvIDEC.py` & `genomap-1.3.0/genomap/utils/ConvIDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.9/genomap/utils/FcDEC.py` & `genomap-1.3.0/genomap/utils/FcDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.9/genomap/utils/FcIDEC.py` & `genomap-1.3.0/genomap/utils/FcIDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.9/genomap/utils/class_discriminative_opt.py` & `genomap-1.3.0/genomap/utils/class_discriminative_opt.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.9/genomap/utils/gTraj_utils.py` & `genomap-1.3.0/genomap/utils/gTraj_utils.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.9/genomap/utils/group_centroid_opt.py` & `genomap-1.3.0/genomap/utils/group_centroid_opt.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.9/genomap/utils/metrics.py` & `genomap-1.3.0/genomap/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.9/genomap/utils/util_Sig.py` & `genomap-1.3.0/genomap/utils/util_Sig.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.9/genomap/utils/utils_MOI.py` & `genomap-1.3.0/genomap/utils/utils_MOI.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.9/genomap.egg-info/PKG-INFO` & `genomap-1.3.0/genomap.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomap
-Version: 1.2.9
+Version: 1.3.0
 Summary: Genomap converts tabular gene expression data into spatially meaningful images.
 Home-page: https://github.com/xinglab-ai/genomap
 Author: Md Tauhidul Islam
 Author-email: tauhid@stanford.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -28,15 +28,15 @@
 
 ## Sample data
 
 To run the example codes below, you will need to download data files from [here](https://drive.google.com/drive/folders/1xq3bBgVP0NCMD7bGTXit0qRkL8fbutZ6?usp=drive_link).
 
 ## Example codes
 
-### Example 1 - Construct a genomap
+### Example 1 - Construct genomaps
 
 ```python
 import pandas as pd # Please install pandas and matplotlib before you run this example
 import matplotlib.pyplot as plt
 import numpy as np
 import scipy
 import genomap as gp
@@ -79,15 +79,15 @@
 n_clusters = len(np.unique(y))
 
 
 resVis=gp.genoVis(data,n_clusters=n_clusters, colNum=33,rowNum=33)
 # Use resVis=gp.genoVis(data, colNum=32,rowNum=32), if you dont know the number
 # of classes in the data
 
-resVisEmb=resVis[0] # Dimensionality reduction and visualization result
+resVisEmb=resVis[0] # Visualization result
 clusIndex=resVis[1] # Clustering result
 
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
 h1=plt.scatter(resVisEmb[:, 0], resVisEmb[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
 plt.xlabel('genoVis1')
 plt.ylabel('genoVis2')
@@ -180,20 +180,18 @@
 ```
 
 ### Example 5 - Try genoMOI for multi-omic data integration
 
 ```python
 import scanpy as sc
 import matplotlib.pyplot as plt
-import genomap.genoMOI as gp
 import scipy.io as sio
 import numpy as np
 import pandas as pd
-import umap
-
+from genomap.genoMOI import genoMOIvis, genoMOItraj
 
 # Load five different pancreatic datasets
 dx = sio.loadmat('dataBaronX.mat')
 data=dx['dataBaron']
 dx = sio.loadmat('dataMuraroX.mat')
 data2=dx['dataMuraro']
 dx = sio.loadmat('dataScapleX.mat')
@@ -205,31 +203,87 @@
 
 # Load class and batch labels
 dx = sio.loadmat('classLabel.mat')
 y = np.squeeze(dx['classLabel'])
 dx = sio.loadmat('batchLabel.mat')
 ybatch = np.squeeze(dx['batchLabel'])
 
-# Apply genoMOI with genomap size of 44x44 and dimension of 32 for the returned integrated data
-resVis=gp.genoMOI(data, data2, data3, data4, data5, colNum=44, rowNum=44, n_dim=32)
+# Apply genomap-based multi omic integration and visualize the integrated data with local structure for cluster analysis
+# returns 2D visualization, cluster labels, and intgerated data
+resVis,cli,int_data=genoMOIvis(data, data2, data3, data4, data5, colNum=12, rowNum=12, n_dim=32, epoch=10, prealign_method='scanorama')
 
-# Visualize the integrated data using UMAP
-embedding = umap.UMAP(n_neighbors=30,min_dist=0.3,n_epochs=200).fit_transform(resVis)
 
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
-h1=plt.scatter(embedding[:, 0], embedding[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
-plt.xlabel('UMAP1')
-plt.ylabel('UMAP2')
+h1=plt.scatter(resVis[:, 0], resVis[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
+plt.xlabel('genoVis1')
+plt.ylabel('genoVis2')
+plt.tight_layout()
+plt.colorbar(h1)
+plt.show()
+
+plt.figure(figsize=(15, 10))
+plt.rcParams.update({'font.size': 28})    
+h1=plt.scatter(resVis[:, 0], resVis[:, 1], c=ybatch,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
+plt.xlabel('genoVis1')
+plt.ylabel('genoVis2')
+plt.tight_layout()
+plt.colorbar(h1)
+plt.show()
+```
+
+```python
+# Apply genomap-based multi omic integration and visualize the integrated data with global structure for trajectory analysis
+
+# returns 2D embedding, cluster labels, and intgerated data
+resTraj,cli,int_data=genoMOItraj(data, data2, data3, data4, data5, colNum=12, rowNum=12, n_dim=32, epoch=10, prealign_method='scanorama')
+
+
+plt.figure(figsize=(15, 10))
+plt.rcParams.update({'font.size': 28})    
+h1=plt.scatter(resTraj[:, 0], resTraj[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
+plt.xlabel('genoTraj1')
+plt.ylabel('genoTraj2')
+plt.tight_layout()
+plt.colorbar(h1)
+plt.show()
+
+plt.figure(figsize=(15, 10))
+plt.rcParams.update({'font.size': 28})    
+h1=plt.scatter(resTraj[:, 0], resTraj[:, 1], c=ybatch,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
+plt.xlabel('genoTraj1')
+plt.ylabel('genoTraj2')
 plt.tight_layout()
 plt.colorbar(h1)
 plt.show()
 ```
 
-### Example 6 - Try genoSig for finding gene signatures for cell/data classes
+### Example 6 - Try genoAnnotate for cell annotation
+
+```python
+import scanpy as sc
+import pandas as pd
+import genomap.genoAnnotate as gp
+#Load the PBMC dataset
+adata = sc.read_10x_mtx("pbmc3k_filtered_gene_bc_matrices/")
+
+# Input: adata: annData containing the raw gene counts
+# tissue type: e.g. Immune system,Pancreas,Liver,Eye,Kidney,Brain,Lung,Adrenal,Heart,Intestine,Muscle,Placenta,Spleen,Stomach,Thymus 
+ 
+adataP = gp.genoAnnotate(adata,tissue_type="Immune system")
+
+
+# Compute UMAP (requires neighborhood graph, see the previous code for Louvain clustering)
+sc.tl.umap(adataP)
+# Create a UMAP plot colored by cell type labels
+cell_annotations=adataP.obs['cell_type']
+sc.pl.umap(adataP, color='cell_type')
+```
+
+### Example 7 - Try genoSig for finding gene signatures for cell/data classes
 
 ```python
 import numpy as np
 import scipy.io as sio
 from genomap.utils.util_Sig import createGenomap_for_sig
 import pandas as pd
 import genomap.genoSig as gp
@@ -253,15 +307,15 @@
 genoMaps,gene_namesRe,T=createGenomap_for_sig(data,gene_names,rowNum,colNum)
 # compute the gene signatures
 result=gp.genoSig(genoMaps,T,label,userPD,gene_namesRe, epochs=50)
 
 print(result.head())
 ```
 
-### Example 7 - Try genoClassification for tabular data classification
+### Example 8 - Try genoClassification for tabular data classification
 
 ```python
 import pandas as pd
 import numpy as np
 import scipy.io as sio
 import genomap.genoClassification as gp
 from genomap.utils.util_genoClassReg import select_random_values
@@ -290,16 +344,15 @@
 test_data=data.values[indxTest-1]
 
 est=gp.genoClassification(training_data, training_labels, test_data, rowNum=rowNum, colNum=colNum, epoch=150)
 
 print('Classification accuracy of genomap approach:'+str(np.sum(est==groundTruthTest) / est.shape[0]))  
 ```
 
-
-### Example 8 - Try genoRegression for tabular data regression
+### Example 9 - Try genoRegression for tabular data regression
 
 ```python
 import pandas as pd
 import numpy as np
 import scipy.io as sio
 import genomap.genoRegression as gp
 from sklearn.metrics import mean_squared_error
```

### Comparing `genomap-1.2.9/genomap.egg-info/SOURCES.txt` & `genomap-1.3.0/genomap.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 genomap.egg-info/PKG-INFO
 genomap.egg-info/SOURCES.txt
 genomap.egg-info/dependency_links.txt
 genomap.egg-info/requires.txt
 genomap.egg-info/top_level.txt
 genomap/bregman_genomap/__init__.py
 genomap/bregman_genomap/bregman_genomap.py
+genomap/genoAnnotate/__init__.py
+genomap/genoAnnotate/genoAnnotate.py
 genomap/genoClassification/__init__.py
 genomap/genoClassification/genoClassification.py
 genomap/genoDR/__init__.py
 genomap/genoDR/genoDimReduction.py
 genomap/genoMOI/__init__.py
 genomap/genoMOI/genoMOI.py
 genomap/genoNet/__init__.py
@@ -33,14 +35,16 @@
 genomap/genoTraj/genoTraj.py
 genomap/genoVis/__init__.py
 genomap/genoVis/genoVis.py
 genomap/genomapOPT/__init__.py
 genomap/genomapOPT/genomapOPT.py
 genomap/genomapT/__init__.py
 genomap/genomapT/genomapT.py
+genomap/genotype/__init__.py
+genomap/genotype/genotype.py
 genomap/utils/ConvDEC.py
 genomap/utils/ConvIDEC.py
 genomap/utils/FcDEC.py
 genomap/utils/FcIDEC.py
 genomap/utils/__init__.py
 genomap/utils/class_discriminative_opt.py
 genomap/utils/gTraj_utils.py
```

### Comparing `genomap-1.2.9/setup.py` & `genomap-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="genomap",
-    version="1.2.9",
+    version="1.3.0",
     author="Md Tauhidul Islam",
     author_email="tauhid@stanford.edu",
     description="Genomap converts tabular gene expression data into spatially meaningful images.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xinglab-ai/genomap",
     classifiers=[
```

