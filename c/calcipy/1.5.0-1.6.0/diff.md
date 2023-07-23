# Comparing `tmp/calcipy-1.5.0.tar.gz` & `tmp/calcipy-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calcipy-1.5.0.tar", max compression
+gzip compressed data, was "calcipy-1.6.0.tar", max compression
```

## Comparing `calcipy-1.5.0.tar` & `calcipy-1.6.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0     1066 2023-07-22 16:02:40.611902 calcipy-1.5.0/LICENSE
--rw-r--r--   0        0        0      167 2023-07-22 16:05:20.845888 calcipy-1.5.0/calcipy/__init__.py
--rw-r--r--   0        0        0     1241 2023-05-13 10:55:19.213121 calcipy-1.5.0/calcipy/can_skip.py
--rw-r--r--   0        0        0      175 2023-03-02 02:58:57.029784 calcipy-1.5.0/calcipy/check_for_stale_packages/__init__.py
--rw-r--r--   0        0        0     8635 2023-07-22 15:18:10.196390 calcipy-1.5.0/calcipy/check_for_stale_packages/_check_for_stale_packages.py
--rw-r--r--   0        0        0     6435 2023-07-17 03:06:34.200957 calcipy-1.5.0/calcipy/cli.py
--rw-r--r--   0        0        0      154 2023-03-02 02:58:57.946199 calcipy-1.5.0/calcipy/code_tag_collector/__init__.py
--rw-r--r--   0        0        0    11292 2023-07-22 15:18:47.182980 calcipy-1.5.0/calcipy/code_tag_collector/_collector.py
--rw-r--r--   0        0        0      140 2023-03-02 02:58:58.498973 calcipy-1.5.0/calcipy/dot_dict/__init__.py
--rw-r--r--   0        0        0      800 2023-07-22 15:18:47.183073 calcipy-1.5.0/calcipy/dot_dict/_dot_dict.py
--rw-r--r--   0        0        0        0 2023-04-05 02:28:27.975837 calcipy-1.5.0/calcipy/experiments/__init__.py
--rw-r--r--   0        0        0     1988 2023-06-18 22:07:03.089724 calcipy-1.5.0/calcipy/experiments/check_duplicate_test_names.py
--rw-r--r--   0        0        0     3294 2023-06-21 22:43:42.721881 calcipy-1.5.0/calcipy/file_search.py
--rw-r--r--   0        0        0     1858 2023-06-25 19:44:08.544986 calcipy-1.5.0/calcipy/invoke_helpers.py
--rw-r--r--   0        0        0      162 2023-03-02 02:58:58.973806 calcipy-1.5.0/calcipy/md_writer/__init__.py
--rw-r--r--   0        0        0     7789 2023-06-21 12:26:00.681287 calcipy-1.5.0/calcipy/md_writer/_writer.py
--rw-r--r--   0        0        0      162 2023-03-02 02:58:59.584964 calcipy-1.5.0/calcipy/noxfile/__init__.py
--rw-r--r--   0        0        0     6444 2023-07-07 09:54:44.784397 calcipy-1.5.0/calcipy/noxfile/_noxfile.py
--rw-r--r--   0        0        0     1418 2023-07-22 16:02:41.621754 calcipy-1.5.0/calcipy/scripts.py
--rw-r--r--   0        0        0        0 2023-02-21 03:18:10.928974 calcipy-1.5.0/calcipy/tasks/__init__.py
--rw-r--r--   0        0        0     3488 2023-05-17 11:01:15.749443 calcipy-1.5.0/calcipy/tasks/all_tasks.py
--rw-r--r--   0        0        0     2026 2023-06-25 19:43:32.341457 calcipy-1.5.0/calcipy/tasks/cl.py
--rw-r--r--   0        0        0     1197 2023-07-22 15:47:06.898958 calcipy-1.5.0/calcipy/tasks/defaults.py
--rw-r--r--   0        0        0     3676 2023-06-25 19:58:27.487137 calcipy-1.5.0/calcipy/tasks/doc.py
--rw-r--r--   0        0        0     1771 2023-06-25 19:43:32.338425 calcipy-1.5.0/calcipy/tasks/executable_utils.py
--rw-r--r--   0        0        0     4334 2023-07-17 03:11:20.928724 calcipy-1.5.0/calcipy/tasks/lint.py
--rw-r--r--   0        0        0      487 2023-06-25 19:20:04.874448 calcipy-1.5.0/calcipy/tasks/nox.py
--rw-r--r--   0        0        0     1703 2023-06-25 19:43:32.341707 calcipy-1.5.0/calcipy/tasks/pack.py
--rw-r--r--   0        0        0      611 2023-06-25 19:05:50.289154 calcipy-1.5.0/calcipy/tasks/stale.py
--rw-r--r--   0        0        0     1555 2023-07-22 15:47:06.898769 calcipy-1.5.0/calcipy/tasks/tags.py
--rw-r--r--   0        0        0     3656 2023-06-25 19:15:31.479851 calcipy-1.5.0/calcipy/tasks/test.py
--rw-r--r--   0        0        0      772 2023-06-25 19:43:32.341220 calcipy-1.5.0/calcipy/tasks/types.py
--rw-r--r--   0        0        0     7709 2023-07-22 16:05:25.950920 calcipy-1.5.0/docs/README.md
--rw-r--r--   0        0        0     6578 2023-07-22 16:05:20.871206 calcipy-1.5.0/pyproject.toml
--rw-r--r--   0        0        0    12322 1970-01-01 00:00:00.000000 calcipy-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-22 19:32:47.690285 calcipy-1.6.0/LICENSE
+-rw-r--r--   0        0        0     1747 2023-07-23 22:36:25.073109 calcipy-1.6.0/calcipy/__init__.py
+-rw-r--r--   0        0        0     1241 2023-05-13 10:55:19.213121 calcipy-1.6.0/calcipy/can_skip.py
+-rw-r--r--   0        0        0      175 2023-03-02 02:58:57.029784 calcipy-1.6.0/calcipy/check_for_stale_packages/__init__.py
+-rw-r--r--   0        0        0     8635 2023-07-22 15:18:10.196390 calcipy-1.6.0/calcipy/check_for_stale_packages/_check_for_stale_packages.py
+-rw-r--r--   0        0        0     6435 2023-07-22 18:26:00.726643 calcipy-1.6.0/calcipy/cli.py
+-rw-r--r--   0        0        0      154 2023-03-02 02:58:57.946199 calcipy-1.6.0/calcipy/code_tag_collector/__init__.py
+-rw-r--r--   0        0        0    11292 2023-07-22 15:18:47.182980 calcipy-1.6.0/calcipy/code_tag_collector/_collector.py
+-rw-r--r--   0        0        0      140 2023-03-02 02:58:58.498973 calcipy-1.6.0/calcipy/dot_dict/__init__.py
+-rw-r--r--   0        0        0      800 2023-07-22 15:18:47.183073 calcipy-1.6.0/calcipy/dot_dict/_dot_dict.py
+-rw-r--r--   0        0        0        0 2023-04-05 02:28:27.975837 calcipy-1.6.0/calcipy/experiments/__init__.py
+-rw-r--r--   0        0        0     1123 2023-07-23 22:29:51.746749 calcipy-1.6.0/calcipy/experiments/bump_programmatically.py
+-rw-r--r--   0        0        0     1988 2023-06-18 22:07:03.089724 calcipy-1.6.0/calcipy/experiments/check_duplicate_test_names.py
+-rw-r--r--   0        0        0     3294 2023-06-21 22:43:42.721881 calcipy-1.6.0/calcipy/file_search.py
+-rw-r--r--   0        0        0     1858 2023-06-25 19:44:08.544986 calcipy-1.6.0/calcipy/invoke_helpers.py
+-rw-r--r--   0        0        0      162 2023-03-02 02:58:58.973806 calcipy-1.6.0/calcipy/md_writer/__init__.py
+-rw-r--r--   0        0        0     7802 2023-07-22 18:29:29.425220 calcipy-1.6.0/calcipy/md_writer/_writer.py
+-rw-r--r--   0        0        0      162 2023-03-02 02:58:59.584964 calcipy-1.6.0/calcipy/noxfile/__init__.py
+-rw-r--r--   0        0        0     6444 2023-07-07 09:54:44.784397 calcipy-1.6.0/calcipy/noxfile/_noxfile.py
+-rw-r--r--   0        0        0     1418 2023-07-22 19:32:48.891548 calcipy-1.6.0/calcipy/scripts.py
+-rw-r--r--   0        0        0        0 2023-02-21 03:18:10.928974 calcipy-1.6.0/calcipy/tasks/__init__.py
+-rw-r--r--   0        0        0     3488 2023-05-17 11:01:15.749443 calcipy-1.6.0/calcipy/tasks/all_tasks.py
+-rw-r--r--   0        0        0     2026 2023-06-25 19:43:32.341457 calcipy-1.6.0/calcipy/tasks/cl.py
+-rw-r--r--   0        0        0     1197 2023-07-22 15:47:06.898958 calcipy-1.6.0/calcipy/tasks/defaults.py
+-rw-r--r--   0        0        0     3676 2023-06-25 19:58:27.487137 calcipy-1.6.0/calcipy/tasks/doc.py
+-rw-r--r--   0        0        0     1771 2023-06-25 19:43:32.338425 calcipy-1.6.0/calcipy/tasks/executable_utils.py
+-rw-r--r--   0        0        0     4334 2023-07-17 03:11:20.928724 calcipy-1.6.0/calcipy/tasks/lint.py
+-rw-r--r--   0        0        0      487 2023-06-25 19:20:04.874448 calcipy-1.6.0/calcipy/tasks/nox.py
+-rw-r--r--   0        0        0     2719 2023-07-23 22:28:53.440756 calcipy-1.6.0/calcipy/tasks/pack.py
+-rw-r--r--   0        0        0      611 2023-06-25 19:05:50.289154 calcipy-1.6.0/calcipy/tasks/stale.py
+-rw-r--r--   0        0        0     1555 2023-07-22 15:47:06.898769 calcipy-1.6.0/calcipy/tasks/tags.py
+-rw-r--r--   0        0        0     3656 2023-06-25 19:15:31.479851 calcipy-1.6.0/calcipy/tasks/test.py
+-rw-r--r--   0        0        0      772 2023-06-25 19:43:32.341220 calcipy-1.6.0/calcipy/tasks/types.py
+-rw-r--r--   0        0        0     7709 2023-07-23 22:36:32.346503 calcipy-1.6.0/docs/README.md
+-rw-r--r--   0        0        0     6544 2023-07-23 22:36:25.128541 calcipy-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0    12318 1970-01-01 00:00:00.000000 calcipy-1.6.0/PKG-INFO
```

### Comparing `calcipy-1.5.0/LICENSE` & `calcipy-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `calcipy-1.5.0/calcipy/can_skip.py` & `calcipy-1.6.0/calcipy/can_skip.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.5.0/calcipy/check_for_stale_packages/_check_for_stale_packages.py` & `calcipy-1.6.0/calcipy/check_for_stale_packages/_check_for_stale_packages.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.5.0/calcipy/cli.py` & `calcipy-1.6.0/calcipy/cli.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.5.0/calcipy/code_tag_collector/_collector.py` & `calcipy-1.6.0/calcipy/code_tag_collector/_collector.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.5.0/calcipy/dot_dict/_dot_dict.py` & `calcipy-1.6.0/calcipy/dot_dict/_dot_dict.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.5.0/calcipy/experiments/check_duplicate_test_names.py` & `calcipy-1.6.0/calcipy/experiments/check_duplicate_test_names.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.5.0/calcipy/file_search.py` & `calcipy-1.6.0/calcipy/file_search.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.5.0/calcipy/invoke_helpers.py` & `calcipy-1.6.0/calcipy/invoke_helpers.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.5.0/calcipy/md_writer/_writer.py` & `calcipy-1.6.0/calcipy/md_writer/_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
             if len(matches) == 1:
                 try:
                     lines.extend(handler_lookup[matches[0]](line, path_file))
                 except _ParseSkipError:
                     lines.append(line)
                     self.end()
             else:
-                logger.error('Could not parse', line=line)
+                logger.warning('Could not parse. Skipping:', line=line)
                 lines.append(line)
                 self.end()
         elif self.state == self.state_user:
             lines.append(line)
         # else: discard the lines in the auto-section
         return lines
```

