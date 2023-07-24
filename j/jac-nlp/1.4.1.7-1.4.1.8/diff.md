# Comparing `tmp/jac_nlp-1.4.1.7.tar.gz` & `tmp/jac_nlp-1.4.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jac_nlp-1.4.1.7.tar", last modified: Thu Jul 20 04:00:55 2023, max compression
+gzip compressed data, was "jac_nlp-1.4.1.8.tar", last modified: Mon Jul 24 16:59:16 2023, max compression
```

## Comparing `jac_nlp-1.4.1.7.tar` & `jac_nlp-1.4.1.8.tar`

### file list

```diff
@@ -1,210 +1,210 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.344596 jac_nlp-1.4.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-20 04:00:55.344596 jac_nlp-1.4.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    42252 2023-07-20 04:00:36.000000 jac_nlp-1.4.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.328596 jac_nlp-1.4.1.7/jac_nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 04:00:36.000000 jac_nlp-1.4.1.7/jac_nlp/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:36.000000 jac_nlp-1.4.1.7/jac_nlp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.328596 jac_nlp-1.4.1.7/jac_nlp/action_configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:36.000000 jac_nlp-1.4.1.7/jac_nlp/action_configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-07-20 04:00:36.000000 jac_nlp-1.4.1.7/jac_nlp/action_configs/bart_sum_action_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-20 04:00:36.000000 jac_nlp-1.4.1.7/jac_nlp/action_configs/bi_enc_action_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-07-20 04:00:36.000000 jac_nlp-1.4.1.7/jac_nlp/action_configs/bi_ner_action_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-07-20 04:00:36.000000 jac_nlp-1.4.1.7/jac_nlp/action_configs/cl_summer_action_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-07-20 04:00:36.000000 jac_nlp-1.4.1.7/jac_nlp/action_configs/ent_ext_action_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-07-20 04:00:36.000000 jac_nlp-1.4.1.7/jac_nlp/action_configs/fast_enc_action_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-07-20 04:00:36.000000 jac_nlp-1.4.1.7/jac_nlp/action_configs/paraphraser_action_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-07-20 04:00:36.000000 jac_nlp-1.4.1.7/jac_nlp/action_configs/sbert_sim_action_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-20 04:00:36.000000 jac_nlp-1.4.1.7/jac_nlp/action_configs/sentiment_action_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-07-20 04:00:36.000000 jac_nlp-1.4.1.7/jac_nlp/action_configs/t5_sum_action_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-07-20 04:00:36.000000 jac_nlp-1.4.1.7/jac_nlp/action_configs/text_seg_action_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-07-20 04:00:36.000000 jac_nlp-1.4.1.7/jac_nlp/action_configs/tfm_ner_action_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-20 04:00:36.000000 jac_nlp-1.4.1.7/jac_nlp/action_configs/topic_ext_action_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-20 04:00:36.000000 jac_nlp-1.4.1.7/jac_nlp/action_configs/use_enc_action_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-07-20 04:00:36.000000 jac_nlp-1.4.1.7/jac_nlp/action_configs/use_qa_action_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-07-20 04:00:36.000000 jac_nlp-1.4.1.7/jac_nlp/action_configs/zs_classifier_action_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.332596 jac_nlp-1.4.1.7/jac_nlp/bart_sum/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-20 04:00:36.000000 jac_nlp-1.4.1.7/jac_nlp/bart_sum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-07-20 04:00:36.000000 jac_nlp-1.4.1.7/jac_nlp/bart_sum/bart_sum.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-20 04:00:36.000000 jac_nlp-1.4.1.7/jac_nlp/bart_sum/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.332596 jac_nlp-1.4.1.7/jac_nlp/bi_enc/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-20 04:00:36.000000 jac_nlp-1.4.1.7/jac_nlp/bi_enc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14563 2023-07-20 04:00:36.000000 jac_nlp-1.4.1.7/jac_nlp/bi_enc/bi_enc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12713 2023-07-20 04:00:36.000000 jac_nlp-1.4.1.7/jac_nlp/bi_enc/poly_enc.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-20 04:00:36.000000 jac_nlp-1.4.1.7/jac_nlp/bi_enc/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-07-20 04:00:36.000000 jac_nlp-1.4.1.7/jac_nlp/bi_enc/sent_enc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.332596 jac_nlp-1.4.1.7/jac_nlp/bi_enc/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:36.000000 jac_nlp-1.4.1.7/jac_nlp/bi_enc/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.332596 jac_nlp-1.4.1.7/jac_nlp/bi_enc/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:36.000000 jac_nlp-1.4.1.7/jac_nlp/bi_enc/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-20 04:00:36.000000 jac_nlp-1.4.1.7/jac_nlp/bi_enc/tests/fixtures/bi_enc.jac
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-07-20 04:00:36.000000 jac_nlp-1.4.1.7/jac_nlp/bi_enc/tests/test_bi_enc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.332596 jac_nlp-1.4.1.7/jac_nlp/bi_enc/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-20 04:00:36.000000 jac_nlp-1.4.1.7/jac_nlp/bi_enc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-07-20 04:00:36.000000 jac_nlp-1.4.1.7/jac_nlp/bi_enc/utils/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-20 04:00:36.000000 jac_nlp-1.4.1.7/jac_nlp/bi_enc/utils/model_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     9975 2023-07-20 04:00:36.000000 jac_nlp-1.4.1.7/jac_nlp/bi_enc/utils/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8153 2023-07-20 04:00:36.000000 jac_nlp-1.4.1.7/jac_nlp/bi_enc/utils/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-07-20 04:00:36.000000 jac_nlp-1.4.1.7/jac_nlp/bi_enc/utils/train.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-20 04:00:36.000000 jac_nlp-1.4.1.7/jac_nlp/bi_enc/utils/train_config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.332596 jac_nlp-1.4.1.7/jac_nlp/bi_ner/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-20 04:00:36.000000 jac_nlp-1.4.1.7/jac_nlp/bi_ner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7382 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/bi_ner/bi_ner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.332596 jac_nlp-1.4.1.7/jac_nlp/bi_ner/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/bi_ner/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/bi_ner/config/m_config.json
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/bi_ner/config/t_config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.332596 jac_nlp-1.4.1.7/jac_nlp/bi_ner/datamodel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/bi_ner/datamodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/bi_ner/datamodel/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/bi_ner/datamodel/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/bi_ner/datamodel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.336596 jac_nlp-1.4.1.7/jac_nlp/bi_ner/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/bi_ner/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14986 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/bi_ner/model/base_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/bi_ner/model/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/bi_ner/model/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/bi_ner/model/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    15772 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/bi_ner/model/ph_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/bi_ner/model/tokenize_data.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/bi_ner/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.336596 jac_nlp-1.4.1.7/jac_nlp/bi_ner/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/bi_ner/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.336596 jac_nlp-1.4.1.7/jac_nlp/bi_ner/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/bi_ner/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/bi_ner/tests/fixtures/bi_ner.jac
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/bi_ner/tests/test_bi_ner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.336596 jac_nlp-1.4.1.7/jac_nlp/cl_summer/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/cl_summer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/cl_summer/cl_summer.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/cl_summer/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.336596 jac_nlp-1.4.1.7/jac_nlp/cl_summer/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/cl_summer/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.336596 jac_nlp-1.4.1.7/jac_nlp/cl_summer/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/cl_summer/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/cl_summer/tests/fixtures/cl_summer.jac
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/cl_summer/tests/test_cl_summer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.336596 jac_nlp-1.4.1.7/jac_nlp/dolly/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/dolly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/dolly/dolly.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/dolly/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.336596 jac_nlp-1.4.1.7/jac_nlp/ent_ext/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/ent_ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/ent_ext/config.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    15307 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/ent_ext/ent_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/ent_ext/entity_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/ent_ext/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.336596 jac_nlp-1.4.1.7/jac_nlp/ent_ext/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/ent_ext/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.336596 jac_nlp-1.4.1.7/jac_nlp/ent_ext/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/ent_ext/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/ent_ext/tests/fixtures/ent_ext.jac
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/ent_ext/tests/test_ent_ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.336596 jac_nlp-1.4.1.7/jac_nlp/gpt2/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/gpt2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/gpt2/gpt2.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/gpt2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/gpt2/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.336596 jac_nlp-1.4.1.7/jac_nlp/gpt3/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/gpt3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/gpt3/gpt3.py
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/gpt3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.340596 jac_nlp-1.4.1.7/jac_nlp/llm/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/llm/dataset_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/llm/llm.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/llm/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.340596 jac_nlp-1.4.1.7/jac_nlp/paraphraser/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/paraphraser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/paraphraser/config.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/paraphraser/paraphraser.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/paraphraser/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.340596 jac_nlp-1.4.1.7/jac_nlp/paraphraser/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/paraphraser/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.340596 jac_nlp-1.4.1.7/jac_nlp/paraphraser/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/paraphraser/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/paraphraser/tests/fixtures/paraphraser.jac
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/paraphraser/tests/test_paraphraser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.340596 jac_nlp-1.4.1.7/jac_nlp/sbert_sim/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/sbert_sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/sbert_sim/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/sbert_sim/sbert_sim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.340596 jac_nlp-1.4.1.7/jac_nlp/sbert_sim/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/sbert_sim/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.340596 jac_nlp-1.4.1.7/jac_nlp/sbert_sim/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/sbert_sim/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/sbert_sim/tests/fixtures/sbert_sim.jac
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/sbert_sim/tests/test_sbert_sim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.340596 jac_nlp-1.4.1.7/jac_nlp/sentiment/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/sentiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/sentiment/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/sentiment/sentiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.340596 jac_nlp-1.4.1.7/jac_nlp/t5_sum/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/t5_sum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/t5_sum/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/t5_sum/t5_sum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.340596 jac_nlp-1.4.1.7/jac_nlp/t5_sum/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/t5_sum/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.340596 jac_nlp-1.4.1.7/jac_nlp/t5_sum/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/t5_sum/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/t5_sum/tests/fixtures/t5_sum.jac
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/t5_sum/tests/test_t5_sum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.340596 jac_nlp-1.4.1.7/jac_nlp/text_seg/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/text_seg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/text_seg/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/text_seg/text_seg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.344596 jac_nlp-1.4.1.7/jac_nlp/tfm_ner/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/tfm_ner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/tfm_ner/entity_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/tfm_ner/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.344596 jac_nlp-1.4.1.7/jac_nlp/tfm_ner/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/tfm_ner/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.344596 jac_nlp-1.4.1.7/jac_nlp/tfm_ner/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/tfm_ner/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/tfm_ner/tests/fixtures/tfm_ner.jac
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/tfm_ner/tests/test_tfm_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7412 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/tfm_ner/tfm_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/tfm_ner/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.344596 jac_nlp-1.4.1.7/jac_nlp/tfm_ner/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/tfm_ner/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/tfm_ner/utils/data_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/tfm_ner/utils/model_config.json
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/tfm_ner/utils/train_config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.344596 jac_nlp-1.4.1.7/jac_nlp/topic_ext/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/topic_ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/topic_ext/action_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/topic_ext/config.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/topic_ext/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/topic_ext/topic_ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.344596 jac_nlp-1.4.1.7/jac_nlp/use_enc/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/use_enc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/use_enc/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.344596 jac_nlp-1.4.1.7/jac_nlp/use_enc/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/use_enc/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.344596 jac_nlp-1.4.1.7/jac_nlp/use_enc/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/use_enc/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/use_enc/tests/fixtures/use_enc.jac
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/use_enc/tests/test_use_enc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/use_enc/use_enc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.344596 jac_nlp-1.4.1.7/jac_nlp/use_qa/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/use_qa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/use_qa/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.344596 jac_nlp-1.4.1.7/jac_nlp/use_qa/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/use_qa/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.344596 jac_nlp-1.4.1.7/jac_nlp/use_qa/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/use_qa/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/use_qa/tests/fixtures/use_qa.jac
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/use_qa/tests/test_use_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/use_qa/use_qa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.344596 jac_nlp-1.4.1.7/jac_nlp/zs_classifier/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/zs_classifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/zs_classifier/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/jac_nlp/zs_classifier/zs_classifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.328596 jac_nlp-1.4.1.7/jac_nlp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-20 04:00:55.000000 jac_nlp-1.4.1.7/jac_nlp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-07-20 04:00:55.000000 jac_nlp-1.4.1.7/jac_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 04:00:55.000000 jac_nlp-1.4.1.7/jac_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-20 04:00:55.000000 jac_nlp-1.4.1.7/jac_nlp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 04:00:55.000000 jac_nlp-1.4.1.7/jac_nlp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 04:00:55.344596 jac_nlp-1.4.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-20 04:00:37.000000 jac_nlp-1.4.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.873016 jac_nlp-1.4.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-24 16:59:16.873016 jac_nlp-1.4.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    42252 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.841016 jac_nlp-1.4.1.8/jac_nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.845016 jac_nlp-1.4.1.8/jac_nlp/action_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/action_configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/action_configs/bart_sum_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/action_configs/bi_enc_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/action_configs/bi_ner_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/action_configs/cl_summer_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/action_configs/ent_ext_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/action_configs/fast_enc_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/action_configs/paraphraser_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/action_configs/sbert_sim_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/action_configs/sentiment_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/action_configs/t5_sum_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/action_configs/text_seg_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/action_configs/tfm_ner_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/action_configs/topic_ext_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/action_configs/use_enc_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/action_configs/use_qa_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/action_configs/zs_classifier_action_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.845016 jac_nlp-1.4.1.8/jac_nlp/bart_sum/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/bart_sum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/bart_sum/bart_sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/bart_sum/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.845016 jac_nlp-1.4.1.8/jac_nlp/bi_enc/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/bi_enc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14563 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/bi_enc/bi_enc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12713 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/bi_enc/poly_enc.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/bi_enc/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/bi_enc/sent_enc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.845016 jac_nlp-1.4.1.8/jac_nlp/bi_enc/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/bi_enc/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.849017 jac_nlp-1.4.1.8/jac_nlp/bi_enc/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/bi_enc/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/bi_enc/tests/fixtures/bi_enc.jac
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/bi_enc/tests/test_bi_enc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.849017 jac_nlp-1.4.1.8/jac_nlp/bi_enc/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/bi_enc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/bi_enc/utils/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/bi_enc/utils/model_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9975 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/bi_enc/utils/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8153 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/bi_enc/utils/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/bi_enc/utils/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/bi_enc/utils/train_config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.849017 jac_nlp-1.4.1.8/jac_nlp/bi_ner/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/bi_ner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7382 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/bi_ner/bi_ner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.849017 jac_nlp-1.4.1.8/jac_nlp/bi_ner/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/bi_ner/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/bi_ner/config/m_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/bi_ner/config/t_config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.849017 jac_nlp-1.4.1.8/jac_nlp/bi_ner/datamodel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/bi_ner/datamodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/bi_ner/datamodel/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/bi_ner/datamodel/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/bi_ner/datamodel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.853016 jac_nlp-1.4.1.8/jac_nlp/bi_ner/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/bi_ner/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14986 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/bi_ner/model/base_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/bi_ner/model/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/bi_ner/model/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/bi_ner/model/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15772 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/bi_ner/model/ph_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/bi_ner/model/tokenize_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/bi_ner/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.853016 jac_nlp-1.4.1.8/jac_nlp/bi_ner/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/bi_ner/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.853016 jac_nlp-1.4.1.8/jac_nlp/bi_ner/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/bi_ner/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/bi_ner/tests/fixtures/bi_ner.jac
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/bi_ner/tests/test_bi_ner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.853016 jac_nlp-1.4.1.8/jac_nlp/cl_summer/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/cl_summer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/cl_summer/cl_summer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/cl_summer/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.853016 jac_nlp-1.4.1.8/jac_nlp/cl_summer/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/cl_summer/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.853016 jac_nlp-1.4.1.8/jac_nlp/cl_summer/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/cl_summer/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/cl_summer/tests/fixtures/cl_summer.jac
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/cl_summer/tests/test_cl_summer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.853016 jac_nlp-1.4.1.8/jac_nlp/dolly/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/dolly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/dolly/dolly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/dolly/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.857016 jac_nlp-1.4.1.8/jac_nlp/ent_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/ent_ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/ent_ext/config.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    15307 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/ent_ext/ent_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/ent_ext/entity_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/ent_ext/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.857016 jac_nlp-1.4.1.8/jac_nlp/ent_ext/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/ent_ext/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.857016 jac_nlp-1.4.1.8/jac_nlp/ent_ext/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/ent_ext/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/ent_ext/tests/fixtures/ent_ext.jac
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/ent_ext/tests/test_ent_ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.857016 jac_nlp-1.4.1.8/jac_nlp/gpt2/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/gpt2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/gpt2/gpt2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/gpt2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/gpt2/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.857016 jac_nlp-1.4.1.8/jac_nlp/gpt3/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/gpt3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/gpt3/gpt3.py
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/gpt3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.857016 jac_nlp-1.4.1.8/jac_nlp/llm/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/llm/dataset_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/llm/llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/llm/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.861016 jac_nlp-1.4.1.8/jac_nlp/paraphraser/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/paraphraser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/paraphraser/config.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/paraphraser/paraphraser.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/paraphraser/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.861016 jac_nlp-1.4.1.8/jac_nlp/paraphraser/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/paraphraser/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.861016 jac_nlp-1.4.1.8/jac_nlp/paraphraser/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/paraphraser/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/paraphraser/tests/fixtures/paraphraser.jac
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/paraphraser/tests/test_paraphraser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.861016 jac_nlp-1.4.1.8/jac_nlp/sbert_sim/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/sbert_sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/sbert_sim/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/sbert_sim/sbert_sim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.861016 jac_nlp-1.4.1.8/jac_nlp/sbert_sim/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/sbert_sim/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.861016 jac_nlp-1.4.1.8/jac_nlp/sbert_sim/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/sbert_sim/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/sbert_sim/tests/fixtures/sbert_sim.jac
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/sbert_sim/tests/test_sbert_sim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.861016 jac_nlp-1.4.1.8/jac_nlp/sentiment/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/sentiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/sentiment/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/sentiment/sentiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.861016 jac_nlp-1.4.1.8/jac_nlp/t5_sum/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/t5_sum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/t5_sum/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/t5_sum/t5_sum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.865017 jac_nlp-1.4.1.8/jac_nlp/t5_sum/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/t5_sum/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.865017 jac_nlp-1.4.1.8/jac_nlp/t5_sum/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/t5_sum/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/t5_sum/tests/fixtures/t5_sum.jac
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/t5_sum/tests/test_t5_sum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.865017 jac_nlp-1.4.1.8/jac_nlp/text_seg/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/text_seg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/text_seg/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/text_seg/text_seg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.865017 jac_nlp-1.4.1.8/jac_nlp/tfm_ner/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/tfm_ner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/tfm_ner/entity_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/tfm_ner/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.865017 jac_nlp-1.4.1.8/jac_nlp/tfm_ner/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/tfm_ner/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.865017 jac_nlp-1.4.1.8/jac_nlp/tfm_ner/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/tfm_ner/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/tfm_ner/tests/fixtures/tfm_ner.jac
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/tfm_ner/tests/test_tfm_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7412 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/tfm_ner/tfm_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/tfm_ner/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.865017 jac_nlp-1.4.1.8/jac_nlp/tfm_ner/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/tfm_ner/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/tfm_ner/utils/data_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/tfm_ner/utils/model_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/tfm_ner/utils/train_config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.869017 jac_nlp-1.4.1.8/jac_nlp/topic_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/topic_ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/topic_ext/action_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/topic_ext/config.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/topic_ext/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/topic_ext/topic_ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.869017 jac_nlp-1.4.1.8/jac_nlp/use_enc/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/use_enc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/use_enc/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.869017 jac_nlp-1.4.1.8/jac_nlp/use_enc/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/use_enc/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.869017 jac_nlp-1.4.1.8/jac_nlp/use_enc/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/use_enc/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/use_enc/tests/fixtures/use_enc.jac
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/use_enc/tests/test_use_enc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/use_enc/use_enc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.869017 jac_nlp-1.4.1.8/jac_nlp/use_qa/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/use_qa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/use_qa/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.869017 jac_nlp-1.4.1.8/jac_nlp/use_qa/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/use_qa/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.869017 jac_nlp-1.4.1.8/jac_nlp/use_qa/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/use_qa/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/use_qa/tests/fixtures/use_qa.jac
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/use_qa/tests/test_use_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/use_qa/use_qa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.869017 jac_nlp-1.4.1.8/jac_nlp/zs_classifier/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/zs_classifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/zs_classifier/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/jac_nlp/zs_classifier/zs_classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:16.841016 jac_nlp-1.4.1.8/jac_nlp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-24 16:59:16.000000 jac_nlp-1.4.1.8/jac_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-07-24 16:59:16.000000 jac_nlp-1.4.1.8/jac_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 16:59:16.000000 jac_nlp-1.4.1.8/jac_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-24 16:59:16.000000 jac_nlp-1.4.1.8/jac_nlp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 16:59:16.000000 jac_nlp-1.4.1.8/jac_nlp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 16:59:16.873016 jac_nlp-1.4.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-24 16:58:51.000000 jac_nlp-1.4.1.8/setup.py
```

### Comparing `jac_nlp-1.4.1.7/PKG-INFO` & `jac_nlp-1.4.1.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jac_nlp
-Version: 1.4.1.7
+Version: 1.4.1.8
 Home-page: https://github.com/Jaseci-Labs/jaseci
 Author: Jason Mars
 Author-email: jason@jaseci.org
 Provides-Extra: all
 Provides-Extra: bart_sum
 Provides-Extra: cl_summer
 Provides-Extra: ent_ext
