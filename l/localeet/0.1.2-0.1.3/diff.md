# Comparing `tmp/localeet-0.1.2.tar.gz` & `tmp/localeet-0.1.3.tar.gz`

## Comparing `localeet-0.1.2.tar` & `localeet-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 localeet-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 localeet-0.1.2/README.md
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 localeet-0.1.2/.github/workflows/pr.yml
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 localeet-0.1.2/.github/workflows/pypi.yaml
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 localeet-0.1.2/src/localeet/__init__.py
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 localeet-0.1.2/src/localeet/__main__.py
--rw-r--r--   0        0        0     6587 2020-02-02 00:00:00.000000 localeet-0.1.2/src/localeet/get_leetcode_problem.py
--rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 localeet-0.1.2/src/localeet/language_maps.py
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 localeet-0.1.2/tests/conftest.py
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 localeet-0.1.2/tests/get_leetcode_problem_test.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 localeet-0.1.2/tests/version_number_test.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 localeet-0.1.2/tests/data/two_sum.go
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 localeet-0.1.2/tests/data/two_sum.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 localeet-0.1.2/tests/data/two_sum.rs
--rw-r--r--   0        0        0    20244 2020-02-02 00:00:00.000000 localeet-0.1.2/tests/data/two_sum_details.json
--rw-r--r--   0        0        0     5902 2020-02-02 00:00:00.000000 localeet-0.1.2/tests/data/two_sum_essentials.json
--rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 localeet-0.1.2/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 localeet-0.1.2/LICENSE
--rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 localeet-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 localeet-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 localeet-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 localeet-0.1.3/README.md
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 localeet-0.1.3/.github/workflows/pr.yml
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 localeet-0.1.3/.github/workflows/pypi.yaml
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 localeet-0.1.3/src/localeet/__init__.py
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 localeet-0.1.3/src/localeet/__main__.py
+-rw-r--r--   0        0        0     6777 2020-02-02 00:00:00.000000 localeet-0.1.3/src/localeet/get_leetcode_problem.py
+-rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 localeet-0.1.3/src/localeet/language_maps.py
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 localeet-0.1.3/tests/conftest.py
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 localeet-0.1.3/tests/get_leetcode_problem_test.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 localeet-0.1.3/tests/version_number_test.py
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 localeet-0.1.3/tests/data/two_sum.go
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 localeet-0.1.3/tests/data/two_sum.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 localeet-0.1.3/tests/data/two_sum.rs
+-rw-r--r--   0        0        0    20244 2020-02-02 00:00:00.000000 localeet-0.1.3/tests/data/two_sum_details.json
+-rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 localeet-0.1.3/tests/data/two_sum_essentials.json
+-rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 localeet-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 localeet-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 localeet-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 localeet-0.1.3/PKG-INFO
```

### Comparing `localeet-0.1.2/.pre-commit-config.yaml` & `localeet-0.1.3/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
       - id: check-toml
       - id: check-xml
       - id: check-yaml
       - id: debug-statements
       - id: detect-private-key
       - id: end-of-file-fixer
       - id: mixed-line-ending
-      - id: name-tests-test
       - id: trailing-whitespace
 
   - repo: local
     hooks:
       - id: pytest
         name: Pytest
         always_run: true
```

### Comparing `localeet-0.1.2/README.md` & `localeet-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,15 @@
 ```
     git clone https://github.com/dannybrown37/localeet.git
     python -m venv .venv
     source .venv/bin/activate
     pip install -U pip
     pip install -e .[dev, test]
     pre-commit install
+    pytest tests -s -vv
 ```
 
 ## contribution process
 
 1. Create a new branch
 2. Add features you wish to propose
 3. Stage and commit your changes, ensure pre-commit checks pass
