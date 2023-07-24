# Comparing `tmp/gptask_cli-0.1.9.tar.gz` & `tmp/gptask_cli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptask_cli-0.1.9.tar", max compression
+gzip compressed data, was "gptask_cli-0.2.0.tar", max compression
```

## Comparing `gptask_cli-0.1.9.tar` & `gptask_cli-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1075 2023-07-21 04:59:46.922687 gptask_cli-0.1.9/LICENSE
--rw-r--r--   0        0        0     1062 2023-07-21 05:10:41.249397 gptask_cli-0.1.9/README.md
--rw-r--r--   0        0        0      118 2023-07-23 17:54:09.950005 gptask_cli-0.1.9/gptask_cli/.gptask.example/prompts/bug-fixer.gptask
--rw-r--r--   0        0        0      557 2023-07-21 05:12:36.150206 gptask_cli-0.1.9/gptask_cli/.gptask.example/prompts/code-docs.gptask
--rw-r--r--   0        0        0      200 2023-07-21 05:11:01.916225 gptask_cli-0.1.9/gptask_cli/.gptask.example/prompts/code-helper.gptask
--rw-r--r--   0        0        0      189 2023-07-23 17:53:29.637217 gptask_cli-0.1.9/gptask_cli/.gptask.example/prompts/code-refactor.gptask
--rw-r--r--   0        0        0      107 2023-07-23 17:53:41.796618 gptask_cli-0.1.9/gptask_cli/.gptask.example/prompts/code-tester.gptask
--rw-r--r--   0        0        0      185 2023-07-23 04:17:03.127227 gptask_cli-0.1.9/gptask_cli/.gptask.example/prompts/doc-reviewer.gptask
--rw-r--r--   0        0        0       58 2023-07-23 17:55:24.137634 gptask_cli-0.1.9/gptask_cli/.gptask.example/prompts/general.gptask
--rw-r--r--   0        0        0      118 2023-07-23 17:54:36.876406 gptask_cli-0.1.9/gptask_cli/.gptask.example/prompts/security-auditor.gptask
--rw-r--r--   0        0        0     3314 2023-07-23 18:05:52.971724 gptask_cli-0.1.9/gptask_cli/__init__.py
--rw-r--r--   0        0        0     1984 2023-07-23 18:05:57.368240 gptask_cli-0.1.9/gptask_cli/conf.py
--rw-r--r--   0        0        0      854 2023-07-21 04:02:06.937324 gptask_cli-0.1.9/gptask_cli/git_checker.py
--rw-r--r--   0        0        0     1392 2023-07-23 03:58:48.423731 gptask_cli-0.1.9/gptask_cli/openai_gptask.py
--rw-r--r--   0        0        0      430 2023-07-24 08:48:00.683515 gptask_cli-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     1576 1970-01-01 00:00:00.000000 gptask_cli-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-24 17:37:19.468581 gptask_cli-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1828 2023-07-24 19:46:19.270292 gptask_cli-0.2.0/README.md
+-rw-r--r--   0        0        0      118 2023-07-24 17:37:19.469855 gptask_cli-0.2.0/gptask_cli/.gptask.example/prompts/bug-fixer.gptask
+-rw-r--r--   0        0        0      557 2023-07-24 17:37:19.470062 gptask_cli-0.2.0/gptask_cli/.gptask.example/prompts/code-docs.gptask
+-rw-r--r--   0        0        0      200 2023-07-24 17:37:19.470369 gptask_cli-0.2.0/gptask_cli/.gptask.example/prompts/code-helper.gptask
+-rw-r--r--   0        0        0      189 2023-07-24 17:37:19.470559 gptask_cli-0.2.0/gptask_cli/.gptask.example/prompts/code-refactor.gptask
+-rw-r--r--   0        0        0      107 2023-07-24 17:37:19.470765 gptask_cli-0.2.0/gptask_cli/.gptask.example/prompts/code-tester.gptask
+-rw-r--r--   0        0        0      185 2023-07-24 17:37:19.471103 gptask_cli-0.2.0/gptask_cli/.gptask.example/prompts/doc-reviewer.gptask
+-rw-r--r--   0        0        0       58 2023-07-24 17:37:19.471333 gptask_cli-0.2.0/gptask_cli/.gptask.example/prompts/general.gptask
+-rw-r--r--   0        0        0      118 2023-07-24 17:37:19.471536 gptask_cli-0.2.0/gptask_cli/.gptask.example/prompts/security-auditor.gptask
+-rw-r--r--   0        0        0     3959 2023-07-24 19:48:30.642636 gptask_cli-0.2.0/gptask_cli/__init__.py
+-rw-r--r--   0        0        0     1984 2023-07-24 17:37:19.472232 gptask_cli-0.2.0/gptask_cli/conf.py
+-rw-r--r--   0        0        0      854 2023-07-24 17:37:19.472571 gptask_cli-0.2.0/gptask_cli/git_checker.py
+-rw-r--r--   0        0        0     1407 2023-07-24 18:00:51.579775 gptask_cli-0.2.0/gptask_cli/openai_gptask.py
+-rw-r--r--   0        0        0      430 2023-07-24 18:01:03.024063 gptask_cli-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2342 1970-01-01 00:00:00.000000 gptask_cli-0.2.0/PKG-INFO
```

### Comparing `gptask_cli-0.1.9/LICENSE` & `gptask_cli-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gptask_cli-0.1.9/gptask_cli/.gptask.example/prompts/code-docs.gptask` & `gptask_cli-0.2.0/gptask_cli/.gptask.example/prompts/code-docs.gptask`

 * *Files identical despite different names*

### Comparing `gptask_cli-0.1.9/gptask_cli/__init__.py` & `gptask_cli-0.2.0/gptask_cli/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,66 +7,79 @@
 
 def check_file_staged_status(file, force):
     if not force and is_staged(file.name):
         click.echo(f"File {file.name} has staged changes. Please unstage the file before running gptask.")
         return False
     return True
 
