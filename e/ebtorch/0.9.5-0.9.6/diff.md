# Comparing `tmp/ebtorch-0.9.5.tar.gz` & `tmp/ebtorch-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebtorch-0.9.5.tar", last modified: Mon Jul 24 14:07:19 2023, max compression
+gzip compressed data, was "ebtorch-0.9.6.tar", last modified: Mon Jul 24 15:52:09 2023, max compression
```

## Comparing `ebtorch-0.9.5.tar` & `ebtorch-0.9.6.tar`

### file list

```diff
@@ -1,57 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:07:19.607460 ebtorch-0.9.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-24 14:07:00.000000 ebtorch-0.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-24 14:07:19.607460 ebtorch-0.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-24 14:07:00.000000 ebtorch-0.9.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:07:19.599460 ebtorch-0.9.5/ebtorch/
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:07:19.599460 ebtorch-0.9.5/ebtorch/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/logging/avgmeter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/logging/logcsv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:07:19.603460 ebtorch-0.9.5/ebtorch/nn/
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13998 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/conv2drp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/convolutional_flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)    13699 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/coordconv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/debuglayers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/fieldtransform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:07:19.603460 ebtorch-0.9.5/ebtorch/nn/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/functional/inner_functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/kwta.py
--rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/laplacenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/mish.py
--rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/nnsemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/reshapelayers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/serf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/serlu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/sinlu.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/smelu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:07:19.603460 ebtorch-0.9.5/ebtorch/nn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/utils/adverutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/utils/autoclip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/utils/onlyutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/utils/patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/nn/utils/reprutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:07:19.607460 ebtorch-0.9.5/ebtorch/optim/
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/optim/adabound.py
--rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/optim/adahessian.py
--rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/optim/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)    20036 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/optim/autowu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/optim/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/optim/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/optim/lookahead.py
--rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/optim/lookaround.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/optim/radam.py
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-07-24 14:07:00.000000 ebtorch-0.9.5/ebtorch/optim/sam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:07:19.599460 ebtorch-0.9.5/ebtorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-24 14:07:19.000000 ebtorch-0.9.5/ebtorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-24 14:07:19.000000 ebtorch-0.9.5/ebtorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 14:07:19.000000 ebtorch-0.9.5/ebtorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 14:07:19.000000 ebtorch-0.9.5/ebtorch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 14:07:19.000000 ebtorch-0.9.5/ebtorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 14:07:19.607460 ebtorch-0.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-24 14:07:00.000000 ebtorch-0.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:52:09.246059 ebtorch-0.9.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-24 15:51:57.000000 ebtorch-0.9.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-24 15:52:09.246059 ebtorch-0.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-24 15:51:57.000000 ebtorch-0.9.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:52:09.230059 ebtorch-0.9.6/ebtorch/
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-24 15:51:57.000000 ebtorch-0.9.6/ebtorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:52:09.234058 ebtorch-0.9.6/ebtorch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-24 15:51:57.000000 ebtorch-0.9.6/ebtorch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16888 2023-07-24 15:51:57.000000 ebtorch-0.9.6/ebtorch/data/cutmixup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-07-24 15:51:57.000000 ebtorch-0.9.6/ebtorch/data/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:52:09.234058 ebtorch-0.9.6/ebtorch/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-24 15:51:57.000000 ebtorch-0.9.6/ebtorch/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-24 15:51:57.000000 ebtorch-0.9.6/ebtorch/logging/avgmeter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-24 15:51:57.000000 ebtorch-0.9.6/ebtorch/logging/logcsv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:52:09.238058 ebtorch-0.9.6/ebtorch/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-24 15:51:57.000000 ebtorch-0.9.6/ebtorch/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13998 2023-07-24 15:51:57.000000 ebtorch-0.9.6/ebtorch/nn/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-07-24 15:51:57.000000 ebtorch-0.9.6/ebtorch/nn/conv2drp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-24 15:51:57.000000 ebtorch-0.9.6/ebtorch/nn/convolutional_flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13699 2023-07-24 15:51:57.000000 ebtorch-0.9.6/ebtorch/nn/coordconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-24 15:51:57.000000 ebtorch-0.9.6/ebtorch/nn/debuglayers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-24 15:51:57.000000 ebtorch-0.9.6/ebtorch/nn/fieldtransform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:52:09.242059 ebtorch-0.9.6/ebtorch/nn/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-24 15:51:57.000000 ebtorch-0.9.6/ebtorch/nn/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-07-24 15:51:57.000000 ebtorch-0.9.6/ebtorch/nn/functional/inner_functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-07-24 15:51:57.000000 ebtorch-0.9.6/ebtorch/nn/kwta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-07-24 15:51:57.000000 ebtorch-0.9.6/ebtorch/nn/laplacenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-24 15:51:57.000000 ebtorch-0.9.6/ebtorch/nn/mish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-07-24 15:51:57.000000 ebtorch-0.9.6/ebtorch/nn/nnsemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-24 15:51:57.000000 ebtorch-0.9.6/ebtorch/nn/reshapelayers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-24 15:51:57.000000 ebtorch-0.9.6/ebtorch/nn/serf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-24 15:51:57.000000 ebtorch-0.9.6/ebtorch/nn/serlu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-24 15:51:57.000000 ebtorch-0.9.6/ebtorch/nn/sinlu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-24 15:51:57.000000 ebtorch-0.9.6/ebtorch/nn/smelu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:52:09.242059 ebtorch-0.9.6/ebtorch/nn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-24 15:51:57.000000 ebtorch-0.9.6/ebtorch/nn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-07-24 15:51:57.000000 ebtorch-0.9.6/ebtorch/nn/utils/adverutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-24 15:51:57.000000 ebtorch-0.9.6/ebtorch/nn/utils/autoclip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-24 15:51:57.000000 ebtorch-0.9.6/ebtorch/nn/utils/onlyutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-24 15:51:57.000000 ebtorch-0.9.6/ebtorch/nn/utils/patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-07-24 15:51:57.000000 ebtorch-0.9.6/ebtorch/nn/utils/reprutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:52:09.246059 ebtorch-0.9.6/ebtorch/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-24 15:51:57.000000 ebtorch-0.9.6/ebtorch/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-07-24 15:51:57.000000 ebtorch-0.9.6/ebtorch/optim/adabound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-07-24 15:51:57.000000 ebtorch-0.9.6/ebtorch/optim/adahessian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-07-24 15:51:57.000000 ebtorch-0.9.6/ebtorch/optim/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20036 2023-07-24 15:51:57.000000 ebtorch-0.9.6/ebtorch/optim/autowu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-07-24 15:51:57.000000 ebtorch-0.9.6/ebtorch/optim/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-24 15:51:57.000000 ebtorch-0.9.6/ebtorch/optim/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-07-24 15:51:57.000000 ebtorch-0.9.6/ebtorch/optim/lookahead.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-07-24 15:51:57.000000 ebtorch-0.9.6/ebtorch/optim/lookaround.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-24 15:51:57.000000 ebtorch-0.9.6/ebtorch/optim/radam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-07-24 15:51:57.000000 ebtorch-0.9.6/ebtorch/optim/sam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:52:09.234058 ebtorch-0.9.6/ebtorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-24 15:52:09.000000 ebtorch-0.9.6/ebtorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-24 15:52:09.000000 ebtorch-0.9.6/ebtorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 15:52:09.000000 ebtorch-0.9.6/ebtorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 15:52:09.000000 ebtorch-0.9.6/ebtorch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 15:52:09.000000 ebtorch-0.9.6/ebtorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 15:52:09.246059 ebtorch-0.9.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-24 15:51:57.000000 ebtorch-0.9.6/setup.py
```

### Comparing `ebtorch-0.9.5/LICENSE` & `ebtorch-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.5/PKG-INFO` & `ebtorch-0.9.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: ebtorch
-Version: 0.9.5
+Version: 0.9.6
 Summary: Collection of PyTorch additions, extensions, utilities, uses and abuses
 Home-page: https://github.com/emaballarin/ebtorch
 Author: Emanuele Ballarin
 Author-email: emanuele@ballarin.cc
 License: Apache-2.0
 Keywords: Deep Learning,Machine Learning
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: ebtorch Version: 0.9.5 Summary: Collection of
+Metadata-Version: 2.1 Name: ebtorch Version: 0.9.6 Summary: Collection of
 PyTorch additions, extensions, utilities, uses and abuses Home-page: https://
 github.com/emaballarin/ebtorch Author: Emanuele Ballarin Author-email:
 emanuele@ballarin.cc License: Apache-2.0 Keywords: Deep Learning,Machine
