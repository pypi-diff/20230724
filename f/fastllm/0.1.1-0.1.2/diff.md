# Comparing `tmp/fastllm-0.1.1.tar.gz` & `tmp/fastllm-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastllm-0.1.1.tar", max compression
+gzip compressed data, was "fastllm-0.1.2.tar", max compression
```

## Comparing `fastllm-0.1.1.tar` & `fastllm-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-07-16 18:54:36.878631 fastllm-0.1.1/LICENSE
--rw-r--r--   0        0        0     4120 2023-07-23 15:50:40.782536 fastllm-0.1.1/README.md
--rw-r--r--   0        0        0      137 2023-07-23 15:51:19.906944 fastllm-0.1.1/fastllm/__init__.py
--rw-r--r--   0        0        0    20280 2023-07-23 15:51:15.498897 fastllm-0.1.1/fastllm/base.py
--rw-r--r--   0        0        0     1443 2023-07-23 15:50:48.598612 fastllm-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5028 1970-01-01 00:00:00.000000 fastllm-0.1.1/setup.py
--rw-r--r--   0        0        0     5153 1970-01-01 00:00:00.000000 fastllm-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-24 18:01:27.056723 fastllm-0.1.2/LICENSE
+-rw-r--r--   0        0        0     4183 2023-07-24 18:16:08.416581 fastllm-0.1.2/README.md
+-rw-r--r--   0        0        0      137 2023-07-24 18:01:27.056723 fastllm-0.1.2/fastllm/__init__.py
+-rw-r--r--   0        0        0    20339 2023-07-24 18:18:54.876555 fastllm-0.1.2/fastllm/base.py
+-rw-r--r--   0        0        0     1449 2023-07-24 18:17:36.726567 fastllm-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5069 1970-01-01 00:00:00.000000 fastllm-0.1.2/PKG-INFO
```

### Comparing `fastllm-0.1.1/LICENSE` & `fastllm-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastllm-0.1.1/README.md` & `fastllm-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -26,24 +26,22 @@
 ```bash
 ['Vienna', 'Salzburg', 'Graz']
 ```
 
 ```python
 from fastllm import Agent, Message, Model, Prompt, Role
 
-s = ";"
-
 creative_name_finder = Agent(
     Message("You are an expert name finder.", Role.SYSTEM),
     Prompt("Find {{ n }} names.", temperature=2.0),
-    Prompt("Print names {{ s }} separated, nothing else!"),
-    model=Model("gpt-4"),
+    Prompt("Print names comma separated, nothing else!"),
+    model=Model(name="gpt-4"),
 )
 
-names = creative_name_finder(n=3, s=s).split(s)
+names = creative_name_finder(n=3).split(",")
 
 print(names)
 ```
 
 ```bash
 ['Ethan Gallagher, Samantha Cheng, Max Thompson']
 ```
@@ -58,15 +56,14 @@
 from fastllm import Agent, Prompt
 
 calculator_agent = Agent(
     Prompt("Calculate the result for task: {{ task }}"),
     Prompt("Only give the result number as result without anything else!"),
 )
 
-
 @calculator_agent.function
 def calculator(a, b, operator: Literal["+", "-", "*", "/"]):
     """A basic calculator using various operators."""
 
     match operator:
         case "+":
             return a + b
@@ -81,15 +78,15 @@
 
 
 result = calculator_agent(task="give the final result for (11 + 14) * (6 - 2)")
 
 print(result)
 
 another_result = calculator_agent(
-    task="if I have 114 apples and 3 children, how many apples will each child get?"
+    task="If I have 114 apples and 3 elephants, how many apples will each elephant get?"
 )
 
 print(another_result)
 ```
 
 ```bash
 100
@@ -105,31 +102,32 @@
 - [x] Able to register functions to agents, models and prompts using decorators
 - [x] Possible to register functions on multiple levels (agent, model, prompt). The function call is only available on the level it was registered.
 - [x] Conversation history. The Model class keeps track of the conversation history.
 - [x] Function schema is inferred from python function type hints, documentation and name
 - [x] Function calling is handled by the Model class itself. Meaning if a LLM response indicate a function call, the Model class will call the function and return the result back to the LLM
 - [ ] Function calling can result in an infinite loop if LLM can not provide function name or arguments properly. This needs to be handled by the Model class.
 - [ ] Prompts with pattern using logit bias to guide LLM completion.