### Comparing `calcipy-1.5.0/calcipy/noxfile/_noxfile.py` & `calcipy-1.6.0/calcipy/noxfile/_noxfile.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.5.0/calcipy/scripts.py` & `calcipy-1.6.0/calcipy/scripts.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.5.0/calcipy/tasks/all_tasks.py` & `calcipy-1.6.0/calcipy/tasks/all_tasks.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.5.0/calcipy/tasks/cl.py` & `calcipy-1.6.0/calcipy/tasks/cl.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.5.0/calcipy/tasks/defaults.py` & `calcipy-1.6.0/calcipy/tasks/defaults.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.5.0/calcipy/tasks/doc.py` & `calcipy-1.6.0/calcipy/tasks/doc.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.5.0/calcipy/tasks/executable_utils.py` & `calcipy-1.6.0/calcipy/tasks/executable_utils.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.5.0/calcipy/tasks/lint.py` & `calcipy-1.6.0/calcipy/tasks/lint.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.5.0/calcipy/tasks/stale.py` & `calcipy-1.6.0/calcipy/tasks/stale.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.5.0/calcipy/tasks/tags.py` & `calcipy-1.6.0/calcipy/tasks/tags.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.5.0/calcipy/tasks/test.py` & `calcipy-1.6.0/calcipy/tasks/test.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.5.0/calcipy/tasks/types.py` & `calcipy-1.6.0/calcipy/tasks/types.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.5.0/docs/README.md` & `calcipy-1.6.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `calcipy-1.5.0/pyproject.toml` & `calcipy-1.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.commitizen]
-version = "1.5.0"
+version = "1.6.0"
 version_files = ["calcipy/__init__.py:^__version", "pyproject.toml:^version"]
 
 [tool.poetry]
 authors = ["Kyle King <dev.act.kyle@gmail.com>"]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Framework :: Pytest",