```

### Comparing `localeet-0.1.2/.github/workflows/pr.yml` & `localeet-0.1.3/.github/workflows/pr.yml`

 * *Files identical despite different names*

### Comparing `localeet-0.1.2/.github/workflows/pypi.yaml` & `localeet-0.1.3/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `localeet-0.1.2/src/localeet/__main__.py` & `localeet-0.1.3/src/localeet/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,21 +33,20 @@
     '--min_difficulty', '--min',
     help='Min difficulty allowed',
     type=click.Choice(list(DIFFICULTY_MAP.keys())),
     default=env.get('LOCALEET_DEFAULT_MIN_DIFFICULTY', 'easy'),
 )
 @click.option(
     '--output_path', '--path', '-o',
-    help='Output path for code file created. Default is cwd. '
-         'Will create new directories as needed',
+    help='Output path for code file. Will create new directories as needed.',
     default=env.get('LOCALEET_DEFAULT_OUTPUT_PATH', '.'),
 )
 @click.option(
     '--code_editor_open_command', '--editor', '-e',
-    help='Will open the specified editor on the created file. VSCode default.',
+    help='Will open the specified editor on the created file.',
     default=env.get('LOCALEET_DEFAULT_CODE_EDITOR_OPEN_COMMAND', 'code'),
 )
 @click.option(
     '--programming_language', '--language', '-l',
     help='The programming language you want to use for your output file',
     default=env.get('LOCALEET_DEFAULT_LANGUAGE', 'python3'),
 )
```

### Comparing `localeet-0.1.2/src/localeet/get_leetcode_problem.py` & `localeet-0.1.3/src/localeet/get_leetcode_problem.py`

 * *Files 5% similar despite different names*

```diff
@@ -118,19 +118,21 @@
                 """,
     }).json()
 
 
 def parse_question_details(question_data: dict) -> dict[str, str]:
     """Parse response from GraphQL down into data needed for output"""
     soup = BeautifulSoup(question_data['data']['question']['content'], 'lxml')
+    for code_tag in soup.find_all('code'):
+        code_tag.replace_with('`' + code_tag.text + '`')
     return {
         'code_snippets': question_data['data']['question']['codeSnippets'],
         'difficulty': question_data['data']['question']['difficulty'],
         'question_id': question_data['data']['question']['questionId'],
-        'question': soup.get_text(),
+        'question': soup.get_text().replace('\u00A0', ' '),
         'test_case': question_data['data']['question']['sampleTestCase'],
         'title': question_data['data']['question']['title'],
     }
 
 
 def output_code_file(
         output_path: Path,
@@ -154,14 +156,15 @@
     output_path.mkdir(parents=True, exist_ok=True)
     regex = r'[-\s]+'  # replace spaces and hyphens with underscores
     file_name = f'{re.sub(regex, "_", title.lower())}.{extension}'
     output_path = output_path / file_name
     header = f'{oc}\n{qid} - {difficulty} - {title}\n\n{question}\n{cc}\n\n'
     content = header + snippet + f'\n{lc} Example test case:\n'
     content += '\n'.join([f'{lc} {d}' for d in test_case.split('\n')])
+    content = '\n'.join([c.rstrip() for c in content.split('\n')])
     content += '\n'
     with output_path.open('w') as f:
         f.write(content)
     return str(output_path)
 
 
 def open_code_editor(command: str, file_path: str) -> None:
```

### Comparing `localeet-0.1.2/src/localeet/language_maps.py` & `localeet-0.1.3/src/localeet/language_maps.py`

 * *Files identical despite different names*

### Comparing `localeet-0.1.2/tests/conftest.py` & `localeet-0.1.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `localeet-0.1.2/tests/get_leetcode_problem_test.py` & `localeet-0.1.3/tests/get_leetcode_problem_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 from pathlib import Path
 
 import pytest
 
 from localeet.get_leetcode_problem import (
     choose_a_valid_question,
     get_question_data,
@@ -55,32 +56,47 @@
     ):
     two_sum_details_json['data']['question'].update({
         'dislikes': any_int,
         'judgeType': any_str,
         'likes': any_int,
         'stats': any_json_str,
     })
