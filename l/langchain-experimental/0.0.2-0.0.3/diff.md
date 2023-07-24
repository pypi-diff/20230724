# Comparing `tmp/langchain_experimental-0.0.2.tar.gz` & `tmp/langchain_experimental-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_experimental-0.0.2.tar", max compression
+gzip compressed data, was "langchain_experimental-0.0.3.tar", max compression
```

## Comparing `langchain_experimental-0.0.2.tar` & `langchain_experimental-0.0.3.tar`

### file list

```diff
@@ -1,52 +1,57 @@
--rw-r--r--   0        0        0       93 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/README.md
--rw-r--r--   0        0        0        0 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/__init__.py
--rw-r--r--   0        0        0      188 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/autonomous_agents/__init__.py
--rw-r--r--   0        0        0        0 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/autonomous_agents/autogpt/__init__.py
--rw-r--r--   0        0        0     5244 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/autonomous_agents/autogpt/agent.py
--rw-r--r--   0        0        0     1072 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/autonomous_agents/autogpt/memory.py
--rw-r--r--   0        0        0     1750 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/autonomous_agents/autogpt/output_parser.py
--rw-r--r--   0        0        0     3274 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/autonomous_agents/autogpt/prompt.py
--rw-r--r--   0        0        0     6587 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/autonomous_agents/autogpt/prompt_generator.py
--rw-r--r--   0        0        0      514 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/autonomous_agents/baby_agi/__init__.py
--rw-r--r--   0        0        0     7469 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/autonomous_agents/baby_agi/baby_agi.py
--rw-r--r--   0        0        0     1284 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/autonomous_agents/baby_agi/task_creation.py
--rw-r--r--   0        0        0      835 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/autonomous_agents/baby_agi/task_execution.py
--rw-r--r--   0        0        0     1076 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/autonomous_agents/baby_agi/task_prioritization.py
--rw-r--r--   0        0        0      100 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/cpal/README.md
--rw-r--r--   0        0        0        0 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/cpal/__init__.py
--rw-r--r--   0        0        0     9041 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/cpal/base.py
--rw-r--r--   0        0        0      198 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/cpal/constants.py
--rw-r--r--   0        0        0     8322 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/cpal/models.py
--rw-r--r--   0        0        0        0 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/cpal/templates/__init__.py
--rw-r--r--   0        0        0        0 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/cpal/templates/univariate/__init__.py
--rw-r--r--   0        0        0     2175 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/cpal/templates/univariate/causal.py
--rw-r--r--   0        0        0      706 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/cpal/templates/univariate/intervention.py
--rw-r--r--   0        0        0     1750 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/cpal/templates/univariate/narrative.py
--rw-r--r--   0        0        0     4503 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/cpal/templates/univariate/query.py
--rw-r--r--   0        0        0      260 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/generative_agents/__init__.py
--rw-r--r--   0        0        0    10150 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/generative_agents/generative_agent.py
--rw-r--r--   0        0        0    12461 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/generative_agents/memory.py
--rw-r--r--   0        0        0      277 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/llms/__init__.py
--rw-r--r--   0        0        0     1838 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/llms/jsonformer_decoder.py
--rw-r--r--   0        0        0     4590 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/llms/llamaapi.py
--rw-r--r--   0        0        0     2027 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/llms/rellm_decoder.py
--rw-r--r--   0        0        0      277 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/pal_chain/__init__.py
--rw-r--r--   0        0        0    12482 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/pal_chain/base.py
--rw-r--r--   0        0        0     2645 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/pal_chain/colored_object_prompt.py
--rw-r--r--   0        0        0     4301 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/pal_chain/math_prompt.py
--rw-r--r--   0        0        0      363 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/plan_and_execute/__init__.py
--rw-r--r--   0        0        0     2078 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/plan_and_execute/agent_executor.py
--rw-r--r--   0        0        0        0 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/plan_and_execute/executors/__init__.py
--rw-r--r--   0        0        0     1464 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/plan_and_execute/executors/agent_executor.py
--rw-r--r--   0        0        0     1156 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/plan_and_execute/executors/base.py
--rw-r--r--   0        0        0        0 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/plan_and_execute/planners/__init__.py
--rw-r--r--   0        0        0     1362 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/plan_and_execute/planners/base.py
--rw-r--r--   0        0        0     1800 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/plan_and_execute/planners/chat_planner.py
--rw-r--r--   0        0        0     1149 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/plan_and_execute/schema.py
--rw-r--r--   0        0        0       87 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/prompts/__init__.py
--rw-r--r--   0        0        0     1873 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/prompts/load.py
--rw-r--r--   0        0        0      140 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/sql/__init__.py
--rw-r--r--   0        0        0    11411 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/sql/base.py
--rw-r--r--   0        0        0    14202 2023-07-23 16:24:29.834769 langchain_experimental-0.0.2/langchain_experimental/sql/prompt.py
--rw-r--r--   0        0        0     1904 2023-07-23 16:24:29.838769 langchain_experimental-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 langchain_experimental-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       93 2023-07-24 04:55:17.016086 langchain_experimental-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-24 04:55:17.016128 langchain_experimental-0.0.3/langchain_experimental/__init__.py
+-rw-r--r--   0        0        0      288 2023-07-24 16:56:12.537948 langchain_experimental-0.0.3/langchain_experimental/autonomous_agents/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-24 04:55:17.016833 langchain_experimental-0.0.3/langchain_experimental/autonomous_agents/autogpt/__init__.py
+-rw-r--r--   0        0        0     5244 2023-07-24 04:55:17.017074 langchain_experimental-0.0.3/langchain_experimental/autonomous_agents/autogpt/agent.py
+-rw-r--r--   0        0        0     1072 2023-07-24 04:55:17.017375 langchain_experimental-0.0.3/langchain_experimental/autonomous_agents/autogpt/memory.py
+-rw-r--r--   0        0        0     1750 2023-07-24 04:55:17.017438 langchain_experimental-0.0.3/langchain_experimental/autonomous_agents/autogpt/output_parser.py
+-rw-r--r--   0        0        0     3274 2023-07-24 04:55:17.017567 langchain_experimental-0.0.3/langchain_experimental/autonomous_agents/autogpt/prompt.py
+-rw-r--r--   0        0        0     6587 2023-07-24 04:55:17.017617 langchain_experimental-0.0.3/langchain_experimental/autonomous_agents/autogpt/prompt_generator.py
+-rw-r--r--   0        0        0      514 2023-07-24 04:55:17.018061 langchain_experimental-0.0.3/langchain_experimental/autonomous_agents/baby_agi/__init__.py
+-rw-r--r--   0        0        0     7469 2023-07-24 04:55:17.018205 langchain_experimental-0.0.3/langchain_experimental/autonomous_agents/baby_agi/baby_agi.py
+-rw-r--r--   0        0        0     1284 2023-07-24 04:55:17.018915 langchain_experimental-0.0.3/langchain_experimental/autonomous_agents/baby_agi/task_creation.py
+-rw-r--r--   0        0        0      835 2023-07-24 04:55:17.019306 langchain_experimental-0.0.3/langchain_experimental/autonomous_agents/baby_agi/task_execution.py
+-rw-r--r--   0        0        0     1076 2023-07-24 04:55:17.019520 langchain_experimental-0.0.3/langchain_experimental/autonomous_agents/baby_agi/task_prioritization.py
+-rw-r--r--   0        0        0        0 2023-07-24 16:56:12.538041 langchain_experimental-0.0.3/langchain_experimental/autonomous_agents/hugginggpt/__init__.py
+-rw-r--r--   0        0        0     1083 2023-07-24 16:56:12.538313 langchain_experimental-0.0.3/langchain_experimental/autonomous_agents/hugginggpt/hugginggpt.py
+-rw-r--r--   0        0        0     1450 2023-07-24 16:56:12.538516 langchain_experimental-0.0.3/langchain_experimental/autonomous_agents/hugginggpt/repsonse_generator.py
+-rw-r--r--   0        0        0     4551 2023-07-24 16:56:12.538956 langchain_experimental-0.0.3/langchain_experimental/autonomous_agents/hugginggpt/task_executor.py
+-rw-r--r--   0        0        0     6439 2023-07-24 16:56:12.539141 langchain_experimental-0.0.3/langchain_experimental/autonomous_agents/hugginggpt/task_planner.py
+-rw-r--r--   0        0        0      100 2023-07-24 04:55:17.019613 langchain_experimental-0.0.3/langchain_experimental/cpal/README.md
+-rw-r--r--   0        0        0        0 2023-07-24 04:55:17.019645 langchain_experimental-0.0.3/langchain_experimental/cpal/__init__.py
+-rw-r--r--   0        0        0     9041 2023-07-24 04:55:17.019799 langchain_experimental-0.0.3/langchain_experimental/cpal/base.py
+-rw-r--r--   0        0        0      198 2023-07-24 04:55:17.019862 langchain_experimental-0.0.3/langchain_experimental/cpal/constants.py
+-rw-r--r--   0        0        0     8322 2023-07-24 04:55:17.020231 langchain_experimental-0.0.3/langchain_experimental/cpal/models.py
+-rw-r--r--   0        0        0        0 2023-07-24 04:55:17.020291 langchain_experimental-0.0.3/langchain_experimental/cpal/templates/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-24 04:55:17.020363 langchain_experimental-0.0.3/langchain_experimental/cpal/templates/univariate/__init__.py
+-rw-r--r--   0        0        0     2175 2023-07-24 04:55:17.020439 langchain_experimental-0.0.3/langchain_experimental/cpal/templates/univariate/causal.py
+-rw-r--r--   0        0        0      706 2023-07-24 04:55:17.020506 langchain_experimental-0.0.3/langchain_experimental/cpal/templates/univariate/intervention.py
+-rw-r--r--   0        0        0     1750 2023-07-24 04:55:17.020567 langchain_experimental-0.0.3/langchain_experimental/cpal/templates/univariate/narrative.py
+-rw-r--r--   0        0        0     4503 2023-07-24 04:55:17.020637 langchain_experimental-0.0.3/langchain_experimental/cpal/templates/univariate/query.py
+-rw-r--r--   0        0        0      260 2023-07-24 04:55:17.021021 langchain_experimental-0.0.3/langchain_experimental/generative_agents/__init__.py
+-rw-r--r--   0        0        0    10150 2023-07-24 04:55:17.021396 langchain_experimental-0.0.3/langchain_experimental/generative_agents/generative_agent.py
+-rw-r--r--   0        0        0    12461 2023-07-24 04:55:17.021840 langchain_experimental-0.0.3/langchain_experimental/generative_agents/memory.py
+-rw-r--r--   0        0        0      277 2023-07-24 04:55:17.022301 langchain_experimental-0.0.3/langchain_experimental/llms/__init__.py
+-rw-r--r--   0        0        0     1838 2023-07-24 04:55:17.022745 langchain_experimental-0.0.3/langchain_experimental/llms/jsonformer_decoder.py
+-rw-r--r--   0        0        0     4590 2023-07-24 04:55:17.023168 langchain_experimental-0.0.3/langchain_experimental/llms/llamaapi.py
+-rw-r--r--   0        0        0     2027 2023-07-24 04:55:17.023571 langchain_experimental-0.0.3/langchain_experimental/llms/rellm_decoder.py
+-rw-r--r--   0        0        0      277 2023-07-24 04:55:17.023692 langchain_experimental-0.0.3/langchain_experimental/pal_chain/__init__.py
+-rw-r--r--   0        0        0    12482 2023-07-24 04:55:17.024040 langchain_experimental-0.0.3/langchain_experimental/pal_chain/base.py
+-rw-r--r--   0        0        0     2645 2023-07-24 04:55:17.024285 langchain_experimental-0.0.3/langchain_experimental/pal_chain/colored_object_prompt.py
+-rw-r--r--   0        0        0     4301 2023-07-24 04:55:17.024347 langchain_experimental-0.0.3/langchain_experimental/pal_chain/math_prompt.py
+-rw-r--r--   0        0        0      363 2023-07-24 04:55:17.024486 langchain_experimental-0.0.3/langchain_experimental/plan_and_execute/__init__.py
+-rw-r--r--   0        0        0     2078 2023-07-24 04:55:17.024747 langchain_experimental-0.0.3/langchain_experimental/plan_and_execute/agent_executor.py
+-rw-r--r--   0        0        0        0 2023-07-24 04:55:17.024797 langchain_experimental-0.0.3/langchain_experimental/plan_and_execute/executors/__init__.py
+-rw-r--r--   0        0        0     1464 2023-07-24 04:55:17.024918 langchain_experimental-0.0.3/langchain_experimental/plan_and_execute/executors/agent_executor.py
+-rw-r--r--   0        0        0     1156 2023-07-24 04:55:17.025033 langchain_experimental-0.0.3/langchain_experimental/plan_and_execute/executors/base.py
+-rw-r--r--   0        0        0        0 2023-07-24 04:55:17.025085 langchain_experimental-0.0.3/langchain_experimental/plan_and_execute/planners/__init__.py
+-rw-r--r--   0        0        0     1362 2023-07-24 04:55:17.025202 langchain_experimental-0.0.3/langchain_experimental/plan_and_execute/planners/base.py
+-rw-r--r--   0        0        0     1800 2023-07-24 04:55:17.025534 langchain_experimental-0.0.3/langchain_experimental/plan_and_execute/planners/chat_planner.py
+-rw-r--r--   0        0        0     1149 2023-07-24 04:55:17.025717 langchain_experimental-0.0.3/langchain_experimental/plan_and_execute/schema.py
+-rw-r--r--   0        0        0       87 2023-07-24 04:55:17.025843 langchain_experimental-0.0.3/langchain_experimental/prompts/__init__.py
+-rw-r--r--   0        0        0     1873 2023-07-24 04:55:17.026702 langchain_experimental-0.0.3/langchain_experimental/prompts/load.py
+-rw-r--r--   0        0        0      140 2023-07-24 04:55:17.027115 langchain_experimental-0.0.3/langchain_experimental/sql/__init__.py
+-rw-r--r--   0        0        0    11411 2023-07-24 04:55:17.027413 langchain_experimental-0.0.3/langchain_experimental/sql/base.py
+-rw-r--r--   0        0        0    14202 2023-07-24 04:55:17.027655 langchain_experimental-0.0.3/langchain_experimental/sql/prompt.py
+-rw-r--r--   0        0        0     1904 2023-07-24 16:56:12.541800 langchain_experimental-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 langchain_experimental-0.0.3/PKG-INFO
```

### Comparing `langchain_experimental-0.0.2/langchain_experimental/autonomous_agents/autogpt/agent.py` & `langchain_experimental-0.0.3/langchain_experimental/autonomous_agents/autogpt/agent.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.2/langchain_experimental/autonomous_agents/autogpt/memory.py` & `langchain_experimental-0.0.3/langchain_experimental/autonomous_agents/autogpt/memory.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.2/langchain_experimental/autonomous_agents/autogpt/output_parser.py` & `langchain_experimental-0.0.3/langchain_experimental/autonomous_agents/autogpt/output_parser.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.2/langchain_experimental/autonomous_agents/autogpt/prompt.py` & `langchain_experimental-0.0.3/langchain_experimental/autonomous_agents/autogpt/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.2/langchain_experimental/autonomous_agents/autogpt/prompt_generator.py` & `langchain_experimental-0.0.3/langchain_experimental/autonomous_agents/autogpt/prompt_generator.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.2/langchain_experimental/autonomous_agents/baby_agi/__init__.py` & `langchain_experimental-0.0.3/langchain_experimental/autonomous_agents/baby_agi/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.2/langchain_experimental/autonomous_agents/baby_agi/baby_agi.py` & `langchain_experimental-0.0.3/langchain_experimental/autonomous_agents/baby_agi/baby_agi.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.2/langchain_experimental/autonomous_agents/baby_agi/task_creation.py` & `langchain_experimental-0.0.3/langchain_experimental/autonomous_agents/baby_agi/task_creation.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.2/langchain_experimental/autonomous_agents/baby_agi/task_execution.py` & `langchain_experimental-0.0.3/langchain_experimental/autonomous_agents/baby_agi/task_execution.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.2/langchain_experimental/autonomous_agents/baby_agi/task_prioritization.py` & `langchain_experimental-0.0.3/langchain_experimental/autonomous_agents/baby_agi/task_prioritization.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.2/langchain_experimental/cpal/base.py` & `langchain_experimental-0.0.3/langchain_experimental/cpal/base.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.2/langchain_experimental/cpal/models.py` & `langchain_experimental-0.0.3/langchain_experimental/cpal/models.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.2/langchain_experimental/cpal/templates/univariate/causal.py` & `langchain_experimental-0.0.3/langchain_experimental/cpal/templates/univariate/causal.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.2/langchain_experimental/cpal/templates/univariate/intervention.py` & `langchain_experimental-0.0.3/langchain_experimental/cpal/templates/univariate/intervention.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.2/langchain_experimental/cpal/templates/univariate/narrative.py` & `langchain_experimental-0.0.3/langchain_experimental/cpal/templates/univariate/narrative.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.2/langchain_experimental/cpal/templates/univariate/query.py` & `langchain_experimental-0.0.3/langchain_experimental/cpal/templates/univariate/query.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.2/langchain_experimental/generative_agents/generative_agent.py` & `langchain_experimental-0.0.3/langchain_experimental/generative_agents/generative_agent.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.2/langchain_experimental/generative_agents/memory.py` & `langchain_experimental-0.0.3/langchain_experimental/generative_agents/memory.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.2/langchain_experimental/llms/jsonformer_decoder.py` & `langchain_experimental-0.0.3/langchain_experimental/llms/jsonformer_decoder.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.2/langchain_experimental/llms/llamaapi.py` & `langchain_experimental-0.0.3/langchain_experimental/llms/llamaapi.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.2/langchain_experimental/llms/rellm_decoder.py` & `langchain_experimental-0.0.3/langchain_experimental/llms/rellm_decoder.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.2/langchain_experimental/pal_chain/base.py` & `langchain_experimental-0.0.3/langchain_experimental/pal_chain/base.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.2/langchain_experimental/pal_chain/colored_object_prompt.py` & `langchain_experimental-0.0.3/langchain_experimental/pal_chain/colored_object_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.2/langchain_experimental/pal_chain/math_prompt.py` & `langchain_experimental-0.0.3/langchain_experimental/pal_chain/math_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.2/langchain_experimental/plan_and_execute/agent_executor.py` & `langchain_experimental-0.0.3/langchain_experimental/plan_and_execute/agent_executor.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.2/langchain_experimental/plan_and_execute/executors/agent_executor.py` & `langchain_experimental-0.0.3/langchain_experimental/plan_and_execute/executors/agent_executor.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.2/langchain_experimental/plan_and_execute/executors/base.py` & `langchain_experimental-0.0.3/langchain_experimental/plan_and_execute/executors/base.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.2/langchain_experimental/plan_and_execute/planners/base.py` & `langchain_experimental-0.0.3/langchain_experimental/plan_and_execute/planners/base.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.2/langchain_experimental/plan_and_execute/planners/chat_planner.py` & `langchain_experimental-0.0.3/langchain_experimental/plan_and_execute/planners/chat_planner.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.2/langchain_experimental/plan_and_execute/schema.py` & `langchain_experimental-0.0.3/langchain_experimental/plan_and_execute/schema.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.2/langchain_experimental/prompts/load.py` & `langchain_experimental-0.0.3/langchain_experimental/prompts/load.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.2/langchain_experimental/sql/base.py` & `langchain_experimental-0.0.3/langchain_experimental/sql/base.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.2/langchain_experimental/sql/prompt.py` & `langchain_experimental-0.0.3/langchain_experimental/sql/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.2/pyproject.toml` & `langchain_experimental-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-experimental"
-version = "0.0.2"
+version = "0.0.3"
 description = "Building applications with LLMs through composability"
 authors = []
 license = "MIT"
 readme = "README.md"
 repository = "https://www.github.com/hwchase17/langchain"
```

### Comparing `langchain_experimental-0.0.2/PKG-INFO` & `langchain_experimental-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-experimental
-Version: 0.0.2
+Version: 0.0.3
 Summary: Building applications with LLMs through composability
 Home-page: https://www.github.com/hwchase17/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