@@ -26,15 +26,15 @@
 include = ["LICENSE"]
 keywords = ["nox", "python-poetry"]
 license = "MIT"
 maintainers = []
 name = "calcipy"
 readme = "docs/README.md"
 repository = "https://github.com/kyleking/calcipy"
-version = "1.5.0"
+version = "1.6.0"
 
 [tool.poetry.dependencies]
 python = "^3.8.12"
 arrow = {optional = true, version = ">=1.2.3"} # tags
 autopep8 = {optional = true, version = ">=2.0.1"} # lint
 bandit = {optional = true, version = ">=1.7.4"} # lint
 beartype = ">=0.15.0"
@@ -48,22 +48,22 @@
 flake8-executable = {optional = true, version = ">=2.1.3"} # flake8
 flake8-expression-complexity = {optional = true, version = ">=0.0.11"} # flake8
 flake8-functions = {optional = true, version = ">=0.0.7"} # flake8
 flake8-pep3101 = {optional = true, version = ">=2.0.0"} # flake8
 flake8-pie = {optional = true, version = ">=0.16.0"} # flake8
 flake8-printf-formatting = {optional = true, version = ">=1.1.2"} # flake8
 flake8-raise = {optional = true, version = ">=0.0.5"} # flake8
-flake8-require-beartype = {optional = true, version = ">=0.1.1"} # flake8
 flake8-sql = {optional = true, version = ">=0.4.1"} # flake8
 flake8-string-format = {optional = true, version = ">=0.3.0"} # flake8
 flake8-super = {optional = true, version = ">=0.1.3"} # flake8
 flake8-tuple = {optional = true, version = ">=0.4.1"} # flake8
 flake8-typing-imports = {optional = true, version = ">=1.14.0"} # flake8
 flake8-use-pathlib = {optional = true, version = ">=0.3.0"} # flake8
 flake8-variables-names = {optional = true, version = ">=0.0.5"} # flake8
