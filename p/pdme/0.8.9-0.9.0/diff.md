# Comparing `tmp/pdme-0.8.9.tar.gz` & `tmp/pdme-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdme-0.8.9.tar", max compression
+gzip compressed data, was "pdme-0.9.0.tar", max compression
```

## Comparing `pdme-0.8.9.tar` & `pdme-0.9.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1229 2023-07-23 23:34:55.200875 pdme-0.8.9/README.md
--rw-r--r--   0        0        0      154 2023-07-23 23:34:55.204876 pdme-0.8.9/pdme/__init__.py
--rw-r--r--   0        0        0      184 2023-07-23 23:34:55.204876 pdme-0.8.9/pdme/inputs/__init__.py
--rw-r--r--   0        0        0      688 2023-07-23 23:34:55.204876 pdme-0.8.9/pdme/inputs/dot_inputs.py
--rw-r--r--   0        0        0      536 2023-07-23 23:34:55.204876 pdme-0.8.9/pdme/measurement/__init__.py
--rw-r--r--   0        0        0      984 2023-07-23 23:34:55.204876 pdme-0.8.9/pdme/measurement/dot_measure.py
--rw-r--r--   0        0        0     1224 2023-07-23 23:34:55.204876 pdme-0.8.9/pdme/measurement/dot_pair_measure.py
--rw-r--r--   0        0        0     1131 2023-07-23 23:34:55.204876 pdme-0.8.9/pdme/measurement/input_types.py
--rw-r--r--   0        0        0     5219 2023-07-23 23:34:55.204876 pdme-0.8.9/pdme/measurement/oscillating_dipole.py
--rw-r--r--   0        0        0       70 2023-07-23 23:34:55.204876 pdme-0.8.9/pdme/meta.py
--rw-r--r--   0        0        0     1066 2023-07-23 23:34:55.204876 pdme-0.8.9/pdme/model/__init__.py
--rw-r--r--   0        0        0     2367 2023-07-23 23:34:55.208876 pdme-0.8.9/pdme/model/fixed_magnitude_model.py
--rw-r--r--   0        0        0     4992 2023-07-23 23:34:55.208876 pdme-0.8.9/pdme/model/log_spaced_random_choice_fixed_orientation_model.py
--rw-r--r--   0        0        0     5332 2023-07-23 23:34:55.208876 pdme-0.8.9/pdme/model/log_spaced_random_choice_model.py
--rw-r--r--   0        0        0     4699 2023-07-23 23:34:55.208876 pdme-0.8.9/pdme/model/log_spaced_random_choice_xy_model.py
--rw-r--r--   0        0        0     3477 2023-07-23 23:34:55.208876 pdme-0.8.9/pdme/model/model.py
--rw-r--r--   0        0        0     2560 2023-07-23 23:34:55.208876 pdme-0.8.9/pdme/model/multidipole_fixed_magnitude_model.py
--rw-r--r--   0        0        0     3076 2023-07-23 23:34:55.208876 pdme-0.8.9/pdme/model/random_count_multidipole_fixed_magnitude_model.py
--rw-r--r--   0        0        0        0 2023-07-23 23:34:55.208876 pdme-0.8.9/pdme/py.typed
--rw-r--r--   0        0        0     1364 2023-07-23 23:34:55.208876 pdme-0.8.9/pdme/subspace_simulation/__init__.py
--rw-r--r--   0        0        0      590 2023-07-23 23:34:55.208876 pdme-0.8.9/pdme/subspace_simulation/mcmc_costs.py
--rw-r--r--   0        0        0        0 2023-07-23 23:34:55.208876 pdme-0.8.9/pdme/util/__init__.py
--rw-r--r--   0        0        0     2952 2023-07-23 23:34:55.208876 pdme-0.8.9/pdme/util/fast_nonlocal_spectrum.py
--rw-r--r--   0        0        0     3604 2023-07-23 23:34:55.208876 pdme-0.8.9/pdme/util/fast_v_calc.py
--rw-r--r--   0        0        0      860 2023-07-23 23:34:55.208876 pdme-0.8.9/pyproject.toml
--rw-r--r--   0        0        0     1972 2023-07-23 23:35:50.523858 pdme-0.8.9/setup.py
--rw-r--r--   0        0        0     1720 2023-07-23 23:35:50.524524 pdme-0.8.9/PKG-INFO
+-rw-r--r--   0        0        0     1229 2023-07-24 01:36:25.966958 pdme-0.9.0/README.md
+-rw-r--r--   0        0        0      154 2023-07-24 01:36:25.970958 pdme-0.9.0/pdme/__init__.py
+-rw-r--r--   0        0        0      184 2023-07-24 01:36:25.970958 pdme-0.9.0/pdme/inputs/__init__.py
+-rw-r--r--   0        0        0      688 2023-07-24 01:36:25.970958 pdme-0.9.0/pdme/inputs/dot_inputs.py
+-rw-r--r--   0        0        0      536 2023-07-24 01:36:25.970958 pdme-0.9.0/pdme/measurement/__init__.py
+-rw-r--r--   0        0        0      984 2023-07-24 01:36:25.970958 pdme-0.9.0/pdme/measurement/dot_measure.py
+-rw-r--r--   0        0        0     1224 2023-07-24 01:36:25.970958 pdme-0.9.0/pdme/measurement/dot_pair_measure.py
+-rw-r--r--   0        0        0     1131 2023-07-24 01:36:25.970958 pdme-0.9.0/pdme/measurement/input_types.py
+-rw-r--r--   0        0        0     5219 2023-07-24 01:36:25.970958 pdme-0.9.0/pdme/measurement/oscillating_dipole.py
+-rw-r--r--   0        0        0       70 2023-07-24 01:36:25.970958 pdme-0.9.0/pdme/meta.py
+-rw-r--r--   0        0        0     1066 2023-07-24 01:36:25.970958 pdme-0.9.0/pdme/model/__init__.py
+-rw-r--r--   0        0        0     2367 2023-07-24 01:36:25.970958 pdme-0.9.0/pdme/model/fixed_magnitude_model.py
+-rw-r--r--   0        0        0     4992 2023-07-24 01:36:25.970958 pdme-0.9.0/pdme/model/log_spaced_random_choice_fixed_orientation_model.py
+-rw-r--r--   0        0        0     5332 2023-07-24 01:36:25.970958 pdme-0.9.0/pdme/model/log_spaced_random_choice_model.py
+-rw-r--r--   0        0        0     4699 2023-07-24 01:36:25.970958 pdme-0.9.0/pdme/model/log_spaced_random_choice_xy_model.py
+-rw-r--r--   0        0        0     3462 2023-07-24 01:36:25.970958 pdme-0.9.0/pdme/model/model.py
+-rw-r--r--   0        0        0     2560 2023-07-24 01:36:25.970958 pdme-0.9.0/pdme/model/multidipole_fixed_magnitude_model.py
+-rw-r--r--   0        0        0     3076 2023-07-24 01:36:25.970958 pdme-0.9.0/pdme/model/random_count_multidipole_fixed_magnitude_model.py
+-rw-r--r--   0        0        0        0 2023-07-24 01:36:25.970958 pdme-0.9.0/pdme/py.typed
+-rw-r--r--   0        0        0     1364 2023-07-24 01:36:25.970958 pdme-0.9.0/pdme/subspace_simulation/__init__.py
+-rw-r--r--   0        0        0      590 2023-07-24 01:36:25.970958 pdme-0.9.0/pdme/subspace_simulation/mcmc_costs.py
+-rw-r--r--   0        0        0        0 2023-07-24 01:36:25.970958 pdme-0.9.0/pdme/util/__init__.py
+-rw-r--r--   0        0        0     2952 2023-07-24 01:36:25.970958 pdme-0.9.0/pdme/util/fast_nonlocal_spectrum.py
+-rw-r--r--   0        0        0     3604 2023-07-24 01:36:25.970958 pdme-0.9.0/pdme/util/fast_v_calc.py
+-rw-r--r--   0        0        0      860 2023-07-24 01:36:25.974958 pdme-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1972 2023-07-24 01:37:26.877416 pdme-0.9.0/setup.py
+-rw-r--r--   0        0        0     1720 2023-07-24 01:37:26.877758 pdme-0.9.0/PKG-INFO
```

### Comparing `pdme-0.8.9/README.md` & `pdme-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pdme-0.8.9/pdme/inputs/dot_inputs.py` & `pdme-0.9.0/pdme/inputs/dot_inputs.py`

 * *Files identical despite different names*

### Comparing `pdme-0.8.9/pdme/measurement/__init__.py` & `pdme-0.9.0/pdme/measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `pdme-0.8.9/pdme/measurement/dot_measure.py` & `pdme-0.9.0/pdme/measurement/dot_measure.py`

 * *Files identical despite different names*

