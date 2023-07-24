# Comparing `tmp/genomap-1.3.1.tar.gz` & `tmp/genomap-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genomap-1.3.1.tar", last modified: Mon Jul 24 18:10:50 2023, max compression
+gzip compressed data, was "genomap-1.3.2.tar", last modified: Mon Jul 24 19:18:09 2023, max compression
```

## Comparing `genomap-1.3.1.tar` & `genomap-1.3.2.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:10:50.137690 genomap-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-24 18:06:15.000000 genomap-1.3.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-24 18:06:15.000000 genomap-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13593 2023-07-24 18:10:50.137690 genomap-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-07-24 18:06:15.000000 genomap-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:10:50.109690 genomap-1.3.1/data/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-24 18:06:15.000000 genomap-1.3.1/data/TM_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:10:50.109690 genomap-1.3.1/genomap/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:10:50.113690 genomap-1.3.1/genomap/bregman_genomap/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/bregman_genomap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   125058 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/bregman_genomap/bregman_genomap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:10:50.113690 genomap-1.3.1/genomap/genoAnnotate/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoAnnotate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoAnnotate/genoAnnotate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:10:50.113690 genomap-1.3.1/genomap/genoClassification/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoClassification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoClassification/genoClassification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:10:50.113690 genomap-1.3.1/genomap/genoDR/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoDR/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoDR/genoDimReduction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:10:50.117690 genomap-1.3.1/genomap/genoMOI/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoMOI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoMOI/genoMOI.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:10:50.117690 genomap-1.3.1/genomap/genoNet/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoNet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoNet/genoNet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:10:50.117690 genomap-1.3.1/genomap/genoNetRegression/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoNetRegression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoNetRegression/genoNet_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:10:50.117690 genomap-1.3.1/genomap/genoNetus/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoNetus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoNetus/genoNetus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:10:50.121690 genomap-1.3.1/genomap/genoRegression/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoRegression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoRegression/genoRegression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:10:50.121690 genomap-1.3.1/genomap/genoSig/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoSig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoSig/genoSig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:10:50.121690 genomap-1.3.1/genomap/genoTraj/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoTraj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoTraj/genoTraj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:10:50.125690 genomap-1.3.1/genomap/genoVis/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoVis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genoVis/genoVis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genomap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:10:50.125690 genomap-1.3.1/genomap/genomapOPT/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genomapOPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genomapOPT/genomapOPT.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:10:50.125690 genomap-1.3.1/genomap/genomapT/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genomapT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genomapT/genomapT.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:10:50.133690 genomap-1.3.1/genomap/genotype/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genotype/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/genotype/genotype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:10:50.137690 genomap-1.3.1/genomap/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/utils/ConvDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/utils/ConvIDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/utils/FcDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/utils/FcIDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/utils/class_discriminative_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/utils/gTraj_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/utils/group_centroid_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/utils/util_Sig.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/utils/util_genoClassReg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-24 18:06:15.000000 genomap-1.3.1/genomap/utils/utils_MOI.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:10:50.109690 genomap-1.3.1/genomap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13593 2023-07-24 18:10:50.000000 genomap-1.3.1/genomap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-24 18:10:50.000000 genomap-1.3.1/genomap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:10:50.000000 genomap-1.3.1/genomap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-24 18:10:50.000000 genomap-1.3.1/genomap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 18:10:50.000000 genomap-1.3.1/genomap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-24 18:06:15.000000 genomap-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 18:10:50.137690 genomap-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-24 18:06:15.000000 genomap-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:09.212290 genomap-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-24 19:13:22.000000 genomap-1.3.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-24 19:13:22.000000 genomap-1.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13593 2023-07-24 19:18:09.212290 genomap-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-07-24 19:13:23.000000 genomap-1.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:09.180290 genomap-1.3.2/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-24 19:13:23.000000 genomap-1.3.2/data/TM_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:09.180290 genomap-1.3.2/genomap/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:09.184290 genomap-1.3.2/genomap/bregman_genomap/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/bregman_genomap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125058 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/bregman_genomap/bregman_genomap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:09.184290 genomap-1.3.2/genomap/genoAnnotate/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoAnnotate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoAnnotate/genoAnnotate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:09.192290 genomap-1.3.2/genomap/genoClassification/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoClassification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoClassification/genoClassification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:09.192290 genomap-1.3.2/genomap/genoDR/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoDR/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoDR/genoDimReduction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:09.192290 genomap-1.3.2/genomap/genoMOI/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoMOI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoMOI/genoMOI.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:09.192290 genomap-1.3.2/genomap/genoNet/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoNet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoNet/genoNet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:09.196290 genomap-1.3.2/genomap/genoNetRegression/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoNetRegression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoNetRegression/genoNet_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:09.196290 genomap-1.3.2/genomap/genoNetus/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoNetus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoNetus/genoNetus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:09.196290 genomap-1.3.2/genomap/genoRegression/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoRegression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoRegression/genoRegression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:09.200290 genomap-1.3.2/genomap/genoSig/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoSig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoSig/genoSig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:09.200290 genomap-1.3.2/genomap/genoTraj/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoTraj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoTraj/genoTraj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:09.200290 genomap-1.3.2/genomap/genoVis/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoVis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genoVis/genoVis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genomap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:09.200290 genomap-1.3.2/genomap/genomapOPT/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genomapOPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genomapOPT/genomapOPT.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:09.200290 genomap-1.3.2/genomap/genomapT/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genomapT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genomapT/genomapT.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:09.204290 genomap-1.3.2/genomap/genotype/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genotype/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9775 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/genotype/genotype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:09.212290 genomap-1.3.2/genomap/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/utils/ConvDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/utils/ConvIDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/utils/FcDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/utils/FcIDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/utils/class_discriminative_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/utils/gTraj_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/utils/group_centroid_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/utils/util_Sig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/utils/util_genoClassReg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-24 19:13:23.000000 genomap-1.3.2/genomap/utils/utils_MOI.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:09.184290 genomap-1.3.2/genomap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13593 2023-07-24 19:18:09.000000 genomap-1.3.2/genomap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-24 19:18:09.000000 genomap-1.3.2/genomap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 19:18:09.000000 genomap-1.3.2/genomap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-24 19:18:09.000000 genomap-1.3.2/genomap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 19:18:09.000000 genomap-1.3.2/genomap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-24 19:13:23.000000 genomap-1.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 19:18:09.212290 genomap-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-24 19:13:23.000000 genomap-1.3.2/setup.py
```

### Comparing `genomap-1.3.1/LICENSE.txt` & `genomap-1.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `genomap-1.3.1/PKG-INFO` & `genomap-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomap
-Version: 1.3.1
+Version: 1.3.2
 Summary: Genomap converts tabular gene expression data into spatially meaningful images.
 Home-page: https://github.com/xinglab-ai/genomap
 Author: Md Tauhidul Islam
 Author-email: tauhid@stanford.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `genomap-1.3.1/README.md` & `genomap-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `genomap-1.3.1/genomap/bregman_genomap/bregman_genomap.py` & `genomap-1.3.2/genomap/bregman_genomap/bregman_genomap.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.1/genomap/genoAnnotate/genoAnnotate.py` & `genomap-1.3.2/genomap/genoAnnotate/genoAnnotate.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,92 +1,94 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Sun Jul 23 15:18:43 2023
-
-@author: Md Tauhidul Islam
-# This code is inspired by scType (https://github.com/IanevskiAleksandr/sc-type)
-# We are in the process of using image matching techique for further enhancement
-# of the cell annotation
-"""
-
-from genomap.genotype import *
-import scanpy as sc
-
-def genoAnnotate(adata,tissue_type,database=None):
-    # Input: adata: annData containing the raw gene counts
-    # tissue type: e.g. Immune system,Pancreas,Liver,Eye,Kidney,Brain,Lung,Adrenal,Heart,Intestine,Muscle,Placenta,Spleen,Stomach,Thymus 
-    # database: User can select his/her own database in excel format
-
-    # Database file
-    if database==None:
-        database = "https://raw.githubusercontent.com/xinglab-ai/self-consistent-expression-recovery-machine/master/demo/data/genoANN_db.xlsx";        
-    
-    # Filter cells
-    sc.pp.filter_cells(adata, min_genes=200)
-    # Normalize data
-    adata.raw = adata
-    sc.pp.normalize_total(adata, target_sum=10000)
-    sc.pp.log1p(adata)
-    sc.pp.highly_variable_genes(adata, n_top_genes=2000)
-    adata = adata[:, adata.var['highly_variable']]
-    # Scale data and run PCA
-    sc.pp.scale(adata, max_value=10)
-    sc.tl.pca(adata)
-    
-    # Prepare positive and negative gene sets
-    result = gene_sets_prepare(database, tissue_type)
-    gs = result['gs_positive']
-    gs2 = result['gs_negative']
-    cell_types = result['cell_types']
-
-
-    data=adata.raw.X.toarray()
-    # Get cell-type by cell matrix
-    scRNAseqData = pd.DataFrame(data, index=adata.raw.obs_names, columns=adata.raw.var_names)
-
-    # Compute cell-type score fro each cell
-    es_max = sctype_score(scRNAseqData=scRNAseqData, scaled=True, gs=gs, gs2=gs2, cell_types=cell_types)
-    es_max.columns = cell_types
-    es_max.index = scRNAseqData.index
-
-    # Calculate neighborhood graph of cells (replace 'adata' with your actual AnnData object)
-    sc.pp.neighbors(adata, n_neighbors=10, use_rep='X_pca')
-    # Perform clustering so that cell-type can be assigned to each cluster
-    sc.tl.leiden(adata)
-    # The cluster labels are stored in `adata.obs['louvain']`
-    results = []
-    for cl in adata.obs['leiden'].unique():
-        cells_in_cluster = adata.obs_names[adata.obs['leiden'] == cl]
-        es_max_cl = es_max.loc[cells_in_cluster].sum().sort_values(ascending=False)
-        results.append(pd.DataFrame({
-            'cluster': cl,
-            'type': es_max_cl.index[:1],
-            'scores': es_max_cl.values[:1],
-            'ncells': len(cells_in_cluster)
-            }))
-
-    results = pd.concat(results)
-    results.loc[results['scores'] < results['ncells'] / 4, 'type'] = 'Unknown'
-    results.set_index('cluster', inplace=True)
-    # Assign the cell type labels to the cells in the AnnData object
-    adata.obs['cell_type'] = results.loc[adata.obs['leiden'], 'type'].values
-    return adata
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
+# -*- coding: utf-8 -*-
+"""
+Created on Sun Jul 23 15:18:43 2023
+
+@author: Md Tauhidul Islam
+# This code is inspired by scType (https://github.com/IanevskiAleksandr/sc-type)
+# We are in the process of using image matching techique for further enhancement
+# of the cell annotation
+"""
+
+
+from genomap.genotype import *
+import scanpy as sc
+
+def genoAnnotate(adata, species, tissue_type, database=None):
+    # Input: adata: annData containing the raw gene counts
+    # species :'human' or 'mouse'
+    # tissue type: e.g. Immune system,Pancreas,Liver,Eye,Kidney,Brain,Lung,Adrenal,Heart,Intestine,Muscle,Placenta,Spleen,Stomach,Thymus 
+    # database: User can select his/her own database in excel format
+
+    # Database file
+    if database==None:
+        database = "https://raw.githubusercontent.com/xinglab-ai/self-consistent-expression-recovery-machine/master/demo/data/genoANN_db.xlsx";        
+    
+    # Filter cells
+    sc.pp.filter_cells(adata, min_genes=200)
+    # Normalize data
+    adata.raw = adata
+    sc.pp.normalize_total(adata, target_sum=10000)
+    sc.pp.log1p(adata)
+    sc.pp.highly_variable_genes(adata, n_top_genes=2000)
+    adata = adata[:, adata.var['highly_variable']]
+    # Scale data and run PCA
+    sc.pp.scale(adata, max_value=10)
+    sc.tl.pca(adata)
+    
+    # Prepare positive and negative gene sets
+    result = gene_sets_prepare(database, tissue_type, species)
+    gs = result['gs_positive']
+    gs2 = result['gs_negative']
+    cell_types = result['cell_types']
+
+
+    data=adata.raw.X.toarray()
+    # Get cell-type by cell matrix
+    scRNAseqData = pd.DataFrame(data, index=adata.raw.obs_names, columns=adata.raw.var_names)
+
+    # Compute cell-type score fro each cell
+    es_max = sctype_score(scRNAseqData=scRNAseqData, scaled=True, gs=gs, gs2=gs2, cell_types=cell_types)
+    es_max.columns = cell_types
+    es_max.index = scRNAseqData.index
+
+    # Calculate neighborhood graph of cells (replace 'adata' with your actual AnnData object)
+    sc.pp.neighbors(adata, n_neighbors=10, use_rep='X_pca')
+    # Perform clustering so that cell-type can be assigned to each cluster
+    sc.tl.leiden(adata)
+    # The cluster labels are stored in `adata.obs['leiden']`
+    results = []
+    for cl in adata.obs['leiden'].unique():
+        cells_in_cluster = adata.obs_names[adata.obs['leiden'] == cl]
+        es_max_cl = es_max.loc[cells_in_cluster].sum().sort_values(ascending=False)
+        results.append(pd.DataFrame({
+            'cluster': cl,
+            'type': es_max_cl.index[:1],
+            'scores': es_max_cl.values[:1],
+            'ncells': len(cells_in_cluster)
+            }))
+
+    results = pd.concat(results)
+    results.loc[results['scores'] < results['ncells'] / 4, 'type'] = 'Unknown'
+    results.set_index('cluster', inplace=True)
+    # Assign the cell type labels to the cells in the AnnData object
+    adata.obs['cell_type'] = results.loc[adata.obs['leiden'], 'type'].values
+    return adata
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
```