```

### Comparing `jac_nlp-1.4.1.7/README.md` & `jac_nlp-1.4.1.8/README.md`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/action_configs/bart_sum_action_config.py` & `jac_nlp-1.4.1.8/jac_nlp/action_configs/bart_sum_action_config.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/action_configs/bi_enc_action_config.py` & `jac_nlp-1.4.1.8/jac_nlp/action_configs/bi_enc_action_config.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/action_configs/bi_ner_action_config.py` & `jac_nlp-1.4.1.8/jac_nlp/action_configs/bi_ner_action_config.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/action_configs/cl_summer_action_config.py` & `jac_nlp-1.4.1.8/jac_nlp/action_configs/cl_summer_action_config.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/action_configs/ent_ext_action_config.py` & `jac_nlp-1.4.1.8/jac_nlp/action_configs/ent_ext_action_config.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/action_configs/fast_enc_action_config.py` & `jac_nlp-1.4.1.8/jac_nlp/action_configs/fast_enc_action_config.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/action_configs/paraphraser_action_config.py` & `jac_nlp-1.4.1.8/jac_nlp/action_configs/paraphraser_action_config.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/action_configs/sbert_sim_action_config.py` & `jac_nlp-1.4.1.8/jac_nlp/action_configs/sbert_sim_action_config.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/action_configs/sentiment_action_config.py` & `jac_nlp-1.4.1.8/jac_nlp/action_configs/sentiment_action_config.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/action_configs/t5_sum_action_config.py` & `jac_nlp-1.4.1.8/jac_nlp/action_configs/t5_sum_action_config.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/action_configs/text_seg_action_config.py` & `jac_nlp-1.4.1.8/jac_nlp/action_configs/text_seg_action_config.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/action_configs/tfm_ner_action_config.py` & `jac_nlp-1.4.1.8/jac_nlp/action_configs/tfm_ner_action_config.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/action_configs/topic_ext_action_config.py` & `jac_nlp-1.4.1.8/jac_nlp/action_configs/topic_ext_action_config.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/action_configs/use_enc_action_config.py` & `jac_nlp-1.4.1.8/jac_nlp/action_configs/use_enc_action_config.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/action_configs/use_qa_action_config.py` & `jac_nlp-1.4.1.8/jac_nlp/action_configs/use_qa_action_config.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/action_configs/zs_classifier_action_config.py` & `jac_nlp-1.4.1.8/jac_nlp/action_configs/zs_classifier_action_config.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/bart_sum/bart_sum.py` & `jac_nlp-1.4.1.8/jac_nlp/bart_sum/bart_sum.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/bi_enc/bi_enc.py` & `jac_nlp-1.4.1.8/jac_nlp/bi_enc/bi_enc.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/bi_enc/poly_enc.py` & `jac_nlp-1.4.1.8/jac_nlp/bi_enc/poly_enc.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/bi_enc/sent_enc.py` & `jac_nlp-1.4.1.8/jac_nlp/bi_enc/sent_enc.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/bi_enc/tests/fixtures/bi_enc.jac` & `jac_nlp-1.4.1.8/jac_nlp/bi_enc/tests/fixtures/bi_enc.jac`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/bi_enc/tests/test_bi_enc.py` & `jac_nlp-1.4.1.8/jac_nlp/bi_enc/tests/test_bi_enc.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/bi_enc/utils/evaluate.py` & `jac_nlp-1.4.1.8/jac_nlp/bi_enc/utils/evaluate.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/bi_enc/utils/models.py` & `jac_nlp-1.4.1.8/jac_nlp/bi_enc/utils/models.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/bi_enc/utils/tokenizer.py` & `jac_nlp-1.4.1.8/jac_nlp/bi_enc/utils/tokenizer.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/bi_enc/utils/train.py` & `jac_nlp-1.4.1.8/jac_nlp/bi_enc/utils/train.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/bi_ner/bi_ner.py` & `jac_nlp-1.4.1.8/jac_nlp/bi_ner/bi_ner.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/bi_ner/datamodel/example.py` & `jac_nlp-1.4.1.8/jac_nlp/bi_ner/datamodel/example.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/bi_ner/datamodel/utils.py` & `jac_nlp-1.4.1.8/jac_nlp/bi_ner/datamodel/utils.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/bi_ner/model/base_encoder.py` & `jac_nlp-1.4.1.8/jac_nlp/bi_ner/model/base_encoder.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/bi_ner/model/inference.py` & `jac_nlp-1.4.1.8/jac_nlp/bi_ner/model/inference.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/bi_ner/model/loss.py` & `jac_nlp-1.4.1.8/jac_nlp/bi_ner/model/loss.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/bi_ner/model/metric.py` & `jac_nlp-1.4.1.8/jac_nlp/bi_ner/model/metric.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/bi_ner/model/ph_model.py` & `jac_nlp-1.4.1.8/jac_nlp/bi_ner/model/ph_model.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/bi_ner/model/tokenize_data.py` & `jac_nlp-1.4.1.8/jac_nlp/bi_ner/model/tokenize_data.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/bi_ner/tests/fixtures/bi_ner.jac` & `jac_nlp-1.4.1.8/jac_nlp/bi_ner/tests/fixtures/bi_ner.jac`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/bi_ner/tests/test_bi_ner.py` & `jac_nlp-1.4.1.8/jac_nlp/bi_ner/tests/test_bi_ner.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/cl_summer/cl_summer.py` & `jac_nlp-1.4.1.8/jac_nlp/cl_summer/cl_summer.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/cl_summer/tests/test_cl_summer.py` & `jac_nlp-1.4.1.8/jac_nlp/cl_summer/tests/test_cl_summer.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/config.py` & `jac_nlp-1.4.1.8/jac_nlp/config.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/dolly/dolly.py` & `jac_nlp-1.4.1.8/jac_nlp/dolly/dolly.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/ent_ext/ent_ext.py` & `jac_nlp-1.4.1.8/jac_nlp/ent_ext/ent_ext.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/ent_ext/entity_utils.py` & `jac_nlp-1.4.1.8/jac_nlp/ent_ext/entity_utils.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/ent_ext/tests/fixtures/ent_ext.jac` & `jac_nlp-1.4.1.8/jac_nlp/ent_ext/tests/fixtures/ent_ext.jac`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/ent_ext/tests/test_ent_ext.py` & `jac_nlp-1.4.1.8/jac_nlp/sbert_sim/tests/test_sbert_sim.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,60 @@
 from jaseci.utils.test_core import CoreTest, jac_testcase
 from jaseci.jsorc.live_actions import load_module_actions, unload_module
 import pytest
 import shutil
 from os import path
 
 
