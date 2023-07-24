# Comparing `tmp/froog-0.1.5.tar.gz` & `tmp/froog-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "froog-0.1.5.tar", last modified: Mon Jul 24 01:54:39 2023, max compression
+gzip compressed data, was "froog-0.1.6.tar", last modified: Mon Jul 24 03:29:19 2023, max compression
```

## Comparing `froog-0.1.5.tar` & `froog-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-07-24 01:54:39.665607 froog-0.1.5/
--rw-r--r--   0 kevinbuhler   (501) staff       (20)       31 2023-07-16 20:10:22.000000 froog-0.1.5/LICENSE
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2415 2023-07-24 01:54:39.665493 froog-0.1.5/PKG-INFO
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2090 2023-07-24 01:53:24.000000 froog-0.1.5/README.md
-drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-07-24 01:54:39.664582 froog-0.1.5/frog/
--rw-r--r--   0 kevinbuhler   (501) staff       (20)       54 2023-07-24 00:15:18.000000 froog-0.1.5/frog/__init__.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2103 2023-07-19 07:06:24.000000 froog-0.1.5/frog/gradcheck.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)    10298 2023-07-24 00:13:42.000000 froog-0.1.5/frog/ops.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2016 2023-07-19 05:23:59.000000 froog-0.1.5/frog/optim.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     3802 2023-07-24 00:17:09.000000 froog-0.1.5/frog/tensor.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2685 2023-07-23 19:46:48.000000 froog-0.1.5/frog/utils.py
-drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-07-24 01:54:39.665283 froog-0.1.5/froog.egg-info/
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2415 2023-07-24 01:54:39.000000 froog-0.1.5/froog.egg-info/PKG-INFO
--rw-r--r--   0 kevinbuhler   (501) staff       (20)      260 2023-07-24 01:54:39.000000 froog-0.1.5/froog.egg-info/SOURCES.txt
--rw-r--r--   0 kevinbuhler   (501) staff       (20)        1 2023-07-24 01:54:39.000000 froog-0.1.5/froog.egg-info/dependency_links.txt
--rw-r--r--   0 kevinbuhler   (501) staff       (20)       15 2023-07-24 01:54:39.000000 froog-0.1.5/froog.egg-info/requires.txt
--rw-r--r--   0 kevinbuhler   (501) staff       (20)        5 2023-07-24 01:54:39.000000 froog-0.1.5/froog.egg-info/top_level.txt
--rw-r--r--   0 kevinbuhler   (501) staff       (20)       38 2023-07-24 01:54:39.665640 froog-0.1.5/setup.cfg
--rw-r--r--   0 kevinbuhler   (501) staff       (20)      849 2023-07-24 01:54:07.000000 froog-0.1.5/setup.py
+drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-07-24 03:29:19.273678 froog-0.1.6/
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)       31 2023-07-16 20:10:22.000000 froog-0.1.6/LICENSE
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2437 2023-07-24 03:29:19.273590 froog-0.1.6/PKG-INFO
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2112 2023-07-24 01:58:06.000000 froog-0.1.6/README.md
+drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-07-24 03:29:19.272624 froog-0.1.6/frog/
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)       54 2023-07-24 00:15:18.000000 froog-0.1.6/frog/__init__.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2103 2023-07-19 07:06:24.000000 froog-0.1.6/frog/gradcheck.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)    10298 2023-07-24 00:13:42.000000 froog-0.1.6/frog/ops.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2016 2023-07-19 05:23:59.000000 froog-0.1.6/frog/optim.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     3802 2023-07-24 00:17:09.000000 froog-0.1.6/frog/tensor.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2685 2023-07-23 19:46:48.000000 froog-0.1.6/frog/utils.py
+drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-07-24 03:29:19.273452 froog-0.1.6/froog.egg-info/
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2437 2023-07-24 03:29:19.000000 froog-0.1.6/froog.egg-info/PKG-INFO
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)      260 2023-07-24 03:29:19.000000 froog-0.1.6/froog.egg-info/SOURCES.txt
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)        1 2023-07-24 03:29:19.000000 froog-0.1.6/froog.egg-info/dependency_links.txt
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)       15 2023-07-24 03:29:19.000000 froog-0.1.6/froog.egg-info/requires.txt
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)        5 2023-07-24 03:29:19.000000 froog-0.1.6/froog.egg-info/top_level.txt
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)       38 2023-07-24 03:29:19.273709 froog-0.1.6/setup.cfg
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)      849 2023-07-24 03:29:13.000000 froog-0.1.6/setup.py
```

### Comparing `froog-0.1.5/PKG-INFO` & `froog-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: froog
-Version: 0.1.5
+Version: 0.1.6
 Summary: FROG: Fast Real-time Optimization of Gradients
 Author: Kevin Buhler
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -53,16 +53,19 @@
 Want to help but don't know where to start? 
 
 Our top bounty is to get EfficientNet v2 model working inside of the <a href="https://github.com/kevbuh/frog/tree/main/examples">examples</a> folder.
 
 #### Easy
 - built in MLP model
 - binary cross entropy
