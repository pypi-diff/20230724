# Comparing `tmp/genomap-1.3.2.tar.gz` & `tmp/genomap-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genomap-1.3.2.tar", last modified: Mon Jul 24 19:18:09 2023, max compression
+gzip compressed data, was "genomap-1.3.3.tar", last modified: Mon Jul 24 20:07:25 2023, max compression
```

## Comparing `genomap-1.3.2.tar` & `genomap-1.3.3.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:09.212290 genomap-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-24 19:13:22.000000 genomap-1.3.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-24 19:13:22.000000 genomap-1.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13593 2023-07-24 19:18:09.212290 genomap-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-07-24 19:13:23.000000 genomap-1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:09.180290 genomap-1.3.2/data/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-24 19:13:23.000000 genomap-1.3.2/data/TM_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:09.180290 genomap-1.3.2/genomap/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:09.184290 genomap-1.3.2/genomap/bregman_genomap/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/bregman_genomap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   125058 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/bregman_genomap/bregman_genomap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:09.184290 genomap-1.3.2/genomap/genoAnnotate/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoAnnotate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoAnnotate/genoAnnotate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:09.192290 genomap-1.3.2/genomap/genoClassification/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoClassification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoClassification/genoClassification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:09.192290 genomap-1.3.2/genomap/genoDR/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoDR/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoDR/genoDimReduction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:09.192290 genomap-1.3.2/genomap/genoMOI/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoMOI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoMOI/genoMOI.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:09.192290 genomap-1.3.2/genomap/genoNet/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoNet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoNet/genoNet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:09.196290 genomap-1.3.2/genomap/genoNetRegression/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoNetRegression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoNetRegression/genoNet_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:09.196290 genomap-1.3.2/genomap/genoNetus/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoNetus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoNetus/genoNetus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:09.196290 genomap-1.3.2/genomap/genoRegression/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoRegression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoRegression/genoRegression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:09.200290 genomap-1.3.2/genomap/genoSig/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoSig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoSig/genoSig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:09.200290 genomap-1.3.2/genomap/genoTraj/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoTraj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoTraj/genoTraj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:09.200290 genomap-1.3.2/genomap/genoVis/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoVis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoVis/genoVis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genomap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:09.200290 genomap-1.3.2/genomap/genomapOPT/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genomapOPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genomapOPT/genomapOPT.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:09.200290 genomap-1.3.2/genomap/genomapT/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genomapT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genomapT/genomapT.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:09.204290 genomap-1.3.2/genomap/genotype/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genotype/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9775 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genotype/genotype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:09.212290 genomap-1.3.2/genomap/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/utils/ConvDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/utils/ConvIDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/utils/FcDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/utils/FcIDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/utils/class_discriminative_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/utils/gTraj_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/utils/group_centroid_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/utils/util_Sig.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/utils/util_genoClassReg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/utils/utils_MOI.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:09.184290 genomap-1.3.2/genomap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13593 2023-07-24 19:18:09.000000 genomap-1.3.2/genomap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-24 19:18:09.000000 genomap-1.3.2/genomap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 19:18:09.000000 genomap-1.3.2/genomap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-24 19:18:09.000000 genomap-1.3.2/genomap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 19:18:09.000000 genomap-1.3.2/genomap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-24 19:13:23.000000 genomap-1.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 19:18:09.212290 genomap-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-24 19:13:23.000000 genomap-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:07:25.653547 genomap-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-24 20:02:37.000000 genomap-1.3.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-24 20:02:37.000000 genomap-1.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13646 2023-07-24 20:07:25.653547 genomap-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13212 2023-07-24 20:02:37.000000 genomap-1.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:07:25.617547 genomap-1.3.3/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-24 20:02:37.000000 genomap-1.3.3/data/TM_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:07:25.617547 genomap-1.3.3/genomap/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:07:25.621547 genomap-1.3.3/genomap/bregman_genomap/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/bregman_genomap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125058 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/bregman_genomap/bregman_genomap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:07:25.621547 genomap-1.3.3/genomap/genoAnnotate/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoAnnotate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoAnnotate/genoAnnotate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:07:25.625547 genomap-1.3.3/genomap/genoClassification/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoClassification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoClassification/genoClassification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:07:25.625547 genomap-1.3.3/genomap/genoDR/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoDR/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoDR/genoDimReduction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:07:25.625547 genomap-1.3.3/genomap/genoMOI/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoMOI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoMOI/genoMOI.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:07:25.629547 genomap-1.3.3/genomap/genoNet/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoNet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoNet/genoNet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:07:25.629547 genomap-1.3.3/genomap/genoNetRegression/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoNetRegression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoNetRegression/genoNet_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:07:25.633547 genomap-1.3.3/genomap/genoNetus/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoNetus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoNetus/genoNetus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:07:25.633547 genomap-1.3.3/genomap/genoRegression/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoRegression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoRegression/genoRegression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:07:25.633547 genomap-1.3.3/genomap/genoSig/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoSig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoSig/genoSig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:07:25.637547 genomap-1.3.3/genomap/genoTraj/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoTraj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoTraj/genoTraj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:07:25.641547 genomap-1.3.3/genomap/genoVis/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoVis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genoVis/genoVis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genomap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:07:25.641547 genomap-1.3.3/genomap/genomapOPT/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genomapOPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genomapOPT/genomapOPT.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:07:25.641547 genomap-1.3.3/genomap/genomapT/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genomapT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genomapT/genomapT.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:07:25.645547 genomap-1.3.3/genomap/genotype/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genotype/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9775 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/genotype/genotype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:07:25.653547 genomap-1.3.3/genomap/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/utils/ConvDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/utils/ConvIDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/utils/FcDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/utils/FcIDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/utils/class_discriminative_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/utils/gTraj_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/utils/group_centroid_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/utils/util_Sig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/utils/util_genoClassReg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-24 20:02:37.000000 genomap-1.3.3/genomap/utils/utils_MOI.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:07:25.621547 genomap-1.3.3/genomap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13646 2023-07-24 20:07:25.000000 genomap-1.3.3/genomap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-24 20:07:25.000000 genomap-1.3.3/genomap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 20:07:25.000000 genomap-1.3.3/genomap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-24 20:07:25.000000 genomap-1.3.3/genomap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 20:07:25.000000 genomap-1.3.3/genomap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-24 20:02:37.000000 genomap-1.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 20:07:25.653547 genomap-1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-24 20:02:37.000000 genomap-1.3.3/setup.py
```

### Comparing `genomap-1.3.2/LICENSE.txt` & `genomap-1.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `genomap-1.3.2/PKG-INFO` & `genomap-1.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomap
-Version: 1.3.2
+Version: 1.3.3
 Summary: Genomap converts tabular gene expression data into spatially meaningful images.
 Home-page: https://github.com/xinglab-ai/genomap
 Author: Md Tauhidul Islam
 Author-email: tauhid@stanford.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -183,15 +183,15 @@
 
 ```python
 import scanpy as sc
 import matplotlib.pyplot as plt
 import scipy.io as sio
 import numpy as np
 import pandas as pd