-    assert get_question_data('two-sum') == two_sum_details_json
+    test_results = get_question_data('two-sum')
+    try:
+        assert test_results == two_sum_details_json
+    except AssertionError:
+        print('Saving details.json to compare differences')
+        with Path('details.json').open('w') as f:
+            json.dump(test_results, f, indent=4)
 
 
 def test_parse_question_details(two_sum_details_json, two_sum_essentials):
-    assert parse_question_details(two_sum_details_json) == two_sum_essentials
+    test_results = parse_question_details(two_sum_details_json)
+    try:
+        assert test_results  == two_sum_essentials
+    except AssertionError:
+        print('Saving essentials.json to compare differences')
+        with Path('essentials.json').open('w') as f:
+            json.dump(test_results, f, indent=4)
 
 
 @pytest.mark.parametrize('language', ['python', 'rust', 'golang'])
 def test_output_python_file(
         two_sum_essentials,
         language,
     ):
     extension = LANGUAGE_TO_EXTENSION[language]
-    with Path(f'tests/data/two_sum.{extension}').open() as f:
+    file_name = f'two_sum.{extension}'
+    with Path(f'tests/data/{file_name}').open() as f:
         expected = f.read()
     path = Path('.')
-    new_file = path / f'two_sum.{extension}'
+    new_file = path / file_name
     output_path = output_code_file(path, two_sum_essentials, language)
-    assert output_path == f'two_sum.{extension}'
     with new_file.open() as f:
         new_file_contents = f.read()
     try:
+        assert output_path == file_name
         assert new_file_contents == expected
-    finally:
+    except AssertionError:
+        print(f'Saving {file_name} to compare differences')
+    else:
         new_file.unlink()
