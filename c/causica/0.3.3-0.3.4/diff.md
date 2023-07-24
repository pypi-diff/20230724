# Comparing `tmp/causica-0.3.3.tar.gz` & `tmp/causica-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causica-0.3.3.tar", max compression
+gzip compressed data, was "causica-0.3.4.tar", max compression
```

## Comparing `causica-0.3.3.tar` & `causica-0.3.4.tar`

### file list

```diff
@@ -1,67 +1,68 @@
--rw-r--r--   0        0        0     1141 2023-06-26 14:58:36.920302 causica-0.3.3/LICENSE
--rw-r--r--   0        0        0     7092 2023-06-26 14:58:36.920302 causica-0.3.3/README.md
--rw-r--r--   0        0        0      746 2023-06-27 09:25:26.129804 causica-0.3.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/__init__.py
--rw-r--r--   0        0        0      172 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/config/lightning/default_data.yaml
--rw-r--r--   0        0        0     1222 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/config/lightning/default_gaussian.yaml
--rw-r--r--   0        0        0     1220 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/config/lightning/default_spline.yaml
--rw-r--r--   0        0        0        0 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/datasets/__init__.py
--rw-r--r--   0        0        0    13602 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/datasets/causica_dataset_format.py
--rw-r--r--   0        0        0     2642 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/datasets/interventional_data.py
--rw-r--r--   0        0        0     1230 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/datasets/loaded_expert_graph_container.py
--rw-r--r--   0        0        0     2454 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/datasets/standardizer.py
--rw-r--r--   0        0        0     1959 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/datasets/tensordict_utils.py
--rw-r--r--   0        0        0      307 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/datasets/variable_types.py
--rw-r--r--   0        0        0      801 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/distributions/__init__.py
--rw-r--r--   0        0        0      613 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/distributions/adjacency/__init__.py
--rw-r--r--   0        0        0     3600 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/distributions/adjacency/adjacency_distributions.py
--rw-r--r--   0        0        0     8635 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/distributions/adjacency/constrained_adjacency_distributions.py
--rw-r--r--   0        0        0     3442 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/distributions/adjacency/directed_acyclic.py
--rw-r--r--   0        0        0     8118 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/distributions/adjacency/enco.py
--rw-r--r--   0        0        0     4125 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/distributions/adjacency/gibbs_dag_prior.py
--rw-r--r--   0        0        0     4897 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/distributions/adjacency/three_way.py
--rw-r--r--   0        0        0      773 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/distributions/distribution_module.py
--rw-r--r--   0        0        0      649 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/distributions/gumbel_binary.py
--rw-r--r--   0        0        0      595 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/distributions/noise/__init__.py
--rw-r--r--   0        0        0     3631 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/distributions/noise/bernoulli.py
--rw-r--r--   0        0        0     3222 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/distributions/noise/categorical.py
--rw-r--r--   0        0        0     7593 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/distributions/noise/joint.py
--rw-r--r--   0        0        0     3389 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/distributions/noise/noise.py
--rw-r--r--   0        0        0      112 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/distributions/noise/spline/__init__.py
--rw-r--r--   0        0        0     6474 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/distributions/noise/spline/bayesiains_nsf_rqs.py
--rw-r--r--   0        0        0     4340 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/distributions/noise/spline/rational_quadratic_transform.py
--rw-r--r--   0        0        0     8024 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/distributions/noise/spline/spline.py
--rw-r--r--   0        0        0     1736 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/distributions/noise/univariate_normal.py
--rw-r--r--   0        0        0     5651 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/distributions/transforms.py
--rw-r--r--   0        0        0      516 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/fsspec_helpers.py
--rw-r--r--   0        0        0      264 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/functional_relationships/__init__.py
--rw-r--r--   0        0        0     4591 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/functional_relationships/do_functional_relationships.py
--rw-r--r--   0        0        0     1559 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/functional_relationships/functional_relationships.py
--rw-r--r--   0        0        0     9076 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/functional_relationships/icgnn.py
--rw-r--r--   0        0        0     2649 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/functional_relationships/linear_functional_relationships.py
--rw-r--r--   0        0        0        0 2023-06-26 14:58:36.930302 causica-0.3.3/src/causica/graph/__init__.py
--rw-r--r--   0        0        0      375 2023-06-26 14:58:36.930302 causica-0.3.3/src/causica/graph/dag_constraint.py
--rw-r--r--   0        0        0     2711 2023-06-26 14:58:36.930302 causica-0.3.3/src/causica/graph/evaluation_metrics.py
--rw-r--r--   0        0        0        0 2023-06-26 14:58:36.930302 causica-0.3.3/src/causica/lightning/__init__.py
--rw-r--r--   0        0        0     3954 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/lightning/callbacks.py
--rw-r--r--   0        0        0      748 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/lightning/cli.py
--rw-r--r--   0        0        0        0 2023-06-26 14:58:36.930302 causica-0.3.3/src/causica/lightning/data_modules/__init__.py
--rw-r--r--   0        0        0     3052 2023-06-26 14:58:36.930302 causica-0.3.3/src/causica/lightning/data_modules/basic_data_module.py
--rw-r--r--   0        0        0     1143 2023-06-26 14:58:36.930302 causica-0.3.3/src/causica/lightning/data_modules/deci_data_module.py
--rw-r--r--   0        0        0     7778 2023-06-26 14:58:36.930302 causica-0.3.3/src/causica/lightning/data_modules/variable_spec_data.py
--rw-r--r--   0        0        0     2098 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/lightning/loggers.py
--rw-r--r--   0        0        0      776 2023-06-26 14:58:36.930302 causica-0.3.3/src/causica/lightning/main.py
--rw-r--r--   0        0        0        0 2023-06-26 14:58:36.930302 causica-0.3.3/src/causica/lightning/modules/__init__.py
--rw-r--r--   0        0        0    12157 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/lightning/modules/deci_module.py
--rw-r--r--   0        0        0     2088 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/lightning/modules/variable_spec_module.py
--rw-r--r--   0        0        0     1289 2023-06-26 14:58:36.930302 causica-0.3.3/src/causica/mlflow_helpers.py
--rw-r--r--   0        0        0        0 2023-06-26 14:58:36.930302 causica-0.3.3/src/causica/sem/__init__.py
--rw-r--r--   0        0        0     3711 2023-06-26 14:58:36.930302 causica-0.3.3/src/causica/sem/distribution_parameters_sem.py
--rw-r--r--   0        0        0     4058 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/sem/sem_distribution.py
--rw-r--r--   0        0        0     6277 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/sem/structural_equation_model.py
--rw-r--r--   0        0        0        0 2023-06-26 14:58:36.930302 causica-0.3.3/src/causica/training/__init__.py
--rw-r--r--   0        0        0    11827 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/training/auglag.py
--rw-r--r--   0        0        0     5286 2023-06-26 14:58:36.930302 causica-0.3.3/src/causica/training/evaluation.py
--rw-r--r--   0        0        0     8958 2023-06-26 14:58:36.930302 causica-0.3.3/src/causica/training/per_variable_metrics.py
--rw-r--r--   0        0        0     1725 2023-06-26 14:58:36.930302 causica-0.3.3/src/causica/triangular_transformations.py
--rw-r--r--   0        0        0     7905 1970-01-01 00:00:00.000000 causica-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1141 2023-07-22 07:16:32.324461 causica-0.3.4/LICENSE
+-rw-r--r--   0        0        0     7092 2023-07-22 07:16:32.324461 causica-0.3.4/README.md
+-rw-r--r--   0        0        0      695 2023-07-24 12:06:48.822883 causica-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/__init__.py
+-rw-r--r--   0        0        0      172 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/config/lightning/default_data.yaml
+-rw-r--r--   0        0        0     1222 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/config/lightning/default_gaussian.yaml
+-rw-r--r--   0        0        0     1220 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/config/lightning/default_spline.yaml
+-rw-r--r--   0        0        0        0 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/datasets/__init__.py
+-rw-r--r--   0        0        0    14326 2023-07-24 12:06:48.822883 causica-0.3.4/src/causica/datasets/causica_dataset_format.py
+-rw-r--r--   0        0        0     2642 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/datasets/interventional_data.py
+-rw-r--r--   0        0        0     1230 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/datasets/loaded_expert_graph_container.py
+-rw-r--r--   0        0        0     2504 2023-07-24 12:06:48.822883 causica-0.3.4/src/causica/datasets/standardizer.py
+-rw-r--r--   0        0        0     6869 2023-07-24 12:06:48.822883 causica-0.3.4/src/causica/datasets/tensordict_utils.py
+-rw-r--r--   0        0        0      307 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/datasets/variable_types.py
+-rw-r--r--   0        0        0      801 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/distributions/__init__.py
+-rw-r--r--   0        0        0      613 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/distributions/adjacency/__init__.py
+-rw-r--r--   0        0        0     3600 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/distributions/adjacency/adjacency_distributions.py
+-rw-r--r--   0        0        0     8635 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/distributions/adjacency/constrained_adjacency_distributions.py
+-rw-r--r--   0        0        0     3442 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/distributions/adjacency/directed_acyclic.py
+-rw-r--r--   0        0        0     8118 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/distributions/adjacency/enco.py
+-rw-r--r--   0        0        0     4125 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/distributions/adjacency/gibbs_dag_prior.py
+-rw-r--r--   0        0        0     4897 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/distributions/adjacency/three_way.py
+-rw-r--r--   0        0        0      773 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/distributions/distribution_module.py
+-rw-r--r--   0        0        0      649 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/distributions/gumbel_binary.py
+-rw-r--r--   0        0        0      595 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/distributions/noise/__init__.py
+-rw-r--r--   0        0        0     3631 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/distributions/noise/bernoulli.py
+-rw-r--r--   0        0        0     3222 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/distributions/noise/categorical.py
+-rw-r--r--   0        0        0     7653 2023-07-24 12:06:48.822883 causica-0.3.4/src/causica/distributions/noise/joint.py
+-rw-r--r--   0        0        0     3389 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/distributions/noise/noise.py
+-rw-r--r--   0        0        0      112 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/distributions/noise/spline/__init__.py
+-rw-r--r--   0        0        0     6474 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/distributions/noise/spline/bayesiains_nsf_rqs.py
+-rw-r--r--   0        0        0     4340 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/distributions/noise/spline/rational_quadratic_transform.py
+-rw-r--r--   0        0        0     8024 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/distributions/noise/spline/spline.py
+-rw-r--r--   0        0        0     1754 2023-07-24 12:06:48.822883 causica-0.3.4/src/causica/distributions/noise/univariate_normal.py
+-rw-r--r--   0        0        0     5557 2023-07-24 12:06:48.822883 causica-0.3.4/src/causica/distributions/transforms.py
+-rw-r--r--   0        0        0      516 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/fsspec_helpers.py
+-rw-r--r--   0        0        0      264 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/functional_relationships/__init__.py
+-rw-r--r--   0        0        0     4591 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/functional_relationships/do_functional_relationships.py
+-rw-r--r--   0        0        0     1559 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/functional_relationships/functional_relationships.py
+-rw-r--r--   0        0        0     9076 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/functional_relationships/icgnn.py
+-rw-r--r--   0        0        0     2649 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/functional_relationships/linear_functional_relationships.py
+-rw-r--r--   0        0        0        0 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/graph/__init__.py
+-rw-r--r--   0        0        0      375 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/graph/dag_constraint.py
+-rw-r--r--   0        0        0     2711 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/graph/evaluation_metrics.py
+-rw-r--r--   0        0        0        0 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/lightning/__init__.py
+-rw-r--r--   0        0        0     3954 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/lightning/callbacks.py
+-rw-r--r--   0        0        0      748 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/lightning/cli.py
+-rw-r--r--   0        0        0        0 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/lightning/data_modules/__init__.py
+-rw-r--r--   0        0        0     2889 2023-07-24 12:06:48.822883 causica-0.3.4/src/causica/lightning/data_modules/basic_data_module.py
+-rw-r--r--   0        0        0     1143 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/lightning/data_modules/deci_data_module.py
+-rw-r--r--   0        0        0     8314 2023-07-24 12:06:48.822883 causica-0.3.4/src/causica/lightning/data_modules/variable_spec_data.py
+-rw-r--r--   0        0        0     2098 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/lightning/loggers.py
+-rw-r--r--   0        0        0      776 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/lightning/main.py
+-rw-r--r--   0        0        0        0 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/lightning/modules/__init__.py
+-rw-r--r--   0        0        0    12127 2023-07-24 12:06:48.822883 causica-0.3.4/src/causica/lightning/modules/deci_module.py
+-rw-r--r--   0        0        0     2088 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/lightning/modules/variable_spec_module.py
+-rw-r--r--   0        0        0     1289 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/mlflow_helpers.py
+-rw-r--r--   0        0        0        0 2023-07-24 12:06:48.822883 causica-0.3.4/src/causica/py.typed
+-rw-r--r--   0        0        0        0 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/sem/__init__.py
+-rw-r--r--   0        0        0     3711 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/sem/distribution_parameters_sem.py
+-rw-r--r--   0        0        0     4247 2023-07-24 12:06:48.822883 causica-0.3.4/src/causica/sem/sem_distribution.py
+-rw-r--r--   0        0        0     6295 2023-07-24 12:06:48.822883 causica-0.3.4/src/causica/sem/structural_equation_model.py
+-rw-r--r--   0        0        0        0 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/training/__init__.py
+-rw-r--r--   0        0        0    11827 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/training/auglag.py
+-rw-r--r--   0        0        0     5286 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/training/evaluation.py
+-rw-r--r--   0        0        0    11285 2023-07-24 12:06:48.822883 causica-0.3.4/src/causica/training/per_variable_metrics.py
+-rw-r--r--   0        0        0     1725 2023-07-22 07:16:32.334461 causica-0.3.4/src/causica/triangular_transformations.py
+-rw-r--r--   0        0        0     7865 1970-01-01 00:00:00.000000 causica-0.3.4/PKG-INFO
```

### Comparing `causica-0.3.3/LICENSE` & `causica-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `causica-0.3.3/README.md` & `causica-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `causica-0.3.3/pyproject.toml` & `causica-0.3.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "causica"
-version = "0.3.3"
+version = "0.3.4"
 description = ""
 readme = "README.md"
 authors = []
 packages = [
     { include = "causica", from = "src" }
 ]
 license = "MIT"