-class EntExtTest(CoreTest):
+class SbertSimTest(CoreTest):
     fixture_src = __file__
-    """
-    Test Class for EntExt Module to test the functionality of api's
-    """
 
     @classmethod
     def setUpClass(cls):
-        super(EntExtTest, cls).setUpClass()
-        ret = load_module_actions("jac_nlp.ent_ext")
+        super(SbertSimTest, cls).setUpClass()
+        ret = load_module_actions("jac_nlp.sbert_sim")
         assert ret is True
 
     @pytest.mark.order(1)
-    @jac_testcase("ent_ext.jac", "test_ent_ext_set_config")
-    def test_ent_ext_set_config(self, ret):
+    @jac_testcase("sbert_sim.jac", "test_sbert_sim_load_model")
+    def test_sbert_sim_load_model(self, ret):
         self.assertEqual(ret["success"], True)
 
     @pytest.mark.order(2)
-    @jac_testcase("ent_ext.jac", "test_train_ner")
-    def test_train_ner(self, ret):
+    @jac_testcase("sbert_sim.jac", "test_train_sbert_sim")
+    def test_train_sbert_sim(self, ret):
         self.assertEqual(ret["success"], True)
+        self.assertEqual(ret["report"][0], "Model Training is completed")
 
-    @pytest.mark.order(3)
-    @jac_testcase("ent_ext.jac", "test_extract_entity")
-    def test_extract_entity(self, ret):
+    @pytest.mark.order(4)
+    @jac_testcase("sbert_sim.jac", "test_get_text_sim")
+    def test_get_text_sim(self, ret):
         self.assertEqual(ret["success"], True)
 
