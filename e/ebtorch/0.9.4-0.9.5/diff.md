# Comparing `tmp/ebtorch-0.9.4.tar.gz` & `tmp/ebtorch-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebtorch-0.9.4.tar", last modified: Sun Jul 23 23:20:12 2023, max compression
+gzip compressed data, was "ebtorch-0.9.5.tar", last modified: Mon Jul 24 14:07:19 2023, max compression
```

## Comparing `ebtorch-0.9.4.tar` & `ebtorch-0.9.5.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:20:12.126189 ebtorch-0.9.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-23 23:20:00.000000 ebtorch-0.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-23 23:20:12.126189 ebtorch-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-23 23:20:00.000000 ebtorch-0.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:20:12.114189 ebtorch-0.9.4/ebtorch/
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-23 23:20:00.000000 ebtorch-0.9.4/ebtorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:20:12.114189 ebtorch-0.9.4/ebtorch/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-23 23:20:00.000000 ebtorch-0.9.4/ebtorch/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-23 23:20:00.000000 ebtorch-0.9.4/ebtorch/logging/avgmeter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-23 23:20:00.000000 ebtorch-0.9.4/ebtorch/logging/logcsv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:20:12.118189 ebtorch-0.9.4/ebtorch/nn/
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-23 23:20:00.000000 ebtorch-0.9.4/ebtorch/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13998 2023-07-23 23:20:00.000000 ebtorch-0.9.4/ebtorch/nn/architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-07-23 23:20:00.000000 ebtorch-0.9.4/ebtorch/nn/conv2drp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-23 23:20:00.000000 ebtorch-0.9.4/ebtorch/nn/convolutional_flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)    13699 2023-07-23 23:20:00.000000 ebtorch-0.9.4/ebtorch/nn/coordconv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-23 23:20:00.000000 ebtorch-0.9.4/ebtorch/nn/debuglayers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-23 23:20:00.000000 ebtorch-0.9.4/ebtorch/nn/fieldtransform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:20:12.118189 ebtorch-0.9.4/ebtorch/nn/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-23 23:20:00.000000 ebtorch-0.9.4/ebtorch/nn/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-07-23 23:20:00.000000 ebtorch-0.9.4/ebtorch/nn/functional/inner_functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-07-23 23:20:00.000000 ebtorch-0.9.4/ebtorch/nn/kwta.py
--rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-07-23 23:20:00.000000 ebtorch-0.9.4/ebtorch/nn/laplacenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-23 23:20:00.000000 ebtorch-0.9.4/ebtorch/nn/mish.py
--rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-07-23 23:20:00.000000 ebtorch-0.9.4/ebtorch/nn/nnsemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-23 23:20:00.000000 ebtorch-0.9.4/ebtorch/nn/reshapelayers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-23 23:20:00.000000 ebtorch-0.9.4/ebtorch/nn/serf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-23 23:20:00.000000 ebtorch-0.9.4/ebtorch/nn/serlu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-23 23:20:00.000000 ebtorch-0.9.4/ebtorch/nn/sinlu.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-23 23:20:00.000000 ebtorch-0.9.4/ebtorch/nn/smelu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:20:12.122189 ebtorch-0.9.4/ebtorch/nn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-23 23:20:00.000000 ebtorch-0.9.4/ebtorch/nn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-07-23 23:20:00.000000 ebtorch-0.9.4/ebtorch/nn/utils/adverutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-23 23:20:00.000000 ebtorch-0.9.4/ebtorch/nn/utils/autoclip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-23 23:20:00.000000 ebtorch-0.9.4/ebtorch/nn/utils/onlyutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-23 23:20:00.000000 ebtorch-0.9.4/ebtorch/nn/utils/patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-07-23 23:20:00.000000 ebtorch-0.9.4/ebtorch/nn/utils/reprutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:20:12.126189 ebtorch-0.9.4/ebtorch/optim/
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-23 23:20:00.000000 ebtorch-0.9.4/ebtorch/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-07-23 23:20:00.000000 ebtorch-0.9.4/ebtorch/optim/adabound.py
--rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-07-23 23:20:00.000000 ebtorch-0.9.4/ebtorch/optim/adahessian.py
--rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-07-23 23:20:00.000000 ebtorch-0.9.4/ebtorch/optim/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)    20042 2023-07-23 23:20:00.000000 ebtorch-0.9.4/ebtorch/optim/autowu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-07-23 23:20:00.000000 ebtorch-0.9.4/ebtorch/optim/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-23 23:20:00.000000 ebtorch-0.9.4/ebtorch/optim/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-07-23 23:20:00.000000 ebtorch-0.9.4/ebtorch/optim/lookahead.py
--rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-07-23 23:20:00.000000 ebtorch-0.9.4/ebtorch/optim/lookaround.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-23 23:20:00.000000 ebtorch-0.9.4/ebtorch/optim/radam.py
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-07-23 23:20:00.000000 ebtorch-0.9.4/ebtorch/optim/sam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:20:12.114189 ebtorch-0.9.4/ebtorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-23 23:20:12.000000 ebtorch-0.9.4/ebtorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-23 23:20:12.000000 ebtorch-0.9.4/ebtorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 23:20:12.000000 ebtorch-0.9.4/ebtorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 23:20:11.000000 ebtorch-0.9.4/ebtorch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-23 23:20:12.000000 ebtorch-0.9.4/ebtorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 23:20:12.126189 ebtorch-0.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-23 23:20:00.000000 ebtorch-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:07:19.607460 ebtorch-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-24 14:07:00.000000 ebtorch-0.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-24 14:07:19.607460 ebtorch-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-24 14:07:00.000000 ebtorch-0.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:07:19.599460 ebtorch-0.9.5/ebtorch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:07:19.599460 ebtorch-0.9.5/ebtorch/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/logging/avgmeter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/logging/logcsv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:07:19.603460 ebtorch-0.9.5/ebtorch/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13998 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/conv2drp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/convolutional_flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13699 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/coordconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/debuglayers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/fieldtransform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:07:19.603460 ebtorch-0.9.5/ebtorch/nn/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/functional/inner_functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/kwta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/laplacenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/mish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/nnsemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/reshapelayers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/serf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/serlu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/sinlu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/smelu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:07:19.603460 ebtorch-0.9.5/ebtorch/nn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/utils/adverutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/utils/autoclip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/utils/onlyutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/utils/patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/utils/reprutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:07:19.607460 ebtorch-0.9.5/ebtorch/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/optim/adabound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/optim/adahessian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/optim/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20036 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/optim/autowu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/optim/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/optim/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/optim/lookahead.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/optim/lookaround.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/optim/radam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/optim/sam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:07:19.599460 ebtorch-0.9.5/ebtorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-24 14:07:19.000000 ebtorch-0.9.5/ebtorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-24 14:07:19.000000 ebtorch-0.9.5/ebtorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 14:07:19.000000 ebtorch-0.9.5/ebtorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 14:07:19.000000 ebtorch-0.9.5/ebtorch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 14:07:19.000000 ebtorch-0.9.5/ebtorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 14:07:19.607460 ebtorch-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-24 14:07:00.000000 ebtorch-0.9.5/setup.py
```

### Comparing `ebtorch-0.9.4/LICENSE` & `ebtorch-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.4/PKG-INFO` & `ebtorch-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebtorch
-Version: 0.9.4
+Version: 0.9.5
 Summary: Collection of PyTorch additions, extensions, utilities, uses and abuses
 Home-page: https://github.com/emaballarin/ebtorch
 Author: Emanuele Ballarin
 Author-email: emanuele@ballarin.cc
 License: Apache-2.0
 Keywords: Deep Learning,Machine Learning
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ebtorch Version: 0.9.4 Summary: Collection of
+Metadata-Version: 2.1 Name: ebtorch Version: 0.9.5 Summary: Collection of
 PyTorch additions, extensions, utilities, uses and abuses Home-page: https://
 github.com/emaballarin/ebtorch Author: Emanuele Ballarin Author-email:
 emanuele@ballarin.cc License: Apache-2.0 Keywords: Deep Learning,Machine
 Learning Classifier: Development Status :: 3 - Alpha Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Environment ::
 Console Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: Apache Software License Requires-Python: >=3.8 Description-
