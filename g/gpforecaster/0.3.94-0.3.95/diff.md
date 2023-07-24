# Comparing `tmp/gpforecaster-0.3.94.tar.gz` & `tmp/gpforecaster-0.3.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpforecaster-0.3.94.tar", last modified: Mon Jul 24 14:08:15 2023, max compression
+gzip compressed data, was "gpforecaster-0.3.95.tar", last modified: Mon Jul 24 17:55:36 2023, max compression
```

## Comparing `gpforecaster-0.3.94.tar` & `gpforecaster-0.3.95.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:08:15.094636 gpforecaster-0.3.94/
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-24 14:08:15.094636 gpforecaster-0.3.94/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:08:15.086636 gpforecaster-0.3.94/gpforecaster/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:08:15.090636 gpforecaster-0.3.94/gpforecaster/model/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/model/gp.py
--rw-r--r--   0 runner    (1001) docker     (123)    39784 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/model/gpf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/model/hyperparameter_tuning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/model/mean_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/model/mlls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:08:15.090636 gpforecaster-0.3.94/gpforecaster/results/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/results/calculate_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:08:15.094636 gpforecaster-0.3.94/gpforecaster/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/tests/test_calculate_results.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/tests/test_early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/tests/test_hyperparameter_tuning.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/tests/test_hyperparameter_tuning_m5.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/tests/test_model_results_m5.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/tests/test_model_results_police.py
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/tests/test_model_results_prison.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/tests/test_results_partial_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/tests/test_run_model_with_sampled_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/tests/test_sparse_gps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/tests/test_store_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/tests/test_svg_gps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/tests/test_tourism_gpf_with_local_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:08:15.094636 gpforecaster-0.3.94/gpforecaster/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/utils/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:08:15.094636 gpforecaster-0.3.94/gpforecaster/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/visualization/plot_predictions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:08:15.086636 gpforecaster-0.3.94/gpforecaster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-24 14:08:14.000000 gpforecaster-0.3.94/gpforecaster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-24 14:08:15.000000 gpforecaster-0.3.94/gpforecaster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 14:08:14.000000 gpforecaster-0.3.94/gpforecaster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-24 14:08:14.000000 gpforecaster-0.3.94/gpforecaster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-24 14:08:14.000000 gpforecaster-0.3.94/gpforecaster.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 14:08:15.094636 gpforecaster-0.3.94/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:55:36.887538 gpforecaster-0.3.95/
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-24 17:55:23.000000 gpforecaster-0.3.95/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-24 17:55:36.887538 gpforecaster-0.3.95/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-07-24 17:55:23.000000 gpforecaster-0.3.95/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:55:36.875538 gpforecaster-0.3.95/gpforecaster/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-24 17:55:23.000000 gpforecaster-0.3.95/gpforecaster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:55:36.879538 gpforecaster-0.3.95/gpforecaster/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-24 17:55:23.000000 gpforecaster-0.3.95/gpforecaster/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-24 17:55:23.000000 gpforecaster-0.3.95/gpforecaster/model/gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42904 2023-07-24 17:55:23.000000 gpforecaster-0.3.95/gpforecaster/model/gpf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-07-24 17:55:23.000000 gpforecaster-0.3.95/gpforecaster/model/hyperparameter_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-24 17:55:23.000000 gpforecaster-0.3.95/gpforecaster/model/mean_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-24 17:55:23.000000 gpforecaster-0.3.95/gpforecaster/model/mlls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:55:36.879538 gpforecaster-0.3.95/gpforecaster/results/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 17:55:23.000000 gpforecaster-0.3.95/gpforecaster/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-07-24 17:55:23.000000 gpforecaster-0.3.95/gpforecaster/results/calculate_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:55:36.887538 gpforecaster-0.3.95/gpforecaster/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:55:23.000000 gpforecaster-0.3.95/gpforecaster/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-24 17:55:23.000000 gpforecaster-0.3.95/gpforecaster/tests/test_calculate_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-24 17:55:23.000000 gpforecaster-0.3.95/gpforecaster/tests/test_early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-24 17:55:23.000000 gpforecaster-0.3.95/gpforecaster/tests/test_hyperparameter_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-24 17:55:23.000000 gpforecaster-0.3.95/gpforecaster/tests/test_hyperparameter_tuning_m5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-24 17:55:23.000000 gpforecaster-0.3.95/gpforecaster/tests/test_model_results_m5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-24 17:55:23.000000 gpforecaster-0.3.95/gpforecaster/tests/test_model_results_police.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-07-24 17:55:23.000000 gpforecaster-0.3.95/gpforecaster/tests/test_model_results_prison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-24 17:55:23.000000 gpforecaster-0.3.95/gpforecaster/tests/test_results_partial_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-24 17:55:23.000000 gpforecaster-0.3.95/gpforecaster/tests/test_run_model_with_sampled_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-24 17:55:23.000000 gpforecaster-0.3.95/gpforecaster/tests/test_sparse_gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-07-24 17:55:23.000000 gpforecaster-0.3.95/gpforecaster/tests/test_store_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-24 17:55:23.000000 gpforecaster-0.3.95/gpforecaster/tests/test_svg_gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-24 17:55:23.000000 gpforecaster-0.3.95/gpforecaster/tests/test_tourism_gpf_with_local_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:55:36.887538 gpforecaster-0.3.95/gpforecaster/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:55:23.000000 gpforecaster-0.3.95/gpforecaster/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-24 17:55:23.000000 gpforecaster-0.3.95/gpforecaster/utils/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:55:36.887538 gpforecaster-0.3.95/gpforecaster/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-24 17:55:23.000000 gpforecaster-0.3.95/gpforecaster/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-24 17:55:23.000000 gpforecaster-0.3.95/gpforecaster/visualization/plot_predictions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:55:36.879538 gpforecaster-0.3.95/gpforecaster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-24 17:55:36.000000 gpforecaster-0.3.95/gpforecaster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-24 17:55:36.000000 gpforecaster-0.3.95/gpforecaster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 17:55:36.000000 gpforecaster-0.3.95/gpforecaster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-24 17:55:36.000000 gpforecaster-0.3.95/gpforecaster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-24 17:55:36.000000 gpforecaster-0.3.95/gpforecaster.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 17:55:36.887538 gpforecaster-0.3.95/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-24 17:55:23.000000 gpforecaster-0.3.95/setup.py
```

### Comparing `gpforecaster-0.3.94/LICENCE` & `gpforecaster-0.3.95/LICENCE`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.94/PKG-INFO` & `gpforecaster-0.3.95/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpforecaster
-Version: 0.3.94
+Version: 0.3.95
 Summary: Hierarchical time series forecasting model using Gaussian Processes
 Home-page: UNKNOWN
 Author: Luis Roque
 Author-email: <roque0luis@gmail.com>
 License: UNKNOWN
 Keywords: python,time series,hierarchical,forecasting,gaussian process,machine learning
 Platform: UNKNOWN
```