-from genomap.genoMOI import genoMOIvis, genoMOItraj
+import genomap.genoMOI as gp
 
 # Load five different pancreatic datasets
 dx = sio.loadmat('dataBaronX.mat')
 data=dx['dataBaron']
 dx = sio.loadmat('dataMuraroX.mat')
 data2=dx['dataMuraro']
 dx = sio.loadmat('dataScapleX.mat')
@@ -205,15 +205,15 @@
 dx = sio.loadmat('classLabel.mat')
 y = np.squeeze(dx['classLabel'])
 dx = sio.loadmat('batchLabel.mat')
 ybatch = np.squeeze(dx['batchLabel'])
 
 # Apply genomap-based multi omic integration and visualize the integrated data with local structure for cluster analysis
 # returns 2D visualization, cluster labels, and intgerated data
-resVis,cli,int_data=genoMOIvis(data, data2, data3, data4, data5, colNum=12, rowNum=12, n_dim=32, epoch=10, prealign_method='scanorama')
+resVis,cli,int_data=gp.genoMOIvis(data, data2, data3, data4, data5, colNum=12, rowNum=12, n_dim=32, epoch=10, prealign_method='scanorama')
 
 
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
 h1=plt.scatter(resVis[:, 0], resVis[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
 plt.xlabel('genoVis1')
 plt.ylabel('genoVis2')
@@ -231,15 +231,15 @@
 plt.show()
 ```
 
 ```python
 # Apply genomap-based multi omic integration and visualize the integrated data with global structure for trajectory analysis
 
 # returns 2D embedding, cluster labels, and intgerated data
-resTraj,cli,int_data=genoMOItraj(data, data2, data3, data4, data5, colNum=12, rowNum=12, n_dim=32, epoch=10, prealign_method='scanorama')
+resTraj,cli,int_data=gp.genoMOItraj(data, data2, data3, data4, data5, colNum=12, rowNum=12, n_dim=32, epoch=10, prealign_method='scanorama')
 
 
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
 h1=plt.scatter(resTraj[:, 0], resTraj[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
 plt.xlabel('genoTraj1')
 plt.ylabel('genoTraj2')
@@ -259,28 +259,30 @@
 
 ### Example 6 - Try genoAnnotate for cell annotation
 
 ```python
 import scanpy as sc
 import pandas as pd
 import genomap.genoAnnotate as gp
+import matplotlib.pyplot as plt
 #Load the PBMC dataset
-adata = sc.read_10x_mtx("pbmc3k_filtered_gene_bc_matrices/")
+adata = sc.read_10x_mtx("./pbmc3k_filtered_gene_bc_matrices/")
 
 # Input: adata: annData containing the raw gene counts
 # tissue type: e.g. Immune system,Pancreas,Liver,Eye,Kidney,Brain,Lung,Adrenal,Heart,Intestine,Muscle,Placenta,Spleen,Stomach,Thymus 
  
-adataP = gp.genoAnnotate(adata,tissue_type="Immune system")
-
-
-# Compute UMAP (requires neighborhood graph, see the previous code for Louvain clustering)
-sc.tl.umap(adataP)
-# Create a UMAP plot colored by cell type labels
+adataP=gp.genoAnnotate(adata,species="human", tissue_type="Immune system")
+cell_annotations=adataP.obs['cell_type'].values # numpy array containing the
+# cell annotations
+
+# Compute t-SNE
+sc.tl.tsne(adataP)
+# Create a t-SNE plot colored by cell type labels
 cell_annotations=adataP.obs['cell_type']
-sc.pl.umap(adataP, color='cell_type')
+sc.pl.tsne(adataP, color='cell_type')
 ```
 
 ### Example 7 - Try genoSig for finding gene signatures for cell/data classes
 
 ```python
 import numpy as np
 import scipy.io as sio
```

### Comparing `genomap-1.3.2/README.md` & `genomap-1.3.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -170,15 +170,15 @@
 
 ```python
 import scanpy as sc
 import matplotlib.pyplot as plt
 import scipy.io as sio
 import numpy as np
 import pandas as pd
-from genomap.genoMOI import genoMOIvis, genoMOItraj
+import genomap.genoMOI as gp
 
 # Load five different pancreatic datasets
 dx = sio.loadmat('dataBaronX.mat')
 data=dx['dataBaron']
 dx = sio.loadmat('dataMuraroX.mat')
 data2=dx['dataMuraro']
 dx = sio.loadmat('dataScapleX.mat')
@@ -192,15 +192,15 @@
 dx = sio.loadmat('classLabel.mat')
 y = np.squeeze(dx['classLabel'])
 dx = sio.loadmat('batchLabel.mat')
 ybatch = np.squeeze(dx['batchLabel'])
 
 # Apply genomap-based multi omic integration and visualize the integrated data with local structure for cluster analysis
 # returns 2D visualization, cluster labels, and intgerated data
-resVis,cli,int_data=genoMOIvis(data, data2, data3, data4, data5, colNum=12, rowNum=12, n_dim=32, epoch=10, prealign_method='scanorama')
+resVis,cli,int_data=gp.genoMOIvis(data, data2, data3, data4, data5, colNum=12, rowNum=12, n_dim=32, epoch=10, prealign_method='scanorama')
 
 
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
 h1=plt.scatter(resVis[:, 0], resVis[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
 plt.xlabel('genoVis1')
 plt.ylabel('genoVis2')
@@ -218,15 +218,15 @@
 plt.show()
 ```
 
 ```python
 # Apply genomap-based multi omic integration and visualize the integrated data with global structure for trajectory analysis
 
 # returns 2D embedding, cluster labels, and intgerated data
-resTraj,cli,int_data=genoMOItraj(data, data2, data3, data4, data5, colNum=12, rowNum=12, n_dim=32, epoch=10, prealign_method='scanorama')
+resTraj,cli,int_data=gp.genoMOItraj(data, data2, data3, data4, data5, colNum=12, rowNum=12, n_dim=32, epoch=10, prealign_method='scanorama')
 
 
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
 h1=plt.scatter(resTraj[:, 0], resTraj[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
 plt.xlabel('genoTraj1')
 plt.ylabel('genoTraj2')
@@ -246,28 +246,30 @@
 
 ### Example 6 - Try genoAnnotate for cell annotation
 
 ```python
 import scanpy as sc
 import pandas as pd
 import genomap.genoAnnotate as gp
+import matplotlib.pyplot as plt
 #Load the PBMC dataset
-adata = sc.read_10x_mtx("pbmc3k_filtered_gene_bc_matrices/")
+adata = sc.read_10x_mtx("./pbmc3k_filtered_gene_bc_matrices/")
 
 # Input: adata: annData containing the raw gene counts
 # tissue type: e.g. Immune system,Pancreas,Liver,Eye,Kidney,Brain,Lung,Adrenal,Heart,Intestine,Muscle,Placenta,Spleen,Stomach,Thymus 
  
-adataP = gp.genoAnnotate(adata,tissue_type="Immune system")
-
-
-# Compute UMAP (requires neighborhood graph, see the previous code for Louvain clustering)
-sc.tl.umap(adataP)
-# Create a UMAP plot colored by cell type labels
+adataP=gp.genoAnnotate(adata,species="human", tissue_type="Immune system")
+cell_annotations=adataP.obs['cell_type'].values # numpy array containing the
+# cell annotations
+
+# Compute t-SNE
+sc.tl.tsne(adataP)
+# Create a t-SNE plot colored by cell type labels
 cell_annotations=adataP.obs['cell_type']
-sc.pl.umap(adataP, color='cell_type')
+sc.pl.tsne(adataP, color='cell_type')
 ```
 
 ### Example 7 - Try genoSig for finding gene signatures for cell/data classes
 
 ```python
 import numpy as np
 import scipy.io as sio
```

### Comparing `genomap-1.3.2/genomap/bregman_genomap/bregman_genomap.py` & `genomap-1.3.3/genomap/bregman_genomap/bregman_genomap.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.2/genomap/genoAnnotate/genoAnnotate.py` & `genomap-1.3.3/genomap/genoAnnotate/genoAnnotate.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.2/genomap/genoClassification/genoClassification.py` & `genomap-1.3.3/genomap/genoClassification/genoClassification.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.2/genomap/genoDR/genoDimReduction.py` & `genomap-1.3.3/genomap/genoDR/genoDimReduction.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.2/genomap/genoMOI/genoMOI.py` & `genomap-1.3.3/genomap/genoMOI/genoMOI.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.2/genomap/genoNet/genoNet.py` & `genomap-1.3.3/genomap/genoNet/genoNet.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.2/genomap/genoNetRegression/genoNet_regression.py` & `genomap-1.3.3/genomap/genoNetRegression/genoNet_regression.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.2/genomap/genoNetus/genoNetus.py` & `genomap-1.3.3/genomap/genoNetus/genoNetus.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.2/genomap/genoRegression/genoRegression.py` & `genomap-1.3.3/genomap/genoRegression/genoRegression.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.2/genomap/genoSig/genoSig.py` & `genomap-1.3.3/genomap/genoSig/genoSig.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.2/genomap/genoTraj/genoTraj.py` & `genomap-1.3.3/genomap/genoTraj/genoTraj.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.2/genomap/genoVis/genoVis.py` & `genomap-1.3.3/genomap/genoVis/genoVis.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.2/genomap/genomap.py` & `genomap-1.3.3/genomap/genomap.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.2/genomap/genomapOPT/genomapOPT.py` & `genomap-1.3.3/genomap/genomapOPT/genomapOPT.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.2/genomap/genomapT/genomapT.py` & `genomap-1.3.3/genomap/genomapT/genomapT.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.2/genomap/genotype/genotype.py` & `genomap-1.3.3/genomap/genotype/genotype.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.2/genomap/utils/ConvDEC.py` & `genomap-1.3.3/genomap/utils/ConvDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.2/genomap/utils/ConvIDEC.py` & `genomap-1.3.3/genomap/utils/ConvIDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.2/genomap/utils/FcDEC.py` & `genomap-1.3.3/genomap/utils/FcDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.2/genomap/utils/FcIDEC.py` & `genomap-1.3.3/genomap/utils/FcIDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.2/genomap/utils/class_discriminative_opt.py` & `genomap-1.3.3/genomap/utils/class_discriminative_opt.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.2/genomap/utils/gTraj_utils.py` & `genomap-1.3.3/genomap/utils/gTraj_utils.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.2/genomap/utils/group_centroid_opt.py` & `genomap-1.3.3/genomap/utils/group_centroid_opt.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.2/genomap/utils/metrics.py` & `genomap-1.3.3/genomap/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.2/genomap/utils/util_Sig.py` & `genomap-1.3.3/genomap/utils/util_Sig.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.2/genomap/utils/utils_MOI.py` & `genomap-1.3.3/genomap/utils/utils_MOI.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.2/genomap.egg-info/PKG-INFO` & `genomap-1.3.3/genomap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomap
-Version: 1.3.2
+Version: 1.3.3
 Summary: Genomap converts tabular gene expression data into spatially meaningful images.
 Home-page: https://github.com/xinglab-ai/genomap
 Author: Md Tauhidul Islam
 Author-email: tauhid@stanford.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -183,15 +183,15 @@
 
 ```python
 import scanpy as sc
 import matplotlib.pyplot as plt
 import scipy.io as sio
 import numpy as np
 import pandas as pd
-from genomap.genoMOI import genoMOIvis, genoMOItraj
+import genomap.genoMOI as gp
 
 # Load five different pancreatic datasets
 dx = sio.loadmat('dataBaronX.mat')
 data=dx['dataBaron']
 dx = sio.loadmat('dataMuraroX.mat')
 data2=dx['dataMuraro']
 dx = sio.loadmat('dataScapleX.mat')
@@ -205,15 +205,15 @@
 dx = sio.loadmat('classLabel.mat')
 y = np.squeeze(dx['classLabel'])
 dx = sio.loadmat('batchLabel.mat')
 ybatch = np.squeeze(dx['batchLabel'])
 
 # Apply genomap-based multi omic integration and visualize the integrated data with local structure for cluster analysis
 # returns 2D visualization, cluster labels, and intgerated data
-resVis,cli,int_data=genoMOIvis(data, data2, data3, data4, data5, colNum=12, rowNum=12, n_dim=32, epoch=10, prealign_method='scanorama')
+resVis,cli,int_data=gp.genoMOIvis(data, data2, data3, data4, data5, colNum=12, rowNum=12, n_dim=32, epoch=10, prealign_method='scanorama')
 
 
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
 h1=plt.scatter(resVis[:, 0], resVis[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
 plt.xlabel('genoVis1')
 plt.ylabel('genoVis2')
@@ -231,15 +231,15 @@
 plt.show()
 ```
 
 ```python
 # Apply genomap-based multi omic integration and visualize the integrated data with global structure for trajectory analysis
 
 # returns 2D embedding, cluster labels, and intgerated data
-resTraj,cli,int_data=genoMOItraj(data, data2, data3, data4, data5, colNum=12, rowNum=12, n_dim=32, epoch=10, prealign_method='scanorama')
+resTraj,cli,int_data=gp.genoMOItraj(data, data2, data3, data4, data5, colNum=12, rowNum=12, n_dim=32, epoch=10, prealign_method='scanorama')
 
 
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
 h1=plt.scatter(resTraj[:, 0], resTraj[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
 plt.xlabel('genoTraj1')
 plt.ylabel('genoTraj2')
@@ -259,28 +259,30 @@
 
 ### Example 6 - Try genoAnnotate for cell annotation
 
 ```python
 import scanpy as sc
 import pandas as pd
 import genomap.genoAnnotate as gp
+import matplotlib.pyplot as plt
 #Load the PBMC dataset
-adata = sc.read_10x_mtx("pbmc3k_filtered_gene_bc_matrices/")
+adata = sc.read_10x_mtx("./pbmc3k_filtered_gene_bc_matrices/")
 
 # Input: adata: annData containing the raw gene counts
 # tissue type: e.g. Immune system,Pancreas,Liver,Eye,Kidney,Brain,Lung,Adrenal,Heart,Intestine,Muscle,Placenta,Spleen,Stomach,Thymus 
  
-adataP = gp.genoAnnotate(adata,tissue_type="Immune system")
-
-
-# Compute UMAP (requires neighborhood graph, see the previous code for Louvain clustering)
-sc.tl.umap(adataP)
-# Create a UMAP plot colored by cell type labels
+adataP=gp.genoAnnotate(adata,species="human", tissue_type="Immune system")
+cell_annotations=adataP.obs['cell_type'].values # numpy array containing the
+# cell annotations
+
+# Compute t-SNE
+sc.tl.tsne(adataP)
+# Create a t-SNE plot colored by cell type labels
 cell_annotations=adataP.obs['cell_type']
-sc.pl.umap(adataP, color='cell_type')
+sc.pl.tsne(adataP, color='cell_type')
 ```
 
 ### Example 7 - Try genoSig for finding gene signatures for cell/data classes
 
 ```python
 import numpy as np
 import scipy.io as sio
```

### Comparing `genomap-1.3.2/genomap.egg-info/SOURCES.txt` & `genomap-1.3.3/genomap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `genomap-1.3.2/setup.py` & `genomap-1.3.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="genomap",
-    version="1.3.2",
+    version="1.3.3",
     author="Md Tauhidul Islam",
     author_email="tauhid@stanford.edu",
     description="Genomap converts tabular gene expression data into spatially meaningful images.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xinglab-ai/genomap",
     classifiers=[
```