+- [ ] Able to switch between models (e.g. 3.5 and 4) within one agent over different prompts.
 - [ ] Handling of multiple response messages from LLMs in a single call. At the moment only the first response is kept.
 - [ ] Supporting non chat based LLMs (e.g. OpenAI's completion LLMs).
-- [ ] Supporting other LLMs over APIs except OpenAI's. (e.g. google, anthropics, etc.)
-- [ ] Supporting local LLMs (e.g. llama-1, llama-2, mpt, etc.)
+- [ ] Supporting other LLMs over APIs except OpenAI's. (e.g. Google etc.)
+- [ ] Supporting local LLMs (e.g. llama-1, llama-2, etc.)
 
 ### Package
 
 - [x] Basic package structure and functionality
 - [x] Test cases and high test coverage
 - [ ] Tests against multiple python versions
 - [ ] 100% test coverage (at the moment around 90%)
 - [ ] Better documentation including readthedocs site.
 - [ ] Better error handling and logging
 - [ ] Better samples using jupyter notebooks
 - [ ] Set up of pre-commit
 - [ ] CI using github actions
-- [ ] Prober release and versioning
+- [ ] Release and versioning
 
 ## Development
 
 Using [poetry](https://python-poetry.org/docs/#installation).
 
 ```bash
 poetry install
```

### Comparing `fastllm-0.1.1/fastllm/base.py` & `fastllm-0.1.2/fastllm/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,14 +125,17 @@
         """Returns the parameters and types of a function."""
 
         params = inspect.signature(function).parameters
         type_hints = get_type_hints(function)
 
         properties = {param: {} for param in params}
         for name, type_hint in type_hints.items():
+            if name == "return":
+                continue
+
             array = False
             literals = None
 
             if get_origin(type_hint) is Literal:
                 literals = get_args(type_hint)
                 literal_types = {type(literal) for literal in literals}
```

### Comparing `fastllm-0.1.1/pyproject.toml` & `fastllm-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "fastllm"
-version = "0.1.1"
+version = "0.1.2"
 description = "Fast and easy wrapper around LLMs."
 authors = ["Clemens Kriechbaumer <clemens.kriechbaumer@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/clemens33/fastllm"
 repository = "https://github.com/clemens33/fastllm"
-keywords = ["agents", "chatbots", "openai", "llm"]
+keywords = ["agents", "chatbots", "openai", "llm", "ai"]
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
 
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     'Programming Language :: Python :: 3.12',
```

### Comparing `fastllm-0.1.1/setup.py` & `fastllm-0.1.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,163 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['fastllm']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['backoff>=2.2.1,<3.0.0',
- 'jinja2>=3.1.2,<4.0.0',
- 'jsonschema>=4.18.4,<5.0.0',
- 'openai>=0.27.8,<0.28.0']
-
-setup_kwargs = {
-    'name': 'fastllm',
-    'version': '0.1.1',
-    'description': 'Fast and easy wrapper around LLMs.',
-    'long_description': '# FastLLM\n\nFast and simple wrapper around LLMs. The package aims to be simply, precise and allows for fast prototyping of agents and applications around LLMs. At the moment focus around OpenAI\'s chat models.\n\n**Warning - experimental package and subject to change.** For features and plans see the [roadmap](#roadmap).\n\n## Samples\n\nRequire an openai api key in `OPENAI_API_KEY` environment variable or `.env` file.\n\n```bash\nexport OPENAI_API_KEY=...\n```\n\n### Agents\n\n```python\nfrom fastllm import Agent\n\nfind_cities = Agent("List {{ n }} cities comma separated in {{ country }}.")\ncities = find_cities(n=3, country="Austria").split(",")\n\nprint(cities)\n```\n\n```bash\n[\'Vienna\', \'Salzburg\', \'Graz\']\n```\n\n```python\nfrom fastllm import Agent, Message, Model, Prompt, Role\n\ns = ";"\n\ncreative_name_finder = Agent(\n    Message("You are an expert name finder.", Role.SYSTEM),\n    Prompt("Find {{ n }} names.", temperature=2.0),\n    Prompt("Print names {{ s }} separated, nothing else!"),\n    model=Model("gpt-4"),\n)\n\nnames = creative_name_finder(n=3, s=s).split(s)\n\nprint(names)\n```\n\n```bash\n[\'Ethan Gallagher, Samantha Cheng, Max Thompson\']\n```\n\n#### Functions\n\nFunctions can be added to Agents, Models or Prompts. Either as initial arguments or as decorator. Functions type hints, documentation and name are inferred from the function and added to the model call.\n\n```python\nfrom typing import Literal\n\nfrom fastllm import Agent, Prompt\n\ncalculator_agent = Agent(\n    Prompt("Calculate the result for task: {{ task }}"),\n    Prompt("Only give the result number as result without anything else!"),\n)\n\n\n@calculator_agent.function\ndef calculator(a, b, operator: Literal["+", "-", "*", "/"]):\n    """A basic calculator using various operators."""\n\n    match operator:\n        case "+":\n            return a + b\n        case "-":\n            return a - b\n        case "*":\n            return a * b\n        case "/":\n            return a / b\n        case _:\n            raise ValueError(f"Unknown operator {operator}")\n\n\nresult = calculator_agent(task="give the final result for (11 + 14) * (6 - 2)")\n\nprint(result)\n\nanother_result = calculator_agent(\n    task="if I have 114 apples and 3 children, how many apples will each child get?"\n)\n\nprint(another_result)\n```\n\n```bash\n100\n38\n```\n\n## Roadmap\n\n### Features\n\n- [x] Prompts using jinja2 templates\n- [x] LLM calling with backoff and retry\n- [x] Able to register functions to agents, models and prompts using decorators\n- [x] Possible to register functions on multiple levels (agent, model, prompt). The function call is only available on the level it was registered.\n- [x] Conversation history. The Model class keeps track of the conversation history.\n- [x] Function schema is inferred from python function type hints, documentation and name\n- [x] Function calling is handled by the Model class itself. Meaning if a LLM response indicate a function call, the Model class will call the function and return the result back to the LLM\n- [ ] Function calling can result in an infinite loop if LLM can not provide function name or arguments properly. This needs to be handled by the Model class.\n- [ ] Prompts with pattern using logit bias to guide LLM completion.\n- [ ] Handling of multiple response messages from LLMs in a single call. At the moment only the first response is kept.\n- [ ] Supporting non chat based LLMs (e.g. OpenAI\'s completion LLMs).\n- [ ] Supporting other LLMs over APIs except OpenAI\'s. (e.g. google, anthropics, etc.)\n- [ ] Supporting local LLMs (e.g. llama-1, llama-2, mpt, etc.)\n\n### Package\n\n- [x] Basic package structure and functionality\n- [x] Test cases and high test coverage\n- [ ] Tests against multiple python versions\n- [ ] 100% test coverage (at the moment around 90%)\n- [ ] Better documentation including readthedocs site.\n- [ ] Better error handling and logging\n- [ ] Better samples using jupyter notebooks\n- [ ] Set up of pre-commit\n- [ ] CI using github actions\n- [ ] Prober release and versioning\n\n## Development\n\nUsing [poetry](https://python-poetry.org/docs/#installation).\n\n```bash\npoetry install\n```\n\n### Tests\n\n```bash\npoetry run pytest\n``` ',
-    'author': 'Clemens Kriechbaumer',
-    'author_email': 'clemens.kriechbaumer@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/clemens33/fastllm',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
-}
-
-
-setup(**setup_kwargs)
+Metadata-Version: 2.1
+Name: fastllm
+Version: 0.1.2
+Summary: Fast and easy wrapper around LLMs.
+Home-page: https://github.com/clemens33/fastllm
+License: Apache-2.0
+Keywords: agents,chatbots,openai,llm,ai
+Author: Clemens Kriechbaumer
+Author-email: clemens.kriechbaumer@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: backoff (>=2.2.1,<3.0.0)
+Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
+Requires-Dist: jsonschema (>=4.18.4,<5.0.0)
+Requires-Dist: openai (>=0.27.8,<0.28.0)
+Project-URL: Repository, https://github.com/clemens33/fastllm
+Description-Content-Type: text/markdown
+
+# FastLLM
+
+Fast and simple wrapper around LLMs. The package aims to be simply, precise and allows for fast prototyping of agents and applications around LLMs. At the moment focus around OpenAI's chat models.
+
+**Warning - experimental package and subject to change.** For features and plans see the [roadmap](#roadmap).
+
+## Samples
+
+Require an openai api key in `OPENAI_API_KEY` environment variable or `.env` file.
+
+```bash
+export OPENAI_API_KEY=...
+```
+
+### Agents
+
+```python
+from fastllm import Agent
+
+find_cities = Agent("List {{ n }} cities comma separated in {{ country }}.")
+cities = find_cities(n=3, country="Austria").split(",")
+
+print(cities)
+```
+
+```bash
+['Vienna', 'Salzburg', 'Graz']
+```
+
+```python
+from fastllm import Agent, Message, Model, Prompt, Role
+
+creative_name_finder = Agent(
+    Message("You are an expert name finder.", Role.SYSTEM),
+    Prompt("Find {{ n }} names.", temperature=2.0),
+    Prompt("Print names comma separated, nothing else!"),
+    model=Model(name="gpt-4"),
+)
+
+names = creative_name_finder(n=3).split(",")
+
+print(names)
+```
+
+```bash
+['Ethan Gallagher, Samantha Cheng, Max Thompson']
+```
+
+#### Functions
+
+Functions can be added to Agents, Models or Prompts. Either as initial arguments or as decorator. Functions type hints, documentation and name are inferred from the function and added to the model call.
+
+```python
+from typing import Literal
+
+from fastllm import Agent, Prompt
+
+calculator_agent = Agent(
+    Prompt("Calculate the result for task: {{ task }}"),
+    Prompt("Only give the result number as result without anything else!"),
+)
+
+@calculator_agent.function
+def calculator(a, b, operator: Literal["+", "-", "*", "/"]):
+    """A basic calculator using various operators."""
+
+    match operator:
+        case "+":
+            return a + b
+        case "-":
+            return a - b
+        case "*":
+            return a * b
+        case "/":
+            return a / b
+        case _:
+            raise ValueError(f"Unknown operator {operator}")
+
+
+result = calculator_agent(task="give the final result for (11 + 14) * (6 - 2)")
+
+print(result)
+
+another_result = calculator_agent(
+    task="If I have 114 apples and 3 elephants, how many apples will each elephant get?"
+)
+
+print(another_result)
+```
+
+```bash
+100
+38
+```
+
+## Roadmap
+
+### Features
+
+- [x] Prompts using jinja2 templates
+- [x] LLM calling with backoff and retry
+- [x] Able to register functions to agents, models and prompts using decorators
+- [x] Possible to register functions on multiple levels (agent, model, prompt). The function call is only available on the level it was registered.
+- [x] Conversation history. The Model class keeps track of the conversation history.
+- [x] Function schema is inferred from python function type hints, documentation and name
+- [x] Function calling is handled by the Model class itself. Meaning if a LLM response indicate a function call, the Model class will call the function and return the result back to the LLM
+- [ ] Function calling can result in an infinite loop if LLM can not provide function name or arguments properly. This needs to be handled by the Model class.
+- [ ] Prompts with pattern using logit bias to guide LLM completion.
+- [ ] Able to switch between models (e.g. 3.5 and 4) within one agent over different prompts.
+- [ ] Handling of multiple response messages from LLMs in a single call. At the moment only the first response is kept.
+- [ ] Supporting non chat based LLMs (e.g. OpenAI's completion LLMs).
+- [ ] Supporting other LLMs over APIs except OpenAI's. (e.g. Google etc.)
+- [ ] Supporting local LLMs (e.g. llama-1, llama-2, etc.)
+
+### Package
+
+- [x] Basic package structure and functionality
+- [x] Test cases and high test coverage
+- [ ] Tests against multiple python versions
+- [ ] 100% test coverage (at the moment around 90%)
+- [ ] Better documentation including readthedocs site.
+- [ ] Better error handling and logging
+- [ ] Better samples using jupyter notebooks
+- [ ] Set up of pre-commit
+- [ ] CI using github actions
+- [ ] Release and versioning
+
+## Development
+
+Using [poetry](https://python-poetry.org/docs/#installation).
+
+```bash
+poetry install
+```
+
+### Tests
+
+```bash
+poetry run pytest
+```
```

