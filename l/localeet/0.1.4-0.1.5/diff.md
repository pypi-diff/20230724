# Comparing `tmp/localeet-0.1.4.tar.gz` & `tmp/localeet-0.1.5.tar.gz`

## Comparing `localeet-0.1.4.tar` & `localeet-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 localeet-0.1.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 localeet-0.1.4/README.md
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 localeet-0.1.4/.github/workflows/pr.yml
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 localeet-0.1.4/.github/workflows/pypi.yaml
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 localeet-0.1.4/src/localeet/__init__.py
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 localeet-0.1.4/src/localeet/__main__.py
--rw-r--r--   0        0        0     7040 2020-02-02 00:00:00.000000 localeet-0.1.4/src/localeet/get_leetcode_problem.py
--rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 localeet-0.1.4/src/localeet/language_maps.py
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 localeet-0.1.4/tests/conftest.py
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 localeet-0.1.4/tests/get_leetcode_problem_test.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 localeet-0.1.4/tests/version_number_test.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 localeet-0.1.4/tests/data/two_sum.go
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 localeet-0.1.4/tests/data/two_sum.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 localeet-0.1.4/tests/data/two_sum.rs
--rw-r--r--   0        0        0    20244 2020-02-02 00:00:00.000000 localeet-0.1.4/tests/data/two_sum_details.json
--rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 localeet-0.1.4/tests/data/two_sum_essentials.json
--rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 localeet-0.1.4/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 localeet-0.1.4/LICENSE
--rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 localeet-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 localeet-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 localeet-0.1.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 localeet-0.1.5/README.md
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 localeet-0.1.5/.github/workflows/pr.yml
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 localeet-0.1.5/.github/workflows/pypi.yaml
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 localeet-0.1.5/src/localeet/__init__.py
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 localeet-0.1.5/src/localeet/__main__.py
+-rw-r--r--   0        0        0     7040 2020-02-02 00:00:00.000000 localeet-0.1.5/src/localeet/get_leetcode_problem.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 localeet-0.1.5/src/localeet/get_version.py
+-rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 localeet-0.1.5/src/localeet/language_maps.py
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 localeet-0.1.5/tests/conftest.py
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 localeet-0.1.5/tests/get_leetcode_problem_test.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 localeet-0.1.5/tests/version_number_test.py
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 localeet-0.1.5/tests/data/two_sum.go
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 localeet-0.1.5/tests/data/two_sum.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 localeet-0.1.5/tests/data/two_sum.rs
+-rw-r--r--   0        0        0    20244 2020-02-02 00:00:00.000000 localeet-0.1.5/tests/data/two_sum_details.json
+-rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 localeet-0.1.5/tests/data/two_sum_essentials.json
+-rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 localeet-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 localeet-0.1.5/LICENSE
+-rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 localeet-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 localeet-0.1.5/PKG-INFO
```

### Comparing `localeet-0.1.4/.pre-commit-config.yaml` & `localeet-0.1.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `localeet-0.1.4/README.md` & `localeet-0.1.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -24,14 +24,21 @@
 Examples of output files:
 * [Python](https://github.com/dannybrown37/localeet/blob/main/tests/data/two_sum.py)
 * [Rust](https://github.com/dannybrown37/localeet/blob/main/tests/data/two_sum.rs)
 * [Go](https://github.com/dannybrown37/localeet/blob/main/tests/data/two_sum.go)
 
 ## CLI Args
 
+See the installed version of localeet with:
+
+```
+localeet --version
+localeet -v
+```
+
 Using any of these CLI args will use the output path provided, and
 create any needed directories in that path as well.
 
 ```
 localeet --output_path ~/leetcode
 localeet --path problems
 localeet -o ~/leetcode/problems/2023-7-22
@@ -96,14 +103,20 @@
 erlang
 erl
 elixir
 ex
 dart
 ```
 
+Print the manual:
+
+```
+localeet --help
+```
+
 ## overriding defaults
 
 If you want to set a different default value permanently, set it in your
 environment like in these examples:
 
 ```
 export LOCALEET_DEFAULT_MAX_DIFFICULTY=medium
```

### Comparing `localeet-0.1.4/.github/workflows/pr.yml` & `localeet-0.1.5/.github/workflows/pr.yml`

 * *Files identical despite different names*

### Comparing `localeet-0.1.4/src/localeet/__main__.py` & `localeet-0.1.5/src/localeet/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """
 Entry point for CLI. Define and parse CLI arguments.
 """
 from os import environ as env
 from pathlib import Path
+from typing import Optional
 
 import click
 
 from localeet.get_leetcode_problem import run
+from localeet.get_version import get_version
 from localeet.language_maps import LANGUAGE_TO_EXTENSION
 
 
 DIFFICULTY_MAP = {
     'easy': 1,
     'medium': 2,
     'hard': 3,
@@ -46,22 +48,30 @@
     default=env.get('LOCALEET_DEFAULT_CODE_EDITOR_OPEN_COMMAND', 'code'),
 )
 @click.option(
     '--programming_language', '--language', '-l',
     help='The programming language you want to use for your output file',
     default=env.get('LOCALEET_DEFAULT_LANGUAGE', 'python3'),
 )