### Comparing `pdme-0.8.9/pdme/measurement/dot_pair_measure.py` & `pdme-0.9.0/pdme/measurement/dot_pair_measure.py`

 * *Files identical despite different names*

### Comparing `pdme-0.8.9/pdme/measurement/input_types.py` & `pdme-0.9.0/pdme/measurement/input_types.py`

 * *Files identical despite different names*

### Comparing `pdme-0.8.9/pdme/measurement/oscillating_dipole.py` & `pdme-0.9.0/pdme/measurement/oscillating_dipole.py`

 * *Files identical despite different names*

### Comparing `pdme-0.8.9/pdme/model/__init__.py` & `pdme-0.9.0/pdme/model/__init__.py`

 * *Files identical despite different names*

### Comparing `pdme-0.8.9/pdme/model/fixed_magnitude_model.py` & `pdme-0.9.0/pdme/model/fixed_magnitude_model.py`

 * *Files identical despite different names*

### Comparing `pdme-0.8.9/pdme/model/log_spaced_random_choice_fixed_orientation_model.py` & `pdme-0.9.0/pdme/model/log_spaced_random_choice_fixed_orientation_model.py`

 * *Files identical despite different names*

### Comparing `pdme-0.8.9/pdme/model/log_spaced_random_choice_model.py` & `pdme-0.9.0/pdme/model/log_spaced_random_choice_model.py`

 * *Files identical despite different names*

