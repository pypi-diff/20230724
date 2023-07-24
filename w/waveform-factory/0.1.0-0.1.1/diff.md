# Comparing `tmp/waveform-factory-0.1.0.tar.gz` & `tmp/waveform_factory-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waveform-factory-0.1.0.tar", last modified: Mon Jul 24 20:55:34 2023, max compression
+gzip compressed data, was "waveform_factory-0.1.1.tar", last modified: Mon Jul 24 21:48:25 2023, max compression
```

## Comparing `waveform-factory-0.1.0.tar` & `waveform_factory-0.1.1.tar`

### file list

```diff
@@ -1,48 +1,51 @@
-drwxr-xr-x   0 paulbennett   (501) staff       (20)        0 2023-07-24 20:55:34.577820 waveform-factory-0.1.0/
--rw-r--r--   0 paulbennett   (501) staff       (20)     1069 2023-07-24 19:12:11.000000 waveform-factory-0.1.0/LICENSE
--rw-r--r--   0 paulbennett   (501) staff       (20)      481 2023-07-24 20:55:34.577698 waveform-factory-0.1.0/PKG-INFO
--rw-r--r--   0 paulbennett   (501) staff       (20)      696 2023-07-24 19:12:11.000000 waveform-factory-0.1.0/README.md
-drwxr-xr-x   0 paulbennett   (501) staff       (20)        0 2023-07-24 20:55:34.574881 waveform-factory-0.1.0/patterns/
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform-factory-0.1.0/patterns/__init__.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform-factory-0.1.0/patterns/arches.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform-factory-0.1.0/patterns/autoregressive.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform-factory-0.1.0/patterns/cosine.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform-factory-0.1.0/patterns/decay.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform-factory-0.1.0/patterns/exponential.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform-factory-0.1.0/patterns/gaussian_noise.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform-factory-0.1.0/patterns/morlet.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform-factory-0.1.0/patterns/rate.py
--rw-r--r--   0 paulbennett   (501) staff       (20)     1387 2023-07-13 16:23:36.000000 waveform-factory-0.1.0/patterns/sawtooth.py
--rw-r--r--   0 paulbennett   (501) staff       (20)     1073 2023-07-13 16:28:42.000000 waveform-factory-0.1.0/patterns/sine.py
--rw-r--r--   0 paulbennett   (501) staff       (20)     1186 2023-07-24 19:34:39.000000 waveform-factory-0.1.0/patterns/square.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform-factory-0.1.0/patterns/step.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform-factory-0.1.0/patterns/triangle.py
--rw-r--r--   0 paulbennett   (501) staff       (20)       38 2023-07-24 20:55:34.577857 waveform-factory-0.1.0/setup.cfg
--rw-r--r--   0 paulbennett   (501) staff       (20)      617 2023-07-24 20:51:55.000000 waveform-factory-0.1.0/setup.py
-drwxr-xr-x   0 paulbennett   (501) staff       (20)        0 2023-07-24 20:55:34.575044 waveform-factory-0.1.0/tests/
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform-factory-0.1.0/tests/__init__.py
-drwxr-xr-x   0 paulbennett   (501) staff       (20)        0 2023-07-24 20:55:34.576674 waveform-factory-0.1.0/tests/patterns/
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform-factory-0.1.0/tests/patterns/__init__.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform-factory-0.1.0/tests/patterns/test_arches.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform-factory-0.1.0/tests/patterns/test_autoregressive.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform-factory-0.1.0/tests/patterns/test_cosine.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform-factory-0.1.0/tests/patterns/test_decay.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform-factory-0.1.0/tests/patterns/test_exponential.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform-factory-0.1.0/tests/patterns/test_gaussian_noise.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform-factory-0.1.0/tests/patterns/test_morlet.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform-factory-0.1.0/tests/patterns/test_rate.py
--rw-r--r--   0 paulbennett   (501) staff       (20)     4769 2023-07-13 16:25:08.000000 waveform-factory-0.1.0/tests/patterns/test_sawtooth.py
--rw-r--r--   0 paulbennett   (501) staff       (20)     4105 2023-07-13 20:30:09.000000 waveform-factory-0.1.0/tests/patterns/test_sine.py
--rw-r--r--   0 paulbennett   (501) staff       (20)     3094 2023-07-24 20:41:33.000000 waveform-factory-0.1.0/tests/patterns/test_square.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform-factory-0.1.0/tests/patterns/test_step.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform-factory-0.1.0/tests/patterns/test_triangle.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform-factory-0.1.0/tests/test_pattern_generator.py
-drwxr-xr-x   0 paulbennett   (501) staff       (20)        0 2023-07-24 20:55:34.576853 waveform-factory-0.1.0/utils/
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform-factory-0.1.0/utils/__init__.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform-factory-0.1.0/utils/helpers.py
-drwxr-xr-x   0 paulbennett   (501) staff       (20)        0 2023-07-24 20:55:34.577516 waveform-factory-0.1.0/waveform_factory.egg-info/
--rw-r--r--   0 paulbennett   (501) staff       (20)      481 2023-07-24 20:55:34.000000 waveform-factory-0.1.0/waveform_factory.egg-info/PKG-INFO
--rw-r--r--   0 paulbennett   (501) staff       (20)     1031 2023-07-24 20:55:34.000000 waveform-factory-0.1.0/waveform_factory.egg-info/SOURCES.txt
--rw-r--r--   0 paulbennett   (501) staff       (20)        1 2023-07-24 20:55:34.000000 waveform-factory-0.1.0/waveform_factory.egg-info/dependency_links.txt
--rw-r--r--   0 paulbennett   (501) staff       (20)       17 2023-07-24 20:55:34.000000 waveform-factory-0.1.0/waveform_factory.egg-info/requires.txt
--rw-r--r--   0 paulbennett   (501) staff       (20)       21 2023-07-24 20:55:34.000000 waveform-factory-0.1.0/waveform_factory.egg-info/top_level.txt
+drwxr-xr-x   0 paulbennett   (501) staff       (20)        0 2023-07-24 21:48:25.607610 waveform_factory-0.1.1/
+-rw-r--r--   0 paulbennett   (501) staff       (20)     1069 2023-07-24 19:12:11.000000 waveform_factory-0.1.1/LICENSE
+-rw-r--r--   0 paulbennett   (501) staff       (20)      264 2023-07-24 21:48:25.607453 waveform_factory-0.1.1/PKG-INFO
+-rw-r--r--   0 paulbennett   (501) staff       (20)      696 2023-07-24 19:12:11.000000 waveform_factory-0.1.1/README.md
+-rw-r--r--   0 paulbennett   (501) staff       (20)       38 2023-07-24 21:48:25.607651 waveform_factory-0.1.1/setup.cfg
+-rw-r--r--   0 paulbennett   (501) staff       (20)      717 2023-07-24 21:48:14.000000 waveform_factory-0.1.1/setup.py
+drwxr-xr-x   0 paulbennett   (501) staff       (20)        0 2023-07-24 21:48:25.603199 waveform_factory-0.1.1/tests/
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/tests/__init__.py
+drwxr-xr-x   0 paulbennett   (501) staff       (20)        0 2023-07-24 21:48:25.604864 waveform_factory-0.1.1/tests/patterns/
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/tests/patterns/__init__.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/tests/patterns/test_arches.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/tests/patterns/test_autoregressive.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/tests/patterns/test_cosine.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/tests/patterns/test_decay.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/tests/patterns/test_exponential.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/tests/patterns/test_gaussian_noise.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/tests/patterns/test_morlet.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/tests/patterns/test_rate.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)     4786 2023-07-24 21:46:24.000000 waveform_factory-0.1.1/tests/patterns/test_sawtooth.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)     4122 2023-07-24 21:46:24.000000 waveform_factory-0.1.1/tests/patterns/test_sine.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)     3111 2023-07-24 21:46:24.000000 waveform_factory-0.1.1/tests/patterns/test_square.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/tests/patterns/test_step.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/tests/patterns/test_triangle.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/tests/test_pattern_generator.py
+drwxr-xr-x   0 paulbennett   (501) staff       (20)        0 2023-07-24 21:48:25.605044 waveform_factory-0.1.1/waveform_factory/
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-24 21:46:11.000000 waveform_factory-0.1.1/waveform_factory/__init__.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/waveform_factory/pattern_generator.py
+drwxr-xr-x   0 paulbennett   (501) staff       (20)        0 2023-07-24 21:48:25.607124 waveform_factory-0.1.1/waveform_factory/patterns/
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/waveform_factory/patterns/__init__.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/waveform_factory/patterns/arches.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/waveform_factory/patterns/autoregressive.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/waveform_factory/patterns/cosine.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/waveform_factory/patterns/decay.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/waveform_factory/patterns/exponential.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/waveform_factory/patterns/gaussian_noise.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/waveform_factory/patterns/morlet.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/waveform_factory/patterns/rate.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)     1387 2023-07-13 16:23:36.000000 waveform_factory-0.1.1/waveform_factory/patterns/sawtooth.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)     1073 2023-07-13 16:28:42.000000 waveform_factory-0.1.1/waveform_factory/patterns/sine.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)     1186 2023-07-24 19:34:39.000000 waveform_factory-0.1.1/waveform_factory/patterns/square.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/waveform_factory/patterns/step.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/waveform_factory/patterns/triangle.py
+drwxr-xr-x   0 paulbennett   (501) staff       (20)        0 2023-07-24 21:48:25.607297 waveform_factory-0.1.1/waveform_factory/utils/
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/waveform_factory/utils/__init__.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/waveform_factory/utils/helpers.py
+drwxr-xr-x   0 paulbennett   (501) staff       (20)        0 2023-07-24 21:48:25.605564 waveform_factory-0.1.1/waveform_factory.egg-info/
+-rw-r--r--   0 paulbennett   (501) staff       (20)      264 2023-07-24 21:48:25.000000 waveform_factory-0.1.1/waveform_factory.egg-info/PKG-INFO
+-rw-r--r--   0 paulbennett   (501) staff       (20)     1370 2023-07-24 21:48:25.000000 waveform_factory-0.1.1/waveform_factory.egg-info/SOURCES.txt
+-rw-r--r--   0 paulbennett   (501) staff       (20)        1 2023-07-24 21:48:25.000000 waveform_factory-0.1.1/waveform_factory.egg-info/dependency_links.txt
+-rw-r--r--   0 paulbennett   (501) staff       (20)       17 2023-07-24 21:48:25.000000 waveform_factory-0.1.1/waveform_factory.egg-info/requires.txt
+-rw-r--r--   0 paulbennett   (501) staff       (20)       17 2023-07-24 21:48:25.000000 waveform_factory-0.1.1/waveform_factory.egg-info/top_level.txt
```

### Comparing `waveform-factory-0.1.0/LICENSE` & `waveform_factory-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `waveform-factory-0.1.0/README.md` & `waveform_factory-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `waveform-factory-0.1.0/patterns/sawtooth.py` & `waveform_factory-0.1.1/waveform_factory/patterns/sawtooth.py`

 * *Files identical despite different names*

### Comparing `waveform-factory-0.1.0/patterns/sine.py` & `waveform_factory-0.1.1/waveform_factory/patterns/sine.py`

 * *Files identical despite different names*

### Comparing `waveform-factory-0.1.0/patterns/square.py` & `waveform_factory-0.1.1/waveform_factory/patterns/square.py`

 * *Files identical despite different names*

### Comparing `waveform-factory-0.1.0/setup.py` & `waveform_factory-0.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
-    name='waveform-factory',
-    version='0.1.0',
+    name='waveform_factory',
+    version='0.1.1',
     url='https://github.com/MrB-Can/waveform-factory',
     author='Paul Bennett',
     author_email='paul@lgis.ca',
