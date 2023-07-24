# Comparing `tmp/bojaxns-1.0.1.tar.gz` & `tmp/bojaxns-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bojaxns-1.0.1.tar", last modified: Thu Jul 20 23:49:52 2023, max compression
+gzip compressed data, was "bojaxns-1.0.2.tar", last modified: Mon Jul 24 01:33:45 2023, max compression
```

## Comparing `bojaxns-1.0.1.tar` & `bojaxns-1.0.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-20 23:49:52.601389 bojaxns-1.0.1/
--rw-rw-r--   0 albert    (1000) albert    (1000)     2553 2023-06-20 14:43:21.000000 bojaxns-1.0.1/LICENSE
--rw-rw-r--   0 albert    (1000) albert    (1000)     2106 2023-07-20 23:49:52.601389 bojaxns-1.0.1/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)     1655 2023-07-20 23:32:59.000000 bojaxns-1.0.1/README.md
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-20 23:49:52.601389 bojaxns-1.0.1/bojaxns/
--rw-rw-r--   0 albert    (1000) albert    (1000)      199 2023-07-20 23:19:20.000000 bojaxns-1.0.1/bojaxns/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5038 2023-06-29 23:24:48.000000 bojaxns-1.0.1/bojaxns/base.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     2218 2023-06-07 17:50:36.000000 bojaxns-1.0.1/bojaxns/basic.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     3282 2023-07-20 23:19:20.000000 bojaxns-1.0.1/bojaxns/experiment.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-20 23:49:52.601389 bojaxns-1.0.1/bojaxns/gaussian_process_formulation/
--rw-rw-r--   0 albert    (1000) albert    (1000)       70 2023-07-20 23:19:20.000000 bojaxns-1.0.1/bojaxns/gaussian_process_formulation/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    10678 2023-07-20 23:19:20.000000 bojaxns-1.0.1/bojaxns/gaussian_process_formulation/bayesian_optimiser.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    15665 2023-07-20 23:19:20.000000 bojaxns-1.0.1/bojaxns/gaussian_process_formulation/distribution_math.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     9088 2023-07-20 23:19:20.000000 bojaxns-1.0.1/bojaxns/gaussian_process_formulation/multi_step_lookahead.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-20 23:49:52.601389 bojaxns-1.0.1/bojaxns/gaussian_process_formulation/tests/
--rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-07-20 16:10:25.000000 bojaxns-1.0.1/bojaxns/gaussian_process_formulation/tests/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     4904 2023-07-20 23:19:20.000000 bojaxns-1.0.1/bojaxns/gaussian_process_formulation/tests/test_bayesian_optimiser.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5939 2023-07-20 23:19:20.000000 bojaxns-1.0.1/bojaxns/gaussian_process_formulation/tests/test_distribution_maths.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5069 2023-07-20 23:19:20.000000 bojaxns-1.0.1/bojaxns/parameter_space.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     9503 2023-07-20 23:19:20.000000 bojaxns-1.0.1/bojaxns/service.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-20 23:49:52.601389 bojaxns-1.0.1/bojaxns/tests/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2022-10-13 02:52:05.000000 bojaxns-1.0.1/bojaxns/tests/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     2181 2023-07-20 23:19:20.000000 bojaxns-1.0.1/bojaxns/tests/test_experiment.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     3508 2023-07-20 23:19:20.000000 bojaxns-1.0.1/bojaxns/tests/test_parameter_space.py
--rw-rw-r--   0 albert    (1000) albert    (1000)      622 2023-07-20 23:19:20.000000 bojaxns-1.0.1/bojaxns/tests/test_utils.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     2986 2023-07-20 22:11:27.000000 bojaxns-1.0.1/bojaxns/utils.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-20 23:49:52.601389 bojaxns-1.0.1/bojaxns.egg-info/
--rw-rw-r--   0 albert    (1000) albert    (1000)     2106 2023-07-20 23:49:52.000000 bojaxns-1.0.1/bojaxns.egg-info/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)      894 2023-07-20 23:49:52.000000 bojaxns-1.0.1/bojaxns.egg-info/SOURCES.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-07-20 23:49:52.000000 bojaxns-1.0.1/bojaxns.egg-info/dependency_links.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)        8 2023-07-20 23:49:52.000000 bojaxns-1.0.1/bojaxns.egg-info/top_level.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)      103 2023-04-19 01:15:53.000000 bojaxns-1.0.1/pyproject.toml
--rw-rw-r--   0 albert    (1000) albert    (1000)       38 2023-07-20 23:49:52.601389 bojaxns-1.0.1/setup.cfg
--rwxrwxr-x   0 albert    (1000) albert    (1000)      997 2023-07-20 23:49:43.000000 bojaxns-1.0.1/setup.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-24 01:33:45.080379 bojaxns-1.0.2/
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2553 2023-07-21 00:04:16.000000 bojaxns-1.0.2/LICENSE
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2259 2023-07-24 01:33:45.080379 bojaxns-1.0.2/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1806 2023-07-23 14:37:43.000000 bojaxns-1.0.2/README.md
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-24 01:33:45.080379 bojaxns-1.0.2/bojaxns/
+-rw-rw-r--   0 albert    (1000) albert    (1000)      199 2023-07-21 00:04:16.000000 bojaxns-1.0.2/bojaxns/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5038 2023-07-21 00:04:16.000000 bojaxns-1.0.2/bojaxns/base.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2005 2023-07-21 12:38:12.000000 bojaxns-1.0.2/bojaxns/basic.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     3282 2023-07-21 00:04:16.000000 bojaxns-1.0.2/bojaxns/experiment.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-24 01:33:45.080379 bojaxns-1.0.2/bojaxns/gaussian_process_formulation/
+-rw-rw-r--   0 albert    (1000) albert    (1000)       70 2023-07-21 00:04:16.000000 bojaxns-1.0.2/bojaxns/gaussian_process_formulation/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    10665 2023-07-23 14:42:45.000000 bojaxns-1.0.2/bojaxns/gaussian_process_formulation/bayesian_optimiser.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    15665 2023-07-21 00:04:16.000000 bojaxns-1.0.2/bojaxns/gaussian_process_formulation/distribution_math.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     9088 2023-07-21 00:04:16.000000 bojaxns-1.0.2/bojaxns/gaussian_process_formulation/multi_step_lookahead.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-24 01:33:45.080379 bojaxns-1.0.2/bojaxns/gaussian_process_formulation/tests/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-07-21 00:04:16.000000 bojaxns-1.0.2/bojaxns/gaussian_process_formulation/tests/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4904 2023-07-21 00:04:16.000000 bojaxns-1.0.2/bojaxns/gaussian_process_formulation/tests/test_bayesian_optimiser.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5939 2023-07-21 00:04:16.000000 bojaxns-1.0.2/bojaxns/gaussian_process_formulation/tests/test_distribution_maths.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5069 2023-07-21 00:04:16.000000 bojaxns-1.0.2/bojaxns/parameter_space.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     9505 2023-07-23 14:22:31.000000 bojaxns-1.0.2/bojaxns/service.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-24 01:33:45.080379 bojaxns-1.0.2/bojaxns/tests/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-07-21 00:04:16.000000 bojaxns-1.0.2/bojaxns/tests/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2181 2023-07-21 00:04:16.000000 bojaxns-1.0.2/bojaxns/tests/test_experiment.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     3508 2023-07-21 00:04:16.000000 bojaxns-1.0.2/bojaxns/tests/test_parameter_space.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)      622 2023-07-21 00:04:16.000000 bojaxns-1.0.2/bojaxns/tests/test_utils.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2986 2023-07-21 00:04:16.000000 bojaxns-1.0.2/bojaxns/utils.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-24 01:33:45.080379 bojaxns-1.0.2/bojaxns.egg-info/
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2259 2023-07-24 01:33:45.000000 bojaxns-1.0.2/bojaxns.egg-info/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)      894 2023-07-24 01:33:45.000000 bojaxns-1.0.2/bojaxns.egg-info/SOURCES.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-07-24 01:33:45.000000 bojaxns-1.0.2/bojaxns.egg-info/dependency_links.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)        8 2023-07-24 01:33:45.000000 bojaxns-1.0.2/bojaxns.egg-info/top_level.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)      103 2023-07-21 00:04:16.000000 bojaxns-1.0.2/pyproject.toml
+-rw-rw-r--   0 albert    (1000) albert    (1000)       38 2023-07-24 01:33:45.080379 bojaxns-1.0.2/setup.cfg
+-rwxrwxr-x   0 albert    (1000) albert    (1000)      961 2023-07-24 01:33:24.000000 bojaxns-1.0.2/setup.py
```

### Comparing `bojaxns-1.0.1/LICENSE` & `bojaxns-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.1/PKG-INFO` & `bojaxns-1.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: bojaxns
-Version: 1.0.1
+Version: 1.0.2
 Summary: Bayesian Optimisation with JAXNS
