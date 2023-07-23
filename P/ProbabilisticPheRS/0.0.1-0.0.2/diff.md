# Comparing `tmp/ProbabilisticPheRS-0.0.1.tar.gz` & `tmp/ProbabilisticPheRS-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProbabilisticPheRS-0.0.1.tar", last modified: Sun Jul 23 23:14:24 2023, max compression
+gzip compressed data, was "ProbabilisticPheRS-0.0.2.tar", last modified: Sun Jul 23 23:51:14 2023, max compression
```

## Comparing `ProbabilisticPheRS-0.0.1.tar` & `ProbabilisticPheRS-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 davidblair   (501) staff       (20)        0 2023-07-23 23:14:24.444107 ProbabilisticPheRS-0.0.1/
--rw-r--r--   0 davidblair   (501) staff       (20)      506 2023-07-23 23:14:24.443966 ProbabilisticPheRS-0.0.1/PKG-INFO
-drwxr-xr-x   0 davidblair   (501) staff       (20)        0 2023-07-23 23:14:24.442956 ProbabilisticPheRS-0.0.1/ProbabilisticPheRS/
--rw-r--r--   0 davidblair   (501) staff       (20)    19266 2023-07-21 03:14:39.000000 ProbabilisticPheRS-0.0.1/ProbabilisticPheRS/DirichletPriorOptimizer.py
--rw-r--r--   0 davidblair   (501) staff       (20)    10527 2023-07-23 22:59:15.000000 ProbabilisticPheRS-0.0.1/ProbabilisticPheRS/MarginalFrequencyPrior.py
--rw-r--r--   0 davidblair   (501) staff       (20)    12541 2023-07-23 22:58:51.000000 ProbabilisticPheRS-0.0.1/ProbabilisticPheRS/PDSBase.py
--rw-r--r--   0 davidblair   (501) staff       (20)     6912 2023-07-23 22:34:51.000000 ProbabilisticPheRS-0.0.1/ProbabilisticPheRS/PDSSim.py
--rw-r--r--   0 davidblair   (501) staff       (20)    25925 2023-07-23 22:58:57.000000 ProbabilisticPheRS-0.0.1/ProbabilisticPheRS/ProbabilisticPheRS.py
--rw-r--r--   0 davidblair   (501) staff       (20)       53 2023-07-23 22:35:51.000000 ProbabilisticPheRS-0.0.1/ProbabilisticPheRS/__init__.py
-drwxr-xr-x   0 davidblair   (501) staff       (20)        0 2023-07-23 23:14:24.443766 ProbabilisticPheRS-0.0.1/ProbabilisticPheRS.egg-info/
--rw-r--r--   0 davidblair   (501) staff       (20)      506 2023-07-23 23:14:24.000000 ProbabilisticPheRS-0.0.1/ProbabilisticPheRS.egg-info/PKG-INFO
--rw-r--r--   0 davidblair   (501) staff       (20)      449 2023-07-23 23:14:24.000000 ProbabilisticPheRS-0.0.1/ProbabilisticPheRS.egg-info/SOURCES.txt
--rw-r--r--   0 davidblair   (501) staff       (20)        1 2023-07-23 23:14:24.000000 ProbabilisticPheRS-0.0.1/ProbabilisticPheRS.egg-info/dependency_links.txt
--rw-r--r--   0 davidblair   (501) staff       (20)       80 2023-07-23 23:14:24.000000 ProbabilisticPheRS-0.0.1/ProbabilisticPheRS.egg-info/requires.txt
--rw-r--r--   0 davidblair   (501) staff       (20)       19 2023-07-23 23:14:24.000000 ProbabilisticPheRS-0.0.1/ProbabilisticPheRS.egg-info/top_level.txt
--rw-r--r--   0 davidblair   (501) staff       (20)      167 2023-07-23 22:44:52.000000 ProbabilisticPheRS-0.0.1/README.md
--rw-r--r--   0 davidblair   (501) staff       (20)       38 2023-07-23 23:14:24.444144 ProbabilisticPheRS-0.0.1/setup.cfg
--rw-r--r--   0 davidblair   (501) staff       (20)     1069 2023-07-23 23:00:36.000000 ProbabilisticPheRS-0.0.1/setup.py
+drwxr-xr-x   0 davidblair   (501) staff       (20)        0 2023-07-23 23:51:14.473224 ProbabilisticPheRS-0.0.2/
+-rw-r--r--   0 davidblair   (501) staff       (20)      506 2023-07-23 23:51:14.473077 ProbabilisticPheRS-0.0.2/PKG-INFO
+drwxr-xr-x   0 davidblair   (501) staff       (20)        0 2023-07-23 23:51:14.471928 ProbabilisticPheRS-0.0.2/ProbabilisticPheRS/
+-rw-r--r--   0 davidblair   (501) staff       (20)    19266 2023-07-21 03:14:39.000000 ProbabilisticPheRS-0.0.2/ProbabilisticPheRS/DirichletPriorOptimizer.py
+-rw-r--r--   0 davidblair   (501) staff       (20)    10527 2023-07-23 22:59:15.000000 ProbabilisticPheRS-0.0.2/ProbabilisticPheRS/MarginalFrequencyPrior.py
+-rw-r--r--   0 davidblair   (501) staff       (20)    12541 2023-07-23 22:58:51.000000 ProbabilisticPheRS-0.0.2/ProbabilisticPheRS/PDSBase.py
+-rw-r--r--   0 davidblair   (501) staff       (20)     6912 2023-07-23 22:34:51.000000 ProbabilisticPheRS-0.0.2/ProbabilisticPheRS/PDSSim.py
+-rw-r--r--   0 davidblair   (501) staff       (20)    25925 2023-07-23 23:49:16.000000 ProbabilisticPheRS-0.0.2/ProbabilisticPheRS/ProbabilisticPheRS.py
+-rw-r--r--   0 davidblair   (501) staff       (20)       53 2023-07-23 22:35:51.000000 ProbabilisticPheRS-0.0.2/ProbabilisticPheRS/__init__.py
+drwxr-xr-x   0 davidblair   (501) staff       (20)        0 2023-07-23 23:51:14.472726 ProbabilisticPheRS-0.0.2/ProbabilisticPheRS.egg-info/
+-rw-r--r--   0 davidblair   (501) staff       (20)      506 2023-07-23 23:51:14.000000 ProbabilisticPheRS-0.0.2/ProbabilisticPheRS.egg-info/PKG-INFO
+-rw-r--r--   0 davidblair   (501) staff       (20)      449 2023-07-23 23:51:14.000000 ProbabilisticPheRS-0.0.2/ProbabilisticPheRS.egg-info/SOURCES.txt
+-rw-r--r--   0 davidblair   (501) staff       (20)        1 2023-07-23 23:51:14.000000 ProbabilisticPheRS-0.0.2/ProbabilisticPheRS.egg-info/dependency_links.txt
+-rw-r--r--   0 davidblair   (501) staff       (20)       85 2023-07-23 23:51:14.000000 ProbabilisticPheRS-0.0.2/ProbabilisticPheRS.egg-info/requires.txt
+-rw-r--r--   0 davidblair   (501) staff       (20)       19 2023-07-23 23:51:14.000000 ProbabilisticPheRS-0.0.2/ProbabilisticPheRS.egg-info/top_level.txt
+-rw-r--r--   0 davidblair   (501) staff       (20)      167 2023-07-23 22:44:52.000000 ProbabilisticPheRS-0.0.2/README.md
+-rw-r--r--   0 davidblair   (501) staff       (20)       38 2023-07-23 23:51:14.473270 ProbabilisticPheRS-0.0.2/setup.cfg
+-rw-r--r--   0 davidblair   (501) staff       (20)     1074 2023-07-23 23:48:55.000000 ProbabilisticPheRS-0.0.2/setup.py
```

### Comparing `ProbabilisticPheRS-0.0.1/ProbabilisticPheRS/DirichletPriorOptimizer.py` & `ProbabilisticPheRS-0.0.2/ProbabilisticPheRS/DirichletPriorOptimizer.py`

 * *Files identical despite different names*

### Comparing `ProbabilisticPheRS-0.0.1/ProbabilisticPheRS/MarginalFrequencyPrior.py` & `ProbabilisticPheRS-0.0.2/ProbabilisticPheRS/MarginalFrequencyPrior.py`

 * *Files identical despite different names*

### Comparing `ProbabilisticPheRS-0.0.1/ProbabilisticPheRS/PDSBase.py` & `ProbabilisticPheRS-0.0.2/ProbabilisticPheRS/PDSBase.py`

 * *Files identical despite different names*

### Comparing `ProbabilisticPheRS-0.0.1/ProbabilisticPheRS/PDSSim.py` & `ProbabilisticPheRS-0.0.2/ProbabilisticPheRS/PDSSim.py`

 * *Files identical despite different names*

### Comparing `ProbabilisticPheRS-0.0.1/ProbabilisticPheRS/ProbabilisticPheRS.py` & `ProbabilisticPheRS-0.0.2/ProbabilisticPheRS/ProbabilisticPheRS.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from .PDSBase import InferenceDataStruct,PDSBase
 from .MarginalFrequencyPrior import MarginalFrequencyPrior
 
 SMALL_FLOAT=np.finfo(np.float64).eps
 MINLOG = np.log(SMALL_FLOAT)
 
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 
 class ProbabilisticPheRS(PDSBase):
 
 	def _cosine_annealing_schedule(self, init_temp,max_temp,n_steps):
 		t=np.linspace(0,1.0,n_steps)
 		return init_temp+0.5*(max_temp-init_temp)*(1-np.cos(t*np.pi))
```

### Comparing `ProbabilisticPheRS-0.0.1/setup.py` & `ProbabilisticPheRS-0.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     install_requires=[
         'numpy',
         'pandas',
         'scipy',
         'torch',
         'PiecewiseBeta',
         'tqdm',
-        'sklearn',
+        'scikit-learn',
         'pytorch-minimize',
         'tensordict'
         ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

