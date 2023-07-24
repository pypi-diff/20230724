# Comparing `tmp/froog-0.1.2.tar.gz` & `tmp/froog-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "froog-0.1.2.tar", last modified: Mon Jul 24 00:42:12 2023, max compression
+gzip compressed data, was "froog-0.1.3.tar", last modified: Mon Jul 24 00:49:29 2023, max compression
```

## Comparing `froog-0.1.2.tar` & `froog-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-07-24 00:42:12.346875 froog-0.1.2/
--rw-r--r--   0 kevinbuhler   (501) staff       (20)       31 2023-07-16 20:10:22.000000 froog-0.1.2/LICENSE
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2144 2023-07-24 00:42:12.346780 froog-0.1.2/PKG-INFO
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     1819 2023-07-24 00:21:57.000000 froog-0.1.2/README.md
-drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-07-24 00:42:12.345956 froog-0.1.2/frog/
--rw-r--r--   0 kevinbuhler   (501) staff       (20)       54 2023-07-24 00:15:18.000000 froog-0.1.2/frog/__init__.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2103 2023-07-19 07:06:24.000000 froog-0.1.2/frog/gradcheck.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)    10298 2023-07-24 00:13:42.000000 froog-0.1.2/frog/ops.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2016 2023-07-19 05:23:59.000000 froog-0.1.2/frog/optim.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     3802 2023-07-24 00:17:09.000000 froog-0.1.2/frog/tensor.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2685 2023-07-23 19:46:48.000000 froog-0.1.2/frog/utils.py
-drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-07-24 00:42:12.346650 froog-0.1.2/froog.egg-info/
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2144 2023-07-24 00:42:12.000000 froog-0.1.2/froog.egg-info/PKG-INFO
--rw-r--r--   0 kevinbuhler   (501) staff       (20)      260 2023-07-24 00:42:12.000000 froog-0.1.2/froog.egg-info/SOURCES.txt
--rw-r--r--   0 kevinbuhler   (501) staff       (20)        1 2023-07-24 00:42:12.000000 froog-0.1.2/froog.egg-info/dependency_links.txt
--rw-r--r--   0 kevinbuhler   (501) staff       (20)       15 2023-07-24 00:42:12.000000 froog-0.1.2/froog.egg-info/requires.txt
--rw-r--r--   0 kevinbuhler   (501) staff       (20)        5 2023-07-24 00:42:12.000000 froog-0.1.2/froog.egg-info/top_level.txt
--rw-r--r--   0 kevinbuhler   (501) staff       (20)       38 2023-07-24 00:42:12.346905 froog-0.1.2/setup.cfg
--rw-r--r--   0 kevinbuhler   (501) staff       (20)      849 2023-07-24 00:40:22.000000 froog-0.1.2/setup.py
+drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-07-24 00:49:29.064152 froog-0.1.3/
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)       31 2023-07-16 20:10:22.000000 froog-0.1.3/LICENSE
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2370 2023-07-24 00:49:29.064060 froog-0.1.3/PKG-INFO
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2045 2023-07-24 00:47:04.000000 froog-0.1.3/README.md
+drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-07-24 00:49:29.063186 froog-0.1.3/frog/
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)       54 2023-07-24 00:15:18.000000 froog-0.1.3/frog/__init__.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2103 2023-07-19 07:06:24.000000 froog-0.1.3/frog/gradcheck.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)    10298 2023-07-24 00:13:42.000000 froog-0.1.3/frog/ops.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2016 2023-07-19 05:23:59.000000 froog-0.1.3/frog/optim.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     3802 2023-07-24 00:17:09.000000 froog-0.1.3/frog/tensor.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2685 2023-07-23 19:46:48.000000 froog-0.1.3/frog/utils.py
+drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-07-24 00:49:29.063862 froog-0.1.3/froog.egg-info/
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2370 2023-07-24 00:49:29.000000 froog-0.1.3/froog.egg-info/PKG-INFO
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)      260 2023-07-24 00:49:29.000000 froog-0.1.3/froog.egg-info/SOURCES.txt
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)        1 2023-07-24 00:49:29.000000 froog-0.1.3/froog.egg-info/dependency_links.txt
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)       15 2023-07-24 00:49:29.000000 froog-0.1.3/froog.egg-info/requires.txt
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)        5 2023-07-24 00:49:29.000000 froog-0.1.3/froog.egg-info/top_level.txt
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)       38 2023-07-24 00:49:29.064188 froog-0.1.3/setup.cfg
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)      849 2023-07-24 00:46:33.000000 froog-0.1.3/setup.py
```

### Comparing `froog-0.1.2/PKG-INFO` & `froog-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 Metadata-Version: 2.1
 Name: froog
