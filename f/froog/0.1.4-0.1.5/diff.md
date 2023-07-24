# Comparing `tmp/froog-0.1.4.tar.gz` & `tmp/froog-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "froog-0.1.4.tar", last modified: Mon Jul 24 01:16:57 2023, max compression
+gzip compressed data, was "froog-0.1.5.tar", last modified: Mon Jul 24 01:54:39 2023, max compression
```

## Comparing `froog-0.1.4.tar` & `froog-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-07-24 01:16:57.289485 froog-0.1.4/
--rw-r--r--   0 kevinbuhler   (501) staff       (20)       31 2023-07-16 20:10:22.000000 froog-0.1.4/LICENSE
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2324 2023-07-24 01:16:57.289394 froog-0.1.4/PKG-INFO
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     1999 2023-07-24 01:05:12.000000 froog-0.1.4/README.md
-drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-07-24 01:16:57.288530 froog-0.1.4/frog/
--rw-r--r--   0 kevinbuhler   (501) staff       (20)       54 2023-07-24 00:15:18.000000 froog-0.1.4/frog/__init__.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2103 2023-07-19 07:06:24.000000 froog-0.1.4/frog/gradcheck.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)    10298 2023-07-24 00:13:42.000000 froog-0.1.4/frog/ops.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2016 2023-07-19 05:23:59.000000 froog-0.1.4/frog/optim.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     3802 2023-07-24 00:17:09.000000 froog-0.1.4/frog/tensor.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2685 2023-07-23 19:46:48.000000 froog-0.1.4/frog/utils.py
-drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-07-24 01:16:57.289221 froog-0.1.4/froog.egg-info/
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2324 2023-07-24 01:16:57.000000 froog-0.1.4/froog.egg-info/PKG-INFO
--rw-r--r--   0 kevinbuhler   (501) staff       (20)      260 2023-07-24 01:16:57.000000 froog-0.1.4/froog.egg-info/SOURCES.txt
--rw-r--r--   0 kevinbuhler   (501) staff       (20)        1 2023-07-24 01:16:57.000000 froog-0.1.4/froog.egg-info/dependency_links.txt
--rw-r--r--   0 kevinbuhler   (501) staff       (20)       15 2023-07-24 01:16:57.000000 froog-0.1.4/froog.egg-info/requires.txt
--rw-r--r--   0 kevinbuhler   (501) staff       (20)        5 2023-07-24 01:16:57.000000 froog-0.1.4/froog.egg-info/top_level.txt
--rw-r--r--   0 kevinbuhler   (501) staff       (20)       38 2023-07-24 01:16:57.289526 froog-0.1.4/setup.cfg
--rw-r--r--   0 kevinbuhler   (501) staff       (20)      849 2023-07-24 01:16:44.000000 froog-0.1.4/setup.py
+drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-07-24 01:54:39.665607 froog-0.1.5/
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)       31 2023-07-16 20:10:22.000000 froog-0.1.5/LICENSE
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2415 2023-07-24 01:54:39.665493 froog-0.1.5/PKG-INFO
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2090 2023-07-24 01:53:24.000000 froog-0.1.5/README.md
+drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-07-24 01:54:39.664582 froog-0.1.5/frog/
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)       54 2023-07-24 00:15:18.000000 froog-0.1.5/frog/__init__.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2103 2023-07-19 07:06:24.000000 froog-0.1.5/frog/gradcheck.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)    10298 2023-07-24 00:13:42.000000 froog-0.1.5/frog/ops.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2016 2023-07-19 05:23:59.000000 froog-0.1.5/frog/optim.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     3802 2023-07-24 00:17:09.000000 froog-0.1.5/frog/tensor.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2685 2023-07-23 19:46:48.000000 froog-0.1.5/frog/utils.py
+drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-07-24 01:54:39.665283 froog-0.1.5/froog.egg-info/
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2415 2023-07-24 01:54:39.000000 froog-0.1.5/froog.egg-info/PKG-INFO
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)      260 2023-07-24 01:54:39.000000 froog-0.1.5/froog.egg-info/SOURCES.txt
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)        1 2023-07-24 01:54:39.000000 froog-0.1.5/froog.egg-info/dependency_links.txt
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)       15 2023-07-24 01:54:39.000000 froog-0.1.5/froog.egg-info/requires.txt
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)        5 2023-07-24 01:54:39.000000 froog-0.1.5/froog.egg-info/top_level.txt
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)       38 2023-07-24 01:54:39.665640 froog-0.1.5/setup.cfg
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)      849 2023-07-24 01:54:07.000000 froog-0.1.5/setup.py
```

### Comparing `froog-0.1.4/PKG-INFO` & `froog-0.1.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: froog
-Version: 0.1.4
+Version: 0.1.5
 Summary: FROG: Fast Real-time Optimization of Gradients
 Author: Kevin Buhler
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -14,15 +14,15 @@
 <div align="center" >
   <img src="https://raw.githubusercontent.com/kevbuh/frog/main/assets/froog.jpeg" alt="froog the frog" height="300">
   <br/>
   frog: fast real-time optimization of gradients 
   <br/>
   a beautifully compact machine-learning library
   <br/>
