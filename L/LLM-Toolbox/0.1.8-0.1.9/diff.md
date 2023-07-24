# Comparing `tmp/LLM-Toolbox-0.1.8.tar.gz` & `tmp/LLM-Toolbox-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LLM-Toolbox-0.1.8.tar", last modified: Fri Jul  7 06:21:13 2023, max compression
+gzip compressed data, was "LLM-Toolbox-0.1.9.tar", last modified: Mon Jul 24 01:22:06 2023, max compression
```

## Comparing `LLM-Toolbox-0.1.8.tar` & `LLM-Toolbox-0.1.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-07 06:21:13.686696 LLM-Toolbox-0.1.8/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11357 2023-06-16 08:04:31.000000 LLM-Toolbox-0.1.8/LICENSE
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-07 06:21:13.676696 LLM-Toolbox-0.1.8/LLM_Toolbox.egg-info/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    17200 2023-07-07 06:21:13.000000 LLM-Toolbox-0.1.8/LLM_Toolbox.egg-info/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      913 2023-07-07 06:21:13.000000 LLM-Toolbox-0.1.8/LLM_Toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-07-07 06:21:13.000000 LLM-Toolbox-0.1.8/LLM_Toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      702 2023-07-07 06:21:13.000000 LLM-Toolbox-0.1.8/LLM_Toolbox.egg-info/entry_points.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       96 2023-07-07 06:21:13.000000 LLM-Toolbox-0.1.8/LLM_Toolbox.egg-info/requires.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       12 2023-07-07 06:21:13.000000 LLM-Toolbox-0.1.8/LLM_Toolbox.egg-info/top_level.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    17200 2023-07-07 06:21:13.686696 LLM-Toolbox-0.1.8/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    16662 2023-06-28 10:02:44.000000 LLM-Toolbox-0.1.8/README.md
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-07 06:21:13.676696 LLM-Toolbox-0.1.8/llm_toolbox/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 18:46:56.000000 LLM-Toolbox-0.1.8/llm_toolbox/__init__.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    16246 2023-07-07 06:16:50.000000 LLM-Toolbox-0.1.8/llm_toolbox/cli.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-07 06:21:13.676696 LLM-Toolbox-0.1.8/llm_toolbox/tools/
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-07 06:21:13.686696 LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      367 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/cheermeup.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      593 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/codereview.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      853 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/commitgen.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1372 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/critique.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      269 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/define.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      331 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/explain.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      747 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/lessonize.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      831 2023-06-27 10:28:40.000000 LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/life.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      532 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/pathlearner.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      422 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/proofread.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      452 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/study.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      411 2023-06-27 04:12:58.000000 LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/summarize.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      817 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/teachlib.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      247 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/thesaurus.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      363 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/translate.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-07-07 06:21:13.686696 LLM-Toolbox-0.1.8/setup.cfg
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2173 2023-07-07 06:20:12.000000 LLM-Toolbox-0.1.8/setup.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-24 01:22:06.266284 LLM-Toolbox-0.1.9/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11357 2023-06-16 08:04:31.000000 LLM-Toolbox-0.1.9/LICENSE
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-24 01:22:06.266284 LLM-Toolbox-0.1.9/LLM_Toolbox.egg-info/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    17200 2023-07-24 01:22:06.000000 LLM-Toolbox-0.1.9/LLM_Toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      913 2023-07-24 01:22:06.000000 LLM-Toolbox-0.1.9/LLM_Toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-07-24 01:22:06.000000 LLM-Toolbox-0.1.9/LLM_Toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      702 2023-07-24 01:22:06.000000 LLM-Toolbox-0.1.9/LLM_Toolbox.egg-info/entry_points.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       96 2023-07-24 01:22:06.000000 LLM-Toolbox-0.1.9/LLM_Toolbox.egg-info/requires.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       12 2023-07-24 01:22:06.000000 LLM-Toolbox-0.1.9/LLM_Toolbox.egg-info/top_level.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    17200 2023-07-24 01:22:06.266284 LLM-Toolbox-0.1.9/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    16662 2023-06-28 10:02:44.000000 LLM-Toolbox-0.1.9/README.md
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-24 01:22:06.266284 LLM-Toolbox-0.1.9/llm_toolbox/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 18:46:56.000000 LLM-Toolbox-0.1.9/llm_toolbox/__init__.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    15930 2023-07-24 01:18:04.000000 LLM-Toolbox-0.1.9/llm_toolbox/cli.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-24 01:22:06.266284 LLM-Toolbox-0.1.9/llm_toolbox/tools/
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-24 01:22:06.266284 LLM-Toolbox-0.1.9/llm_toolbox/tools/templates/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      367 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.9/llm_toolbox/tools/templates/cheermeup.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      593 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.9/llm_toolbox/tools/templates/codereview.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      853 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.9/llm_toolbox/tools/templates/commitgen.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1372 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.9/llm_toolbox/tools/templates/critique.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      269 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.9/llm_toolbox/tools/templates/define.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      331 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.9/llm_toolbox/tools/templates/explain.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      747 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.9/llm_toolbox/tools/templates/lessonize.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      832 2023-07-24 01:14:52.000000 LLM-Toolbox-0.1.9/llm_toolbox/tools/templates/life.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      532 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.9/llm_toolbox/tools/templates/pathlearner.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      422 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.9/llm_toolbox/tools/templates/proofread.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      452 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.9/llm_toolbox/tools/templates/study.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      411 2023-06-27 04:12:58.000000 LLM-Toolbox-0.1.9/llm_toolbox/tools/templates/summarize.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      817 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.9/llm_toolbox/tools/templates/teachlib.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      247 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.9/llm_toolbox/tools/templates/thesaurus.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      363 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.9/llm_toolbox/tools/templates/translate.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-07-24 01:22:06.266284 LLM-Toolbox-0.1.9/setup.cfg
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2178 2023-07-24 01:21:02.000000 LLM-Toolbox-0.1.9/setup.py
```

### Comparing `LLM-Toolbox-0.1.8/LICENSE` & `LLM-Toolbox-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.8/LLM_Toolbox.egg-info/PKG-INFO` & `LLM-Toolbox-0.1.9/LLM_Toolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LLM-Toolbox
-Version: 0.1.8
+Version: 0.1.9
 Summary: A versatile collection of CLI tools leveraging large language models
 Home-page: https://github.com/sderev/llm-toolbox
 Author: Sébastien De Revière
 License: Apache Licence, Version 2.0
 Project-URL: Documentation, https://github.com/sderev/llm-toolbox
 Project-URL: Issues, http://github.com/sderev/llm-toolbox/issues
 Project-URL: Changelog, https://github.com/sderev/llm-toolbox/releases
