# Comparing `tmp/fast_bert-2.0.7.tar.gz` & `tmp/fast_bert-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_bert-2.0.7.tar", last modified: Tue Sep 20 14:00:14 2022, max compression
+gzip compressed data, was "fast_bert-2.0.9.tar", last modified: Thu Sep 22 11:35:32 2022, max compression
```

## Comparing `fast_bert-2.0.7.tar` & `fast_bert-2.0.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 kaushaltrivedi   (501) staff       (20)        0 2022-09-20 14:00:14.932412 fast_bert-2.0.7/
--rw-r--r--   0 kaushaltrivedi   (501) staff       (20)    11357 2022-04-11 22:58:20.000000 fast_bert-2.0.7/LICENSE
--rw-r--r--   0 kaushaltrivedi   (501) staff       (20)    23885 2022-09-20 14:00:14.932250 fast_bert-2.0.7/PKG-INFO
--rw-r--r--   0 kaushaltrivedi   (501) staff       (20)    23314 2022-04-11 22:58:20.000000 fast_bert-2.0.7/README.md
-drwxr-xr-x   0 kaushaltrivedi   (501) staff       (20)        0 2022-09-20 14:00:14.929789 fast_bert-2.0.7/fast_bert/
--rw-r--r--   0 kaushaltrivedi   (501) staff       (20)      809 2022-04-11 22:58:20.000000 fast_bert-2.0.7/fast_bert/__init__.py
--rw-r--r--   0 kaushaltrivedi   (501) staff       (20)      636 2022-04-11 22:58:20.000000 fast_bert-2.0.7/fast_bert/bert_layers.py
--rw-r--r--   0 kaushaltrivedi   (501) staff       (20)    19780 2022-04-11 22:58:20.000000 fast_bert-2.0.7/fast_bert/data.py
--rw-r--r--   0 kaushaltrivedi   (501) staff       (20)    12261 2022-04-11 22:58:20.000000 fast_bert-2.0.7/fast_bert/data_abs.py
--rw-r--r--   0 kaushaltrivedi   (501) staff       (20)    22127 2022-04-11 22:58:20.000000 fast_bert-2.0.7/fast_bert/data_cls.py
--rw-r--r--   0 kaushaltrivedi   (501) staff       (20)    11609 2022-04-11 22:58:20.000000 fast_bert-2.0.7/fast_bert/data_lm.py
--rw-r--r--   0 kaushaltrivedi   (501) staff       (20)    18574 2022-04-11 22:58:20.000000 fast_bert-2.0.7/fast_bert/data_ner.py
--rw-r--r--   0 kaushaltrivedi   (501) staff       (20)    26904 2022-04-11 22:58:20.000000 fast_bert-2.0.7/fast_bert/data_qa.py
--rw-r--r--   0 kaushaltrivedi   (501) staff       (20)     5819 2022-04-11 22:58:20.000000 fast_bert-2.0.7/fast_bert/learner_abs.py
--rw-r--r--   0 kaushaltrivedi   (501) staff       (20)    34679 2022-04-11 22:58:20.000000 fast_bert-2.0.7/fast_bert/learner_cls.py
--rw-r--r--   0 kaushaltrivedi   (501) staff       (20)    34168 2022-04-11 22:58:20.000000 fast_bert-2.0.7/fast_bert/learner_cls_old.py
--rw-r--r--   0 kaushaltrivedi   (501) staff       (20)    11865 2022-04-11 22:58:20.000000 fast_bert-2.0.7/fast_bert/learner_lm.py
--rw-r--r--   0 kaushaltrivedi   (501) staff       (20)    10700 2022-09-20 13:58:20.000000 fast_bert-2.0.7/fast_bert/learner_ner.py
--rw-r--r--   0 kaushaltrivedi   (501) staff       (20)    35024 2022-04-11 22:58:20.000000 fast_bert-2.0.7/fast_bert/learner_qa.py
--rw-r--r--   0 kaushaltrivedi   (501) staff       (20)     4304 2022-04-11 22:58:20.000000 fast_bert-2.0.7/fast_bert/learner_util.py
--rw-r--r--   0 kaushaltrivedi   (501) staff       (20)     3680 2022-04-11 22:58:20.000000 fast_bert-2.0.7/fast_bert/metrics.py
--rw-r--r--   0 kaushaltrivedi   (501) staff       (20)    18682 2022-04-11 22:58:20.000000 fast_bert-2.0.7/fast_bert/modeling.py
--rw-r--r--   0 kaushaltrivedi   (501) staff       (20)     1089 2022-04-11 22:58:20.000000 fast_bert-2.0.7/fast_bert/onnx_helper.py
--rw-r--r--   0 kaushaltrivedi   (501) staff       (20)    13028 2022-04-11 22:58:20.000000 fast_bert-2.0.7/fast_bert/optimization.py
--rw-r--r--   0 kaushaltrivedi   (501) staff       (20)     8819 2022-09-08 22:45:54.000000 fast_bert-2.0.7/fast_bert/prediction.py
-drwxr-xr-x   0 kaushaltrivedi   (501) staff       (20)        0 2022-09-20 14:00:14.931553 fast_bert-2.0.7/fast_bert/summarisation/
--rw-r--r--   0 kaushaltrivedi   (501) staff       (20)       69 2022-04-11 22:58:20.000000 fast_bert-2.0.7/fast_bert/summarisation/__init__.py
--rw-r--r--   0 kaushaltrivedi   (501) staff       (20)     3360 2022-04-11 22:58:20.000000 fast_bert-2.0.7/fast_bert/summarisation/configuration_bertabs.py
--rw-r--r--   0 kaushaltrivedi   (501) staff       (20)    41062 2022-04-11 22:58:20.000000 fast_bert-2.0.7/fast_bert/summarisation/modeling_bertabs.py
-drwxr-xr-x   0 kaushaltrivedi   (501) staff       (20)        0 2022-09-20 14:00:14.931990 fast_bert-2.0.7/fast_bert/utils/
--rw-r--r--   0 kaushaltrivedi   (501) staff       (20)       39 2022-04-11 22:58:20.000000 fast_bert-2.0.7/fast_bert/utils/__init__.py
--rw-r--r--   0 kaushaltrivedi   (501) staff       (20)      886 2022-04-11 22:58:20.000000 fast_bert-2.0.7/fast_bert/utils/spellcheck.py
--rw-r--r--   0 kaushaltrivedi   (501) staff       (20)    12491 2022-04-11 22:58:20.000000 fast_bert-2.0.7/fast_bert/utils_squad_evaluate.py
-drwxr-xr-x   0 kaushaltrivedi   (501) staff       (20)        0 2022-09-20 14:00:14.930728 fast_bert-2.0.7/fast_bert.egg-info/
--rw-r--r--   0 kaushaltrivedi   (501) staff       (20)    23885 2022-09-20 14:00:14.000000 fast_bert-2.0.7/fast_bert.egg-info/PKG-INFO
--rw-r--r--   0 kaushaltrivedi   (501) staff       (20)      912 2022-09-20 14:00:14.000000 fast_bert-2.0.7/fast_bert.egg-info/SOURCES.txt
--rw-r--r--   0 kaushaltrivedi   (501) staff       (20)        1 2022-09-20 14:00:14.000000 fast_bert-2.0.7/fast_bert.egg-info/dependency_links.txt
--rw-r--r--   0 kaushaltrivedi   (501) staff       (20)        1 2022-04-11 23:07:57.000000 fast_bert-2.0.7/fast_bert.egg-info/not-zip-safe
--rw-r--r--   0 kaushaltrivedi   (501) staff       (20)      161 2022-09-20 14:00:14.000000 fast_bert-2.0.7/fast_bert.egg-info/requires.txt
--rw-r--r--   0 kaushaltrivedi   (501) staff       (20)       10 2022-09-20 14:00:14.000000 fast_bert-2.0.7/fast_bert.egg-info/top_level.txt
--rw-r--r--   0 kaushaltrivedi   (501) staff       (20)       38 2022-09-20 14:00:14.932458 fast_bert-2.0.7/setup.cfg
--rw-r--r--   0 kaushaltrivedi   (501) staff       (20)      988 2022-09-20 13:59:43.000000 fast_bert-2.0.7/setup.py
+drwxr-xr-x   0 kaushaltrivedi   (501) staff       (20)        0 2022-09-22 11:35:32.377143 fast_bert-2.0.9/
+-rw-r--r--   0 kaushaltrivedi   (501) staff       (20)    11357 2022-04-11 22:58:20.000000 fast_bert-2.0.9/LICENSE
+-rw-r--r--   0 kaushaltrivedi   (501) staff       (20)    23885 2022-09-22 11:35:32.376916 fast_bert-2.0.9/PKG-INFO
+-rw-r--r--   0 kaushaltrivedi   (501) staff       (20)    23314 2022-04-11 22:58:20.000000 fast_bert-2.0.9/README.md
+drwxr-xr-x   0 kaushaltrivedi   (501) staff       (20)        0 2022-09-22 11:35:32.374372 fast_bert-2.0.9/fast_bert/
+-rw-r--r--   0 kaushaltrivedi   (501) staff       (20)      809 2022-04-11 22:58:20.000000 fast_bert-2.0.9/fast_bert/__init__.py
+-rw-r--r--   0 kaushaltrivedi   (501) staff       (20)      636 2022-04-11 22:58:20.000000 fast_bert-2.0.9/fast_bert/bert_layers.py
+-rw-r--r--   0 kaushaltrivedi   (501) staff       (20)    19780 2022-04-11 22:58:20.000000 fast_bert-2.0.9/fast_bert/data.py
+-rw-r--r--   0 kaushaltrivedi   (501) staff       (20)    12261 2022-04-11 22:58:20.000000 fast_bert-2.0.9/fast_bert/data_abs.py
+-rw-r--r--   0 kaushaltrivedi   (501) staff       (20)    22127 2022-04-11 22:58:20.000000 fast_bert-2.0.9/fast_bert/data_cls.py
+-rw-r--r--   0 kaushaltrivedi   (501) staff       (20)    11609 2022-04-11 22:58:20.000000 fast_bert-2.0.9/fast_bert/data_lm.py
+-rw-r--r--   0 kaushaltrivedi   (501) staff       (20)    19981 2022-09-22 11:09:25.000000 fast_bert-2.0.9/fast_bert/data_ner.py
+-rw-r--r--   0 kaushaltrivedi   (501) staff       (20)    26904 2022-04-11 22:58:20.000000 fast_bert-2.0.9/fast_bert/data_qa.py
+-rw-r--r--   0 kaushaltrivedi   (501) staff       (20)     5819 2022-04-11 22:58:20.000000 fast_bert-2.0.9/fast_bert/learner_abs.py
+-rw-r--r--   0 kaushaltrivedi   (501) staff       (20)    34679 2022-04-11 22:58:20.000000 fast_bert-2.0.9/fast_bert/learner_cls.py
+-rw-r--r--   0 kaushaltrivedi   (501) staff       (20)    34168 2022-04-11 22:58:20.000000 fast_bert-2.0.9/fast_bert/learner_cls_old.py
+-rw-r--r--   0 kaushaltrivedi   (501) staff       (20)    11865 2022-04-11 22:58:20.000000 fast_bert-2.0.9/fast_bert/learner_lm.py
+-rw-r--r--   0 kaushaltrivedi   (501) staff       (20)    12814 2022-09-22 11:24:23.000000 fast_bert-2.0.9/fast_bert/learner_ner.py
+-rw-r--r--   0 kaushaltrivedi   (501) staff       (20)    35024 2022-04-11 22:58:20.000000 fast_bert-2.0.9/fast_bert/learner_qa.py
+-rw-r--r--   0 kaushaltrivedi   (501) staff       (20)     4304 2022-04-11 22:58:20.000000 fast_bert-2.0.9/fast_bert/learner_util.py
+-rw-r--r--   0 kaushaltrivedi   (501) staff       (20)     3680 2022-04-11 22:58:20.000000 fast_bert-2.0.9/fast_bert/metrics.py
+-rw-r--r--   0 kaushaltrivedi   (501) staff       (20)    18682 2022-04-11 22:58:20.000000 fast_bert-2.0.9/fast_bert/modeling.py
+-rw-r--r--   0 kaushaltrivedi   (501) staff       (20)     1089 2022-04-11 22:58:20.000000 fast_bert-2.0.9/fast_bert/onnx_helper.py
+-rw-r--r--   0 kaushaltrivedi   (501) staff       (20)    13028 2022-04-11 22:58:20.000000 fast_bert-2.0.9/fast_bert/optimization.py
+-rw-r--r--   0 kaushaltrivedi   (501) staff       (20)     8819 2022-09-08 22:45:54.000000 fast_bert-2.0.9/fast_bert/prediction.py
+drwxr-xr-x   0 kaushaltrivedi   (501) staff       (20)        0 2022-09-22 11:35:32.375865 fast_bert-2.0.9/fast_bert/summarisation/
+-rw-r--r--   0 kaushaltrivedi   (501) staff       (20)       69 2022-04-11 22:58:20.000000 fast_bert-2.0.9/fast_bert/summarisation/__init__.py
+-rw-r--r--   0 kaushaltrivedi   (501) staff       (20)     3360 2022-04-11 22:58:20.000000 fast_bert-2.0.9/fast_bert/summarisation/configuration_bertabs.py
+-rw-r--r--   0 kaushaltrivedi   (501) staff       (20)    41062 2022-04-11 22:58:20.000000 fast_bert-2.0.9/fast_bert/summarisation/modeling_bertabs.py
+drwxr-xr-x   0 kaushaltrivedi   (501) staff       (20)        0 2022-09-22 11:35:32.376570 fast_bert-2.0.9/fast_bert/utils/
+-rw-r--r--   0 kaushaltrivedi   (501) staff       (20)       39 2022-04-11 22:58:20.000000 fast_bert-2.0.9/fast_bert/utils/__init__.py
+-rw-r--r--   0 kaushaltrivedi   (501) staff       (20)      886 2022-04-11 22:58:20.000000 fast_bert-2.0.9/fast_bert/utils/spellcheck.py
+-rw-r--r--   0 kaushaltrivedi   (501) staff       (20)    12491 2022-04-11 22:58:20.000000 fast_bert-2.0.9/fast_bert/utils_squad_evaluate.py
+drwxr-xr-x   0 kaushaltrivedi   (501) staff       (20)        0 2022-09-22 11:35:32.375379 fast_bert-2.0.9/fast_bert.egg-info/
+-rw-r--r--   0 kaushaltrivedi   (501) staff       (20)    23885 2022-09-22 11:35:32.000000 fast_bert-2.0.9/fast_bert.egg-info/PKG-INFO
+-rw-r--r--   0 kaushaltrivedi   (501) staff       (20)      912 2022-09-22 11:35:32.000000 fast_bert-2.0.9/fast_bert.egg-info/SOURCES.txt
+-rw-r--r--   0 kaushaltrivedi   (501) staff       (20)        1 2022-09-22 11:35:32.000000 fast_bert-2.0.9/fast_bert.egg-info/dependency_links.txt
+-rw-r--r--   0 kaushaltrivedi   (501) staff       (20)        1 2022-04-11 23:07:57.000000 fast_bert-2.0.9/fast_bert.egg-info/not-zip-safe
+-rw-r--r--   0 kaushaltrivedi   (501) staff       (20)      161 2022-09-22 11:35:32.000000 fast_bert-2.0.9/fast_bert.egg-info/requires.txt
+-rw-r--r--   0 kaushaltrivedi   (501) staff       (20)       10 2022-09-22 11:35:32.000000 fast_bert-2.0.9/fast_bert.egg-info/top_level.txt
+-rw-r--r--   0 kaushaltrivedi   (501) staff       (20)       38 2022-09-22 11:35:32.377205 fast_bert-2.0.9/setup.cfg
+-rw-r--r--   0 kaushaltrivedi   (501) staff       (20)      988 2022-09-22 11:25:22.000000 fast_bert-2.0.9/setup.py
```

### Comparing `fast_bert-2.0.7/LICENSE` & `fast_bert-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_bert-2.0.7/PKG-INFO` & `fast_bert-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast_bert
-Version: 2.0.7
+Version: 2.0.9
 Summary: AI Library using BERT
 Home-page: https://github.com/kaushaltrivedi/fast-bert
 Author: Kaushal Trivedi
 Author-email: kaushaltrivedi@me.com
 License: Apache2
 Keywords: BERT NLP deep learning google
 Platform: UNKNOWN