@@ -18,15 +18,14 @@
 tensorboard = "^2.9.0"
 pytorch-lightning = {version = "^1.9.0", extras= ["extra"]}
 jsonargparse = "<4.21.0"  # 4.21.0 breaks lightning cli
 dataclasses-json = "^0.5.7"
 types-PyYAML = "^6.0.12.2"
 tensordict = "^0.1.0"
 torch = "2.0.0"
-numba = "^0.56.0"  # needed to make the build work
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 pytest-cov = "^3.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `causica-0.3.3/src/causica/config/lightning/default_gaussian.yaml` & `causica-0.3.4/src/causica/config/lightning/default_gaussian.yaml`

 * *Files identical despite different names*

### Comparing `causica-0.3.3/src/causica/config/lightning/default_spline.yaml` & `causica-0.3.4/src/causica/config/lightning/default_spline.yaml`

 * *Files identical despite different names*

### Comparing `causica-0.3.3/src/causica/datasets/causica_dataset_format.py` & `causica-0.3.4/src/causica/datasets/causica_dataset_format.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 """
 A module to load data from the standard directory structure (i.e. the one followed by csuite)
 """
 import json
 import logging
 import os
+from collections import defaultdict
+from dataclasses import dataclass
 from enum import Enum
 from functools import partial
 from typing import Any, Counter, Optional
 
 import fsspec
 import numpy as np
 import torch
+from dataclasses_json import dataclass_json
 from tensordict import TensorDict
 
 from causica.datasets.interventional_data import CounterfactualData, InterventionData
 from causica.datasets.tensordict_utils import convert_one_hot
 from causica.datasets.variable_types import DTYPE_MAP, VariableTypeEnum
 
-CSUITE_DATASETS_PATH = "https://azuastoragepublic.blob.core.windows.net/datasets"
+CAUSICA_DATASETS_PATH = "https://azuastoragepublic.z6.web.core.windows.net/"
 
 
 InterventionWithEffects = tuple[InterventionData, InterventionData, set[str]]
 CounterfactualWithEffects = tuple[CounterfactualData, Optional[CounterfactualData], set[str]]
 
 logger = logging.getLogger(__name__)
 
@@ -31,41 +34,55 @@
     TEST = "test.csv"
     INTERVENTIONS = "interventions.json"
     COUNTERFACTUALS = "counterfactuals.json"
     TRUE_ADJACENCY = "adj_matrix.csv"
     VARIABLES_JSON = "variables.json"
 
 
-def convert_variable_types_to_enum(variable_metadata: dict[str, Any]):
-    # Convert the types to the enum
-    for variable in variable_metadata["variables"]:
-        variable["type"] = VariableTypeEnum(variable["type"])
+@dataclass_json
+@dataclass(frozen=True)
+class Variable:
+    """Class to represent a variable in the variables metadata json object.
 