+@click.option(
+    '--version', '-v',
+    help='Print the current version of localeet',
+    is_flag=True,
+)
 def main(
         max_difficulty: str,
         min_difficulty: str,
         output_path: str,
         code_editor_open_command: str,
         programming_language: str,
-    ) -> None:
+        version: bool,
+    ) -> Optional[str]:
     """Entry point for CLI. Parse CLI arguments."""
+    if version:
+        return get_version()
 
     max_difficulty = DIFFICULTY_MAP.get(max_difficulty)
     min_difficulty = DIFFICULTY_MAP.get(min_difficulty)
 
     output_path = Path(output_path)
 
     language = programming_language.lower()
@@ -76,7 +86,8 @@
     run(
         max_difficulty,
         min_difficulty,
         output_path,
         code_editor_open_command,
         language,
     )
+    return None
```

### Comparing `localeet-0.1.4/src/localeet/get_leetcode_problem.py` & `localeet-0.1.5/src/localeet/get_leetcode_problem.py`

 * *Files identical despite different names*

### Comparing `localeet-0.1.4/src/localeet/language_maps.py` & `localeet-0.1.5/src/localeet/language_maps.py`

 * *Files identical despite different names*

### Comparing `localeet-0.1.4/tests/conftest.py` & `localeet-0.1.5/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,24 @@
 
 @pytest.fixture(scope='session')
 def any_str() -> MockValue:
     return MockValue('STR', str)
 
 
 @pytest.fixture(scope='session')
+def any_version() -> MockValue:
+    parts_in_semantic_version = 3
+    return MockValue(
+        'VERSION_NUMBER',
+        str,
+        lambda x: len(x.split('.')) == parts_in_semantic_version,
+    )
+
+
+@pytest.fixture(scope='session')
 def any_json_str() -> MockValue:
     return MockValue('JSON_STR', str, lambda x: json.loads(x))
 
 
 @pytest.fixture(scope='session')
 def two_sum_details_json() -> dict:
     with Path('tests/data/two_sum_details.json').open() as f:
```

### Comparing `localeet-0.1.4/tests/get_leetcode_problem_test.py` & `localeet-0.1.5/tests/get_leetcode_problem_test.py`

 * *Files identical despite different names*

### Comparing `localeet-0.1.4/tests/version_number_test.py` & `localeet-0.1.5/tests/version_number_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 from os import environ as env
 from pathlib import Path
 
 import pytest
 import requests
 
 import localeet
+from localeet.get_version import get_version
+
+from conftest import MockValue
+
 
 RUNNING_LOCALLY = env.get('CI') is None and env.get('PRE_COMMIT') is None
 SKIP_REASON = """
 Version number must be updated prior to deploying a
 new version to PyPI. Run this test when committing
 new code and in CI, but don't run on a simple call
 of `pytest tests`, as tests should pass by default
@@ -29,14 +33,18 @@
     # add local repo to path to ensure we get local version
     project_dir = Path(__file__).resolve().parent
     sys.path.insert(0, str(project_dir))
     importlib.reload(localeet)
     assert localeet.__version__ > pypi_version
 
 
+def test_get_version(any_version: MockValue) -> None:
+    assert get_version() == any_version
+
+
 def get_pypi_version() -> str:
     """Return latest localeet version published to PyPI"""
     try:
         pypi_url = 'https://pypi.org/pypi/localeet/json'
         response = requests.get(pypi_url, timeout=5)
         response.raise_for_status()
         data = response.json()
```

### Comparing `localeet-0.1.4/tests/data/two_sum.go` & `localeet-0.1.5/tests/data/two_sum.go`

 * *Files identical despite different names*

### Comparing `localeet-0.1.4/tests/data/two_sum.py` & `localeet-0.1.5/tests/data/two_sum.py`

 * *Files identical despite different names*

### Comparing `localeet-0.1.4/tests/data/two_sum.rs` & `localeet-0.1.5/tests/data/two_sum.rs`

 * *Files identical despite different names*

### Comparing `localeet-0.1.4/tests/data/two_sum_details.json` & `localeet-0.1.5/tests/data/two_sum_details.json`

 * *Files identical despite different names*

### Comparing `localeet-0.1.4/tests/data/two_sum_essentials.json` & `localeet-0.1.5/tests/data/two_sum_essentials.json`

 * *Files identical despite different names*

### Comparing `localeet-0.1.4/.gitignore` & `localeet-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `localeet-0.1.4/LICENSE` & `localeet-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `localeet-0.1.4/pyproject.toml` & `localeet-0.1.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -104,7 +104,11 @@
 inline-quotes = "single"
 
 [tool.ruff.per-file-ignores]
 "tests/get_leetcode_problem_test.py" = [
   "ANN001",  # no fixture annotations
   "ANN201",  # no return annotatons for test functions
 ]
+"src/localeet/__main__.py" = [
+  "PLR0913",  # CLI has lots of options and thus needs lots of args
+  "FBT001",  # boolean flags are cool
+]
```

### Comparing `localeet-0.1.4/PKG-INFO` & `localeet-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localeet
-Version: 0.1.4
+Version: 0.1.5
 Summary: A CLI tool to do LeetCode and LeetCode-like exercises
 Author-email: Danny Brown <dannybrown37@gmail.com>
 License-File: LICENSE
 Requires-Dist: bs4
 Requires-Dist: click
 Requires-Dist: lxml
 Requires-Dist: requests
```

