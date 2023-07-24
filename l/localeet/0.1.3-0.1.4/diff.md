# Comparing `tmp/localeet-0.1.3.tar.gz` & `tmp/localeet-0.1.4.tar.gz`

## Comparing `localeet-0.1.3.tar` & `localeet-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 localeet-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 localeet-0.1.3/README.md
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 localeet-0.1.3/.github/workflows/pr.yml
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 localeet-0.1.3/.github/workflows/pypi.yaml
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 localeet-0.1.3/src/localeet/__init__.py
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 localeet-0.1.3/src/localeet/__main__.py
--rw-r--r--   0        0        0     6777 2020-02-02 00:00:00.000000 localeet-0.1.3/src/localeet/get_leetcode_problem.py
--rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 localeet-0.1.3/src/localeet/language_maps.py
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 localeet-0.1.3/tests/conftest.py
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 localeet-0.1.3/tests/get_leetcode_problem_test.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 localeet-0.1.3/tests/version_number_test.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 localeet-0.1.3/tests/data/two_sum.go
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 localeet-0.1.3/tests/data/two_sum.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 localeet-0.1.3/tests/data/two_sum.rs
--rw-r--r--   0        0        0    20244 2020-02-02 00:00:00.000000 localeet-0.1.3/tests/data/two_sum_details.json
--rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 localeet-0.1.3/tests/data/two_sum_essentials.json
--rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 localeet-0.1.3/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 localeet-0.1.3/LICENSE
--rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 localeet-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 localeet-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 localeet-0.1.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 localeet-0.1.4/README.md
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 localeet-0.1.4/.github/workflows/pr.yml
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 localeet-0.1.4/.github/workflows/pypi.yaml
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 localeet-0.1.4/src/localeet/__init__.py
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 localeet-0.1.4/src/localeet/__main__.py
+-rw-r--r--   0        0        0     7040 2020-02-02 00:00:00.000000 localeet-0.1.4/src/localeet/get_leetcode_problem.py
+-rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 localeet-0.1.4/src/localeet/language_maps.py
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 localeet-0.1.4/tests/conftest.py
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 localeet-0.1.4/tests/get_leetcode_problem_test.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 localeet-0.1.4/tests/version_number_test.py
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 localeet-0.1.4/tests/data/two_sum.go
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 localeet-0.1.4/tests/data/two_sum.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 localeet-0.1.4/tests/data/two_sum.rs
+-rw-r--r--   0        0        0    20244 2020-02-02 00:00:00.000000 localeet-0.1.4/tests/data/two_sum_details.json
+-rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 localeet-0.1.4/tests/data/two_sum_essentials.json
+-rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 localeet-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 localeet-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 localeet-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 localeet-0.1.4/PKG-INFO
```

### Comparing `localeet-0.1.3/.pre-commit-config.yaml` & `localeet-0.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `localeet-0.1.3/README.md` & `localeet-0.1.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -17,14 +17,21 @@
 
 This will find a random question from LeetCode's free question set.
 It will create a code file shell (Python by default) with the question
 description and other metadata in it in your current working directory.
 It will then pop open a code editor (VSCode by default) with the new
 file opened in it.
 
+Examples of output files:
+* [Python](https://github.com/dannybrown37/localeet/blob/main/tests/data/two_sum.py)
+* [Rust](https://github.com/dannybrown37/localeet/blob/main/tests/data/two_sum.rs)
+* [Go](https://github.com/dannybrown37/localeet/blob/main/tests/data/two_sum.go)
+
+## CLI Args
+
 Using any of these CLI args will use the output path provided, and
 create any needed directories in that path as well.
 
 ```
 localeet --output_path ~/leetcode
 localeet --path problems
 localeet -o ~/leetcode/problems/2023-7-22
```

### Comparing `localeet-0.1.3/.github/workflows/pr.yml` & `localeet-0.1.4/.github/workflows/pr.yml`

 * *Files identical despite different names*

### Comparing `localeet-0.1.3/.github/workflows/pypi.yaml` & `localeet-0.1.4/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `localeet-0.1.3/src/localeet/__main__.py` & `localeet-0.1.4/src/localeet/__main__.py`

 * *Files identical despite different names*