-    @pytest.mark.order(4)
-    @jac_testcase("ent_ext.jac", "test_ent_ext_save_model")
-    def test_ent_ext_save_model(self, ret):
+    @pytest.mark.order(5)
+    @jac_testcase("sbert_sim.jac", "test_sbert_sim_get_train_config")
+    def test_sbert_sim_get_train_config(self, ret):
+        self.assertEqual(ret["success"], True)
+
+    @pytest.mark.order(5)
+    @jac_testcase("sbert_sim.jac", "test_sbert_sim_get_cos_score")
+    def test_sbert_sim_cos_score(self, ret):
+        self.assertEqual(ret["success"], True)
+
+    @pytest.mark.order(5)
+    @jac_testcase("sbert_sim.jac", "test_sbert_sim_get_dot_score")
+    def test_sbert_sim_get_dot_score(self, ret):
         self.assertEqual(ret["success"], True)
 
     @pytest.mark.order(5)
-    @jac_testcase("ent_ext.jac", "test_ent_ext_load_model")
-    def test_ent_ext_load_model(self, ret):
+    @jac_testcase("sbert_sim.jac", "test_sbert_sim_get_embeddings")
+    def test_sbert_sim_get_embeddings(self, ret):
         self.assertEqual(ret["success"], True)
 
     @classmethod
     def tearDownClass(cls):