-Home-page: https://github.com/joshuaalbert/bojax
+Home-page: https://github.com/joshuaalbert/bojaxns
 Author: Joshua G. Albert
 Author-email: albert@strw.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Python](https://img.shields.io/pypi/pyversions/bojaxns.svg)](https://badge.fury.io/py/bojaxns)
 [![PyPI](https://badge.fury.io/py/bojaxns.svg)](https://badge.fury.io/py/bojaxns)
+[![Documentation Status](https://readthedocs.org/projects/bojaxns/badge/?version=latest)](https://bojaxns.readthedocs.io/en/latest/?badge=latest)
 
 Main
-Status: ![Workflow name](https://github.com/JoshuaAlbert/bojax/actions/workflows/unittests.yml/badge.svg?branch=main)
+Status: ![Workflow name](https://github.com/JoshuaAlbert/bojaxns/actions/workflows/unittests.yml/badge.svg?branch=main)
 
 Develop
-Status: ![Workflow name](https://github.com/JoshuaAlbert/bojax/actions/workflows/unittests.yml/badge.svg?branch=develop)
+Status: ![Workflow name](https://github.com/JoshuaAlbert/bojaxns/actions/workflows/unittests.yml/badge.svg?branch=develop)
 
 ## Mission: _To make advanced Bayesian Optimisation easy._
 
 # What is it?
 
 Bojaxns is:
 
@@ -64,10 +65,11 @@
 
 ```bash
 cd bojaxns
 pip install -r requirements.txt
 pip install -r requirements-tests.txt
 pip install .
 ```
+
 # Change Log
 
 20 July, 2023 -- Bojaxns 1.0.0 released
```

### Comparing `bojaxns-1.0.1/README.md` & `bojaxns-1.0.2/bojaxns.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,30 @@
+Metadata-Version: 2.1
+Name: bojaxns
+Version: 1.0.2
+Summary: Bayesian Optimisation with JAXNS
+Home-page: https://github.com/joshuaalbert/bojaxns
+Author: Joshua G. Albert
+Author-email: albert@strw.leidenuniv.nl
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![Python](https://img.shields.io/pypi/pyversions/bojaxns.svg)](https://badge.fury.io/py/bojaxns)
 [![PyPI](https://badge.fury.io/py/bojaxns.svg)](https://badge.fury.io/py/bojaxns)
+[![Documentation Status](https://readthedocs.org/projects/bojaxns/badge/?version=latest)](https://bojaxns.readthedocs.io/en/latest/?badge=latest)
 
 Main
-Status: ![Workflow name](https://github.com/JoshuaAlbert/bojax/actions/workflows/unittests.yml/badge.svg?branch=main)
+Status: ![Workflow name](https://github.com/JoshuaAlbert/bojaxns/actions/workflows/unittests.yml/badge.svg?branch=main)
 
 Develop
-Status: ![Workflow name](https://github.com/JoshuaAlbert/bojax/actions/workflows/unittests.yml/badge.svg?branch=develop)
+Status: ![Workflow name](https://github.com/JoshuaAlbert/bojaxns/actions/workflows/unittests.yml/badge.svg?branch=develop)
 
 ## Mission: _To make advanced Bayesian Optimisation easy._
 
 # What is it?
 
 Bojaxns is:
 
@@ -50,10 +65,11 @@
 
 ```bash
 cd bojaxns
 pip install -r requirements.txt
 pip install -r requirements-tests.txt
 pip install .
 ```
+
 # Change Log
 
 20 July, 2023 -- Bojaxns 1.0.0 released
```

### Comparing `bojaxns-1.0.1/bojaxns/base.py` & `bojaxns-1.0.2/bojaxns/base.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.1/bojaxns/basic.py` & `bojaxns-1.0.2/bojaxns/basic.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 import inspect
 from typing import Callable, Dict, Any, Type, List, TypeVar
 
 import numpy as np
-import ujson
 from pydantic import BaseModel
 
 
 # How many decimal places to retain. Note we use a fast but approximate method to compute.
 # Note: results will vary after serialisation and loading an array due to the truncation applied.
 
 
 class SerialisableBaseModel(BaseModel):
     class Config:
         validate_assignment = True
         arbitrary_types_allowed = True
-        json_loads = ujson.loads  # can use because ujson decodes NaN and Infinity
-        json_dumps = ujson.dumps  # (currently not possible because ujson doesn't encode NaN and Infinity like json)
         # json_dumps = lambda *args, **kwargs: json.dumps(*args, **kwargs, separators=(',', ':'))
         json_encoders = {np.ndarray: lambda x: x.tolist()}
 
     @classmethod
     def _deserialise(cls, kwargs):
         """Required for this class's __reduce__ method to be picklable."""
         return cls(**kwargs)
```

### Comparing `bojaxns-1.0.1/bojaxns/experiment.py` & `bojaxns-1.0.2/bojaxns/experiment.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.1/bojaxns/gaussian_process_formulation/bayesian_optimiser.py` & `bojaxns-1.0.2/bojaxns/gaussian_process_formulation/bayesian_optimiser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os.path
 
 import numpy as np
 import tensorflow_probability.substrates.jax as tfp
-from etils.array_types import PRNGKey
+from chex import PRNGKey
 from jax import random, numpy as jnp, vmap
 from jax._src.lax.control_flow import scan
 from jaxns import Model, TerminationCondition, NestedSamplerResults, ApproximateNestedSampler, \
     UniformSampler, UniDimSliceSampler
 from jaxns.types import float_type
 
 from bojaxns.base import AbstractAcquisition, MarginalisedAcquisitionFunction, MarginalisationData
```

### Comparing `bojaxns-1.0.1/bojaxns/gaussian_process_formulation/distribution_math.py` & `bojaxns-1.0.2/bojaxns/gaussian_process_formulation/distribution_math.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.1/bojaxns/gaussian_process_formulation/multi_step_lookahead.py` & `bojaxns-1.0.2/bojaxns/gaussian_process_formulation/multi_step_lookahead.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.1/bojaxns/gaussian_process_formulation/tests/test_bayesian_optimiser.py` & `bojaxns-1.0.2/bojaxns/gaussian_process_formulation/tests/test_bayesian_optimiser.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.1/bojaxns/gaussian_process_formulation/tests/test_distribution_maths.py` & `bojaxns-1.0.2/bojaxns/gaussian_process_formulation/tests/test_distribution_maths.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.1/bojaxns/parameter_space.py` & `bojaxns-1.0.2/bojaxns/parameter_space.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.1/bojaxns/service.py` & `bojaxns-1.0.2/bojaxns/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
                 experiment=self.experiment,
                 U=U,
                 prior_model=prior_model
             )
             self._experiment.trials[trial.trial_id] = trial
             return trial.trial_id
 
-        # get new trial parameter from bojax
+        # get new trial parameter from bojaxns
         bo = BayesianOptimiser(experiment=self._experiment, beta=beta, S=128)
         # U = bo.choose_next_U_multistep(
         #     key=key,
         #     batch_size=1,
         #     max_depth=2,
         #     num_simulations=1000,
         #     branch_factor=100
```

### Comparing `bojaxns-1.0.1/bojaxns/tests/test_experiment.py` & `bojaxns-1.0.2/bojaxns/tests/test_experiment.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.1/bojaxns/tests/test_parameter_space.py` & `bojaxns-1.0.2/bojaxns/tests/test_parameter_space.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.1/bojaxns/tests/test_utils.py` & `bojaxns-1.0.2/bojaxns/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.1/bojaxns/utils.py` & `bojaxns-1.0.2/bojaxns/utils.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.1/bojaxns.egg-info/SOURCES.txt` & `bojaxns-1.0.2/bojaxns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.1/setup.py` & `bojaxns-1.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages
 from setuptools import setup
 
-setup_requires = []
-# with open("requirements.txt", 'r') as fh:
-#     for line in fh:
-#         setup_requires.append(line)
+setup_requires = [
+    'jaxns>=2.2.1',
+    'tensorflow_probability',
+    'pydantic'
+]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='bojaxns',
-      version='1.0.1',
+      version='1.0.2',
       description='Bayesian Optimisation with JAXNS',
       long_description=long_description,
       long_description_content_type="text/markdown",
-      url="https://github.com/joshuaalbert/bojax",
+      url="https://github.com/joshuaalbert/bojaxns",
       author='Joshua G. Albert',
       author_email='albert@strw.leidenuniv.nl',
       setup_requires=setup_requires,
       tests_require=[
           'pytest>=2.8',
       ],
       package_dir={'': './'},
```