```

### Comparing `ebtorch-0.9.4/ebtorch/__init__.py` & `ebtorch-0.9.5/ebtorch/__init__.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.4/ebtorch/logging/__init__.py` & `ebtorch-0.9.5/ebtorch/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.4/ebtorch/logging/avgmeter.py` & `ebtorch-0.9.5/ebtorch/logging/avgmeter.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.4/ebtorch/logging/logcsv.py` & `ebtorch-0.9.5/ebtorch/logging/logcsv.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.4/ebtorch/nn/__init__.py` & `ebtorch-0.9.5/ebtorch/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.4/ebtorch/nn/architectures.py` & `ebtorch-0.9.5/ebtorch/nn/architectures.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.4/ebtorch/nn/conv2drp.py` & `ebtorch-0.9.5/ebtorch/nn/conv2drp.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.4/ebtorch/nn/convolutional_flatten.py` & `ebtorch-0.9.5/ebtorch/nn/convolutional_flatten.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.4/ebtorch/nn/coordconv.py` & `ebtorch-0.9.5/ebtorch/nn/coordconv.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.4/ebtorch/nn/debuglayers.py` & `ebtorch-0.9.5/ebtorch/nn/debuglayers.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.4/ebtorch/nn/fieldtransform.py` & `ebtorch-0.9.5/ebtorch/nn/fieldtransform.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.4/ebtorch/nn/functional/__init__.py` & `ebtorch-0.9.5/ebtorch/nn/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.4/ebtorch/nn/functional/inner_functional.py` & `ebtorch-0.9.5/ebtorch/nn/functional/inner_functional.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.4/ebtorch/nn/kwta.py` & `ebtorch-0.9.5/ebtorch/nn/kwta.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.4/ebtorch/nn/laplacenet.py` & `ebtorch-0.9.5/ebtorch/nn/laplacenet.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.4/ebtorch/nn/mish.py` & `ebtorch-0.9.5/ebtorch/nn/mish.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.4/ebtorch/nn/nnsemble.py` & `ebtorch-0.9.5/ebtorch/nn/nnsemble.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.4/ebtorch/nn/reshapelayers.py` & `ebtorch-0.9.5/ebtorch/nn/reshapelayers.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.4/ebtorch/nn/serf.py` & `ebtorch-0.9.5/ebtorch/nn/serf.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.4/ebtorch/nn/serlu.py` & `ebtorch-0.9.5/ebtorch/nn/serlu.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.4/ebtorch/nn/sinlu.py` & `ebtorch-0.9.5/ebtorch/nn/sinlu.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.4/ebtorch/nn/smelu.py` & `ebtorch-0.9.5/ebtorch/nn/smelu.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.4/ebtorch/nn/utils/__init__.py` & `ebtorch-0.9.5/ebtorch/nn/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.4/ebtorch/nn/utils/adverutils.py` & `ebtorch-0.9.5/ebtorch/nn/utils/adverutils.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.4/ebtorch/nn/utils/autoclip.py` & `ebtorch-0.9.5/ebtorch/nn/utils/autoclip.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.4/ebtorch/nn/utils/onlyutils.py` & `ebtorch-0.9.5/ebtorch/nn/utils/onlyutils.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.4/ebtorch/nn/utils/patches.py` & `ebtorch-0.9.5/ebtorch/nn/utils/patches.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.4/ebtorch/nn/utils/reprutils.py` & `ebtorch-0.9.5/ebtorch/nn/utils/reprutils.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.4/ebtorch/optim/__init__.py` & `ebtorch-0.9.5/ebtorch/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.4/ebtorch/optim/adabound.py` & `ebtorch-0.9.5/ebtorch/optim/adabound.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.4/ebtorch/optim/adahessian.py` & `ebtorch-0.9.5/ebtorch/optim/adahessian.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.4/ebtorch/optim/adan.py` & `ebtorch-0.9.5/ebtorch/optim/adan.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.4/ebtorch/optim/autowu.py` & `ebtorch-0.9.5/ebtorch/optim/autowu.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         if noise:
             pred_dist = self.likelihood(self.gp_model(pred_locs))
         else:
             pred_dist = self.gp_model(pred_locs)
         return pred_dist
 
 