-  <a href="https://github.com/kevbuh/frog">homepage</a> | <a href="https://github.com/kevbuh/frog/tree/main/docs">documentation</a> | <a href="https://github.com/kevbuh/frog/tree/main/examples">examples</a>| <a href="https://pypi.org/project/froog/">pip</a>
+  <a href="https://github.com/kevbuh/frog">homepage</a> | <a href="https://github.com/kevbuh/frog/tree/main/docs">documentation</a> | <a href="https://github.com/kevbuh/frog/tree/main/examples">examples</a> | <a href="https://pypi.org/project/froog/">pip</a>
   <br/>
   <br/>
 </div>
 
 <!-- modern ml development is unintuitive, time consuming, and unaccessible. why not make it possible for anyone to build? -->
 # Installation
 ```bash
@@ -32,51 +32,48 @@
 ### Overview of Features
 - Tensors
 - Automatic Differentiation
     - Forward and backward passes
 - Input/gradient shape-tracking
 - MNIST example
 - 2D Convolutions (im2col)
-- Gradient checking
+- Numerical gradient checking
 - The most common optimizers (SGD, Adam, RMSProp)
 
 ### Math Operations
 - Scalar-Matrix Multiplication
 - Dot Product
 - Sum
 - ReLU
 - Log Softmax
-- 2D Convolution
+- 2D Convolutions
+- Avg & Max pooling
+- <a href="https://github.com/kevbuh/frog/blob/main/frog/ops.py">More</a> 
 
 # Bounties
-We really want to get a useful model working right out of the box! Our top bounty is to get EfficientNet v2 model working inside of the <a href="https://github.com/kevbuh/frog/tree/main/examples">examples</a>  folder.
+Want to help but don't know where to start? 
 
-- EfficientNet v2 (**top priority**)
+Our top bounty is to get EfficientNet v2 model working inside of the <a href="https://github.com/kevbuh/frog/tree/main/examples">examples</a> folder.
 
 #### Easy
 - built in MLP model
 - binary cross entropy
 - dropout layer
 - flatten
-
 #### Medium
 - simplify how context and gradients are handled
-
 #### Hard
-- Transformers
-- Stable Diffusion
-- Winograd Convs
+- efficientNet
+- transformers
+- stable Diffusion
+- winograd Convs
 - MPS support
 - CUDA support
 
 # Contributing
+here are some basic guidelines for contributing:
+* reduce complexity (currently at 585 lines of code)
+* increase speed
+* add features, must include <a href="https://github.com/kevbuh/frog/tree/main/tests">tests</a>
+* in that order
 
-Here are some basic guidelines for contributing:
-
-* Reduce code, currently at 585 lines
-* Increase speed
-* Add features
-* In that order
-
-Bug fixes are the best and always welcome
-Conceptual cleanups are great
-All features must include <a href="https://github.com/kevbuh/frog/tree/main/tests">tests</a>
+more info on <a href="https://github.com/kevbuh/frog/blob/main/docs/contributing.md">contributing</a>
```

#### html2text {}

