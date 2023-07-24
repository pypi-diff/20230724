# Comparing `tmp/bytetrade-recommend-model-sdk-0.0.27.tar.gz` & `tmp/bytetrade-recommend-model-sdk-0.0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bytetrade-recommend-model-sdk-0.0.27.tar", last modified: Sat Jul 22 02:13:46 2023, max compression
+gzip compressed data, was "bytetrade-recommend-model-sdk-0.0.28.tar", last modified: Mon Jul 24 08:53:04 2023, max compression
```

## Comparing `bytetrade-recommend-model-sdk-0.0.27.tar` & `bytetrade-recommend-model-sdk-0.0.28.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-22 02:13:46.691041 bytetrade-recommend-model-sdk-0.0.27/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.27/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-07-22 02:13:46.691041 bytetrade-recommend-model-sdk-0.0.27/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1904 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.27/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-22 02:13:46.683041 bytetrade-recommend-model-sdk-0.0.27/bytetrade_recommend_model_sdk.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-07-22 02:13:46.000000 bytetrade-recommend-model-sdk-0.0.27/bytetrade_recommend_model_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2178 2023-07-22 02:13:46.000000 bytetrade-recommend-model-sdk-0.0.27/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-22 02:13:46.000000 bytetrade-recommend-model-sdk-0.0.27/bytetrade_recommend_model_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       63 2023-07-22 02:13:46.000000 bytetrade-recommend-model-sdk-0.0.27/bytetrade_recommend_model_sdk.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-07-22 02:13:46.000000 bytetrade-recommend-model-sdk-0.0.27/bytetrade_recommend_model_sdk.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-22 02:13:46.683041 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-22 02:13:46.687041 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/embeddings/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/embeddings/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3875 2023-07-16 23:12:22.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/embeddings/bert_embedding.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      872 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/embeddings/embedding_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5430 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/embeddings/word2vec_embedding.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-22 02:13:46.687041 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-22 02:13:46.687041 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/config/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/config/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      675 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/config/content_similar_config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      396 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/config/dnn_click_predictor_config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      201 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/config/mind_base_config.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-22 02:13:46.687041 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/dataset/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/dataset/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4244 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/dataset/mind_base_dataset.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1769 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_dataset.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2719 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_parsed_dataset.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2180 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/dataset/mind_news_dataset.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2873 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/dataset/mind_user_dataset.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-22 02:13:46.687041 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/eval/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/eval/__init_.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1113 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/eval/eval_operation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11667 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/eval/mind_eval_tool.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-22 02:13:46.687041 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/exp/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/exp/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11826 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/exp/mind_dnn_click_predictor_train_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       96 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/experiment_enum.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-22 02:13:46.687041 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/model/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/model/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14888 2023-07-16 23:12:22.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/model/content_similar_model.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2330 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/model/dnn_click_predictor.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-22 02:13:46.687041 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/proto_class/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/proto_class/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23340 2023-07-21 09:10:35.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/proto_class/embedding_pb2.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-22 02:13:46.687041 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/recommend/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/recommend/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4976 2023-07-16 23:12:22.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/recommend/recommend_common_util.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1774 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/recommend/recommend_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2150 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/recommend/time_weight_decay_tool.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-22 02:13:46.687041 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/resources/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/resources/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2508 2023-07-16 23:12:22.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/resources/model_management.json
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-22 02:13:46.691041 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/tools/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/tools/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5148 2023-07-21 12:55:09.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/tools/aws_s3_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10416 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/tools/common_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    36818 2023-07-21 12:58:15.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/tools/model_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-22 02:13:46.691041 bytetrade-recommend-model-sdk-0.0.27/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      978 2023-07-22 01:51:32.000000 bytetrade-recommend-model-sdk-0.0.27/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-24 08:53:04.696969 bytetrade-recommend-model-sdk-0.0.28/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.28/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-07-24 08:53:04.696969 bytetrade-recommend-model-sdk-0.0.28/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1904 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.28/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-24 08:53:04.692969 bytetrade-recommend-model-sdk-0.0.28/bytetrade_recommend_model_sdk.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-07-24 08:53:04.000000 bytetrade-recommend-model-sdk-0.0.28/bytetrade_recommend_model_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2178 2023-07-24 08:53:04.000000 bytetrade-recommend-model-sdk-0.0.28/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-24 08:53:04.000000 bytetrade-recommend-model-sdk-0.0.28/bytetrade_recommend_model_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      155 2023-07-24 08:53:04.000000 bytetrade-recommend-model-sdk-0.0.28/bytetrade_recommend_model_sdk.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-07-24 08:53:04.000000 bytetrade-recommend-model-sdk-0.0.28/bytetrade_recommend_model_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-24 08:53:04.692969 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-24 08:53:04.692969 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/embeddings/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/embeddings/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3875 2023-07-16 23:12:22.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/embeddings/bert_embedding.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      872 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/embeddings/embedding_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5430 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/embeddings/word2vec_embedding.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-24 08:53:04.692969 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-24 08:53:04.692969 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/config/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/config/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      675 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/config/content_similar_config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      396 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/config/dnn_click_predictor_config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      201 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/config/mind_base_config.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-24 08:53:04.692969 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/dataset/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/dataset/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4244 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/dataset/mind_base_dataset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1769 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_dataset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2719 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_parsed_dataset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2180 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/dataset/mind_news_dataset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2873 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/dataset/mind_user_dataset.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-24 08:53:04.692969 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/eval/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/eval/__init_.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1113 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/eval/eval_operation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11667 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/eval/mind_eval_tool.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-24 08:53:04.692969 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/exp/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/exp/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11826 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/exp/mind_dnn_click_predictor_train_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       96 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/experiment_enum.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-24 08:53:04.692969 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/model/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/model/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14888 2023-07-16 23:12:22.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/model/content_similar_model.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2330 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/model/dnn_click_predictor.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-24 08:53:04.696969 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/proto_class/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/proto_class/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23340 2023-07-21 09:10:35.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/proto_class/embedding_pb2.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-24 08:53:04.696969 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/recommend/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/recommend/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4976 2023-07-16 23:12:22.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/recommend/recommend_common_util.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1774 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/recommend/recommend_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2150 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/recommend/time_weight_decay_tool.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-24 08:53:04.696969 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/resources/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/resources/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2508 2023-07-16 23:12:22.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/resources/model_management.json
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-24 08:53:04.696969 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/tools/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/tools/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5148 2023-07-21 12:55:09.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/tools/aws_s3_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10416 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/tools/common_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    37549 2023-07-24 08:47:31.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/tools/model_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-24 08:53:04.696969 bytetrade-recommend-model-sdk-0.0.28/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1125 2023-07-24 08:51:25.000000 bytetrade-recommend-model-sdk-0.0.28/setup.py
```

### Comparing `bytetrade-recommend-model-sdk-0.0.27/README.md` & `bytetrade-recommend-model-sdk-0.0.28/README.md`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.27/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt` & `bytetrade-recommend-model-sdk-0.0.28/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/embeddings/bert_embedding.py` & `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/embeddings/bert_embedding.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/embeddings/embedding_tool.py` & `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/embeddings/embedding_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/embeddings/word2vec_embedding.py` & `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/embeddings/word2vec_embedding.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/config/content_similar_config.py` & `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/config/content_similar_config.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/dataset/mind_base_dataset.py` & `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/dataset/mind_base_dataset.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_dataset.py` & `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_dataset.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_parsed_dataset.py` & `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_parsed_dataset.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/dataset/mind_news_dataset.py` & `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/dataset/mind_news_dataset.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/dataset/mind_user_dataset.py` & `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/dataset/mind_user_dataset.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/eval/eval_operation.py` & `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/eval/eval_operation.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/eval/mind_eval_tool.py` & `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/eval/mind_eval_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/exp/mind_dnn_click_predictor_train_tool.py` & `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/exp/mind_dnn_click_predictor_train_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/model/content_similar_model.py` & `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/model/content_similar_model.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/model/dnn_click_predictor.py` & `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/model/dnn_click_predictor.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/proto_class/embedding_pb2.py` & `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/proto_class/embedding_pb2.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/recommend/recommend_common_util.py` & `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/recommend/recommend_common_util.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/recommend/recommend_tool.py` & `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/recommend/recommend_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/recommend/time_weight_decay_tool.py` & `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/recommend/time_weight_decay_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/resources/model_management.json` & `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/resources/model_management.json`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/tools/aws_s3_tool.py` & `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/tools/aws_s3_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/tools/common_tool.py` & `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/tools/common_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/tools/model_tool.py` & `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/tools/model_tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import base64
 from datetime import datetime