-    return variable_metadata
+    Args:
+        group_name: The name of the group the variable belongs to.
+        name: The name of the variable.
+        type: The type of the variable.
+        lower: The lower bound of the variable (if it is continuous).
+        upper: The upper bound of the variable (if it is continuous).
+        always_observed: Whether the variable is always observed.
+    """
 
+    group_name: str
+    name: str
+    type: VariableTypeEnum = VariableTypeEnum.CONTINUOUS
+    lower: Optional[float] = None
+    upper: Optional[float] = None
+    always_observed: bool = True
 
-def convert_enum_to_variable_types(variable_metadata: dict[str, Any]):
-    # Convert enum to types
-    for variable in variable_metadata["variables"]:
-        variable["type"] = VariableTypeEnum(variable["type"]).value
 
-    return variable_metadata
+@dataclass_json
+@dataclass(frozen=True)
+class VariablesMetadata:
+    """Class to represent the variables metadata json object."""
+
+    variables: list[Variable]
 
 
 def load_data(
     root_path: str,
     data_enum: DataEnum,
-    variables_metadata: Optional[dict[str, Any]] = None,
+    variables_metadata: Optional[VariablesMetadata] = None,
     **storage_options: dict[str, Any],
 ):
     """
     Load the Data from the location, dataset name and type of data.
 
     Args:
-        root_path: The root path to the Data e.g. `CSUITE_DATASETS_PATH/csuite_linexp_2`
+        root_path: The root path to the Data e.g. `CAUSICA_DATASETS_PATH/csuite_linexp_2`
         data_enum: The type of dataset for which to return the path
         variables_metadata: Optional variables object (to save downloading it multiple times)
         **storage_options: Keyword args passed to `fsspec.open`
     Return:
         The downloaded data (the type depends on the data requested)
     """
 
@@ -79,53 +96,51 @@
         with fsspec_open(path_name) as f:
             return torch.tensor(np.loadtxt(f, dtype=int, delimiter=","))
 
     if data_enum == DataEnum.VARIABLES_JSON:
         if variables_metadata is not None:
             raise ValueError("Variables metadata was supplied and requested")
         with fsspec_open(path_name) as f:
-            return convert_variable_types_to_enum(json.load(f))
+            return VariablesMetadata.from_json(f.read())  # type: ignore
 
     if variables_metadata is None:
         variables_metadata = load_data(root_path, data_enum=DataEnum.VARIABLES_JSON)
 
     with fsspec_open(path_name) as f:
         match data_enum:
             case (DataEnum.TRAIN | DataEnum.TEST):
                 arr = np.loadtxt(f, delimiter=",")
-                categorical_sizes = _get_categorical_sizes(variables_list=variables_metadata["variables"])
+                categorical_sizes = _get_categorical_sizes(variables_list=variables_metadata.variables)
                 return convert_one_hot(
-                    tensordict_from_variables_metadata(arr, variables_metadata["variables"]),
+                    tensordict_from_variables_metadata(arr, variables_metadata.variables),
                     one_hot_sizes=categorical_sizes,
                 )
             case DataEnum.INTERVENTIONS:
                 return _load_interventions(json_object=json.load(f), metadata=variables_metadata)
             case DataEnum.COUNTERFACTUALS:
                 return _load_counterfactuals(json_object=json.load(f), metadata=variables_metadata)
 
         raise RuntimeError("Unrecognized data type")
 
 
-def _load_interventions(json_object: dict[str, Any], metadata: dict[str, Any]) -> list[InterventionWithEffects]:
+def _load_interventions(json_object: dict[str, Any], metadata: VariablesMetadata) -> list[InterventionWithEffects]:
     """
     Load the Interventional Datasets as a list of interventions/counterfactuals.
 
     Args:
         json_object: The .json file loaded as a json object.
         metadata: Metadata of the dataset containing names and types.
 
     Returns:
         A list of interventions and the nodes we want to observe for each
     """
-    variables_list = metadata["variables"]
-
     intervened_column_to_group_name: dict[int, str] = dict(
         zip(
             json_object["metadata"]["columns_to_nodes"],
-            list(item["group_name"] for item in variables_list),
+            list(item.group_name for item in metadata.variables),
         )
     )
 
     interventions_list = []
     for environment in json_object["environments"]:
         conditioning_idxs = environment["conditioning_idxs"]
         if conditioning_idxs is None:
@@ -135,87 +150,85 @@
 
         intervention_nodes = [intervened_column_to_group_name[idx] for idx in environment["intervention_idxs"]]
 
         intervention = _to_intervention(
             np.array(environment["test_data"]),
             intervention_nodes=intervention_nodes,
             condition_nodes=condition_nodes,
-            variables_list=variables_list,
+            variables_list=metadata.variables,
         )
         # if the json has reference data create another intervention dataclass
         if (reference_data := environment["reference_data"]) is None:
             raise RuntimeError()
         reference = _to_intervention(
             np.array(reference_data),
             intervention_nodes=intervention_nodes,
             condition_nodes=condition_nodes,
-            variables_list=variables_list,
+            variables_list=metadata.variables,
         )
 
         # store the nodes we're interested in observing
         effect_nodes = set(intervened_column_to_group_name[idx] for idx in environment["effect_idxs"])
         # default to all nodes
         if not effect_nodes:
             effect_nodes = set(intervention.sampled_nodes)
         interventions_list.append((intervention, reference, effect_nodes))
     return interventions_list
 
 
-def _load_counterfactuals(json_object: dict[str, Any], metadata: dict[str, Any]) -> list[CounterfactualWithEffects]:
+def _load_counterfactuals(json_object: dict[str, Any], metadata: VariablesMetadata) -> list[CounterfactualWithEffects]:
     """
     Load the Interventional Datasets as a list of counterfactuals.
 
     Args:
         json_object: The .json file in loaded as a json object.
         metadata: Metadata of the dataset containing names and types.
 
     Returns:
         A list of counterfactuals and the nodes we want to observe for each
     """
-    variables_list = metadata["variables"]
-
     intervened_column_to_group_name: dict[int, str] = dict(
         zip(
             json_object["metadata"]["columns_to_nodes"],
-            list(item["group_name"] for item in variables_list),
+            list(item.group_name for item in metadata.variables),
         )
     )
 
     cf_list = []
     for environment in json_object["environments"]:
         factual_data = np.array(environment["conditioning_values"])
         intervention_nodes = [intervened_column_to_group_name[idx] for idx in environment["intervention_idxs"]]
         intervention = _to_counterfactual(
             np.array(environment["test_data"]),
             factual_data,
             intervention_nodes=intervention_nodes,
-            variables_list=variables_list,
+            variables_list=metadata.variables,
         )
         # if the json has reference data create another intervention dataclass
         if (reference_data := environment["reference_data"]) is None:
             reference = None
         else:
             reference = _to_counterfactual(
                 np.array(reference_data),
                 factual_data,
                 intervention_nodes=intervention_nodes,
-                variables_list=variables_list,
+                variables_list=metadata.variables,
             )
 
         # store the nodes we're interested in observing
         effect_nodes = set(intervened_column_to_group_name[idx] for idx in environment["effect_idxs"])
         # default to all nodes
         if not effect_nodes:
             effect_nodes = set(intervention.sampled_nodes)
         cf_list.append((intervention, reference, effect_nodes))
     return cf_list
 
 
 def _to_intervention(
-    data: np.ndarray, intervention_nodes: list[str], condition_nodes: list[str], variables_list: list[dict[str, Any]]
+    data: np.ndarray, intervention_nodes: list[str], condition_nodes: list[str], variables_list: list[Variable]
 ) -> InterventionData:
     """Create an `InterventionData` object from the data within the json file."""
     interv_data = tensordict_from_variables_metadata(data, variables_list=variables_list)
 
     # all the intervention values in the dataset should be the same, so we use the first row
     first_row = interv_data[0]
     assert all(torch.allclose(interv_data[node_name], first_row[node_name]) for node_name in intervention_nodes)
@@ -235,15 +248,15 @@
         ),
         intervention_data=convert_one_hot(interv_data, _intersect_dicts_left(categorical_sizes, interv_data)),
         condition_values=convert_one_hot(condition_values, _intersect_dicts_left(categorical_sizes, condition_values)),
     )
 
 
 def _to_counterfactual(
-    data: np.ndarray, base_data: np.ndarray, intervention_nodes: list[str], variables_list: list[dict[str, Any]]
+    data: np.ndarray, base_data: np.ndarray, intervention_nodes: list[str], variables_list: list[Variable]
 ) -> CounterfactualData:
     """Create an `CounterfactualData` object from the data within the json file."""
     interv_data = tensordict_from_variables_metadata(data, variables_list=variables_list)
     # all the intervention values in the dataset should be the same, so we use the first row
     first_row = interv_data[0]
     assert all(torch.allclose(interv_data[node_name], first_row[node_name]) for node_name in intervention_nodes)
     intervention_values = TensorDict(
@@ -258,39 +271,39 @@
             intervention_values, _intersect_dicts_left(categorical_sizes, intervention_values)
         ),
         counterfactual_data=convert_one_hot(interv_data, _intersect_dicts_left(categorical_sizes, interv_data)),
         factual_data=convert_one_hot(factual_data, _intersect_dicts_left(categorical_sizes, factual_data)),
     )
 
 
-def _get_categorical_sizes(variables_list: list[dict[str, Any]]) -> dict[str, int]:
+def _get_categorical_sizes(variables_list: list[Variable]) -> dict[str, int]:
     categorical_sizes = {}
     for item in variables_list:
-        if item["type"] == VariableTypeEnum.CATEGORICAL:
-            upper = item.get("upper")
-            lower = item.get("lower")
+        if item.type == VariableTypeEnum.CATEGORICAL:
+            upper = item.upper
+            lower = item.lower
             if upper is not None and lower is not None:
-                categorical_sizes[item["group_name"]] = item["upper"] - item["lower"] + 1
+                categorical_sizes[item.group_name] = int(upper - lower + 1)
             else:
                 assert upper is None and lower is None, "Please specify either both limits or neither"
-                categorical_sizes[item["group_name"]] = -1
+                categorical_sizes[item.group_name] = -1
     return categorical_sizes
 
 
-def tensordict_from_variables_metadata(data: np.ndarray, variables_list: list[dict[str, Any]]) -> TensorDict:
+def tensordict_from_variables_metadata(data: np.ndarray, variables_list: list[Variable]) -> TensorDict:
     """Returns a tensor created by concatenating all values along the last dim."""
     assert data.ndim == 2, "Numpy loading only supported for 2d data"
     batch_size = data.shape[0]
 
     # guaranteed to be ordered correctly in python 3.7+ https://docs.python.org/3/library/collections.html#collections.Counter
-    sizes = Counter(d["group_name"] for d in variables_list)  # get the dimensions of each key from the variables
+    sizes = Counter(d.group_name for d in variables_list)  # get the dimensions of each key from the variables
     assert sum(sizes.values()) == data.shape[1], "Variable sizes do not match data shape"
 
     # NOTE: This assumes that variables in the same group will have the same type.
-    dtypes = {item["group_name"]: DTYPE_MAP[item["type"]] for item in variables_list}
+    dtypes = {item.group_name: DTYPE_MAP[item.type] for item in variables_list}
 
     # slice the numpy array and assign the slices to the values of keys in the dictionary
     d = TensorDict({}, batch_size=batch_size)
     curr_idx = 0
     for key, length in sizes.items():
         d[key] = torch.Tensor(data[:, curr_idx : curr_idx + length]).to(dtype=dtypes[key])
         curr_idx += length
@@ -306,24 +319,33 @@
 
 
 def _intersect_dicts_left(dict_1: dict, dict_2: dict) -> dict:
     """Select the keys that are in both dictionaries, with values from the first."""
     return {key: dict_1[key] for key in dict_1.keys() & dict_2.keys()}
 
 
-def get_group_names(variables_dict: dict[str, Any]) -> list[str]:
+def get_group_names(variables_metadata: VariablesMetadata) -> list[str]:
     """Get the names of the groups in the variables dict."""
-    return list(dict.fromkeys([var["group_name"] for var in variables_dict["variables"]]))
+    return list(dict.fromkeys([var.group_name for var in variables_metadata.variables]))
 
 
-def get_group_idxs(variables_dict: dict[str, Any]) -> list[list[int]]:
+def get_group_idxs(variables_metadata: VariablesMetadata) -> list[list[int]]:
     """Get the indices of the nodes/groups in each group."""
-    group_names = get_group_names(variables_dict)
+    group_names = get_group_names(variables_metadata)
     return [
-        [idx for idx, var in enumerate(variables_dict["variables"]) if var["group_name"] == group_name]
+        [idx for idx, var in enumerate(variables_metadata.variables) if var.group_name == group_name]
         for group_name in group_names
     ]
 
 
-def get_name_to_idx(variables_dict: dict[str, Any]) -> dict[str, int]:
+def get_group_variable_names(variable_metadata: VariablesMetadata) -> dict[str, list[str]]:
+    """Get a dictionary mapping node/group names to the variables in that group."""
+    variable_groups = defaultdict(list)
+    for variable in variable_metadata.variables:
+        variable_groups[variable.group_name].append(variable.name)
+
+    return variable_groups
+
+
+def get_name_to_idx(variables_metadata: VariablesMetadata) -> dict[str, int]:
     """Get a dictionary mapping node/group names to their index in the variables dict."""
-    return {var["name"]: idx for idx, var in enumerate(variables_dict["variables"])}
+    return {var.name: idx for idx, var in enumerate(variables_metadata.variables)}
```

### Comparing `causica-0.3.3/src/causica/datasets/interventional_data.py` & `causica-0.3.4/src/causica/datasets/interventional_data.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.3/src/causica/datasets/loaded_expert_graph_container.py` & `causica-0.3.4/src/causica/datasets/loaded_expert_graph_container.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.3/src/causica/datasets/standardizer.py` & `causica-0.3.4/src/causica/datasets/standardizer.py`

 * *Files 9% similar despite different names*

```diff
@@ -59,13 +59,17 @@
 
     def forward(self) -> JointTransform:
         return JointTransform({key: module() for key, module in self.transform_modules.items()})
 
 
 def fit_standardizer(data: TensorDict) -> JointStandardizer:
     """Calculate the mean and standard deviation over the first dimension of each variable in the TensorDict and return a standardizer."""
-    means = data.apply(lambda x: torch.mean(x, dim=0, keepdim=True), batch_size=(1,))
-    # Filter out std == 0
-    stds = data.apply(lambda x: torch.std(x, dim=0, keepdim=True), batch_size=(1,)).apply(
-        lambda x: torch.where(x == 0, torch.ones_like(x), x)
+    means = data.apply(
+        lambda x: torch.mean(x, dim=0, keepdim=False),
+        batch_size=torch.Size(),
     )
+    # Filter out std == 0
+    stds = data.apply(
+        lambda x: torch.std(x, dim=0, keepdim=False),
+        batch_size=torch.Size(),
+    ).apply(lambda x: torch.where(x == 0, torch.ones_like(x), x))
     return JointStandardizer(means=means, stds=stds)
```

### Comparing `causica-0.3.3/src/causica/distributions/__init__.py` & `causica-0.3.4/src/causica/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.3/src/causica/distributions/adjacency/__init__.py` & `causica-0.3.4/src/causica/distributions/adjacency/__init__.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.3/src/causica/distributions/adjacency/adjacency_distributions.py` & `causica-0.3.4/src/causica/distributions/adjacency/adjacency_distributions.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.3/src/causica/distributions/adjacency/constrained_adjacency_distributions.py` & `causica-0.3.4/src/causica/distributions/adjacency/constrained_adjacency_distributions.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.3/src/causica/distributions/adjacency/directed_acyclic.py` & `causica-0.3.4/src/causica/distributions/adjacency/directed_acyclic.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.3/src/causica/distributions/adjacency/enco.py` & `causica-0.3.4/src/causica/distributions/adjacency/enco.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.3/src/causica/distributions/adjacency/gibbs_dag_prior.py` & `causica-0.3.4/src/causica/distributions/adjacency/gibbs_dag_prior.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.3/src/causica/distributions/adjacency/three_way.py` & `causica-0.3.4/src/causica/distributions/adjacency/three_way.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.3/src/causica/distributions/distribution_module.py` & `causica-0.3.4/src/causica/distributions/distribution_module.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.3/src/causica/distributions/gumbel_binary.py` & `causica-0.3.4/src/causica/distributions/gumbel_binary.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.3/src/causica/distributions/noise/__init__.py` & `causica-0.3.4/src/causica/distributions/noise/__init__.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.3/src/causica/distributions/noise/bernoulli.py` & `causica-0.3.4/src/causica/distributions/noise/bernoulli.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.3/src/causica/distributions/noise/categorical.py` & `causica-0.3.4/src/causica/distributions/noise/categorical.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.3/src/causica/distributions/noise/joint.py` & `causica-0.3.4/src/causica/distributions/noise/joint.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 
 class JointNoise(Noise[TensorDict]):
     """Represents an independent joint noise distribution of multiple variables types.
 
     Samples are TensorDicts containining independent variables.
     """
 
+    arg_constraints = {}
+
     def __init__(self, independent_noise_dists: dict[str, Noise[torch.Tensor]]):
         shapes = defaultdict[torch.Size, list[str]](list)
         for name, noise_dist in independent_noise_dists.items():
             shapes[noise_dist.batch_shape].append(name)
         if len(shapes) > 1:
             raise ValueError(f"Incompatible batch shapes: {shapes}")
 
@@ -117,14 +119,15 @@
         Dict of independent noise modules following the shape and type specifications.
     """
     noise_modules: dict[str, NoiseModule] = {}
     for key, shape in shapes.items():
         size = shape[-1]
         var_type = types[key]
 
