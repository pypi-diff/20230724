# Comparing `tmp/zshgpt-0.3.0.tar.gz` & `tmp/zshgpt-0.3.3.tar.gz`

## Comparing `zshgpt-0.3.0.tar` & `zshgpt-0.3.3.tar`

### file list

```diff
@@ -1,17 +1,20 @@
--rw-r--r--   0        0        0    81149 2020-02-02 00:00:00.000000 zshgpt-0.3.0/Peek 2023-07-17 17-27.gif
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 zshgpt-0.3.0/cicd_plan.md
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 zshgpt-0.3.0/.github/workflows/release.yml
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 zshgpt-0.3.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 zshgpt-0.3.0/src/zshgpt/__about__.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zshgpt-0.3.0/src/zshgpt/__init__.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 zshgpt-0.3.0/src/zshgpt/__main__.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 zshgpt-0.3.0/src/zshgpt/cli/__init__.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 zshgpt-0.3.0/src/zshgpt/cli/messages.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zshgpt-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 zshgpt-0.3.0/tests/test_main.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 zshgpt-0.3.0/zsh_plugin/zsh_plugin.zsh
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 zshgpt-0.3.0/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 zshgpt-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 zshgpt-0.3.0/README.md
--rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 zshgpt-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 zshgpt-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 zshgpt-0.3.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    81149 2020-02-02 00:00:00.000000 zshgpt-0.3.3/Peek 2023-07-17 17-27.gif
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 zshgpt-0.3.3/cicd_plan.md
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 zshgpt-0.3.3/.github/workflows/buildtagdebug.yml
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 zshgpt-0.3.3/.github/workflows/release.yml
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 zshgpt-0.3.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 zshgpt-0.3.3/snap/snapcraft.yaml
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 zshgpt-0.3.3/src/zshgpt/__about__.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zshgpt-0.3.3/src/zshgpt/__init__.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 zshgpt-0.3.3/src/zshgpt/__main__.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 zshgpt-0.3.3/src/zshgpt/cli/__init__.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 zshgpt-0.3.3/src/zshgpt/cli/messages.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zshgpt-0.3.3/tests/__init__.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 zshgpt-0.3.3/tests/test_main.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 zshgpt-0.3.3/zsh_plugin/zsh_plugin.zsh
+-rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 zshgpt-0.3.3/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 zshgpt-0.3.3/LICENSE.txt
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 zshgpt-0.3.3/README.md
+-rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 zshgpt-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     3430 2020-02-02 00:00:00.000000 zshgpt-0.3.3/PKG-INFO
```

### Comparing `zshgpt-0.3.0/Peek 2023-07-17 17-27.gif` & `zshgpt-0.3.3/Peek 2023-07-17 17-27.gif`

 * *Files identical despite different names*

### Comparing `zshgpt-0.3.0/.github/workflows/release.yml` & `zshgpt-0.3.3/.github/workflows/buildtagdebug.yml`

 * *Files 22% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 permissions:
   contents: write
   pull-requests: read
 
 on:
   push:
-    branches:
-      - 'main'
-      - 'releases/**'
+    tags:
+      - '*'
+
 
 env:
   SERVER: production
 
 
 jobs:
   run:
@@ -26,25 +26,15 @@
       uses: actions/setup-python@v4
       with:
         python-version: 3.11
 
     - name: Install Hatch
       run: pip install --upgrade hatch
 
-    - name: Bump version
-      run: hatch version minor
-
-    - name: Commit version bumb
-      run: |
-          git config user.name github-actions
-          git config user.email github-actions@github.com
-          git commit -am "Automatic minor version bump"
-          git push
-    
     - name: build
       run: hatch build
-    
-    - name: publish
+
+    - name: publish-dummy
       env:
         HATCH_INDEX_USER: __token__
         HATCH_INDEX_AUTH: ${{ secrets.PYPI_TOKEN }}
-      run: hatch publish
+      run: hatch version
```

### Comparing `zshgpt-0.3.0/.github/workflows/test.yml` & `zshgpt-0.3.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `zshgpt-0.3.0/src/zshgpt/cli/__init__.py` & `zshgpt-0.3.3/src/zshgpt/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `zshgpt-0.3.0/src/zshgpt/cli/messages.py` & `zshgpt-0.3.3/src/zshgpt/cli/messages.py`

 * *Files identical despite different names*

### Comparing `zshgpt-0.3.0/zsh_plugin/zsh_plugin.zsh` & `zshgpt-0.3.3/zsh_plugin/zsh_plugin.zsh`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/bin/zsh
 
-# This ZSH plugin reads the text from the current buffer 
+# This ZSH plugin reads the text from the current buffer
 # and uses a Python script to complete the text.
 
 create_completion() {
     # Get the text typed until now.
     text=${BUFFER}
     completion=$(zshgpt $text )
     # Add completion to the current buffer.
@@ -13,8 +13,8 @@
     CURSOR=${#BUFFER}
 }
 
 # Bind the create_completion function to a key.
 zle -N create_completion
 
 setopt interactivecomments
-bindkey '^G' create_completion
+bindkey '^G' create_completion
```