```diff
@@ -1,25 +1,24 @@
-Metadata-Version: 2.1 Name: froog Version: 0.1.4 Summary: FROG: Fast Real-time
+Metadata-Version: 2.1 Name: froog Version: 0.1.5 Summary: FROG: Fast Real-time
 Optimization of Gradients Author: Kevin Buhler License: MIT Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Requires-Python: >=3.6 Description-Content-Type: text/markdown License-
 File: LICENSE # frog [unit test badge]
                                [froog the frog]
                 frog: fast real-time optimization of gradients
                 a beautifully compact machine-learning library
-                   homepage | documentation | examples| pip
+                  homepage | documentation | examples | pip
 
  # Installation ```bash pip install froog ``` ### Overview of Features -
 Tensors - Automatic Differentiation - Forward and backward passes - Input/
-gradient shape-tracking - MNIST example - 2D Convolutions (im2col) - Gradient
-checking - The most common optimizers (SGD, Adam, RMSProp) ### Math Operations
-- Scalar-Matrix Multiplication - Dot Product - Sum - ReLU - Log Softmax - 2D
-Convolution # Bounties We really want to get a useful model working right out
-of the box! Our top bounty is to get EfficientNet v2 model working inside of
-the examples folder. - EfficientNet v2 (**top priority**) #### Easy - built in
-MLP model - binary cross entropy - dropout layer - flatten #### Medium -
-simplify how context and gradients are handled #### Hard - Transformers -
-Stable Diffusion - Winograd Convs - MPS support - CUDA support # Contributing
-Here are some basic guidelines for contributing: * Reduce code, currently at
-585 lines * Increase speed * Add features * In that order Bug fixes are the
-best and always welcome Conceptual cleanups are great All features must include
-tests
+gradient shape-tracking - MNIST example - 2D Convolutions (im2col) - Numerical
+gradient checking - The most common optimizers (SGD, Adam, RMSProp) ### Math
+Operations - Scalar-Matrix Multiplication - Dot Product - Sum - ReLU - Log
+Softmax - 2D Convolutions - Avg & Max pooling - More # Bounties Want to help
+but don't know where to start? Our top bounty is to get EfficientNet v2 model
+working inside of the examples folder. #### Easy - built in MLP model - binary
+cross entropy - dropout layer - flatten #### Medium - simplify how context and
+gradients are handled #### Hard - efficientNet - transformers - stable
+Diffusion - winograd Convs - MPS support - CUDA support # Contributing here are
+some basic guidelines for contributing: * reduce complexity (currently at 585
+lines of code) * increase speed * add features, must include tests * in that
+order more info on contributing
```

### Comparing `froog-0.1.4/README.md` & `froog-0.1.5/froog.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,28 @@
+Metadata-Version: 2.1
+Name: froog
+Version: 0.1.5
+Summary: FROG: Fast Real-time Optimization of Gradients
+Author: Kevin Buhler
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # frog <img src="https://github.com/kevbuh/frog/actions/workflows/test.yml/badge.svg" alt="unit test badge" >
 <div align="center" >
   <img src="https://raw.githubusercontent.com/kevbuh/frog/main/assets/froog.jpeg" alt="froog the frog" height="300">
   <br/>
   frog: fast real-time optimization of gradients 
   <br/>
   a beautifully compact machine-learning library
   <br/>
-  <a href="https://github.com/kevbuh/frog">homepage</a> | <a href="https://github.com/kevbuh/frog/tree/main/docs">documentation</a> | <a href="https://github.com/kevbuh/frog/tree/main/examples">examples</a>| <a href="https://pypi.org/project/froog/">pip</a>
+  <a href="https://github.com/kevbuh/frog">homepage</a> | <a href="https://github.com/kevbuh/frog/tree/main/docs">documentation</a> | <a href="https://github.com/kevbuh/frog/tree/main/examples">examples</a> | <a href="https://pypi.org/project/froog/">pip</a>
   <br/>
   <br/>
 </div>
 
 <!-- modern ml development is unintuitive, time consuming, and unaccessible. why not make it possible for anyone to build? -->
 # Installation
 ```bash
@@ -20,51 +32,48 @@
 ### Overview of Features
 - Tensors
 - Automatic Differentiation
     - Forward and backward passes
 - Input/gradient shape-tracking
 - MNIST example
 - 2D Convolutions (im2col)
-- Gradient checking
+- Numerical gradient checking
 - The most common optimizers (SGD, Adam, RMSProp)
 
 ### Math Operations
 - Scalar-Matrix Multiplication
 - Dot Product
 - Sum
 - ReLU
 - Log Softmax
-- 2D Convolution
+- 2D Convolutions
+- Avg & Max pooling
+- <a href="https://github.com/kevbuh/frog/blob/main/frog/ops.py">More</a> 
 
 # Bounties
-We really want to get a useful model working right out of the box! Our top bounty is to get EfficientNet v2 model working inside of the <a href="https://github.com/kevbuh/frog/tree/main/examples">examples</a>  folder.
+Want to help but don't know where to start? 
 
-- EfficientNet v2 (**top priority**)
+Our top bounty is to get EfficientNet v2 model working inside of the <a href="https://github.com/kevbuh/frog/tree/main/examples">examples</a> folder.
 
 #### Easy
 - built in MLP model
 - binary cross entropy
 - dropout layer
 - flatten
-
 #### Medium
 - simplify how context and gradients are handled
-
 #### Hard
-- Transformers
-- Stable Diffusion
-- Winograd Convs
+- efficientNet
+- transformers
+- stable Diffusion
+- winograd Convs
 - MPS support
 - CUDA support
 
 # Contributing
+here are some basic guidelines for contributing:
+* reduce complexity (currently at 585 lines of code)
+* increase speed
+* add features, must include <a href="https://github.com/kevbuh/frog/tree/main/tests">tests</a>
+* in that order
 
-Here are some basic guidelines for contributing:
-
-* Reduce code, currently at 585 lines
-* Increase speed
-* Add features
-* In that order
-
-Bug fixes are the best and always welcome
-Conceptual cleanups are great
-All features must include <a href="https://github.com/kevbuh/frog/tree/main/tests">tests</a>
+more info on <a href="https://github.com/kevbuh/frog/blob/main/docs/contributing.md">contributing</a>
```

