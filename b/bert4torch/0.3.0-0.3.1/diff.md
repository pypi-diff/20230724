# Comparing `tmp/bert4torch-0.3.0.tar.gz` & `tmp/bert4torch-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bert4torch-0.3.0.tar", last modified: Sun Jul 16 11:37:02 2023, max compression
+gzip compressed data, was "bert4torch-0.3.1.tar", last modified: Mon Jul 24 16:10:44 2023, max compression
```

## Comparing `bert4torch-0.3.0.tar` & `bert4torch-0.3.1.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 11:37:02.416569 bert4torch-0.3.0/
--rw-rw-rw-   0        0        0     1089 2022-03-12 16:30:24.000000 bert4torch-0.3.0/LICENSE
--rw-rw-rw-   0        0        0    25777 2023-07-16 11:37:02.415552 bert4torch-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0    25525 2023-07-16 10:38:17.000000 bert4torch-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 11:37:02.382552 bert4torch-0.3.0/bert4torch/
--rw-rw-rw-   0        0        0        0 2022-11-28 12:30:45.000000 bert4torch-0.3.0/bert4torch/__init__.py
--rw-rw-rw-   0        0        0     3228 2023-06-30 17:02:35.000000 bert4torch-0.3.0/bert4torch/activations.py
--rw-rw-rw-   0        0        0    10939 2023-07-06 12:55:22.000000 bert4torch-0.3.0/bert4torch/callbacks.py
--rw-rw-rw-   0        0        0    40578 2023-07-16 10:39:25.000000 bert4torch-0.3.0/bert4torch/generation.py
-drwxrwxrwx   0        0        0        0 2023-07-16 11:37:02.395563 bert4torch-0.3.0/bert4torch/layers/
--rw-rw-rw-   0        0        0      296 2023-07-06 12:55:22.000000 bert4torch-0.3.0/bert4torch/layers/__init__.py
--rw-rw-rw-   0        0        0    25425 2023-07-16 09:13:49.000000 bert4torch-0.3.0/bert4torch/layers/attention.py
--rw-rw-rw-   0        0        0     8515 2023-07-15 16:04:22.000000 bert4torch-0.3.0/bert4torch/layers/core.py
--rw-rw-rw-   0        0        0    12699 2023-07-06 12:55:22.000000 bert4torch-0.3.0/bert4torch/layers/crf.py
--rw-rw-rw-   0        0        0     4474 2023-07-06 12:55:22.000000 bert4torch-0.3.0/bert4torch/layers/global_point.py
--rw-rw-rw-   0        0        0    17108 2023-07-11 14:03:23.000000 bert4torch-0.3.0/bert4torch/layers/misc.py
--rw-rw-rw-   0        0        0    14305 2023-07-16 10:41:24.000000 bert4torch-0.3.0/bert4torch/layers/position_encoding.py
--rw-rw-rw-   0        0        0    16283 2023-07-11 14:03:23.000000 bert4torch-0.3.0/bert4torch/layers/transformer_block.py
--rw-rw-rw-   0        0        0    16631 2023-06-26 16:27:26.000000 bert4torch-0.3.0/bert4torch/losses.py
-drwxrwxrwx   0        0        0        0 2023-07-16 11:37:02.414553 bert4torch-0.3.0/bert4torch/models/
--rw-rw-rw-   0        0        0     7651 2023-07-14 15:19:38.000000 bert4torch-0.3.0/bert4torch/models/__init__.py
--rw-rw-rw-   0        0        0     7811 2023-07-06 12:55:22.000000 bert4torch-0.3.0/bert4torch/models/albert.py
--rw-rw-rw-   0        0        0     6913 2023-07-06 12:55:22.000000 bert4torch-0.3.0/bert4torch/models/bart.py
--rw-rw-rw-   0        0        0    20254 2023-07-16 10:07:15.000000 bert4torch-0.3.0/bert4torch/models/base.py
--rw-rw-rw-   0        0        0    18082 2023-07-11 14:03:23.000000 bert4torch-0.3.0/bert4torch/models/bert.py
--rw-rw-rw-   0        0        0     4283 2023-07-06 12:55:22.000000 bert4torch-0.3.0/bert4torch/models/deberta.py
--rw-rw-rw-   0        0        0     2233 2023-07-06 12:55:22.000000 bert4torch-0.3.0/bert4torch/models/electra.py
--rw-rw-rw-   0        0        0      932 2023-07-06 12:55:22.000000 bert4torch-0.3.0/bert4torch/models/erinie.py
--rw-rw-rw-   0        0        0     1728 2023-07-11 14:03:23.000000 bert4torch-0.3.0/bert4torch/models/gau_alpha.py
--rw-rw-rw-   0        0        0    12236 2023-07-14 14:25:09.000000 bert4torch-0.3.0/bert4torch/models/glm.py
--rw-rw-rw-   0        0        0     7917 2023-07-11 14:03:23.000000 bert4torch-0.3.0/bert4torch/models/gpt.py
--rw-rw-rw-   0        0        0     4535 2023-07-15 10:36:15.000000 bert4torch-0.3.0/bert4torch/models/llama.py
--rw-rw-rw-   0        0        0      457 2023-07-06 12:55:22.000000 bert4torch-0.3.0/bert4torch/models/nezha.py
--rw-rw-rw-   0        0        0     2399 2023-07-11 14:03:23.000000 bert4torch-0.3.0/bert4torch/models/roformer.py
--rw-rw-rw-   0        0        0    10276 2023-07-11 14:03:23.000000 bert4torch-0.3.0/bert4torch/models/t5.py
--rw-rw-rw-   0        0        0     5268 2023-07-06 12:55:22.000000 bert4torch-0.3.0/bert4torch/models/transformer.py
--rw-rw-rw-   0        0        0     9217 2023-07-06 12:55:22.000000 bert4torch-0.3.0/bert4torch/models/transformer_xl.py
--rw-rw-rw-   0        0        0     2469 2023-07-06 12:55:22.000000 bert4torch-0.3.0/bert4torch/models/uie.py
--rw-rw-rw-   0        0        0     4802 2023-07-06 12:55:22.000000 bert4torch-0.3.0/bert4torch/models/xlnet.py
--rw-rw-rw-   0        0        0     7619 2023-03-29 15:35:29.000000 bert4torch-0.3.0/bert4torch/optimizers.py
--rw-rw-rw-   0        0        0    20808 2023-07-16 10:34:11.000000 bert4torch-0.3.0/bert4torch/quantization.py
--rw-rw-rw-   0        0        0    23410 2023-07-16 10:34:24.000000 bert4torch-0.3.0/bert4torch/snippets.py
--rw-rw-rw-   0        0        0    35456 2023-07-13 15:00:01.000000 bert4torch-0.3.0/bert4torch/tokenizers.py
-drwxrwxrwx   0        0        0        0 2023-07-16 11:37:02.387556 bert4torch-0.3.0/bert4torch.egg-info/
--rw-rw-rw-   0        0        0    25777 2023-07-16 11:37:02.000000 bert4torch-0.3.0/bert4torch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1196 2023-07-16 11:37:02.000000 bert4torch-0.3.0/bert4torch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 11:37:02.000000 bert4torch-0.3.0/bert4torch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-07-16 11:37:02.000000 bert4torch-0.3.0/bert4torch.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-16 11:37:02.000000 bert4torch-0.3.0/bert4torch.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 11:37:02.417566 bert4torch-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      551 2023-07-16 10:05:26.000000 bert4torch-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 16:10:44.773348 bert4torch-0.3.1/
+-rw-rw-rw-   0        0        0     1089 2022-03-12 16:30:24.000000 bert4torch-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0    27568 2023-07-24 16:10:44.771352 bert4torch-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0    27316 2023-07-24 16:05:28.000000 bert4torch-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 16:10:44.728347 bert4torch-0.3.1/bert4torch/
+-rw-rw-rw-   0        0        0        0 2022-11-28 12:30:45.000000 bert4torch-0.3.1/bert4torch/__init__.py
+-rw-rw-rw-   0        0        0     3228 2023-06-30 17:02:35.000000 bert4torch-0.3.1/bert4torch/activations.py
+-rw-rw-rw-   0        0        0    10939 2023-07-06 12:55:22.000000 bert4torch-0.3.1/bert4torch/callbacks.py
+-rw-rw-rw-   0        0        0    40539 2023-07-19 13:35:56.000000 bert4torch-0.3.1/bert4torch/generation.py
+drwxrwxrwx   0        0        0        0 2023-07-24 16:10:44.743347 bert4torch-0.3.1/bert4torch/layers/
+-rw-rw-rw-   0        0        0      296 2023-07-06 12:55:22.000000 bert4torch-0.3.1/bert4torch/layers/__init__.py
+-rw-rw-rw-   0        0        0    25499 2023-07-19 14:29:14.000000 bert4torch-0.3.1/bert4torch/layers/attention.py
+-rw-rw-rw-   0        0        0     8515 2023-07-15 16:04:22.000000 bert4torch-0.3.1/bert4torch/layers/core.py
+-rw-rw-rw-   0        0        0    12699 2023-07-06 12:55:22.000000 bert4torch-0.3.1/bert4torch/layers/crf.py
+-rw-rw-rw-   0        0        0     4738 2023-07-20 15:32:46.000000 bert4torch-0.3.1/bert4torch/layers/global_point.py
+-rw-rw-rw-   0        0        0    17536 2023-07-22 13:42:00.000000 bert4torch-0.3.1/bert4torch/layers/misc.py
+-rw-rw-rw-   0        0        0    13868 2023-07-19 14:29:40.000000 bert4torch-0.3.1/bert4torch/layers/position_encoding.py
+-rw-rw-rw-   0        0        0    16281 2023-07-21 13:58:57.000000 bert4torch-0.3.1/bert4torch/layers/transformer_block.py
+-rw-rw-rw-   0        0        0    16631 2023-06-26 16:27:26.000000 bert4torch-0.3.1/bert4torch/losses.py
+drwxrwxrwx   0        0        0        0 2023-07-24 16:10:44.768351 bert4torch-0.3.1/bert4torch/models/
+-rw-rw-rw-   0        0        0     7712 2023-07-18 14:14:06.000000 bert4torch-0.3.1/bert4torch/models/__init__.py
+-rw-rw-rw-   0        0        0     7811 2023-07-06 12:55:22.000000 bert4torch-0.3.1/bert4torch/models/albert.py
+-rw-rw-rw-   0        0        0     6913 2023-07-06 12:55:22.000000 bert4torch-0.3.1/bert4torch/models/bart.py
+-rw-rw-rw-   0        0        0    20254 2023-07-16 10:07:15.000000 bert4torch-0.3.1/bert4torch/models/base.py
+-rw-rw-rw-   0        0        0    18082 2023-07-11 14:03:23.000000 bert4torch-0.3.1/bert4torch/models/bert.py
+-rw-rw-rw-   0        0        0      760 2023-07-22 15:51:05.000000 bert4torch-0.3.1/bert4torch/models/bloom.py
+-rw-rw-rw-   0        0        0     4283 2023-07-06 12:55:22.000000 bert4torch-0.3.1/bert4torch/models/deberta.py
+-rw-rw-rw-   0        0        0     2233 2023-07-06 12:55:22.000000 bert4torch-0.3.1/bert4torch/models/electra.py
+-rw-rw-rw-   0        0        0      932 2023-07-06 12:55:22.000000 bert4torch-0.3.1/bert4torch/models/erinie.py
+-rw-rw-rw-   0        0        0     1728 2023-07-11 14:03:23.000000 bert4torch-0.3.1/bert4torch/models/gau_alpha.py
+-rw-rw-rw-   0        0        0    10808 2023-07-22 14:30:17.000000 bert4torch-0.3.1/bert4torch/models/glm.py
+-rw-rw-rw-   0        0        0     4566 2023-07-22 13:03:58.000000 bert4torch-0.3.1/bert4torch/models/gpt.py
+-rw-rw-rw-   0        0        0     2294 2023-07-22 13:18:50.000000 bert4torch-0.3.1/bert4torch/models/llama.py
+-rw-rw-rw-   0        0        0      457 2023-07-06 12:55:22.000000 bert4torch-0.3.1/bert4torch/models/nezha.py
+-rw-rw-rw-   0        0        0     2399 2023-07-11 14:03:23.000000 bert4torch-0.3.1/bert4torch/models/roformer.py
+-rw-rw-rw-   0        0        0    10336 2023-07-21 13:58:57.000000 bert4torch-0.3.1/bert4torch/models/t5.py
+-rw-rw-rw-   0        0        0     6769 2023-07-22 13:26:18.000000 bert4torch-0.3.1/bert4torch/models/transformer.py
+-rw-rw-rw-   0        0        0     9219 2023-07-20 15:32:46.000000 bert4torch-0.3.1/bert4torch/models/transformer_xl.py
+-rw-rw-rw-   0        0        0     2469 2023-07-06 12:55:22.000000 bert4torch-0.3.1/bert4torch/models/uie.py
+-rw-rw-rw-   0        0        0     4808 2023-07-20 15:32:46.000000 bert4torch-0.3.1/bert4torch/models/xlnet.py
+-rw-rw-rw-   0        0        0     7619 2023-03-29 15:35:29.000000 bert4torch-0.3.1/bert4torch/optimizers.py
+-rw-rw-rw-   0        0        0    20808 2023-07-16 10:34:11.000000 bert4torch-0.3.1/bert4torch/quantization.py
+-rw-rw-rw-   0        0        0    23410 2023-07-16 10:34:24.000000 bert4torch-0.3.1/bert4torch/snippets.py
+-rw-rw-rw-   0        0        0    35456 2023-07-13 15:00:01.000000 bert4torch-0.3.1/bert4torch/tokenizers.py
+drwxrwxrwx   0        0        0        0 2023-07-24 16:10:44.732346 bert4torch-0.3.1/bert4torch.egg-info/
+-rw-rw-rw-   0        0        0    27568 2023-07-24 16:10:44.000000 bert4torch-0.3.1/bert4torch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1223 2023-07-24 16:10:44.000000 bert4torch-0.3.1/bert4torch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 16:10:44.000000 bert4torch-0.3.1/bert4torch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-07-24 16:10:44.000000 bert4torch-0.3.1/bert4torch.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-24 16:10:44.000000 bert4torch-0.3.1/bert4torch.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 16:10:44.774347 bert4torch-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      551 2023-07-24 16:05:33.000000 bert4torch-0.3.1/setup.py
```

### Comparing `bert4torch-0.3.0/LICENSE` & `bert4torch-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.0/PKG-INFO` & `bert4torch-0.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bert4torch
-Version: 0.3.0
+Version: 0.3.1
 Summary: an elegant bert4torch
 Home-page: https://github.com/Tongjilibo/bert4torch
 Author: Tongjilibo
 License: MIT Licence
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -39,21 +39,20 @@
 
 - **注意事项**：pip包的发布慢于git上的开发版本，git clone**注意引用路径**，注意权重是否需要转换
 - **测试用例**：`git clone https://github.com/Tongjilibo/bert4torch`，修改example中的预训练模型文件路径和数据路径即可启动脚本
 - **自行训练**：针对自己的数据，修改相应的数据处理代码块
 - **开发环境**：原使用`torch==1.10`版本进行开发，现已切换到`torch2.0`开发，如其他版本遇到不适配，欢迎反馈
 
 ## 2. 功能