+        noise_module: NoiseModule
         if var_type == VariableTypeEnum.CATEGORICAL:
             noise_module = CategoricalNoiseModule(size)
         elif var_type == VariableTypeEnum.BINARY:
             noise_module = BernoulliNoiseModule(size)
         elif var_type == VariableTypeEnum.CONTINUOUS:
             if continuous_noise_dist == ContinuousNoiseDist.SPLINE:
                 noise_module = SplineNoiseModule(size)
```

### Comparing `causica-0.3.3/src/causica/distributions/noise/noise.py` & `causica-0.3.4/src/causica/distributions/noise/noise.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.3/src/causica/distributions/noise/spline/bayesiains_nsf_rqs.py` & `causica-0.3.4/src/causica/distributions/noise/spline/bayesiains_nsf_rqs.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.3/src/causica/distributions/noise/spline/rational_quadratic_transform.py` & `causica-0.3.4/src/causica/distributions/noise/spline/rational_quadratic_transform.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.3/src/causica/distributions/noise/spline/spline.py` & `causica-0.3.4/src/causica/distributions/noise/spline/spline.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.3/src/causica/distributions/noise/univariate_normal.py` & `causica-0.3.4/src/causica/distributions/noise/univariate_normal.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             noise: noise variable with shape sample_shape + batch_shape.
         Returns:
             The generated samples with shape sample_shape + batch_shape + event_shape
         """
         return noise + self.loc
 
 
-class UnivariateNormalNoiseModule(NoiseModule[UnivariateNormalNoise]):
+class UnivariateNormalNoiseModule(NoiseModule[IndependentNoise[UnivariateNormalNoise]]):
     """Represents a UnivariateNormalNoise with learnable parameters for independent variables."""
 
     def __init__(self, dim: int, init_log_scale: float = 0.0):
         """
         Args:
             dim: Number of dimensions for the NormalNoise.
         """
```

### Comparing `causica-0.3.3/src/causica/distributions/transforms.py` & `causica-0.3.4/src/causica/distributions/transforms.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 """
 Wrapper around torch.distributions.transforms to allow for joint transforms on TensorDicts.
 """
+from typing import Mapping
 
 import torch
 import torch.distributions as td
 from tensordict import TensorDict
 
 
 class JointTransform(td.Transform):
     """A joint transform that applies a different transform to each key in the TensorDict.
 