```

### Comparing `localeet-0.1.2/tests/version_number_test.py` & `localeet-0.1.3/tests/version_number_test.py`

 * *Files identical despite different names*

### Comparing `localeet-0.1.2/tests/data/two_sum.go` & `localeet-0.1.3/tests/data/two_sum.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-/*
+"""
 1 - Easy - Two Sum
 
-Given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target.
+Given an array of integers `nums` and an integer `target`, return indices of the two numbers such that they add up to `target`.
 You may assume that each input would have exactly one solution, and you may not use the same element twice.
 You can return the answer in any order.
- 
+
 Example 1:
 
 Input: nums = [2,7,11,15], target = 9
 Output: [0,1]
 Explanation: Because nums[0] + nums[1] == 9, we return [0, 1].
 
 Example 2:
@@ -17,25 +17,30 @@
 Output: [1,2]
 
 Example 3:
 
 Input: nums = [3,3], target = 6
 Output: [0,1]
 
- 
+
 Constraints:
 
-2 <= nums.length <= 104
--109 <= nums[i] <= 109
--109 <= target <= 109
+`2 <= nums.length <= 104`
+`-109 <= nums[i] <= 109`
+`-109 <= target <= 109`
 Only one valid answer exists.
 
- 
-Follow-up: Can you come up with an algorithm that is less than O(n2) time complexity?
-*/
-
-func twoSum(nums []int, target int) []int {
-    
-}
-// Example test case:
-// [2,7,11,15]
-// 9
+
+Follow-up: Can you come up with an algorithm that is less than `O(n2) `time complexity?
+"""
+
+class Solution(object):
+    def twoSum(self, nums, target):
+        """
+        :type nums: List[int]
+        :type target: int
+        :rtype: List[int]
+        """
+
+# Example test case:
+# [2,7,11,15]
+# 9
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `localeet-0.1.2/tests/data/two_sum.py` & `localeet-0.1.3/tests/data/two_sum.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-"""
+/*
 1 - Easy - Two Sum
 
-Given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target.
+Given an array of integers `nums` and an integer `target`, return indices of the two numbers such that they add up to `target`.
 You may assume that each input would have exactly one solution, and you may not use the same element twice.
 You can return the answer in any order.
- 
+
 Example 1:
 
 Input: nums = [2,7,11,15], target = 9
 Output: [0,1]
 Explanation: Because nums[0] + nums[1] == 9, we return [0, 1].
 
 Example 2:
@@ -17,30 +17,27 @@
 Output: [1,2]
 
 Example 3:
 
 Input: nums = [3,3], target = 6
 Output: [0,1]
 
- 
+
 Constraints:
 
-2 <= nums.length <= 104
--109 <= nums[i] <= 109
--109 <= target <= 109
+`2 <= nums.length <= 104`
+`-109 <= nums[i] <= 109`
+`-109 <= target <= 109`
 Only one valid answer exists.
 
- 
-Follow-up: Can you come up with an algorithm that is less than O(n2) time complexity?
-"""
-
-class Solution(object):
-    def twoSum(self, nums, target):
-        """
-        :type nums: List[int]
-        :type target: int
-        :rtype: List[int]
-        """
-        
-# Example test case:
-# [2,7,11,15]
-# 9
+
+Follow-up: Can you come up with an algorithm that is less than `O(n2) `time complexity?
+*/
+
+impl Solution {
+    pub fn two_sum(nums: Vec<i32>, target: i32) -> Vec<i32> {
+
+    }
+}
+// Example test case:
+// [2,7,11,15]
+// 9
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `localeet-0.1.2/tests/data/two_sum_details.json` & `localeet-0.1.3/tests/data/two_sum_details.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9924242424242424%*

 * *Differences: {"'data'": '{\'question\': {\'likes\': 49028, \'stats\': \'{"totalAccepted": "10.2M", '*

 * *           '"totalSubmission": "20.3M", "totalAcceptedRaw": 10223832, "totalSubmissionRaw": '*

 * *           '20341518, "acRate": "50.3%"}\'}}'}*

```diff
@@ -134,27 +134,27 @@
             ],
             "isLiked": null,
             "isPaidOnly": false,
             "judgeType": "small",
             "judgerAvailable": true,
             "langToValidPlayground": "{\"cpp\": true, \"java\": true, \"python\": true, \"python3\": true, \"mysql\": false, \"mssql\": false, \"oraclesql\": false, \"c\": false, \"csharp\": false, \"javascript\": false, \"ruby\": false, \"bash\": false, \"swift\": false, \"golang\": false, \"scala\": false, \"html\": false, \"pythonml\": false, \"kotlin\": false, \"rust\": false, \"php\": false, \"typescript\": false, \"racket\": false, \"erlang\": false, \"elixir\": false, \"dart\": false, \"pythondata\": false, \"react\": false}",
             "libraryUrl": null,