-Version: 0.1.2
+Version: 0.1.3
 Summary: FROG: Fast Real-time Optimization of Gradients
 Author: Kevin Buhler
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # frog <img src="https://github.com/kevbuh/frog/actions/workflows/test.yml/badge.svg" alt="unit test badge" >
 <div align="center" >
-  <img src="https://github.com/kevbuh/frog/blob/main/assets/froog.jpeg" alt="froog the frog" height="300">
+  <img src="https://raw.githubusercontent.com/kevbuh/frog/main/assets/froog.jpeg" alt="froog the frog" height="300">
   
   <br/>
   frog: fast real-time optimization of gradients 
   <br/>
-  <a href="https://github.com/kevbuh/frog/tree/main/docs">documentation</a> | <a href="https://github.com/kevbuh/frog/tree/main/examples">examples</a> 
+  <a href="https://github.com/kevbuh/frog/tree/main/docs">documentation</a> | <a href="https://github.com/kevbuh/frog/tree/main/examples">examples</a> | <a href="https://github.com/kevbuh/frog/tree/main/docs">documentation</a> | <a href="https://pypi.org/project/froog/">pypi</a> | <a href="https://github.com/kevbuh/frog">github</a>
   <br/>
   <br/>
 </div>
 
 a beautifully compact machine-learning library
 
-modern ml development is unintuitive, time consuming, and unaccessible. why not make it possible for anyone to build?
-
+<!-- modern ml development is unintuitive, time consuming, and unaccessible. why not make it possible for anyone to build? -->
+# Installation
+```bash
+pip install froog
+```
 
 ### Overview of Features
 - Tensors
 - Automatic Differentiation
     - Forward and backward passes
 - Input/gradient shape-tracking
 - MNIST example
@@ -42,27 +45,25 @@
 - Dot Product
 - Sum
 - ReLU
 - Log Softmax
 - 2D Convolution
 
 # Bounties
-
 We really want to get a useful model working right out of the box! Our top bounty is to get EfficientNet v2 model working inside of the <a href="https://github.com/kevbuh/frog/tree/main/examples">examples</a>  folder.
 
 - EfficientNet v2 (**top priority**)
 
 #### Easy
 - built in MLP model
 - binary cross entropy
 - dropout layer
 - flatten
 
 #### Medium
-- publish to pip3
 - simplify how context and gradients are handled
 
 #### Hard
 - Transformers
 - Stable Diffusion
 - Winograd Convs
 - MPS support
```

#### html2text {}

```diff
@@ -1,25 +1,24 @@
-Metadata-Version: 2.1 Name: froog Version: 0.1.2 Summary: FROG: Fast Real-time
+Metadata-Version: 2.1 Name: froog Version: 0.1.3 Summary: FROG: Fast Real-time
 Optimization of Gradients Author: Kevin Buhler License: MIT Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Requires-Python: >=3.6 Description-Content-Type: text/markdown License-
 File: LICENSE # frog [unit test badge]
                                [froog the frog]
                 frog: fast real-time optimization of gradients
-                           documentation | examples
+           documentation | examples | documentation | pypi | github
 