-    description='Waveform Factory is a python library that generates various types of waveform patterns. It is '
+    description='Wave form data generator',
+    lonmg_description='Waveform Factory is a python library that generates various types of waveform patterns. It is '
                 'designed to aid in the creation, manipulation, and analysis of waveform data for various '
                 'applications including music, signal processing, and more.',
-    packages=find_packages(),
+    packages=find_packages(include=['waveform_factory', 'waveform_factory.*']),
     install_requires=[
         'numpy',
         'matplotlib',
     ],
 )
```

### Comparing `waveform-factory-0.1.0/tests/patterns/test_sawtooth.py` & `waveform_factory-0.1.1/tests/patterns/test_sawtooth.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 from matplotlib import pyplot as plt
 
-from patterns import sawtooth
+from waveform_factory.patterns import sawtooth
 
 
 def test_generate_sawtooth():
     frequency = 440  # A4 note
     amplitude = 1.0  # max amplitude
     length = 2.0  # 2 seconds
     sample_rate = 44100  # standard audio CD sample rate
```

### Comparing `waveform-factory-0.1.0/tests/patterns/test_sine.py` & `waveform_factory-0.1.1/tests/patterns/test_sine.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 from matplotlib import pyplot as plt
-from patterns.sine import generate_sine_wave
+from waveform_factory.patterns.sine import generate_sine_wave
 
 class SineWaveTest:
     def run_tests(self):
         self.test_generate_sine_wave()
 
     def test_generate_sine_wave(self):
         frequency = 440
```

### Comparing `waveform-factory-0.1.0/tests/patterns/test_square.py` & `waveform_factory-0.1.1/tests/patterns/test_square.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 from matplotlib import pyplot as plt
-from patterns.square import generate_square_wave
+from waveform_factory.patterns.square import generate_square_wave
 
 class SquareWaveTest:
     def run_tests(self):
         self.test_generate_square_wave()
 
 
     def test_generate_square_wave(self):
```

