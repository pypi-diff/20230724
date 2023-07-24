# Comparing `tmp/auto-eval-0.3.5.tar.gz` & `tmp/auto-eval-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-eval-0.3.5.tar", last modified: Sat Jul 22 09:46:39 2023, max compression
+gzip compressed data, was "auto-eval-0.3.6.tar", last modified: Mon Jul 24 03:08:52 2023, max compression
```

## Comparing `auto-eval-0.3.5.tar` & `auto-eval-0.3.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-22 09:46:39.014622 auto-eval-0.3.5/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1071 2023-04-28 07:53:45.000000 auto-eval-0.3.5/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)    16509 2023-07-22 09:46:39.014422 auto-eval-0.3.5/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)    16083 2023-06-07 06:25:31.000000 auto-eval-0.3.5/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-22 09:46:39.010857 auto-eval-0.3.5/auto_eval.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)    16509 2023-07-22 09:46:38.000000 auto-eval-0.3.5/auto_eval.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      465 2023-07-22 09:46:38.000000 auto-eval-0.3.5/auto_eval.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-07-22 09:46:38.000000 auto-eval-0.3.5/auto_eval.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       59 2023-07-22 09:46:38.000000 auto-eval-0.3.5/auto_eval.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       49 2023-07-22 09:46:38.000000 auto-eval-0.3.5/auto_eval.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        5 2023-07-22 09:46:38.000000 auto-eval-0.3.5/auto_eval.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-22 09:46:39.011311 auto-eval-0.3.5/eval/
--rw-r--r--   0 zhangchong   (501) staff       (20)      136 2023-05-08 07:54:51.000000 auto-eval-0.3.5/eval/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)    15263 2023-07-22 09:38:05.000000 auto-eval-0.3.5/eval/auto_llms_eval.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-22 09:46:39.011915 auto-eval-0.3.5/eval/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:32:15.000000 auto-eval-0.3.5/eval/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     6145 2023-07-22 06:52:22.000000 auto-eval-0.3.5/eval/commands/auto_eval.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-22 09:46:39.013116 auto-eval-0.3.5/eval/prompt_template/
--rw-r--r--   0 zhangchong   (501) staff       (20)      198 2023-05-19 08:23:31.000000 auto-eval-0.3.5/eval/prompt_template/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     3094 2023-06-27 06:27:16.000000 auto-eval-0.3.5/eval/prompt_template/prompter.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     2646 2023-06-28 02:43:09.000000 auto-eval-0.3.5/eval/prompt_template/prompts.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-22 09:46:39.013934 auto-eval-0.3.5/eval/utils/
--rw-r--r--   0 zhangchong   (501) staff       (20)       26 2023-04-28 09:40:19.000000 auto-eval-0.3.5/eval/utils/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     4197 2023-06-29 07:42:59.000000 auto-eval-0.3.5/eval/utils/data_utils.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-22 09:46:39.014670 auto-eval-0.3.5/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)      956 2023-07-22 09:39:26.000000 auto-eval-0.3.5/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-24 03:08:52.686622 auto-eval-0.3.6/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1071 2023-04-28 07:53:45.000000 auto-eval-0.3.6/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)    16509 2023-07-24 03:08:52.686370 auto-eval-0.3.6/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)    16083 2023-06-07 06:25:31.000000 auto-eval-0.3.6/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-24 03:08:52.681293 auto-eval-0.3.6/auto_eval.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)    16509 2023-07-24 03:08:52.000000 auto-eval-0.3.6/auto_eval.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      465 2023-07-24 03:08:52.000000 auto-eval-0.3.6/auto_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-07-24 03:08:52.000000 auto-eval-0.3.6/auto_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       59 2023-07-24 03:08:52.000000 auto-eval-0.3.6/auto_eval.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       49 2023-07-24 03:08:52.000000 auto-eval-0.3.6/auto_eval.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        5 2023-07-24 03:08:52.000000 auto-eval-0.3.6/auto_eval.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-24 03:08:52.681801 auto-eval-0.3.6/eval/
+-rw-r--r--   0 zhangchong   (501) staff       (20)      136 2023-05-08 07:54:51.000000 auto-eval-0.3.6/eval/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)    15857 2023-07-24 03:05:07.000000 auto-eval-0.3.6/eval/auto_llms_eval.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-24 03:08:52.683014 auto-eval-0.3.6/eval/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:32:15.000000 auto-eval-0.3.6/eval/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     6171 2023-07-24 02:32:35.000000 auto-eval-0.3.6/eval/commands/auto_eval.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-24 03:08:52.684405 auto-eval-0.3.6/eval/prompt_template/
+-rw-r--r--   0 zhangchong   (501) staff       (20)      198 2023-05-19 08:23:31.000000 auto-eval-0.3.6/eval/prompt_template/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3094 2023-06-27 06:27:16.000000 auto-eval-0.3.6/eval/prompt_template/prompter.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2646 2023-06-28 02:43:09.000000 auto-eval-0.3.6/eval/prompt_template/prompts.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-24 03:08:52.685363 auto-eval-0.3.6/eval/utils/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       26 2023-04-28 09:40:19.000000 auto-eval-0.3.6/eval/utils/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     4197 2023-06-29 07:42:59.000000 auto-eval-0.3.6/eval/utils/data_utils.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-24 03:08:52.686676 auto-eval-0.3.6/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)      956 2023-07-22 10:07:13.000000 auto-eval-0.3.6/setup.py
```

### Comparing `auto-eval-0.3.5/LICENSE` & `auto-eval-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `auto-eval-0.3.5/PKG-INFO` & `auto-eval-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-eval
-Version: 0.3.5
+Version: 0.3.6
 Summary: Using only one line of commmands to evaluate multiple models
 Home-page: https://github.com/muximus3/Auto-Eval
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `auto-eval-0.3.5/README.md` & `auto-eval-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `auto-eval-0.3.5/auto_eval.egg-info/PKG-INFO` & `auto-eval-0.3.6/auto_eval.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-eval
-Version: 0.3.5
+Version: 0.3.6
 Summary: Using only one line of commmands to evaluate multiple models
 Home-page: https://github.com/muximus3/Auto-Eval
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `auto-eval-0.3.5/eval/auto_llms_eval.py` & `auto-eval-0.3.6/eval/auto_llms_eval.py`

 * *Files 8% similar despite different names*

```diff
@@ -243,21 +243,21 @@
 def save_results(results_df: pd.DataFrame, output_path: str):
     print(f'Saving evaluation results: {output_path}')
     df_saver(results_df, output_path)
     print(f'Saved successfully.')
 
 @dataclass
 class EvalConfig:
-    api_config_files: str
+    api_config_files: list
     eval_prompter: Prompter
     eval_data_path: str
     question_column_names: Optional[List[str]] = None
     answer_column_names: Optional[List[str]] = None
     output_path: str = ''
-    engine: str = ''
+    engines: Optional[List[str]] = None
     eval_categories: Optional[List[str]] = None
     eval_models: Optional[List[str]] = None
     score_by: Optional[List[str]] = None
     sample_num: int = 0
     request_interval: int = 1
     retry: bool = True
     temperature: float = 0.1
@@ -266,31 +266,37 @@
 def eval_groups(
     eval_config: EvalConfig
 ):
     # Preparing data
     scored_groups, unscored_groups = prepare_eval_data(eval_config.eval_data_path, eval_config.eval_categories, eval_config.question_column_names, eval_config.answer_column_names, eval_config.sample_num, eval_config.eval_models)
 
     process_num = len(eval_config.api_config_files)
+    if eval_config.engines is not None and len(eval_config.engines) > 1:
+        assert len(eval_config.engines) == process_num, f'Number of engines must be equal to number of api config files when specific multiple engines, but got {len(eval_config.engines)} engines and {process_num} api config files.'
+    if eval_config.engines is not None and len(eval_config.engines) == 1:
+        eval_config.engines = eval_config.engines * process_num
+    eval_config.engines = eval_config.engines if eval_config.engines is not None else [''] * process_num
+
     # Init api tool and prompter
     if process_num == 1:
         failed_groups = []
         tool = OneAPITool.from_config_file(eval_config.api_config_files[0])
         for group in tqdm(unscored_groups):
-            result, status = eval_one_group(tool, eval_config.eval_prompter,  group,  eval_config.engine, eval_config.temperature, eval_config.max_new_tokens)
+            result, status = eval_one_group(tool, eval_config.eval_prompter,  group,  eval_config.engines[0], eval_config.temperature, eval_config.max_new_tokens)
             if status:
                 scored_groups.append(result)
             else:
                 failed_groups.append(group)
             time.sleep(eval_config.request_interval)
 
         # Retry failed requests
         if len(failed_groups) > 0 and eval_config.retry:
             retry_failed_groups = []
             for group in tqdm(failed_groups, desc='RETRY'):
-                result, status = eval_one_group(tool, eval_config.eval_prompter,  group,  eval_config.engine, eval_config.temperature, eval_config.max_new_tokens)
+                result, status = eval_one_group(tool, eval_config.eval_prompter,  group,  eval_config.engines[0], eval_config.temperature, eval_config.max_new_tokens)
                 if status:
                     scored_groups.append(result)
                 else:
                     retry_failed_groups.append(group)
                 time.sleep(eval_config.request_interval)
     else:
         score_results = asyncio.run(aeval_groups(eval_config, unscored_groups))