```

### Comparing `LLM-Toolbox-0.1.8/LLM_Toolbox.egg-info/SOURCES.txt` & `LLM-Toolbox-0.1.9/LLM_Toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.8/LLM_Toolbox.egg-info/entry_points.txt` & `LLM-Toolbox-0.1.9/LLM_Toolbox.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.8/PKG-INFO` & `LLM-Toolbox-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LLM-Toolbox
-Version: 0.1.8
+Version: 0.1.9
 Summary: A versatile collection of CLI tools leveraging large language models
 Home-page: https://github.com/sderev/llm-toolbox
 Author: Sébastien De Revière
 License: Apache Licence, Version 2.0
 Project-URL: Documentation, https://github.com/sderev/llm-toolbox
 Project-URL: Issues, http://github.com/sderev/llm-toolbox/issues
 Project-URL: Changelog, https://github.com/sderev/llm-toolbox/releases
```

### Comparing `LLM-Toolbox-0.1.8/README.md` & `LLM-Toolbox-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.8/llm_toolbox/cli.py` & `LLM-Toolbox-0.1.9/llm_toolbox/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 import json
 import os
 import shutil
 import subprocess
 import sys
 import tempfile
-import requests
 from datetime import datetime
 from functools import wraps
 from pathlib import Path
 
 import click
-import validators
+import requests
 from strip_tags.lib import strip_tags
+import validators
+import yaml
+
 
-from lmt_cli.lib import *
-from lmt_cli.cli import VALID_MODELS
+from lmt_cli.cli import validate_model_name, validate_temperature
+from lmt_cli.lib import prepare_and_generate_response
+from lmt_cli.templates import get_template_content, TEMPLATES_DIR
 
 
 def install_templates():
     """
-    Installs the templates in the user's home directory.
+    Installs the templates in ~/.config/lmt/templates.
     """
     dest_path = Path.home() / ".config/lmt/templates"
     dest_path.mkdir(parents=True, exist_ok=True)
 
     config_file = Path.home() / ".config/lmt/config.json"
     config_file.touch(exist_ok=True)
 
@@ -55,38 +58,14 @@
         json.dump(config, file, indent=4)
     print()
 
 
 install_templates()
 
 
-def validate_model_name(ctx, param, value):
-    """
-    Validates the model name parameter.
-    """
-    model_name = value.lower()
-    if model_name in VALID_MODELS:
-        return VALID_MODELS[model_name]
-
-    if model_name in VALID_MODELS.values():
-        return model_name
-
-    if not any(model_name in items for items in VALID_MODELS.items()):
-        raise click.BadParameter(f"Invalid model: {model_name}")
-
-
-def validate_temperature(ctx, param, value):
-    """
-    Validates the temperature parameter.
-    """
-    if 0 <= value <= 2:
-        return value
-    raise click.BadParameter("Temperature must be between 0 and 2.")
-
-
 @click.group()
 @click.pass_context
 @click.version_option()
 def cli():
     pass
 
 