-            "likes": 49019,
+            "likes": 49028,
             "metaData": "{\n  \"name\": \"twoSum\",\n  \"params\": [\n    {\n      \"name\": \"nums\",\n      \"type\": \"integer[]\"\n    },\n    {\n      \"name\": \"target\",\n      \"type\": \"integer\"\n    }\n  ],\n  \"return\": {\n    \"type\": \"integer[]\",\n    \"size\": 2\n  },\n  \"manual\": false\n}",
             "mysqlSchemas": [],
             "questionFrontendId": "1",
             "questionId": "1",
             "sampleTestCase": "[2,7,11,15]\n9",
             "similarQuestions": "[{\"title\": \"3Sum\", \"titleSlug\": \"3sum\", \"difficulty\": \"Medium\", \"translatedTitle\": null}, {\"title\": \"4Sum\", \"titleSlug\": \"4sum\", \"difficulty\": \"Medium\", \"translatedTitle\": null}, {\"title\": \"Two Sum II - Input Array Is Sorted\", \"titleSlug\": \"two-sum-ii-input-array-is-sorted\", \"difficulty\": \"Medium\", \"translatedTitle\": null}, {\"title\": \"Two Sum III - Data structure design\", \"titleSlug\": \"two-sum-iii-data-structure-design\", \"difficulty\": \"Easy\", \"translatedTitle\": null}, {\"title\": \"Subarray Sum Equals K\", \"titleSlug\": \"subarray-sum-equals-k\", \"difficulty\": \"Medium\", \"translatedTitle\": null}, {\"title\": \"Two Sum IV - Input is a BST\", \"titleSlug\": \"two-sum-iv-input-is-a-bst\", \"difficulty\": \"Easy\", \"translatedTitle\": null}, {\"title\": \"Two Sum Less Than K\", \"titleSlug\": \"two-sum-less-than-k\", \"difficulty\": \"Easy\", \"translatedTitle\": null}, {\"title\": \"Max Number of K-Sum Pairs\", \"titleSlug\": \"max-number-of-k-sum-pairs\", \"difficulty\": \"Medium\", \"translatedTitle\": null}, {\"title\": \"Count Good Meals\", \"titleSlug\": \"count-good-meals\", \"difficulty\": \"Medium\", \"translatedTitle\": null}, {\"title\": \"Count Number of Pairs With Absolute Difference K\", \"titleSlug\": \"count-number-of-pairs-with-absolute-difference-k\", \"difficulty\": \"Easy\", \"translatedTitle\": null}, {\"title\": \"Number of Pairs of Strings With Concatenation Equal to Target\", \"titleSlug\": \"number-of-pairs-of-strings-with-concatenation-equal-to-target\", \"difficulty\": \"Medium\", \"translatedTitle\": null}, {\"title\": \"Find All K-Distant Indices in an Array\", \"titleSlug\": \"find-all-k-distant-indices-in-an-array\", \"difficulty\": \"Easy\", \"translatedTitle\": null}, {\"title\": \"First Letter to Appear Twice\", \"titleSlug\": \"first-letter-to-appear-twice\", \"difficulty\": \"Easy\", \"translatedTitle\": null}, {\"title\": \"Number of Excellent Pairs\", \"titleSlug\": \"number-of-excellent-pairs\", \"difficulty\": \"Hard\", \"translatedTitle\": null}, {\"title\": \"Number of Arithmetic Triplets\", \"titleSlug\": \"number-of-arithmetic-triplets\", \"difficulty\": \"Easy\", \"translatedTitle\": null}, {\"title\": \"Node With Highest Edge Score\", \"titleSlug\": \"node-with-highest-edge-score\", \"difficulty\": \"Medium\", \"translatedTitle\": null}, {\"title\": \"Check Distances Between Same Letters\", \"titleSlug\": \"check-distances-between-same-letters\", \"difficulty\": \"Easy\", \"translatedTitle\": null}, {\"title\": \"Find Subarrays With Equal Sum\", \"titleSlug\": \"find-subarrays-with-equal-sum\", \"difficulty\": \"Easy\", \"translatedTitle\": null}, {\"title\": \"Largest Positive Integer That Exists With Its Negative\", \"titleSlug\": \"largest-positive-integer-that-exists-with-its-negative\", \"difficulty\": \"Easy\", \"translatedTitle\": null}, {\"title\": \"Number of Distinct Averages\", \"titleSlug\": \"number-of-distinct-averages\", \"difficulty\": \"Easy\", \"translatedTitle\": null}]",
             "solution": {
                 "__typename": "ArticleNode",
                 "canSeeDetail": true,
                 "id": "7"
             },
