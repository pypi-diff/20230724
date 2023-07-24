# Comparing `tmp/perming-1.4.2-py3-none-any.whl.zip` & `tmp/perming-1.4.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 13757 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat      887 b- defN 23-Jul-22 02:42 perming/__init__.py
+Zip file size: 13756 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat      887 b- defN 23-Jul-24 13:50 perming/__init__.py
 -rw-rw-rw-  2.0 fat      176 b- defN 23-May-29 15:03 perming/_typing.py
--rw-rw-rw-  2.0 fat    22854 b- defN 23-Jul-22 02:49 perming/_utils.py
+-rw-rw-rw-  2.0 fat    22971 b- defN 23-Jul-24 14:04 perming/_utils.py
 -rw-rw-rw-  2.0 fat      568 b- defN 23-May-29 16:53 perming/_version.py
--rw-rw-rw-  2.0 fat    13988 b- defN 23-Jul-13 04:45 perming/common.py
+-rw-rw-rw-  2.0 fat    13949 b- defN 23-Jul-24 14:08 perming/common.py
 -rw-rw-rw-  2.0 fat     5605 b- defN 23-Jul-13 07:33 perming/general.py
--rw-rw-rw-  2.0 fat    10809 b- defN 23-Jul-22 03:13 perming-1.4.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-22 03:13 perming-1.4.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-22 03:13 perming-1.4.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      747 b- defN 23-Jul-22 03:13 perming-1.4.2.dist-info/RECORD
-10 files, 55734 bytes uncompressed, 12503 bytes compressed:  77.6%
+-rw-rw-rw-  2.0 fat    10828 b- defN 23-Jul-24 14:19 perming-1.4.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-24 14:19 perming-1.4.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-24 14:19 perming-1.4.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      747 b- defN 23-Jul-24 14:19 perming-1.4.3.dist-info/RECORD
+10 files, 55831 bytes uncompressed, 12502 bytes compressed:  77.6%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: perming/common.py
 Comment: 
 
 Filename: perming/general.py
 Comment: 
 
-Filename: perming-1.4.2.dist-info/METADATA
+Filename: perming-1.4.3.dist-info/METADATA
 Comment: 
 
-Filename: perming-1.4.2.dist-info/WHEEL
+Filename: perming-1.4.3.dist-info/WHEEL
 Comment: 
 
-Filename: perming-1.4.2.dist-info/top_level.txt
+Filename: perming-1.4.3.dist-info/top_level.txt
 Comment: 
 
-Filename: perming-1.4.2.dist-info/RECORD
+Filename: perming-1.4.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## perming/__init__.py

```diff
@@ -23,8 +23,8 @@
 COMMON_MODELS = {
     'Regression': Regressier,
     'Binary-classification': Binarier,
     'Multi-classification': Mutipler,
     'Multi-outputs': Ranker
 }
 
-__version__ = '1.4.2'
+__version__ = '1.4.3'
```

## perming/_utils.py