### Comparing `localeet-0.1.3/src/localeet/get_leetcode_problem.py` & `localeet-0.1.4/src/localeet/get_leetcode_problem.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 parameters and then output a local Python file to work on
 said question.
 """
 
 import random
 import re
 import subprocess
+import textwrap
 from pathlib import Path
 from typing import Literal
 
 import requests
 from bs4 import BeautifulSoup
 
 from localeet.language_maps import (
@@ -156,16 +157,23 @@
     output_path.mkdir(parents=True, exist_ok=True)
     regex = r'[-\s]+'  # replace spaces and hyphens with underscores
     file_name = f'{re.sub(regex, "_", title.lower())}.{extension}'
     output_path = output_path / file_name
     header = f'{oc}\n{qid} - {difficulty} - {title}\n\n{question}\n{cc}\n\n'
     content = header + snippet + f'\n{lc} Example test case:\n'
     content += '\n'.join([f'{lc} {d}' for d in test_case.split('\n')])
-    content = '\n'.join([c.rstrip() for c in content.split('\n')])
-    content += '\n'
+    content = [c.rstrip() for c in content.split('\n')]
+    wrapped_content = []
+    for s in content:
+        if not s.strip():
+            wrapped_content.append('')
+            continue
+        wrapped_lines = textwrap.wrap(s, width=79)
+        wrapped_content.extend(wrapped_lines)
+    content = '\n'.join(wrapped_content) + '\n'
     with output_path.open('w') as f:
         f.write(content)
     return str(output_path)
 
 
 def open_code_editor(command: str, file_path: str) -> None:
     subprocess.run([command, file_path])  # noqa: S603
```

### Comparing `localeet-0.1.3/src/localeet/language_maps.py` & `localeet-0.1.4/src/localeet/language_maps.py`

 * *Files identical despite different names*

### Comparing `localeet-0.1.3/tests/conftest.py` & `localeet-0.1.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `localeet-0.1.3/tests/get_leetcode_problem_test.py` & `localeet-0.1.4/tests/get_leetcode_problem_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,24 +63,26 @@
     test_results = get_question_data('two-sum')
     try:
         assert test_results == two_sum_details_json
     except AssertionError:
         print('Saving details.json to compare differences')
         with Path('details.json').open('w') as f:
             json.dump(test_results, f, indent=4)
+        raise
 
 
 def test_parse_question_details(two_sum_details_json, two_sum_essentials):
     test_results = parse_question_details(two_sum_details_json)
     try:
         assert test_results  == two_sum_essentials
     except AssertionError:
         print('Saving essentials.json to compare differences')
         with Path('essentials.json').open('w') as f:
             json.dump(test_results, f, indent=4)
+        raise
 
 
 @pytest.mark.parametrize('language', ['python', 'rust', 'golang'])
 def test_output_python_file(
         two_sum_essentials,
         language,
     ):
@@ -94,9 +96,10 @@
     with new_file.open() as f:
         new_file_contents = f.read()
     try:
         assert output_path == file_name
         assert new_file_contents == expected
     except AssertionError:
         print(f'Saving {file_name} to compare differences')
+        raise
     else:
         new_file.unlink()
```

### Comparing `localeet-0.1.3/tests/version_number_test.py` & `localeet-0.1.4/tests/version_number_test.py`

 * *Files identical despite different names*

### Comparing `localeet-0.1.3/tests/data/two_sum.go` & `localeet-0.1.4/tests/data/two_sum.go`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 /*
 1 - Easy - Two Sum
 
-Given an array of integers `nums` and an integer `target`, return indices of the two numbers such that they add up to `target`.
-You may assume that each input would have exactly one solution, and you may not use the same element twice.
+Given an array of integers `nums` and an integer `target`, return indices of
+the two numbers such that they add up to `target`.
+You may assume that each input would have exactly one solution, and you may not
+use the same element twice.
 You can return the answer in any order.
 
 Example 1:
 
 Input: nums = [2,7,11,15], target = 9
 Output: [0,1]
 Explanation: Because nums[0] + nums[1] == 9, we return [0, 1].
@@ -26,15 +28,16 @@
 
 `2 <= nums.length <= 104`
 `-109 <= nums[i] <= 109`
 `-109 <= target <= 109`
 Only one valid answer exists.
 
 
-Follow-up: Can you come up with an algorithm that is less than `O(n2) `time complexity?
+Follow-up: Can you come up with an algorithm that is less than `O(n2) `time
+complexity?
 */
 
 func twoSum(nums []int, target int) []int {
 
 }
 // Example test case:
 // [2,7,11,15]
```

### Comparing `localeet-0.1.3/tests/data/two_sum.py` & `localeet-0.1.4/tests/data/two_sum.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """
 1 - Easy - Two Sum
 
