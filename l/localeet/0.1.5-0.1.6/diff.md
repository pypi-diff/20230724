# Comparing `tmp/localeet-0.1.5.tar.gz` & `tmp/localeet-0.1.6.tar.gz`

## Comparing `localeet-0.1.5.tar` & `localeet-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 localeet-0.1.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 localeet-0.1.5/README.md
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 localeet-0.1.5/.github/workflows/pr.yml
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 localeet-0.1.5/.github/workflows/pypi.yaml
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 localeet-0.1.5/src/localeet/__init__.py
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 localeet-0.1.5/src/localeet/__main__.py
--rw-r--r--   0        0        0     7040 2020-02-02 00:00:00.000000 localeet-0.1.5/src/localeet/get_leetcode_problem.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 localeet-0.1.5/src/localeet/get_version.py
--rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 localeet-0.1.5/src/localeet/language_maps.py
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 localeet-0.1.5/tests/conftest.py
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 localeet-0.1.5/tests/get_leetcode_problem_test.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 localeet-0.1.5/tests/version_number_test.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 localeet-0.1.5/tests/data/two_sum.go
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 localeet-0.1.5/tests/data/two_sum.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 localeet-0.1.5/tests/data/two_sum.rs
--rw-r--r--   0        0        0    20244 2020-02-02 00:00:00.000000 localeet-0.1.5/tests/data/two_sum_details.json
--rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 localeet-0.1.5/tests/data/two_sum_essentials.json
--rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 localeet-0.1.5/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 localeet-0.1.5/LICENSE
--rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 localeet-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 localeet-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 localeet-0.1.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 localeet-0.1.6/README.md
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 localeet-0.1.6/.github/workflows/pr.yml
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 localeet-0.1.6/.github/workflows/pypi.yaml
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 localeet-0.1.6/src/localeet/__init__.py
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 localeet-0.1.6/src/localeet/__main__.py
+-rw-r--r--   0        0        0     7040 2020-02-02 00:00:00.000000 localeet-0.1.6/src/localeet/get_leetcode_problem.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 localeet-0.1.6/src/localeet/get_version.py
+-rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 localeet-0.1.6/src/localeet/language_maps.py
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 localeet-0.1.6/tests/conftest.py
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 localeet-0.1.6/tests/get_leetcode_problem_test.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 localeet-0.1.6/tests/version_number_test.py
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 localeet-0.1.6/tests/data/two_sum.go
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 localeet-0.1.6/tests/data/two_sum.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 localeet-0.1.6/tests/data/two_sum.rs
+-rw-r--r--   0        0        0    20244 2020-02-02 00:00:00.000000 localeet-0.1.6/tests/data/two_sum_details.json
+-rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 localeet-0.1.6/tests/data/two_sum_essentials.json
+-rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 localeet-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 localeet-0.1.6/LICENSE
+-rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 localeet-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 localeet-0.1.6/PKG-INFO
```

### Comparing `localeet-0.1.5/.pre-commit-config.yaml` & `localeet-0.1.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `localeet-0.1.5/README.md` & `localeet-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `localeet-0.1.5/.github/workflows/pr.yml` & `localeet-0.1.6/.github/workflows/pr.yml`

 * *Files identical despite different names*

### Comparing `localeet-0.1.5/.github/workflows/pypi.yaml` & `localeet-0.1.6/.github/workflows/pypi.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -11,36 +11,32 @@
     steps:
     - name: Checkout Code
       uses: actions/checkout@v2
     - name: Set up Python
       uses: actions/setup-python@v2
       with:
         python-version: 3.9
-    - name: Read version from __init__.py
-      run: |
-        version=$(grep "__version__" src/localeet/__init__.py | cut -d "'" -f 2)
-        echo "Version from __init__.py: $version"
-        echo "::set-output name=version::$version"
     - name: Install distribution dependencies
       run: |
         pip install -U pip
         pip install .[pypi]
     - name: Build distribution
       run: hatchling build
     - name: Publish to PyPI
       env:
         TWINE_USERNAME: __token__
         TWINE_PASSWORD: ${{ secrets.PYPI_API_TOKEN }}
       run: twine upload dist/*
     - name: pip install localeet
       run: pip install localeet
-    - name: Compare Versions
+    - name: Compare Repo and Pip Versions
       run: |
-        local_version=$(localeet --version)
-        echo "Local version: $local_version"
-        echo "GitHub Actions version: ${{ steps.localeet_version.outputs.stdout }}"
-        if [ "$local_version" = "${{ steps.localeet_version.outputs.stdout }}" ]; then
+        repo_version=$(grep "__version__" src/localeet/__init__.py | cut -d "'" -f 2)
+        echo "Version from __init__.py: $repo_version"
+        pip_version=$(localeet --version)
+        echo "Local version: $pip_version"
+        if [[ $repo_version = $pip_version ]]; then
           echo "Latest version successfully deployed and pip installed"
         else
           echo "Versions do not match! There was an issue with deployment"
           exit 1
         fi
```

### Comparing `localeet-0.1.5/src/localeet/__main__.py` & `localeet-0.1.6/src/localeet/__main__.py`

 * *Files identical despite different names*

### Comparing `localeet-0.1.5/src/localeet/get_leetcode_problem.py` & `localeet-0.1.6/src/localeet/get_leetcode_problem.py`

 * *Files identical despite different names*

### Comparing `localeet-0.1.5/src/localeet/language_maps.py` & `localeet-0.1.6/src/localeet/language_maps.py`

 * *Files identical despite different names*

### Comparing `localeet-0.1.5/tests/conftest.py` & `localeet-0.1.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `localeet-0.1.5/tests/get_leetcode_problem_test.py` & `localeet-0.1.6/tests/get_leetcode_problem_test.py`

 * *Files identical despite different names*

### Comparing `localeet-0.1.5/tests/version_number_test.py` & `localeet-0.1.6/tests/version_number_test.py`

 * *Files identical despite different names*

### Comparing `localeet-0.1.5/tests/data/two_sum.go` & `localeet-0.1.6/tests/data/two_sum.go`

 * *Files identical despite different names*

### Comparing `localeet-0.1.5/tests/data/two_sum.py` & `localeet-0.1.6/tests/data/two_sum.py`

 * *Files identical despite different names*

### Comparing `localeet-0.1.5/tests/data/two_sum.rs` & `localeet-0.1.6/tests/data/two_sum.rs`

 * *Files identical despite different names*

### Comparing `localeet-0.1.5/tests/data/two_sum_details.json` & `localeet-0.1.6/tests/data/two_sum_details.json`

 * *Files identical despite different names*

### Comparing `localeet-0.1.5/tests/data/two_sum_essentials.json` & `localeet-0.1.6/tests/data/two_sum_essentials.json`

 * *Files identical despite different names*

### Comparing `localeet-0.1.5/.gitignore` & `localeet-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `localeet-0.1.5/LICENSE` & `localeet-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `localeet-0.1.5/pyproject.toml` & `localeet-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `localeet-0.1.5/PKG-INFO` & `localeet-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localeet
-Version: 0.1.5
+Version: 0.1.6
 Summary: A CLI tool to do LeetCode and LeetCode-like exercises
 Author-email: Danny Brown <dannybrown37@gmail.com>
 License-File: LICENSE
 Requires-Dist: bs4
 Requires-Dist: click
 Requires-Dist: lxml
 Requires-Dist: requests
```