-Learning Classifier: Development Status :: 3 - Alpha Classifier: Topic ::
+Learning Classifier: Development Status :: 4 - Beta Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Environment ::
 Console Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: Apache Software License Requires-Python: >=3.8 Description-
 Content-Type: text/markdown License-File: LICENSE # :fire: `ebtorch` [https://
 ballarin.cc/cdn/ebtorch_dalle2.png] Collection of [PyTorch](https://
 pytorch.org/) additions, extensions, utilities, *uses and abuses*.
```

### Comparing `ebtorch-0.9.5/ebtorch/__init__.py` & `ebtorch-0.9.6/ebtorch/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,18 +17,28 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 # ==============================================================================
 #
 # SPDX-License-Identifier: Apache-2.0
 # Imports (wildcard)
+from .data import *
 from .logging import *
 from .nn import *
 from .optim import *
 
+# Deletions (from .data)
+del FastCollateMixup
+del Mixup
+del cifarhundred_dataloader_dispatcher
+del cifarten_dataloader_dispatcher
+del fashionmnist_dataloader_dispatcher
+del imagenette_dataloader_dispatcher
+del mnist_dataloader_dispatcher
+
 # Deletions (from .nn)
 del ArgMaxLayer
 del BatchNorm2dRP
 del BinarizeLayer
 del BrokenReLU
 del CausalConv1d
 del Conv2dRP