-
-- **LLM模型**: 加载chatglm-6b和llama-7b进行推理和finetune
+- **LLM模型**: 加载chatglm、llama、 baichuan、ziya、bloom等开源大模型权重进行推理和微调
 - **核心功能**：加载bert、roberta、albert、xlnet、nezha、bart、RoFormer、RoFormer_V2、ELECTRA、GPT、GPT2、T5、GAU-alpha、ERNIE等预训练权重继续进行finetune、并支持在bert基础上灵活定义自己模型
-- [**丰富示例**](https://github.com/Tongjilibo/bert4torch/blob/master/examples/)：包含[pretrain](https://github.com/Tongjilibo/bert4torch/blob/master/examples/pretrain)、[sentence_classfication](https://github.com/Tongjilibo/bert4torch/blob/master/examples/sentence_classfication)、[sentence_embedding](https://github.com/Tongjilibo/bert4torch/tree/master/examples/sentence_embedding)、[sequence_labeling](https://github.com/Tongjilibo/bert4torch/blob/master/examples/sequence_labeling)、[relation_extraction](https://github.com/Tongjilibo/bert4torch/blob/master/examples/relation_extraction)、[seq2seq](https://github.com/Tongjilibo/bert4torch/blob/master/examples/seq2seq)、[serving](https://github.com/Tongjilibo/bert4torch/blob/master/examples/serving/)等多种解决方案
+- [**丰富示例**](https://github.com/Tongjilibo/bert4torch/blob/master/examples/)：包含[llm](https://github.com/Tongjilibo/bert4torch/blob/master/examples/llm)、[pretrain](https://github.com/Tongjilibo/bert4torch/blob/master/examples/pretrain)、[sentence_classfication](https://github.com/Tongjilibo/bert4torch/blob/master/examples/sentence_classfication)、[sentence_embedding](https://github.com/Tongjilibo/bert4torch/tree/master/examples/sentence_embedding)、[sequence_labeling](https://github.com/Tongjilibo/bert4torch/blob/master/examples/sequence_labeling)、[relation_extraction](https://github.com/Tongjilibo/bert4torch/blob/master/examples/relation_extraction)、[seq2seq](https://github.com/Tongjilibo/bert4torch/blob/master/examples/seq2seq)、[serving](https://github.com/Tongjilibo/bert4torch/blob/master/examples/serving/)等多种解决方案
 - **实验验证**：已在公开数据集实验验证，使用如下[examples数据集](https://github.com/Tongjilibo/bert4torch/blob/master/examples/README.md)
 - **易用trick**：集成了常见的[trick](https://github.com/Tongjilibo/bert4torch/blob/master/examples/training_trick)，即插即用
-- **其他特性**：[加载transformers库模型](https://github.com/Tongjilibo/bert4torch/blob/master/examples/tutorials/tutorials_load_transformers_model.py)一起使用；调用方式简洁高效；有训练进度条动态展示；配合torchinfo打印参数量；默认Logger和Tensorboard简便记录训练过程；自定义fit过程，满足高阶需求
+- **其他特性**：[加载transformers库模型](https://github.com/Tongjilibo/bert4torch/blob/master//tutorials/tutorials_load_transformers_model.py)一起使用；调用方式简洁高效；有训练进度条动态展示；配合torchinfo打印参数量；默认Logger和Tensorboard简便记录训练过程；自定义fit过程，满足高阶需求
 - **训练过程**：
 
   ```text
   2022-10-28 23:16:10 - Start Training
   2022-10-28 23:16:10 - Epoch: 1/2
   5000/5000 [==============================] - 13s 3ms/step - loss: 0.1351 - acc: 0.9601
   Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 798.09it/s] 
@@ -63,25 +62,38 @@
   5000/5000 [==============================] - 13s 3ms/step - loss: 0.0465 - acc: 0.9862
   Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 635.78it/s] 
   test_acc: 0.98280. best_test_acc: 0.98280
 
   2022-10-28 23:16:44 - Finish Training
   ```
 
+|          功能                | bert4torch |  transformers | 备注 |
+|-----------------------------|------------|:--------------|--------|
+|训练进度条                     | ✅         |      ✅        |进度条打印loss和定义的metrics|
+|分布式训练dp/ddp               | ✅         |      ✅        |torch自带dp/ddp|
+|各类callbacks                 | ✅         |      ✅        |日志/tensorboard/earlystop/wandb等|
+|大模型推理，stream/batch输出    | ✅         |      ✅        |各个模型是通用的，无需单独维护脚本|
+|大模型微调                     | ✅         |      ✅        |lora依赖peft库，pv2自带|
+|丰富tricks                    | ✅         |      ❌        |对抗训练等tricks即插即用|
+|代码简洁易懂，自定义空间大        | ✅         |      ❌        |代码复用度高, keras代码训练风格|
+|仓库的维护能力/影响力/使用量/兼容性| ❌         |      ✅        |目前仓库个人维护|
+
+
 ## 3. 快速上手
 
 - [Quick-Start](https://bert4torch.readthedocs.io/en/latest//Quick-Start.html)
-- [快速上手教程](https://github.com/Tongjilibo/bert4torch/blob/master/examples/tutorials/Tutorials.md)，[教程示例](https://github.com/Tongjilibo/bert4torch/blob/master/examples/tutorials)，[实战示例](https://github.com/Tongjilibo/bert4torch/blob/master/examples)
+- [快速上手教程](https://github.com/Tongjilibo/bert4torch/blob/master//tutorials/README.md)，[教程示例](https://github.com/Tongjilibo/bert4torch/blob/master//tutorials)，[实战示例](https://github.com/Tongjilibo/bert4torch/blob/master/examples)
 - [bert4torch介绍(知乎)](https://zhuanlan.zhihu.com/p/486329434)，[bert4torch快速上手(知乎)](https://zhuanlan.zhihu.com/p/508890807)，[bert4torch又双叒叕更新啦(知乎)](https://zhuanlan.zhihu.com/p/560885427?)
 
 ## 4. 版本历史
 
 <details><summary><b>点击查看</b></summary>
 
 **版本说明**
+- **v0.3.1**：20230725 修改baichuan的alibi逻辑，增加bloom, 简化decoder架构代码(gpt, llama, chatglm均继承decoder)
 - **v0.3.0**：20230716 修改models和layers为文件夹方便扩展, 增加flash_attention参数控制，修改skip_init逻辑减少显存占用，generation增加repetition_penalty，修复chatglm的pv2的bug，generation支持transformers的tokenize，增加ziya，Baichuan
 - **v0.2.9**: 20230705 使用accelerate来实现skip_init精简代码, 修复add_trainer的代码提示, 增加chatglm的load_in_8bit+lora/qlora的训练, 修复grad_chechpoint, 增加chinese_llama_alpaca, torch2.0默认使用scaled_dot_product_attention加速, 增加chatglm2-6b+pv2+lora微调
 - **v0.2.8**：20230518 【新增模型】增加chatglm-6b/llama-7b/BELLE_llama/vicuna/moss/苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型/fnlp的bart2.0, 增加量化模块并适配llama，增加skip_init参数加快加载, 增加stream输出/网页demo, 增加ptuning_v2和lora; 【generation】生成式解码新增SeqGeneration和Seq2SeqGeneration，单向decoder模型和encoder decoder模型解码增加cache, 增加batch_generate()/stream_generate功能；【其他】修改rope为不使用max_position，修复model.half()类型不一致问题，支持加载多个权重文件, gpt系列默认不加softmax，增加苏神Tiger的pytorch实现, 增加了对attention_key_size的入参支持，把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段
 - **v0.2.7.post2**：20230310 增加lion优化器, 修复albert_unshared加载权重, 修复lm系列(gpt, seq2seq)存在的forward参数不对的问题，修复GlobalPointer使用rope的bug
 - **v0.2.7**：20230213 修复random_sample()的bug，适配v0.0.6的torch4keras：增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现，增加了AccelerateCallback
 - **v0.2.6**：20221231 build_transformer_model需显式指定add_trainer才从BaseModel继承, 增加guwenbert, macbert，text2vec-bert-chinese, wobert预训练模型，允许position_ids从padding开始, transformer.configs支持点操作，可以使用torch4keras的Trainer(net)来初始化, 修复tokenizer的切分subtoken的bug, 允许embedding_size!=hidden_size
 - **v0.2.5**：20221127 对抗训练从compile转为使用Callback来实现，修复1.7.1版本兼容bug, uie模型内置
@@ -98,14 +110,15 @@
 - **v0.1.4**：20220421 增加了VAT，修复了linux下apply_embedding返回项有问题的情况
 - **v0.1.3**：20220409 初始版本
 
 **版本对应关系**
 
 | bert4torch版本 | torch4keras版本 |
 | ---------------- | ----------------- |
+| 0.3.1          | 0.1.0           |
 | 0.3.0          | 0.0.9           |
 | 0.2.9          | 0.0.8           |
 | 0.2.8          | 0.0.7.post3     |
 | 0.2.7.post2    | 0.0.6           |
 | 0.2.7          | 0.0.6           |
 | 0.2.6          | 0.0.5           |
 | 0.2.5          | 0.0.4           |
@@ -115,14 +128,15 @@
 
 </details>
 
 
 ## 5. 更新历史：
 <details><summary><b>点击查看</b></summary>
 
+- **20230725**：修改baichuan的alibi逻辑，增加bloom, 简化decoder架构代码(gpt, llama, chatglm均继承decoder)
 - **20230716**：修改models和layers为文件夹方便扩展, 增加flash_attention参数控制，增加chatglm-api示例，修改skip_init逻辑减少显存占用，generation增加repetition_penalty，修复chatglm的pv2的bug，generation支持transformers的tokenize，增加ziya，Baichuan
 - **20230705**：使用accelerate来实现skip_init精简代码, 修复add_trainer的代码提示, 增加chatglm的load_in_8bit+lora/qlora的训练, 修复grad_chechpoint, 增加chinese_llama_alpaca, torch2.0默认使用scaled_dot_product_attention加速, 增加chatglm2-6b+pv2+lora微调
 - **20230518**：增加vicuna的集成, 增加batch_generate()功能, 把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段
 - **20230408**：增加苏神Tiger的pytorch实现, 集成苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型, 增加了对attention_key_size的入参支持，单向decoder模型和encoder decoder模型解码增加cache, 更新fnlp的bart2.0, 增加chatglm-6b预训练模型推理, 集成BELLE_llama模型, 增加量化模块并适配llama，增加skip_init参数加快加载, 增加stream输出/网页demo, 增加ptuning_v2，增加moss模型的int4/int8推理
 - **20230326**：增加llama-7b预训练模型, 修改rope为不使用max_position, 增加prompt_clue和nezha_gpt_dialog的finetune示例(skykiseki用户)，修复model.half()类型不一致问题，生成式解码新增SeqGeneration和Seq2SeqGeneration, 支持加载多个权重文件, gpt系列默认不加softmax
 - **20230310**：增加lion优化器, 修改dp和ddp示例更易用，增加PromptCLUE模型, 修复albert_unshared加载权重, 增加uer-gpt2-chinese预训练模型，修复lm系列(gpt, seq2seq)存在的forward参数不对的问题，修复GlobalPointer使用rope的bug
 - **20230212**：兼容accelerate包, 增加ChatYuan v1模型，修复random_sample()的bug
@@ -192,19 +206,22 @@
 | bart| 复旦| [torch](https://github.com/fastnlp/CPT), [v1.0](https://huggingface.co/fnlp/bart-base-chinese/tree/v1.0), [v2.0](https://huggingface.co/fnlp/bart-base-chinese/tree/v2.0)| [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_bart_fudanNLP.py) |
 | text2vec| text2vec-base-chinese | [torch](https://huggingface.co/shibing624/text2vec-base-chinese) | |
 | chatyuan v1&v2| clue-ai | [torch](https://github.com/clue-ai/ChatYuan) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
 | PromptCLUE| clue-ai | [torch](https://github.com/clue-ai/PromptCLUE) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
 | chatglm-6b | THUDM | [git](https://github.com/THUDM/ChatGLM-6B), [v0.1.0](https://huggingface.co/THUDM/chatglm-6b/tree/v0.1.0), [v1.1.0](https://huggingface.co/THUDM/chatglm-6b/tree/v1.1.0), [int8](https://huggingface.co/THUDM/chatglm-6b-int8), [int4](https://huggingface.co/THUDM/chatglm-6b-int4) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_chatglm.py) |
 | chatglm2-6b | THUDM | [git](https://github.com/THUDM/ChatGLM2-6B), [v2](https://huggingface.co/THUDM/chatglm2-6b), [int4](https://huggingface.co/THUDM/chatglm2-6b-int4) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_chatglm.py) |
 | llama | facebook| [git](https://github.com/facebookresearch/llama) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_pth.py)|
+| llama2 | facebook| [git](https://github.com/facebookresearch/llama) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_hf.py)|
 |chinese_llama_alpaca|Yiming Cui|[git](https://github.com/ymcui/Chinese-LLaMA-Alpaca) |[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_pth.py)|
 | vicuna | FastChat| [torch](https://huggingface.co/AlekseyKorshuk/vicuna-7b) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_hf.py)|
 | Belle_llama| LianjiaTech| [git](https://github.com/LianjiaTech/BELLE), [7B-2M-enc](https://huggingface.co/BelleGroup/BELLE-LLaMA-7B-2M-enc) | [合成说明](https://github.com/LianjiaTech/BELLE/tree/main/models)、[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_hf.py)|
 | Ziya | IDEA-CCNL | [v1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-v1), [v1.1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-v1.1), [pretrain-v1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-Pretrain-v1) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_pth.py) |
 | Baichuan | baichuan-inc | [7B](https://github.com/baichuan-inc/Baichuan-7B), [13B-Base](https://huggingface.co/baichuan-inc/Baichuan-13B-Base), [13B-Chat](https://huggingface.co/baichuan-inc/Baichuan-13B-Chat) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_hf.py) |
+| bloom | bigscience | [560m](https://huggingface.co/bigscience/bloom-560m) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_bloom.py) |
+
 
 ## 7. 鸣谢
 
 - 感谢苏神实现的[bert4keras](https://github.com/bojone/bert4keras)，本实现有不少地方参考了bert4keras的源码，在此衷心感谢大佬的无私奉献;
 - 其次感谢项目[bert4pytorch](https://github.com/MuQiuJun-AI/bert4pytorch)，也是在该项目的指引下给了我用pytorch来复现bert4keras的想法和思路。
 
 ## 8. 引用
```

### Comparing `bert4torch-0.3.0/README.md` & `bert4torch-0.3.1/bert4torch.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: bert4torch
+Version: 0.3.1
+Summary: an elegant bert4torch
+Home-page: https://github.com/Tongjilibo/bert4torch
+Author: Tongjilibo
+License: MIT Licence
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![bert4torch](https://github.com/Tongjilibo/bert4torch/blob/master/docs/pics/bert4torch.png)
 
 [![licence](https://img.shields.io/github/license/Tongjilibo/bert4torch.svg?maxAge=3600)](https://github.com/Tongjilibo/bert4torch/blob/master/LICENSE)
 [![GitHub release](https://img.shields.io/github/release/Tongjilibo/bert4torch.svg?maxAge=3600)](https://github.com/Tongjilibo/bert4torch/releases)
 [![PyPI](https://img.shields.io/pypi/v/bert4torch?label=pypi%20package)](https://pypi.org/project/bert4torch/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/bert4torch)](https://pypistats.org/packages/bert4torch)
 [![GitHub stars](https://img.shields.io/github/stars/Tongjilibo/bert4torch?style=social)](https://github.com/Tongjilibo/bert4torch)
@@ -29,21 +39,20 @@
 
 - **注意事项**：pip包的发布慢于git上的开发版本，git clone**注意引用路径**，注意权重是否需要转换
 - **测试用例**：`git clone https://github.com/Tongjilibo/bert4torch`，修改example中的预训练模型文件路径和数据路径即可启动脚本
 - **自行训练**：针对自己的数据，修改相应的数据处理代码块
 - **开发环境**：原使用`torch==1.10`版本进行开发，现已切换到`torch2.0`开发，如其他版本遇到不适配，欢迎反馈
 
 ## 2. 功能
-
-- **LLM模型**: 加载chatglm-6b和llama-7b进行推理和finetune
+- **LLM模型**: 加载chatglm、llama、 baichuan、ziya、bloom等开源大模型权重进行推理和微调
 - **核心功能**：加载bert、roberta、albert、xlnet、nezha、bart、RoFormer、RoFormer_V2、ELECTRA、GPT、GPT2、T5、GAU-alpha、ERNIE等预训练权重继续进行finetune、并支持在bert基础上灵活定义自己模型
-- [**丰富示例**](https://github.com/Tongjilibo/bert4torch/blob/master/examples/)：包含[pretrain](https://github.com/Tongjilibo/bert4torch/blob/master/examples/pretrain)、[sentence_classfication](https://github.com/Tongjilibo/bert4torch/blob/master/examples/sentence_classfication)、[sentence_embedding](https://github.com/Tongjilibo/bert4torch/tree/master/examples/sentence_embedding)、[sequence_labeling](https://github.com/Tongjilibo/bert4torch/blob/master/examples/sequence_labeling)、[relation_extraction](https://github.com/Tongjilibo/bert4torch/blob/master/examples/relation_extraction)、[seq2seq](https://github.com/Tongjilibo/bert4torch/blob/master/examples/seq2seq)、[serving](https://github.com/Tongjilibo/bert4torch/blob/master/examples/serving/)等多种解决方案
+- [**丰富示例**](https://github.com/Tongjilibo/bert4torch/blob/master/examples/)：包含[llm](https://github.com/Tongjilibo/bert4torch/blob/master/examples/llm)、[pretrain](https://github.com/Tongjilibo/bert4torch/blob/master/examples/pretrain)、[sentence_classfication](https://github.com/Tongjilibo/bert4torch/blob/master/examples/sentence_classfication)、[sentence_embedding](https://github.com/Tongjilibo/bert4torch/tree/master/examples/sentence_embedding)、[sequence_labeling](https://github.com/Tongjilibo/bert4torch/blob/master/examples/sequence_labeling)、[relation_extraction](https://github.com/Tongjilibo/bert4torch/blob/master/examples/relation_extraction)、[seq2seq](https://github.com/Tongjilibo/bert4torch/blob/master/examples/seq2seq)、[serving](https://github.com/Tongjilibo/bert4torch/blob/master/examples/serving/)等多种解决方案
 - **实验验证**：已在公开数据集实验验证，使用如下[examples数据集](https://github.com/Tongjilibo/bert4torch/blob/master/examples/README.md)
 - **易用trick**：集成了常见的[trick](https://github.com/Tongjilibo/bert4torch/blob/master/examples/training_trick)，即插即用
-- **其他特性**：[加载transformers库模型](https://github.com/Tongjilibo/bert4torch/blob/master/examples/tutorials/tutorials_load_transformers_model.py)一起使用；调用方式简洁高效；有训练进度条动态展示；配合torchinfo打印参数量；默认Logger和Tensorboard简便记录训练过程；自定义fit过程，满足高阶需求
+- **其他特性**：[加载transformers库模型](https://github.com/Tongjilibo/bert4torch/blob/master//tutorials/tutorials_load_transformers_model.py)一起使用；调用方式简洁高效；有训练进度条动态展示；配合torchinfo打印参数量；默认Logger和Tensorboard简便记录训练过程；自定义fit过程，满足高阶需求
 - **训练过程**：
 
   ```text
   2022-10-28 23:16:10 - Start Training
   2022-10-28 23:16:10 - Epoch: 1/2
   5000/5000 [==============================] - 13s 3ms/step - loss: 0.1351 - acc: 0.9601
   Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 798.09it/s] 
@@ -53,25 +62,38 @@
   5000/5000 [==============================] - 13s 3ms/step - loss: 0.0465 - acc: 0.9862
   Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 635.78it/s] 
   test_acc: 0.98280. best_test_acc: 0.98280
 
   2022-10-28 23:16:44 - Finish Training
   ```
 
+|          功能                | bert4torch |  transformers | 备注 |
+|-----------------------------|------------|:--------------|--------|
+|训练进度条                     | ✅         |      ✅        |进度条打印loss和定义的metrics|
+|分布式训练dp/ddp               | ✅         |      ✅        |torch自带dp/ddp|
+|各类callbacks                 | ✅         |      ✅        |日志/tensorboard/earlystop/wandb等|
+|大模型推理，stream/batch输出    | ✅         |      ✅        |各个模型是通用的，无需单独维护脚本|
+|大模型微调                     | ✅         |      ✅        |lora依赖peft库，pv2自带|
+|丰富tricks                    | ✅         |      ❌        |对抗训练等tricks即插即用|
+|代码简洁易懂，自定义空间大        | ✅         |      ❌        |代码复用度高, keras代码训练风格|
+|仓库的维护能力/影响力/使用量/兼容性| ❌         |      ✅        |目前仓库个人维护|
+
+
 ## 3. 快速上手
 
 - [Quick-Start](https://bert4torch.readthedocs.io/en/latest//Quick-Start.html)
-- [快速上手教程](https://github.com/Tongjilibo/bert4torch/blob/master/examples/tutorials/Tutorials.md)，[教程示例](https://github.com/Tongjilibo/bert4torch/blob/master/examples/tutorials)，[实战示例](https://github.com/Tongjilibo/bert4torch/blob/master/examples)
+- [快速上手教程](https://github.com/Tongjilibo/bert4torch/blob/master//tutorials/README.md)，[教程示例](https://github.com/Tongjilibo/bert4torch/blob/master//tutorials)，[实战示例](https://github.com/Tongjilibo/bert4torch/blob/master/examples)
 - [bert4torch介绍(知乎)](https://zhuanlan.zhihu.com/p/486329434)，[bert4torch快速上手(知乎)](https://zhuanlan.zhihu.com/p/508890807)，[bert4torch又双叒叕更新啦(知乎)](https://zhuanlan.zhihu.com/p/560885427?)
 
 ## 4. 版本历史
 
 <details><summary><b>点击查看</b></summary>
 
 **版本说明**
+- **v0.3.1**：20230725 修改baichuan的alibi逻辑，增加bloom, 简化decoder架构代码(gpt, llama, chatglm均继承decoder)
 - **v0.3.0**：20230716 修改models和layers为文件夹方便扩展, 增加flash_attention参数控制，修改skip_init逻辑减少显存占用，generation增加repetition_penalty，修复chatglm的pv2的bug，generation支持transformers的tokenize，增加ziya，Baichuan
 - **v0.2.9**: 20230705 使用accelerate来实现skip_init精简代码, 修复add_trainer的代码提示, 增加chatglm的load_in_8bit+lora/qlora的训练, 修复grad_chechpoint, 增加chinese_llama_alpaca, torch2.0默认使用scaled_dot_product_attention加速, 增加chatglm2-6b+pv2+lora微调
 - **v0.2.8**：20230518 【新增模型】增加chatglm-6b/llama-7b/BELLE_llama/vicuna/moss/苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型/fnlp的bart2.0, 增加量化模块并适配llama，增加skip_init参数加快加载, 增加stream输出/网页demo, 增加ptuning_v2和lora; 【generation】生成式解码新增SeqGeneration和Seq2SeqGeneration，单向decoder模型和encoder decoder模型解码增加cache, 增加batch_generate()/stream_generate功能；【其他】修改rope为不使用max_position，修复model.half()类型不一致问题，支持加载多个权重文件, gpt系列默认不加softmax，增加苏神Tiger的pytorch实现, 增加了对attention_key_size的入参支持，把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段
 - **v0.2.7.post2**：20230310 增加lion优化器, 修复albert_unshared加载权重, 修复lm系列(gpt, seq2seq)存在的forward参数不对的问题，修复GlobalPointer使用rope的bug
 - **v0.2.7**：20230213 修复random_sample()的bug，适配v0.0.6的torch4keras：增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现，增加了AccelerateCallback
 - **v0.2.6**：20221231 build_transformer_model需显式指定add_trainer才从BaseModel继承, 增加guwenbert, macbert，text2vec-bert-chinese, wobert预训练模型，允许position_ids从padding开始, transformer.configs支持点操作，可以使用torch4keras的Trainer(net)来初始化, 修复tokenizer的切分subtoken的bug, 允许embedding_size!=hidden_size
 - **v0.2.5**：20221127 对抗训练从compile转为使用Callback来实现，修复1.7.1版本兼容bug, uie模型内置
@@ -88,14 +110,15 @@
 - **v0.1.4**：20220421 增加了VAT，修复了linux下apply_embedding返回项有问题的情况
 - **v0.1.3**：20220409 初始版本
 
 **版本对应关系**
 
 | bert4torch版本 | torch4keras版本 |
 | ---------------- | ----------------- |
+| 0.3.1          | 0.1.0           |
 | 0.3.0          | 0.0.9           |
 | 0.2.9          | 0.0.8           |
 | 0.2.8          | 0.0.7.post3     |
 | 0.2.7.post2    | 0.0.6           |
 | 0.2.7          | 0.0.6           |
 | 0.2.6          | 0.0.5           |
 | 0.2.5          | 0.0.4           |
@@ -105,14 +128,15 @@
 
 </details>
 
 
 ## 5. 更新历史：
 <details><summary><b>点击查看</b></summary>
 
+- **20230725**：修改baichuan的alibi逻辑，增加bloom, 简化decoder架构代码(gpt, llama, chatglm均继承decoder)
 - **20230716**：修改models和layers为文件夹方便扩展, 增加flash_attention参数控制，增加chatglm-api示例，修改skip_init逻辑减少显存占用，generation增加repetition_penalty，修复chatglm的pv2的bug，generation支持transformers的tokenize，增加ziya，Baichuan
 - **20230705**：使用accelerate来实现skip_init精简代码, 修复add_trainer的代码提示, 增加chatglm的load_in_8bit+lora/qlora的训练, 修复grad_chechpoint, 增加chinese_llama_alpaca, torch2.0默认使用scaled_dot_product_attention加速, 增加chatglm2-6b+pv2+lora微调
 - **20230518**：增加vicuna的集成, 增加batch_generate()功能, 把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段
 - **20230408**：增加苏神Tiger的pytorch实现, 集成苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型, 增加了对attention_key_size的入参支持，单向decoder模型和encoder decoder模型解码增加cache, 更新fnlp的bart2.0, 增加chatglm-6b预训练模型推理, 集成BELLE_llama模型, 增加量化模块并适配llama，增加skip_init参数加快加载, 增加stream输出/网页demo, 增加ptuning_v2，增加moss模型的int4/int8推理
 - **20230326**：增加llama-7b预训练模型, 修改rope为不使用max_position, 增加prompt_clue和nezha_gpt_dialog的finetune示例(skykiseki用户)，修复model.half()类型不一致问题，生成式解码新增SeqGeneration和Seq2SeqGeneration, 支持加载多个权重文件, gpt系列默认不加softmax
 - **20230310**：增加lion优化器, 修改dp和ddp示例更易用，增加PromptCLUE模型, 修复albert_unshared加载权重, 增加uer-gpt2-chinese预训练模型，修复lm系列(gpt, seq2seq)存在的forward参数不对的问题，修复GlobalPointer使用rope的bug
 - **20230212**：兼容accelerate包, 增加ChatYuan v1模型，修复random_sample()的bug
@@ -182,19 +206,22 @@
 | bart| 复旦| [torch](https://github.com/fastnlp/CPT), [v1.0](https://huggingface.co/fnlp/bart-base-chinese/tree/v1.0), [v2.0](https://huggingface.co/fnlp/bart-base-chinese/tree/v2.0)| [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_bart_fudanNLP.py) |
 | text2vec| text2vec-base-chinese | [torch](https://huggingface.co/shibing624/text2vec-base-chinese) | |
 | chatyuan v1&v2| clue-ai | [torch](https://github.com/clue-ai/ChatYuan) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
 | PromptCLUE| clue-ai | [torch](https://github.com/clue-ai/PromptCLUE) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
 | chatglm-6b | THUDM | [git](https://github.com/THUDM/ChatGLM-6B), [v0.1.0](https://huggingface.co/THUDM/chatglm-6b/tree/v0.1.0), [v1.1.0](https://huggingface.co/THUDM/chatglm-6b/tree/v1.1.0), [int8](https://huggingface.co/THUDM/chatglm-6b-int8), [int4](https://huggingface.co/THUDM/chatglm-6b-int4) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_chatglm.py) |
 | chatglm2-6b | THUDM | [git](https://github.com/THUDM/ChatGLM2-6B), [v2](https://huggingface.co/THUDM/chatglm2-6b), [int4](https://huggingface.co/THUDM/chatglm2-6b-int4) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_chatglm.py) |
 | llama | facebook| [git](https://github.com/facebookresearch/llama) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_pth.py)|
+| llama2 | facebook| [git](https://github.com/facebookresearch/llama) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_hf.py)|
 |chinese_llama_alpaca|Yiming Cui|[git](https://github.com/ymcui/Chinese-LLaMA-Alpaca) |[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_pth.py)|
 | vicuna | FastChat| [torch](https://huggingface.co/AlekseyKorshuk/vicuna-7b) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_hf.py)|
 | Belle_llama| LianjiaTech| [git](https://github.com/LianjiaTech/BELLE), [7B-2M-enc](https://huggingface.co/BelleGroup/BELLE-LLaMA-7B-2M-enc) | [合成说明](https://github.com/LianjiaTech/BELLE/tree/main/models)、[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_hf.py)|
 | Ziya | IDEA-CCNL | [v1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-v1), [v1.1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-v1.1), [pretrain-v1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-Pretrain-v1) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_pth.py) |
 | Baichuan | baichuan-inc | [7B](https://github.com/baichuan-inc/Baichuan-7B), [13B-Base](https://huggingface.co/baichuan-inc/Baichuan-13B-Base), [13B-Chat](https://huggingface.co/baichuan-inc/Baichuan-13B-Chat) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_hf.py) |
+| bloom | bigscience | [560m](https://huggingface.co/bigscience/bloom-560m) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_bloom.py) |
+
 
 ## 7. 鸣谢
 
 - 感谢苏神实现的[bert4keras](https://github.com/bojone/bert4keras)，本实现有不少地方参考了bert4keras的源码，在此衷心感谢大佬的无私奉献;
 - 其次感谢项目[bert4pytorch](https://github.com/MuQiuJun-AI/bert4pytorch)，也是在该项目的指引下给了我用pytorch来复现bert4keras的想法和思路。
 
 ## 8. 引用
@@ -234,8 +261,8 @@
     <tr align="center" >
       <td>
          <a href="https://star-history.com/#Tongjilibo/bert4torch&Date"><img width="400" height="250" src="https://api.star-history.com/svg?repos=Tongjilibo/bert4torch&type=Date" alt="pic"></a><br>
          <a href="https://star-history.com/#Tongjilibo/bert4torch&Date">Star History Chart</a> 
       </td>
     </tr>
   </tbody>
-</table>
+</table>
```

### Comparing `bert4torch-0.3.0/bert4torch/activations.py` & `bert4torch-0.3.1/bert4torch/activations.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.0/bert4torch/callbacks.py` & `bert4torch-0.3.1/bert4torch/callbacks.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.0/bert4torch/generation.py` & `bert4torch-0.3.1/bert4torch/generation.py`

 * *Files 0% similar despite different names*

```diff
@@ -556,15 +556,14 @@
         assert isinstance(inputs, (tuple, list))
         if states is not None:
             assert self.use_states is True, 'Args `use_states` must be True when return states is not None'
         
         # 使用cache, 输入只能padding在左侧
         if self.use_states:
             states = {'use_states': True} if states is None else states
-            states['step'] = self.step
 
             # next_inputs：step=0时候输入全部，>=1时候输入last_token
             next_inputs = self._prepare_next_inputs(inputs, output_ids, include_past=self.step==0)
 
             # past_token_ids: inputs+output_ids
             if self.step >= 1:
                 states['past_token_ids'] = self._prepare_next_inputs(inputs, output_ids)[0]
```

### Comparing `bert4torch-0.3.0/bert4torch/layers/attention.py` & `bert4torch-0.3.1/bert4torch/layers/attention.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,18 +142,18 @@
 
         if self.attention_scale:
             # 是否进行attention scale
             attention_scores = attention_scores / math.sqrt(self.attention_head_size)
         
         if self.p_bias == 'alibi':
             # ==================== alibi相对位置编码 ====================
-            key_position_scores_r_t = self.relative_positions_encoding(query_layer)
+            key_position_scores_r_t = self.relative_positions_encoding(key_layer)
             attention_scores = attention_scores + key_position_scores_r_t
             attention_scores = torch.max(attention_scores, torch.tensor(torch.finfo(attention_scores.dtype).min))  # baichuan-13b逻辑
-            attention_mask = None
+            # attention_mask = None  # baichuan的实现是不使用attention_mask，个人认为有点问题
 
         # 执行attention mask，对于mask为0部分的attention mask，
         # 值为-1e10，经过softmax后，attention_probs几乎为0，所以不会attention到mask为0的部分
         if attention_mask is not None:
             # attention_mask = attention_mask * attention_mask.squeeze(-2).unsqueeze(-1)  # deberta_v2中使用，但是不使用也不影响
             # attention_scores = attention_scores.masked_fill(attention_mask == 0, -1e10)  # 下一行的另一种写法
             attention_mask = (1.0 - attention_mask) * -10000.0  # 所以传入的mask的非padding部分为1, padding部分为0
```

### Comparing `bert4torch-0.3.0/bert4torch/layers/core.py` & `bert4torch-0.3.1/bert4torch/layers/core.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.0/bert4torch/layers/crf.py` & `bert4torch-0.3.1/bert4torch/layers/crf.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.0/bert4torch/layers/global_point.py` & `bert4torch-0.3.1/bert4torch/layers/global_point.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 from bert4torch.activations import get_activation
 
 
 class GlobalPointer(nn.Module):
     """全局指针模块
     将序列的每个(start, end)作为整体来进行判断
     参考：https://kexue.fm/archives/8373
+
+    :param hidden_size: 即模型最顶层输出的hidden_size
+    :param heads heads: 在实体识别和关系提取中，分别代表着实体个数和关系个数
+    :param head_size: 即每个heads的神经元个数，点积时候使用，相当于attention
     """
     def __init__(self, hidden_size, heads, head_size, RoPE=True, use_bias=True, tril_mask=True):
         super().__init__()
         self.heads = heads
         self.head_size = head_size
         self.RoPE = RoPE
         self.tril_mask = tril_mask
```

### Comparing `bert4torch-0.3.0/bert4torch/layers/misc.py` & `bert4torch-0.3.1/bert4torch/layers/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,22 @@
 
 
 class BlockIdentity(nn.Module):
     def __init__(self, *args, **kwargs):
         super(BlockIdentity, self).__init__()
 
     def forward(self, *args, **kwargs):
-        return kwargs
+        if (len(args) > 0) and (len(kwargs) > 0):
+            return args, kwargs
+        elif len(args) > 0:
+            return args[0] if len(args) == 1 else args
+        elif len(kwargs) > 0:
+            return kwargs
+        else:
+            return None
 
 
 class BERT_WHITENING():
     def __init__(self):
         self.kernel = None
         self.bias = None
 
@@ -361,21 +368,28 @@
     
 def add_adapter(model, adapter_method='bottleneck', bottlenect_size=64):
     # 冻结模型参数
     for param in model.parameters():
         param.requires_grad = False
     if adapter_method == 'bottleneck':
         # 顺序为: Attention --> Adapter --> Add --> LN --> FeedForward --> Adapter --> Add --> LayerNorm
+        
+        try:
+            layers = model.encoderLayer
+        except:
+            layers = model.decoderLayer
+        
+        # TODO: 这里需要测试一下前面layers赋值是否真的对原始的layers修改了
         for layer_id in range(model.num_hidden_layers):
-            transformer_layer = model.encoderLayer[layer_id].multiHeadAttention.o
+            transformer_layer = layers[layer_id].multiHeadAttention.o
             out_featuers = transformer_layer.out_features
             adapter1 = BottleneckAdapterLayer(out_featuers, bottleneck_size=bottlenect_size)
-            model.encoderLayer[layer_id].dropout1 = nn.Sequential(transformer_layer, adapter1)
+            layers[layer_id].dropout1 = nn.Sequential(transformer_layer, adapter1)
 
-            transformer_layer = model.encoderLayer[layer_id].feedForward
+            transformer_layer = layers[layer_id].feedForward
             out_featuers = transformer_layer.outputDense.out_features
             adapter2 = BottleneckAdapterLayer(out_featuers, bottleneck_size=bottlenect_size)
-            model.encoderLayer[layer_id].feedForward = nn.Sequential(transformer_layer, adapter2)
+            layers[layer_id].feedForward = nn.Sequential(transformer_layer, adapter2)
     # 待新增其余类型adapter
     else:
         pass
     return model
```

### Comparing `bert4torch-0.3.0/bert4torch/layers/position_encoding.py` & `bert4torch-0.3.1/bert4torch/layers/position_encoding.py`

 * *Files 2% similar despite different names*

```diff
@@ -273,33 +273,24 @@
         if math.log2(n).is_integer():
             return _get_interleave_power_of_2(n)
         else:
             closest_power_of_2 = 2 ** math.floor(math.log2(n))
             return _get_interleave_power_of_2(closest_power_of_2) + \
                 self._get_interleave(2 * closest_power_of_2)[0::2][:n - closest_power_of_2]
 
-    def _fill_with_neg_inf(self, t):
-        """FP16-compatible function that fills a tensor with -inf."""
-        return t.float().fill_(float("-inf")).type_as(t)
-
     def _gen_alibi_mask(self, seq_len):
         slopes = torch.Tensor(self._get_interleave(self.n_head))
         alibi = slopes.unsqueeze(1).unsqueeze(1) * torch.arange(seq_len).unsqueeze(0).unsqueeze(0).expand(self.n_head, -1, -1)
         alibi = alibi.view(self.n_head, 1, seq_len)
-        alibi_mask = torch.triu(self._fill_with_neg_inf(torch.zeros([seq_len, seq_len])), 1)
-        alibi_mask = alibi_mask.unsqueeze(0) + alibi
-        return alibi_mask
+        return alibi
     
-    def forward(self, query_layer):
+    def forward(self, key_layer):
         '''
-        query_layer: [btz, n_head, q_len, hdsz]
-        attention_mask: [btz, 1, q_len, k_len]
+        key_layer: [btz, n_head, q_len, hdsz]
         '''
-        seq_length_with_past = query_layer.shape[2]
+        seq_length_with_past = key_layer.shape[2]
         if seq_length_with_past > self.max_cache_pos:
             self.max_cache_pos = seq_length_with_past
-            self.future_mask = self._gen_alibi_mask(seq_length_with_past).to(query_layer)
+            self.future_mask = self._gen_alibi_mask(seq_length_with_past).to(key_layer)
         
         mask = self.future_mask[:self.n_head, :seq_length_with_past, :seq_length_with_past] 
-        if mask.size(-2) == 1:
-            mask = mask[:, -1:, :]
         return mask.unsqueeze(0)
```

### Comparing `bert4torch-0.3.0/bert4torch/layers/transformer_block.py` & `bert4torch-0.3.1/bert4torch/layers/transformer_block.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             model_kwargs['cross_past_key_value'] = cross_attn_output[-1]
             hidden_states = self.layerNorm3(hidden_states, conditional_emb) if not self.pre_layernorm else hidden_states
 
         # ============== feedforward ==============
         x = self.layerNorm2(hidden_states, conditional_emb) if self.pre_layernorm else hidden_states  # pre/post layernorm
         feedforward_output = self.feedForward(x)
         residual = x if self.apply_residual_post_layernorm else hidden_states
-        hidden_states = residual + + self.dropout2(feedforward_output)
+        hidden_states = residual + self.dropout2(feedforward_output)
         hidden_states = self.layerNorm2(hidden_states, conditional_emb) if not self.pre_layernorm else hidden_states
         
         if self.is_decoder:
             model_kwargs['past_key_value'] = self_attn_output[-1]
         model_kwargs['hidden_states'] = hidden_states
         return model_kwargs
```

### Comparing `bert4torch-0.3.0/bert4torch/losses.py` & `bert4torch-0.3.1/bert4torch/losses.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.0/bert4torch/models/__init__.py` & `bert4torch-0.3.1/bert4torch/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from bert4torch.models.nezha import *
 from bert4torch.models.roformer import *
 from bert4torch.models.t5 import *
 from bert4torch.models.transformer import *
 from bert4torch.models.transformer_xl import *
 from bert4torch.models.uie import *
 from bert4torch.models.xlnet import *
+from bert4torch.models.bloom import *
 
 
 def build_transformer_model(config_path=None, checkpoint_path=None, model='bert', application='encoder', add_trainer=False, **kwargs):
     """根据配置文件构建模型，可选加载checkpoint权重
 
     :param config_path: str, 模型的config文件地址
     :param checkpoint_path: str/list[str], 模型文件地址, 默认值None表示不加载预训练模型
@@ -104,14 +105,15 @@
         't5.1.1_encoder': T5_Encoder,
         't5.1.1_decoder': T5_Decoder,
         'mt5.1.1': T5,
         'mt5.1.1_encoder': T5_Encoder,
         'mt5.1.1_decoder': T5_Decoder,
         'transformer_xl': Transformer_XL,
         'xlnet': XLNET,
+        'bloom': Bloom
     }
 
     if isinstance(model, str):  # string表示使用自带的模型
         MODEL = models[model.lower()]
         if model.endswith('t5.1.1'):
             configs['version'] = model
     elif isinstance(model, type) and issubclass(model, BERT_BASE): # nn.Module表示使用自定义的模型：
```

### Comparing `bert4torch-0.3.0/bert4torch/models/albert.py` & `bert4torch-0.3.1/bert4torch/models/albert.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.0/bert4torch/models/bart.py` & `bert4torch-0.3.1/bert4torch/models/bart.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.0/bert4torch/models/base.py` & `bert4torch-0.3.1/bert4torch/models/base.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.0/bert4torch/models/bert.py` & `bert4torch-0.3.1/bert4torch/models/bert.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.0/bert4torch/models/deberta.py` & `bert4torch-0.3.1/bert4torch/models/deberta.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.0/bert4torch/models/electra.py` & `bert4torch-0.3.1/bert4torch/models/electra.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.0/bert4torch/models/erinie.py` & `bert4torch-0.3.1/bert4torch/models/erinie.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.0/bert4torch/models/gau_alpha.py` & `bert4torch-0.3.1/bert4torch/models/gau_alpha.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.0/bert4torch/models/glm.py` & `bert4torch-0.3.1/bert4torch/models/glm.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,81 +1,68 @@
-from bert4torch.models.base import LM_Mask
-from bert4torch.models.bert import BERT
+from bert4torch.models.transformer import Decoder
 from bert4torch.layers import LayerNorm, BertLayer, BlockIdentity
 from bert4torch.snippets import delete_arguments
 from bert4torch.activations import get_activation
 import torch
 from torch import nn
 import copy
 
 
-class GLM(LM_Mask, BERT):
+class GLM(Decoder):
     '''GLM: https://github.com/THUDM/GLM, ChatGLM-6B: https://github.com/THUDM/ChatGLM-6B
     Unilm设计，可定义为GLM(UniLM_MASK, BERT)但是要求传入segement_ids比较麻烦，这里继承LM_MASK并使用get_masks()重新构造attention_mask
     模型结构特点：
     1）rotary使用的updown+position_encoding_2d
     2）qkv合并成一个权重convert时不是concat在一起的
     3）attention_mask类似于Unilm，最后一个token仅能访问之前的，之前的tokens可以互相访问
     4）跳跃连接有权重设计
+    5) embedding之后没有layernorm
     '''
     @delete_arguments('with_pool', 'with_mlm', 'with_nsp')
     def __init__(self, *args, **kwargs):
-        kwargs.update({'p_bias': 'rotary', 'weight': True, 'is_decoder': True})
+        kwargs.update({'p_bias': 'rotary', 'weight': True, 'is_decoder': True, 'final_layernorm': True})
         super().__init__(*args, **kwargs)
         self.bos_token_id, self.mask_token_id, self.gmask_token_id = kwargs.get('bos_token_id'), kwargs.get('mask_token_id'), kwargs.get('gmask_token_id')
         self.position_encoding_2d = kwargs.get('position_encoding_2d', True)
         del self.embeddings.layerNorm
         layer = self.GLMBlock(**self.get_kw('hidden_size', 'num_attention_heads', 'dropout_rate', 'attention_probs_dropout_prob', 
                                             'intermediate_size', 'hidden_act', 'is_dropout', 'conditional_size', 'num_hidden_layers', **kwargs))
-        self.encoderLayer = nn.ModuleList([copy.deepcopy(layer) if layer_id in self.keep_hidden_layers else BlockIdentity() for layer_id in range(self.num_hidden_layers)])
+        self.decoderLayer = nn.ModuleList([copy.deepcopy(layer) if layer_id in self.keep_hidden_layers else BlockIdentity() for layer_id in range(self.num_hidden_layers)])
         self.LayerNormFinal = torch.nn.LayerNorm(self.hidden_size, eps=kwargs.get('layer_norm_eps', 1e-12))
-        self.dense = nn.Linear(self.hidden_size, self.vocab_size, bias=False)
-        self.final_activation = get_activation(kwargs.get('final_activation', 'linear'))
-        self.tie_weights()
-
-    def tie_weights(self):
-        if self.tie_emb_prj_weight:
-            self.dense.weight = self.embeddings.word_embeddings.weight
-    
+
     def load_variable(self, state_dict, name, prefix='transformer'):
-        """加载单个变量的函数, 这里的名称均为映射前的
-        """
-        variable = state_dict[name]
-        if name in {f'{prefix}.embeddings.word_embeddings.weight', 'lm_head.weight'}:
-            return self.load_embeddings(variable)
-        else:
-            return variable
+        return super(GLM, self).load_variable(state_dict, name, prefix=prefix)
         
     def variable_mapping(self, prefix='transformer'):
         # 映射到权重格式
         mapping = {
             'LayerNormFinal.weight': "transformer.final_layernorm.weight",
             'LayerNormFinal.bias': "transformer.final_layernorm.bias",
-            'dense.weight': "lm_head.weight",
+            'lm_head.weight': "lm_head.weight",
             'embeddings.word_embeddings.weight': 'transformer.word_embeddings.weight'}
 
         for i in range(self.num_hidden_layers):
             prefix_i = f'{prefix}.layers.%d.' % i
             mapping.update({
-                f'encoderLayer.{i}.layerNorm1.weight': prefix_i + 'input_layernorm.weight',
-                f'encoderLayer.{i}.layerNorm1.bias': prefix_i + 'input_layernorm.bias',
-                f'encoderLayer.{i}.layerNorm2.weight': prefix_i + 'post_attention_layernorm.weight',
-                f'encoderLayer.{i}.layerNorm2.bias': prefix_i + 'post_attention_layernorm.bias',
-                f'encoderLayer.{i}.multiHeadAttention.q.weight': prefix_i + 'attention.self.query.weight',
-                f'encoderLayer.{i}.multiHeadAttention.q.bias': prefix_i + 'attention.self.query.bias',
-                f'encoderLayer.{i}.multiHeadAttention.k.weight': prefix_i + 'attention.self.key.weight',
-                f'encoderLayer.{i}.multiHeadAttention.k.bias': prefix_i + 'attention.self.key.bias',
-                f'encoderLayer.{i}.multiHeadAttention.v.weight': prefix_i + 'attention.self.value.weight',
-                f'encoderLayer.{i}.multiHeadAttention.v.bias': prefix_i + 'attention.self.value.bias',
-                f'encoderLayer.{i}.multiHeadAttention.o.weight': prefix_i + 'attention.dense.weight',
-                f'encoderLayer.{i}.multiHeadAttention.o.bias': prefix_i + 'attention.dense.bias',
-                f'encoderLayer.{i}.feedForward.intermediateDense.weight': prefix_i + 'mlp.dense_h_to_4h.weight',
-                f'encoderLayer.{i}.feedForward.intermediateDense.bias': prefix_i + 'mlp.dense_h_to_4h.bias',
-                f'encoderLayer.{i}.feedForward.outputDense.weight': prefix_i + 'mlp.dense_4h_to_h.weight',
-                f'encoderLayer.{i}.feedForward.outputDense.bias': prefix_i + 'mlp.dense_4h_to_h.bias',
+                f'decoderLayer.{i}.layerNorm1.weight': prefix_i + 'input_layernorm.weight',
+                f'decoderLayer.{i}.layerNorm1.bias': prefix_i + 'input_layernorm.bias',
+                f'decoderLayer.{i}.layerNorm2.weight': prefix_i + 'post_attention_layernorm.weight',
+                f'decoderLayer.{i}.layerNorm2.bias': prefix_i + 'post_attention_layernorm.bias',
+                f'decoderLayer.{i}.multiHeadAttention.q.weight': prefix_i + 'attention.self.query.weight',
+                f'decoderLayer.{i}.multiHeadAttention.q.bias': prefix_i + 'attention.self.query.bias',
+                f'decoderLayer.{i}.multiHeadAttention.k.weight': prefix_i + 'attention.self.key.weight',
+                f'decoderLayer.{i}.multiHeadAttention.k.bias': prefix_i + 'attention.self.key.bias',
+                f'decoderLayer.{i}.multiHeadAttention.v.weight': prefix_i + 'attention.self.value.weight',
+                f'decoderLayer.{i}.multiHeadAttention.v.bias': prefix_i + 'attention.self.value.bias',
+                f'decoderLayer.{i}.multiHeadAttention.o.weight': prefix_i + 'attention.dense.weight',
+                f'decoderLayer.{i}.multiHeadAttention.o.bias': prefix_i + 'attention.dense.bias',
+                f'decoderLayer.{i}.feedForward.intermediateDense.weight': prefix_i + 'mlp.dense_h_to_4h.weight',
+                f'decoderLayer.{i}.feedForward.intermediateDense.bias': prefix_i + 'mlp.dense_h_to_4h.bias',
+                f'decoderLayer.{i}.feedForward.outputDense.weight': prefix_i + 'mlp.dense_4h_to_h.weight',
+                f'decoderLayer.{i}.feedForward.outputDense.bias': prefix_i + 'mlp.dense_4h_to_h.bias',
                 })
         return mapping
 
     def get_masks(self, attention_mask, context_lens, prepad_lens):
         '''调整mask使得在content_lens前是bi_attention'''
         for i, (prepad_len, context_len) in enumerate(zip(prepad_lens, context_lens)):
             attention_mask[i, :, :, prepad_len:context_len] = 1
@@ -127,20 +114,15 @@
             model_kwargs['position_ids'] = self.get_position_ids(position_ids, seq_len, context_lens, mask_positions, prepad_lens, gmask=use_gmask)
         return model_kwargs
 
     def apply_embeddings(self, *inputs, **model_kwargs):
         model_kwargs = super().apply_embeddings(*inputs, **model_kwargs)
         model_kwargs = self.prepare_inputs(*inputs, **model_kwargs)
         return model_kwargs
-    
-    def apply_final_layers(self, **model_kwargs):
-        hidden_state = super().apply_final_layers(**model_kwargs)
-        logit = self.dense(self.LayerNormFinal(hidden_state))
-        return self.final_activation(logit)
-    
+       
     class GLMBlock(BertLayer):
         '''顺序：LN --> Att --> Add --> LN --> FFN --> Add'''
         def __init__(self, *args, **kwargs):
             super().__init__(*args, **kwargs)
             self.num_hidden_layers = kwargs['num_hidden_layers']
             hidden_size, eps = kwargs['hidden_size'], kwargs.get('layer_norm_eps', 1e-5)
             self.layerNorm1 = torch.nn.LayerNorm(hidden_size, eps=eps)
@@ -167,38 +149,24 @@
 class GLM2(GLM):
     """CHATGLM2-6B: https://github.com/THUDM/ChatGLM2-6B
     主要修改：1）不使用Unilm式的mask
              2) flash_attention
              3) multi_query_attention
     """
     def __init__(self, *args, **kwargs):
+        kwargs.update({'norm_mode': 'rmsnorm', 'pre_layernorm': True})
         super().__init__(*args, **kwargs)
         self.LayerNormFinal = LayerNorm(self.hidden_size, eps=kwargs.get('layer_norm_eps', 1e-5), norm_mode='rmsnorm', bias=False)
-        
+
     def prepare_inputs(self, *inputs, **model_kwargs):
         return model_kwargs
     
     class GLMBlock(BertLayer):
         '''顺序：LN --> Att --> Add --> LN --> FFN --> Add'''
         def __init__(self, *args, **kwargs):
             super().__init__(*args, **kwargs)
-            self.num_hidden_layers = kwargs['num_hidden_layers']
             hidden_size, eps = kwargs['hidden_size'], kwargs.get('layer_norm_eps', 1e-5)
             self.layerNorm1 = LayerNorm(hidden_size, eps=eps, norm_mode='rmsnorm', bias=False)
             self.layerNorm2 = LayerNorm(hidden_size, eps=eps, norm_mode='rmsnorm', bias=False)
             self.multiHeadAttention.o.register_parameter('bias', None)
             self.feedForward.intermediateDense.register_parameter('bias', None)
             self.feedForward.outputDense.register_parameter('bias', None)
-
-        def forward(self, hidden_states=None, attention_mask=None, past_key_value=None, **model_kwargs):
-            x = self.layerNorm1(hidden_states)
-            self_attn_output = self.multiHeadAttention(x, attention_mask, past_key_value=past_key_value, **model_kwargs)
-            hidden_states = hidden_states + self.dropout1(self_attn_output[0])
-
-            x = self.layerNorm2(hidden_states)
-            hidden_states = hidden_states + self.dropout2(self.feedForward(x))
-
-            if self.is_decoder:
-                model_kwargs['past_key_value'] = self_attn_output[-1]
-            model_kwargs['hidden_states'] = hidden_states
-            return model_kwargs
-
```

### Comparing `bert4torch-0.3.0/bert4torch/models/gpt.py` & `bert4torch-0.3.1/bert4torch/models/transformer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,140 +1,143 @@
-from bert4torch.models.base import LM_Mask
 from bert4torch.models.bert import BERT
-from bert4torch.snippets import delete_arguments
+from bert4torch.models.base import LM_Mask, BERT_BASE
+from bert4torch.snippets import delete_arguments, insert_arguments
 from bert4torch.activations import get_activation
-from bert4torch.layers import LayerNorm, BertLayer, BlockIdentity
+from bert4torch.layers import LayerNorm
 from torch import nn
-import copy
+import torch
 
 
-class GPT(LM_Mask, BERT):
-    """构建GPT模型；
-    链接：https://github.com/openai/finetune-transformer-lm
-    Todo: 理论上gpt系列应该从Decoder继承，自动实现is_decoder=True，且使用decoderLayer
-    """
-    @delete_arguments('with_pool', 'with_mlm', 'with_nsp')
+class Encoder(BERT):
     def __init__(self, *args, **kwargs):
-        """GPT的embedding是token、position、segment三者embedding之和，跟BERT的主要区别是三者相加之后没有加LayerNormalization层。
-           使用LM_Mask实现预训练ckpt中的bias参数，最后的全连接层由于和embedding层权重一致，因此直接从word_embedding取
+        kwargs['vocab_size'] = kwargs.get('src_vocab_size', kwargs['vocab_size'])
+        super().__init__(*args, **kwargs)
+        # encoder需要返回encoder_attention_mask
+        self.encoder_attention_mask = None
+    
+    def forward(self, *inputs, **model_kwargs):
+        """因为encoder需要返回encoder_attention_mask，因此这里从新定义一下，多返回一个参数
         """
-        super(GPT, self).__init__(*args, is_decoder=True, **kwargs)
-        del self.embeddings.layerNorm
-        self.dense = nn.Linear(self.hidden_size, self.vocab_size, bias=False)
-        self.dense.weight = self.embeddings.word_embeddings.weight
-        self.final_activation = get_activation(kwargs.get('final_activation', 'linear'))
-
-    def apply_final_layers(self, **model_kwargs):
-        hidden_state = super().apply_final_layers(**model_kwargs)
-        logit = self.dense(hidden_state)
-        return self.final_activation(logit)
-
-    def load_variable(self, state_dict, name):
-        return super(GPT, self).load_variable(state_dict, name, prefix='gpt')
-
-    def variable_mapping(self):
-        # 映射到GPT权重格式
-        mapping =  super(GPT, self).variable_mapping(prefix='gpt')
-        return mapping
+        # 返回model_kwargs方便解析attention_mask
+        outputs, model_kwargs = super().forward(*inputs, use_states=True, **model_kwargs)
+        # return: [encoder_hidden_states, encoder_attention_mask]
+        return ([outputs] if isinstance(outputs, torch.Tensor) else outputs) + [model_kwargs['attention_mask']]
 
 
-class GPT2(LM_Mask, BERT):
-    """构建GPT模型；
-    链接：https://github.com/openai/finetune-transformer-lm
-    """
+class Decoder(LM_Mask, BERT):
     @delete_arguments('with_pool', 'with_mlm', 'with_nsp')
-    def __init__(self, *args, **kwargs):
-        """GPT2的embedding是token、position两者embedding之和。
-           1、跟BERT的主要区别是三者相加之后没有加LayerNormalization层。
-           2、bert的layernorm是在attn/ffc之后，OpenAi-gpt2是在之前。
-           使用LM_Mask实现预训练ckpt中的bias参数，最后的全连接层由于和embedding层权重一致，因此直接从word_embedding取
+    @insert_arguments(with_lm=True)
+    def __init__(self, *args, logit_scale=False, final_layernorm=False, **kwargs):
+        kwargs['vocab_size'] = kwargs.get('tgt_vocab_size', kwargs['vocab_size'])
+        kwargs['is_decoder'] = True  # 标记是decoder
+        super().__init__(*args, **kwargs)
+        self.decoderLayer = self.encoderLayer
+        del self.encoderLayer
+        self.final_layernorm = final_layernorm
+
+        # 从hidden_states映射到logit
+        if self.with_lm:
+            self.lm_head = nn.Linear(self.hidden_size, self.vocab_size, bias=False)
+            self.final_activation = get_activation('linear' if self.with_lm is True else self.with_lm)  # 添加激活，一般是线性激活或softmax
+
+            # decoder底层的embedding和顶层的全连接共享
+            # [True]: fudan_bart和uer_t5的t5, [False]: mt5和t5_pegasus
+            self.tie_weights()
+            if logit_scale:  # T5默认会有logit_scale, bart默认没有
+                self.logit_scale = (self.hidden_size ** -0.5)
+        
+        if self.final_layernorm:
+            self.LayerNormFinal = LayerNorm(self.hidden_size, eps=kwargs.get('layer_norm_eps', 1e-12), 
+                                            conditional_size=self.conditional_size, norm_mode=kwargs.get('norm_mode', 'normal'),
+                                            weight=kwargs.get('weight', True), bias=kwargs.get('bias', True))
+
+    def tie_weights(self):
+        if self.tie_emb_prj_weight is True:
+            self.lm_head.weight = self.embeddings.word_embeddings.weight
+
+    def apply_main_layers(self, **model_kwargs):
+        """Dencoder主体是基于Self-Attention、Cross-Attention的模块；
+        顺序：Att1 --> Add --> LN --> Att2 --> Add -->  LN --> FFN --> Add --> LN
         """
-        super(GPT2, self).__init__(*args, **kwargs)
-        del self.embeddings.layerNorm
-        layer = self.Gpt2Layer(is_decoder=True, **self.get_kw('hidden_size', 'num_attention_heads', 'dropout_rate', 'attention_probs_dropout_prob', 
-                                                              'intermediate_size', 'hidden_act', 'is_dropout', 'conditional_size', **kwargs))
-        self.encoderLayer = nn.ModuleList([copy.deepcopy(layer) if layer_id in self.keep_hidden_layers else BlockIdentity() for layer_id in range(self.num_hidden_layers)])
-        self.LayerNormFinal = LayerNorm(self.hidden_size, eps=1e-12, conditional_size=self.conditional_size, bias=kwargs.get('bias', True))
-        self.dense = nn.Linear(self.hidden_size, self.vocab_size, bias=False) 
-        self.dense.weight = self.embeddings.word_embeddings.weight
-        self.final_activation = get_activation(kwargs.get('final_activation', 'linear'))
-
+        decoded_layers = [model_kwargs['hidden_states']] # 添加embedding的输出
+        for l_i, layer_module in enumerate(self.decoderLayer):
+            model_kwargs = self.apply_on_layer_begin(l_i, **model_kwargs)
+            outputs = self.layer_forward(layer_module, model_kwargs)
+            model_kwargs.update(outputs)
+            hidden_states = model_kwargs['hidden_states']
+            model_kwargs = self.apply_on_layer_end(l_i, **model_kwargs)
+
+            if self.output_all_encoded_layers:
+                decoded_layers.append(hidden_states)
+        if not self.output_all_encoded_layers:
+            decoded_layers.append(hidden_states)
+        model_kwargs['decoded_layers'] = decoded_layers
+        return model_kwargs
+    
     def apply_final_layers(self, **model_kwargs):
-        hidden_state = super().apply_final_layers(**model_kwargs)
-        logit = self.dense(self.LayerNormFinal(hidden_state))
-        return self.final_activation(logit)
-
-    def load_variable(self, state_dict, name):
-        return super(GPT2, self).load_variable(state_dict, name, prefix='gpt2')
-
-    def variable_mapping(self):
-        # 映射到GPT权重格式
-        mapping = super(GPT2, self).variable_mapping(prefix='gpt2')
-        mapping.update({'LayerNormFinal.weight': 'gpt2.LayerNormFinal.weight',
-                        'LayerNormFinal.bias': 'gpt2.LayerNormFinal.bias'})
+        hidden_states = model_kwargs['decoded_layers'][-1]  # decoder顶层的hidden_states [btz, seq_len, hdsz]
+
+        if self.final_layernorm:
+            hidden_states = self.LayerNormFinal(hidden_states)
+        
+        if self.with_lm:
+            logits = self.lm_head(hidden_states)  # [btz, seq_len, vocab_size]
+            logits = logits * self.logit_scale if hasattr(self, 'logit_scale') else logits
+            logits = self.final_activation(logits)
+            return logits
+        return hidden_states
+
+    def load_variable(self, state_dict, name, prefix='bert'):
+        """加载单个变量的函数, 这里的名称均为映射前的"""
+        variable = state_dict[name]
+        if name in {f'{prefix}.embeddings.word_embeddings.weight', 'lm_head.weight'}:
+            return self.load_embeddings(variable)
+        elif name == f'{prefix}.embeddings.position_embeddings.weight':
+            return self.load_pos_embeddings(variable)
+        else:
+            return variable
+        
+    def variable_mapping(self, prefix='bert'):
+        raw_mapping = super().variable_mapping(prefix)
+        mapping = {}
+        for k, v in raw_mapping.items():
+            mapping[k.replace('encoderLayer', 'decoderLayer')] = v
+        
+        if self.final_layernorm:
+            mapping.update({'LayerNormFinal.weight': f'{prefix}.LayerNormFinal.weight',
+                            'LayerNormFinal.bias': f'{prefix}.LayerNormFinal.bias'})
+        if self.with_lm and (not self.tie_emb_prj_weight):  # 当且仅当未绑定权重的时候
+            mapping.update({'lm_head.weight': f'{prefix}.lm_head.weight'})
         return mapping
-    
-    class Gpt2Layer(BertLayer):
-        '''顺序：LN --> Att --> Add --> LN --> FFN --> Add'''
-        def forward(self, hidden_states=None, attention_mask=None, conditional_emb=None, past_key_value=None, **model_kwargs):
-            # bert的layernorm是在attn/ffc之后，Openai-gpt2是在之前
-            x = self.layerNorm1(hidden_states, conditional_emb)
-            self_attn_output = self.multiHeadAttention(x, attention_mask, past_key_value=past_key_value)
-            hidden_states = hidden_states + self.dropout1(self_attn_output[0])
-
-            x = self.layerNorm2(hidden_states, conditional_emb)
-            ffn_output = self.feedForward(x)
-            hidden_states = hidden_states + self.dropout2(ffn_output)
-
-            if self.is_decoder:
-                model_kwargs['past_key_value'] = self_attn_output[-1]
-            model_kwargs['hidden_states'] = hidden_states
-            return model_kwargs
-
-
-class GPT2_ML(LM_Mask, BERT):
-    """构建GPT2_ML模型；
-    链接: https://github.com/imcaspar/gpt2-ml；
-    注意：GPT2_ML虽然号称GPT2，但是它的结构其实更接近GPT，它自称GPT2的原因大概是因为它开源的版本参数量达到了GPT2的15亿参数。
-    看完ckpt中的key，和GPT的区别是embedding后也有layernorm，和bert的区别是第二个跳跃链接的输入是在layernorm前，bert是在之后
-    """
+
+
+class Transformer(BERT_BASE):
+    '''encoder-decoder结构'''
     @delete_arguments('with_pool', 'with_mlm', 'with_nsp')
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        layer = self.Gpt2MlLayer(self.hidden_size, self.num_attention_heads, self.dropout_rate, self.attention_probs_dropout_prob, self.intermediate_size, self.hidden_act, 
-                                 is_dropout=self.is_dropout, conditional_size=self.conditional_size, is_decoder=True)
-        self.encoderLayer = nn.ModuleList([copy.deepcopy(layer) if layer_id in self.keep_hidden_layers else BlockIdentity() for layer_id in range(self.num_hidden_layers)])
-        self.dense = nn.Linear(self.hidden_size, self.vocab_size, bias=False)
-        self.dense.weight = self.embeddings.word_embeddings.weight
-        self.final_activation = get_activation(kwargs.get('final_activation', 'linear'))
+    def __init__(self, *args, tie_emb_src_tgt_weight=False, **kwargs):
+        super(Transformer, self).__init__(*args, **kwargs)
 
-    def apply_final_layers(self, **model_kwargs):
-        hidden_state = super().apply_final_layers(**model_kwargs)
-        logit = self.dense(hidden_state)
-        return self.final_activation(logit)
-
-    def load_variable(self, state_dict, name):
-        return super(GPT2_ML, self).load_variable(state_dict, name, prefix='gpt2_ml')
-
-    def variable_mapping(self):
-        # 映射到GPT2权重格式
-        mapping =  super(GPT2_ML, self).variable_mapping(prefix='gpt2_ml')
-        return mapping
+        # encoder
+        self.encoder = Encoder(*args, **kwargs)
+
+        # decoder
+        self.decoder = Decoder(*args, add_cross_attention=True, **kwargs)
+
+        if tie_emb_src_tgt_weight:
+            # encoder和decoder的embedding权重共享
+            assert self.encoder.vocab_size == self.decoder.vocab_size, "To share word embedding, the vocab size of src/tgt shall be the same."
+            self.encoder.embeddings.word_embeddings.weight = self.decoder.embeddings.word_embeddings.weight
+
+    def forward(self, *inputs):
+        inputs = self.args_segmentate(inputs)
+        encoder_input, decoder_input = inputs[:2]
+
+        # encoder
+        encoder_hidden_states, encoder_attention_mask = self.encoder(encoder_input)
+
+        # decoder
+        decoder_outputs = self.decoder(decoder_input + [encoder_hidden_states, encoder_attention_mask])
+        
+        # 输出encoder_hidden_state和decoder_hidden_state，以应对一些多任务情况
+        # with_lm=True时候，decoder_outputs为logits, False时候为decoder_hidden_state
+        return [encoder_hidden_states] + [decoder_outputs]
 
-    class Gpt2MlLayer(BertLayer):
-        '''未定义在layer.py中是因为该层针对gpt2_ml模型，不可复用；
-        顺序：Att --> Add --> LN --> FFN --> Add --> LN
-        '''
-        def forward(self, hidden_states=None, attention_mask=None, conditional_emb=None, past_key_value=None, **model_kwargs):
-            self_attn_output = self.multiHeadAttention(hidden_states, attention_mask, past_key_value=past_key_value)
-            hidden_states = hidden_states + self.dropout1(self_attn_output[0])
-            x = self.layerNorm1(hidden_states, conditional_emb)
-
-            ffn_output = self.feedForward(x)
-            # bert的第二个跳跃连接的输入1是经过了multiHeadAttention+layerNorm1的hidden_states, 即这里的x
-            # gpt2_ml的第二个跳跃连接的输入1是经过了multiHeadAttention的hidden_states, 不加layerNorm1
-            hidden_states = hidden_states + self.dropout2(ffn_output)
-            hidden_states = self.layerNorm2(hidden_states, conditional_emb)
-            if self.is_decoder:
-                model_kwargs['past_key_value'] = self_attn_output[-1]
-            model_kwargs['hidden_states'] = hidden_states
-            return model_kwargs
```

### Comparing `bert4torch-0.3.0/bert4torch/models/roformer.py` & `bert4torch-0.3.1/bert4torch/models/roformer.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.0/bert4torch/models/t5.py` & `bert4torch-0.3.1/bert4torch/models/t5.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             return variable
 
     def variable_mapping(self, prefix=''):
         # 查看check_point发现'shared.weight'
         mapping = {f'{prefix}embeddings.word_embeddings.weight': 'decoder.embed_tokens.weight',
                    f'{prefix}decoderLayer.0.multiHeadAttention.relative_positions_encoding.weight': 'decoder.block.0.layer.0.SelfAttention.relative_attention_bias.weight',
                    f'{prefix}final_layer_norm.weight': 'decoder.final_layer_norm.weight',
-                   f'{prefix}final_dense.weight': 'lm_head.weight'}
+                   f'{prefix}lm_head.weight': 'lm_head.weight'}
 
         for i in range(self.num_hidden_layers):
             mapping.update({
                 f'{prefix}decoderLayer.{i}.multiHeadAttention.q.weight': f'decoder.block.{i}.layer.0.SelfAttention.q.weight',
                 f'{prefix}decoderLayer.{i}.multiHeadAttention.k.weight': f'decoder.block.{i}.layer.0.SelfAttention.k.weight',
                 f'{prefix}decoderLayer.{i}.multiHeadAttention.v.weight': f'decoder.block.{i}.layer.0.SelfAttention.v.weight',
                 f'{prefix}decoderLayer.{i}.multiHeadAttention.o.weight': f'decoder.block.{i}.layer.0.SelfAttention.o.weight',
@@ -134,14 +134,15 @@
         self.tie_emb_src_tgt_weight = tie_emb_src_tgt_weight
 
         # encoder
         self.encoder = T5_Encoder(*args, **kwargs)
 
         # decoder
         kwargs['add_cross_attention'] = True
+        kwargs['logit_scale'] = kwargs.get('logit_scale', True)
         self.decoder = T5_Decoder(*args, **kwargs)
 
     def load_variable(self, state_dict, name, prefix=''):
         # 加载单个变量的函数
         variable = state_dict[name]
         if name in {'shared.weight', 'encoder.embed_tokens.weight', 'decoder.embed_tokens.weight', 'lm_head.weight'}:
             return self.load_embeddings(variable)
```

### Comparing `bert4torch-0.3.0/bert4torch/models/transformer_xl.py` & `bert4torch-0.3.1/bert4torch/models/transformer_xl.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         # transformer block
         layer = XlnetLayer(r_s_bias=None, **self.get_kw('hidden_size', 'num_attention_heads', 'dropout_rate', 'attention_probs_dropout_prob', 'intermediate_size', 
                                                         'hidden_act', 'is_dropout', 'conditional_size', 'r_w_bias', 'r_r_bias', **kwargs))
         self.encoderLayer = nn.ModuleList([copy.deepcopy(layer) if layer_id in self.keep_hidden_layers else BlockIdentity() for layer_id in range(self.num_hidden_layers)])
 
         # 映射
         if self.with_lm:
-            self.dense = nn.Linear(self.hidden_size, self.vocab_size, bias=True)
+            self.lm_head = nn.Linear(self.hidden_size, self.vocab_size, bias=True)
 
     def init_mems(self, bsz):
         '''初始化mems, 用于记忆mlen的各层隐含层状态'''
         if isinstance(self.mem_len, (int, float)) and (self.mem_len > 0):
             mems = []
             param = next(self.parameters())
             for _ in range(self.num_hidden_layers+1):
```

### Comparing `bert4torch-0.3.0/bert4torch/models/uie.py` & `bert4torch-0.3.1/bert4torch/models/uie.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.0/bert4torch/models/xlnet.py` & `bert4torch-0.3.1/bert4torch/models/xlnet.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
         pos_emb = self.dropout(pos_emb)  # 用word_emb的dropout
         return pos_emb
 
     def apply_final_layers(self, **model_kwargs):
         hidden_state = super().apply_final_layers(**model_kwargs)
         if self.with_lm:
-            return [hidden_state, self.dense(hidden_state)]
+            return [hidden_state, self.lm_head(hidden_state)]
         else:
             return hidden_state
 
     def load_variable(self, state_dict, name, prefix='transformer'):
         # 加载单个变量的函数
         variable = state_dict[name]
         if name in {f'{prefix}.word_embedding.weight', 'lm_loss.weight', 'lm_loss.bias'}:
@@ -61,16 +61,16 @@
             return variable.reshape(variable.shape[0], -1)
         else:
             return variable
 
     def variable_mapping(self, prefix='transformer'):
         mapping = {
             'embeddings.weight': f'{prefix}.word_embedding.weight',
-            'dense.weight': 'lm_loss.weight',
-            'dense.bias': 'lm_loss.bias',
+            'lm_head.weight': 'lm_loss.weight',
+            'lm_head.bias': 'lm_loss.bias',
         }
         for i in range(self.num_hidden_layers):
             prefix_i = f'{prefix}.layer.%d.' % i
             mapping.update({f'encoderLayer.{i}.multiHeadAttention.q.weight': prefix_i + 'rel_attn.q',
                             f'encoderLayer.{i}.multiHeadAttention.k.weight': prefix_i + 'rel_attn.k',
                             f'encoderLayer.{i}.multiHeadAttention.v.weight': prefix_i + 'rel_attn.v',
                             f'encoderLayer.{i}.multiHeadAttention.o.weight': prefix_i + 'rel_attn.o',
```

### Comparing `bert4torch-0.3.0/bert4torch/optimizers.py` & `bert4torch-0.3.1/bert4torch/optimizers.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.0/bert4torch/quantization.py` & `bert4torch-0.3.1/bert4torch/quantization.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.0/bert4torch/snippets.py` & `bert4torch-0.3.1/bert4torch/snippets.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.0/bert4torch/tokenizers.py` & `bert4torch-0.3.1/bert4torch/tokenizers.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.0/bert4torch.egg-info/PKG-INFO` & `bert4torch-0.3.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: bert4torch
-Version: 0.3.0
-Summary: an elegant bert4torch
-Home-page: https://github.com/Tongjilibo/bert4torch
-Author: Tongjilibo
-License: MIT Licence
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![bert4torch](https://github.com/Tongjilibo/bert4torch/blob/master/docs/pics/bert4torch.png)
 
 [![licence](https://img.shields.io/github/license/Tongjilibo/bert4torch.svg?maxAge=3600)](https://github.com/Tongjilibo/bert4torch/blob/master/LICENSE)
 [![GitHub release](https://img.shields.io/github/release/Tongjilibo/bert4torch.svg?maxAge=3600)](https://github.com/Tongjilibo/bert4torch/releases)
 [![PyPI](https://img.shields.io/pypi/v/bert4torch?label=pypi%20package)](https://pypi.org/project/bert4torch/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/bert4torch)](https://pypistats.org/packages/bert4torch)
 [![GitHub stars](https://img.shields.io/github/stars/Tongjilibo/bert4torch?style=social)](https://github.com/Tongjilibo/bert4torch)
@@ -39,21 +29,20 @@
 
 - **注意事项**：pip包的发布慢于git上的开发版本，git clone**注意引用路径**，注意权重是否需要转换
 - **测试用例**：`git clone https://github.com/Tongjilibo/bert4torch`，修改example中的预训练模型文件路径和数据路径即可启动脚本
 - **自行训练**：针对自己的数据，修改相应的数据处理代码块
 - **开发环境**：原使用`torch==1.10`版本进行开发，现已切换到`torch2.0`开发，如其他版本遇到不适配，欢迎反馈
 
 ## 2. 功能
-
-- **LLM模型**: 加载chatglm-6b和llama-7b进行推理和finetune
+- **LLM模型**: 加载chatglm、llama、 baichuan、ziya、bloom等开源大模型权重进行推理和微调
 - **核心功能**：加载bert、roberta、albert、xlnet、nezha、bart、RoFormer、RoFormer_V2、ELECTRA、GPT、GPT2、T5、GAU-alpha、ERNIE等预训练权重继续进行finetune、并支持在bert基础上灵活定义自己模型
-- [**丰富示例**](https://github.com/Tongjilibo/bert4torch/blob/master/examples/)：包含[pretrain](https://github.com/Tongjilibo/bert4torch/blob/master/examples/pretrain)、[sentence_classfication](https://github.com/Tongjilibo/bert4torch/blob/master/examples/sentence_classfication)、[sentence_embedding](https://github.com/Tongjilibo/bert4torch/tree/master/examples/sentence_embedding)、[sequence_labeling](https://github.com/Tongjilibo/bert4torch/blob/master/examples/sequence_labeling)、[relation_extraction](https://github.com/Tongjilibo/bert4torch/blob/master/examples/relation_extraction)、[seq2seq](https://github.com/Tongjilibo/bert4torch/blob/master/examples/seq2seq)、[serving](https://github.com/Tongjilibo/bert4torch/blob/master/examples/serving/)等多种解决方案
+- [**丰富示例**](https://github.com/Tongjilibo/bert4torch/blob/master/examples/)：包含[llm](https://github.com/Tongjilibo/bert4torch/blob/master/examples/llm)、[pretrain](https://github.com/Tongjilibo/bert4torch/blob/master/examples/pretrain)、[sentence_classfication](https://github.com/Tongjilibo/bert4torch/blob/master/examples/sentence_classfication)、[sentence_embedding](https://github.com/Tongjilibo/bert4torch/tree/master/examples/sentence_embedding)、[sequence_labeling](https://github.com/Tongjilibo/bert4torch/blob/master/examples/sequence_labeling)、[relation_extraction](https://github.com/Tongjilibo/bert4torch/blob/master/examples/relation_extraction)、[seq2seq](https://github.com/Tongjilibo/bert4torch/blob/master/examples/seq2seq)、[serving](https://github.com/Tongjilibo/bert4torch/blob/master/examples/serving/)等多种解决方案
 - **实验验证**：已在公开数据集实验验证，使用如下[examples数据集](https://github.com/Tongjilibo/bert4torch/blob/master/examples/README.md)
 - **易用trick**：集成了常见的[trick](https://github.com/Tongjilibo/bert4torch/blob/master/examples/training_trick)，即插即用
-- **其他特性**：[加载transformers库模型](https://github.com/Tongjilibo/bert4torch/blob/master/examples/tutorials/tutorials_load_transformers_model.py)一起使用；调用方式简洁高效；有训练进度条动态展示；配合torchinfo打印参数量；默认Logger和Tensorboard简便记录训练过程；自定义fit过程，满足高阶需求
+- **其他特性**：[加载transformers库模型](https://github.com/Tongjilibo/bert4torch/blob/master//tutorials/tutorials_load_transformers_model.py)一起使用；调用方式简洁高效；有训练进度条动态展示；配合torchinfo打印参数量；默认Logger和Tensorboard简便记录训练过程；自定义fit过程，满足高阶需求
 - **训练过程**：
 
   ```text
   2022-10-28 23:16:10 - Start Training
   2022-10-28 23:16:10 - Epoch: 1/2
   5000/5000 [==============================] - 13s 3ms/step - loss: 0.1351 - acc: 0.9601
   Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 798.09it/s] 
@@ -63,25 +52,38 @@
   5000/5000 [==============================] - 13s 3ms/step - loss: 0.0465 - acc: 0.9862
   Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 635.78it/s] 
   test_acc: 0.98280. best_test_acc: 0.98280
 
   2022-10-28 23:16:44 - Finish Training
   ```
 
+|          功能                | bert4torch |  transformers | 备注 |
+|-----------------------------|------------|:--------------|--------|
+|训练进度条                     | ✅         |      ✅        |进度条打印loss和定义的metrics|
+|分布式训练dp/ddp               | ✅         |      ✅        |torch自带dp/ddp|
+|各类callbacks                 | ✅         |      ✅        |日志/tensorboard/earlystop/wandb等|
+|大模型推理，stream/batch输出    | ✅         |      ✅        |各个模型是通用的，无需单独维护脚本|
+|大模型微调                     | ✅         |      ✅        |lora依赖peft库，pv2自带|
+|丰富tricks                    | ✅         |      ❌        |对抗训练等tricks即插即用|
+|代码简洁易懂，自定义空间大        | ✅         |      ❌        |代码复用度高, keras代码训练风格|
+|仓库的维护能力/影响力/使用量/兼容性| ❌         |      ✅        |目前仓库个人维护|
+
+
 ## 3. 快速上手
 
 - [Quick-Start](https://bert4torch.readthedocs.io/en/latest//Quick-Start.html)
-- [快速上手教程](https://github.com/Tongjilibo/bert4torch/blob/master/examples/tutorials/Tutorials.md)，[教程示例](https://github.com/Tongjilibo/bert4torch/blob/master/examples/tutorials)，[实战示例](https://github.com/Tongjilibo/bert4torch/blob/master/examples)
+- [快速上手教程](https://github.com/Tongjilibo/bert4torch/blob/master//tutorials/README.md)，[教程示例](https://github.com/Tongjilibo/bert4torch/blob/master//tutorials)，[实战示例](https://github.com/Tongjilibo/bert4torch/blob/master/examples)
 - [bert4torch介绍(知乎)](https://zhuanlan.zhihu.com/p/486329434)，[bert4torch快速上手(知乎)](https://zhuanlan.zhihu.com/p/508890807)，[bert4torch又双叒叕更新啦(知乎)](https://zhuanlan.zhihu.com/p/560885427?)
 
 ## 4. 版本历史
 
 <details><summary><b>点击查看</b></summary>
 
 **版本说明**
+- **v0.3.1**：20230725 修改baichuan的alibi逻辑，增加bloom, 简化decoder架构代码(gpt, llama, chatglm均继承decoder)
 - **v0.3.0**：20230716 修改models和layers为文件夹方便扩展, 增加flash_attention参数控制，修改skip_init逻辑减少显存占用，generation增加repetition_penalty，修复chatglm的pv2的bug，generation支持transformers的tokenize，增加ziya，Baichuan
 - **v0.2.9**: 20230705 使用accelerate来实现skip_init精简代码, 修复add_trainer的代码提示, 增加chatglm的load_in_8bit+lora/qlora的训练, 修复grad_chechpoint, 增加chinese_llama_alpaca, torch2.0默认使用scaled_dot_product_attention加速, 增加chatglm2-6b+pv2+lora微调
 - **v0.2.8**：20230518 【新增模型】增加chatglm-6b/llama-7b/BELLE_llama/vicuna/moss/苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型/fnlp的bart2.0, 增加量化模块并适配llama，增加skip_init参数加快加载, 增加stream输出/网页demo, 增加ptuning_v2和lora; 【generation】生成式解码新增SeqGeneration和Seq2SeqGeneration，单向decoder模型和encoder decoder模型解码增加cache, 增加batch_generate()/stream_generate功能；【其他】修改rope为不使用max_position，修复model.half()类型不一致问题，支持加载多个权重文件, gpt系列默认不加softmax，增加苏神Tiger的pytorch实现, 增加了对attention_key_size的入参支持，把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段
 - **v0.2.7.post2**：20230310 增加lion优化器, 修复albert_unshared加载权重, 修复lm系列(gpt, seq2seq)存在的forward参数不对的问题，修复GlobalPointer使用rope的bug
 - **v0.2.7**：20230213 修复random_sample()的bug，适配v0.0.6的torch4keras：增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现，增加了AccelerateCallback
 - **v0.2.6**：20221231 build_transformer_model需显式指定add_trainer才从BaseModel继承, 增加guwenbert, macbert，text2vec-bert-chinese, wobert预训练模型，允许position_ids从padding开始, transformer.configs支持点操作，可以使用torch4keras的Trainer(net)来初始化, 修复tokenizer的切分subtoken的bug, 允许embedding_size!=hidden_size
 - **v0.2.5**：20221127 对抗训练从compile转为使用Callback来实现，修复1.7.1版本兼容bug, uie模型内置
@@ -98,14 +100,15 @@
 - **v0.1.4**：20220421 增加了VAT，修复了linux下apply_embedding返回项有问题的情况
 - **v0.1.3**：20220409 初始版本
 
 **版本对应关系**
 
 | bert4torch版本 | torch4keras版本 |
 | ---------------- | ----------------- |
+| 0.3.1          | 0.1.0           |
 | 0.3.0          | 0.0.9           |
 | 0.2.9          | 0.0.8           |
 | 0.2.8          | 0.0.7.post3     |
 | 0.2.7.post2    | 0.0.6           |
 | 0.2.7          | 0.0.6           |
 | 0.2.6          | 0.0.5           |
 | 0.2.5          | 0.0.4           |
@@ -115,14 +118,15 @@
 
 </details>
 
 
 ## 5. 更新历史：
 <details><summary><b>点击查看</b></summary>
 
+- **20230725**：修改baichuan的alibi逻辑，增加bloom, 简化decoder架构代码(gpt, llama, chatglm均继承decoder)
 - **20230716**：修改models和layers为文件夹方便扩展, 增加flash_attention参数控制，增加chatglm-api示例，修改skip_init逻辑减少显存占用，generation增加repetition_penalty，修复chatglm的pv2的bug，generation支持transformers的tokenize，增加ziya，Baichuan
 - **20230705**：使用accelerate来实现skip_init精简代码, 修复add_trainer的代码提示, 增加chatglm的load_in_8bit+lora/qlora的训练, 修复grad_chechpoint, 增加chinese_llama_alpaca, torch2.0默认使用scaled_dot_product_attention加速, 增加chatglm2-6b+pv2+lora微调
 - **20230518**：增加vicuna的集成, 增加batch_generate()功能, 把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段
 - **20230408**：增加苏神Tiger的pytorch实现, 集成苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型, 增加了对attention_key_size的入参支持，单向decoder模型和encoder decoder模型解码增加cache, 更新fnlp的bart2.0, 增加chatglm-6b预训练模型推理, 集成BELLE_llama模型, 增加量化模块并适配llama，增加skip_init参数加快加载, 增加stream输出/网页demo, 增加ptuning_v2，增加moss模型的int4/int8推理
 - **20230326**：增加llama-7b预训练模型, 修改rope为不使用max_position, 增加prompt_clue和nezha_gpt_dialog的finetune示例(skykiseki用户)，修复model.half()类型不一致问题，生成式解码新增SeqGeneration和Seq2SeqGeneration, 支持加载多个权重文件, gpt系列默认不加softmax
 - **20230310**：增加lion优化器, 修改dp和ddp示例更易用，增加PromptCLUE模型, 修复albert_unshared加载权重, 增加uer-gpt2-chinese预训练模型，修复lm系列(gpt, seq2seq)存在的forward参数不对的问题，修复GlobalPointer使用rope的bug
 - **20230212**：兼容accelerate包, 增加ChatYuan v1模型，修复random_sample()的bug
@@ -192,19 +196,22 @@
 | bart| 复旦| [torch](https://github.com/fastnlp/CPT), [v1.0](https://huggingface.co/fnlp/bart-base-chinese/tree/v1.0), [v2.0](https://huggingface.co/fnlp/bart-base-chinese/tree/v2.0)| [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_bart_fudanNLP.py) |
 | text2vec| text2vec-base-chinese | [torch](https://huggingface.co/shibing624/text2vec-base-chinese) | |
 | chatyuan v1&v2| clue-ai | [torch](https://github.com/clue-ai/ChatYuan) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
 | PromptCLUE| clue-ai | [torch](https://github.com/clue-ai/PromptCLUE) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
 | chatglm-6b | THUDM | [git](https://github.com/THUDM/ChatGLM-6B), [v0.1.0](https://huggingface.co/THUDM/chatglm-6b/tree/v0.1.0), [v1.1.0](https://huggingface.co/THUDM/chatglm-6b/tree/v1.1.0), [int8](https://huggingface.co/THUDM/chatglm-6b-int8), [int4](https://huggingface.co/THUDM/chatglm-6b-int4) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_chatglm.py) |
 | chatglm2-6b | THUDM | [git](https://github.com/THUDM/ChatGLM2-6B), [v2](https://huggingface.co/THUDM/chatglm2-6b), [int4](https://huggingface.co/THUDM/chatglm2-6b-int4) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_chatglm.py) |
 | llama | facebook| [git](https://github.com/facebookresearch/llama) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_pth.py)|
+| llama2 | facebook| [git](https://github.com/facebookresearch/llama) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_hf.py)|
 |chinese_llama_alpaca|Yiming Cui|[git](https://github.com/ymcui/Chinese-LLaMA-Alpaca) |[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_pth.py)|
 | vicuna | FastChat| [torch](https://huggingface.co/AlekseyKorshuk/vicuna-7b) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_hf.py)|
 | Belle_llama| LianjiaTech| [git](https://github.com/LianjiaTech/BELLE), [7B-2M-enc](https://huggingface.co/BelleGroup/BELLE-LLaMA-7B-2M-enc) | [合成说明](https://github.com/LianjiaTech/BELLE/tree/main/models)、[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_hf.py)|
 | Ziya | IDEA-CCNL | [v1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-v1), [v1.1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-v1.1), [pretrain-v1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-Pretrain-v1) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_pth.py) |
 | Baichuan | baichuan-inc | [7B](https://github.com/baichuan-inc/Baichuan-7B), [13B-Base](https://huggingface.co/baichuan-inc/Baichuan-13B-Base), [13B-Chat](https://huggingface.co/baichuan-inc/Baichuan-13B-Chat) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_hf.py) |
+| bloom | bigscience | [560m](https://huggingface.co/bigscience/bloom-560m) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_bloom.py) |
+
 
 ## 7. 鸣谢
 
 - 感谢苏神实现的[bert4keras](https://github.com/bojone/bert4keras)，本实现有不少地方参考了bert4keras的源码，在此衷心感谢大佬的无私奉献;
 - 其次感谢项目[bert4pytorch](https://github.com/MuQiuJun-AI/bert4pytorch)，也是在该项目的指引下给了我用pytorch来复现bert4keras的想法和思路。
 
 ## 8. 引用
@@ -244,8 +251,8 @@
     <tr align="center" >
       <td>
          <a href="https://star-history.com/#Tongjilibo/bert4torch&Date"><img width="400" height="250" src="https://api.star-history.com/svg?repos=Tongjilibo/bert4torch&type=Date" alt="pic"></a><br>
          <a href="https://star-history.com/#Tongjilibo/bert4torch&Date">Star History Chart</a> 
       </td>
     </tr>
   </tbody>
-</table>
+</table>
```

### Comparing `bert4torch-0.3.0/bert4torch.egg-info/SOURCES.txt` & `bert4torch-0.3.1/bert4torch.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 bert4torch/layers/position_encoding.py
 bert4torch/layers/transformer_block.py
 bert4torch/models/__init__.py
 bert4torch/models/albert.py
 bert4torch/models/bart.py
 bert4torch/models/base.py
 bert4torch/models/bert.py
+bert4torch/models/bloom.py
 bert4torch/models/deberta.py
 bert4torch/models/electra.py
 bert4torch/models/erinie.py
 bert4torch/models/gau_alpha.py
 bert4torch/models/glm.py
 bert4torch/models/gpt.py
 bert4torch/models/llama.py
```

### Comparing `bert4torch-0.3.0/setup.py` & `bert4torch-0.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='bert4torch',
-    version='v0.3.0',
+    version='v0.3.1',
     description='an elegant bert4torch',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT Licence',
     url='https://github.com/Tongjilibo/bert4torch',
     author='Tongjilibo',
-    install_requires=['torch>1.6', 'torch4keras==0.0.9'],
+    install_requires=['torch>1.6', 'torch4keras==0.1.0'],
     packages=find_packages()
 )
```