+    Keys in the input that are not found in the transform are left unchanged.
+
     This is heavily inspired by the `torch.distributions.transforms.StackTransform` class.
     See https://pytorch.org/docs/stable/distributions.html#torch.distributions.transforms.StackTransform
     """
 
-    def __init__(self, transformations: dict[str, td.Transform], cache_size: int = 0):
+    def __init__(self, transformations: Mapping[str, td.Transform], cache_size: int = 0):
         """
         Args:
             transformations: A dictionary of transforms, where the keys are the keys in the TensorDict
             cache_size: Size of cache. If zero, no caching is done. If one, the latest single value is cached.
                 Only 0 and 1 are supported.
         """
         assert all(
@@ -27,26 +30,25 @@
         if cache_size:
             transformations = {key: t.with_cache(cache_size) for key, t in transformations.items()}
         super().__init__(cache_size=cache_size)
 
         self.transformations = transformations
 
     def _call(self, x: TensorDict) -> TensorDict:
-        if not set(self.transformations.keys()).issubset(x.keys()):
-            raise ValueError("All keys in transformations must be in x.")
-
-        return x.clone().update({key: transform(x[key]) for key, transform in self.transformations.items()})
+        return x.clone().update(
+            {key: transform(x[key]) for key, transform in self.transformations.items() if key in x.keys()}
+        )
 
     def _inverse(self, y: TensorDict) -> TensorDict:
         # We cannot use ._inv as pylint complains with E202: _inv is hidden because of `self._inv = None`
         # in td.Transform.__init__
-        if not set(self.transformations.keys()).issubset(y.keys()):
-            raise ValueError("All keys in transformations must be in y.")
 
-        return y.clone().update({key: transform.inv(y[key]) for key, transform in self.transformations.items()})
+        return y.clone().update(
+            {key: transform.inv(y[key]) for key, transform in self.transformations.items() if key in y.keys()}
+        )
 
     def log_abs_det_jacobian(self, x: TensorDict, y: TensorDict) -> torch.Tensor:
         if set(x.keys()) != set(y.keys()):
             raise ValueError("x and y must have the same keys.")
 
         if not set(self.transformations.keys()).issubset(x.keys()):
             raise ValueError("All keys in transformations must be in x and y.")
```

### Comparing `causica-0.3.3/src/causica/fsspec_helpers.py` & `causica-0.3.4/src/causica/fsspec_helpers.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.3/src/causica/functional_relationships/do_functional_relationships.py` & `causica-0.3.4/src/causica/functional_relationships/do_functional_relationships.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.3/src/causica/functional_relationships/functional_relationships.py` & `causica-0.3.4/src/causica/functional_relationships/functional_relationships.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.3/src/causica/functional_relationships/icgnn.py` & `causica-0.3.4/src/causica/functional_relationships/icgnn.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.3/src/causica/functional_relationships/linear_functional_relationships.py` & `causica-0.3.4/src/causica/functional_relationships/linear_functional_relationships.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.3/src/causica/graph/evaluation_metrics.py` & `causica-0.3.4/src/causica/graph/evaluation_metrics.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.3/src/causica/lightning/callbacks.py` & `causica-0.3.4/src/causica/lightning/callbacks.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.3/src/causica/lightning/cli.py` & `causica-0.3.4/src/causica/lightning/cli.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.3/src/causica/lightning/data_modules/basic_data_module.py` & `causica-0.3.4/src/causica/lightning/data_modules/basic_data_module.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,45 @@
 from collections import defaultdict
 
 import pandas as pd
 import torch
 from tensordict import TensorDict
 from torch.utils.data import DataLoader
 
-from causica.datasets.causica_dataset_format import convert_variable_types_to_enum, tensordict_from_variables_metadata
+from causica.datasets.causica_dataset_format import Variable, tensordict_from_variables_metadata
 from causica.datasets.standardizer import fit_standardizer
 from causica.datasets.tensordict_utils import identity, tensordict_shapes
 from causica.datasets.variable_types import VariableTypeEnum
 from causica.lightning.data_modules.deci_data_module import DECIDataModule
 
 
 class BasicDECIDataModule(DECIDataModule):
     """A datamodule interface for a dataframe and variable specification."""
 
     def __init__(
         self,
         dataframe: pd.DataFrame,
-        variables_spec: dict,
+        variables: list[Variable],
         batch_size: int,
         normalize: bool = False,
         dataset_name: str = "anonymous_dataset",
     ):
         super().__init__()
         self.dataset_df = dataframe
-        self.variables_metadata = convert_variable_types_to_enum(variables_spec)
+        self.variables = variables
         self._dataset_name = dataset_name
         self.normalize = normalize
         self.batch_size = batch_size
 
-        self._dataset_train = tensordict_from_variables_metadata(
-            self.dataset_df.to_numpy(), self.variables_metadata["variables"]
-        )
+        self._dataset_train = tensordict_from_variables_metadata(self.dataset_df.to_numpy(), self.variables)
         self._variable_shapes = tensordict_shapes(self._dataset_train)
-        self._variable_types = {var["group_name"]: var["type"] for var in self.variables_metadata["variables"]}
+        self._variable_types = {var.group_name: var.type for var in self.variables}
         self._column_names = defaultdict(list)
-        for variable in self.variables_metadata["variables"]:
-            self._column_names[variable["group_name"]].append(variable["name"])
+        for variable in self.variables:
+            self._column_names[variable.group_name].append(variable.name)
 
         if self.normalize:
             continuous_keys = [k for k, v in self._variable_types.items() if v == VariableTypeEnum.CONTINUOUS]
             self.normalizer = fit_standardizer(self._dataset_train.select(*continuous_keys))
 
             transform = self.normalizer()
             self._dataset_train = transform(self._dataset_train)
```

### Comparing `causica-0.3.3/src/causica/lightning/data_modules/deci_data_module.py` & `causica-0.3.4/src/causica/lightning/data_modules/deci_data_module.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.3/src/causica/lightning/data_modules/variable_spec_data.py` & `causica-0.3.4/src/causica/lightning/data_modules/variable_spec_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Lightning Classes for loading data in the default format used in Azure Blob Storage."""
 import os
 from collections import defaultdict
 from functools import partial