-class AutoWU(object):
+class AutoWU:
     """Automatic LR scheduler using GP regression of diagnostics.
 
     Args:
         optimizer (torch.optim.Optimizer): Base optimizer.
         steps_per_epoch (int): Number of steps in an epoch.
         total_epochs (int): Total number of epochs.
         max_warmup_fraction (float, optional): The maximum fraction of total steps for
@@ -253,15 +253,15 @@
 
         self.start_warmup_phase_once()
 
     def step(self, loss):
         """Adjust LR when needed."""
         self.last_step += 1
 
-        scheduler_args = tuple()
+        scheduler_args: tuple = ()
 
         time_to_cooldown = (
             self.last_step
             >= (1 - self.cooldown_phase_states["fraction"]) * self.total_steps
         )
         if time_to_cooldown:
             self.start_cooldown_phase_once()
```

### Comparing `ebtorch-0.9.4/ebtorch/optim/custom.py` & `ebtorch-0.9.5/ebtorch/optim/custom.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.4/ebtorch/optim/lion.py` & `ebtorch-0.9.5/ebtorch/optim/lion.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.4/ebtorch/optim/lookahead.py` & `ebtorch-0.9.5/ebtorch/optim/lookahead.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.4/ebtorch/optim/lookaround.py` & `ebtorch-0.9.5/ebtorch/optim/lookaround.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.4/ebtorch/optim/radam.py` & `ebtorch-0.9.5/ebtorch/optim/radam.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.4/ebtorch/optim/sam.py` & `ebtorch-0.9.5/ebtorch/optim/sam.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.4/ebtorch.egg-info/PKG-INFO` & `ebtorch-0.9.5/ebtorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebtorch
-Version: 0.9.4
+Version: 0.9.5
 Summary: Collection of PyTorch additions, extensions, utilities, uses and abuses
 Home-page: https://github.com/emaballarin/ebtorch
 Author: Emanuele Ballarin
 Author-email: emanuele@ballarin.cc
 License: Apache-2.0
 Keywords: Deep Learning,Machine Learning
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ebtorch Version: 0.9.4 Summary: Collection of
+Metadata-Version: 2.1 Name: ebtorch Version: 0.9.5 Summary: Collection of
 PyTorch additions, extensions, utilities, uses and abuses Home-page: https://
 github.com/emaballarin/ebtorch Author: Emanuele Ballarin Author-email:
 emanuele@ballarin.cc License: Apache-2.0 Keywords: Deep Learning,Machine
 Learning Classifier: Development Status :: 3 - Alpha Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Environment ::
 Console Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: Apache Software License Requires-Python: >=3.8 Description-
```

### Comparing `ebtorch-0.9.4/ebtorch.egg-info/SOURCES.txt` & `ebtorch-0.9.5/ebtorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.4/setup.py` & `ebtorch-0.9.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 check_dependencies(DEPENDENCY_PACKAGE_NAMES)
 
 PACKAGENAME: str = "ebtorch"
 
 
 setup(
     name=PACKAGENAME,
-    version="0.9.4",
+    version="0.9.5",
     author="Emanuele Ballarin",
     author_email="emanuele@ballarin.cc",
     url="https://github.com/emaballarin/ebtorch",
     description="Collection of PyTorch additions, extensions, utilities, uses and abuses",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     keywords=["Deep Learning", "Machine Learning"],
```