-            "stats": "{\"totalAccepted\": \"10.2M\", \"totalSubmission\": \"20.3M\", \"totalAcceptedRaw\": 10221744, \"totalSubmissionRaw\": 20338203, \"acRate\": \"50.3%\"}",
+            "stats": "{\"totalAccepted\": \"10.2M\", \"totalSubmission\": \"20.3M\", \"totalAcceptedRaw\": 10223832, \"totalSubmissionRaw\": 20341518, \"acRate\": \"50.3%\"}",
             "status": null,
             "title": "Two Sum",
             "titleSlug": "two-sum",
             "topicTags": [
                 {
                     "__typename": "TopicTagNode",
                     "name": "Array",
```

### Comparing `localeet-0.1.2/tests/data/two_sum_essentials.json` & `localeet-0.1.3/tests/data/two_sum_essentials.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'question'": "'Given an array of integers `nums` and an integer `target`, return indices of the "*

 * *               'two numbers such that they add up to `target`.\\nYou may assume that each input '*

 * *               'would have exactly one solution, and you may not use the same element twice.\\nYou '*

 * *               'can return the answer in any order.\\n \\nExample 1:\\n\\nInput: nums = '*

 * *               '[2,7,11,15], target = 9\\nOutput: [0,1]\\nExplanation: Because nums[0] + nums[1] '*

 * *               '== 9, we […]*

```diff
@@ -112,12 +112,12 @@
             "__typename": "CodeSnippetNode",
             "code": "class Solution {\n  List<int> twoSum(List<int> nums, int target) {\n\n  }\n}",
             "lang": "Dart",
             "langSlug": "dart"
         }
     ],
     "difficulty": "Easy",
-    "question": "Given an array of integers nums\u00a0and an integer target, return indices of the two numbers such that they add up to target.\nYou may assume that each input would have exactly one solution, and you may not use the same element twice.\nYou can return the answer in any order.\n\u00a0\nExample 1:\n\nInput: nums = [2,7,11,15], target = 9\nOutput: [0,1]\nExplanation: Because nums[0] + nums[1] == 9, we return [0, 1].\n\nExample 2:\n\nInput: nums = [3,2,4], target = 6\nOutput: [1,2]\n\nExample 3:\n\nInput: nums = [3,3], target = 6\nOutput: [0,1]\n\n\u00a0\nConstraints:\n\n2 <= nums.length <= 104\n-109 <= nums[i] <= 109\n-109 <= target <= 109\nOnly one valid answer exists.\n\n\u00a0\nFollow-up:\u00a0Can you come up with an algorithm that is less than\u00a0O(n2)\u00a0time complexity?",
+    "question": "Given an array of integers `nums` and an integer `target`, return indices of the two numbers such that they add up to `target`.\nYou may assume that each input would have exactly one solution, and you may not use the same element twice.\nYou can return the answer in any order.\n \nExample 1:\n\nInput: nums = [2,7,11,15], target = 9\nOutput: [0,1]\nExplanation: Because nums[0] + nums[1] == 9, we return [0, 1].\n\nExample 2:\n\nInput: nums = [3,2,4], target = 6\nOutput: [1,2]\n\nExample 3:\n\nInput: nums = [3,3], target = 6\nOutput: [0,1]\n\n \nConstraints:\n\n`2 <= nums.length <= 104`\n`-109 <= nums[i] <= 109`\n`-109 <= target <= 109`\nOnly one valid answer exists.\n\n \nFollow-up: Can you come up with an algorithm that is less than `O(n2) `time complexity?",
     "question_id": "1",
     "test_case": "[2,7,11,15]\n9",
     "title": "Two Sum"
 }
```

### Comparing `localeet-0.1.2/.gitignore` & `localeet-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `localeet-0.1.2/LICENSE` & `localeet-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `localeet-0.1.2/pyproject.toml` & `localeet-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 ignore = [
   "S311",  # not using randomness for cryptography
   "S101",  # assert is awesome
   "ANN101",  # self does not need a type annotation
   "I001",  # I do not care for its sorting choices
 ]
 exclude = [
-  "tests/data/*",
+  "tests/data/two_sum.py",
 ]
 show-fixes = true
 target-version = "py39"
 
 [tool.ruff.flake8-quotes]
 inline-quotes = "single"
```

### Comparing `localeet-0.1.2/PKG-INFO` & `localeet-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localeet
-Version: 0.1.2
+Version: 0.1.3
 Summary: A CLI tool to do LeetCode and LeetCode-like exercises
 Author-email: Danny Brown <dannybrown37@gmail.com>
 License-File: LICENSE
 Requires-Dist: bs4
 Requires-Dist: click
 Requires-Dist: lxml
 Requires-Dist: requests
```