```

### Comparing `ebtorch-0.9.5/ebtorch/logging/__init__.py` & `ebtorch-0.9.6/ebtorch/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.5/ebtorch/logging/avgmeter.py` & `ebtorch-0.9.6/ebtorch/logging/avgmeter.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.5/ebtorch/logging/logcsv.py` & `ebtorch-0.9.6/ebtorch/logging/logcsv.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.5/ebtorch/nn/__init__.py` & `ebtorch-0.9.6/ebtorch/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.5/ebtorch/nn/architectures.py` & `ebtorch-0.9.6/ebtorch/nn/architectures.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.5/ebtorch/nn/conv2drp.py` & `ebtorch-0.9.6/ebtorch/nn/conv2drp.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.5/ebtorch/nn/convolutional_flatten.py` & `ebtorch-0.9.6/ebtorch/nn/convolutional_flatten.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.5/ebtorch/nn/coordconv.py` & `ebtorch-0.9.6/ebtorch/nn/coordconv.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.5/ebtorch/nn/debuglayers.py` & `ebtorch-0.9.6/ebtorch/nn/debuglayers.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.5/ebtorch/nn/fieldtransform.py` & `ebtorch-0.9.6/ebtorch/nn/fieldtransform.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.5/ebtorch/nn/functional/__init__.py` & `ebtorch-0.9.6/ebtorch/nn/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.5/ebtorch/nn/functional/inner_functional.py` & `ebtorch-0.9.6/ebtorch/nn/functional/inner_functional.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.5/ebtorch/nn/kwta.py` & `ebtorch-0.9.6/ebtorch/nn/kwta.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.5/ebtorch/nn/laplacenet.py` & `ebtorch-0.9.6/ebtorch/nn/laplacenet.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.5/ebtorch/nn/mish.py` & `ebtorch-0.9.6/ebtorch/nn/mish.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.5/ebtorch/nn/nnsemble.py` & `ebtorch-0.9.6/ebtorch/nn/nnsemble.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.5/ebtorch/nn/reshapelayers.py` & `ebtorch-0.9.6/ebtorch/nn/reshapelayers.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.5/ebtorch/nn/serf.py` & `ebtorch-0.9.6/ebtorch/nn/serf.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.5/ebtorch/nn/serlu.py` & `ebtorch-0.9.6/ebtorch/nn/serlu.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.5/ebtorch/nn/sinlu.py` & `ebtorch-0.9.6/ebtorch/nn/sinlu.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.5/ebtorch/nn/smelu.py` & `ebtorch-0.9.6/ebtorch/nn/smelu.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.5/ebtorch/nn/utils/__init__.py` & `ebtorch-0.9.6/ebtorch/nn/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.5/ebtorch/nn/utils/adverutils.py` & `ebtorch-0.9.6/ebtorch/nn/utils/adverutils.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.5/ebtorch/nn/utils/autoclip.py` & `ebtorch-0.9.6/ebtorch/nn/utils/autoclip.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.5/ebtorch/nn/utils/onlyutils.py` & `ebtorch-0.9.6/ebtorch/nn/utils/onlyutils.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.5/ebtorch/nn/utils/patches.py` & `ebtorch-0.9.6/ebtorch/nn/utils/patches.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.5/ebtorch/nn/utils/reprutils.py` & `ebtorch-0.9.6/ebtorch/nn/utils/reprutils.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.5/ebtorch/optim/__init__.py` & `ebtorch-0.9.6/ebtorch/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.5/ebtorch/optim/adabound.py` & `ebtorch-0.9.6/ebtorch/optim/adabound.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.5/ebtorch/optim/adahessian.py` & `ebtorch-0.9.6/ebtorch/optim/adahessian.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.5/ebtorch/optim/adan.py` & `ebtorch-0.9.6/ebtorch/optim/adan.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.5/ebtorch/optim/autowu.py` & `ebtorch-0.9.6/ebtorch/optim/autowu.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.5/ebtorch/optim/custom.py` & `ebtorch-0.9.6/ebtorch/optim/custom.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.5/ebtorch/optim/lion.py` & `ebtorch-0.9.6/ebtorch/optim/lion.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.5/ebtorch/optim/lookahead.py` & `ebtorch-0.9.6/ebtorch/optim/lookahead.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.5/ebtorch/optim/lookaround.py` & `ebtorch-0.9.6/ebtorch/optim/lookaround.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.5/ebtorch/optim/radam.py` & `ebtorch-0.9.6/ebtorch/optim/radam.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.5/ebtorch/optim/sam.py` & `ebtorch-0.9.6/ebtorch/optim/sam.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.5/ebtorch.egg-info/PKG-INFO` & `ebtorch-0.9.6/ebtorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: ebtorch
-Version: 0.9.5
+Version: 0.9.6
 Summary: Collection of PyTorch additions, extensions, utilities, uses and abuses
 Home-page: https://github.com/emaballarin/ebtorch
 Author: Emanuele Ballarin
 Author-email: emanuele@ballarin.cc
 License: Apache-2.0
 Keywords: Deep Learning,Machine Learning
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: ebtorch Version: 0.9.5 Summary: Collection of
+Metadata-Version: 2.1 Name: ebtorch Version: 0.9.6 Summary: Collection of
 PyTorch additions, extensions, utilities, uses and abuses Home-page: https://
 github.com/emaballarin/ebtorch Author: Emanuele Ballarin Author-email:
 emanuele@ballarin.cc License: Apache-2.0 Keywords: Deep Learning,Machine
