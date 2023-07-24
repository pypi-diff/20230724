# Comparing `tmp/alpaca_eval-0.2.4.tar.gz` & `tmp/alpaca_eval-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpaca_eval-0.2.4.tar", last modified: Fri Jul 21 15:23:03 2023, max compression
+gzip compressed data, was "alpaca_eval-0.2.5.tar", last modified: Mon Jul 24 17:25:59 2023, max compression
```

## Comparing `alpaca_eval-0.2.4.tar` & `alpaca_eval-0.2.5.tar`

### file list

```diff
@@ -1,232 +1,233 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.139952 alpaca_eval-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-07-21 15:22:38.000000 alpaca_eval-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-21 15:22:38.000000 alpaca_eval-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    67440 2023-07-21 15:23:03.139952 alpaca_eval-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    66618 2023-07-21 15:22:38.000000 alpaca_eval-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.115952 alpaca_eval-0.2.4/example/
--rw-r--r--   0 runner    (1001) docker     (123)   500735 2023-07-21 15:22:38.000000 alpaca_eval-0.2.4/example/outputs.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 15:23:03.139952 alpaca_eval-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.091951 alpaca_eval-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.119952 alpaca_eval-0.2.4/src/alpaca_eval/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-21 15:22:48.000000 alpaca_eval-0.2.4/src/alpaca_eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21377 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/analyze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.123952 alpaca_eval-0.2.4/src/alpaca_eval/annotators/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/annotators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26474 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/annotators/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16494 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/annotators/pairwise_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/completion_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.127952 alpaca_eval-0.2.4/src/alpaca_eval/decoders/
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/decoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/decoders/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/decoders/cohere.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/decoders/huggingface_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/decoders/huggingface_local.py
--rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/decoders/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/decoders/replicate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.127952 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.127952 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.127952 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/alpaca_eval_fn.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.127952 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.127952 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.127952 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/aviary_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/aviary_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.127952 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/chatgpt/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/chatgpt/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.127952 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/chatgpt_fn/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/chatgpt_fn/basic_function_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/chatgpt_fn/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.127952 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/claude/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/claude/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.127952 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/claude_2/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/claude_2/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/claude_ranking/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/claude_ranking/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/cohere/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/cohere/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/guanaco_33b/
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/guanaco_33b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/lmsys_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/lmsys_gpt4/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/test/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/test/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/text_davinci_003/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/text_davinci_003/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.099952 alpaca_eval-0.2.4/src/alpaca_eval/leaderboards/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/leaderboards/data_AlpacaEval/
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/leaderboards/data_AlpacaEval/chatgpt_fn_leaderboard.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/leaderboards/data_AlpacaEval/text_davinci_003_leaderboard.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/leaderboards/evaluators/
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv
--rw-r--r--   0 runner    (1001) docker     (123)    21848 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.111952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/airoboros-33b/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/airoboros-33b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/airoboros-33b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/airoboros-65b/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/airoboros-65b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/alpaca-7b/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/alpaca-7b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/alpaca-7b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/baichuan-13b-chat/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/baichuan-13b-chat/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/baichuan-13b-chat/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/baize-v2-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/baize-v2-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/baize-v2-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/baize-v2-7b/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/baize-v2-7b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/chatglm2-6b/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/chatglm2-6b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/chatglm2-6b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/chatgpt/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/chatgpt/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.135952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/claude/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/claude/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/claude/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.135952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/claude-2/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/claude-2/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.135952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/cohere/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/cohere/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/cohere/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.135952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/cohere-chat/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/cohere-chat/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.135952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/falcon-40b-instruct/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/falcon-40b-instruct/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.135952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/falcon-7b-instruct/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/falcon-7b-instruct/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.135952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/gpt4/chatml_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.135952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/guanaco-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/guanaco-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.135952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/guanaco-33b/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/guanaco-33b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.135952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/guanaco-65b/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/guanaco-65b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.135952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/guanaco-7b/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/guanaco-7b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/guanaco-7b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.135952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/llama-2-13b-chat-hf/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/llama-2-13b-chat-hf/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.135952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/llama-2-70b-chat-hf/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/llama-2-70b-chat-hf/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.135952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.135952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate-noprompt/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate-noprompt/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate-noprompt/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.135952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/llama-2-7b-chat-hf/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/llama-2-7b-chat-hf/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/llama-2-7b-chat-hf/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.135952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/minotaur-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/minotaur-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/minotaur-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.135952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/nous-hermes-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/nous-hermes-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/nous-hermes-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.135952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.135952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/oasst-sft-llama-33b/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/oasst-sft-llama-33b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/oasst-sft-llama-33b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.135952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.139952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/openchat-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/openchat-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/openchat-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.139952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/openchat-v2-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/openchat-v2-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.139952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/openchat-v2-w-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/openchat-v2-w-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.139952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/openchat8192-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/openchat8192-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.139952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/opencoderplus-15b/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/opencoderplus-15b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.139952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/pythia-12b-mix-sft/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/pythia-12b-mix-sft/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.139952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/text_davinci_001/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/text_davinci_001/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.139952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/text_davinci_003/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/text_davinci_003/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/text_davinci_003/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.139952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/ultralm-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/ultralm-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/ultralm-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.139952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/vicuna-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/vicuna-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.139952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/vicuna-13b-v1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/vicuna-13b-v1.3/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.139952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/vicuna-33b-v1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/vicuna-33b-v1.3/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.139952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/vicuna-7b/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/vicuna-7b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/vicuna-7b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.139952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/vicuna-7b-v1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/vicuna-7b-v1.3/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.139952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/wizardlm-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/wizardlm-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/wizardlm-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.139952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/wizardlm-13b-v1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/wizardlm-13b-v1.1/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20680 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.123952 alpaca_eval-0.2.4/src/alpaca_eval.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    67440 2023-07-21 15:23:03.000000 alpaca_eval-0.2.4/src/alpaca_eval.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-07-21 15:23:03.000000 alpaca_eval-0.2.4/src/alpaca_eval.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 15:23:03.000000 alpaca_eval-0.2.4/src/alpaca_eval.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-21 15:23:03.000000 alpaca_eval-0.2.4/src/alpaca_eval.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-21 15:23:03.000000 alpaca_eval-0.2.4/src/alpaca_eval.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-21 15:23:03.000000 alpaca_eval-0.2.4/src/alpaca_eval.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.139952 alpaca_eval-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/tests/test_analyze.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/tests/test_decoders_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/tests/test_pairwise_evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.397300 alpaca_eval-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    67440 2023-07-24 17:25:59.397300 alpaca_eval-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    66618 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.377300 alpaca_eval-0.2.5/example/
+-rw-r--r--   0 runner    (1001) docker     (123)   500735 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/example/outputs.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 17:25:59.397300 alpaca_eval-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.373300 alpaca_eval-0.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.381300 alpaca_eval-0.2.5/src/alpaca_eval/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-24 17:25:43.000000 alpaca_eval-0.2.5/src/alpaca_eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21377 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/analyze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.381300 alpaca_eval-0.2.5/src/alpaca_eval/annotators/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/annotators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27986 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/annotators/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15833 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/annotators/pairwise_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/completion_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.381300 alpaca_eval-0.2.5/src/alpaca_eval/decoders/
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/decoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/decoders/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/decoders/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/decoders/huggingface_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/decoders/huggingface_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/decoders/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/decoders/replicate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.381300 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.385300 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.385300 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/alpaca_eval_fn.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.385300 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.385300 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.385300 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/aviary_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/aviary_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.385300 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/chatgpt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/chatgpt/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.385300 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/chatgpt_fn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/chatgpt_fn/basic_function_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/chatgpt_fn/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.385300 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/claude/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/claude/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.385300 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/claude_2/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/claude_2/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.385300 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/claude_ranking/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/claude_ranking/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.385300 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/cohere/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/cohere/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.389300 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.389300 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/guanaco_33b/
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/guanaco_33b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.389300 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.389300 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.389300 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/lmsys_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/lmsys_gpt4/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.389300 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.389300 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/test/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.389300 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/text_davinci_003/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/text_davinci_003/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.373300 alpaca_eval-0.2.5/src/alpaca_eval/leaderboards/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.389300 alpaca_eval-0.2.5/src/alpaca_eval/leaderboards/data_AlpacaEval/
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/leaderboards/data_AlpacaEval/chatgpt_fn_leaderboard.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/leaderboards/data_AlpacaEval/text_davinci_003_leaderboard.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.389300 alpaca_eval-0.2.5/src/alpaca_eval/leaderboards/evaluators/
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21848 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.377300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.389300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/airoboros-33b/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/airoboros-33b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/airoboros-33b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.389300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/airoboros-65b/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/airoboros-65b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.389300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/alpaca-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/alpaca-7b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/alpaca-7b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.389300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.389300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.389300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/baichuan-13b-chat/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/baichuan-13b-chat/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/baichuan-13b-chat/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.389300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/baize-v2-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/baize-v2-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/baize-v2-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.389300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/baize-v2-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/baize-v2-7b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.389300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/chatglm2-6b/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/chatglm2-6b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/chatglm2-6b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.393300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/chatgpt/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/chatgpt/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.393300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/claude/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/claude/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/claude/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.393300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/claude-2/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/claude-2/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.393300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/cohere/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/cohere/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/cohere/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.393300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/cohere-chat/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/cohere-chat/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.393300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/falcon-40b-instruct/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/falcon-40b-instruct/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.393300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/falcon-7b-instruct/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/falcon-7b-instruct/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.393300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/gpt4/chatml_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.393300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/guanaco-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/guanaco-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.393300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/guanaco-33b/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/guanaco-33b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.393300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/guanaco-65b/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/guanaco-65b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.393300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/guanaco-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/guanaco-7b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/guanaco-7b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.393300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/llama-2-13b-chat-hf/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/llama-2-13b-chat-hf/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.393300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/llama-2-70b-chat-hf/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/llama-2-70b-chat-hf/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.393300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.393300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate-noprompt/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate-noprompt/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate-noprompt/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.393300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/llama-2-7b-chat-hf/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/llama-2-7b-chat-hf/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/llama-2-7b-chat-hf/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.393300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/minotaur-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/minotaur-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/minotaur-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.393300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/nous-hermes-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/nous-hermes-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/nous-hermes-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.393300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.393300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/oasst-sft-llama-33b/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/oasst-sft-llama-33b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/oasst-sft-llama-33b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.397300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.397300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/openchat-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/openchat-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/openchat-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.397300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/openchat-v2-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/openchat-v2-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.397300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/openchat-v2-w-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/openchat-v2-w-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.397300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/openchat8192-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/openchat8192-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.397300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/opencoderplus-15b/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/opencoderplus-15b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.397300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/pythia-12b-mix-sft/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/pythia-12b-mix-sft/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.397300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/text_davinci_001/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/text_davinci_001/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.397300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/text_davinci_003/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/text_davinci_003/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/text_davinci_003/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.397300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/ultralm-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/ultralm-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/ultralm-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.397300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/vicuna-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/vicuna-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.397300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/vicuna-13b-v1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/vicuna-13b-v1.3/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.397300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/vicuna-33b-v1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/vicuna-33b-v1.3/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.397300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/vicuna-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/vicuna-7b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/vicuna-7b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.397300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/vicuna-7b-v1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/vicuna-7b-v1.3/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.397300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/wizardlm-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/wizardlm-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/wizardlm-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.397300 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/wizardlm-13b-v1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/models_configs/wizardlm-13b-v1.1/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20680 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14843 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/src/alpaca_eval/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.381300 alpaca_eval-0.2.5/src/alpaca_eval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    67440 2023-07-24 17:25:59.000000 alpaca_eval-0.2.5/src/alpaca_eval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8442 2023-07-24 17:25:59.000000 alpaca_eval-0.2.5/src/alpaca_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 17:25:59.000000 alpaca_eval-0.2.5/src/alpaca_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-24 17:25:59.000000 alpaca_eval-0.2.5/src/alpaca_eval.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-24 17:25:59.000000 alpaca_eval-0.2.5/src/alpaca_eval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-24 17:25:59.000000 alpaca_eval-0.2.5/src/alpaca_eval.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:25:59.397300 alpaca_eval-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/tests/test_analyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/tests/test_decoders_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-07-24 17:25:30.000000 alpaca_eval-0.2.5/tests/test_pairwise_evaluator.py
```

### Comparing `alpaca_eval-0.2.4/LICENSE` & `alpaca_eval-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/PKG-INFO` & `alpaca_eval-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaca_eval
-Version: 0.2.4
+Version: 0.2.5
 Summary: AlpacaEval : An Automatic Evaluator of Instruction-following Models
 Author: The Alpaca Team
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: alpaca_eval Version: 0.2.4 Summary: AlpacaEval : An
+Metadata-Version: 2.1 Name: alpaca_eval Version: 0.2.5 Summary: AlpacaEval : An
 Automatic Evaluator of Instruction-following Models Author: The Alpaca Team
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Education Classifier: Intended Audience :: Science/Research Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: Topic :: Scientific/Engineering :: Artificial
```

### Comparing `alpaca_eval-0.2.4/README.md` & `alpaca_eval-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/example/outputs.json` & `alpaca_eval-0.2.5/example/outputs.json`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/setup.py` & `alpaca_eval-0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/analyze.py` & `alpaca_eval-0.2.5/src/alpaca_eval/analyze.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/annotators/base.py` & `alpaca_eval-0.2.5/src/alpaca_eval/annotators/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from functools import partial
 from pathlib import Path
 from typing import Any, Callable, Optional, Sequence, Type, Union
 
 import numpy as np
 import pandas as pd
 
-from .. import completion_parsers, constants, utils
+from .. import completion_parsers, constants, processors, utils
 from ..decoders import get_fn_completions
 
 CURRENT_DIR = Path(__file__).parent
 logging.getLogger().setLevel(logging.INFO)
 
 __all__ = ["BaseAnnotator", "BaseAnnotatorJSON", "SingleAnnotator"]
 
@@ -131,15 +131,15 @@
     ### Public methods ###
     @property
     def annotator_name(self) -> str:
         return Path(self.annotators_config).parent.name
 
     def __call__(
         self,
-        to_annotate: Union[Sequence[dict[str, Any]], pd.DataFrame],
+        to_annotate: utils.AnyData,
         **decoding_kwargs,
     ) -> list[dict[str, Any]]:
         """Main function for annotating.
 
         Parameters
         ----------
         to_annotate : list of dict or dataframe
@@ -200,15 +200,15 @@
         else:
             for c in missing_primary_keys:
                 df[c] = None
 
     def _preprocess(self, to_annotate: utils.AnyData) -> pd.DataFrame:
         """Preprocess the examples to annotate. In particular takes care of filtering unnecessary examples."""
 
-        df_to_annotate = utils.convert_to_dataframe(to_annotate).copy()
+        df_to_annotate = utils.convert_to_dataframe(to_annotate)
         self._add_missing_primary_keys_(df_to_annotate)
 
         for c in self.other_keys_to_keep + [self.annotation_key]:
             if c in df_to_annotate.columns:
                 logging.warning(f"""{c} column is already in the dataframe. We will overwrite it.""")
                 df_to_annotate[c] = None
 
@@ -251,15 +251,15 @@
             df_annotated = self._merge_annotations(df_annotated, curr_annotated)
 
         return df_annotated
 
     def _postprocess_and_store_(
         self,
         df_annotated: pd.DataFrame,
-        to_annotate: Union[Sequence[dict[str, Any]], pd.DataFrame],
+        to_annotate: utils.AnyData,
     ) -> list[dict[str, Any]]:
         """Convert the dataframe into a list of dictionaries to be returned, and store current anntations."""
 
         df_to_annotate = utils.convert_to_dataframe(to_annotate)
         self._add_missing_primary_keys_(df_to_annotate)
 
         # select available annotations
@@ -463,14 +463,22 @@
         to this directory.
 
     annotation_column : str, optional
         Name of the annotation column in the output dataframe.
 
     is_store_raw_completions : bool, optional
         Whether to store raw completions at `"raw_completion"` column in the output dataframe.
+
+    processors_to_kwargs : Sequence[dict(str, dict)], optional
+        A dictionary of BaseProcessor objects to apply for preprocessing the  dataframe before making the prompts and
+        prostprocessing after anntoations. The key should be the names of the BaseProcessor objectsto use in
+        `processors.py` the values are the kwargs for the constructor of the Processor. Order matters.
+
+    is_add_default_processors : bool, optional
+        Whether to add the default processors to the list of processors.
     """
 
     def __init__(
         self,
         prompt_template: utils.AnyPath,
         fn_completion_parser: Optional[Union[Callable, str]] = "regex_parser",
         completion_parser_kwargs: Optional[dict[str, Any]] = None,
@@ -478,14 +486,16 @@
         completions_kwargs: Optional[dict[str, Any]] = None,
         is_shuffle: bool = True,
         seed: Optional[int] = 123,
         batch_size: int = 1,
         base_dir: utils.AnyPath = constants.EVALUATORS_CONFIG_DIR,
         annotation_column: str = "annotation",
         is_store_raw_completions: bool = False,
+        processors_to_kwargs: Optional[dict[str, dict]] = None,
+        is_add_default_processors: bool = True,
     ):
         self.base_dir = Path(base_dir)
         self.prompt_template = self._get_prompt_template(prompt_template)
 
         if fn_completion_parser is None:
             fn_completion_parser = lambda x: [x]
         elif isinstance(fn_completion_parser, str):
@@ -497,14 +507,27 @@
         self.completions_kwargs = completions_kwargs or {}
         self.seed = seed
         self.is_shuffle = is_shuffle
         self.batch_size = batch_size
         self.annotation_column = annotation_column
         self.completion_column = "raw_completion" if is_store_raw_completions else None
 
+        self.is_add_default_processors = is_add_default_processors
+        self.processors = []
+        processors_to_kwargs = processors_to_kwargs or {}
+        if batch_size > 1 and self.is_add_default_processors:
+            processors_to_kwargs["PaddingForBatchesProcessor"] = {
+                "batch_size": batch_size,
+                "padding_example": DUMMY_EXAMPLE,
+            }
+        for processor, processor_kwargs in processors_to_kwargs.items():
+            processor_kwargs["seed"] = self.seed
+            Processor = self._search_processor(processor)
+            self.processors += [Processor(**processor_kwargs)]
+
     ### Public methods ###
     def __call__(self, df_to_annotate: pd.DataFrame, **decoding_kwargs) -> pd.DataFrame:
         """Annotates the given examples.
 
         Parameters
         ----------
         df_to_annotate : pd.DataFrame
@@ -546,14 +569,18 @@
     ######################
 
     ### Private methods ###
     def _search_fn_completion_parser(self, name: str) -> Callable:
         """Search for a completion parser by name."""
         return getattr(completion_parsers, name)
 
+    def _search_processor(self, name: str) -> Type["processors.BaseProcessor"]:
+        """Search for a Processor class by name."""
+        return getattr(processors, name)
+
     def _get_prompt_template(self, prompt_template: utils.AnyPath):
         return utils.read_or_return(self.base_dir / prompt_template)
 
     def _make_prompts(
         self, df_to_annotate: pd.DataFrame, prompt_template: Optional[str] = None
     ) -> tuple[list[str], pd.DataFrame]:
         """Make all the prompts for the given examples.
@@ -577,14 +604,17 @@
         if prompt_template is None:
             prompt_template = self.prompt_template
         return utils.make_prompts(df=df_to_annotate, template=prompt_template, batch_size=self.batch_size)
 
     def _preprocess(self, df_to_annotate: pd.DataFrame) -> pd.DataFrame:
         """Preprocess the examples before annotating. In particular, takes care of all the randomization."""
 
+        for processor in self.processors:
+            df_to_annotate = processor.preprocess(df_to_annotate)
+
         if self.is_shuffle:
             df_to_annotate = df_to_annotate.sample(frac=1, random_state=self.seed)
 
         return df_to_annotate
 
     def _parse_completions(self, completions: list[str]) -> tuple[list[Any], list[Any]]:
         """Converts the completions into annotations."""
@@ -609,21 +639,21 @@
             all_annotations += batch_annotations
             all_completions += [completion] * self.batch_size
         return all_annotations, all_completions
 
     def _postprocess(self, df_annotated: pd.DataFrame) -> pd.DataFrame:
         """Postprocess the annotated examples."""
 
-        # remove padding examples when using batch_size > 1
-        df_annotated = df_annotated.query("is_padding == False").drop(columns=["is_padding"])
-
         arr_is_na = df_annotated[self.annotation_column].isna()
         if arr_is_na.any():
             logging.warning(
                 f"{arr_is_na.sum().item()} samples had no auto annotation. We are filtering them for now. "
                 f"If you are using chain of thought it might be that max_tokens limit is too low. "
             )
             df_annotated = df_annotated[~arr_is_na]
 
+        for processor in self.processors[::-1]:  # postprocess in reverted order => no interactions between processors
+            df_annotated = processor.postprocess(df_annotated)
+
         return df_annotated
 
     #######################
```

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/annotators/pairwise_evaluator.py` & `alpaca_eval-0.2.5/src/alpaca_eval/annotators/pairwise_evaluator.py`

 * *Files 12% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         self.input_keys = list(input_keys)
         self.output_keys = list(output_keys)
         super().__init__(*args, **kwargs, primary_keys=self.input_keys + self.output_keys)
         self.p_label_flip = p_label_flip
 
     @property
     def SingleAnnotator(self) -> Type["SingleAnnotator"]:
-        return partial(SinglePairwiseAnnotator, random_seed_column=self.random_seed_key)
+        return SinglePairwiseAnnotator
 
     @property
     def annotation_key(self) -> str:
         return "preference"
 
     @property
     def random_seed_key(self) -> list[str]:
@@ -336,46 +336,36 @@
         The column to use to seed the randomization of output_1, output_2.
     """
     )
 
     def __init__(
         self,
         *args,
-        is_randomize_output_order: bool = True,
         annotation_column: str = "preference",
         random_seed_column: Sequence[str] = ("instruction",),
+        processors_to_kwargs: Optional[dict[str, dict]] = None,
+        is_randomize_output_order: bool = True,
         **kwargs,
     ):
-        super().__init__(*args, annotation_column=annotation_column, **kwargs)
-        self.is_randomize_output_order = is_randomize_output_order
-        self.random_seed_column = list(random_seed_column)
-
-    def _preprocess(self, df_to_annotate: pd.DataFrame) -> pd.DataFrame:
-        if self.is_randomize_output_order:
-            # randomize order of output_1, output_2 base on inputs
-            df_to_annotate["is_switched_outputs"] = df_to_annotate.apply(
-                # we add "is_switched_outputs" at the beginning to not use the same seed for all tasks
-                lambda x: utils.random_seeded_choice(
-                    seed="is_switched_outputs" + "".join(x[self.random_seed_column]) + str(self.seed),
-                    choices=[False, True],
-                ),
-                axis=1,
+        processors_to_kwargs = processors_to_kwargs or {}
+        if is_randomize_output_order:
+            # swith output columns by default
+            processors_to_kwargs["RandomSwitchTwoColumnsProcessor"] = dict(
+                two_columns_to_switch=["output_1", "output_2"],
+                replace_if_switch_kwargs={"preference": {1: 2, 2: 1}},
+                random_seed_columns=random_seed_column,
+                _switch_column="is_switched_outputs",  # backward compatibility
             )
-            df_to_annotate = utils.shuffle_pairwise_preferences(df_to_annotate, df_to_annotate["is_switched_outputs"])
 
-        df_to_annotate = super()._preprocess(df_to_annotate)
-
-        return df_to_annotate
+        super().__init__(
+            *args, annotation_column=annotation_column, processors_to_kwargs=processors_to_kwargs, **kwargs
+        )
+        self.random_seed_column = list(random_seed_column)
 
     def _postprocess(self, df_annotated: pd.DataFrame) -> pd.DataFrame:
         df_annotated = super()._postprocess(df_annotated)
 
         all_values = df_annotated[self.annotation_column]
         all_values = all_values[~all_values.isna()]
         assert set(all_values.unique().tolist()) <= {0, 1, 2, np.nan}
 
-        if self.is_randomize_output_order:
-            # unshuffles output 1 and output 2. For binary preference, unshuffling is equivalent to reshuffling
-            df_annotated = utils.shuffle_pairwise_preferences(df_annotated, df_annotated["is_switched_outputs"])
-            df_annotated = df_annotated.drop(columns=["is_switched_outputs"])
-
         return df_annotated
```

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/completion_parsers.py` & `alpaca_eval-0.2.5/src/alpaca_eval/completion_parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
         return [rank]
     except Exception as e:
         logging.error(f"{e}\nContent: {completion}\n" "You must manually fix the score pair.")
         return [np.nan]
 
 
 def json_parser(completion: str, annotation_key: str) -> list[Any]:
-    """Parse the completion by reading it as a JSON and selecting "annotation_key".
+    r"""Parse the completion by reading it as a JSON and selecting "annotation_key".
 
     Examples
     --------
     >>> completion = '{"short_explanation": "that is why", "is_incorporated": true}'
     >>> json_parser(completion, "is_incorporated")
     [True]
     >>> completion = '[{"short_explanation": "that is why", "is_incorporated": true}, {"is_incorporated": false}]'
```

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/constants.py` & `alpaca_eval-0.2.5/src/alpaca_eval/constants.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/decoders/__init__.py` & `alpaca_eval-0.2.5/src/alpaca_eval/decoders/__init__.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/decoders/anthropic.py` & `alpaca_eval-0.2.5/src/alpaca_eval/decoders/anthropic.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/decoders/cohere.py` & `alpaca_eval-0.2.5/src/alpaca_eval/decoders/cohere.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/decoders/huggingface_api.py` & `alpaca_eval-0.2.5/src/alpaca_eval/decoders/huggingface_api.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/decoders/huggingface_local.py` & `alpaca_eval-0.2.5/src/alpaca_eval/decoders/huggingface_local.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/decoders/openai.py` & `alpaca_eval-0.2.5/src/alpaca_eval/decoders/openai.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/decoders/replicate.py` & `alpaca_eval-0.2.5/src/alpaca_eval/decoders/replicate.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/README.md` & `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/README.md`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt` & `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/alpaca_eval_fn.txt` & `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/alpaca_eval_fn.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/configs.yaml` & `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt` & `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt` & `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt` & `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt` & `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt` & `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt` & `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt` & `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt` & `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml` & `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt` & `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt` & `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt` & `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt` & `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt` & `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt` & `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt` & `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/chatgpt_fn/basic_function_prompt.txt` & `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/chatgpt_fn/basic_function_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/chatgpt_fn/configs.yaml` & `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/chatgpt_fn/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt` & `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt` & `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt` & `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt` & `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt` & `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt` & `alpaca_eval-0.2.5/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv` & `alpaca_eval-0.2.5/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/leaderboards/data_AlpacaEval/chatgpt_fn_leaderboard.csv` & `alpaca_eval-0.2.5/src/alpaca_eval/leaderboards/data_AlpacaEval/chatgpt_fn_leaderboard.csv`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv` & `alpaca_eval-0.2.5/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv` & `alpaca_eval-0.2.5/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/main.py` & `alpaca_eval-0.2.5/src/alpaca_eval/main.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/metrics.py` & `alpaca_eval-0.2.5/src/alpaca_eval/metrics.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/models_configs/llama-2-7b-chat-hf/prompt.txt` & `alpaca_eval-0.2.5/src/alpaca_eval/models_configs/llama-2-7b-chat-hf/prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/plotting.py` & `alpaca_eval-0.2.5/src/alpaca_eval/plotting.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval/utils.py` & `alpaca_eval-0.2.5/src/alpaca_eval/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,37 +44,14 @@
 
 
 def random_seeded_choice(seed: Union[int, str, float], choices, **kwargs):
     """Random choice with a (potentially string) seed."""
     return random.Random(seed).choices(choices, k=1, **kwargs)[0]
 
 
-def shuffle_pairwise_preferences(df: pd.DataFrame, arr_is_shuffle: Sequence[int]) -> pd.DataFrame:
-    """Shuffle the outputs of a pairwise preference dataframe.
-
-    Examples
-    --------
-    >>> df = pd.DataFrame([dict(instruction='2+2', output_1='3', output_2='4', preference=2),
-    ...                    dict(instruction='2+3', output_1='5', output_2='4', preference=1)])
-    >>> print(shuffle_pairwise_preferences(df, [True, False]))
-        instruction output_1 output_2  preference
-    0         2+2        4        3           1
-    1         2+3        5        4           1
-    """
-    col_1 = df["output_1"].copy()
-    col_2 = df["output_2"].copy()
-    df["output_1"] = np.where(arr_is_shuffle, col_2, col_1)
-    df["output_2"] = np.where(arr_is_shuffle, col_1, col_2)
-
-    if "preference" in df.columns:
-        df["preference"] = np.where(arr_is_shuffle, 3 - df["preference"], df["preference"])
-
-    return df
-
-
 def is_derangement(arr1, arr2):
     """Whether 2 arrays are derangements of one another"""
     return all([a != b for a, b in zip(arr1, arr2)])
 
 
 def random_derangement(arr, max_loop=10, seed=None):
     """
@@ -110,68 +87,64 @@
             first_match = match
             first_key = key
 
     return first_match, first_key
 
 
 def make_prompts(
-    df: pd.DataFrame, template: str, batch_size: int = 1, padding_example=DUMMY_EXAMPLE
+    df: pd.DataFrame,
+    template: str,
+    batch_size: int = 1,
 ) -> tuple[list[str], pd.DataFrame]:
-    """Helper function to make batch prompts for a single template.
+    r"""Helper function to make batch prompts for a single template.
 
     Parameters
     ----------
     df : pd.DataFrame
         Examples to annotate
 
     template : str
         Template for the prompt. Should have batch_size number of placeholder {key} where key is a column in df.
 
     batch_size : int
         Number of examples to batch in a single prompt.
 
-    padding_example : dict
-        Padding example to use if len(df) not divisible by batch_size.
-
     Returns
     -------
     prompts : list[str]
         List of formatted prompts.
 
     df_out : pd.DataFrame
         All examples. Will be df with potential padding examples.
 
     Example
     -------
     >>> import pandas as pd
-    >>> from alpaca_eval.utils import make_prompts
-    >>> df = pd.DataFrame({"instruction": ["solve", "write backwards", "other 1"],
-    ...                    "input": ["1+1", "'abc'", ""]})
-    >>> make_prompts(df, template="first: {instruction} {input}, second: {instruction} {input}",
-    ...              batch_size=2, padding_example=dict(instruction="pad", input="pad_in"))[0]
-    ["first: solve 1+1, second: write backwards 'abc'",
-     'first: other 1 , second: pad pad_in']
+    >>> df = pd.DataFrame({"instruction": ["solve", "write backwards", "other 1", "pad"],
+    ...                    "input": ["1+1", "'abc'", "", "pad_in"]})
+    >>> make_prompts(df, template="first: {instruction} {input}, second: {instruction} {input}", batch_size=2)[0]
+    ["first: solve 1+1, second: write backwards 'abc'", 'first: other 1 , second: pad pad_in']
     """
 
     if df.empty:
         return [], df
 
     text_to_format = re.findall("{([^ \s]+?)}", template)
     n_occurrences = Counter(text_to_format)
 
     if not all([n == batch_size for n in n_occurrences.values()]):
         raise ValueError(f"All placeholders should be repeated batch_size={batch_size} times but {n_occurrences}.")
 
-    # padding if you don't have enough examples
-    n_to_pad = (batch_size - len(df)) % batch_size
-    padding = pd.DataFrame([padding_example] * n_to_pad)
-    padding["is_padding"] = True
-    df_out = pd.concat([df, padding], axis=0, ignore_index=True)
-    df_out["is_padding"] = df_out["is_padding"].fillna(False)
+    if len(df) % batch_size > 0:
+        raise ValueError(
+            f"The number of rows should be dividable by the batch_size={batch_size} but got {len(df)}."
+            "You should use PaddingForBatchesProcessor"
+        )
 
+    df_out = df.copy()
     prompts = []
     # ugly for loops, not trivial to vectorize because of the batching
     for i in range(0, len(df_out), batch_size):
         current_prompt = copy.deepcopy(template)
         for j in range(batch_size):
             for to_format in n_occurrences.keys():
                 # replace only first occurrence (that's why we don't use .format)
@@ -236,15 +209,15 @@
 
     return preferences
 
 
 def convert_to_dataframe(data: AnyData) -> pd.DataFrame:
     """Convert input that AlpacaEval accepts into a dataframe."""
     if isinstance(data, pd.DataFrame):
-        return data
+        return data.copy()
     elif isinstance(data, datasets.Dataset):
         return data.data.to_pandas()
     elif isinstance(data, list):
         return pd.DataFrame.from_records(data)
     else:
         # try
         return pd.DataFrame(data)
```

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval.egg-info/PKG-INFO` & `alpaca_eval-0.2.5/src/alpaca_eval.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaca-eval
-Version: 0.2.4
+Version: 0.2.5
 Summary: AlpacaEval : An Automatic Evaluator of Instruction-following Models
 Author: The Alpaca Team
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: alpaca-eval Version: 0.2.4 Summary: AlpacaEval : An
+Metadata-Version: 2.1 Name: alpaca-eval Version: 0.2.5 Summary: AlpacaEval : An
 Automatic Evaluator of Instruction-following Models Author: The Alpaca Team
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Education Classifier: Intended Audience :: Science/Research Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: Topic :: Scientific/Engineering :: Artificial
```

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval.egg-info/SOURCES.txt` & `alpaca_eval-0.2.5/src/alpaca_eval.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 src/alpaca_eval/__init__.py
 src/alpaca_eval/analyze.py
 src/alpaca_eval/completion_parsers.py
 src/alpaca_eval/constants.py
 src/alpaca_eval/main.py
 src/alpaca_eval/metrics.py
 src/alpaca_eval/plotting.py
+src/alpaca_eval/processors.py
 src/alpaca_eval/types.py
 src/alpaca_eval/utils.py
 src/alpaca_eval.egg-info/PKG-INFO
 src/alpaca_eval.egg-info/SOURCES.txt
 src/alpaca_eval.egg-info/dependency_links.txt
 src/alpaca_eval.egg-info/entry_points.txt
 src/alpaca_eval.egg-info/requires.txt
```

### Comparing `alpaca_eval-0.2.4/src/alpaca_eval.egg-info/requires.txt` & `alpaca_eval-0.2.5/src/alpaca_eval.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/tests/test_analyze.py` & `alpaca_eval-0.2.5/tests/test_analyze.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/tests/test_decoders_unit.py` & `alpaca_eval-0.2.5/tests/test_decoders_unit.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/tests/test_main.py` & `alpaca_eval-0.2.5/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.4/tests/test_pairwise_evaluator.py` & `alpaca_eval-0.2.5/tests/test_pairwise_evaluator.py`

 * *Files identical despite different names*