-a beautifully compact machine-learning library modern ml development is
-unintuitive, time consuming, and unaccessible. why not make it possible for
-anyone to build? ### Overview of Features - Tensors - Automatic Differentiation
-- Forward and backward passes - Input/gradient shape-tracking - MNIST example -
-2D Convolutions (im2col) - Gradient checking - The most common optimizers (SGD,
-Adam, RMSProp) ### Math Operations - Scalar-Matrix Multiplication - Dot Product
-- Sum - ReLU - Log Softmax - 2D Convolution # Bounties We really want to get a
-useful model working right out of the box! Our top bounty is to get
-EfficientNet v2 model working inside of the examples folder. - EfficientNet v2
-(**top priority**) #### Easy - built in MLP model - binary cross entropy -
-dropout layer - flatten #### Medium - publish to pip3 - simplify how context
-and gradients are handled #### Hard - Transformers - Stable Diffusion -
+a beautifully compact machine-learning library  # Installation ```bash pip
+install froog ``` ### Overview of Features - Tensors - Automatic
+Differentiation - Forward and backward passes - Input/gradient shape-tracking -
+MNIST example - 2D Convolutions (im2col) - Gradient checking - The most common
+optimizers (SGD, Adam, RMSProp) ### Math Operations - Scalar-Matrix
+Multiplication - Dot Product - Sum - ReLU - Log Softmax - 2D Convolution #
+Bounties We really want to get a useful model working right out of the box! Our
+top bounty is to get EfficientNet v2 model working inside of the examples
+folder. - EfficientNet v2 (**top priority**) #### Easy - built in MLP model -
+binary cross entropy - dropout layer - flatten #### Medium - simplify how
+context and gradients are handled #### Hard - Transformers - Stable Diffusion -
 Winograd Convs - MPS support - CUDA support # Contributing Here are some basic
 guidelines for contributing: * Reduce code * Increase speed * Add features * In
 that order Bug fixes are the best and always welcome Conceptual cleanups are
 great All features must include tests
```

### Comparing `froog-0.1.2/README.md` & `froog-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 # frog <img src="https://github.com/kevbuh/frog/actions/workflows/test.yml/badge.svg" alt="unit test badge" >
 <div align="center" >
-  <img src="https://github.com/kevbuh/frog/blob/main/assets/froog.jpeg" alt="froog the frog" height="300">
+  <img src="https://raw.githubusercontent.com/kevbuh/frog/main/assets/froog.jpeg" alt="froog the frog" height="300">
   
   <br/>
   frog: fast real-time optimization of gradients 
   <br/>
-  <a href="https://github.com/kevbuh/frog/tree/main/docs">documentation</a> | <a href="https://github.com/kevbuh/frog/tree/main/examples">examples</a> 
+  <a href="https://github.com/kevbuh/frog/tree/main/docs">documentation</a> | <a href="https://github.com/kevbuh/frog/tree/main/examples">examples</a> | <a href="https://github.com/kevbuh/frog/tree/main/docs">documentation</a> | <a href="https://pypi.org/project/froog/">pypi</a> | <a href="https://github.com/kevbuh/frog">github</a>
   <br/>
   <br/>
 </div>
 
 a beautifully compact machine-learning library
 
-modern ml development is unintuitive, time consuming, and unaccessible. why not make it possible for anyone to build?
-
+<!-- modern ml development is unintuitive, time consuming, and unaccessible. why not make it possible for anyone to build? -->
+# Installation
+```bash
+pip install froog
+```
 
 ### Overview of Features
 - Tensors
 - Automatic Differentiation
     - Forward and backward passes
 - Input/gradient shape-tracking
 - MNIST example
@@ -30,27 +33,25 @@
 - Dot Product
 - Sum
 - ReLU
 - Log Softmax
 - 2D Convolution
 
 # Bounties
-
 We really want to get a useful model working right out of the box! Our top bounty is to get EfficientNet v2 model working inside of the <a href="https://github.com/kevbuh/frog/tree/main/examples">examples</a>  folder.
 
 - EfficientNet v2 (**top priority**)
 
 #### Easy
 - built in MLP model
 - binary cross entropy
 - dropout layer
 - flatten
 
 #### Medium
-- publish to pip3
 - simplify how context and gradients are handled
 
 #### Hard
 - Transformers
 - Stable Diffusion
 - Winograd Convs
 - MPS support
```

#### html2text {}

```diff
@@ -1,21 +1,20 @@
 # frog [unit test badge]
                                [froog the frog]
                 frog: fast real-time optimization of gradients
-                           documentation | examples
+           documentation | examples | documentation | pypi | github
 
