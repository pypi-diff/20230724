# Comparing `tmp/torch4keras-0.0.9.tar.gz` & `tmp/torch4keras-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch4keras-0.0.9.tar", last modified: Sun Jul 16 10:02:37 2023, max compression
+gzip compressed data, was "torch4keras-0.1.0.tar", last modified: Mon Jul 24 13:32:48 2023, max compression
```

## Comparing `torch4keras-0.0.9.tar` & `torch4keras-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 10:02:37.006085 torch4keras-0.0.9/
--rw-rw-rw-   0        0        0    11558 2022-10-19 12:34:20.000000 torch4keras-0.0.9/LICENSE
--rw-rw-rw-   0        0        0     7489 2023-07-16 10:02:37.005087 torch4keras-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     7235 2023-07-16 09:59:31.000000 torch4keras-0.0.9/README.md
--rw-rw-rw-   0        0        0       42 2023-07-16 10:02:37.006085 torch4keras-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      522 2023-07-16 10:01:39.000000 torch4keras-0.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 10:02:36.998088 torch4keras-0.0.9/torch4keras/
--rw-rw-rw-   0        0        0        0 2023-05-30 14:28:06.000000 torch4keras-0.0.9/torch4keras/__init__.py
--rw-rw-rw-   0        0        0    51485 2023-06-10 11:46:06.000000 torch4keras-0.0.9/torch4keras/callbacks.py
--rw-rw-rw-   0        0        0    28990 2023-07-07 13:01:23.000000 torch4keras-0.0.9/torch4keras/model.py
--rw-rw-rw-   0        0        0    17329 2023-07-12 15:43:50.000000 torch4keras-0.0.9/torch4keras/snippets.py
-drwxrwxrwx   0        0        0        0 2023-07-16 10:02:37.003083 torch4keras-0.0.9/torch4keras.egg-info/
--rw-rw-rw-   0        0        0     7489 2023-07-16 10:02:36.000000 torch4keras-0.0.9/torch4keras.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-07-16 10:02:36.000000 torch4keras-0.0.9/torch4keras.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 10:02:36.000000 torch4keras-0.0.9/torch4keras.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-16 10:02:36.000000 torch4keras-0.0.9/torch4keras.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 13:32:48.543826 torch4keras-0.1.0/
+-rw-rw-rw-   0        0        0    11558 2022-10-19 12:34:20.000000 torch4keras-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     7963 2023-07-24 13:32:48.542829 torch4keras-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7709 2023-07-24 12:53:02.000000 torch4keras-0.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-24 13:32:48.543826 torch4keras-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      522 2023-07-22 16:30:44.000000 torch4keras-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 13:32:48.524417 torch4keras-0.1.0/torch4keras/
+-rw-rw-rw-   0        0        0        0 2023-05-30 14:28:06.000000 torch4keras-0.1.0/torch4keras/__init__.py
+-rw-rw-rw-   0        0        0    53316 2023-07-24 12:53:02.000000 torch4keras-0.1.0/torch4keras/callbacks.py
+-rw-rw-rw-   0        0        0    31227 2023-07-24 12:53:02.000000 torch4keras-0.1.0/torch4keras/model.py
+-rw-rw-rw-   0        0        0    17219 2023-07-24 12:53:02.000000 torch4keras-0.1.0/torch4keras/snippets.py
+drwxrwxrwx   0        0        0        0 2023-07-24 13:32:48.541824 torch4keras-0.1.0/torch4keras.egg-info/
+-rw-rw-rw-   0        0        0     7963 2023-07-24 13:32:48.000000 torch4keras-0.1.0/torch4keras.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-07-24 13:32:48.000000 torch4keras-0.1.0/torch4keras.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 13:32:48.000000 torch4keras-0.1.0/torch4keras.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-24 13:32:48.000000 torch4keras-0.1.0/torch4keras.egg-info/top_level.txt
```

### Comparing `torch4keras-0.0.9/LICENSE` & `torch4keras-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `torch4keras-0.0.9/PKG-INFO` & `torch4keras-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: torch4keras
-Version: 0.0.9
+Version: 0.1.0
 Summary: Use torch like keras
 Home-page: https://github.com/Tongjilibo/torch4keras
 Author: Tongjilibo
 License: Apache License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# torch4keras
-**Use torch like keras**
+![torch4keras](https://github.com/Tongjilibo/torch4keras/blob/master/docs/pics/torch4keras.png)
+
 
 [![licence](https://img.shields.io/github/license/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/blob/master/LICENSE) 
 [![GitHub release](https://img.shields.io/github/release/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/releases) 
 [![PyPI](https://img.shields.io/pypi/v/torch4keras?label=pypi%20package)](https://pypi.org/project/torch4keras/) 
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/torch4keras)](https://pypistats.org/packages/torch4keras)
 [![GitHub stars](https://img.shields.io/github/stars/Tongjilibo/torch4keras?style=social)](https://github.com/Tongjilibo/torch4keras)
 [![GitHub Issues](https://img.shields.io/github/issues/Tongjilibo/torch4keras.svg)](https://github.com/Tongjilibo/torch4keras/issues)
@@ -71,28 +71,30 @@
     ```
 
 ## 3. 快速上手
 - 参考[bert4torch](https://github.com/Tongjilibo/bert4torch)的训练过程
 - 简单示例: [turorials_mnist](https://github.com/Tongjilibo/torch4keras/blob/master/examples/turorials_mnist.py)
 
 ## 4. 版本说明
+- **v0.1.0**: 允许调整进度条的显示参数, 进度条和日志同步（如果进度条平滑了则日志也平滑）, 自动把tensor转到model.device上, 允许打印第一个batch来检查样本
 - **v0.0.9**：20230716 增加auto_set_cuda_devices自动选择显卡，增加log_info，log_warn, log_error等小函数
 - **v0.0.8**：20230625 增加EmailCallback和WandbCallback, 增加AccelerateTrainer和DeepSpeedTrainer, grad_accumulation_steps内算一个batch，修改Trainer中部分成员函数
 - **v0.0.7.post3**: 20230517 修复保存scheduler
 - **v0.0.7.post2**: 20230517 Checkpoint Calback增加保存scheduler, save_weights可自行创建目录，Logger, Tensorboard模块加入lr, 修改predict和add_trainer
 - **v0.0.7**：20230505 独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
 - **v0.0.6**：20230212 增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现(增加几个成员变量、增加initilize()、删除对forward参数个数的判断、dp和ddp不解析module、修改use_amp参数为mixed_precision)，增加了AccelerateCallback
 - **v0.0.5**：20221217 增加Summary的Callback, 增加Tqdm的进度条展示，保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
 - **v0.0.4**：20221127 为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
 - **v0.0.3.post2**：20221107 修复DDP下打印的bug
 - **v0.0.3**：20221106 参考Keras修改了callback的逻辑
 - **v0.0.2**：20221023 增加Checkpoint, Evaluator等自带Callback, 修改BaseModel(net)方式，修复DP和DDP的__init__()
 - **v0.0.1**：20221019 初始版本
 
 ## 5. 更新：
+- **20230721**: 允许调整进度条的显示参数, 进度条和日志同步（如果进度条平滑了则日志也平滑）, 自动把tensor转到model.device上, 允许打印第一个batch来检查样本
 - **20230716**：增加auto_set_cuda_devices自动选择显卡，增加log_info，log_warn, log_error等小函数
 - **20230625**：增加EmailCallback和WandbCallback, 增加AccelerateTrainer和DeepSpeedTrainer, grad_accumulation_steps内算一个batch，修改Trainer中部分成员函数
 - **20230517**：Checkpoint Calback增加保存scheduler, save_weights可自行创建目录，Logger, Tensorboard模块加入lr, 修改predict和add_trainer
 - **20230505**：独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
 - **20230212**：增加hf的accelerator测试用例, ddp需要外部控制执行callback, 混合精度支持bf16
 - **20230116**：增加resume_from_checkpoint和save_to_checkpoint，动态为nn.Module增加Trainer的方法add_trainer
 - **20221217**：保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
```

### Comparing `torch4keras-0.0.9/README.md` & `torch4keras-0.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# torch4keras
-**Use torch like keras**
+![torch4keras](https://github.com/Tongjilibo/torch4keras/blob/master/docs/pics/torch4keras.png)
+
 
 [![licence](https://img.shields.io/github/license/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/blob/master/LICENSE) 
 [![GitHub release](https://img.shields.io/github/release/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/releases) 
 [![PyPI](https://img.shields.io/pypi/v/torch4keras?label=pypi%20package)](https://pypi.org/project/torch4keras/) 
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/torch4keras)](https://pypistats.org/packages/torch4keras)
 [![GitHub stars](https://img.shields.io/github/stars/Tongjilibo/torch4keras?style=social)](https://github.com/Tongjilibo/torch4keras)
 [![GitHub Issues](https://img.shields.io/github/issues/Tongjilibo/torch4keras.svg)](https://github.com/Tongjilibo/torch4keras/issues)
@@ -61,28 +61,30 @@
     ```
 
 ## 3. 快速上手
 - 参考[bert4torch](https://github.com/Tongjilibo/bert4torch)的训练过程
 - 简单示例: [turorials_mnist](https://github.com/Tongjilibo/torch4keras/blob/master/examples/turorials_mnist.py)
 
 ## 4. 版本说明
+- **v0.1.0**: 允许调整进度条的显示参数, 进度条和日志同步（如果进度条平滑了则日志也平滑）, 自动把tensor转到model.device上, 允许打印第一个batch来检查样本
 - **v0.0.9**：20230716 增加auto_set_cuda_devices自动选择显卡，增加log_info，log_warn, log_error等小函数
 - **v0.0.8**：20230625 增加EmailCallback和WandbCallback, 增加AccelerateTrainer和DeepSpeedTrainer, grad_accumulation_steps内算一个batch，修改Trainer中部分成员函数
 - **v0.0.7.post3**: 20230517 修复保存scheduler
 - **v0.0.7.post2**: 20230517 Checkpoint Calback增加保存scheduler, save_weights可自行创建目录，Logger, Tensorboard模块加入lr, 修改predict和add_trainer
 - **v0.0.7**：20230505 独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
 - **v0.0.6**：20230212 增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现(增加几个成员变量、增加initilize()、删除对forward参数个数的判断、dp和ddp不解析module、修改use_amp参数为mixed_precision)，增加了AccelerateCallback
 - **v0.0.5**：20221217 增加Summary的Callback, 增加Tqdm的进度条展示，保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
 - **v0.0.4**：20221127 为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
 - **v0.0.3.post2**：20221107 修复DDP下打印的bug
 - **v0.0.3**：20221106 参考Keras修改了callback的逻辑
 - **v0.0.2**：20221023 增加Checkpoint, Evaluator等自带Callback, 修改BaseModel(net)方式，修复DP和DDP的__init__()
 - **v0.0.1**：20221019 初始版本
 
 ## 5. 更新：
+- **20230721**: 允许调整进度条的显示参数, 进度条和日志同步（如果进度条平滑了则日志也平滑）, 自动把tensor转到model.device上, 允许打印第一个batch来检查样本
 - **20230716**：增加auto_set_cuda_devices自动选择显卡，增加log_info，log_warn, log_error等小函数
 - **20230625**：增加EmailCallback和WandbCallback, 增加AccelerateTrainer和DeepSpeedTrainer, grad_accumulation_steps内算一个batch，修改Trainer中部分成员函数
 - **20230517**：Checkpoint Calback增加保存scheduler, save_weights可自行创建目录，Logger, Tensorboard模块加入lr, 修改predict和add_trainer
 - **20230505**：独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
 - **20230212**：增加hf的accelerator测试用例, ddp需要外部控制执行callback, 混合精度支持bf16
 - **20230116**：增加resume_from_checkpoint和save_to_checkpoint，动态为nn.Module增加Trainer的方法add_trainer
 - **20221217**：保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
```

### Comparing `torch4keras-0.0.9/setup.py` & `torch4keras-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='torch4keras',
-    version='v0.0.9',
+    version='v0.1.0',
     description='Use torch like keras',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License',
     url='https://github.com/Tongjilibo/torch4keras',
     author='Tongjilibo',
     install_requires=[],
```

### Comparing `torch4keras-0.0.9/torch4keras/callbacks.py` & `torch4keras-0.1.0/torch4keras/callbacks.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,65 +1,90 @@
-from contextlib import redirect_stderr
 import sys
 import collections
 import time
 import numpy as np
 from datetime import datetime
 import warnings
 from collections import deque
 import json
 import copy
 import os
-from torch import nn
-from torch4keras.snippets import send_email, info_level_prefix
+from torch4keras.snippets import log_error, send_email
+
+
+SKIP_METRICS = {'size'}
+
+
+def _process_stateful_metrics(stateful_metrics):
+    ''''''
+    if stateful_metrics is None:
+        stateful_metrics_new = set()
+    elif isinstance(stateful_metrics, str):
+        stateful_metrics_new = {stateful_metrics}
+    elif isinstance(stateful_metrics, (set, tuple, list)):
+        stateful_metrics_new = set(stateful_metrics)
+    else:
+        raise ValueError('Args `stateful_metrics` only support `int/set/tuple/list` format')
+    stateful_metrics_new.add('lr')  # 学习率是不能平滑
+    return stateful_metrics_new
 
 
 class Progbar(object):
     """进度条，直接从keras引入"""
-    def __init__(self, target, width=30, verbose=1, interval=0.05, stateful_metrics=None):
+    def __init__(self, target, width=30, verbose=1, time_interval=0.05, stateful_metrics=None, smooth_interval=None):
+        '''
+        :param target: 进度条的step数量
+        :param width: 进度条的宽度
+        :param verbose: 是否展示进度条
+        :param time_interval: 更新进度条的最短时间间隔
+        :param stateful_metrics: list, 以状态量记录指标的格式
+        :param smooth_interval: int, 平滑时候使用的的step个数
+        '''
         self.target = target
         self.width = width
         self.verbose = verbose
-        self.interval = interval
-        if stateful_metrics:
-            self.stateful_metrics = set(stateful_metrics)
-        else:
-            self.stateful_metrics = set()
-
+        self.time_interval = time_interval
+        assert (smooth_interval is None) or isinstance(smooth_interval, int), 'Args `smooth_interval` only support `int` format'
+        self.smooth_interval = smooth_interval
+        self.stateful_metrics = _process_stateful_metrics(stateful_metrics)
+        
         self._dynamic_display = ((hasattr(sys.stdout, 'isatty') and sys.stdout.isatty()) or 'ipykernel' in sys.modules)
         self._total_width = 0
         self._seen_so_far = 0
-        self._values = collections.OrderedDict()
+        self._values = collections.OrderedDict()  # OrderedDict([('loss', [11.60657262802124, 5]), ('acc', [0.25, 5])])
+        self._smooth_values = dict()  # 存储滑动平均的结果，stateful_metrics时候滑动平均结果和不滑动一致
         self._start = time.time()
         self._last_update = 0
 
     def update(self, current, values=None):
         """Updates the progress bar."""
         values = values or []
         for k, v in values:
             if k not in self.stateful_metrics:
                 if k not in self._values:
-                    self._values[k] = [v * (current - self._seen_so_far),
-                                       current - self._seen_so_far]
+                    self._values[k] = [v * (current - self._seen_so_far), current - self._seen_so_far]
+                elif (self.smooth_interval is not None) and (current % self.smooth_interval == 0):
+                    # 如果定义了累积smooth_interval，则需要重新累计
+                    self._values[k] = [v, 1]
                 else:
                     self._values[k][0] += v * (current - self._seen_so_far)
                     self._values[k][1] += (current - self._seen_so_far)
             else:
                 # Stateful metrics output a numeric value.  This representation
                 # means "take an average from a single value" but keeps the
                 # numeric formatting.
                 self._values[k] = [v, 1]
         
         self._seen_so_far = current
 
         now = time.time()
         info = ' - %.0fs' % (now - self._start)
         if self.verbose == 1:
-            if (now - self._last_update < self.interval and
-                    self.target is not None and current < self.target):
+            if (now - self._last_update < self.time_interval and self.target is not None and current < self.target):
+                # 训练每个step太快了，则不更新进度条，累计达到一定的时间间隔再更新进度条
                 return
 
             prev_total_width = self._total_width
             if self._dynamic_display:
                 sys.stdout.write('\b' * prev_total_width)
                 sys.stdout.write('\r')
             else:
@@ -88,16 +113,15 @@
             if current:
                 time_per_unit = (now - self._start) / current
             else:
                 time_per_unit = 0
             if self.target is not None and current < self.target:
                 eta = time_per_unit * (self.target - current)
                 if eta > 3600:
-                    eta_format = ('%d:%02d:%02d' %
-                                  (eta // 3600, (eta % 3600) // 60, eta % 60))
+                    eta_format = ('%d:%02d:%02d' % (eta // 3600, (eta % 3600) // 60, eta % 60))
                 elif eta > 60:
                     eta_format = '%d:%02d' % (eta // 60, eta % 60)
                 else:
                     eta_format = '%ds' % eta
 
                 info = ' - ETA: %s' % eta_format
             else:
@@ -107,16 +131,16 @@
                     info += ' %.0fms/step' % (time_per_unit * 1e3)
                 else:
                     info += ' %.0fus/step' % (time_per_unit * 1e6)
 
             for k in self._values:
                 info += ' - %s:' % k
                 if isinstance(self._values[k], list):
-                    avg = np.mean(
-                        self._values[k][0] / max(1, self._values[k][1]))
+                    avg = np.mean(self._values[k][0] / max(1, self._values[k][1]))  # 指标平滑
+                    self._smooth_values[k] = avg  # 存储滑动平均的结果
                     if abs(avg) > 1e-3:
                         info += ' %.4f' % avg
                     else:
                         info += ' %.4e' % avg
                 else:
                     info += ' %s' % self._values[k]
             info += ' '  # 最后加个空格，防止中途有别的打印
@@ -307,18 +331,15 @@
 class BaseLogger(Callback):
     """计算metrics的均值, 默认是callbacks中第一项, 主要是为History服务
     
     :param stateful_metrics: List[str], 仅保留状态信息的指标
     """
     def __init__(self, stateful_metrics=None, **kwargs):
         super(BaseLogger, self).__init__(**kwargs)
-        if stateful_metrics:
-            self.stateful_metrics = set(stateful_metrics)
-        else:
-            self.stateful_metrics = set()
+        self.stateful_metrics = _process_stateful_metrics(stateful_metrics)
 
     def on_epoch_begin(self, global_step, epoch, logs=None):
         self.seen = 0
         self.totals = {}
 
     def on_batch_end(self, global_step, local_step, logs=None):
         logs = logs or {}
@@ -350,37 +371,36 @@
 class TerminateOnNaN(Callback):
     """Loss出现NAN停止训练"""
     def on_batch_end(self, global_step, local_step, logs=None):
         logs = logs or {}
         loss = logs.get('loss')
         if loss is not None:
             if np.isnan(loss) or np.isinf(loss):
-                info_level_prefix('Step %d: Invalid loss, terminating training' % global_step, 2)
+                log_error('Step %d: Invalid loss, terminating training' % global_step)
                 self.trainer.stop_training = True
 
 
 class KerasProgbar(Callback):
     """ keras进度条 """
-    def __init__(self, stateful_metrics=None, **kwargs):
+    def __init__(self, stateful_metrics=None, smooth_interval=None, width=30, **kwargs):
         super(KerasProgbar, self).__init__(**kwargs)
-        if stateful_metrics:
-            self.stateful_metrics = set(stateful_metrics)
-        else:
-            self.stateful_metrics = set()
+        self.stateful_metrics = _process_stateful_metrics(stateful_metrics)
+        self.smooth_interval = smooth_interval
+        self.width = width
 
     def add_metrics(self, metrics, stateful_metrics=None, add_position=None):
         '''在指定位置插入metrics指标
         '''
         if add_position is None:
             add_position = len(self.params['metrics'])
         metrics = [metrics] if isinstance(metrics, str) else metrics
         if stateful_metrics:
-            stateful_metrics = [stateful_metrics] if isinstance(stateful_metrics, str) else stateful_metrics
-            self.stateful_metrics.update(set(stateful_metrics))
-            self.progbar.stateful_metrics.update(set(stateful_metrics))
+            stateful_metrics = _process_stateful_metrics(stateful_metrics)
+            self.stateful_metrics.update(stateful_metrics)
+            self.progbar.stateful_metrics.update(stateful_metrics)
 
         add_metrics = []
         for metric in metrics:
             if metric not in self.params['metrics']:
                 add_metrics.append(metric)
         self.params['metrics'] = self.params['metrics'][:add_position] + add_metrics + self.params['metrics'][add_position:]
 
@@ -392,108 +412,103 @@
             print('%s - Start Training' % (time_start))
 
     def on_epoch_begin(self, global_step=None, epoch=None, logs=None):
         if self.verbose:
             time_start = datetime.now().strftime('%Y-%m-%d %H:%M:%S')
             print('%s - Epoch: %d/%d' % (time_start, epoch+1, self.epochs))
             self.target = self.params['steps']
-            self.progbar = Progbar(target=self.target, verbose=self.verbose, stateful_metrics=self.stateful_metrics)
+            self.progbar = Progbar(target=self.target, width=self.width, verbose=self.verbose, 
+                                   stateful_metrics=self.stateful_metrics, smooth_interval=self.smooth_interval)
         self.seen = 0
 
-    def on_batch_begin(self, global_step=None, local_step=None, logs=None):
-        if self.seen < self.target:
-            self.log_values = []
-
     def on_batch_end(self, global_step=None, local_step=None, logs=None):
         logs = logs or {}
         self.seen += 1
-        for k in self.params['metrics']:
-            if k in logs:
-                self.log_values.append((k, logs[k]))
-
+        log_values = [(k, logs[k]) for k in self.params['metrics'] if k in logs]
         # Skip progbar update for the last batch;
         # will be handled by on_epoch_end.
         if self.verbose and self.seen < self.target:
-            self.progbar.update(self.seen, self.log_values)
+            self.progbar.update(self.seen, log_values)
+            logs.update(self.progbar._smooth_values)  # 如果进度条是平滑的，那这里的logs也覆盖掉
 
     def on_epoch_end(self, global_step=None, epoch=None, logs=None):
         logs = logs or {}
-        for k in self.params['metrics']:
-            if k in logs:
-                self.log_values.append((k, logs[k]))
+        log_values = [(k, logs[k]) for k in self.params['metrics'] if k in logs]
         if self.verbose:
-            self.progbar.update(self.seen, self.log_values)
+            self.progbar.update(self.seen, log_values)
+            logs.update(self.progbar._smooth_values)
     
     def on_train_end(self, logs=None):
         if self.verbose:
             time_start = datetime.now().strftime('%Y-%m-%d %H:%M:%S')
             print('%s - Finish Training' % (time_start))
-
+        
 
 class TqdmProgbar(KerasProgbar):
     """ Tqdm进度条 """
+    def __init__(self, stateful_metrics=None, smooth_interval=None, width=None, **kwargs):
+        super().__init__(stateful_metrics, smooth_interval, width, **kwargs)
+
     def on_epoch_begin(self, global_step=None, epoch=None, logs=None):
         if self.verbose:
             from tqdm import tqdm
             time_start = datetime.now().strftime('%Y-%m-%d %H:%M:%S')
             print('%s - Epoch: %d/%d' % (time_start, epoch+1, self.epochs))
             self.target = self.params['steps']
-            self.progbar = tqdm(total=self.params['steps'], desc='Training', dynamic_ncols=False, file=sys.stdout, smoothing=0)
+            self.progbar = tqdm(total=self.params['steps'], desc='Training', dynamic_ncols=False, file=sys.stdout, smoothing=0, ncols=self.width)
         self.seen = 0
         self._values = collections.OrderedDict()
+        self._smooth_values = dict()
         self._seen_so_far = 0
 
-    def on_batch_begin(self, global_step=None, local_step=None, logs=None):
-        if self.seen < self.target:
-            self.log_values = []
-
     def on_batch_end(self, global_step=None, local_step=None, logs=None):
         self.seen += 1
-        logs = self.smooth_values(self.seen, logs or {})
-        for k in self.params['metrics']:
-            if k in logs:
-                self.log_values.append((k, logs[k]))
+        logs_new = self.smooth_values(self.seen, logs or {})
+        log_values = [(k, logs_new[k]) for k in self.params['metrics'] if k in logs_new]
 
         # Skip progbar update for the last batch;
         # will be handled by on_epoch_end.
         if self.verbose and self.seen < self.target:
             self.progbar.n = self.seen
             self.progbar.refresh()
-            self.progbar.set_postfix(self.log_values)
+            self.progbar.set_postfix(log_values)
+            logs.update(self._smooth_values)
 
     def on_epoch_end(self, global_step=None, epoch=None, logs=None):
-        logs = self.smooth_values(self.seen, logs or {})
-        for k in self.params['metrics']:
-            if k in logs:
-                self.log_values.append((k, logs[k]))
+        logs_new = self.smooth_values(self.seen, logs or {})
+        log_values = [(k, logs_new[k]) for k in self.params['metrics'] if k in logs_new]
         if self.verbose:
             self.progbar.n = self.seen
             self.progbar.refresh()
-            self.progbar.set_postfix(self.log_values)
+            self.progbar.set_postfix(log_values)
+            logs.update(self._smooth_values)
             self.progbar.close()
     
     def smooth_values(self, current, values=None):
         '''从Progbar迁移过来'''
         values = values or []
         for k, v in values.items():
             if k not in self.stateful_metrics:
                 if k not in self._values:
                     self._values[k] = [v * (current - self._seen_so_far), current - self._seen_so_far]
+                elif (self.smooth_interval is not None) and (current % self.smooth_interval == 0):
+                    # 如果定义了累积smooth_interval，则需要重新累计
+                    self._values[k] = [v, 1]
                 else:
                     self._values[k][0] += v * (current - self._seen_so_far)
                     self._values[k][1] += (current - self._seen_so_far)
             else:
                 self._values[k] = [v, 1]
         self._seen_so_far = current
 
         logs = collections.OrderedDict()
         for k in self._values:
             if isinstance(self._values[k], list):
-                avg = np.mean(
-                    self._values[k][0] / max(1, self._values[k][1]))
+                avg = np.mean(self._values[k][0] / max(1, self._values[k][1]))
+                self._smooth_values[k] = avg
                 if abs(avg) > 1e-3:
                     logs[k] = ' %.4f' % avg
                 else:
                     logs[k] = ' %.4e' % avg
             else:
                 logs[k] = ' %s' % self._values[k]
 
@@ -514,35 +529,34 @@
                 widgets.append(progressbar.Variable(param, precision=7))
                 if i < len(self.params['metrics'])-1:
                     widgets.append(' - ')
             self.progbar = progressbar.bar.ProgressBar(min_value=0, max_value=self.params['steps'], widgets=widgets, 
                                                        redirect_stdout=True, redirect_stderr=True)
         self.seen = 0
         self._values = collections.OrderedDict()
+        self._smooth_values = dict()
         self._seen_so_far = 0
 
-    def on_batch_begin(self, global_step=None, local_step=None, logs=None):
-        if self.seen < self.target:
-            self.log_values = []
-
     def on_batch_end(self, global_step=None, local_step=None, logs=None):
         self.seen += 1
-        logs = self.smooth_values(self.seen, logs or {})
-        logs_new = {k:logs[k].strip() for k in self.params['metrics'] if k in logs}
+        logs_new = self.smooth_values(self.seen, logs or {})
+        logs_new = {k:logs_new[k].strip() for k in self.params['metrics'] if k in logs_new}
 
         # Skip progbar update for the last batch;
         # will be handled by on_epoch_end.
         if self.verbose and self.seen < self.target:
             self.progbar.update(self.seen, **logs_new)
+            logs.update(self._smooth_values)
 
     def on_epoch_end(self, global_step=None, epoch=None, logs=None):
-        logs = self.smooth_values(self.seen, logs or {})
-        logs_new = {k:logs[k].strip() for k in self.params['metrics'] if k in logs}
+        logs_new = self.smooth_values(self.seen, logs or {})
+        logs_new = {k:logs_new[k].strip() for k in self.params['metrics'] if k in logs_new}
         if self.verbose:
             self.progbar.update(self.seen, **logs_new)
+            logs.update(self._smooth_values)
             self.progbar.finish()
     
 
 class History(Callback):
     """指标历史，默认是fit的返回项, 这里仅记录epoch_end的指标"""
     def on_train_begin(self, logs=None):
         self.epoch = []
@@ -911,20 +925,20 @@
     def on_train_end(self, logs=None):
         self.logger.info('Finish Training'.center(40, '='))
 
     def on_epoch_begin(self, global_step, epoch, logs=None):
         self.logger.info(f'Epoch {epoch+1}'.center(40, '='))
 
     def on_epoch_end(self, global_step, epoch, logs=None):
-        log_str = f'{self.sep}'.join([f'{k}={v:.5f}' for k, v in logs.items() if k not in {'size'}])
+        log_str = f'{self.sep}'.join([f'{k}={v:.5f}' for k, v in logs.items() if k not in SKIP_METRICS])
         self.logger.info(f'epoch={epoch+1}{self.sep}{log_str}')
 
     def on_batch_end(self, global_step, local_step, logs=None):
         if (global_step+1) % self.interval == 0:
-            log_str = f'{self.sep}'.join([f'{k}={v:.5f}' for k, v in logs.items() if k not in {'size'}])
+            log_str = f'{self.sep}'.join([f'{k}={v:.5f}' for k, v in logs.items() if k not in SKIP_METRICS])
             self.logger.info(f'step={global_step+1}{self.sep}{log_str}')
 
 
 class Tensorboard(Callback):
     '''默认Tensorboard
     对于valid/dev和test的Tensorboard需要在evaluate之后对log进行赋值，如log['dev/f1']=f1，并在Evaluator之后调用
     赋值需要分栏目的用'/'进行分隔
@@ -958,15 +972,15 @@
         # 默认记录的是global_step
         if (self.method == 'step') and ((global_step+1) % self.interval == 0):
             self.process(global_step+1, logs)
 
     def process(self, iteration, logs):
         logs = logs or {}
         for k, v in logs.items():
-            if k in {'size'}:
+            if k in SKIP_METRICS:
                 continue
             index = k if '/' in k else f"{self.prefix}{k}"
             self.writer.add_scalar(index, v, iteration)
 
 
 class LambdaCallback(Callback):
     """lambda表达式
@@ -1102,25 +1116,24 @@
             self.run_name = self.trial_name
         self.watch = watch
         self.interval = interval
         self.save_code = save_code
         self.config = config or {}
         self.run_id = None
         self.metrics = set()
-        self.hidden_metrics = {'size'}
 
     def define_metric(self, logs=None):
         if getattr(self._wandb, "define_metric", None):
             for m in logs.keys():
                 if m not in self.metrics:
-                    self._wandb.define_metric(name=m, step_metric=self.method, hidden=True if m in self.hidden_metrics else False)
+                    self._wandb.define_metric(name=m, step_metric=self.method, hidden=True if m in SKIP_METRICS else False)
                     self.metrics.add(m)
     def adjust_logs(self, logs, **kwargs):
         logs_new = {**logs, **kwargs}
-        return {k:v for k,v in logs_new.items() if k not in self.hidden_metrics}
+        return {k:v for k,v in logs_new.items() if k not in SKIP_METRICS}
 
     def on_epoch_end(self, global_step, epoch, logs=None):
         if self._wandb is None:
             return
         if self.method == 'epoch':
             self.define_metric(logs)
             self._wandb.log(self.adjust_logs(logs, epoch=epoch+1))
```

### Comparing `torch4keras-0.0.9/torch4keras/model.py` & `torch4keras-0.1.0/torch4keras/model.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from torch import nn
 import torch
-from torch4keras.snippets import DottableDict, metric_mapping, get_parameter_device, info_level_prefix, print_trainable_parameters
+from torch4keras.snippets import DottableDict, metric_mapping, get_parameter_device, log_info, log_warn, log_error, print_trainable_parameters, colorful
 from torch4keras.callbacks import KerasProgbar, TqdmProgbar, ProgressBar2Progbar, Callback, CallbackList, BaseLogger, History
 from collections import OrderedDict
 from inspect import isfunction
 import os
 import json
 import math
 
@@ -16,38 +16,45 @@
     """
     def __init__(self, module=None):
         super(Trainer, self).__init__()
         self.initialize(module)
     
     def initialize(self, module=None):
         # 这里主要是为了外面调用用到
-        self.global_step, self.local_step, self.total_steps, self.epoch, self.steps_per_epoch, self.train_dataloader = 0, 0, 0, 0, None, None
+        self.global_step, self.local_step, self.total_steps, self.batch_step, self.epoch, self.steps_per_epoch, self.train_dataloader = 0, 0, 0, 0, 0, None, None
         self.resume_step, self.resume_epoch = 0, 0
         self.retain_graph = False  # loss.backward()是否保留计算图
+        self.move_to_model_device = True  # 自动把tensor转到model所在的device
+        self.log_first_step = False  # 是否打印第一个step的数据
         self.callbacks = []
         # 传入Module实例方式
         if module is not None:
             assert isinstance(module, nn.Module), 'Args `module` only support nn.Module format'
             self.module = module
         # 是否运行Callbacks，目前主要是在DDP模式下运用
         self.run_callbacks = True
 
     def compile(self, loss, optimizer, scheduler=None, clip_grad_norm=None, mixed_precision=False, metrics=None, 
-                stateful_metrics=None, grad_accumulation_steps=1, **kwargs):
+                grad_accumulation_steps=1, progbar_config=None, **kwargs):
         '''complile: 定义loss, optimizer, metrics等参数
         
         :param loss: loss
         :param optimizer: 优化器
         :param scheduler: scheduler
         :param clip_grad_norm: bool, 是否使用梯度裁剪, 默认为False
         :param mixed_precision: bool, 是否使用混合精度，默认为False
         :param metrics: str/List[str]/dict, 训练过程中需要打印的指标, loss相关指标默认会打印, 目前支持accuracy, 也支持自定义metric，形式为{key: func}
-        :param stateful_metrics: List[str], 不滑动平均仅进行状态记录的metric，指标抖动会更加明显
         :param grad_accumulation_steps: int, 梯度累积步数，默认为1
         :param bar: str, 使用进度条的种类，从kwargs中解析，默认为keras, 可选keras, tqdm, progressbar2
+        :param progbar_config: 进度条的配置，如果使用指标平滑会更新到后续其他callbacks中（比如Logger），实现进度条显示和日志会保持一致
+            bar: str, 默认为keras
+            stateful_metrics: List[str], 表示不使用指标平滑仅进行状态记录的metric，指标抖动会更加明显，默认为None表示使用指标平滑
+            smooth_interval: int, 表示指标平滑时候的累计步数，默认为None表示对整个epoch进行平滑
+            width: int, keras进度条下表示进度条的长度
+
         :return: None
         '''
         self.criterion = loss
         self.optimizer = optimizer
         self.scheduler = scheduler
         self.clip_grad_norm = clip_grad_norm
         assert mixed_precision in {True, False, 'fp16', 'bf16'}
@@ -71,58 +78,85 @@
             elif isinstance(metric, dict):
                 self.metrics.update(metric)
             # 函数形式，key和value都赋值metric
             elif isfunction(metric):
                 self.metrics.update({metric: metric})
             else:
                 raise ValueError('Args metrics only support `String, Dict, Callback, List[String, Dict, Callback]` format')
-        self.stateful_metrics = stateful_metrics
 
         # 梯度累积
         self.grad_accumulation_steps = grad_accumulation_steps
 
         # 进度条参数
-        self.bar = kwargs.get('bar', 'keras')
-        assert self.bar in {'keras', 'tqdm', 'progressbar2'}, f'Args `bar`={self.bar} illegal, only support `keras, tqdm, progressbar2`'
-    
+        self.progbar_config = progbar_config or {'bar': 'keras', 'stateful_metrics': None}
+        progbar_config_keys = ['bar', 'stateful_metrics', 'smooth_interval', 'width']
+        self.progbar_config.update({k:v for k, v in kwargs.items() if k in progbar_config_keys})  # 直接传参也可以
+        self.progbar_config['bar'] = self.progbar_config.get('bar', 'keras')
+        assert self.progbar_config['bar'] in {'keras', 'tqdm', 'progressbar2'}, \
+            f'Args `bar`={self.progbar_config["bar"]} illegal, only support `keras, tqdm, progressbar2`'
+
     def print_trainable_parameters(self):
         """打印可训练的参数量"""
         print_trainable_parameters(self.unwrap_model())
 
     @property
     def device(self) -> torch.device:
         """获取model所在的device"""
         return get_parameter_device(self.unwrap_model())
         
-    def to_model_device(self, *inputs, **input_kwargs):
+    def _move_to_model_device(self, inputs, **input_kwargs):
         '''遍历并转移到model.device上'''
-        # TODO
-        pass
+        def _to_device(tensor):
+            if isinstance(tensor, torch.Tensor) and (tensor.device != self.device):
+                return tensor.to(self.device)
+            else:
+                return tensor
+
+        if self.move_to_model_device:
+            if isinstance(inputs, torch.Tensor):  # tensor不展开
+                inputs = _to_device(inputs)
+            elif isinstance(inputs, (tuple, list)):
+                inputs = [_to_device(i) for i in inputs]
+            
+            input_kwargs = {k: _to_device(v) for k, v in input_kwargs.items()}
+        return inputs, input_kwargs
+
+    def _log_first_step(self, resume_step):
+        '''打印第一个step的数据'''
+        if self.log_first_step and self.verbose and (self.global_step == resume_step):
+            print(colorful('[Train_data]: ', color='green'), + self.train_X)
+            print(colorful('[Label]: ', color='green'), + self.train_X)
 
     def _forward(self, *inputs, **input_kwargs):
-        # 如果传入了网络结构module，则调用module的forward
-        # 如果是继承方式，则调用自身的forward
-        if (len(inputs)==1) and isinstance(inputs[0], (tuple,list)):
+        '''调用模型的forward
+        如果传入了网络结构module，则调用module的forward；如果是继承方式，则调用自身的forward
+        '''
+        if (len(inputs)==1) and isinstance(inputs[0], (tuple,list)):  # 防止([])嵌套
             inputs = inputs[0]
+        inputs, input_kwargs = self._move_to_model_device(inputs, **input_kwargs)
+        
         if isinstance(inputs, torch.Tensor):  # tensor不展开
             return self.unwrap_model().forward(inputs, **input_kwargs)
         elif isinstance(inputs, (tuple, list)):
             return self.unwrap_model().forward(*inputs, **input_kwargs)
         else:
             return self.unwrap_model().forward(inputs, **input_kwargs)
 
     def train_step(self, train_X, train_y):
+        ''' Perform a training step on a batch of inputs. '''
+        self.train_y, _ = self._move_to_model_device(train_y)  # TODO: train_y可否是dict
+
         # 计算loss
         if self.mixed_precision:
             with self.autocast(dtype=torch.float16 if self.mixed_precision=='fp16' else torch.bfloat16):
                 output = self._forward(train_X)
-                loss_detail = self.criterion(output, train_y)
+                loss_detail = self.criterion(output, self.train_y)
         else:
             output = self._forward(train_X)
-            loss_detail = self.criterion(output, train_y)
+            loss_detail = self.criterion(output, self.train_y)
 
         # 整理loss
         if isinstance(loss_detail, torch.Tensor):
             loss = loss_detail
             loss_detail = {}
         elif isinstance(loss_detail, dict):
             loss = loss_detail['loss']  # 还存在其他loss，仅用于打印
@@ -196,27 +230,27 @@
             callbacks = []
         elif isinstance(callbacks, Callback):
             callbacks = [callbacks]
         for callback in callbacks:
             assert isinstance(callback, Callback), "Args `callbacks` only support Callback() inputs"
 
         history = History()
-        callbacks_ = [BaseLogger(self.stateful_metrics)]
+        callbacks_ = [BaseLogger(**self.progbar_config)]
 
         # 进度条
         progbarlogger = None
         if self.verbose:
-            if self.bar == 'keras':
-                progbarlogger = KerasProgbar(stateful_metrics=self.stateful_metrics)
-            elif self.bar == 'tqdm':
-                progbarlogger = TqdmProgbar(stateful_metrics=self.stateful_metrics)
-            elif self.bar == 'progressbar2':
-                progbarlogger = ProgressBar2Progbar(stateful_metrics=self.stateful_metrics)
+            if self.progbar_config['bar'] == 'keras':
+                progbarlogger = KerasProgbar(**self.progbar_config)
+            elif self.progbar_config['bar'] == 'tqdm':
+                progbarlogger = TqdmProgbar(**self.progbar_config)
+            elif self.progbar_config['bar'] == 'progressbar2':
+                progbarlogger = ProgressBar2Progbar(**self.progbar_config)
             else:
-                progbarlogger = KerasProgbar(stateful_metrics=self.stateful_metrics)
+                progbarlogger = KerasProgbar(**self.progbar_config)
             callbacks_.append(progbarlogger)
         callbacks_  += callbacks + [history]
         self.callbacks = CallbackList(callbacks_, run_callbacks=self.run_callbacks)
         callback_trainer = self
         callback_model = self.unwrap_model()
         params = {
             'epochs': self.epochs,
@@ -231,18 +265,19 @@
         return history, callback_trainer, progbarlogger
 
     def _prepare_nextbatch(self):
         '''准备下一个batch数据'''
         # 循环dataloader, 不要试用itertools的cycle，遇到过变量不释放的问题
         try:
             batch = next(self.train_dataloader_iter)
+            self.batch_step += 1
         except StopIteration:
             self.callbacks.on_dataloader_end()  # 适用于数据量较大时，动态读取文件并重新生成self.train_dataloader的情况，如预训练
             self.train_dataloader_iter = iter(self.train_dataloader)  # shuffle=True时候，其实顺序也重新生成了
-            self.bti = 0
+            self.batch_step = 0
             batch = next(self.train_dataloader_iter)
         return batch
 
     def fit(self, train_dataloader, steps_per_epoch=None, epochs=1, callbacks=None, verbose=1):
         '''模型训练
         
         :param train_dataloader: Dataloader, 训练数据集
@@ -254,19 +289,18 @@
         '''
         # 输入处理
         self._prepare_inputs(train_dataloader, steps_per_epoch, epochs, verbose)
 
         # 准备callbacks
         history, callback_trainer, progbarlogger  = self._prepare_callbacks(callbacks)
 
-        # epoch：当前epoch
-        # global_step：当前全局训练步数
-        # local_step: 当前epoch内的训练步数，不同epoch中相同local_step对应的batch数据不一定相同，在steps_per_epoch=None时相同
-        # bti：在dataloader中的index，不同epoch中相同的bti对应的batch数据一般相同，除非重新生成dataloader
-        self.bti = 0
+        #       epoch: 当前epoch
+        # global_step: 当前全局训练步数
+        #  local_step: 当前epoch内的训练步数，不同epoch中相同local_step对应的batch数据不一定相同，在steps_per_epoch=None时相同
+        #  batch_step: 在dataloader中的index，不同epoch中相同的bti对应的batch数据一般相同，除非重新生成dataloader
         for epoch in range(self.resume_epoch, epochs):
             self.epoch = epoch
             # resume_step：判断local_step的起点，以及进度条的起始位置
             resume_step = self.resume_step if epoch==self.resume_epoch else 0
             self.callbacks.on_epoch_begin(self.global_step, self.epoch)
             if self.verbose:
                 progbarlogger.seen = resume_step  # 这里设置进度条的seen，在callbacks中也会修改
@@ -278,14 +312,15 @@
                 self.callbacks.on_batch_begin(self.global_step, self.local_step, logs)
 
                 # forward和backward
                 self.unwrap_model().train()  # 设置为train模式
                 tr_loss, tr_loss_detail = 0, {}
                 for _ in range(self.grad_accumulation_steps):
                     self.train_X, self.train_y = self._prepare_nextbatch()  # 获取下一个batch的训练数据
+                    self._log_first_step(resume_step)  # log第一个step
                     self.output, self.loss, self.loss_detail = self.train_step(self.train_X, self.train_y)
                     self.callbacks.on_train_step_end()
                     tr_loss += self.loss.item()
                     for k, v in self.loss_detail.items():
                         tr_loss_detail[k] = tr_loss_detail.get(k, 0) + v
                 # TODO: 理论上梯度累积时需对output和train_y进行合并，主要是为了metric_mapping计算的准确
                 
@@ -306,15 +341,14 @@
                                 progbarlogger.add_metrics(list(perf.keys()))
                             logs.update(perf)
                         elif isinstance(metric, str):  # 直接传入回调函数(有key)
                             logs[metric] = perf
 
                 self.callbacks.on_batch_end(self.global_step, self.local_step, logs)
 
-                self.bti += 1
             self.callbacks.on_epoch_end(self.global_step, self.epoch, logs)
             # TerminateOnNaN、EarlyStopping等停止训练策略
             if callback_trainer.stop_training:
                 break
         self.callbacks.on_train_end(logs)
         return history
 
@@ -537,15 +571,15 @@
         super().__init__(module)
         from accelerate import Accelerator
         accelerator = Accelerator(**configs)
         self.model = accelerator.prepare(module)
         self.accelerator = accelerator
         self.device = accelerator.device
         self.verbose = 1 if accelerator.is_local_main_process else 0
-        print(info_level_prefix('AcclerateTrainer may not be compatible with several callbacks, you may use custom callbacks instead.', 1))
+        log_warn('AcclerateTrainer may not be compatible with several callbacks, you may use custom callbacks instead.')
     
     def compile(self, *args, **kwargs):
         super().compile(*args, **kwargs)
         self.optimizer, self.scheduler, self.criterion = self.accelerator.prepare(self.optimizer, self.scheduler, self.criterion)
 
     def _prepare_inputs(self, *args):
         super()._prepare_inputs(*args)
@@ -588,30 +622,30 @@
             "critical": logging.CRITICAL,
         }
 
         ds_logger.setLevel(log_levels.get(log_level, logging.WARNING))
 
         if inference:
             # only Z3 makes sense for the inference
-            info_level_prefix("ZeRO inference only makes sense with ZeRO Stage 3", 1)
+            log_warn("ZeRO inference only makes sense with ZeRO Stage 3")
             self.optimizer, self.scheduler = None, None
             model_parameters = None
         else:
             model_parameters = list(filter(lambda p: p.requires_grad, self.model.parameters()))
         
         kwargs = {
             "model": self.model,  # deepspeed的forward默认是计算到loss输出的
             "model_parameters": model_parameters,
             "config_params": self.config,
             "optimizer": self.optimizer,
             "lr_scheduler": self.scheduler,
         }
         if self.config.get('zero_optimization', {}).get('offload_optimizer', {}).get('device') == 'cpu':
             kwargs.pop('optimizer')
-            print(info_level_prefix('You may not use custom optimizer when offload_optimizer=`cpu`', 1))
+            log_warn('You may not use custom optimizer when offload_optimizer=`cpu`')
         self.deepspeed_engine, self.optimizer, _, self.scheduler = deepspeed.initialize(**kwargs)
         self.verbose = 1 if self.deepspeed_engine.local_rank == master_rank else 0
 
     def unwrap_model(self):
         # 执行deepspeed_engine的forward
         return self.deepspeed_engine
```

### Comparing `torch4keras-0.0.9/torch4keras/snippets.py` & `torch4keras-0.1.0/torch4keras/snippets.py`

 * *Files 9% similar despite different names*

```diff
@@ -183,15 +183,15 @@
     :param seed: int, 随机种子
     '''
     max_seed_value = np.iinfo(np.uint32).max
     min_seed_value = np.iinfo(np.uint32).min
 
     if (seed is None) or not (min_seed_value <= seed <= max_seed_value):
         seed = random.randint(np.iinfo(np.uint32).min, np.iinfo(np.uint32).max)
-    print(f"Global seed set to {seed}")
+    log_info(f"Global seed set to {seed}")
     os.environ["PYTHONHASHSEED"] = str(seed)
     random.seed(seed)
     np.random.seed(seed)
     torch.manual_seed(seed)
     torch.cuda.manual_seed(seed)
     torch.cuda.manual_seed_all(seed)
     torch.backends.cudnn.benchmark = False
@@ -244,17 +244,16 @@
         smtpObj = smtplib.SMTP() 
         smtpObj.connect(mail_host, 25)  # 连接到服务器
         smtpObj.login(mail_user, mail_pwd)  # 登录到服务器
         smtpObj.sendmail(sender, receivers, message.as_string())  # 发送
         smtpObj.quit()  # 退出
         print('[INFO] Send email success')
     except smtplib.SMTPException as e:
-        error = info_level_prefix('Send email error : '+str(e), 2)
-        print(error)
-        return error
+        log_error('Send email error : '+str(e))
+        return str(e)
 
 
 def email_when_error(receivers, **configs):
     """装饰器，异常则发邮件
     Example:
     --------
     @email_when_error(receivers='tongjilibo@163.com')
@@ -399,30 +398,30 @@
     接下来，该函数解析 nvidia-smi 命令的输出，并计算每个 GPU 设备的得分。得分由 GPU 利用率和可用内存计算得出。
     最后，该函数选择得分最高的 best_num 个 GPU 设备，并将其索引作为字符串连接起来。然后将环境变量 CUDA_VISIBLE_DEVICES 设置为该字符串并返回。
     """
     import subprocess
 
     # 无需重复设置
     if "CUDA_VISIBLE_DEVICES" in os.environ:
-        print(info_level_prefix("Environment variable `CUDA_VISIBLE_DEVICES` has already been set", 'w'))
+        log_warn("Environment variable `CUDA_VISIBLE_DEVICES` has already been set")
         return os.environ["CUDA_VISIBLE_DEVICES"]
 
     if best_num == -1:
-        print(info_level_prefix(f"SET CUDA_VISIBLE_DEVICES=-1"))
+        log_info(f"SET CUDA_VISIBLE_DEVICES=-1")
         os.environ["CUDA_VISIBLE_DEVICES"] = "-1"
         return "-1"
 
     try:
         p = subprocess.Popen(
             ["nvidia-smi",
              "--query-gpu=index,utilization.gpu,memory.total,memory.free",
              "--format=csv,noheader,nounits"],
             stdout=subprocess.PIPE)
     except FileNotFoundError:
-        print(info_level_prefix("`nvidia-smi` not exists"), 'e')
+        log_error("`nvidia-smi` not exists")
         os.environ["CUDA_VISIBLE_DEVICES"] = "-1"
         return "-1"
 
     if best_num is None:
         best_num = os.environ.get("LOCAL_WORLD_SIZE", 1)
     best_num = int(best_num)
 
@@ -440,11 +439,11 @@
         score = gpu_score + memory_score
         scores.append(score)
 
     best_num = min(best_num, len(scores))
     topk_idx = (-np.asarray(scores)).argsort()[:best_num]
 
     topk_idx_str = ",".join(map(str, topk_idx))
-    print(info_level_prefix(f"SET CUDA_VISIBLE_DEVICES={topk_idx_str}"))
+    log_info(f"SET CUDA_VISIBLE_DEVICES={topk_idx_str}")
     os.environ["CUDA_VISIBLE_DEVICES"] = topk_idx_str
 
     return topk_idx_str
```

### Comparing `torch4keras-0.0.9/torch4keras.egg-info/PKG-INFO` & `torch4keras-0.1.0/torch4keras.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: torch4keras
-Version: 0.0.9
+Version: 0.1.0
 Summary: Use torch like keras
 Home-page: https://github.com/Tongjilibo/torch4keras
 Author: Tongjilibo
 License: Apache License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# torch4keras
-**Use torch like keras**
+![torch4keras](https://github.com/Tongjilibo/torch4keras/blob/master/docs/pics/torch4keras.png)
+
 
 [![licence](https://img.shields.io/github/license/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/blob/master/LICENSE) 
 [![GitHub release](https://img.shields.io/github/release/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/releases) 
 [![PyPI](https://img.shields.io/pypi/v/torch4keras?label=pypi%20package)](https://pypi.org/project/torch4keras/) 
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/torch4keras)](https://pypistats.org/packages/torch4keras)
 [![GitHub stars](https://img.shields.io/github/stars/Tongjilibo/torch4keras?style=social)](https://github.com/Tongjilibo/torch4keras)
 [![GitHub Issues](https://img.shields.io/github/issues/Tongjilibo/torch4keras.svg)](https://github.com/Tongjilibo/torch4keras/issues)
@@ -71,28 +71,30 @@
     ```
 
 ## 3. 快速上手
 - 参考[bert4torch](https://github.com/Tongjilibo/bert4torch)的训练过程
 - 简单示例: [turorials_mnist](https://github.com/Tongjilibo/torch4keras/blob/master/examples/turorials_mnist.py)
 
 ## 4. 版本说明
+- **v0.1.0**: 允许调整进度条的显示参数, 进度条和日志同步（如果进度条平滑了则日志也平滑）, 自动把tensor转到model.device上, 允许打印第一个batch来检查样本
 - **v0.0.9**：20230716 增加auto_set_cuda_devices自动选择显卡，增加log_info，log_warn, log_error等小函数
 - **v0.0.8**：20230625 增加EmailCallback和WandbCallback, 增加AccelerateTrainer和DeepSpeedTrainer, grad_accumulation_steps内算一个batch，修改Trainer中部分成员函数
 - **v0.0.7.post3**: 20230517 修复保存scheduler
 - **v0.0.7.post2**: 20230517 Checkpoint Calback增加保存scheduler, save_weights可自行创建目录，Logger, Tensorboard模块加入lr, 修改predict和add_trainer
 - **v0.0.7**：20230505 独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
 - **v0.0.6**：20230212 增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现(增加几个成员变量、增加initilize()、删除对forward参数个数的判断、dp和ddp不解析module、修改use_amp参数为mixed_precision)，增加了AccelerateCallback
 - **v0.0.5**：20221217 增加Summary的Callback, 增加Tqdm的进度条展示，保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
 - **v0.0.4**：20221127 为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
 - **v0.0.3.post2**：20221107 修复DDP下打印的bug
 - **v0.0.3**：20221106 参考Keras修改了callback的逻辑
 - **v0.0.2**：20221023 增加Checkpoint, Evaluator等自带Callback, 修改BaseModel(net)方式，修复DP和DDP的__init__()
 - **v0.0.1**：20221019 初始版本
 
 ## 5. 更新：
+- **20230721**: 允许调整进度条的显示参数, 进度条和日志同步（如果进度条平滑了则日志也平滑）, 自动把tensor转到model.device上, 允许打印第一个batch来检查样本
 - **20230716**：增加auto_set_cuda_devices自动选择显卡，增加log_info，log_warn, log_error等小函数
 - **20230625**：增加EmailCallback和WandbCallback, 增加AccelerateTrainer和DeepSpeedTrainer, grad_accumulation_steps内算一个batch，修改Trainer中部分成员函数
 - **20230517**：Checkpoint Calback增加保存scheduler, save_weights可自行创建目录，Logger, Tensorboard模块加入lr, 修改predict和add_trainer
 - **20230505**：独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
 - **20230212**：增加hf的accelerator测试用例, ddp需要外部控制执行callback, 混合精度支持bf16
 - **20230116**：增加resume_from_checkpoint和save_to_checkpoint，动态为nn.Module增加Trainer的方法add_trainer
 - **20221217**：保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
```

