# Comparing `tmp/zshgpt-0.3.3.tar.gz` & `tmp/zshgpt-0.3.6.tar.gz`

## Comparing `zshgpt-0.3.3.tar` & `zshgpt-0.3.6.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 zshgpt-0.3.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0    81149 2020-02-02 00:00:00.000000 zshgpt-0.3.3/Peek 2023-07-17 17-27.gif
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 zshgpt-0.3.3/cicd_plan.md
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 zshgpt-0.3.3/.github/workflows/buildtagdebug.yml
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 zshgpt-0.3.3/.github/workflows/release.yml
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 zshgpt-0.3.3/.github/workflows/test.yml
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 zshgpt-0.3.3/snap/snapcraft.yaml
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 zshgpt-0.3.3/src/zshgpt/__about__.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zshgpt-0.3.3/src/zshgpt/__init__.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 zshgpt-0.3.3/src/zshgpt/__main__.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 zshgpt-0.3.3/src/zshgpt/cli/__init__.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 zshgpt-0.3.3/src/zshgpt/cli/messages.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zshgpt-0.3.3/tests/__init__.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 zshgpt-0.3.3/tests/test_main.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 zshgpt-0.3.3/zsh_plugin/zsh_plugin.zsh
--rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 zshgpt-0.3.3/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 zshgpt-0.3.3/LICENSE.txt
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 zshgpt-0.3.3/README.md
--rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 zshgpt-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     3430 2020-02-02 00:00:00.000000 zshgpt-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 zshgpt-0.3.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    81149 2020-02-02 00:00:00.000000 zshgpt-0.3.6/Peek 2023-07-17 17-27.gif
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 zshgpt-0.3.6/cicd_plan.md
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 zshgpt-0.3.6/.github/workflows/release.yml
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 zshgpt-0.3.6/.github/workflows/test.yml
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 zshgpt-0.3.6/snap/snapcraft.yaml
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 zshgpt-0.3.6/src/zshgpt/__about__.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zshgpt-0.3.6/src/zshgpt/__init__.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 zshgpt-0.3.6/src/zshgpt/__main__.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 zshgpt-0.3.6/src/zshgpt/cli/__init__.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 zshgpt-0.3.6/src/zshgpt/cli/messages.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zshgpt-0.3.6/tests/__init__.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 zshgpt-0.3.6/tests/test_main.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 zshgpt-0.3.6/zsh_plugin/zsh_plugin.zsh
+-rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 zshgpt-0.3.6/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 zshgpt-0.3.6/LICENSE.txt
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 zshgpt-0.3.6/README.md
+-rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 zshgpt-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     3430 2020-02-02 00:00:00.000000 zshgpt-0.3.6/PKG-INFO
```

### Comparing `zshgpt-0.3.3/Peek 2023-07-17 17-27.gif` & `zshgpt-0.3.6/Peek 2023-07-17 17-27.gif`

 * *Files identical despite different names*

### Comparing `zshgpt-0.3.3/.github/workflows/test.yml` & `zshgpt-0.3.6/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `zshgpt-0.3.3/src/zshgpt/cli/__init__.py` & `zshgpt-0.3.6/src/zshgpt/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `zshgpt-0.3.3/src/zshgpt/cli/messages.py` & `zshgpt-0.3.6/src/zshgpt/cli/messages.py`

 * *Files identical despite different names*

### Comparing `zshgpt-0.3.3/zsh_plugin/zsh_plugin.zsh` & `zshgpt-0.3.6/zsh_plugin/zsh_plugin.zsh`

 * *Files identical despite different names*

### Comparing `zshgpt-0.3.3/.gitignore` & `zshgpt-0.3.6/.gitignore`

 * *Files identical despite different names*

### Comparing `zshgpt-0.3.3/LICENSE.txt` & `zshgpt-0.3.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zshgpt-0.3.3/README.md` & `zshgpt-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `zshgpt-0.3.3/pyproject.toml` & `zshgpt-0.3.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zshgpt-0.3.3/PKG-INFO` & `zshgpt-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zshgpt
-Version: 0.3.3
+Version: 0.3.6
 Summary: Level up z shell with GPT
 Project-URL: Documentation, https://github.com/unknown/zshgpt#readme
 Project-URL: Issues, https://github.com/unknown/zshgpt/issues
 Project-URL: Source, https://github.com/unknown/zshgpt
 Author-email: Anders Steen <anders.steen@knowit.no>
 License-Expression: MIT
 License-File: LICENSE.txt
```