```

### Comparing `fast_bert-2.0.7/README.md` & `fast_bert-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `fast_bert-2.0.7/fast_bert/__init__.py` & `fast_bert-2.0.9/fast_bert/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_bert-2.0.7/fast_bert/bert_layers.py` & `fast_bert-2.0.9/fast_bert/bert_layers.py`

 * *Files identical despite different names*

### Comparing `fast_bert-2.0.7/fast_bert/data.py` & `fast_bert-2.0.9/fast_bert/data.py`

 * *Files identical despite different names*

### Comparing `fast_bert-2.0.7/fast_bert/data_abs.py` & `fast_bert-2.0.9/fast_bert/data_abs.py`

 * *Files identical despite different names*

### Comparing `fast_bert-2.0.7/fast_bert/data_cls.py` & `fast_bert-2.0.9/fast_bert/data_cls.py`

 * *Files identical despite different names*

### Comparing `fast_bert-2.0.7/fast_bert/data_lm.py` & `fast_bert-2.0.9/fast_bert/data_lm.py`

 * *Files identical despite different names*

### Comparing `fast_bert-2.0.7/fast_bert/data_ner.py` & `fast_bert-2.0.9/fast_bert/data_ner.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,14 +75,15 @@
     def __init__(
         self,
         data_dir: str,
         file_name: str,
         tokenizer,
         labels: List[str],
         model_type: str,
+        texts=None,
         max_seq_length: Optional[int] = None,
         overwrite_cache=False,
         mode: Split = Split.train,
         logger=logging.getLogger(__name__),
     ):
         # # Load data features from cache or dataset file
         # cached_features_file = os.path.join(