-- dropout layer
 - flatten
+- batch_norm
+- pad
+- swish
+- dropout 
 #### Medium
 - simplify how context and gradients are handled
 #### Hard
 - efficientNet
 - transformers
 - stable Diffusion
 - winograd Convs
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: froog Version: 0.1.5 Summary: FROG: Fast Real-time
+Metadata-Version: 2.1 Name: froog Version: 0.1.6 Summary: FROG: Fast Real-time
 Optimization of Gradients Author: Kevin Buhler License: MIT Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Requires-Python: >=3.6 Description-Content-Type: text/markdown License-
 File: LICENSE # frog [unit test badge]
                                [froog the frog]
                 frog: fast real-time optimization of gradients
                 a beautifully compact machine-learning library
@@ -12,13 +12,13 @@
 Tensors - Automatic Differentiation - Forward and backward passes - Input/
 gradient shape-tracking - MNIST example - 2D Convolutions (im2col) - Numerical
 gradient checking - The most common optimizers (SGD, Adam, RMSProp) ### Math
 Operations - Scalar-Matrix Multiplication - Dot Product - Sum - ReLU - Log
 Softmax - 2D Convolutions - Avg & Max pooling - More # Bounties Want to help
 but don't know where to start? Our top bounty is to get EfficientNet v2 model
 working inside of the examples folder. #### Easy - built in MLP model - binary
-cross entropy - dropout layer - flatten #### Medium - simplify how context and
-gradients are handled #### Hard - efficientNet - transformers - stable
-Diffusion - winograd Convs - MPS support - CUDA support # Contributing here are
-some basic guidelines for contributing: * reduce complexity (currently at 585
-lines of code) * increase speed * add features, must include tests * in that
-order more info on contributing
+cross entropy - flatten - batch_norm - pad - swish - dropout #### Medium -
+simplify how context and gradients are handled #### Hard - efficientNet -
+transformers - stable Diffusion - winograd Convs - MPS support - CUDA support #
+Contributing here are some basic guidelines for contributing: * reduce
+complexity (currently at 585 lines of code) * increase speed * add features,
+must include tests * in that order more info on contributing
```

### Comparing `froog-0.1.5/README.md` & `froog-0.1.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -41,16 +41,19 @@
 Want to help but don't know where to start? 
 
 Our top bounty is to get EfficientNet v2 model working inside of the <a href="https://github.com/kevbuh/frog/tree/main/examples">examples</a> folder.
 
 #### Easy
 - built in MLP model
 - binary cross entropy
-- dropout layer
 - flatten
+- batch_norm
+- pad
+- swish
+- dropout 
 #### Medium
 - simplify how context and gradients are handled
 #### Hard
 - efficientNet
 - transformers
 - stable Diffusion
 - winograd Convs
```

#### html2text {}

```diff
@@ -8,13 +8,13 @@
 Tensors - Automatic Differentiation - Forward and backward passes - Input/
 gradient shape-tracking - MNIST example - 2D Convolutions (im2col) - Numerical
 gradient checking - The most common optimizers (SGD, Adam, RMSProp) ### Math
 Operations - Scalar-Matrix Multiplication - Dot Product - Sum - ReLU - Log
 Softmax - 2D Convolutions - Avg & Max pooling - More # Bounties Want to help
 but don't know where to start? Our top bounty is to get EfficientNet v2 model
 working inside of the examples folder. #### Easy - built in MLP model - binary
