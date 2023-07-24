# Comparing `tmp/deepdog-0.7.1.tar.gz` & `tmp/deepdog-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepdog-0.7.1.tar", max compression
+gzip compressed data, was "deepdog-0.7.2.tar", max compression
```

## Comparing `deepdog-0.7.1.tar` & `deepdog-0.7.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      605 2023-07-24 07:05:18.226134 deepdog-0.7.1/deepdog/__init__.py
--rw-r--r--   0        0        0     8197 2023-07-24 07:05:18.226134 deepdog-0.7.1/deepdog/bayes_run.py
--rw-r--r--   0        0        0    11705 2023-07-24 07:05:18.226134 deepdog-0.7.1/deepdog/bayes_run_simulpairs.py
--rw-r--r--   0        0        0     6623 2023-07-24 07:05:18.226134 deepdog-0.7.1/deepdog/bayes_run_with_ss.py
--rw-r--r--   0        0        0       73 2023-07-24 07:05:18.226134 deepdog-0.7.1/deepdog/meta.py
--rw-r--r--   0        0        0     8471 2023-07-24 07:05:18.226134 deepdog-0.7.1/deepdog/real_spectrum_run.py
--rw-r--r--   0        0        0      110 2023-07-24 07:05:18.226134 deepdog-0.7.1/deepdog/subset_simulation/__init__.py
--rw-r--r--   0        0        0     8754 2023-07-24 07:05:18.230134 deepdog-0.7.1/deepdog/subset_simulation/subset_simulation_impl.py
--rw-r--r--   0        0        0     6794 2023-07-24 07:05:18.230134 deepdog-0.7.1/deepdog/temp_aware_real_spectrum_run.py
--rw-r--r--   0        0        0      898 2023-07-24 07:05:18.230134 deepdog-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      662 2023-07-24 07:06:20.769951 deepdog-0.7.1/setup.py
--rw-r--r--   0        0        0      361 2023-07-24 07:06:20.770362 deepdog-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0      605 2023-07-24 15:47:03.783448 deepdog-0.7.2/deepdog/__init__.py
+-rw-r--r--   0        0        0     8197 2023-07-24 15:47:03.783448 deepdog-0.7.2/deepdog/bayes_run.py
+-rw-r--r--   0        0        0    11705 2023-07-24 15:47:03.783448 deepdog-0.7.2/deepdog/bayes_run_simulpairs.py
+-rw-r--r--   0        0        0     6778 2023-07-24 15:47:03.783448 deepdog-0.7.2/deepdog/bayes_run_with_ss.py
+-rw-r--r--   0        0        0       73 2023-07-24 15:47:03.783448 deepdog-0.7.2/deepdog/meta.py
+-rw-r--r--   0        0        0     8471 2023-07-24 15:47:03.783448 deepdog-0.7.2/deepdog/real_spectrum_run.py
+-rw-r--r--   0        0        0      110 2023-07-24 15:47:03.787449 deepdog-0.7.2/deepdog/subset_simulation/__init__.py
+-rw-r--r--   0        0        0     8754 2023-07-24 15:47:03.787449 deepdog-0.7.2/deepdog/subset_simulation/subset_simulation_impl.py
+-rw-r--r--   0        0        0     6794 2023-07-24 15:47:03.787449 deepdog-0.7.2/deepdog/temp_aware_real_spectrum_run.py
+-rw-r--r--   0        0        0      898 2023-07-24 15:47:03.787449 deepdog-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0      662 2023-07-24 15:48:06.191608 deepdog-0.7.2/setup.py
+-rw-r--r--   0        0        0      361 2023-07-24 15:48:06.191916 deepdog-0.7.2/PKG-INFO
```

### Comparing `deepdog-0.7.1/deepdog/__init__.py` & `deepdog-0.7.2/deepdog/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.7.1/deepdog/bayes_run.py` & `deepdog-0.7.2/deepdog/bayes_run.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.7.1/deepdog/bayes_run_simulpairs.py` & `deepdog-0.7.2/deepdog/bayes_run_simulpairs.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.7.1/deepdog/bayes_run_with_ss.py` & `deepdog-0.7.2/deepdog/bayes_run_with_ss.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 # TODO: remove hardcode
 CHUNKSIZE = 50
 
 # TODO: It's garbage to have this here duplicated from pdme.
 DotInput = Tuple[numpy.typing.ArrayLike, float]
 
 
+CLAMPING_FACTOR = 10
+
 _logger = logging.getLogger(__name__)
 
 
 class BayesRunWithSubspaceSimulation:
 	"""
 	A single Bayes run for a given set of dots.
 
@@ -189,18 +191,20 @@
 					_logger.info(f"Not writing anymore, saw end after {i}")
 					break
 
 			likelihoods: List[float] = []
 
 			for (name, result) in zip(self.model_names, results):
 				if result.over_target_likelihood is None:
-					_logger.error("got a none result, bye")
-					return
-				likelihoods.append(result.over_target_likelihood)
-				row[f"{name}_likelihood"] = result.over_target_likelihood
+					clamped_likelihood = result.probs_list[-1][0] / CLAMPING_FACTOR
+					_logger.warning(f"got a none result, clamping to {clamped_likelihood}")
+				else:
+					clamped_likelihood = result.over_target_likelihood
+				likelihoods.append(clamped_likelihood)
+				row[f"{name}_likelihood"] = clamped_likelihood
 
 			success_weight = sum(
 				[
 					likelihood * prob
 					for likelihood, prob in zip(likelihoods, self.probabilities)
 				]
 			)
```

### Comparing `deepdog-0.7.1/deepdog/real_spectrum_run.py` & `deepdog-0.7.2/deepdog/real_spectrum_run.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.7.1/deepdog/subset_simulation/subset_simulation_impl.py` & `deepdog-0.7.2/deepdog/subset_simulation/subset_simulation_impl.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.7.1/deepdog/temp_aware_real_spectrum_run.py` & `deepdog-0.7.2/deepdog/temp_aware_real_spectrum_run.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.7.1/pyproject.toml` & `deepdog-0.7.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deepdog"
-version = "0.7.1"
+version = "0.7.2"
 description = ""
 authors = ["Deepak Mallubhotla <dmallubhotla+github@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.10"
 pdme = "^0.9.1"
 numpy = "1.22.3"
```

### Comparing `deepdog-0.7.1/setup.py` & `deepdog-0.7.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['numpy==1.22.3', 'pdme>=0.9.1,<0.10.0', 'scipy==1.10']
 
 setup_kwargs = {
     'name': 'deepdog',
-    'version': '0.7.1',
+    'version': '0.7.2',
     'description': '',
     'long_description': None,
     'author': 'Deepak Mallubhotla',
     'author_email': 'dmallubhotla+github@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