-        super(EntExtTest, cls).tearDownClass()
-        ret = unload_module("jac_nlp.ent_ext.ent_ext")
+        super(SbertSimTest, cls).tearDownClass()
+        ret = unload_module("jac_nlp.sbert_sim.sbert_sim")
         assert ret is True
-        for temp_path in ["modeloutput", "train"]:
+        for temp_path in ["output"]:
             if path.exists(temp_path) and path.isdir(temp_path):
                 shutil.rmtree(temp_path)
```

### Comparing `jac_nlp-1.4.1.7/jac_nlp/gpt2/gpt2.py` & `jac_nlp-1.4.1.8/jac_nlp/gpt2/gpt2.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/gpt2/train.py` & `jac_nlp-1.4.1.8/jac_nlp/gpt2/train.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/gpt3/gpt3.py` & `jac_nlp-1.4.1.8/jac_nlp/gpt3/gpt3.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/llm/dataset_builder.py` & `jac_nlp-1.4.1.8/jac_nlp/llm/dataset_builder.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/llm/llm.py` & `jac_nlp-1.4.1.8/jac_nlp/llm/llm.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/paraphraser/paraphraser.py` & `jac_nlp-1.4.1.8/jac_nlp/paraphraser/paraphraser.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/paraphraser/tests/test_paraphraser.py` & `jac_nlp-1.4.1.8/jac_nlp/paraphraser/tests/test_paraphraser.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/sbert_sim/sbert_sim.py` & `jac_nlp-1.4.1.8/jac_nlp/sbert_sim/sbert_sim.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/sbert_sim/tests/fixtures/sbert_sim.jac` & `jac_nlp-1.4.1.8/jac_nlp/sbert_sim/tests/fixtures/sbert_sim.jac`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/sentiment/sentiment.py` & `jac_nlp-1.4.1.8/jac_nlp/sentiment/sentiment.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/t5_sum/t5_sum.py` & `jac_nlp-1.4.1.8/jac_nlp/t5_sum/t5_sum.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/t5_sum/tests/test_t5_sum.py` & `jac_nlp-1.4.1.8/jac_nlp/t5_sum/tests/test_t5_sum.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/text_seg/text_seg.py` & `jac_nlp-1.4.1.8/jac_nlp/text_seg/text_seg.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/tfm_ner/entity_utils.py` & `jac_nlp-1.4.1.8/jac_nlp/tfm_ner/entity_utils.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/tfm_ner/tests/fixtures/tfm_ner.jac` & `jac_nlp-1.4.1.8/jac_nlp/tfm_ner/tests/fixtures/tfm_ner.jac`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/tfm_ner/tests/test_tfm_ner.py` & `jac_nlp-1.4.1.8/jac_nlp/tfm_ner/tests/test_tfm_ner.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/tfm_ner/tfm_ner.py` & `jac_nlp-1.4.1.8/jac_nlp/tfm_ner/tfm_ner.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/tfm_ner/train.py` & `jac_nlp-1.4.1.8/jac_nlp/tfm_ner/train.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/tfm_ner/utils/data_tokens.py` & `jac_nlp-1.4.1.8/jac_nlp/tfm_ner/utils/data_tokens.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/topic_ext/action_utils.py` & `jac_nlp-1.4.1.8/jac_nlp/topic_ext/action_utils.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/topic_ext/topic_ext.py` & `jac_nlp-1.4.1.8/jac_nlp/topic_ext/topic_ext.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/use_enc/tests/fixtures/use_enc.jac` & `jac_nlp-1.4.1.8/jac_nlp/use_enc/tests/fixtures/use_enc.jac`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/use_enc/tests/test_use_enc.py` & `jac_nlp-1.4.1.8/jac_nlp/use_enc/tests/test_use_enc.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/use_enc/use_enc.py` & `jac_nlp-1.4.1.8/jac_nlp/use_enc/use_enc.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/use_qa/tests/fixtures/use_qa.jac` & `jac_nlp-1.4.1.8/jac_nlp/use_qa/tests/fixtures/use_qa.jac`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/use_qa/tests/test_use_qa.py` & `jac_nlp-1.4.1.8/jac_nlp/use_qa/tests/test_use_qa.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/use_qa/use_qa.py` & `jac_nlp-1.4.1.8/jac_nlp/use_qa/use_qa.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp/zs_classifier/zs_classifier.py` & `jac_nlp-1.4.1.8/jac_nlp/zs_classifier/zs_classifier.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp.egg-info/PKG-INFO` & `jac_nlp-1.4.1.8/jac_nlp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jac-nlp
-Version: 1.4.1.7
+Version: 1.4.1.8
 Home-page: https://github.com/Jaseci-Labs/jaseci
 Author: Jason Mars
 Author-email: jason@jaseci.org
 Provides-Extra: all
 Provides-Extra: bart_sum
 Provides-Extra: cl_summer
 Provides-Extra: ent_ext