### Comparing `gpforecaster-0.3.94/README.md` & `gpforecaster-0.3.95/README.md`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.94/gpforecaster/model/gp.py` & `gpforecaster-0.3.95/gpforecaster/model/gp.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,18 +43,23 @@
         train_y,
         likelihood,
         cov,
         changepoints,
         mean_func,
         inducing_points,
         device,
+        m,
+        k,
+        b,
     ):
         super().__init__(train_x, train_y, likelihood)
         self.changepoints = changepoints
-        self.mean_module = mean_func(self.changepoints, device)
+        self.mean_module = mean_func(
+            changepoints=self.changepoints, device=device, m=m, k=k, b=b
+        )
         # Use an InducingPointKernel instead of a standard kernel
         self.covar_module = InducingPointKernel(
             cov, inducing_points=inducing_points, likelihood=likelihood
         )
 
     def forward(self, x):
         mean_x = self.mean_module(x).to(torch.float32)
@@ -69,29 +74,34 @@
         train_y,
         likelihood,
         cov,
         changepoints,
         mean_func,
         inducing_points,
         device,
+        m,
+        k,
+        b,
     ):
         variational_distribution = CholeskyVariationalDistribution(
             inducing_points.size(0)
         ).to(torch.float32)
         variational_strategy = VariationalStrategy(
             self,
             inducing_points=inducing_points,
             variational_distribution=variational_distribution,
             learn_inducing_locations=True,
         )
         super(SvgGPModel, self).__init__(variational_strategy)
         self.train_inputs = train_x
         self.train_targets = train_y
         self.changepoints = changepoints