### Comparing `genomap-1.3.1/genomap/genoClassification/genoClassification.py` & `genomap-1.3.2/genomap/genoClassification/genoClassification.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.1/genomap/genoDR/genoDimReduction.py` & `genomap-1.3.2/genomap/genoDR/genoDimReduction.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.1/genomap/genoMOI/genoMOI.py` & `genomap-1.3.2/genomap/genoMOI/genoMOI.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.1/genomap/genoNet/genoNet.py` & `genomap-1.3.2/genomap/genoNet/genoNet.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.1/genomap/genoNetRegression/genoNet_regression.py` & `genomap-1.3.2/genomap/genoNetRegression/genoNet_regression.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.1/genomap/genoNetus/genoNetus.py` & `genomap-1.3.2/genomap/genoNetus/genoNetus.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.1/genomap/genoRegression/genoRegression.py` & `genomap-1.3.2/genomap/genoRegression/genoRegression.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.1/genomap/genoSig/genoSig.py` & `genomap-1.3.2/genomap/genoSig/genoSig.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.1/genomap/genoTraj/genoTraj.py` & `genomap-1.3.2/genomap/genoTraj/genoTraj.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.1/genomap/genoVis/genoVis.py` & `genomap-1.3.2/genomap/genoVis/genoVis.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.1/genomap/genomap.py` & `genomap-1.3.2/genomap/genomap.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.1/genomap/genomapOPT/genomapOPT.py` & `genomap-1.3.2/genomap/genomapOPT/genomapOPT.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.1/genomap/genomapT/genomapT.py` & `genomap-1.3.2/genomap/genomapT/genomapT.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.1/genomap/genotype/genotype.py` & `genomap-1.3.2/genomap/genotype/genotype.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,226 +1,227 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Thu Jul 20 16:57:36 2023
-
-@author: Md Tauhidul Islam
-# This code is inspired by scType (https://github.com/IanevskiAleksandr/sc-type)
-# We are in the process of using image matching techique for further enhancement
-# of the cell annotation
-"""
-import pandas as pd
-import numpy as np
-import scipy
-import openpyxl
-from pybiomart import Dataset
-import re
-
-def sctype_score(scRNAseqData, scaled=True, gs=None, gs2=None, gene_names_to_uppercase=True, cell_types=None):
-    # Ensure input is a pandas DataFrame
-    if not isinstance(scRNAseqData, pd.DataFrame):
-        print("scRNAseqData doesn't seem to be a DataFrame")
-        return None
-    
-    # Check if DataFrame is empty
-    if scRNAseqData.empty:
-        print("The input scRNAseqData DataFrame is empty")
-        return None
-
-    # Marker sensitivity
-    marker_stat = pd.Series([gene for sublist in gs for gene in sublist]).value_counts().sort_values(ascending=False)
-    marker_sensitivity = pd.DataFrame({
-        "score_marker_sensitivity": (len(gs)-marker_stat.values) / (len(gs) - 1),
-        "gene_": marker_stat.index
-    }) 
-
-    # Convert gene names to uppercase
-    if gene_names_to_uppercase:
-        scRNAseqData.columns = scRNAseqData.columns.astype(str).str.upper()
-
-    # Subselect genes found in data
-    gs = [[gene for gene in sublist if gene in scRNAseqData.columns] for sublist in gs]
-    gs2 = [[gene for gene in sublist if gene in scRNAseqData.columns] for sublist in gs2]
-
-    cell_markers_genes_score = marker_sensitivity[marker_sensitivity['gene_'].isin(np.unique(np.concatenate(gs)))]
-
-    Z = scRNAseqData.copy()
-    
-    #scanpy.pp.scale(Z)
-    Z= scipy.stats.zscore(Z, axis=0, ddof=1)  
-    Z = Z.fillna(0)
-
-    # Multiply by marker sensitivity
-    Z = Z.T
-    for idx, row in cell_markers_genes_score.iterrows():
-        Z.loc[row["gene_"]] *= row["score_marker_sensitivity"]
-    Z = Z.T
-    # Subselect only with marker genes
-    Z = Z[np.unique(np.concatenate(gs + gs2))]    
-    Z=Z.T
-    score_series_list = []
-    # Loop over each gene symbol (gss_) in gs
-    
-    for i in range(0,len(gs)):
-        gss_=np.array(gs[i])
-        gss2_=np.array(gs2[i])
-        scores = []    
-        # Loop over each column (j) in Z
-        for j in range(Z.shape[1]):
-            gs_z = Z.loc[gss_].iloc[:, j]  # Using iloc for integer-based indexing  
-            gz_2 = Z.loc[gss2_].iloc[:, j] * -1  # Using iloc for integer-based indexing
-            sum_t1 = np.sum(gs_z) / np.sqrt(len(gs_z))
-            sum_t2 = np.sum(gz_2) / np.sqrt(len(gz_2))        
-            if np.isnan(sum_t2):
-                sum_t2 = 0        
-            scores.append(sum_t1 + sum_t2)    
-        # Convert the scores list to a pandas Series and add it to the score_series_list
-        score_series_list.append(pd.Series(scores))
-    # Concatenate the score series in score_series_list along axis 0 to create a DataFrame
-    es = pd.concat(score_series_list, axis=1)
-
-    # Remove rows with all NA or empty values
-    es = es.dropna(how='all')
-    es = es[~(es == "").all(axis=1)]
-
-    return es
-
-def gene_sets_prepare(path_to_db_file, cell_type):
-    # Read the Excel file
-    cell_markers = pd.read_excel(path_to_db_file, engine='openpyxl')
-
-    # Select rows where 'tissueType' matches 'cell_type'
-    cell_markers = cell_markers[cell_markers['tissueType'] == cell_type]
-    # Apply the function to each row in the DataFrame 'cell_markers'
-    # cell_markers['geneSymbolmore1'] = cell_markers['geneSymbolmore1'].apply(correct_gene_symbols)
-
-
-    # Convert to string and clean 'geneSymbolmore1' and 'geneSymbolmore2' columns
-    cell_markers['geneSymbolmore1'] = cell_markers['geneSymbolmore1'].astype(str).str.replace(" ", "")
-    cell_markers['geneSymbolmore2'] = cell_markers['geneSymbolmore2'].astype(str).str.replace(" ", "")
-    
- 
-    cell_markers["geneSymbolmore1"] = cell_markers["geneSymbolmore1"].apply(lambda x: correct_gene_symbols(x))
-    cell_markers["geneSymbolmore2"] = cell_markers["geneSymbolmore2"].apply(lambda x: correct_gene_symbols(x))
-    
-
-    # Define a helper function to handle potential NaN values
-    def process_genes(x):
-        if x == 'nan':
-            return []
-        else:
-            return sorted([i for i in x.split(",") if i not in ["NA", ""]])
-
-    # Split 'geneSymbolmore1' and 'geneSymbolmore2' into lists of genes
-    cell_markers['geneSymbolmore1'] = cell_markers['geneSymbolmore1'].apply(process_genes)
-    cell_markers['geneSymbolmore2'] = cell_markers['geneSymbolmore2'].apply(process_genes)
-
-    # Replace '///' with ',' and remove spaces
-    cell_markers['geneSymbolmore1'] = cell_markers['geneSymbolmore1'].apply(lambda x: ",".join(x).replace("///", ",").replace(" ", ""))
-    cell_markers['geneSymbolmore2'] = cell_markers['geneSymbolmore2'].apply(lambda x: ",".join(x).replace("///", ",").replace(" ", ""))
-
-    # Split 'geneSymbolmore1' and 'geneSymbolmore2' into lists of genes again
-    cell_markers['geneSymbolmore1'] = cell_markers['geneSymbolmore1'].str.split(",")
-    cell_markers['geneSymbolmore2'] = cell_markers['geneSymbolmore2'].str.split(",")
-
-    # Prepare 'gs' and 'gs2' lists
-    gs = [genes for genes in cell_markers['geneSymbolmore1']]
-    gs2 = [genes for genes in cell_markers['geneSymbolmore2']]
-    
-    # Prepare cell types list
-    cell_types = list(cell_markers['cellName'])
-
-    return {'gs_positive': gs, 'gs_negative': gs2, 'cell_types': cell_types}
-
-def correct_gene_symbols(gene_symbols, species="human"):
-    if isinstance(gene_symbols, str):
-        gene_symbols = gene_symbols.split(",")
-    gene_symbols = [gs.strip().replace(" ", "").upper() for gs in gene_symbols if gs.strip().upper() not in ["NA", ""]]
-    gene_symbols = sorted(set(gene_symbols))
-
-    if len(gene_symbols) > 0:
-        # Assuming you have defined and imported the gene_symbol_mapping function
-        # This function should perform the gene symbol mapping using pybiomart or any other method you have implemented.
-        # gene_symbol_mapping(markers_all) should return a DataFrame with the "Suggested.Symbol" column.
-        # For simplicity, I'll use a dummy function that returns an empty DataFrame here.
-        #def gene_symbol_mapping(gene_symbols):
-            #return pd.DataFrame(columns=["Suggested.Symbol"])
-
-        suppressMessages = lambda x: x  # Suppressing messages in Python is not necessary
-
-        markers_all = check_gene_symbols(gene_symbols)
-        markers_all = markers_all.dropna(subset=["Suggested.Symbol"])
-        markers_all = sorted(set(markers_all["Suggested.Symbol"]))
-
-        return ",".join(markers_all)
-    else:
-        return ""
-
-
-def check_gene_symbols(x, unmapped_as_na=True, map=None, species="human"):
-    if species == "human":
-        dataset_name = 'hsapiens_gene_ensembl'
-    elif species == "mouse":
-        dataset_name = 'mmusculus_gene_ensembl'
-    else:
-        raise ValueError("Species must be 'human' or 'mouse'")
-
-    biomart = Dataset(name=dataset_name, host='http://www.ensembl.org')
-    biomart_df = biomart.query(attributes=['external_gene_name', 'gene_biotype'])
-
-
-    casecorrection = False
-    if species == "human":
-        casecorrection = True
-        if map is None:
-            #lastupdate = biomart_df["date"].max()
-            #print("Maps last updated on:", lastupdate)
-            map = biomart_df[['Gene name', 'Gene type']].drop_duplicates()
-    elif species == "mouse" and map is None:
-        #lastupdate = biomart_df["date"].max()
-        #print("Maps last updated on:", lastupdate)
-        map = biomart_df[['Gene name', 'Gene type']].drop_duplicates()
-    else:
-        if map is None:
-            raise ValueError("If species is not 'human' or 'mouse', then map argument must be specified")
-
-    if not isinstance(map, pd.DataFrame) or not set(map.columns) == {"Gene name", "Gene type"}:
-        raise ValueError("If map is specified, it must be a dataframe with two columns named 'external_gene_name' and 'gene_biotype'")
-
-    approved = [sym in map["Gene name"].values for sym in x]
-
-    if casecorrection:
-        x_casecorrected = [sym.upper() for sym in x]
-        x_casecorrected = [re.sub(r"(.*C[0-9XY]+)ORF(.+)", r"\1orf\2", sym) for sym in x_casecorrected]
-    else:
-        x_casecorrected = x.split()
-
-    approvedaftercasecorrection = [sym in map["Gene name"].values for sym in x_casecorrected]
-
-    if x != " ".join(x_casecorrected):
-        print("Human gene symbols should be all upper-case except for the 'orf' in open reading frames. The case of some letters was corrected.")
-
-    alias = [sym in map["Gene name"].values for sym in x_casecorrected]
-
-    suggested_symbols = []
-    for i in range(len(x_casecorrected)):
-        if approved[i]:
-            suggested_symbols.append(x_casecorrected[i])
-        else:
-            if alias[i]:
-                suggested_symbols.append(" /// ".join(map.loc[map["Gene name"] == x_casecorrected[i], "Gene name"]))
-            elif approvedaftercasecorrection[i]:
-                suggested_symbols.append(x_casecorrected[i])
-            else:
-                suggested_symbols.append(None)
-
-    df = pd.DataFrame({"x": x, "Approved": approved, "Suggested.Symbol": suggested_symbols})
-    df["Approved"][df["x"].isnull()] = False
-
-    if not unmapped_as_na:
-        df.loc[df["Suggested.Symbol"].isnull(), "Suggested.Symbol"] = df.loc[df["Suggested.Symbol"].isnull(), "x"]
-
-    if df["Approved"].sum() != df.shape[0]:
-        print("x contains non-approved gene symbols")
-
-    return df
-
-
+# -*- coding: utf-8 -*-
+"""
+Created on Thu Jul 20 16:57:36 2023
+
+@author: Md Tauhidul Islam
+# This code is inspired by scType (https://github.com/IanevskiAleksandr/sc-type)
+# We are in the process of using image matching techique for further enhancement
+# of the cell annotation
+"""
+import numpy as np
+import openpyxl
+import pandas as pd
+from pybiomart import Dataset
+import re
+import scipy
+
+def sctype_score(scRNAseqData, scaled=True, gs=None, gs2=None, gene_names_to_uppercase=True, cell_types=None):
+    # Ensure input is a pandas DataFrame
+    if not isinstance(scRNAseqData, pd.DataFrame):
+        print("scRNAseqData doesn't seem to be a DataFrame")
+        return None
+    
+    # Check if DataFrame is empty
+    if scRNAseqData.empty:
+        print("The input scRNAseqData DataFrame is empty")
+        return None
+
+    # Marker sensitivity
+    marker_stat = pd.Series([gene for sublist in gs for gene in sublist]).value_counts().sort_values(ascending=False)
+    marker_sensitivity = pd.DataFrame({
+        "score_marker_sensitivity": (len(gs)-marker_stat.values) / (len(gs) - 1),
+        "gene_": marker_stat.index
+    }) 
+
+    # Convert gene names to uppercase
+    if gene_names_to_uppercase:
+        scRNAseqData.columns = scRNAseqData.columns.astype(str).str.upper()
+
+    # Subselect genes found in data
+    gs = [[gene for gene in sublist if gene in scRNAseqData.columns] for sublist in gs]
+    gs2 = [[gene for gene in sublist if gene in scRNAseqData.columns] for sublist in gs2]
+
+    cell_markers_genes_score = marker_sensitivity[marker_sensitivity['gene_'].isin(np.unique(np.concatenate(gs)))]
+
+    Z = scRNAseqData.copy()
+    
+    #scanpy.pp.scale(Z)
+    Z= scipy.stats.zscore(Z, axis=0, ddof=1)  
+    Z = Z.fillna(0)
+
+    # Multiply by marker sensitivity
+    Z = Z.T
+    for idx, row in cell_markers_genes_score.iterrows():
+        Z.loc[row["gene_"]] *= row["score_marker_sensitivity"]
+    Z = Z.T
+    # Subselect only with marker genes
+    Z = Z[np.unique(np.concatenate(gs + gs2))]    
+    Z=Z.T
+    score_series_list = []
+    # Loop over each gene symbol (gss_) in gs
+    
+    for i in range(0,len(gs)):
+        gss_=np.array(gs[i])
+        gss2_=np.array(gs2[i])
+        scores = []    
+        # Loop over each column (j) in Z
+        for j in range(Z.shape[1]):
+            gs_z = Z.loc[gss_].iloc[:, j]  # Using iloc for integer-based indexing  
+            gz_2 = Z.loc[gss2_].iloc[:, j] * -1  # Using iloc for integer-based indexing
+            sum_t1 = np.sum(gs_z) / np.sqrt(len(gs_z))
+            sum_t2 = np.sum(gz_2) / np.sqrt(len(gz_2))        
+            if np.isnan(sum_t2):
+                sum_t2 = 0        
+            scores.append(sum_t1 + sum_t2)    
+        # Convert the scores list to a pandas Series and add it to the score_series_list
+        score_series_list.append(pd.Series(scores))
+    # Concatenate the score series in score_series_list along axis 0 to create a DataFrame
+    es = pd.concat(score_series_list, axis=1)
+
+    # Remove rows with all NA or empty values
+    es = es.dropna(how='all')
+    es = es[~(es == "").all(axis=1)]
+
+    return es
+
+
+def gene_sets_prepare(path_to_db_file, cell_type, species="human"):
+    # Read the Excel file
+    cell_markers = pd.read_excel(path_to_db_file, engine='openpyxl')
+
+    # Select rows where 'tissueType' matches 'cell_type'
+    cell_markers = cell_markers[cell_markers['tissueType'] == cell_type]
+    # Apply the function to each row in the DataFrame 'cell_markers'
+    # cell_markers['geneSymbolmore1'] = cell_markers['geneSymbolmore1'].apply(correct_gene_symbols)
+
+
+    # Convert to string and clean 'geneSymbolmore1' and 'geneSymbolmore2' columns
+    cell_markers['geneSymbolmore1'] = cell_markers['geneSymbolmore1'].astype(str).str.replace(" ", "")
+    cell_markers['geneSymbolmore2'] = cell_markers['geneSymbolmore2'].astype(str).str.replace(" ", "")
+    
+ 
+    cell_markers["geneSymbolmore1"] = cell_markers["geneSymbolmore1"].apply(lambda x: correct_gene_symbols(x, species=species))
+    cell_markers["geneSymbolmore2"] = cell_markers["geneSymbolmore2"].apply(lambda x: correct_gene_symbols(x, species=species))
+    
+
+    # Define a helper function to handle potential NaN values
+    def process_genes(x):
+        if x == 'nan':
+            return []
+        else:
+            return sorted([i for i in x.split(",") if i not in ["NA", ""]])
+
+    # Split 'geneSymbolmore1' and 'geneSymbolmore2' into lists of genes
+    cell_markers['geneSymbolmore1'] = cell_markers['geneSymbolmore1'].apply(process_genes)
+    cell_markers['geneSymbolmore2'] = cell_markers['geneSymbolmore2'].apply(process_genes)
+
+    # Replace '///' with ',' and remove spaces
+    cell_markers['geneSymbolmore1'] = cell_markers['geneSymbolmore1'].apply(lambda x: ",".join(x).replace("///", ",").replace(" ", ""))
+    cell_markers['geneSymbolmore2'] = cell_markers['geneSymbolmore2'].apply(lambda x: ",".join(x).replace("///", ",").replace(" ", ""))
+
+    # Split 'geneSymbolmore1' and 'geneSymbolmore2' into lists of genes again
+    cell_markers['geneSymbolmore1'] = cell_markers['geneSymbolmore1'].str.split(",")
+    cell_markers['geneSymbolmore2'] = cell_markers['geneSymbolmore2'].str.split(",")
+
+    # Prepare 'gs' and 'gs2' lists
+    gs = [genes for genes in cell_markers['geneSymbolmore1']]
+    gs2 = [genes for genes in cell_markers['geneSymbolmore2']]
+    
+    # Prepare cell types list
+    cell_types = list(cell_markers['cellName'])
+
+    return {'gs_positive': gs, 'gs_negative': gs2, 'cell_types': cell_types}
+
+def correct_gene_symbols(gene_symbols, species="human"):
+    if isinstance(gene_symbols, str):
+        gene_symbols = gene_symbols.split(",")
+    gene_symbols = [gs.strip().replace(" ", "").upper() for gs in gene_symbols if gs.strip().upper() not in ["NA", ""]]
+    gene_symbols = sorted(set(gene_symbols))
+
+    if len(gene_symbols) > 0:
+        # Assuming you have defined and imported the gene_symbol_mapping function
+        # This function should perform the gene symbol mapping using pybiomart or any other method you have implemented.
+        # gene_symbol_mapping(markers_all) should return a DataFrame with the "Suggested.Symbol" column.
+        # For simplicity, I'll use a dummy function that returns an empty DataFrame here.
+        #def gene_symbol_mapping(gene_symbols):
+            #return pd.DataFrame(columns=["Suggested.Symbol"])
+
+        suppressMessages = lambda x: x  # Suppressing messages in Python is not necessary
+
+        markers_all = check_gene_symbols(gene_symbols)
+        markers_all = markers_all.dropna(subset=["Suggested.Symbol"])
+        markers_all = sorted(set(markers_all["Suggested.Symbol"]))
+
+        return ",".join(markers_all)
+    else:
+        return ""
+
+
+def check_gene_symbols(x, unmapped_as_na=True, map=None, species="human"):
+    if species == "human":
+        dataset_name = 'hsapiens_gene_ensembl'
+    elif species == "mouse":
+        dataset_name = 'mmusculus_gene_ensembl'
+    else:
+        raise ValueError("Species must be 'human' or 'mouse'")
+
+    biomart = Dataset(name=dataset_name, host='http://www.ensembl.org')
+    biomart_df = biomart.query(attributes=['external_gene_name', 'gene_biotype'])
+
+
+    casecorrection = False
+    if species == "human":
+        casecorrection = True
+        if map is None:
+            #lastupdate = biomart_df["date"].max()
+            #print("Maps last updated on:", lastupdate)
+            map = biomart_df[['Gene name', 'Gene type']].drop_duplicates()
+    elif species == "mouse" and map is None:
+        #lastupdate = biomart_df["date"].max()
+        #print("Maps last updated on:", lastupdate)
+        map = biomart_df[['Gene name', 'Gene type']].drop_duplicates()
+    else:
+        if map is None:
+            raise ValueError("If species is not 'human' or 'mouse', then map argument must be specified")
+
+    if not isinstance(map, pd.DataFrame) or not set(map.columns) == {"Gene name", "Gene type"}:
+        raise ValueError("If map is specified, it must be a dataframe with two columns named 'external_gene_name' and 'gene_biotype'")
+
+    approved = [sym in map["Gene name"].values for sym in x]
+
+    if casecorrection:
+        x_casecorrected = [sym.upper() for sym in x]
+        x_casecorrected = [re.sub(r"(.*C[0-9XY]+)ORF(.+)", r"\1orf\2", sym) for sym in x_casecorrected]
+    else:
+        x_casecorrected = x.split()
+
+    approvedaftercasecorrection = [sym in map["Gene name"].values for sym in x_casecorrected]
+
+    if x != " ".join(x_casecorrected):
+        print("Human gene symbols should be all upper-case except for the 'orf' in open reading frames. The case of some letters was corrected.")
+
+    alias = [sym in map["Gene name"].values for sym in x_casecorrected]
+
+    suggested_symbols = []
+    for i in range(len(x_casecorrected)):
+        if approved[i]:
+            suggested_symbols.append(x_casecorrected[i])
+        else:
+            if alias[i]:
+                suggested_symbols.append(" /// ".join(map.loc[map["Gene name"] == x_casecorrected[i], "Gene name"]))
+            elif approvedaftercasecorrection[i]:
+                suggested_symbols.append(x_casecorrected[i])
+            else:
+                suggested_symbols.append(None)
+
+    df = pd.DataFrame({"x": x, "Approved": approved, "Suggested.Symbol": suggested_symbols})
+    df["Approved"][df["x"].isnull()] = False
+
+    if not unmapped_as_na:
+        df.loc[df["Suggested.Symbol"].isnull(), "Suggested.Symbol"] = df.loc[df["Suggested.Symbol"].isnull(), "x"]
+
+    if df["Approved"].sum() != df.shape[0]:
+        print("x contains non-approved gene symbols")
+
+    return df
+
+
```

### Comparing `genomap-1.3.1/genomap/utils/ConvDEC.py` & `genomap-1.3.2/genomap/utils/ConvDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.1/genomap/utils/ConvIDEC.py` & `genomap-1.3.2/genomap/utils/ConvIDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.1/genomap/utils/FcDEC.py` & `genomap-1.3.2/genomap/utils/FcDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.1/genomap/utils/FcIDEC.py` & `genomap-1.3.2/genomap/utils/FcIDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.1/genomap/utils/class_discriminative_opt.py` & `genomap-1.3.2/genomap/utils/class_discriminative_opt.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.1/genomap/utils/gTraj_utils.py` & `genomap-1.3.2/genomap/utils/gTraj_utils.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.1/genomap/utils/group_centroid_opt.py` & `genomap-1.3.2/genomap/utils/group_centroid_opt.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.1/genomap/utils/metrics.py` & `genomap-1.3.2/genomap/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.1/genomap/utils/util_Sig.py` & `genomap-1.3.2/genomap/utils/util_Sig.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.1/genomap/utils/utils_MOI.py` & `genomap-1.3.2/genomap/utils/utils_MOI.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.1/genomap.egg-info/PKG-INFO` & `genomap-1.3.2/genomap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomap
-Version: 1.3.1
+Version: 1.3.2
 Summary: Genomap converts tabular gene expression data into spatially meaningful images.
 Home-page: https://github.com/xinglab-ai/genomap
 Author: Md Tauhidul Islam
 Author-email: tauhid@stanford.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `genomap-1.3.1/genomap.egg-info/SOURCES.txt` & `genomap-1.3.2/genomap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `genomap-1.3.1/setup.py` & `genomap-1.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="genomap",
-    version="1.3.1",
+    version="1.3.2",
     author="Md Tauhidul Islam",
     author_email="tauhid@stanford.edu",
     description="Genomap converts tabular gene expression data into spatially meaningful images.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xinglab-ai/genomap",
     classifiers=[
```