```diff
@@ -6,34 +6,34 @@
 from ._typing import TabularData, Tuple, Dict, Optional, Any
 from ._version import parse_torch_version
 
 class TabularDataset(torch.utils.data.Dataset):
     '''
     Tabular Data Constructed with `numpy.array` noted as `TabularData`.
     :param features: TabularData, composed of n-row samples and m-column features.
-    :param target: TabularData, consists of correct labels or values with size at n.
-    :param roc: bool, regression or classification. it represents a regression problem when `roc=True`.
+    :param target: TabularData, consists of correct labels or outputs with size at n.
+    :param roc: bool, as_tensor to torch.float or torch.long. select torch.float when `roc=True`.
     '''
     def __init__(self, features: TabularData, target: TabularData, roc: bool) -> None:
         self.features = torch.as_tensor(features, dtype=torch.float)
         self.target = torch.as_tensor(target, dtype=torch.float) if roc else torch.as_tensor(target, dtype=torch.long)
 
     def __getitem__(self, index):
         return self.features[index], self.target[index]
 
     def __len__(self) -> int:
         return len(self.features)
 
 class MLP(torch.nn.Module):
     '''
     Construct Model Layers with `input_`, `num_classes`, `hidden_layer_sizes`, `activation`.
-    :param input_: int, features' dimension of tabular data is input_.
-    :param num_classes: int, total number of correct label categories.
-    :param hidden_layer_sizes: Tuple[int], configure the size of each hidden layer. default: (100,).
-    :param activation:, activation configured by Classfier. default: torch.nn.ReLU().
+    :param input_: int, input dataset with features' dimension of tabular data is input_.
+    :param num_classes: int, total number of correct label categories or multi-outputs.
+    :param hidden_layer_sizes: Tuple[int], configure the length and size of each hidden layer.
+    :param activation:, activation configured by Box, Regressier, Binarier, Multipler, and Ranker.
     '''
     def __init__(self, input_: int, num_classes: int, hidden_layer_sizes: Tuple[int], activation) -> None:
         super(MLP, self).__init__()
         self.squeeze: bool = False if num_classes > 1 else True
         if hidden_layer_sizes: # for linear indivisible datasets
             assert hidden_layer_sizes[0] > 0, "Please ensure any layer of hidden_layer_sizes > 0"
             model_layers, hidden_length = OrderedDict(), len(hidden_layer_sizes)
@@ -53,16 +53,16 @@
     def forward(self, x):
         output = self.mlp(x)
         return output.squeeze(-1) if self.squeeze else output
 
 class BaseModel:
     '''
     Basic Model for Configuring Common Models and General Box.
-    :param input_: int, features' dimension of tabular data is input_.
-    :param num_classes: int, total number of correct label categories.
+    :param input_: int, input dataset with features' dimension of tabular data is input_.
+    :param num_classes: int, total number of correct label categories or multi-outputs.
     :param hidden_layer_sizes: Tuple[int], configure the size of each hidden layer.
     :param device: Any, device configured by common models and general box.
     :param activation: Any, activated function configured by common models and general box.
     :param criterion: Any, loss function determined by common models and general box.
     :param solver: str, optimization coordinated with `torch.optim.lr_scheduler`. (modified more params in `_solver`.)
     :param batch_size: int, batch size of tabular dataset in one training process.
     :param learning_rate_init: float, initialize the learning rate of the optimizer.
@@ -75,28 +75,27 @@
                  device: Any,
                  activation: Any,
                  criterion: Any,
                  solver: str, 
                  batch_size: int, 
                  learning_rate_init: float,
                  lr_scheduler: Optional[str]=None) -> None:
-
         assert input_ > 0, 'BaseModel need samples with dataset features named input_ > 0.'
         assert num_classes > 0, 'Supervised learning problems with num_classes ranges from (1, 2, 3, ...).'
         assert batch_size > 0, 'Batch size initialized with int value mostly 2^n(n=1, 2, 3), like 64, 128, 256.'
-        assert learning_rate_init > 0 and learning_rate_init < 1.0, 'Please assert learning rate initialized value in (0, 1.0).'
+        assert learning_rate_init > 1e-6 and learning_rate_init < 1.0, 'Please assert learning rate initialized value in (1e-6, 1.0).'
         self.input: int = input_
         self.num_classes: int = num_classes
         self.activation = activation # function activate high-dimensional features
         self.device = device # device configuration
         self.criterion = criterion # criterion with classification & torch.long, regression & torch.float, and multi-outputs & roc
         self.batch_size: int = batch_size
         self.lr: float = learning_rate_init
         self.model = MLP(self.input, self.num_classes, hidden_layer_sizes, self.activation).to(self.device)
-        if parse_torch_version(torch.__version__)[0] >= ['2', '0', '0']:
+        if parse_torch_version(torch.__version__)[0] >= ['2', '0', '0']: # compile model
             self.model = torch.compile(self.model)
         self.solver = self._solver(solver)
         self.lr_scheduler = self._scheduler(lr_scheduler)
 
     def _solver(self, solver: str):
         '''
         Configure Optimizer with `solver`.
@@ -151,15 +150,15 @@
                     worker_set: Dict[str, int]={'train': 8, 'test': 2, 'val': 1},
                     random_seed: Optional[int]=None) -> None:
         '''
         Encapsulate Dataset to DataLoader from Tabular Dataset.
         :param features: TabularData, composed of n-row samples and m-column features: (n_samples, n_features).
         :param target: TabularData, consists of correct labels or values: (n_samples,) or (n_samples, n_outputs).
         :param ratio_set: Dict[str, int], stores the proportion of train-set, test-set and val-set. default: {'train': 8, 'test': 1, 'val': 1}.
-        :param worker_set: Dict[str, int], load the configuration of DataLoader with multi-threaded. default: {'train': 8, 'test': 2, 'val': 1}.
+        :param worker_set: Dict[str, int], load the num_workers of DataLoader with multi-threaded. default: {'train': 8, 'test': 2, 'val': 1}.
         :param random_seed: int | None, random.seed(random_seed) used for fixed random datasets. default: None.
         '''
         assert ratio_set['train'] > 0 and ratio_set['test'] > 0 and ratio_set['val'] > 0
         assert ratio_set['train'] > 4 * ratio_set['test'], 'The training set needs to be larger than the test set.'
         assert ratio_set['train'] + ratio_set['test'] + ratio_set['val'] == 10, 'The sum of 3 datasets ratio needs to be 10.'
         assert isinstance(features, TabularData) and features.ndim == 2, 'Please ensure features with dimension at (n_samples, n_features).'
         assert features.shape[1] == self.input, 'Please ensure `input_` is equal to `features.shape[1]`.'
@@ -205,15 +204,15 @@
         '''
         assert num_epochs > 0 and interval > 0, 'With num_epochs > 0 and interval > 0 to train parameters into outputs.'
         assert tolerance > 1e-9 and tolerance < 1.0, 'Set tolerance to early stop training and validation process within patience.'
         assert patience >= 10 and patience <= 100, 'Value coordinate with tolerance should fit about num_epochs and batch_size.' 
         assert n_jobs == -1 or n_jobs > 0, 'Take full jobs with setting n_jobs=-1 or manually set nums of jobs.'
         total_step = len(self.train_loader)
         self._set_container(backend, n_jobs)
-        val_length = len(self.val_container)
+        val_length: int = len(self.val_container)
         self.stop_iter: bool = False # init state of train_val
         for epoch in range(num_epochs):
             gc.collect()
             torch.cuda.empty_cache()
             for i, (features, target) in enumerate(self.train_loader):
                 features = features.to(self.device)
                 target = target.to(self.device)
@@ -230,15 +229,15 @@
                 # validation with val_container
                 self.val_loss = 0 # int value at cpu
                 with parallel_backend(backend, n_jobs=n_jobs):
                     for val_set in self.val_container:
                         outputs_val = self.model(val_set[0].to(self.device)) # return value from cuda
                         self.val_loss += self.criterion(outputs_val, val_set[1].to(self.device))
                 self.val_loss /= val_length
-                val_counts = i + 1 + total_step * epoch
+                val_counts = i + 1 + total_step * epoch # times of val_loss renewed
 
                 # early stop
                 if early_stop:
                     if val_counts == 1: # record first time of val_loss
                         val_loss_pre, val_pos_ini = self.val_loss, 1
                     else:
                         if val_loss_pre < self.val_loss:
@@ -340,15 +339,15 @@
                 return outputs # Multi-outputs
             else:
                 regress.update(loss_)
                 return regress
 
     def _set_container(self, backend: str, n_jobs: int) -> None:
         '''
-        Acquire Validation Container with `parallel_backend` at `n_jobs`.
+        Validation Container with `parallel_backend` at `n_jobs`.
         :param backend: str, "threading", "multiprocessing, 'locky'.
         :param n_jobs: int, set jobs with backend to accelerate process.
         '''
         with parallel_backend(backend, n_jobs=n_jobs):
             val_iter, self.val_container = iter(self.val_loader), []
             while 1:
                 try:
```