+from langdetect import detect
+
 import os
 from google.protobuf.json_format import Parse, ParseDict,MessageToDict
 import nltk
 import zlib
 
 from recommend_model_sdk.tools.aws_s3_tool import AWSS3Tool
 from recommend_model_sdk.tools.common_tool import CommonTool
@@ -686,7 +688,25 @@
         
         decompress_bytes = zlib.decompress(current_package_compress_byte)
         current_latest_package = rec_proto_embebding.KeywordSortedInfoPackage()
         current_latest_package.ParseFromString(decompress_bytes)
         
         keyword_sortinfo_dict = MessageToDict(current_latest_package,preserving_proto_field_name=True)
         return keyword_sortinfo_dict["keyword_sortinfo_list"]
+    
+    def infer_text_language_type(self,text):
+        """
+        af, ar, bg, bn, ca, cs, cy, da, de, el, en, es, et, fa, fi, fr, gu, he,
+        hi, hr, hu, id, it, ja, kn, ko, lt, lv, mk, ml, mr, ne, nl, no, pa, pl,
+        pt, ro, ru, sk, sl, so, sq, sv, sw, ta, te, th, tl, tr, uk, ur, vi, zh-cn, zh-tw
+        https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes
+        """
+        if isinstance(text,str) is False:
+            raise ValueError("text is not str")
+        language_type = None
+        try:
+            language_type = detect(text)
+        except Exception as ex:
+            self.__logger.debug(f'language_type ex: {str(ex)}')
+        return language_type
+        
+
```

### Comparing `bytetrade-recommend-model-sdk-0.0.27/setup.py` & `bytetrade-recommend-model-sdk-0.0.28/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -21,18 +21,23 @@
 sys.path.append(os.path.dirname(__file__) + "/recommend-model")
 
 
 
 
 setup(
     name="bytetrade-recommend-model-sdk",
-    version="0.0.27",
+    version="0.0.28",
     # packages=find_packages(exclude="unit_test"),
     install_requires=[
         "pandas==2.0.0",
         "gensim==4.3.1",
         "protobuf==3.20.1",
         "nltk==3.8.1",
-        "boto3"
+        "boto3",
+        "faiss-cpu==1.7.4",
+        "matplotlib",
+        "rake-nltk==1.0.6",
+        "sentence-transformers==2.2.2",
+        "langdetect==1.0.9"
     ],
     include_package_data=True
 )
```