@@ -329,17 +308,19 @@
     ) as temp:
         temp.write(commit_message)
         temp_path = temp.name
 
     # Open git commit with temp file as template
     try:
         if choice == "yes":
-            subprocess.run(["git", "commit", "-F", temp_path])
+            subprocess.run(["git", "commit", "-F", temp_path], check=True)
         elif choice == "edit":
-            subprocess.run(["git", "commit", "-e", "-t", temp_path])
+            subprocess.run(["git", "commit", "-e", "-t", temp_path], check=True)
+    except subprocess.CalledProcessError as error:
+        click.echo(f"{click.style('Error occurred: {error}', fg='red')}", err=True)
     finally:
         os.remove(temp_path)
 
 
 @cli.command()
 @click.argument("file_to_review", type=click.File("r"), required=False)
 @click.pass_context
@@ -375,15 +356,15 @@
     Summarize the text, the content of a given file, or a webpage (provided as URL).
     """
     source_str = " ".join(source)
 
     prompt_input = ""
 
     if validators.url(source_str):
-        source_content = requests.get(source_str).text
+        source_content = requests.get(source_str, timeout=5).text
         prompt_input = strip_tags(input=source_content, minify=True)
     else:
         if source:
             content = "".join(source)
             prompt_input += content
 
     process_command(
@@ -527,15 +508,15 @@
         raw,
         debug,
     )
 
 
 @cli.command()
 @click.pass_context
-@click.option("--reset", is_flag=True, help="Reset the template file.")
+@click.option("--reset", is_flag=True, help="Reset the name and the date of birth.")
 @common_options
 def life(ctx, reset, model, emoji, temperature, tokens, no_stream, raw, debug):
     """
     Comment on the remaining lifespan of a person.
     """
     template_file = get_template_content("life")
     user_info = template_file["user_info"]
@@ -618,14 +599,15 @@
                     ),
                     fg="yellow",
                 )
                 + "\n---"
             )
             prompt_input = sys.stdin.read()
             click.echo()
+
     if template == "summarize":
         prompt_input = "".join(prompt_input).rstrip()
     else:
         prompt_input = " ".join(prompt_input).rstrip()
 
     return prepare_and_generate_response(
         system=None,
```

### Comparing `LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/codereview.yaml` & `LLM-Toolbox-0.1.9/llm_toolbox/tools/templates/codereview.yaml`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/commitgen.yaml` & `LLM-Toolbox-0.1.9/llm_toolbox/tools/templates/commitgen.yaml`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/critique.yaml` & `LLM-Toolbox-0.1.9/llm_toolbox/tools/templates/critique.yaml`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/lessonize.yaml` & `LLM-Toolbox-0.1.9/llm_toolbox/tools/templates/lessonize.yaml`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/life.yaml` & `LLM-Toolbox-0.1.9/llm_toolbox/tools/templates/life.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
   name:
   date_of_birth:
   life_expectancy: 28470 # Average life expectancy in days, approximately 78 years
 
 system: >
   As a friend, write a thoughtful, genuine message for {user_name},
   who has about {remaining_days} days ahead of them,
-  which represents approximately {percentage}% of their expected life span.
+  which represents approximately {percentage} % of their expected life span.
   Based on this percentage, provide a unique perspective
   on how {user_name} might view their future.
   Keep in mind that these are statistical estimations
   and the uncertainty of life is what makes it precious.
   Make sure to reference these numbers in your message,
   but avoid sounding overly sentimental or like a self-help book.
   Rather than using clichéd quotes, try to draw on the wisdom of philosophers,
```

### Comparing `LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/pathlearner.yaml` & `LLM-Toolbox-0.1.9/llm_toolbox/tools/templates/pathlearner.yaml`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.8/llm_toolbox/tools/templates/teachlib.yaml` & `LLM-Toolbox-0.1.9/llm_toolbox/tools/templates/teachlib.yaml`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.8/setup.py` & `LLM-Toolbox-0.1.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-from setuptools import setup, find_packages
-from setuptools.command.develop import develop
-from setuptools.command.install import install
-from pathlib import Path
 import shutil
+from setuptools import setup, find_packages
 
-VERSION = "0.1.8"
+VERSION = "0.1.9"
 
 
 def read_requirements():
-    with open("requirements.txt") as file:
+    """
+    Read requirements from requirements.txt.
+    """
+    with open("requirements.txt", encoding="UTF-8") as file:
         return list(file)
 
 
 def get_long_description():
-    with open("README.md", encoding="utf8") as file:
+    """
+    Read the README.md file.
+    """
+    with open("README.md", encoding="UTF8") as file:
         return file.read()
 
 
 setup(
     name="LLM-Toolbox",
     description="A versatile collection of CLI tools leveraging large language models",
     long_description=get_long_description(),
```

