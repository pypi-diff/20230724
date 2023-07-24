# Comparing `tmp/nasti-0.1.3.tar.gz` & `tmp/nasti-0.1.4.tar.gz`

## Comparing `nasti-0.1.3.tar` & `nasti-0.1.4.tar`

### file list

```diff
@@ -1,46 +1,45 @@
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 nasti-0.1.3/Makefile
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 nasti-0.1.3/Pipfile
--rw-r--r--   0        0        0    28335 2020-02-02 00:00:00.000000 nasti-0.1.3/Pipfile.lock
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 nasti-0.1.3/entry_points.txt
--rw-r--r--   0        0        0    70731 2020-02-02 00:00:00.000000 nasti-0.1.3/logo.png
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 nasti-0.1.3/nasti.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 nasti-0.1.3/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 nasti-0.1.3/.github/workflows/tests.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nasti-0.1.3/nasti/__init__.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 nasti-0.1.3/nasti/cli.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 nasti-0.1.3/nasti/exceptions.py
--rw-r--r--   0        0        0     7086 2020-02-02 00:00:00.000000 nasti-0.1.3/nasti/mutation.py
--rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 nasti-0.1.3/nasti/nasti.py
--rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 nasti-0.1.3/nasti/nastifile.py
--rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 nasti-0.1.3/nasti/source_handlers.py
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 nasti-0.1.3/nasti/validation.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/mocks.py
--rw-r--r--   0        0        0     5435 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/test_mutation.py
--rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/test_nastifile.py
--rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/test_source_handlers.py
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/test_validation.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/nastifiles/bad_yaml/nasti.yaml
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/nastifiles/mutation_empty_files/nasti.yaml
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/nastifiles/mutation_file_doesnt_contain_replacement_text/nasti.yaml
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/nastifiles/mutation_file_doesnt_contain_replacement_text/test.txt
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/nastifiles/mutation_files_dont_exist/nasti.yaml
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/nastifiles/mutation_misconfigured_validation/nasti.yaml
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/nastifiles/mutation_no_files/nasti.yaml
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/nastifiles/mutation_run/nasti.yaml
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/nastifiles/mutation_text_replacement_fails/nasti.yaml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/nastifiles/mutation_text_replacement_fails/test.txt
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/nastifiles/mutation_unknown_keys/nasti.yaml
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/nastifiles/mutation_unmentioned_files/nasti.yaml
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/nastifiles/mutation_unmentioned_files/files/.dontsearch
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/nastifiles/mutation_unmentioned_files/files/ref.txt
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/nastifiles/mutation_unmentioned_files/files/unmentioned
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/nastifiles/mutation_unmentioned_files/files/nested/searchbutnotfind
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/nastifiles/mutation_unmentioned_files/files/nested/unmentioned
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/nastifiles/no_mutations/nasti.yaml
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 nasti-0.1.3/tests/nastifiles/valid/nasti.yaml
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nasti-0.1.3/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 nasti-0.1.3/LICENSE
--rw-r--r--   0        0        0     9246 2020-02-02 00:00:00.000000 nasti-0.1.3/README.md
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 nasti-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     9785 2020-02-02 00:00:00.000000 nasti-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 nasti-0.1.4/Makefile
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 nasti-0.1.4/Pipfile
+-rw-r--r--   0        0        0    28335 2020-02-02 00:00:00.000000 nasti-0.1.4/Pipfile.lock
+-rw-r--r--   0        0        0    70731 2020-02-02 00:00:00.000000 nasti-0.1.4/logo.png
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 nasti-0.1.4/nasti.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 nasti-0.1.4/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 nasti-0.1.4/.github/workflows/tests.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nasti-0.1.4/nasti/__init__.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 nasti-0.1.4/nasti/cli.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 nasti-0.1.4/nasti/exceptions.py
+-rw-r--r--   0        0        0     7086 2020-02-02 00:00:00.000000 nasti-0.1.4/nasti/mutation.py
+-rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 nasti-0.1.4/nasti/nasti.py
+-rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 nasti-0.1.4/nasti/nastifile.py
+-rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 nasti-0.1.4/nasti/source_handlers.py
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 nasti-0.1.4/nasti/validation.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/mocks.py
+-rw-r--r--   0        0        0     5435 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/test_mutation.py
+-rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/test_nastifile.py
+-rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/test_source_handlers.py
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/test_validation.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/nastifiles/bad_yaml/nasti.yaml
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/nastifiles/mutation_empty_files/nasti.yaml
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/nastifiles/mutation_file_doesnt_contain_replacement_text/nasti.yaml
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/nastifiles/mutation_file_doesnt_contain_replacement_text/test.txt
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/nastifiles/mutation_files_dont_exist/nasti.yaml
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/nastifiles/mutation_misconfigured_validation/nasti.yaml
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/nastifiles/mutation_no_files/nasti.yaml
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/nastifiles/mutation_run/nasti.yaml
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/nastifiles/mutation_text_replacement_fails/nasti.yaml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/nastifiles/mutation_text_replacement_fails/test.txt
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/nastifiles/mutation_unknown_keys/nasti.yaml
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/nastifiles/mutation_unmentioned_files/nasti.yaml
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/nastifiles/mutation_unmentioned_files/files/.dontsearch
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/nastifiles/mutation_unmentioned_files/files/ref.txt
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/nastifiles/mutation_unmentioned_files/files/unmentioned
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/nastifiles/mutation_unmentioned_files/files/nested/searchbutnotfind
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/nastifiles/mutation_unmentioned_files/files/nested/unmentioned
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/nastifiles/no_mutations/nasti.yaml
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/nastifiles/valid/nasti.yaml
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nasti-0.1.4/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 nasti-0.1.4/LICENSE
+-rw-r--r--   0        0        0     9246 2020-02-02 00:00:00.000000 nasti-0.1.4/README.md
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 nasti-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     9785 2020-02-02 00:00:00.000000 nasti-0.1.4/PKG-INFO
```