-        self.mean_module = mean_func(self.changepoints, device)
+        self.mean_module = mean_func(
+            changepoints=self.changepoints, device=device, m=m, k=k, b=b
+        )
         self.covar_module = cov
         self.likelihood = likelihood
 
     def forward(self, x):
         if x.requires_grad:
             x = x.detach()
         mean_x = self.mean_module(x)
```

### Comparing `gpforecaster-0.3.94/gpforecaster/model/gpf.py` & `gpforecaster-0.3.95/gpforecaster/model/gpf.py`

 * *Files 10% similar despite different names*

```diff
@@ -143,14 +143,15 @@
         self.inducing_points = (
             torch.rand(int(inducing_points_perc * self.n_train), dtype=torch.float32)
             * self.n_train
         ).to(self.device)
         self.inducing_points, sorted_indices = self.inducing_points.sort()
         self.losses = []
         self.val_losses = []
+        self.test_losses = []
         self.avg_loss = []
         self.avg_val_loss = []
         self.mll = None
 
         self.mase = MeanAbsoluteScaledError(multioutput="raw_values")
         self.seasonality = self.groups["seasonality"]
 
@@ -219,19 +220,23 @@
         )
         groups["predict"]["data_matrix"] = convert_and_transform_data(
             groups["predict"]["data_matrix"], scaler, fit=False
         )
 
         return groups, scaler
 
-    def hierarchical_data_summary(self, bottom_series=None):
+    def hierarchical_data_summary(self, bottom_series=None, test_data=False):
         groups_names = list(self.groups["train"]["groups_names"].keys())
         if bottom_series is None:
-            bottom_series = self.groups["train"]["data"]
-            n_samples = self.groups["train"]["n"]
+            if test_data:
+                bottom_series = self.test_y
+                n_samples = self.groups["h"]
+            else:
+                bottom_series = self.groups["train"]["data"]
+                n_samples = self.groups["train"]["n"]
         else:
             n_samples = bottom_series.shape[0]
 
         summary = {
             "total": torch.sum(
                 torch.tensor(bottom_series, dtype=torch.float32, device=self.device),
                 dim=1,
@@ -495,27 +500,33 @@
                         train_y=y[:, i],
                         likelihood=likelihood_list[i],
                         cov=mixed_covs[i],
                         changepoints=changepoints,
                         mean_func=PiecewiseLinearMean,
                         inducing_points=self.inducing_points.to(torch.float32),
                         device=self.device,
+                        m=m,
+                        k=k,
+                        b=b,
                     )
                 )
             elif self.gp_type == "svg":
                 model_list.append(
                     SvgGPModel(
                         train_x=x,
                         train_y=y[:, i],
                         likelihood=likelihood_list[i],
                         cov=mixed_covs[i],
                         changepoints=changepoints,
                         mean_func=PiecewiseLinearMean,
                         inducing_points=self.inducing_points,
                         device=self.device,
+                        m=m,
+                        k=k,
+                        b=b,
                     )
                 )
 
         return likelihood_list, model_list
 
     def early_stopping(self, val_losses, patience: int):
         if not val_losses:
@@ -574,19 +585,21 @@
         self,
         epoch: int,
         model,
         likelihood,
         train_y,
         val_x,
         val_y,