### Comparing `pdme-0.8.9/pdme/model/log_spaced_random_choice_xy_model.py` & `pdme-0.9.0/pdme/model/log_spaced_random_choice_xy_model.py`

 * *Files identical despite different names*

### Comparing `pdme-0.8.9/pdme/model/model.py` & `pdme-0.9.0/pdme/model/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 		raise NotImplementedError
 
 	def get_mcmc_chain(
 		self,
 		seed,
 		cost_function,
 		chain_length,
+		threshold_cost: float,
 		stdevs: pdme.subspace_simulation.MCMCStandardDeviation,
 		initial_cost: Optional[float] = None,
 		rng_arg: Optional[numpy.random.Generator] = None,
 	) -> List[Tuple[float, numpy.ndarray]]:
 		"""
 		performs constrained markov chain monte carlo starting on seed parameter.
 		The cost function given is used as a constrained to condition the chain;
@@ -69,31 +70,30 @@
 		"""
 		_logger.debug(
 			f"Starting Markov Chain Monte Carlo with seed: {seed} for chain length {chain_length} and provided stdevs {stdevs}"
 		)
 		chain: List[Tuple[float, numpy.ndarray]] = []
 		current = seed
 		if initial_cost is None:
-			cost_to_compare = cost_function(current)
+			current_cost = cost_function(current)
 		else:
-			cost_to_compare = initial_cost
-		current_cost = cost_to_compare
+			current_cost = initial_cost
 		for i in range(chain_length):
 			dips = []
 			for dipole_index, dipole in enumerate(current):
 				stdev = stdevs[dipole_index]
 				tentative_dip = self.markov_chain_monte_carlo_proposal(
 					dipole, stdev, rng_arg
 				)
 
 				dips.append(tentative_dip)
 			dips_array = pdme.subspace_simulation.sort_array_of_dipoles_by_frequency(
 				dips
 			)
 			tentative_cost = cost_function(dips_array)