### Comparing `zshgpt-0.3.0/.gitignore` & `zshgpt-0.3.3/.gitignore`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,18 @@
-.ruff_cache/
+#Editor settings
 .vscode/
 
+#Autgenerated __about__ file
+src/zshgpt/__about__.py
+
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
+.ruff_cache/
 
 # C extensions
 *.so
 
 # Distribution / packaging
 .Python
 build/
@@ -23,14 +27,15 @@
 sdist/
 var/
 wheels/
 share/python-wheels/
 *.egg-info/
 .installed.cfg
 *.egg
+*.snap
 MANIFEST
 
 # PyInstaller
 #  Usually these files are written by a python script from a template
 #  before PyInstaller builds the exe, so as to inject date/other infos into it.
 *.manifest
 *.spec
```

### Comparing `zshgpt-0.3.0/LICENSE.txt` & `zshgpt-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zshgpt-0.3.0/README.md` & `zshgpt-0.3.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 Hit `enter` to execute or `ctrl+c` to deny.
 
 If asked a question that will not resolve in a command, GPT is instructed to use `#`.
 
 ```bash
 # Who was Norways first prime minister?
 # Norway's first prime minister was Frederik Stang, serving from 1873 to 1880.
-``` 
+```
 
 ## Prerequisite
 * Python >= 3.7
 * ZSH + Oh-my-zsh
 * Valid Openai API-key
     * make sure to save under `OPENAI_API_KEY` env.
     * `export OPENAI_API_KEY='sk-...'`
```

### Comparing `zshgpt-0.3.0/pyproject.toml` & `zshgpt-0.3.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["hatchling"]
+requires = ["hatchling", "hatch-vcs"]
 build-backend = "hatchling.build"
 
 [project]
 name = "zshgpt"
 dynamic = ["version"]
 description = 'Level up z shell with GPT'
 readme = "README.md"
@@ -36,14 +36,15 @@
 [project.scripts]
 zshgpt = "zshgpt.cli:zshgpt"
 
 [tool.hatch.envs.default]
 dependencies = [
   "coverage[toml]>=6.5",
   "pytest",
+  "pre-commit"
 ]
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = [
   "- coverage combine",
   "coverage report",
@@ -52,28 +53,32 @@
   "test-cov",
   "cov-report",
 ]
 
 [[tool.hatch.envs.all.matrix]]
 python = ["3.7", "3.8", "3.9", "3.10", "3.11"]
 
+
+[tool.hatch.version]
+# path = "src/zshgpt/__about__.py"
+source = "vcs"
+
+[tool.hatch.build.hooks.vcs]
+version-file = "src/zshgpt/__about__.py"
+
+[tool.hatch.build.targets.app]
+
+
 [tool.hatch.envs.lint]
 detached = true
 dependencies = [
   "black>=23.1.0",
   "mypy>=1.0.0",
   "ruff>=0.0.243",
 ]
-
-[tool.hatch.version]
-path = "src/zshgpt/__about__.py"
-
-[tool.hatch.build.targets.app]
-
-
 [tool.hatch.envs.lint.scripts]
 typing = "mypy --install-types --non-interactive {args:src/zshgpt tests}"
 style = [
   "ruff {args:.}",
   "black --check --diff {args:.}",
 ]
 fmt = [
```

### Comparing `zshgpt-0.3.0/PKG-INFO` & `zshgpt-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zshgpt
-Version: 0.3.0
+Version: 0.3.3
 Summary: Level up z shell with GPT
 Project-URL: Documentation, https://github.com/unknown/zshgpt#readme
 Project-URL: Issues, https://github.com/unknown/zshgpt/issues
 Project-URL: Source, https://github.com/unknown/zshgpt
 Author-email: Anders Steen <anders.steen@knowit.no>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -54,15 +54,15 @@
 Hit `enter` to execute or `ctrl+c` to deny.
 
 If asked a question that will not resolve in a command, GPT is instructed to use `#`.
 
 ```bash
 # Who was Norways first prime minister?
 # Norway's first prime minister was Frederik Stang, serving from 1873 to 1880.
-``` 
+```
 
 ## Prerequisite
 * Python >= 3.7
 * ZSH + Oh-my-zsh
 * Valid Openai API-key
     * make sure to save under `OPENAI_API_KEY` env.
     * `export OPENAI_API_KEY='sk-...'`
```