### Comparing `nasti-0.1.3/Pipfile.lock` & `nasti-0.1.4/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `nasti-0.1.3/logo.png` & `nasti-0.1.4/logo.png`

 * *Files identical despite different names*

### Comparing `nasti-0.1.3/.github/workflows/coverage.yml` & `nasti-0.1.4/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `nasti-0.1.3/.github/workflows/tests.yml` & `nasti-0.1.4/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `nasti-0.1.3/nasti/cli.py` & `nasti-0.1.4/nasti/cli.py`

 * *Files identical despite different names*

### Comparing `nasti-0.1.3/nasti/exceptions.py` & `nasti-0.1.4/nasti/exceptions.py`

 * *Files identical despite different names*

### Comparing `nasti-0.1.3/nasti/mutation.py` & `nasti-0.1.4/nasti/mutation.py`

 * *Files identical despite different names*

### Comparing `nasti-0.1.3/nasti/nasti.py` & `nasti-0.1.4/nasti/nasti.py`

 * *Files identical despite different names*

### Comparing `nasti-0.1.3/nasti/nastifile.py` & `nasti-0.1.4/nasti/nastifile.py`

 * *Files identical despite different names*

### Comparing `nasti-0.1.3/nasti/source_handlers.py` & `nasti-0.1.4/nasti/source_handlers.py`

 * *Files identical despite different names*

### Comparing `nasti-0.1.3/nasti/validation.py` & `nasti-0.1.4/nasti/validation.py`

 * *Files identical despite different names*

### Comparing `nasti-0.1.3/tests/mocks.py` & `nasti-0.1.4/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `nasti-0.1.3/tests/test_mutation.py` & `nasti-0.1.4/tests/test_mutation.py`

 * *Files identical despite different names*

### Comparing `nasti-0.1.3/tests/test_nastifile.py` & `nasti-0.1.4/tests/test_nastifile.py`

 * *Files identical despite different names*

### Comparing `nasti-0.1.3/tests/test_source_handlers.py` & `nasti-0.1.4/tests/test_source_handlers.py`

 * *Files identical despite different names*

### Comparing `nasti-0.1.3/tests/test_validation.py` & `nasti-0.1.4/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `nasti-0.1.3/.gitignore` & `nasti-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `nasti-0.1.3/LICENSE` & `nasti-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nasti-0.1.3/README.md` & `nasti-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `nasti-0.1.3/PKG-INFO` & `nasti-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NASTI
-Version: 0.1.3
+Version: 0.1.4
 Summary: NASTI is Not A Starndard Templating Implementation
 Project-URL: Homepage, https://github.com/adamrdrew/nasti
 Project-URL: Bug Tracker, https://github.com/adamrdrew/nasti/issues
 Author-email: Adam Drew <adamrdrew@live.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