+        test_x,
+        test_y,
         mll: gpytorch.mlls.MarginalLogLikelihood,
         standard_optimizer: Optional[torch.optim.Adam] = None,
         scheduler: Optional[Any] = None,
         early_stopping: bool = True,
-    ) -> Tuple[float, Optional[float]]:
+    ) -> Tuple[float, Optional[float], Optional[float]]:
         """
         Perform a single iteration of the training loop.
 
         Parameters:
             epoch: The current epoch number.
             model: The model to be trained.
             likelihood: The likelihood function for the model.
@@ -602,32 +615,41 @@
         """
         standard_optimizer.zero_grad()
 
         output = model(*model.train_inputs)
         loss = -mll(output, model.train_targets)
 
         val_loss = None
+        test_loss = None
         if early_stopping and epoch % 5 == 0:
             model.eval()
             likelihood.eval()
-            val_loss = self.validate(model, val_x, val_y, train_y, likelihood)
+            val_loss, test_loss = self.validate(
+                model=model,
+                val_x=val_x,
+                val_y=val_y,
+                train_y=train_y,
+                test_x=test_x,
+                test_y=test_y,
+                likelihood=likelihood,
+            )
 
             model.train()
             likelihood.train()
 
         loss.backward()
         standard_optimizer.step()
 
         if scheduler:
             scheduler.step()
 
         if epoch % 30 == 0:
             self._log_memory()
 