+griffe = ">=0.32.3" # experimental
 httpx = {optional = true, version = ">=0.24.1"} # stale
 invoke = ">=2.1.2"
 mkdocs = {optional = true, version = ">=1.4.1"} # doc
 mkdocs-build-plantuml-plugin = {optional = true, version = ">=1.7.4"} # doc
 mkdocs-gen-files = {optional = true, version = ">=0.4.0"} # doc
 mkdocs-git-revision-date-localized-plugin = {optional = true, version = ">=1.0.1"} # doc
 mkdocs-include-markdown-plugin = {markers = "python_version < '3.12'", optional = true, version = ">=4.0.3"} # doc
@@ -83,14 +83,15 @@
 pytest-cov = {optional = true, version = ">=4.0.0"} # test
 pytest-randomly = {optional = true, version = ">=3.12.0"} # test
 pytest-watcher = {optional = true, version = ">=0.2.6"} # test
 python-box = {optional = true, version = ">=6.0.2"} # ddict
 pyyaml = {optional = true, version = ">=5.2"} # doc,tags
 ruff = {optional = true, version = ">=0.0.280"} # lint
 semgrep = {optional = true, version = ">=1.12.1"} # lint
+semver = ">=3.0.1" # experimental
 tabulate = {optional = true, version = ">=0.9.0"} # tags: Required for pandas to markdown
 transitions = {optional = true, version = ">=0.9.0"} # tags: docs
 
 [tool.poetry.extras]
 ddict = ["python-box"]
 doc = [
   "commitizen",
@@ -117,15 +118,14 @@
   "flake8-executable",
   "flake8-expression-complexity",
   "flake8-functions",
   "flake8-pep3101",
   "flake8-pie",
   "flake8-printf-formatting",
   "flake8-raise",
-  "flake8-require-beartype",
   "flake8-sql",
   "flake8-string-format",
   "flake8-super",
   "flake8-tuple",
   "flake8-typing-imports",
   "flake8-use-pathlib",
   "flake8-variables-names",
```

### Comparing `calcipy-1.5.0/PKG-INFO` & `calcipy-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calcipy
-Version: 1.5.0
+Version: 1.6.0
 Summary: Python package to simplify development
 Home-page: https://github.com/kyleking/calcipy
 License: MIT
 Keywords: nox,python-poetry
 Author: Kyle King
 Author-email: dev.act.kyle@gmail.com
 Requires-Python: >=3.8.12,<4.0.0
@@ -44,22 +44,22 @@
 Requires-Dist: flake8-executable (>=2.1.3) ; extra == "flake8"
 Requires-Dist: flake8-expression-complexity (>=0.0.11) ; extra == "flake8"
 Requires-Dist: flake8-functions (>=0.0.7) ; extra == "flake8"
 Requires-Dist: flake8-pep3101 (>=2.0.0) ; extra == "flake8"
 Requires-Dist: flake8-pie (>=0.16.0) ; extra == "flake8"
 Requires-Dist: flake8-printf-formatting (>=1.1.2) ; extra == "flake8"
 Requires-Dist: flake8-raise (>=0.0.5) ; extra == "flake8"
-Requires-Dist: flake8-require-beartype (>=0.1.1) ; extra == "flake8"
 Requires-Dist: flake8-sql (>=0.4.1) ; extra == "flake8"
 Requires-Dist: flake8-string-format (>=0.3.0) ; extra == "flake8"
 Requires-Dist: flake8-super (>=0.1.3) ; extra == "flake8"
 Requires-Dist: flake8-tuple (>=0.4.1) ; extra == "flake8"
 Requires-Dist: flake8-typing-imports (>=1.14.0) ; extra == "flake8"
 Requires-Dist: flake8-use-pathlib (>=0.3.0) ; extra == "flake8"
 Requires-Dist: flake8-variables-names (>=0.0.5) ; extra == "flake8"
+Requires-Dist: griffe (>=0.32.3)
 Requires-Dist: httpx (>=0.24.1) ; extra == "stale"
 Requires-Dist: invoke (>=2.1.2)
 Requires-Dist: mkdocs (>=1.4.1) ; extra == "doc"
 Requires-Dist: mkdocs-build-plantuml-plugin (>=1.7.4) ; extra == "doc"
 Requires-Dist: mkdocs-gen-files (>=0.4.0) ; extra == "doc"
 Requires-Dist: mkdocs-git-revision-date-localized-plugin (>=1.0.1) ; extra == "doc"
 Requires-Dist: mkdocs-include-markdown-plugin (>=4.0.3) ; (python_version < "3.12") and (extra == "doc")
@@ -79,14 +79,15 @@
 Requires-Dist: pytest-cov (>=4.0.0) ; extra == "test"
 Requires-Dist: pytest-randomly (>=3.12.0) ; extra == "test"
 Requires-Dist: pytest-watcher (>=0.2.6) ; extra == "test"
 Requires-Dist: python-box (>=6.0.2) ; extra == "ddict"
 Requires-Dist: pyyaml (>=5.2) ; extra == "doc" or extra == "tags"
 Requires-Dist: ruff (>=0.0.280) ; extra == "lint"
 Requires-Dist: semgrep (>=1.12.1) ; extra == "lint"
+Requires-Dist: semver (>=3.0.1)
 Requires-Dist: tabulate (>=0.9.0) ; extra == "tags"
 Requires-Dist: transitions (>=0.9.0) ; extra == "doc"
 Project-URL: Bug Tracker, https://github.com/kyleking/calcipy/issues
 Project-URL: Changelog, https://github.com/kyleking/calcipy/blob/main/docs/docs/CHANGELOG.md
 Project-URL: Documentation, https://calcipy.kyleking.me
 Project-URL: Repository, https://github.com/kyleking/calcipy
 Description-Content-Type: text/markdown
```