-			if tentative_cost < cost_to_compare:
+			if tentative_cost < threshold_cost:
 				chain.append((tentative_cost, dips_array))
 				current = dips_array
 				current_cost = tentative_cost
 			else:
 				chain.append((current_cost, current))
 		return chain
```

### Comparing `pdme-0.8.9/pdme/model/multidipole_fixed_magnitude_model.py` & `pdme-0.9.0/pdme/model/multidipole_fixed_magnitude_model.py`

 * *Files identical despite different names*

### Comparing `pdme-0.8.9/pdme/model/random_count_multidipole_fixed_magnitude_model.py` & `pdme-0.9.0/pdme/model/random_count_multidipole_fixed_magnitude_model.py`

 * *Files identical despite different names*

### Comparing `pdme-0.8.9/pdme/subspace_simulation/__init__.py` & `pdme-0.9.0/pdme/subspace_simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `pdme-0.8.9/pdme/subspace_simulation/mcmc_costs.py` & `pdme-0.9.0/pdme/subspace_simulation/mcmc_costs.py`

 * *Files identical despite different names*

### Comparing `pdme-0.8.9/pdme/util/fast_nonlocal_spectrum.py` & `pdme-0.9.0/pdme/util/fast_nonlocal_spectrum.py`

 * *Files identical despite different names*

### Comparing `pdme-0.8.9/pdme/util/fast_v_calc.py` & `pdme-0.9.0/pdme/util/fast_v_calc.py`

 * *Files identical despite different names*

### Comparing `pdme-0.8.9/pyproject.toml` & `pdme-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdme"
-version = "0.8.9"
+version = "0.9.0"
 description = "Python dipole model evaluator"
 authors = ["Deepak <dmallubhotla+github@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.10"
```

### Comparing `pdme-0.8.9/setup.py` & `pdme-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 {'': ['*']}
 
 install_requires = \
 ['numpy>=1.22.3,<2.0.0', 'scipy>=1.10,<1.11']
 
 setup_kwargs = {
     'name': 'pdme',
-    'version': '0.8.9',
+    'version': '0.9.0',
     'description': 'Python dipole model evaluator',
     'long_description': '# pdme - the python dipole model evaluator\n\n[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-green.svg?style=flat-square)](https://conventionalcommits.org)\n[![PyPI](https://img.shields.io/pypi/v/pdme?style=flat-square)](https://pypi.org/project/pdme/)\n[![Jenkins](https://img.shields.io/jenkins/build?jobUrl=https%3A%2F%2Fjenkins.deepak.science%2Fjob%2Fgitea-physics%2Fjob%2Fpdme%2Fjob%2Fmaster&style=flat-square)](https://jenkins.deepak.science/job/gitea-physics/job/pdme/job/master/)\n![Jenkins tests](https://img.shields.io/jenkins/tests?compact_message&jobUrl=https%3A%2F%2Fjenkins.deepak.science%2Fjob%2Fgitea-physics%2Fjob%2Fpdme%2Fjob%2Fmaster%2F&style=flat-square)\n![Jenkins Coverage](https://img.shields.io/jenkins/coverage/cobertura?jobUrl=https%3A%2F%2Fjenkins.deepak.science%2Fjob%2Fgitea-physics%2Fjob%2Fpdme%2Fjob%2Fmaster%2F&style=flat-square)\n![Maintenance](https://img.shields.io/maintenance/yes/2023?style=flat-square)\n\nThis repo has library code for evaluating dipole models.\n\n## Getting started\n\n`poetry install` to start locally\n\nCommit using [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/), and when commits are on master, release with `doo release`.\n',
     'author': 'Deepak',
     'author_email': 'dmallubhotla+github@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `pdme-0.8.9/PKG-INFO` & `pdme-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdme
-Version: 0.8.9
+Version: 0.9.0
 Summary: Python dipole model evaluator
 License: GPL-3.0-only
 Author: Deepak
 Author-email: dmallubhotla+github@gmail.com
 Requires-Python: >=3.8.1,<3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