-from typing import Any, Optional
+from typing import Any, Iterable, Optional, Union
 
 import torch
 from tensordict import TensorDict
 from torch.utils.data import DataLoader
 
-from causica.datasets.causica_dataset_format import DataEnum, load_data
+from causica.datasets.causica_dataset_format import CAUSICA_DATASETS_PATH, DataEnum, VariablesMetadata, load_data
 from causica.datasets.standardizer import JointStandardizer, fit_standardizer
 from causica.datasets.tensordict_utils import identity, tensordict_shapes
 from causica.datasets.variable_types import VariableTypeEnum
 from causica.lightning.data_modules.deci_data_module import DECIDataModule
 
 
 class VariableSpecDataModule(DECIDataModule):
@@ -30,34 +30,37 @@
     """
 
     def __init__(
         self,
         root_path: str,
         batch_size: int = 128,
         dataset_name: str = "anonymous_dataset",
-        normalize: bool = False,
+        normalize: Union[bool, Iterable[str]] = False,
+        exclude_normalization: Iterable[str] = tuple(),
         load_counterfactual: bool = False,
-        **storage_options: dict[str, Any],
+        **storage_options: Any,
     ):
         """
         Args:
             root_path: Path to directory with causal data
             batch_size: Batch size for training and test data.
             storage_options: Storage options forwarded to `fsspec` when loading files.
             dataset_name: A name for the dataset
             load_counterfactual: Whether there is counterfactual data
-            normalize: Whether to normalize the data
+            normalize: Whether to normalize the data or list of variables to normalize
+            exclude_normalization: Which variables to exclude from normalization
         """
         super().__init__()
         self.batch_size = batch_size
         self._dataset_name = dataset_name
         self.root_path = root_path
         self.batch_size = batch_size
         self.storage_options = storage_options
         self.normalize = normalize
+        self.exclude_normalization = set(exclude_normalization)
         self.load_counterfactual = load_counterfactual
 
         self.normalizer: Optional[JointStandardizer] = None
 
     @property
     def variable_shapes(self) -> dict[str, torch.Size]:
         return _check_exists(self, "_variable_shapes")
@@ -78,15 +81,15 @@
     def dataset_test(self) -> TensorDict:
         return _check_exists(self, "_dataset_test")
 
     @property
     def dataset_name(self) -> str:
         return self._dataset_name
 
-    def _load_all_data(self, variables_metadata: dict):
+    def _load_all_data(self, variables_metadata: VariablesMetadata):
         _load_data = partial(
             load_data, root_path=self.root_path, variables_metadata=variables_metadata, **self.storage_options
         )
 
         self._dataset_train = _load_data(data_enum=DataEnum.TRAIN)
         self._dataset_test = _load_data(data_enum=DataEnum.TEST)
         self.true_adj = _load_data(data_enum=DataEnum.TRUE_ADJACENCY)
@@ -108,32 +111,40 @@
         # ...
         # data:
         #  class_path: causica.lightning.data_modules.VariableSpecDataModule
         #  init_args:
         #    ...
         #    variables_metadata: null
         _load_data = partial(load_data, root_path=self.root_path, **self.storage_options)
-        variables_metadata = _load_data(data_enum=DataEnum.VARIABLES_JSON)
+        variables_metadata: VariablesMetadata = _load_data(data_enum=DataEnum.VARIABLES_JSON)
 
         self._load_all_data(variables_metadata)
 
         train_keys = set(self._dataset_train.keys())
         test_keys = set(self._dataset_test.keys())
         assert (
             train_keys == test_keys
         ), f"node_names for the training and test data must match. Diff: {train_keys.symmetric_difference(test_keys)}"
         self._variable_shapes = tensordict_shapes(self._dataset_train)
-        self._variable_types = {var["group_name"]: var["type"] for var in variables_metadata["variables"]}
+        self._variable_types = {var.group_name: var.type for var in variables_metadata.variables}
         self._column_names = defaultdict(list)
-        for variable in variables_metadata["variables"]:
-            self._column_names[variable["group_name"]].append(variable["name"])
+        for variable in variables_metadata.variables:
+            self._column_names[variable.group_name].append(variable.name)
 
         if self.normalize:
-            continuous_keys = [k for k, v in self._variable_types.items() if v == VariableTypeEnum.CONTINUOUS]
-            self.normalizer = fit_standardizer(self._dataset_train.select(*continuous_keys))
+            if isinstance(self.normalize, Iterable):
+                normalization_variables = set(self.normalize) - self.exclude_normalization
+            else:
+                normalization_variables = {
+                    k
+                    for k, v in self._variable_types.items()
+                    if v == VariableTypeEnum.CONTINUOUS and k not in self.exclude_normalization
+                }
+
+            self.normalizer = fit_standardizer(self._dataset_train.select(*normalization_variables))
 
             transform = self.normalizer()
             self._dataset_train = transform(self._dataset_train)
             self._dataset_test = transform(self._dataset_test)
 
     def train_dataloader(self):
         return DataLoader(
@@ -164,21 +175,19 @@
 
     Args:
         dataset_name: Name of the dataset to load.
         batch_size: Batch size for all datasets.
         dataset_path: Path to CSuite dataset mirror.
     """
 