-Given an array of integers `nums` and an integer `target`, return indices of the two numbers such that they add up to `target`.
-You may assume that each input would have exactly one solution, and you may not use the same element twice.
+Given an array of integers `nums` and an integer `target`, return indices of
+the two numbers such that they add up to `target`.
+You may assume that each input would have exactly one solution, and you may not
+use the same element twice.
 You can return the answer in any order.
 
 Example 1:
 
 Input: nums = [2,7,11,15], target = 9
 Output: [0,1]
 Explanation: Because nums[0] + nums[1] == 9, we return [0, 1].
@@ -26,15 +28,16 @@
 
 `2 <= nums.length <= 104`
 `-109 <= nums[i] <= 109`
 `-109 <= target <= 109`
 Only one valid answer exists.
 
 
-Follow-up: Can you come up with an algorithm that is less than `O(n2) `time complexity?
+Follow-up: Can you come up with an algorithm that is less than `O(n2) `time
+complexity?
 """
 
 class Solution(object):
     def twoSum(self, nums, target):
         """
         :type nums: List[int]
         :type target: int
```

### Comparing `localeet-0.1.3/tests/data/two_sum.rs` & `localeet-0.1.4/tests/data/two_sum.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 /*
 1 - Easy - Two Sum
 
-Given an array of integers `nums` and an integer `target`, return indices of the two numbers such that they add up to `target`.
-You may assume that each input would have exactly one solution, and you may not use the same element twice.
+Given an array of integers `nums` and an integer `target`, return indices of
+the two numbers such that they add up to `target`.
+You may assume that each input would have exactly one solution, and you may not
+use the same element twice.
 You can return the answer in any order.
 
 Example 1:
 
 Input: nums = [2,7,11,15], target = 9
 Output: [0,1]
 Explanation: Because nums[0] + nums[1] == 9, we return [0, 1].
@@ -26,15 +28,16 @@
 
 `2 <= nums.length <= 104`
 `-109 <= nums[i] <= 109`
 `-109 <= target <= 109`
 Only one valid answer exists.
 
 
-Follow-up: Can you come up with an algorithm that is less than `O(n2) `time complexity?
+Follow-up: Can you come up with an algorithm that is less than `O(n2) `time
+complexity?
 */
 
 impl Solution {
     pub fn two_sum(nums: Vec<i32>, target: i32) -> Vec<i32> {
 
     }
 }
```

### Comparing `localeet-0.1.3/tests/data/two_sum_details.json` & `localeet-0.1.4/tests/data/two_sum_details.json`

 * *Files identical despite different names*

### Comparing `localeet-0.1.3/tests/data/two_sum_essentials.json` & `localeet-0.1.4/tests/data/two_sum_essentials.json`

 * *Files identical despite different names*

### Comparing `localeet-0.1.3/.gitignore` & `localeet-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `localeet-0.1.3/LICENSE` & `localeet-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `localeet-0.1.3/pyproject.toml` & `localeet-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `localeet-0.1.3/PKG-INFO` & `localeet-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localeet
-Version: 0.1.3
+Version: 0.1.4
 Summary: A CLI tool to do LeetCode and LeetCode-like exercises
 Author-email: Danny Brown <dannybrown37@gmail.com>
 License-File: LICENSE
 Requires-Dist: bs4
 Requires-Dist: click
 Requires-Dist: lxml
 Requires-Dist: requests
```