```

### Comparing `jac_nlp-1.4.1.7/jac_nlp.egg-info/SOURCES.txt` & `jac_nlp-1.4.1.8/jac_nlp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.1.7/jac_nlp.egg-info/requires.txt` & `jac_nlp-1.4.1.8/jac_nlp.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-jaseci==1.4.1.7
+jaseci==1.4.1.8
 pytest<7.1,>=7.0.1
 pytest-order<1.1,>=1.0.1
 
 [all]
 transformers>=4.25.1
 beautifulsoup4<4.13.0,>=4.12.2
 torch<2.0.0,>=1.10.2
@@ -13,16 +13,16 @@
 transformers==4.25.1
 sentencepiece==0.1.95
 spacy==3.3.0
 datasets==2.8.0
 evaluate<0.3,>=0.2.2
 seqeval<1.3,>=1.2.2
 tensorflow-hub<1.0.0,>=0.12.0
-tensorflow-text<3.0.0,>=2.7.3
-tensorflow<3.0.0,>=2.8.0
+tensorflow-text<2.9.0,>=2.7.3
+tensorflow<2.9.0,>=2.8.0
 torch
 numpy>=1.23.0
 scikit-learn>=1.2.0
 pandas==1.5.2
 sentence-transformers==2.2.2
 scikit-learn>=0.24.2
 openai>=0.26.5
@@ -123,16 +123,16 @@
 pandas==1.5.2
 transformers==4.25.1
 sentencepiece==0.1.95
 sentence-transformers==2.2.2
 
 [use_enc]
 tensorflow-hub<1.0.0,>=0.12.0
-tensorflow-text<3.0.0,>=2.7.3
-tensorflow<3.0.0,>=2.8.0
+tensorflow-text<2.9.0,>=2.7.3
+tensorflow<2.9.0,>=2.8.0
 
 [use_qa]
-tensorflow<3.0.0,>=2.8.0
 tensorflow-hub<1.0.0,>=0.12.0
-tensorflow-text<3.0.0,>=2.7.3
+tensorflow-text<2.9.0,>=2.7.3
+tensorflow<2.9.0,>=2.8.0
 
 [zs_classifier]
```

### Comparing `jac_nlp-1.4.1.7/setup.py` & `jac_nlp-1.4.1.8/setup.py`

 * *Files identical despite different names*