-a beautifully compact machine-learning library modern ml development is
-unintuitive, time consuming, and unaccessible. why not make it possible for
-anyone to build? ### Overview of Features - Tensors - Automatic Differentiation
-- Forward and backward passes - Input/gradient shape-tracking - MNIST example -
-2D Convolutions (im2col) - Gradient checking - The most common optimizers (SGD,
-Adam, RMSProp) ### Math Operations - Scalar-Matrix Multiplication - Dot Product
-- Sum - ReLU - Log Softmax - 2D Convolution # Bounties We really want to get a
-useful model working right out of the box! Our top bounty is to get
-EfficientNet v2 model working inside of the examples folder. - EfficientNet v2
-(**top priority**) #### Easy - built in MLP model - binary cross entropy -
-dropout layer - flatten #### Medium - publish to pip3 - simplify how context
-and gradients are handled #### Hard - Transformers - Stable Diffusion -
+a beautifully compact machine-learning library  # Installation ```bash pip
+install froog ``` ### Overview of Features - Tensors - Automatic
+Differentiation - Forward and backward passes - Input/gradient shape-tracking -
+MNIST example - 2D Convolutions (im2col) - Gradient checking - The most common
+optimizers (SGD, Adam, RMSProp) ### Math Operations - Scalar-Matrix
+Multiplication - Dot Product - Sum - ReLU - Log Softmax - 2D Convolution #
+Bounties We really want to get a useful model working right out of the box! Our
+top bounty is to get EfficientNet v2 model working inside of the examples
+folder. - EfficientNet v2 (**top priority**) #### Easy - built in MLP model -
+binary cross entropy - dropout layer - flatten #### Medium - simplify how
+context and gradients are handled #### Hard - Transformers - Stable Diffusion -
 Winograd Convs - MPS support - CUDA support # Contributing Here are some basic
 guidelines for contributing: * Reduce code * Increase speed * Add features * In
 that order Bug fixes are the best and always welcome Conceptual cleanups are
 great All features must include tests
```

### Comparing `froog-0.1.2/frog/gradcheck.py` & `froog-0.1.3/frog/gradcheck.py`

 * *Files identical despite different names*

### Comparing `froog-0.1.2/frog/ops.py` & `froog-0.1.3/frog/ops.py`

 * *Files identical despite different names*

### Comparing `froog-0.1.2/frog/optim.py` & `froog-0.1.3/frog/optim.py`

 * *Files identical despite different names*

### Comparing `froog-0.1.2/frog/tensor.py` & `froog-0.1.3/frog/tensor.py`

 * *Files identical despite different names*

### Comparing `froog-0.1.2/frog/utils.py` & `froog-0.1.3/frog/utils.py`

 * *Files identical despite different names*

### Comparing `froog-0.1.2/froog.egg-info/PKG-INFO` & `froog-0.1.3/froog.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 Metadata-Version: 2.1
 Name: froog
-Version: 0.1.2
+Version: 0.1.3
 Summary: FROG: Fast Real-time Optimization of Gradients
 Author: Kevin Buhler
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # frog <img src="https://github.com/kevbuh/frog/actions/workflows/test.yml/badge.svg" alt="unit test badge" >
 <div align="center" >
-  <img src="https://github.com/kevbuh/frog/blob/main/assets/froog.jpeg" alt="froog the frog" height="300">
+  <img src="https://raw.githubusercontent.com/kevbuh/frog/main/assets/froog.jpeg" alt="froog the frog" height="300">
   
   <br/>
   frog: fast real-time optimization of gradients 
   <br/>
-  <a href="https://github.com/kevbuh/frog/tree/main/docs">documentation</a> | <a href="https://github.com/kevbuh/frog/tree/main/examples">examples</a> 
+  <a href="https://github.com/kevbuh/frog/tree/main/docs">documentation</a> | <a href="https://github.com/kevbuh/frog/tree/main/examples">examples</a> | <a href="https://github.com/kevbuh/frog/tree/main/docs">documentation</a> | <a href="https://pypi.org/project/froog/">pypi</a> | <a href="https://github.com/kevbuh/frog">github</a>
   <br/>
   <br/>
 </div>
 
 a beautifully compact machine-learning library
 