-    DEFAULT_CSUITE_PATH = "https://azuastoragepublic.blob.core.windows.net/datasets"
-
     def __init__(
         self,
         dataset_name: str,
         batch_size: int = 128,
-        dataset_path: str = DEFAULT_CSUITE_PATH,
+        dataset_path: str = CAUSICA_DATASETS_PATH,
         load_counterfactual: bool = False,
     ):
         super().__init__(
             root_path=os.path.join(dataset_path, dataset_name),
             batch_size=batch_size,
             dataset_name=dataset_name,
             load_counterfactual=load_counterfactual,
```

### Comparing `causica-0.3.3/src/causica/lightning/loggers.py` & `causica-0.3.4/src/causica/lightning/loggers.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.3/src/causica/lightning/main.py` & `causica-0.3.4/src/causica/lightning/main.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.3/src/causica/lightning/modules/deci_module.py` & `causica-0.3.4/src/causica/lightning/modules/deci_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,14 @@
         self.variable_group_shapes = None
         self.variable_types = None
         self.variable_names = None
 
     def prepare_data(self) -> None:
         """Set the constraint matrix (if necessary)."""
         if self.constraint_matrix_path:
-            # NOTE: This assumes that adlfs paths will be opened non-anonymously
             storage_options = get_storage_options_for_path(self.constraint_matrix_path)
 
             with fsspec.open(self.constraint_matrix_path, **storage_options) as f:
                 if self.constraint_matrix_path.endswith("npy"):
                     constraint_matrix = np.load(f)
                 else:
                     raise ValueError(f"Unsupported constraint matrix format: {self.constraint_matrix_path}")
@@ -178,22 +177,24 @@
 
         batch_log_prob = sem.log_prob(batch).mean()
         sem_distribution_entropy = sem_distribution.entropy()
         prior_term = self.prior.log_prob(sem.graph)
         objective = (-sem_distribution_entropy - prior_term) / self.num_samples - batch_log_prob
         constraint = calculate_dagness(sem.graph)
         step_output = {
+            "alpha": self.auglag_loss.alpha,
+            "rho": self.auglag_loss.rho,
             "loss": self.auglag_loss(objective, constraint / self.num_samples),
             "batch_log_prob": batch_log_prob,
             "constraint": constraint,
             "num_edges": (sem.graph > 0.0).count_nonzero(),
             "vardist_entropy": sem_distribution_entropy,
             "prior_term": prior_term,
         }
-        self.log_dict({"alpha": self.auglag_loss.alpha, "rho": self.auglag_loss.rho, **step_output}, prog_bar=True)
+        self.log_dict(step_output, on_epoch=True)  # Only log this on epoch end
         return step_output
 
     def configure_optimizers(self):
         """Set the learning rates for different sets of parameters."""
         modules = {
             "icgnn": self.sem_module.functional_relationships,
             "vardist": self.sem_module.adjacency_module,
@@ -218,15 +219,16 @@
 
     def test_step_observational(self, batch: TensorDict, *args, **kwargs):
         """Evaluate the log prob of the model on the test set using multiple graph samples."""
         batch = batch.apply(lambda t: t.to(torch.float32, non_blocking=True))
         sems = self.sem_module().sample(torch.Size([NUM_GRAPH_SAMPLES]))
         dataset_size = self.trainer.datamodule.dataset_test.batch_size  # type: ignore
         assert len(dataset_size) == 1, "Only one batch size is supported"
-        # estimate log prob for each sample using graph samples and report the mean over graphs
+
+        # Estimate log prob for each sample using graph samples and report the mean over graphs
         log_prob_test = list_logsumexp([sem.log_prob(batch) for sem in sems]) - np.log(NUM_GRAPH_SAMPLES)
         self.log(
             "eval/test_LL",
             torch.sum(log_prob_test, dim=-1).item() / dataset_size[0],
             reduce_fx=sum,
             add_dataloader_idx=False,
         )
```

### Comparing `causica-0.3.3/src/causica/lightning/modules/variable_spec_module.py` & `causica-0.3.4/src/causica/lightning/modules/variable_spec_module.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.3/src/causica/mlflow_helpers.py` & `causica-0.3.4/src/causica/mlflow_helpers.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.3/src/causica/sem/distribution_parameters_sem.py` & `causica-0.3.4/src/causica/sem/distribution_parameters_sem.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.3/src/causica/sem/sem_distribution.py` & `causica-0.3.4/src/causica/sem/sem_distribution.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 from causica.functional_relationships.functional_relationships import FunctionalRelationships
 from causica.sem.distribution_parameters_sem import DistributionParametersSEM
 
 
 class SEMDistribution(td.Distribution):
     """A distribution over structural equation models.
 
-    Samples are instances of DistributionParametersSEM.
+    Samples are instances of DistributionParametersSEM. Note however that this was created before
+    pytorch set the expected type of samples to torch.Tensor, so this is breaking the types a bit.
 
     The distribution is essentially the same as the given adjacency distribution but with samples converted to SEMs.
     Therefore, all distribution properties such as entropy, mean and mode are given by the equivalent properties for the
     adjacency distribution.
     """
 
     arg_constraints: dict[str, Constraint] = {}
@@ -61,30 +62,30 @@
         graphs = self._adjacency_dist.relaxed_sample(sample_shape=sample_shape, temperature=temperature)
         return self._create_sems(graphs)
 
     def entropy(self) -> torch.Tensor:
         return self._adjacency_dist.entropy()
 
     @property
-    def mean(self) -> DistributionParametersSEM:
+    def mean(self) -> DistributionParametersSEM:  # type: ignore
         return DistributionParametersSEM(
             graph=self._adjacency_dist.mean,
             noise_dist=self._noise_module,
             func=self._functional_relationships,
         )
 
     @property
-    def mode(self) -> DistributionParametersSEM:
+    def mode(self) -> DistributionParametersSEM:  # type: ignore
         return DistributionParametersSEM(
             graph=self._adjacency_dist.mode,
             noise_dist=self._noise_module,
             func=self._functional_relationships,
         )
 
-    def log_prob(self, value: DistributionParametersSEM) -> torch.Tensor:
+    def log_prob(self, value: DistributionParametersSEM) -> torch.Tensor:  # type: ignore
         return self._adjacency_dist.log_prob(value.graph)
 
 
 class SEMDistributionModule(DistributionModule[SEMDistribution]):
     """Represents a SEMDistribution with learnable parameters."""
 
     def __init__(
```

### Comparing `causica-0.3.3/src/causica/sem/structural_equation_model.py` & `causica-0.3.4/src/causica/sem/structural_equation_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import abc
-from typing import Optional, Sequence
+from typing import Iterable, Optional, Sequence
 
 import torch
 import torch.distributions as dist
 from tensordict import TensorDict
 
 
 class SEM(dist.Distribution, abc.ABC):
@@ -106,15 +106,15 @@
 
 
 def ite(
     sem: SEM,
     factual_data: TensorDict,
     intervention_a: TensorDict,
     intervention_b: TensorDict,
-    effects: Optional[list[str]] = None,
+    effects: Optional[Iterable[str]] = None,
 ) -> TensorDict:
     """Calculate ITE of intervention A and B on some factual data for a list of effects.
 
     Args:
         factual_data: Factual data to abduct the noise from.
         intervention_a: Specification of intervention A.
         intervention_b: Specification of intervention B.
@@ -146,15 +146,15 @@
     return sem.do(interventions=intervention).noise_to_sample(sem.sample_to_noise(factual_data))
 
 
 def ate(
     sem: SEM,
     intervention_a: TensorDict,
     intervention_b: TensorDict,
-    effects: Optional[list[str]] = None,
+    effects: Optional[Iterable[str]] = None,
     num_samples: int = 1000,
 ) -> TensorDict:
     """Calculate the ATE of intervention A and B for a list of effects.
 
     Args:
         intervention_a: Specification of intervention A.
         intervention_b: Specification of intervention B.
```

### Comparing `causica-0.3.3/src/causica/training/auglag.py` & `causica-0.3.4/src/causica/training/auglag.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.3/src/causica/training/evaluation.py` & `causica-0.3.4/src/causica/training/evaluation.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.3/src/causica/triangular_transformations.py` & `causica-0.3.4/src/causica/triangular_transformations.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.3/PKG-INFO` & `causica-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: causica
-Version: 0.3.3
+Version: 0.3.4
 Summary: 
 License: MIT
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: azureml-mlflow (>=1.46.0,<2.0.0)
 Requires-Dist: dataclasses-json (>=0.5.7,<0.6.0)
 Requires-Dist: jsonargparse (<4.21.0)
 Requires-Dist: mlflow (>=2.0.0,<3.0.0)
-Requires-Dist: numba (>=0.56.0,<0.57.0)
 Requires-Dist: numpy (>=1.22.4,<2.0.0)
 Requires-Dist: pandas (>=1.4.2,<2.0.0)
 Requires-Dist: pytorch-lightning[extra] (>=1.9.0,<2.0.0)
 Requires-Dist: tensorboard (>=2.9.0,<3.0.0)
 Requires-Dist: tensordict (>=0.1.0,<0.2.0)
 Requires-Dist: torch (==2.0.0)
 Requires-Dist: types-PyYAML (>=6.0.12.2,<7.0.0.0)
```