-        return loss.item(), val_loss
+        return loss.item(), val_loss, test_loss
 
     def _log_memory(self):
         process = psutil.Process(os.getpid())
         mem = process.memory_info().rss / (1024**3)
         self.logger_train.info(f"train used {mem:.3f} GB of RAM")
 
     def train(
@@ -691,14 +713,15 @@
         if cross_validation:
             tscv = TimeSeriesSplit(n_splits=n_splits, test_size=self.groups["h"])
         else:
             # Just split once for training and validation
             tscv = TimeSeriesSplit(n_splits=2, test_size=self.groups["h"])
         self.val_losses = []
         self.losses = []
+        self.test_losses = []
 
         # Cross-validation loop
         for fold_idx, (train_indices, val_indices) in enumerate(
             tscv.split(self.train_x)
         ):
             # If not cross-validation and because min number of folds for tscv is 2
             # we skip the first one
@@ -714,14 +737,17 @@
             else:
                 train_x = self.train_x[train_indices]
                 train_y = self.train_y[train_indices]
                 train_y_split = concatenated_hierarchical_data[train_indices]
 
             val_x = self.train_x[val_indices]
             val_y = concatenated_hierarchical_data[val_indices]
+            test_x = self.test_x
+            hierarchical_data_test = self.hierarchical_data_summary(test_data=True)
+            test_y = self.concatenate_arrays(hierarchical_data_test)
 
             likelihood_list, model_list = self._build_model(
                 x=train_x,
                 y=train_y,
                 random_init=random_init,
                 rbf_kernel_lengthscale=rbf_kernel_lengthscale,
                 scale_rbf_kernel_outputscale=scale_rbf_kernel_outputscale,
@@ -742,109 +768,126 @@
             optimizer = self._create_standard_optimizer(model, lr, weight_decay)
             scheduler = self._create_scheduler(
                 scheduler_type, optimizer, epochs, gamma_rate
             )
 
             fold_losses = []
             fold_val_losses = []
+            fold_test_losses = []
 
             for epoch in range(epochs):
-                loss, val_loss = self._train_loop_iteration(
+                loss, val_loss, test_loss = self._train_loop_iteration(
                     epoch,
                     model,
                     likelihood,
                     val_x=val_x,
                     val_y=val_y,
+                    test_x=test_x,
+                    test_y=test_y,
                     train_y=train_y_split,
                     mll=self.mll,
                     standard_optimizer=optimizer,
                     scheduler=scheduler,
                     early_stopping=early_stopping,
                 )
 
                 # Storing losses per epoch per fold
                 fold_losses.append(loss)
                 if val_loss is not None:
                     fold_val_losses.append(val_loss)
+                    fold_test_losses.append(test_loss)
 
                 if verbose:
                     print(
                         f"Fold {fold_idx + 1} - Iter {epoch} - "
                         f"Loss: {np.round(loss, 3)}, "
                         f"Validation Loss: {np.round(val_loss, 3) if val_loss is not None else 'N/A'}"
+                        f"Test Loss: {np.round(test_loss, 3) if test_loss is not None else 'N/A'}"
                     )
 
                 if (
                     early_stopping
                     and val_loss is not None
                     and self.early_stopping(fold_val_losses, patience=patience)
                 ):
                     break
 
             self.losses.append(fold_losses)
             self.val_losses.append(fold_val_losses)
+            self.test_losses.append(fold_test_losses)
 
-            self._log_training_information(epoch, loss, val_loss)
+            self._log_training_information(epoch, loss, val_loss, test_loss)
 
         # Computing average losses over folds
         self.avg_loss = [fold[-1] for fold in self.losses]
         self.avg_val_loss = (
             [fold[-1] for fold in self.val_losses] if self.val_losses else None
         )
+        self.avg_test_loss = (
+            [fold[-1] for fold in self.test_losses] if self.test_losses else None
+        )
         print(
-            f"Average training loss: {self.avg_loss}, average validation loss: {self.avg_val_loss}"
+            f"Average training loss: {self.avg_loss}, "
+            f"average validation loss: {self.avg_val_loss}"
+            f"average test loss: {self.avg_test_loss}"
         )
 
         return model, likelihood
 
     def _initialize_mll(self, model, likelihood) -> None:
         if self.gp_type == "svg":
             self.mll = SumVariationalELBO(
                 likelihood, model, num_data=self.train_y.size(0)
             )
         else:
             self.mll = SumMarginalLogLikelihood(likelihood, model)
 
     def _log_training_information(
-        self, epoch: int, loss: float, val_loss: Optional[float]
+        self,
+        epoch: int,
+        loss: float,
+        val_loss: Optional[float],
+        test_loss: Optional[float],
     ) -> None:
         wall_time_train = time.time() - self.timer_start
         training_duration = timedelta(seconds=int(wall_time_train))
 
         self._log_memory()
 
         log_message = (
             f"Epoch {epoch} - "
             f"Duration: {str(training_duration)} - "
             f"Training Loss: {loss:.2f}"
         )
 
         if val_loss is not None:
             log_message += f" - Validation Loss: {val_loss:.2f}"
+            log_message += f" - Test Loss: {test_loss:.2f}"
 
         self.logger_train.info(log_message)
 
     def validate(
         self,
         model: IndependentModelList,
         val_x,
         val_y,
+        test_x,
+        test_y,
         train_y,
         likelihood,
-    ) -> float:
+    ) -> Tuple[float, float]:
         """
         Validate the model.
 
-        Parameters:
-            model (ExactGPModel): The GP model
-
         Returns:
-            float: The negative log likelihood of the model on the validation set.
+            tuple: The negative log likelihood of the model on the validation set
+                   and MASE on the test set.
         """
         with torch.no_grad(), gpytorch.settings.fast_pred_var():
+            # Validation
             val_output = likelihood(
                 *model(*[val_x for i in range(self.groups["predict"]["s"])])
             )
             val_pred = (
                 torch.zeros((val_x.shape[0], self.s)).to(torch.float32).to(self.device)
             )
             for ts in range(self.s):
@@ -865,30 +908,58 @@
             val_loss = self.mase(
                 y_pred=concatenated_pred,
                 y_true=val_y,
                 y_train=train_y,
                 sp=sp,
             ).mean()
 
-        return val_loss.item()
+            # Testing
+            test_output = likelihood(
+                *model(*[test_x for i in range(self.groups["predict"]["s"])])
+            )
+            test_pred = (
+                torch.zeros((test_x.shape[0], self.s)).to(torch.float32).to(self.device)
+            )
+            for ts in range(self.s):
+                test_pred[:, ts] = test_output[ts].mean
+
+            hierarchical_pred_test = self.hierarchical_data_summary(test_pred)
+            concatenated_pred_test = self.concatenate_arrays(hierarchical_pred_test)
+
+            concatenated_pred_test = concatenated_pred_test.cpu().numpy()
+            test_y = test_y.cpu().numpy()
+
+            test_mase = self.mase(
+                y_pred=concatenated_pred_test,
+                y_true=test_y,
+                y_train=train_y,  # Note: We use train_y for scaling
+                sp=sp,
+            ).mean()
+
+        return val_loss.item(), test_mase.item()
 
     @staticmethod
     def _create_directory_if_not_exists(directory_path):
         if not os.path.exists(directory_path):
             os.makedirs(directory_path)
 
     def plot_losses(self, start_idx: int = 5):
         self._create_directory_if_not_exists("plots")
 
-        n_iterations, val_losses_interp = self._prepare_loss_data()
+        n_iterations, val_losses_interp, test_losses_interp = self._prepare_loss_data()
 
         # assuming self.losses and val_losses_interp are lists of lists, where each sub-list corresponds to a fold
-        for i, (losses, val_losses) in enumerate(zip(self.losses, val_losses_interp)):
+        for i, (losses, val_losses, test_losses) in enumerate(
+            zip(self.losses, val_losses_interp, test_losses_interp)
+        ):
             self._plot_loss_data(
-                n_iterations[start_idx:], losses[start_idx:], val_losses[start_idx:]
+                n_iterations[start_idx:],
+                losses[start_idx:],
+                val_losses[start_idx:],
+                test_losses[start_idx:],
             )
             self._customize_plot(i + 1)
 
             timestamp = time.strftime("%Y%m%d-%H%M%S", time.gmtime())
             plt.savefig(
                 f"./plots/gpf_{__version__}_loss_{self.dataset}_fold_{i + 1}_{timestamp}.pdf",
                 format="pdf",
@@ -899,35 +970,48 @@
     def _prepare_loss_data(self):
         n_iterations_total = np.arange(len(self.losses[0]))
 
         val_interval = round(len(self.losses[0]) / len(self.val_losses[0]))
         val_indices = np.arange(0, len(self.losses[0]), val_interval)
 
         val_losses_interp = []
+        test_losses_interp = []
         for val_losses_fold in self.val_losses:  # Loop over each fold
             interp_func = interp1d(
                 val_indices,
                 val_losses_fold,
                 kind="linear",
                 fill_value="extrapolate",
             )
             val_losses_interp.append(interp_func(n_iterations_total))
 
+        for test_losses_fold in self.test_losses:  # Loop over each fold
+            interp_func = interp1d(
+                val_indices,
+                test_losses_fold,
+                kind="linear",
+                fill_value="extrapolate",
+            )
+            test_losses_interp.append(interp_func(n_iterations_total))
+
         n_iterations = n_iterations_total
 
-        return n_iterations, val_losses_interp
+        return n_iterations, val_losses_interp, test_losses_interp
 
     @staticmethod
-    def _plot_loss_data(n_iterations, train_losses, val_losses_interp):
+    def _plot_loss_data(
+        n_iterations, train_losses, val_losses_interp, test_losses_interp
+    ):
         plt.plot(n_iterations, train_losses, label="Training Loss")
-        plt.plot(n_iterations, val_losses_interp, marker="*", label="Validation Loss")
+        plt.plot(n_iterations, val_losses_interp, marker="^", label="Validation Loss")
+        plt.plot(n_iterations, test_losses_interp, marker="*", label="Test Loss")
 
     @staticmethod
     def _customize_plot(fold_num: int):
-        plt.title(f"Training and Validation Losses for Fold {fold_num}")
+        plt.title(f"Training, Validation and Test Losses for Fold {fold_num}")
         plt.xlabel("Iteration")
         plt.ylabel("Loss")
         plt.legend()
 
     def predict(
         self,
         model: IndependentModelList,
```

### Comparing `gpforecaster-0.3.94/gpforecaster/model/hyperparameter_tuning.py` & `gpforecaster-0.3.95/gpforecaster/model/hyperparameter_tuning.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     dataset_name: str,
     hierarchical_data: Dict[str, List],
     hyperparameters: Dict[str, Any],
     gp_type: str,
     device: str,
     logger_tuning: Logger,
     trial_num: int,
-) -> Tuple[float, Dict[str, Any]]:
+) -> Tuple[float, float, Dict[str, Any]]:
     """
     Train a single GPF model with the given hyperparameters.
 
     Args:
         dataset_name (str): The name of the dataset.
         hierarchical_data (Dict[str, List]): The hierarchical data for the model.
         hyperparameters (Dict[str, Any]): The hyperparameters to use for the model.
@@ -59,31 +59,34 @@
             periodic_kernel_lengthscale=hyperparameters["periodic_kernel_lengthscale"],
             scale_periodic_kernel_outputscale=hyperparameters["scale_periodic_kernel_outputscale"],
             m=hyperparameters["m"],
             k=hyperparameters["k"],
             b=hyperparameters["b"]
         )
         val_loss = np.mean(gpf.avg_val_loss)
+        test_loss = np.mean(gpf.avg_test_loss)
         if np.isnan(val_loss):
             val_loss = np.finfo(np.float32).max
+            test_loss = np.finfo(np.float32).max
     except:
         val_loss = np.finfo(np.float32).max
+        test_loss = np.finfo(np.float32).max
 
     log_and_print_best_hyperparameters(
-        gp_type, dataset_name, hyperparameters, val_loss, logger_tuning
+        gp_type, dataset_name, hyperparameters, val_loss, test_loss, logger_tuning
     )
 
     if model is not None:
         del model
     if like is not None:
         del like
     del gpf
     gc.collect()
 
-    return (val_loss, hyperparameters)
+    return (val_loss, test_loss, hyperparameters)
 
 
 def optimize_hyperparameters_bayesian(
     dataset_name: str,
     hierarchical_data: Dict[str, List],
     num_trials: int,
     gp_type: str = "exact",
@@ -119,19 +122,20 @@
         Real(0.05, 0.3, name="m"),
         Real(0.05, 0.3, name="k"),
         Real(0.05, 0.3, name="b")
     ]
 
     optimizer = Optimizer(search_space)
     trial_num = 0
+    test_loss = 0
 
     @use_named_args(search_space)
     def wrapped_single_trial(**hyperparameters):
-        nonlocal trial_num
-        val_loss, _ = single_trial(
+        nonlocal trial_num, test_loss
+        val_loss, test_loss, _ = single_trial(
             dataset_name,
             hierarchical_data,
             hyperparameters,
             gp_type,
             device,
             logger_tuning,
             trial_num=trial_num
@@ -143,25 +147,27 @@
     best_hyperparameters = {k.name: v for k, v in zip(search_space, results.x)}
 
     log_and_print_best_hyperparameters(
         gp_type,
         dataset_name,
         best_hyperparameters,
         results.fun,
+        test_loss,
         logger_tuning,
         best="BEST",
     )
     return best_hyperparameters
 
 
 def log_and_print_best_hyperparameters(
     gp_type: str,
     dataset_name: str,
     best_hyperparameters: Dict[str, Any],
     best_val_loss: float,
+    best_test_loss: float,
     logger_tuning: Logger,
     best="",
 ):
     """
     Log and print the best hyperparameters and validation loss.
 
     Args:
@@ -174,17 +180,19 @@
     logger_tuning.info(
         f"\n{best} -> "
         f"Algorithm: gpf_{gp_type}, "
         f"Version: {__version__}, "
         f"Dataset: {dataset_name}, "
         f"{best} hyperparameters: {best_hyperparameters}, "
         f"Validation loss: {best_val_loss}\n"
+        f"Test loss: {best_test_loss}\n"
     )
 
     print(
         f"\n{best} -> "
         f"Algorithm: gpf_{gp_type}, \n"
         f"Version: {__version__}, \n"
         f"Dataset: {dataset_name}, \n"
         f"{best} hyperparameters: {best_hyperparameters}, \n"
         f"Validation loss: {best_val_loss}\n"
+        f"Test loss: {best_test_loss}\n"
     )
```

### Comparing `gpforecaster-0.3.94/gpforecaster/model/mean_functions.py` & `gpforecaster-0.3.95/gpforecaster/model/mean_functions.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.94/gpforecaster/model/mlls.py` & `gpforecaster-0.3.95/gpforecaster/model/mlls.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.94/gpforecaster/results/calculate_metrics.py` & `gpforecaster-0.3.95/gpforecaster/results/calculate_metrics.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.94/gpforecaster/tests/test_calculate_results.py` & `gpforecaster-0.3.95/gpforecaster/tests/test_calculate_results.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.94/gpforecaster/tests/test_early_stopping.py` & `gpforecaster-0.3.95/gpforecaster/tests/test_early_stopping.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.94/gpforecaster/tests/test_hyperparameter_tuning.py` & `gpforecaster-0.3.95/gpforecaster/tests/test_hyperparameter_tuning.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.94/gpforecaster/tests/test_hyperparameter_tuning_m5.py` & `gpforecaster-0.3.95/gpforecaster/tests/test_hyperparameter_tuning_m5.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.94/gpforecaster/tests/test_model_results_m5.py` & `gpforecaster-0.3.95/gpforecaster/tests/test_model_results_m5.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.94/gpforecaster/tests/test_model_results_police.py` & `gpforecaster-0.3.95/gpforecaster/tests/test_model_results_police.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.94/gpforecaster/tests/test_model_results_prison.py` & `gpforecaster-0.3.95/gpforecaster/tests/test_model_results_prison.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.94/gpforecaster/tests/test_results_partial_data.py` & `gpforecaster-0.3.95/gpforecaster/tests/test_results_partial_data.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.94/gpforecaster/tests/test_run_model_with_sampled_dataset.py` & `gpforecaster-0.3.95/gpforecaster/tests/test_run_model_with_sampled_dataset.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.94/gpforecaster/tests/test_sparse_gps.py` & `gpforecaster-0.3.95/gpforecaster/tests/test_sparse_gps.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.94/gpforecaster/tests/test_store_results.py` & `gpforecaster-0.3.95/gpforecaster/tests/test_store_results.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.94/gpforecaster/tests/test_svg_gps.py` & `gpforecaster-0.3.95/gpforecaster/tests/test_svg_gps.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.94/gpforecaster/tests/test_tourism_gpf_with_local_file.py` & `gpforecaster-0.3.95/gpforecaster/tests/test_tourism_gpf_with_local_file.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.94/gpforecaster/utils/logger.py` & `gpforecaster-0.3.95/gpforecaster/utils/logger.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.94/gpforecaster/visualization/plot_predictions.py` & `gpforecaster-0.3.95/gpforecaster/visualization/plot_predictions.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.94/gpforecaster.egg-info/PKG-INFO` & `gpforecaster-0.3.95/gpforecaster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpforecaster
-Version: 0.3.94
+Version: 0.3.95
 Summary: Hierarchical time series forecasting model using Gaussian Processes
 Home-page: UNKNOWN
 Author: Luis Roque
 Author-email: <roque0luis@gmail.com>
 License: UNKNOWN
 Keywords: python,time series,hierarchical,forecasting,gaussian process,machine learning
 Platform: UNKNOWN
```

### Comparing `gpforecaster-0.3.94/gpforecaster.egg-info/SOURCES.txt` & `gpforecaster-0.3.95/gpforecaster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.94/setup.py` & `gpforecaster-0.3.95/setup.py`

 * *Files identical despite different names*