## perming/common.py

```diff
@@ -2,20 +2,20 @@
 
 from ._typing import Tuple, Optional
 from ._utils import BaseModel, torch
 
 class Regressier(BaseModel):
     '''
     Supervised Learning Regressier for Tabular Data.
-    :param input_: int, features' dimension of tabular data is input_.
+    :param input_: int, input dataset with features' dimension of tabular data is input_.
     :param hidden_layer_sizes: Tuple[int], configure the size of each hidden layer. default: (100,).
     :param activation: str, configure function that activates the hidden layer. default: relu.
     :param criterion: str, loss function determined by different learning problem. default: MSELoss.
     :param solver: str, optimization function initialized with `learning_rate_init`. default: adam.
-    :param batch_size: int, batch size of dataset in one training process. default: 32.
+    :param batch_size: int, batch size of dataset in one training and validation process. default: 32.
     :param learning_rate_init: float, initialize the learning rate of the optimizer. default: 1e-2.
     :param lr_scheduler: str | None, set the learning rate scheduler integrated with the optimizer. default: None.
     '''
     def __init__(self, 
                  input_: int, 
                  hidden_layer_sizes: Tuple[int]=(100,),
                  *,
@@ -70,20 +70,20 @@
             return torch.nn.KLDivLoss()
         else:
             raise ValueError("Criterion Configuration Supports Options: MSELoss, L1Loss, SmoothL1Loss, KLDivLoss.")
 
 class Binarier(BaseModel):
     '''
     Binary Supervised Learning Classifier for Tabular Data.
-    :param input_: int, features' dimension of tabular data is input_.
+    :param input_: int, input dataset with features' dimension of tabular data is input_.
     :param hidden_layer_sizes: Tuple[int], configure the size of each hidden layer. default: (100,).
     :param activation: str, configure function that activates the hidden layer. default: relu.
     :param criterion: str, loss function determined by different learning problem. default: BCELoss.
     :param solver: str, optimization function coordinated with `torch.optim.lr_scheduler`. default: adam.
-    :param batch_size: int, batch size of dataset in one training process. default: 32.
+    :param batch_size: int, batch size of dataset in one training and validation process. default: 32.
     :param learning_rate_init: float, initialize the learning rate of the optimizer. default: 1e-2.
     :param lr_scheduler: str | None, set the learning rate scheduler integrated with the optimizer. default: None.
     '''
     def __init__(self, 
                  input_: int, 
                  hidden_layer_sizes: Tuple[int]=(100,),
                  *,
@@ -103,15 +103,15 @@
                                        solver, 
                                        batch_size, 
                                        learning_rate_init, 
                                        lr_scheduler)
 
     def _activate(self, activation: str):
         '''
-        Configure Activation with `activation` and `inplace=True`.
+        Configure Activation with `activation` and partly `inplace=True`.
         :param activation: str, 'relu', 'tanh', 'sigmoid', 'rrelu', 'leaky_relu', 'elu', 'celu'.
         '''
         if activation == 'relu':
             return torch.nn.ReLU(inplace=True)
         elif activation == 'tanh':
             return torch.nn.Tanh()
         elif activation == 'sigmoid':
@@ -138,22 +138,21 @@
             return torch.nn.BCEWithLogitsLoss()
         else:
             raise ValueError("Criterion Configuration Supports Options: BCELoss, BCEWithLogitsLoss.")
 
 class Mutipler(BaseModel):
     '''
     Mutiple Supervised Learning Classifier for Tabular Data.
-    :param input_: int, features' dimension of tabular data is input_.
+    :param input_: int, input dataset with features' dimension of tabular data is input_.
     :param num_classes: int, total number of correct label categories.
     :param hidden_layer_sizes: Tuple[int], configure the size of each hidden layer. default: (100,).
     :param activation: str, configure function that activates the hidden layer. default: relu.
-    :param inplace_on: bool, whether to use `inplace=True` on activation. default: False.
     :param criterion: str, loss function determined by different learning problem. default: CrossEntropyLoss.
     :param solver: str, optimization function coordinated with `torch.optim.lr_scheduler`. default: adam.
-    :param batch_size: int, batch size of dataset in one training process. default: 32.
+    :param batch_size: int, batch size of dataset in one training and validation process. default: 32.
     :param learning_rate_init: float, initialize the learning rate of the optimizer. default: 1e-2.
     :param lr_scheduler: str | None, set the learning rate scheduler integrated with the optimizer. default: None.
     '''
     def __init__(self, 
                  input_: int, 
                  num_classes: int,
                  hidden_layer_sizes: Tuple[int]=(100,),
@@ -206,22 +205,21 @@
             return torch.nn.NLLLoss()
         else:
             raise ValueError("Criterion Configuration Supports Options: CrossEntropyLoss, NLLLoss.")
         
 class Ranker(BaseModel):
     '''
     Supervised Learning Outputs Ranker for Tabular Data.
-    :param input_: int, features' dimension of tabular data is input_.
+    :param input_: int, input dataset with features' dimension of tabular data is input_.
     :param num_outputs: int, total number of correct label outputs.
     :param hidden_layer_sizes: Tuple[int], configure the size of each hidden layer. default: (100,).
     :param activation: str, configure function that activates the hidden layer. default: relu.
-    :param inplace_on: bool, whether to use `inplace=True` on activation. default: False.
     :param criterion: str, loss function determined by different learning problem. default: MultiLabelSoftMarginLoss.
     :param solver: str, optimization function coordinated with `torch.optim.lr_scheduler`. default: adam.
-    :param batch_size: int, batch size of dataset in one training process. default: 32.
+    :param batch_size: int, batch size of dataset in one training and validation process. default: 32.
     :param learning_rate_init: float, initialize the learning rate of the optimizer. default: 1e-2.
     :param lr_scheduler: str | None, set the learning rate scheduler integrated with the optimizer. default: None.
     '''
     def __init__(self, 
                  input_: int, 
                  num_outputs: int,
                  hidden_layer_sizes: Tuple[int]=(100,),
@@ -243,15 +241,15 @@
                                      batch_size, 
                                      learning_rate_init, 
                                      lr_scheduler)
 
     def _activate(self, activation: str):
         '''
         Configure Activation with `activation` and `inplace=True`.
-        :param activation: str, "relu", "rrelu", "leaky_relu", "elu", "celu".
+        :param activation: str, 'relu', 'rrelu', 'leaky_relu', 'elu', 'celu'.
         '''
         if activation == 'relu':
             return torch.nn.ReLU(inplace=True)
         elif activation == 'rrelu':
             return torch.nn.RReLU(inplace=True)
         elif activation == 'leaky_relu':
             return torch.nn.LeakyReLU(inplace=True)
```