#### html2text {}

```diff
@@ -1,21 +1,24 @@
-# frog [unit test badge]
+Metadata-Version: 2.1 Name: froog Version: 0.1.5 Summary: FROG: Fast Real-time
+Optimization of Gradients Author: Kevin Buhler License: MIT Classifier:
+Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
+License Requires-Python: >=3.6 Description-Content-Type: text/markdown License-
+File: LICENSE # frog [unit test badge]
                                [froog the frog]
                 frog: fast real-time optimization of gradients
                 a beautifully compact machine-learning library
-                   homepage | documentation | examples| pip
+                  homepage | documentation | examples | pip
 
  # Installation ```bash pip install froog ``` ### Overview of Features -
 Tensors - Automatic Differentiation - Forward and backward passes - Input/
-gradient shape-tracking - MNIST example - 2D Convolutions (im2col) - Gradient
-checking - The most common optimizers (SGD, Adam, RMSProp) ### Math Operations
-- Scalar-Matrix Multiplication - Dot Product - Sum - ReLU - Log Softmax - 2D
-Convolution # Bounties We really want to get a useful model working right out
-of the box! Our top bounty is to get EfficientNet v2 model working inside of
-the examples folder. - EfficientNet v2 (**top priority**) #### Easy - built in
-MLP model - binary cross entropy - dropout layer - flatten #### Medium -
-simplify how context and gradients are handled #### Hard - Transformers -
-Stable Diffusion - Winograd Convs - MPS support - CUDA support # Contributing
-Here are some basic guidelines for contributing: * Reduce code, currently at
-585 lines * Increase speed * Add features * In that order Bug fixes are the
-best and always welcome Conceptual cleanups are great All features must include
-tests
+gradient shape-tracking - MNIST example - 2D Convolutions (im2col) - Numerical
+gradient checking - The most common optimizers (SGD, Adam, RMSProp) ### Math
+Operations - Scalar-Matrix Multiplication - Dot Product - Sum - ReLU - Log
+Softmax - 2D Convolutions - Avg & Max pooling - More # Bounties Want to help
+but don't know where to start? Our top bounty is to get EfficientNet v2 model
+working inside of the examples folder. #### Easy - built in MLP model - binary
+cross entropy - dropout layer - flatten #### Medium - simplify how context and
+gradients are handled #### Hard - efficientNet - transformers - stable
+Diffusion - winograd Convs - MPS support - CUDA support # Contributing here are
+some basic guidelines for contributing: * reduce complexity (currently at 585
+lines of code) * increase speed * add features, must include tests * in that
+order more info on contributing
```

### Comparing `froog-0.1.4/frog/gradcheck.py` & `froog-0.1.5/frog/gradcheck.py`

 * *Files identical despite different names*

### Comparing `froog-0.1.4/frog/ops.py` & `froog-0.1.5/frog/ops.py`

 * *Files identical despite different names*

### Comparing `froog-0.1.4/frog/optim.py` & `froog-0.1.5/frog/optim.py`

 * *Files identical despite different names*

### Comparing `froog-0.1.4/frog/tensor.py` & `froog-0.1.5/frog/tensor.py`

 * *Files identical despite different names*

### Comparing `froog-0.1.4/frog/utils.py` & `froog-0.1.5/frog/utils.py`

 * *Files identical despite different names*

### Comparing `froog-0.1.4/setup.py` & `froog-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(directory, 'README.md'), encoding='utf-8') as f:
   long_description = f.read()
 
 setup(name='froog',
-      version='0.1.4',
+      version='0.1.5',
       description='FROG: Fast Real-time Optimization of Gradients',
       author='Kevin Buhler',
       license='MIT',
       long_description=long_description,
       long_description_content_type='text/markdown',
       packages = ['frog'],
       classifiers=[
```