-Learning Classifier: Development Status :: 3 - Alpha Classifier: Topic ::
+Learning Classifier: Development Status :: 4 - Beta Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Environment ::
 Console Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: Apache Software License Requires-Python: >=3.8 Description-
 Content-Type: text/markdown License-File: LICENSE # :fire: `ebtorch` [https://
 ballarin.cc/cdn/ebtorch_dalle2.png] Collection of [PyTorch](https://
 pytorch.org/) additions, extensions, utilities, *uses and abuses*.
```

### Comparing `ebtorch-0.9.5/ebtorch.egg-info/SOURCES.txt` & `ebtorch-0.9.6/ebtorch.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 setup.py
 ebtorch/__init__.py
 ebtorch.egg-info/PKG-INFO
 ebtorch.egg-info/SOURCES.txt
 ebtorch.egg-info/dependency_links.txt
 ebtorch.egg-info/not-zip-safe
 ebtorch.egg-info/top_level.txt
+ebtorch/data/__init__.py
+ebtorch/data/cutmixup.py
+ebtorch/data/datasets.py
 ebtorch/logging/__init__.py
 ebtorch/logging/avgmeter.py
 ebtorch/logging/logcsv.py
 ebtorch/nn/__init__.py
 ebtorch/nn/architectures.py
 ebtorch/nn/conv2drp.py
 ebtorch/nn/convolutional_flatten.py
```

### Comparing `ebtorch-0.9.5/setup.py` & `ebtorch-0.9.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,42 +34,44 @@
 
     if missing_dependencies:
         warnings.warn(f"Missing dependencies: {missing_dependencies}")
 
 
 DEPENDENCY_PACKAGE_NAMES: list[str] = [
     "advertorch",
+    "gpytorch",
     "numpy",
     "requests",
     "torch",
     "torchattacks",
+    "torchvision",
     "tqdm",
 ]
 
 check_dependencies(DEPENDENCY_PACKAGE_NAMES)
 
 PACKAGENAME: str = "ebtorch"
 
 
 setup(
     name=PACKAGENAME,
-    version="0.9.5",
+    version="0.9.6",
     author="Emanuele Ballarin",
     author_email="emanuele@ballarin.cc",
     url="https://github.com/emaballarin/ebtorch",
     description="Collection of PyTorch additions, extensions, utilities, uses and abuses",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     keywords=["Deep Learning", "Machine Learning"],
     license="Apache-2.0",
     packages=[
         package for package in find_packages() if package.startswith(PACKAGENAME)
     ],
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 4 - Beta",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Environment :: Console",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
     ],
     python_requires=">=3.8",
     include_package_data=True,
```