## Comparing `perming-1.4.2.dist-info/METADATA` & `perming-1.4.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: perming
-Version: 1.4.2
+Version: 1.4.3
 Summary: The supervised learning framework based on perceptron for tabular data.
 Home-page: https://github.com/linjing-lab/easy-pytorch/tree/main/released_box
 Download-URL: https://github.com/linjing-lab/easy-pytorch/tags
 Author: 林景
 Author-email: linjing010729@163.com
 License: MPL 2.0
 Project-URL: Source, https://github.com/linjing-lab/easy-pytorch/tree/main/released_box/perming
 Project-URL: Tracker, https://github.com/linjing-lab/easy-pytorch/issues
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -116,7 +117,8 @@
 cd easy-pytorch/released_box
 pip install -e . --verbose
 ```
 download stable version:
 ```text
 pip install perming --upgrade
 ```
+
```

## Comparing `perming-1.4.2.dist-info/RECORD` & `perming-1.4.3.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-perming/__init__.py,sha256=DrB4epQKGcgbBlcG0vRfB9MWupr2Y-X6CjI1pa5hUIU,887
+perming/__init__.py,sha256=iLONaHLqN3t0omi27mthtNVzohjSYYyFVGXgH_XWuCE,887
 perming/_typing.py,sha256=SGQP3QKfMZr-ciHT6jIrv4NUDmgqkx-RhYxIQloBSC4,176