@@ -310,15 +316,15 @@
                 else:
                     retry_failed_groups.append(result)
     failed_groups = retry_failed_groups if eval_config.retry and len(failed_groups) > 0 else failed_groups
     scored_results_df = pd.concat(scored_groups)
     log_score_results(eval_results_df=scored_results_df, score_by=eval_config.score_by)
     log_eval_prompt_scores_loss(eval_results_df=scored_results_df)
     # Log score results
-    print(f'Eval engine: {eval_config.engine}')
+    print(f'Eval engine: {eval_config.engines}')
     print(f'Eval files: {eval_config.eval_data_path}')
     print(f'Failed requests: {len(failed_groups)}/{len(scored_groups) + len(failed_groups)}')
     results_df = pd.concat([scored_results_df, pd.concat(failed_groups)]) if len(failed_groups) > 0 else scored_results_df
     # Save results
     if eval_config.output_path:
         save_results(results_df=results_df, output_path=eval_config.output_path)
 
@@ -331,15 +337,15 @@
 
 async def aeval_groups(eval_config: EvalConfig, unscored_groups: List[pd.DataFrame], desc: str='EVAL'):
     # Preparing data
     process_num = len(eval_config.api_config_files)
     pbar = tqdm(total=len(unscored_groups), desc=desc)
     sem = asyncio.Semaphore(process_num)
     tools = [OneAPITool.from_config_file(config_file) for config_file in eval_config.api_config_files]
-    tasks = [asyncio.ensure_future(bound_fetch(sem, tools[i%process_num], eval_config.eval_prompter,  group,  eval_config.engine, eval_config.temperature, eval_config.max_new_tokens)) for i, group in enumerate(unscored_groups)]
+    tasks = [asyncio.ensure_future(bound_fetch(sem, tools[i%process_num], eval_config.eval_prompter,  group,  eval_config.engines[i%process_num], eval_config.temperature, eval_config.max_new_tokens)) for i, group in enumerate(unscored_groups)]
     task_batches = [tasks[i:i + process_num] for i in range(0, len(tasks), process_num)]
     results = []
     async with aiohttp.ClientSession() as session:
         openai.aiosession.set(session)
         for task_batch in task_batches:
             batch_results = await asyncio.gather(*task_batch)
             results.extend(batch_results)
```

### Comparing `auto-eval-0.3.5/eval/commands/auto_eval.py` & `auto-eval-0.3.6/eval/commands/auto_eval.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,16 @@
         default=False,
         help="print every prompt and response detail",
         required=False,
     )
     parser.add_argument(
         "-m",
         "--model",
-        default='',
+        default=None,
+        nargs="+", 
         help="evaluate model name, e.g., gpt-35-turbo, gpt-4, please using larger models like GPT-4 for more difficult questions and faster models like GPT-3.5-turbo for simpler ones.",
         required=False,
     )
     parser.add_argument(
         "-te",
         "--temperature",
         type=float,
@@ -162,30 +163,30 @@
         tool = OneAPITool.from_config_file(args.config_files[0])
         score, raw_response = eval_one_qa(
             api_tool=tool,
             eval_prompter=eval_prompter,
             question=args.prompt,
             candidate_answers=args.answers,
             target=args.target,
-            engine=args.model,
+            engine=args.model[0],
             temperature=args.temperature,
             max_new_tokens=args.max_new_tokens,
         )
         print(f"\nSCORE:\n{score}")
 
     elif args.command == "file":
         eval_groups(
             EvalConfig(
                 api_config_files=args.config_files,
                 eval_prompter=eval_prompter,
                 eval_data_path=args.eval_data_path,
                 question_column_names=args.question_column_names,
                 answer_column_names=args.answer_column_names,
                 output_path=args.output_path,
-                engine=args.model,
+                engines=args.model,
                 eval_categories=args.eval_categories,
                 eval_models=args.eval_models,
                 sample_num=args.sample_num,
                 request_interval=args.interval,
                 retry=args.retry,
                 score_by = args.score_by,
                 temperature=args.temperature,
```

### Comparing `auto-eval-0.3.5/eval/prompt_template/prompter.py` & `auto-eval-0.3.6/eval/prompt_template/prompter.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.3.5/eval/prompt_template/prompts.py` & `auto-eval-0.3.6/eval/prompt_template/prompts.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.3.5/eval/utils/data_utils.py` & `auto-eval-0.3.6/eval/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.3.5/setup.py` & `auto-eval-0.3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="auto-eval",
-    version="0.3.5",
+    version="0.3.6",
     packages=find_packages(),
     # package_data={
     #   "eval":["prompt_template/eval_prompt_template.json"]  
     # },
     install_requires=[
         # Add your library's dependencies here
         "one-api-tool",
```