-cross entropy - dropout layer - flatten #### Medium - simplify how context and
-gradients are handled #### Hard - efficientNet - transformers - stable
-Diffusion - winograd Convs - MPS support - CUDA support # Contributing here are
-some basic guidelines for contributing: * reduce complexity (currently at 585
-lines of code) * increase speed * add features, must include tests * in that
-order more info on contributing
+cross entropy - flatten - batch_norm - pad - swish - dropout #### Medium -
+simplify how context and gradients are handled #### Hard - efficientNet -
+transformers - stable Diffusion - winograd Convs - MPS support - CUDA support #
+Contributing here are some basic guidelines for contributing: * reduce
+complexity (currently at 585 lines of code) * increase speed * add features,
+must include tests * in that order more info on contributing
```

### Comparing `froog-0.1.5/frog/gradcheck.py` & `froog-0.1.6/frog/gradcheck.py`

 * *Files identical despite different names*

### Comparing `froog-0.1.5/frog/ops.py` & `froog-0.1.6/frog/ops.py`

 * *Files identical despite different names*

### Comparing `froog-0.1.5/frog/optim.py` & `froog-0.1.6/frog/optim.py`

 * *Files identical despite different names*

### Comparing `froog-0.1.5/frog/tensor.py` & `froog-0.1.6/frog/tensor.py`

 * *Files identical despite different names*

### Comparing `froog-0.1.5/frog/utils.py` & `froog-0.1.6/frog/utils.py`

 * *Files identical despite different names*

### Comparing `froog-0.1.5/froog.egg-info/PKG-INFO` & `froog-0.1.6/froog.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: froog
-Version: 0.1.5
+Version: 0.1.6
 Summary: FROG: Fast Real-time Optimization of Gradients
 Author: Kevin Buhler
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -53,16 +53,19 @@
 Want to help but don't know where to start? 
 
 Our top bounty is to get EfficientNet v2 model working inside of the <a href="https://github.com/kevbuh/frog/tree/main/examples">examples</a> folder.
 
 #### Easy
 - built in MLP model
 - binary cross entropy
-- dropout layer
 - flatten
+- batch_norm
+- pad
+- swish
+- dropout 
 #### Medium
 - simplify how context and gradients are handled
 #### Hard
 - efficientNet
 - transformers
 - stable Diffusion
 - winograd Convs
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: froog Version: 0.1.5 Summary: FROG: Fast Real-time
+Metadata-Version: 2.1 Name: froog Version: 0.1.6 Summary: FROG: Fast Real-time
 Optimization of Gradients Author: Kevin Buhler License: MIT Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Requires-Python: >=3.6 Description-Content-Type: text/markdown License-
 File: LICENSE # frog [unit test badge]
                                [froog the frog]
                 frog: fast real-time optimization of gradients
                 a beautifully compact machine-learning library
@@ -12,13 +12,13 @@
 Tensors - Automatic Differentiation - Forward and backward passes - Input/
 gradient shape-tracking - MNIST example - 2D Convolutions (im2col) - Numerical
 gradient checking - The most common optimizers (SGD, Adam, RMSProp) ### Math
 Operations - Scalar-Matrix Multiplication - Dot Product - Sum - ReLU - Log
 Softmax - 2D Convolutions - Avg & Max pooling - More # Bounties Want to help
 but don't know where to start? Our top bounty is to get EfficientNet v2 model
 working inside of the examples folder. #### Easy - built in MLP model - binary
-cross entropy - dropout layer - flatten #### Medium - simplify how context and
-gradients are handled #### Hard - efficientNet - transformers - stable
-Diffusion - winograd Convs - MPS support - CUDA support # Contributing here are
-some basic guidelines for contributing: * reduce complexity (currently at 585
-lines of code) * increase speed * add features, must include tests * in that
-order more info on contributing
+cross entropy - flatten - batch_norm - pad - swish - dropout #### Medium -
+simplify how context and gradients are handled #### Hard - efficientNet -
+transformers - stable Diffusion - winograd Convs - MPS support - CUDA support #
+Contributing here are some basic guidelines for contributing: * reduce
+complexity (currently at 585 lines of code) * increase speed * add features,
+must include tests * in that order more info on contributing
```

### Comparing `froog-0.1.5/setup.py` & `froog-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(directory, 'README.md'), encoding='utf-8') as f:
   long_description = f.read()
 
 setup(name='froog',
-      version='0.1.5',
+      version='0.1.6',
       description='FROG: Fast Real-time Optimization of Gradients',
       author='Kevin Buhler',
       license='MIT',
       long_description=long_description,
       long_description_content_type='text/markdown',
       packages = ['frog'],
       classifiers=[
```