-modern ml development is unintuitive, time consuming, and unaccessible. why not make it possible for anyone to build?
-
+<!-- modern ml development is unintuitive, time consuming, and unaccessible. why not make it possible for anyone to build? -->
+# Installation
+```bash
+pip install froog
+```
 
 ### Overview of Features
 - Tensors
 - Automatic Differentiation
     - Forward and backward passes
 - Input/gradient shape-tracking
 - MNIST example
@@ -42,27 +45,25 @@
 - Dot Product
 - Sum
 - ReLU
 - Log Softmax
 - 2D Convolution
 
 # Bounties
-
 We really want to get a useful model working right out of the box! Our top bounty is to get EfficientNet v2 model working inside of the <a href="https://github.com/kevbuh/frog/tree/main/examples">examples</a>  folder.
 
 - EfficientNet v2 (**top priority**)
 
 #### Easy
 - built in MLP model
 - binary cross entropy
 - dropout layer
 - flatten
 
 #### Medium
-- publish to pip3
 - simplify how context and gradients are handled
 
 #### Hard
 - Transformers
 - Stable Diffusion
 - Winograd Convs
 - MPS support
```

#### html2text {}

```diff
@@ -1,25 +1,24 @@
-Metadata-Version: 2.1 Name: froog Version: 0.1.2 Summary: FROG: Fast Real-time
+Metadata-Version: 2.1 Name: froog Version: 0.1.3 Summary: FROG: Fast Real-time
 Optimization of Gradients Author: Kevin Buhler License: MIT Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Requires-Python: >=3.6 Description-Content-Type: text/markdown License-
 File: LICENSE # frog [unit test badge]
                                [froog the frog]
                 frog: fast real-time optimization of gradients
-                           documentation | examples
+           documentation | examples | documentation | pypi | github
 
-a beautifully compact machine-learning library modern ml development is
-unintuitive, time consuming, and unaccessible. why not make it possible for
-anyone to build? ### Overview of Features - Tensors - Automatic Differentiation
-- Forward and backward passes - Input/gradient shape-tracking - MNIST example -
-2D Convolutions (im2col) - Gradient checking - The most common optimizers (SGD,
-Adam, RMSProp) ### Math Operations - Scalar-Matrix Multiplication - Dot Product
-- Sum - ReLU - Log Softmax - 2D Convolution # Bounties We really want to get a
-useful model working right out of the box! Our top bounty is to get
-EfficientNet v2 model working inside of the examples folder. - EfficientNet v2
-(**top priority**) #### Easy - built in MLP model - binary cross entropy -
-dropout layer - flatten #### Medium - publish to pip3 - simplify how context
-and gradients are handled #### Hard - Transformers - Stable Diffusion -
+a beautifully compact machine-learning library  # Installation ```bash pip
+install froog ``` ### Overview of Features - Tensors - Automatic
+Differentiation - Forward and backward passes - Input/gradient shape-tracking -
+MNIST example - 2D Convolutions (im2col) - Gradient checking - The most common
+optimizers (SGD, Adam, RMSProp) ### Math Operations - Scalar-Matrix
+Multiplication - Dot Product - Sum - ReLU - Log Softmax - 2D Convolution #
+Bounties We really want to get a useful model working right out of the box! Our
+top bounty is to get EfficientNet v2 model working inside of the examples
+folder. - EfficientNet v2 (**top priority**) #### Easy - built in MLP model -
+binary cross entropy - dropout layer - flatten #### Medium - simplify how
+context and gradients are handled #### Hard - Transformers - Stable Diffusion -
 Winograd Convs - MPS support - CUDA support # Contributing Here are some basic
 guidelines for contributing: * Reduce code * Increase speed * Add features * In
 that order Bug fixes are the best and always welcome Conceptual cleanups are
 great All features must include tests
```

### Comparing `froog-0.1.2/setup.py` & `froog-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(directory, 'README.md'), encoding='utf-8') as f:
   long_description = f.read()
 
 setup(name='froog',
-      version='0.1.2',
+      version='0.1.3',
       description='FROG: Fast Real-time Optimization of Gradients',
       author='Kevin Buhler',
       license='MIT',
       long_description=long_description,
       long_description_content_type='text/markdown',
       packages = ['frog'],
       classifiers=[
```