@@ -183,14 +184,15 @@
         logger=logging.getLogger(),
         clear_cache=False,
         no_cache=False,
         use_fast_tokenizer=True,
         custom_sampler=None,
         train_size=0.8,
         random_state=None,
+        test_file_name=None
     ):
         DATA_PATH = Path(data_dir)
 
         labels = []
 
         with open(DATA_PATH / file_name, "r") as f:
             lines = f.readlines()
@@ -199,14 +201,24 @@
                 for label in line["labels"]:
                     labels.append(label[2])
 
         train, val = train_test_split(
             lines, train_size=train_size, random_state=random_state
         )
 
+        if test_file_name is not None:
+            try:
+                with open(DATA_PATH / test_file_name, "r") as f:
+                    test_lines = f.readlines()
+                    modified_test = flatten_all(convert_data(test_lines))
+                    json_to_text(modified_test, str(DATA_PATH / "test.txt"))
+            except FileNotFoundError:
+                logger.info("Test file not found, skipping")
+                test_lines = None
+
         modified_train = convert_data(train)
         modified_val = convert_data(val)
 
         modified_train = flatten_all(modified_train)
         json_to_text(modified_train, str(DATA_PATH / "train.txt"))
 
         modified_val = flatten_all(modified_val)
@@ -234,14 +246,15 @@
 
     def __init__(
         self,
         data_dir,
         tokenizer,
         train_file="train.txt",
         val_file="val.txt",
+        test_file="test.txt",
         label_file="labels.txt",
         batch_size_per_gpu=16,
         max_seq_length=512,
         multi_gpu=True,
         backend="nccl",
         model_type="bert",
         logger=logging.getLogger(),
@@ -319,14 +332,36 @@
 
             self.val_batch_size = self.batch_size_per_gpu * 2 * max(1, self.n_gpu)
             val_sampler = SequentialSampler(val_dataset)
             self.val_dl = DataLoader(
                 val_dataset, sampler=val_sampler, batch_size=self.val_batch_size
             )
 
+        try:
+            if test_file:
+                test_dataset = NerDataset(
+                    data_dir=data_dir,
+                    file_name=test_file,
+                    tokenizer=tokenizer,
+                    labels=self.labels,
+                    model_type=self.model_type,
+                    max_seq_length=max_seq_length,
+                    overwrite_cache=clear_cache,
+                    mode=Split.test,
+                )
+
+                self.test_batch_size = self.batch_size_per_gpu * 2 * max(1, self.n_gpu)
+                test_sampler = SequentialSampler(test_dataset)
+                self.test_dl = DataLoader(
+                    test_dataset, sampler=test_sampler, batch_size=self.test_batch_size
+                )
+        except FileNotFoundError:
+            self.logger.info("Test file not found, skipping")
+            self.test_dl = None
+
 
 def convert_examples_to_features(
     examples: List[InputExample],
     label_list: List[str],
     max_seq_length: int,
     tokenizer: PreTrainedTokenizer,
     cls_token_at_end=False,
```

### Comparing `fast_bert-2.0.7/fast_bert/data_qa.py` & `fast_bert-2.0.9/fast_bert/data_qa.py`

 * *Files identical despite different names*

### Comparing `fast_bert-2.0.7/fast_bert/learner_abs.py` & `fast_bert-2.0.9/fast_bert/learner_abs.py`

 * *Files identical despite different names*

### Comparing `fast_bert-2.0.7/fast_bert/learner_cls.py` & `fast_bert-2.0.9/fast_bert/learner_cls.py`

 * *Files identical despite different names*

### Comparing `fast_bert-2.0.7/fast_bert/learner_cls_old.py` & `fast_bert-2.0.9/fast_bert/learner_cls_old.py`

 * *Files identical despite different names*

### Comparing `fast_bert-2.0.7/fast_bert/learner_lm.py` & `fast_bert-2.0.9/fast_bert/learner_lm.py`

 * *Files identical despite different names*

### Comparing `fast_bert-2.0.7/fast_bert/learner_ner.py` & `fast_bert-2.0.9/fast_bert/learner_ner.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import logging
 import torch
 import numpy as np
 from .data_ner import BertNERDataBunch
 from torch import nn
 from seqeval.metrics import f1_score, precision_score, recall_score
 from typing import Dict, List, Optional, Tuple
 from .learner_util import Learner
@@ -181,14 +182,75 @@
             self.logger.info("Running evaluation")
             self.logger.info("  Num examples = %d", len(self.data.val_dl.dataset))
             self.logger.info("  Batch size = %d", self.data.val_batch_size)
 
         result = self.get_trainer().evaluate()
         return result
 
+    ### Return Predictions ###
+    def predict_batch(self, group=True, exclude_entities=["O"], return_metrics=True, verbose=True):
+
+        if verbose:
+            if self.logger is None:
+                self.logger = logging.getLogger(__name__)
+        
+        if self.data.test_dl:
+            dl = self.data.test_dl
+        else:
+            dl = self.data.val_dl
+
+        label_list = self.data.labels
+        tokenizer = self.data.tokenizer
+        results = self.get_trainer().predict(test_dataset=dl.dataset)
+        outputs = torch.Tensor(results.predictions)
+        outputs = outputs.softmax(dim=2)
+        predictions = torch.argmax(outputs, dim=2)
+
+        preds = []
+        for index, prediction in enumerate(predictions):
+            text = tokenizer.decode(dl.dataset[index].input_ids, skip_special_tokens=True)
+            tokens = tokenizer.tokenize(tokenizer.decode(tokenizer.encode(text)))
+
+            processed_pred = [
+                (token, label_list[pred], out[pred])
+                for token, out, pred in zip(
+                    tokens, outputs[index].tolist(), prediction.tolist()
+                )
+            ][1:-1]
+
+            processed_pred = [
+                {
+                    "index": index,
+                    "word": pred[0],
+                    "entity": pred[1],
+                    "score": pred[2],
+                }
+                for index, pred in enumerate(processed_pred)
+            ]
+            if group is True:
+                processed_pred = group_entities(processed_pred)
+
+            out_preds = []
+            for pred in processed_pred:
+                if pred["entity"] not in exclude_entities:
+                    try:
+                        pred["entity"] = pred["entity"].split("-")[1]
+                    except Exception:
+                        pass
+
+                    out_preds.append(pred)
+
+            preds.append({"text": text, "labels": out_preds})
+        out_res = {
+            "predictions": preds,
+        }
+        if return_metrics:
+            out_res["metrics"] = results.metrics
+        return out_res
+
     def predict(self, text, group=True, exclude_entities=["O"]):
         if exclude_entities is None:
             exclude_entities = []
         label_list = self.data.labels
 
         tokenizer = self.data.tokenizer
         tokens = tokenizer.tokenize(tokenizer.decode(tokenizer.encode(text)))
```

### Comparing `fast_bert-2.0.7/fast_bert/learner_qa.py` & `fast_bert-2.0.9/fast_bert/learner_qa.py`

 * *Files identical despite different names*

### Comparing `fast_bert-2.0.7/fast_bert/learner_util.py` & `fast_bert-2.0.9/fast_bert/learner_util.py`

 * *Files identical despite different names*

### Comparing `fast_bert-2.0.7/fast_bert/metrics.py` & `fast_bert-2.0.9/fast_bert/metrics.py`

 * *Files identical despite different names*

### Comparing `fast_bert-2.0.7/fast_bert/modeling.py` & `fast_bert-2.0.9/fast_bert/modeling.py`

 * *Files identical despite different names*

### Comparing `fast_bert-2.0.7/fast_bert/onnx_helper.py` & `fast_bert-2.0.9/fast_bert/onnx_helper.py`

 * *Files identical despite different names*

### Comparing `fast_bert-2.0.7/fast_bert/optimization.py` & `fast_bert-2.0.9/fast_bert/optimization.py`

 * *Files identical despite different names*

### Comparing `fast_bert-2.0.7/fast_bert/prediction.py` & `fast_bert-2.0.9/fast_bert/prediction.py`

 * *Files identical despite different names*

### Comparing `fast_bert-2.0.7/fast_bert/summarisation/configuration_bertabs.py` & `fast_bert-2.0.9/fast_bert/summarisation/configuration_bertabs.py`

 * *Files identical despite different names*

### Comparing `fast_bert-2.0.7/fast_bert/summarisation/modeling_bertabs.py` & `fast_bert-2.0.9/fast_bert/summarisation/modeling_bertabs.py`

 * *Files identical despite different names*

### Comparing `fast_bert-2.0.7/fast_bert/utils/spellcheck.py` & `fast_bert-2.0.9/fast_bert/utils/spellcheck.py`

 * *Files identical despite different names*

### Comparing `fast_bert-2.0.7/fast_bert/utils_squad_evaluate.py` & `fast_bert-2.0.9/fast_bert/utils_squad_evaluate.py`

 * *Files identical despite different names*

### Comparing `fast_bert-2.0.7/fast_bert.egg-info/PKG-INFO` & `fast_bert-2.0.9/fast_bert.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-bert
-Version: 2.0.7
+Version: 2.0.9
 Summary: AI Library using BERT
 Home-page: https://github.com/kaushaltrivedi/fast-bert
 Author: Kaushal Trivedi
 Author-email: kaushaltrivedi@me.com
 License: Apache2
 Keywords: BERT NLP deep learning google
 Platform: UNKNOWN
```

### Comparing `fast_bert-2.0.7/fast_bert.egg-info/SOURCES.txt` & `fast_bert-2.0.9/fast_bert.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fast_bert-2.0.7/setup.py` & `fast_bert-2.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 with open("requirements.txt") as f:
     install_requires = f.read().strip().split("\n")
 
 setup(
     name="fast_bert",
-    version="2.0.7",
+    version="2.0.9",
     description="AI Library using BERT",
     author="Kaushal Trivedi",
     author_email="kaushaltrivedi@me.com",
     license="Apache2",
     url="https://github.com/kaushaltrivedi/fast-bert",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
```