-def get_files_to_process(recursive, file):
-    if file:
-        return [file]
-    if recursive:
-        return [open(f, 'r') for f in glob.glob(recursive, recursive=True)]
-    click.echo("Either a file or directory must be provided.")
-    return []
+def _get_path_list(path: str, is_recursive: bool):
+    """
+    Returns a list of paths from a glob pattern, file, or directory to recurse through.
+    """
+    if("*" in path):
+        return glob.glob(path, recursive=True)
+    elif os.path.isfile(path):
+        return [path]
+    elif(path[-1] == "/"):
+        path = path[:-1]
+    
+    # Recurse (or don't) through directory
+    return glob.glob(path + "/**/*" if is_recursive else path + "/*", recursive=True)
+
+def _get_files_from_paths(path_list: list[str]):
+    return [f for f in path_list if os.path.isfile(f)]
+
+def _get_file_list (pattern: str, is_recursive: bool):
+    paths = _get_path_list(pattern, is_recursive)
+    return _get_files_from_paths(paths)
+
+def _get_file_contents_to_process(pattern: str, is_recursive: bool):
+    file_list = _get_file_list(pattern, is_recursive)
+    return [open(f, 'r') for f in file_list]
 
 def get_prompt_contents(prompt, all_prompts):
     if(".gptask" in prompt):
         return all_prompts[prompt[:-7]]
     else:
         return all_prompts[prompt]
 
-def _print_files(start_path):
-    for root, _, files in os.walk(start_path):
-        for file in files:
-            file_path = os.path.join(root, file)
-            print(f"File Name: {file_path}")
-            with open(file_path, 'r') as f:
-                print(f"File Contents:\n{f.read()}\n")
-
 @click.command()
 @click.version_option()
 @click.option('-p', '--prompt', help='Prompts in ~/.gptask/prompts')
 @click.option('-f', '--force', is_flag=True, help='Force execution even if conditions are not met')
-@click.option('-r', '--recursive', type=click.STRING, help='Directory with files to be processed')
+@click.option('-r', '--recursive', is_flag=True, help='If true and pattern is a directory, files will be recursively prompted instead of just the top level')
 @click.option('-l', '--print-files', is_flag=True, help='Prints the files to be processed')
 @click.option('-a', '--print-prompts', is_flag=True, help='Prints all available prompts')
 @click.option('-g', '--reload-example-prompts', is_flag=True, help='Reloads example prompts')
-@click.argument('file', type=click.File('r'), required=False)
-def main(prompt, force, print_files, recursive, print_prompts,reload_example_prompts, file):
+@click.argument('pattern', type=click.STRING, required=True)
+def main(prompt, force, print_files, recursive, print_prompts,reload_example_prompts, pattern):
 
     setup()
     if reload_example_prompts:
         run_reload_example_prompts()
         return
     
-    if print_files and recursive:
-        _print_files(recursive)
+    if print_files:
+        click.echo("Files to be processed:")
+        files_to_print = _get_file_list(pattern, recursive)
+        for file in files_to_print:
+            click.echo(f"  {file}")
         return
 
     all_prompts = load_prompts()
     if print_prompts:
         click.echo("Available prompts:")
         all_prompts = load_prompts()
         for key in all_prompts.keys():
             click.echo(f"  {key}")
         return
 
-    files_to_process = get_files_to_process(recursive, file)
-    if not files_to_process:
+    files_to_process = _get_file_contents_to_process(pattern, recursive)
+    if not files_to_process or len(files_to_process) == 0:
+        click.echo(f"No files found for path/pattern/directory: {pattern}")
         return
 
     if not all(check_file_staged_status(f, force) for f in files_to_process):
         return
 
     click.echo(f"The following files will be processed: {[f.name for f in files_to_process]}")
     if not click.confirm("Do you want to continue?", default=True):
```

### Comparing `gptask_cli-0.1.9/gptask_cli/conf.py` & `gptask_cli-0.2.0/gptask_cli/conf.py`

 * *Files identical despite different names*

### Comparing `gptask_cli-0.1.9/gptask_cli/git_checker.py` & `gptask_cli-0.2.0/gptask_cli/git_checker.py`

 * *Files identical despite different names*

### Comparing `gptask_cli-0.1.9/gptask_cli/openai_gptask.py` & `gptask_cli-0.2.0/gptask_cli/openai_gptask.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,10 +34,10 @@
                 'role': 'assistant',
                 'content': assistant_helper_prompt
             }
         ],
         temperature=0.0,
     )
     
-    res: str= response.choices[0].message.content
+    res: str= response.choices[0].message.content # type: ignore
     res.replace(seperator, '')
     return res
```