-perming/_utils.py,sha256=E42H10-HmjkwqoQQILbhRDmv-PuHVEPokc0dZlG0uvc,22854
+perming/_utils.py,sha256=mOG_39IpZdBbuq4W9b7iS5_rqNKh7H8RzPLQ5T3bzks,22971
 perming/_version.py,sha256=K3CPQxLgHmXPNpNWlhpnrp6Bt8v5rU9wZyVRBsRTI3E,568
-perming/common.py,sha256=_-wi8gZFYCtO81XNvu8y-WLJQiZj1-IJ9Ipr2YHWlYw,13988
+perming/common.py,sha256=X_n-3VxTkPbt8NJJWe1SeorolebHkK-UhsLhEi3viq8,13949
 perming/general.py,sha256=sUjieRqdWa3o6PXdici5ABarVHcBTCVuv1Wg2K1kggI,5605
-perming-1.4.2.dist-info/METADATA,sha256=IOSInhqM3mdKEnhxUhr36Enl_HbPyl3w-lK53_ad67Q,10809
-perming-1.4.2.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-perming-1.4.2.dist-info/top_level.txt,sha256=mxFGHPJW81IzoNdyMqNWWZA7gUBzz0RtiAw5cQ0qzX8,8
-perming-1.4.2.dist-info/RECORD,,
+perming-1.4.3.dist-info/METADATA,sha256=IE8AFkdhJ0St1bMs0Q2xVCJuGgwOacNzuD9qtHP4HXc,10828
+perming-1.4.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+perming-1.4.3.dist-info/top_level.txt,sha256=mxFGHPJW81IzoNdyMqNWWZA7gUBzz0RtiAw5cQ0qzX8,8
+perming-1.4.3.dist-info/RECORD,,
```

