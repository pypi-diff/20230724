# Comparing `tmp/pdme-0.8.8.tar.gz` & `tmp/pdme-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdme-0.8.8.tar", max compression
+gzip compressed data, was "pdme-0.8.9.tar", max compression
```

## Comparing `pdme-0.8.8.tar` & `pdme-0.8.9.tar`

### file list

```diff
@@ -1,25 +1,27 @@
--rw-r--r--   0        0        0     1229 2023-04-09 21:35:05.220972 pdme-0.8.8/README.md
--rw-r--r--   0        0        0      154 2023-04-09 21:35:05.220972 pdme-0.8.8/pdme/__init__.py
--rw-r--r--   0        0        0      184 2023-04-09 21:35:05.220972 pdme-0.8.8/pdme/inputs/__init__.py
--rw-r--r--   0        0        0      688 2023-04-09 21:35:05.224972 pdme-0.8.8/pdme/inputs/dot_inputs.py
--rw-r--r--   0        0        0      536 2023-04-09 21:35:05.224972 pdme-0.8.8/pdme/measurement/__init__.py
--rw-r--r--   0        0        0      984 2023-04-09 21:35:05.224972 pdme-0.8.8/pdme/measurement/dot_measure.py
--rw-r--r--   0        0        0     1224 2023-04-09 21:35:05.224972 pdme-0.8.8/pdme/measurement/dot_pair_measure.py
--rw-r--r--   0        0        0     1131 2023-04-09 21:35:05.224972 pdme-0.8.8/pdme/measurement/input_types.py
--rw-r--r--   0        0        0     5219 2023-04-09 21:35:05.224972 pdme-0.8.8/pdme/measurement/oscillating_dipole.py
--rw-r--r--   0        0        0       70 2023-04-09 21:35:05.224972 pdme-0.8.8/pdme/meta.py
--rw-r--r--   0        0        0     1066 2023-04-09 21:35:05.224972 pdme-0.8.8/pdme/model/__init__.py
--rw-r--r--   0        0        0     2367 2023-04-09 21:35:05.224972 pdme-0.8.8/pdme/model/fixed_magnitude_model.py
--rw-r--r--   0        0        0     3721 2023-04-09 21:35:05.224972 pdme-0.8.8/pdme/model/log_spaced_random_choice_fixed_orientation_model.py
--rw-r--r--   0        0        0     3372 2023-04-09 21:35:05.224972 pdme-0.8.8/pdme/model/log_spaced_random_choice_model.py
--rw-r--r--   0        0        0     3176 2023-04-09 21:35:05.224972 pdme-0.8.8/pdme/model/log_spaced_random_choice_xy_model.py
--rw-r--r--   0        0        0     1076 2023-04-09 21:35:05.224972 pdme-0.8.8/pdme/model/model.py
--rw-r--r--   0        0        0     2560 2023-04-09 21:35:05.224972 pdme-0.8.8/pdme/model/multidipole_fixed_magnitude_model.py
--rw-r--r--   0        0        0     3076 2023-04-09 21:35:05.224972 pdme-0.8.8/pdme/model/random_count_multidipole_fixed_magnitude_model.py
--rw-r--r--   0        0        0        0 2023-04-09 21:35:05.224972 pdme-0.8.8/pdme/py.typed
--rw-r--r--   0        0        0        0 2023-04-09 21:35:05.224972 pdme-0.8.8/pdme/util/__init__.py
--rw-r--r--   0        0        0     2952 2023-04-09 21:35:05.224972 pdme-0.8.8/pdme/util/fast_nonlocal_spectrum.py
--rw-r--r--   0        0        0     3604 2023-04-09 21:35:05.224972 pdme-0.8.8/pdme/util/fast_v_calc.py
--rw-r--r--   0        0        0      839 2023-04-09 21:35:05.224972 pdme-0.8.8/pyproject.toml
--rw-r--r--   0        0        0     1937 2023-04-09 21:36:06.738076 pdme-0.8.8/setup.py
--rw-r--r--   0        0        0     1768 2023-04-09 21:36:06.738456 pdme-0.8.8/PKG-INFO
+-rw-r--r--   0        0        0     1229 2023-07-23 23:34:55.200875 pdme-0.8.9/README.md
+-rw-r--r--   0        0        0      154 2023-07-23 23:34:55.204876 pdme-0.8.9/pdme/__init__.py
+-rw-r--r--   0        0        0      184 2023-07-23 23:34:55.204876 pdme-0.8.9/pdme/inputs/__init__.py
+-rw-r--r--   0        0        0      688 2023-07-23 23:34:55.204876 pdme-0.8.9/pdme/inputs/dot_inputs.py
+-rw-r--r--   0        0        0      536 2023-07-23 23:34:55.204876 pdme-0.8.9/pdme/measurement/__init__.py
+-rw-r--r--   0        0        0      984 2023-07-23 23:34:55.204876 pdme-0.8.9/pdme/measurement/dot_measure.py
+-rw-r--r--   0        0        0     1224 2023-07-23 23:34:55.204876 pdme-0.8.9/pdme/measurement/dot_pair_measure.py
+-rw-r--r--   0        0        0     1131 2023-07-23 23:34:55.204876 pdme-0.8.9/pdme/measurement/input_types.py
+-rw-r--r--   0        0        0     5219 2023-07-23 23:34:55.204876 pdme-0.8.9/pdme/measurement/oscillating_dipole.py
+-rw-r--r--   0        0        0       70 2023-07-23 23:34:55.204876 pdme-0.8.9/pdme/meta.py
+-rw-r--r--   0        0        0     1066 2023-07-23 23:34:55.204876 pdme-0.8.9/pdme/model/__init__.py
+-rw-r--r--   0        0        0     2367 2023-07-23 23:34:55.208876 pdme-0.8.9/pdme/model/fixed_magnitude_model.py
+-rw-r--r--   0        0        0     4992 2023-07-23 23:34:55.208876 pdme-0.8.9/pdme/model/log_spaced_random_choice_fixed_orientation_model.py
+-rw-r--r--   0        0        0     5332 2023-07-23 23:34:55.208876 pdme-0.8.9/pdme/model/log_spaced_random_choice_model.py
+-rw-r--r--   0        0        0     4699 2023-07-23 23:34:55.208876 pdme-0.8.9/pdme/model/log_spaced_random_choice_xy_model.py
+-rw-r--r--   0        0        0     3477 2023-07-23 23:34:55.208876 pdme-0.8.9/pdme/model/model.py
+-rw-r--r--   0        0        0     2560 2023-07-23 23:34:55.208876 pdme-0.8.9/pdme/model/multidipole_fixed_magnitude_model.py
+-rw-r--r--   0        0        0     3076 2023-07-23 23:34:55.208876 pdme-0.8.9/pdme/model/random_count_multidipole_fixed_magnitude_model.py
+-rw-r--r--   0        0        0        0 2023-07-23 23:34:55.208876 pdme-0.8.9/pdme/py.typed
+-rw-r--r--   0        0        0     1364 2023-07-23 23:34:55.208876 pdme-0.8.9/pdme/subspace_simulation/__init__.py
+-rw-r--r--   0        0        0      590 2023-07-23 23:34:55.208876 pdme-0.8.9/pdme/subspace_simulation/mcmc_costs.py
+-rw-r--r--   0        0        0        0 2023-07-23 23:34:55.208876 pdme-0.8.9/pdme/util/__init__.py
+-rw-r--r--   0        0        0     2952 2023-07-23 23:34:55.208876 pdme-0.8.9/pdme/util/fast_nonlocal_spectrum.py
+-rw-r--r--   0        0        0     3604 2023-07-23 23:34:55.208876 pdme-0.8.9/pdme/util/fast_v_calc.py
+-rw-r--r--   0        0        0      860 2023-07-23 23:34:55.208876 pdme-0.8.9/pyproject.toml
+-rw-r--r--   0        0        0     1972 2023-07-23 23:35:50.523858 pdme-0.8.9/setup.py
+-rw-r--r--   0        0        0     1720 2023-07-23 23:35:50.524524 pdme-0.8.9/PKG-INFO
```

### Comparing `pdme-0.8.8/README.md` & `pdme-0.8.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pdme - the python dipole model evaluator
 
 [![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-green.svg?style=flat-square)](https://conventionalcommits.org)
 [![PyPI](https://img.shields.io/pypi/v/pdme?style=flat-square)](https://pypi.org/project/pdme/)
 [![Jenkins](https://img.shields.io/jenkins/build?jobUrl=https%3A%2F%2Fjenkins.deepak.science%2Fjob%2Fgitea-physics%2Fjob%2Fpdme%2Fjob%2Fmaster&style=flat-square)](https://jenkins.deepak.science/job/gitea-physics/job/pdme/job/master/)
 ![Jenkins tests](https://img.shields.io/jenkins/tests?compact_message&jobUrl=https%3A%2F%2Fjenkins.deepak.science%2Fjob%2Fgitea-physics%2Fjob%2Fpdme%2Fjob%2Fmaster%2F&style=flat-square)
 ![Jenkins Coverage](https://img.shields.io/jenkins/coverage/cobertura?jobUrl=https%3A%2F%2Fjenkins.deepak.science%2Fjob%2Fgitea-physics%2Fjob%2Fpdme%2Fjob%2Fmaster%2F&style=flat-square)
-![Maintenance](https://img.shields.io/maintenance/yes/2022?style=flat-square)
+![Maintenance](https://img.shields.io/maintenance/yes/2023?style=flat-square)
 
 This repo has library code for evaluating dipole models.
 
 ## Getting started
 
 `poetry install` to start locally
```

### Comparing `pdme-0.8.8/pdme/inputs/dot_inputs.py` & `pdme-0.8.9/pdme/inputs/dot_inputs.py`

 * *Files identical despite different names*

### Comparing `pdme-0.8.8/pdme/measurement/__init__.py` & `pdme-0.8.9/pdme/measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `pdme-0.8.8/pdme/measurement/dot_measure.py` & `pdme-0.8.9/pdme/measurement/dot_measure.py`

 * *Files identical despite different names*

### Comparing `pdme-0.8.8/pdme/measurement/dot_pair_measure.py` & `pdme-0.8.9/pdme/measurement/dot_pair_measure.py`

 * *Files identical despite different names*

### Comparing `pdme-0.8.8/pdme/measurement/input_types.py` & `pdme-0.8.9/pdme/measurement/input_types.py`

 * *Files identical despite different names*

### Comparing `pdme-0.8.8/pdme/measurement/oscillating_dipole.py` & `pdme-0.8.9/pdme/measurement/oscillating_dipole.py`

 * *Files identical despite different names*

### Comparing `pdme-0.8.8/pdme/model/__init__.py` & `pdme-0.8.9/pdme/model/__init__.py`

 * *Files identical despite different names*

### Comparing `pdme-0.8.8/pdme/model/fixed_magnitude_model.py` & `pdme-0.8.9/pdme/model/fixed_magnitude_model.py`

 * *Files identical despite different names*

### Comparing `pdme-0.8.8/pdme/model/log_spaced_random_choice_fixed_orientation_model.py` & `pdme-0.8.9/pdme/model/log_spaced_random_choice_fixed_orientation_model.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import numpy
 import numpy.random
 from pdme.model.model import DipoleModel
 from pdme.measurement import (
 	OscillatingDipole,
 	OscillatingDipoleArrangement,
 )
+import logging
+from typing import Optional
+import pdme.subspace_simulation
+
+_logger = logging.getLogger(__name__)
 
 
 class LogSpacedRandomCountMultipleDipoleFixedMagnitudeFixedOrientationModel(
 	DipoleModel
 ):
 	"""
 	Model of multiple oscillating dipoles with a fixed magnitude and fixed rotation. Spaced log uniformly in relaxation time.
@@ -134,7 +139,55 @@
 		sx = rng.uniform(self.xmin, self.xmax, shape)
 		sy = rng.uniform(self.ymin, self.ymax, shape)
 		sz = rng.uniform(self.zmin, self.zmax, shape)
 
 		w = 10 ** rng.uniform(self.wexp_min, self.wexp_max, shape)
 
 		return numpy.stack([px, py, pz, sx, sy, sz, w], axis=-1)
+
+	def markov_chain_monte_carlo_proposal(
+		self,
+		dipole: numpy.ndarray,
+		stdev: pdme.subspace_simulation.DipoleStandardDeviation,
+		rng_arg: Optional[numpy.random.Generator] = None,
+	) -> numpy.ndarray:
+		if rng_arg is None:
+			rng_to_use = self.rng
+		else:
+			rng_to_use = rng_arg
+
+		px = dipole[0]
+		py = dipole[1]
+		pz = dipole[2]
+		# won't change p for this model of fixed dipole moment.
+
+		rx = dipole[3]
+		ry = dipole[4]
+		rz = dipole[5]
+
+		tentative_rx = rx + stdev.rx_step * rng_to_use.uniform(-1, 1)
+		if tentative_rx < self.xmin or tentative_rx > self.xmax:
+			tentative_rx = rx
+
+		tentative_ry = ry + stdev.ry_step * rng_to_use.uniform(-1, 1)
+		if tentative_ry < self.ymin or tentative_ry > self.ymax:
+			tentative_ry = ry
+		tentative_rz = rz + stdev.rz_step * rng_to_use.uniform(-1, 1)
+		if tentative_rz < self.zmin or tentative_rz > self.zmax:
+			tentative_rz = rz
+
+		w = dipole[6]
+		tentative_w = numpy.exp(
+			numpy.log(w) + (stdev.w_log_step * rng_to_use.uniform(-1, 1))
+		)
+		tentative_dip = numpy.array(
+			[
+				px,
+				py,
+				pz,
+				tentative_rx,
+				tentative_ry,
+				tentative_rz,
+				tentative_w,
+			]
+		)
+		return tentative_dip
```

### Comparing `pdme-0.8.8/pdme/model/log_spaced_random_choice_model.py` & `pdme-0.8.9/pdme/model/random_count_multidipole_fixed_magnitude_model.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,24 +3,20 @@
 from pdme.model.model import DipoleModel
 from pdme.measurement import (
 	OscillatingDipole,
 	OscillatingDipoleArrangement,
 )
 
 
-class LogSpacedRandomCountMultipleDipoleFixedMagnitudeModel(DipoleModel):
+class RandomCountMultipleDipoleFixedMagnitudeModel(DipoleModel):
 	"""
-	Model of multiple oscillating dipoles with a fixed magnitude, but free rotation. Spaced logarithmically.
+	Model of multiple oscillating dipoles with a fixed magnitude, but free rotation.
 
 	Parameters
 	----------
-
-	wexp_min: log-10 lower bound for dipole frequency
-	wexp_min: log-10 upper bound for dipole frequency
-
 	pfixed : float
 	The fixed dipole magnitude.
 
 	n_max : int
 	The maximum number of dipoles.
 
 	prob_occupancy : float
@@ -31,39 +27,35 @@
 		self,
 		xmin: float,
 		xmax: float,
 		ymin: float,
 		ymax: float,
 		zmin: float,
 		zmax: float,
-		wexp_min: float,
-		wexp_max: float,
 		pfixed: float,
 		n_max: int,
 		prob_occupancy: float,
 	) -> None:
 		self.xmin = xmin
 		self.xmax = xmax
 		self.ymin = ymin
 		self.ymax = ymax
 		self.zmin = zmin
 		self.zmax = zmax
-		self.wexp_min = wexp_min
-		self.wexp_max = wexp_max
 		self.pfixed = pfixed
 		self.rng = numpy.random.default_rng()
 		self.n_max = n_max
 		if prob_occupancy >= 1 or prob_occupancy <= 0:
 			raise ValueError(
 				f"The probability of a dipole site occupancy must be between 0 and 1, got {prob_occupancy}"
 			)
 		self.prob_occupancy = prob_occupancy
 
 	def __repr__(self) -> str:
-		return f"LogSpacedRandomCountMultipleDipoleFixedMagnitudeModel({self.xmin}, {self.xmax}, {self.ymin}, {self.ymax}, {self.zmin}, {self.zmax}, {self.wexp_min}, {self.wexp_max}, {self.pfixed}, {self.n_max}, {self.prob_occupancy})"
+		return f"RandomCountMultipleDipoleFixedMagnitudeModel({self.xmin}, {self.xmax}, {self.ymin}, {self.ymax}, {self.zmin}, {self.zmax}, {self.pfixed}, {self.n_max}, {self.prob_occupancy})"
 
 	def get_dipoles(
 		self, max_frequency: float, rng_to_use: numpy.random.Generator = None
 	) -> OscillatingDipoleArrangement:
 		rng: numpy.random.Generator
 		if rng_to_use is None:
 			rng = self.rng
@@ -83,25 +75,25 @@
 			s_pts = numpy.array(
 				(
 					rng.uniform(self.xmin, self.xmax),
 					rng.uniform(self.ymin, self.ymax),
 					rng.uniform(self.zmin, self.zmax),
 				)
 			)
-			frequency = 10 ** rng.uniform(self.wexp_min, self.wexp_max)
+			frequency = rng.uniform(0, max_frequency)
 
 			dipoles.append(
 				OscillatingDipole(numpy.array([px, py, pz]), s_pts, frequency)
 			)
 		return OscillatingDipoleArrangement(dipoles)
 
 	def get_monte_carlo_dipole_inputs(
 		self,
 		monte_carlo_n: int,
-		_: float,
+		max_frequency: float,
 		rng_to_use: numpy.random.Generator = None,
 	) -> numpy.ndarray:
 
 		rng: numpy.random.Generator
 		if rng_to_use is None:
 			rng = self.rng
 		else:
@@ -118,10 +110,10 @@
 		py = p_magnitude * numpy.sin(theta) * numpy.sin(phi)
 		pz = p_magnitude * numpy.cos(phi)
 
 		sx = rng.uniform(self.xmin, self.xmax, shape)
 		sy = rng.uniform(self.ymin, self.ymax, shape)
 		sz = rng.uniform(self.zmin, self.zmax, shape)
 
-		w = 10 ** rng.uniform(self.wexp_min, self.wexp_max, shape)
+		w = rng.uniform(1, max_frequency, shape)
 
 		return numpy.stack([px, py, pz, sx, sy, sz, w], axis=-1)
```

### Comparing `pdme-0.8.8/pdme/model/multidipole_fixed_magnitude_model.py` & `pdme-0.8.9/pdme/model/multidipole_fixed_magnitude_model.py`

 * *Files identical despite different names*

### Comparing `pdme-0.8.8/pdme/util/fast_nonlocal_spectrum.py` & `pdme-0.8.9/pdme/util/fast_nonlocal_spectrum.py`

 * *Files identical despite different names*

### Comparing `pdme-0.8.8/pdme/util/fast_v_calc.py` & `pdme-0.8.9/pdme/util/fast_v_calc.py`

 * *Files identical despite different names*

### Comparing `pdme-0.8.8/pyproject.toml` & `pdme-0.8.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [tool.poetry]
 name = "pdme"
-version = "0.8.8"
+version = "0.8.9"
 description = "Python dipole model evaluator"
 authors = ["Deepak <dmallubhotla+github@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.8,<3.10"
+python = ">=3.8.1,<3.10"
 numpy = "^1.22.3"
 scipy = "~1.10"
 
 [tool.poetry.dev-dependencies]
 pytest = ">=6"
 flake8 = "^4.0.0"
-pytest-cov = "^3.0.0"
+pytest-cov = "^4.1.0"
 mypy = "^0.961"
 ipython = "^8.2.0"
 black = "^22.3.0"
+syrupy = "^4.0.8"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
```

### Comparing `pdme-0.8.8/setup.py` & `pdme-0.8.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['pdme', 'pdme.inputs', 'pdme.measurement', 'pdme.model', 'pdme.util']
+['pdme',
+ 'pdme.inputs',
+ 'pdme.measurement',
+ 'pdme.model',
+ 'pdme.subspace_simulation',
+ 'pdme.util']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['numpy>=1.22.3,<2.0.0', 'scipy>=1.10,<1.11']
 
 setup_kwargs = {
     'name': 'pdme',
-    'version': '0.8.8',
+    'version': '0.8.9',
     'description': 'Python dipole model evaluator',
-    'long_description': '# pdme - the python dipole model evaluator\n\n[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-green.svg?style=flat-square)](https://conventionalcommits.org)\n[![PyPI](https://img.shields.io/pypi/v/pdme?style=flat-square)](https://pypi.org/project/pdme/)\n[![Jenkins](https://img.shields.io/jenkins/build?jobUrl=https%3A%2F%2Fjenkins.deepak.science%2Fjob%2Fgitea-physics%2Fjob%2Fpdme%2Fjob%2Fmaster&style=flat-square)](https://jenkins.deepak.science/job/gitea-physics/job/pdme/job/master/)\n![Jenkins tests](https://img.shields.io/jenkins/tests?compact_message&jobUrl=https%3A%2F%2Fjenkins.deepak.science%2Fjob%2Fgitea-physics%2Fjob%2Fpdme%2Fjob%2Fmaster%2F&style=flat-square)\n![Jenkins Coverage](https://img.shields.io/jenkins/coverage/cobertura?jobUrl=https%3A%2F%2Fjenkins.deepak.science%2Fjob%2Fgitea-physics%2Fjob%2Fpdme%2Fjob%2Fmaster%2F&style=flat-square)\n![Maintenance](https://img.shields.io/maintenance/yes/2022?style=flat-square)\n\nThis repo has library code for evaluating dipole models.\n\n## Getting started\n\n`poetry install` to start locally\n\nCommit using [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/), and when commits are on master, release with `doo release`.\n',
+    'long_description': '# pdme - the python dipole model evaluator\n\n[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-green.svg?style=flat-square)](https://conventionalcommits.org)\n[![PyPI](https://img.shields.io/pypi/v/pdme?style=flat-square)](https://pypi.org/project/pdme/)\n[![Jenkins](https://img.shields.io/jenkins/build?jobUrl=https%3A%2F%2Fjenkins.deepak.science%2Fjob%2Fgitea-physics%2Fjob%2Fpdme%2Fjob%2Fmaster&style=flat-square)](https://jenkins.deepak.science/job/gitea-physics/job/pdme/job/master/)\n![Jenkins tests](https://img.shields.io/jenkins/tests?compact_message&jobUrl=https%3A%2F%2Fjenkins.deepak.science%2Fjob%2Fgitea-physics%2Fjob%2Fpdme%2Fjob%2Fmaster%2F&style=flat-square)\n![Jenkins Coverage](https://img.shields.io/jenkins/coverage/cobertura?jobUrl=https%3A%2F%2Fjenkins.deepak.science%2Fjob%2Fgitea-physics%2Fjob%2Fpdme%2Fjob%2Fmaster%2F&style=flat-square)\n![Maintenance](https://img.shields.io/maintenance/yes/2023?style=flat-square)\n\nThis repo has library code for evaluating dipole models.\n\n## Getting started\n\n`poetry install` to start locally\n\nCommit using [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/), and when commits are on master, release with `doo release`.\n',
     'author': 'Deepak',
     'author_email': 'dmallubhotla+github@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.10',
+    'python_requires': '>=3.8.1,<3.10',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `pdme-0.8.8/PKG-INFO` & `pdme-0.8.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: pdme
-Version: 0.8.8
+Version: 0.8.9
 Summary: Python dipole model evaluator
 License: GPL-3.0-only
 Author: Deepak
 Author-email: dmallubhotla+github@gmail.com
-Requires-Python: >=3.8,<3.10
+Requires-Python: >=3.8.1,<3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: numpy (>=1.22.3,<2.0.0)
 Requires-Dist: scipy (>=1.10,<1.11)
 Description-Content-Type: text/markdown
 
 # pdme - the python dipole model evaluator
 
 [![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-green.svg?style=flat-square)](https://conventionalcommits.org)
 [![PyPI](https://img.shields.io/pypi/v/pdme?style=flat-square)](https://pypi.org/project/pdme/)
 [![Jenkins](https://img.shields.io/jenkins/build?jobUrl=https%3A%2F%2Fjenkins.deepak.science%2Fjob%2Fgitea-physics%2Fjob%2Fpdme%2Fjob%2Fmaster&style=flat-square)](https://jenkins.deepak.science/job/gitea-physics/job/pdme/job/master/)
 ![Jenkins tests](https://img.shields.io/jenkins/tests?compact_message&jobUrl=https%3A%2F%2Fjenkins.deepak.science%2Fjob%2Fgitea-physics%2Fjob%2Fpdme%2Fjob%2Fmaster%2F&style=flat-square)
 ![Jenkins Coverage](https://img.shields.io/jenkins/coverage/cobertura?jobUrl=https%3A%2F%2Fjenkins.deepak.science%2Fjob%2Fgitea-physics%2Fjob%2Fpdme%2Fjob%2Fmaster%2F&style=flat-square)
-![Maintenance](https://img.shields.io/maintenance/yes/2022?style=flat-square)
+![Maintenance](https://img.shields.io/maintenance/yes/2023?style=flat-square)
 
 This repo has library code for evaluating dipole models.
 
 ## Getting started
 
 `poetry install` to start locally
```

