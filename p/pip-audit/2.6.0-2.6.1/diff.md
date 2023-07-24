# Comparing `tmp/pip_audit-2.6.0.tar.gz` & `tmp/pip_audit-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip_audit-2.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pip_audit-2.6.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pip_audit-2.6.0.tar` & `pip_audit-2.6.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    10174 2023-07-02 13:32:31.064548 pip_audit-2.6.0/LICENSE
--rw-r--r--   0        0        0    21113 2023-07-02 13:32:31.064548 pip_audit-2.6.0/README.md
--rw-r--r--   0        0        0       53 2023-07-02 13:32:31.064548 pip_audit-2.6.0/pip_audit/__init__.py
--rw-r--r--   0        0        0      144 2023-07-02 13:32:31.064548 pip_audit-2.6.0/pip_audit/__main__.py
--rw-r--r--   0        0        0     3158 2023-07-02 13:32:31.064548 pip_audit-2.6.0/pip_audit/_audit.py
--rw-r--r--   0        0        0     6223 2023-07-02 13:32:31.064548 pip_audit-2.6.0/pip_audit/_cache.py
--rw-r--r--   0        0        0    19978 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pip_audit/_cli.py
--rw-r--r--   0        0        0      579 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pip_audit/_dependency_source/__init__.py
--rw-r--r--   0        0        0     1738 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pip_audit/_dependency_source/interface.py
--rw-r--r--   0        0        0     6853 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pip_audit/_dependency_source/pip.py
--rw-r--r--   0        0        0     5416 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pip_audit/_dependency_source/pyproject.py
--rw-r--r--   0        0        0    15336 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pip_audit/_dependency_source/requirement.py
--rw-r--r--   0        0        0     3683 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pip_audit/_fix.py
--rw-r--r--   0        0        0      380 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pip_audit/_format/__init__.py
--rw-r--r--   0        0        0     5318 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pip_audit/_format/columns.py
--rw-r--r--   0        0        0     2800 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pip_audit/_format/cyclonedx.py
--rw-r--r--   0        0        0     1119 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pip_audit/_format/interface.py
--rw-r--r--   0        0        0     3160 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pip_audit/_format/json.py
--rw-r--r--   0        0        0     4844 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pip_audit/_format/markdown.py
--rw-r--r--   0        0        0      536 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pip_audit/_service/__init__.py
--rw-r--r--   0        0        0     5265 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pip_audit/_service/interface.py
--rw-r--r--   0        0        0     5898 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pip_audit/_service/osv.py
--rw-r--r--   0        0        0     5047 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pip_audit/_service/pypi.py
--rw-r--r--   0        0        0     8716 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pip_audit/_state.py
--rw-r--r--   0        0        0     2332 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pip_audit/_subprocess.py
--rw-r--r--   0        0        0      662 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pip_audit/_util.py
--rw-r--r--   0        0        0     6326 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pip_audit/_virtual_env.py
--rw-r--r--   0        0        0     3166 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pyproject.toml
--rw-r--r--   0        0        0    23270 1970-01-01 00:00:00.000000 pip_audit-2.6.0/PKG-INFO
+-rw-r--r--   0        0        0    10174 2023-07-24 18:47:23.676035 pip_audit-2.6.1/LICENSE
+-rw-r--r--   0        0        0    21113 2023-07-24 18:47:23.676035 pip_audit-2.6.1/README.md
+-rw-r--r--   0        0        0       53 2023-07-24 18:47:23.676035 pip_audit-2.6.1/pip_audit/__init__.py
+-rw-r--r--   0        0        0      144 2023-07-24 18:47:23.676035 pip_audit-2.6.1/pip_audit/__main__.py
+-rw-r--r--   0        0        0     3158 2023-07-24 18:47:23.676035 pip_audit-2.6.1/pip_audit/_audit.py
+-rw-r--r--   0        0        0     6223 2023-07-24 18:47:23.676035 pip_audit-2.6.1/pip_audit/_cache.py
+-rw-r--r--   0        0        0    19978 2023-07-24 18:47:23.676035 pip_audit-2.6.1/pip_audit/_cli.py
+-rw-r--r--   0        0        0      579 2023-07-24 18:47:23.676035 pip_audit-2.6.1/pip_audit/_dependency_source/__init__.py
+-rw-r--r--   0        0        0     1738 2023-07-24 18:47:23.676035 pip_audit-2.6.1/pip_audit/_dependency_source/interface.py
+-rw-r--r--   0        0        0     6853 2023-07-24 18:47:23.676035 pip_audit-2.6.1/pip_audit/_dependency_source/pip.py
+-rw-r--r--   0        0        0     5681 2023-07-24 18:47:23.676035 pip_audit-2.6.1/pip_audit/_dependency_source/pyproject.py
+-rw-r--r--   0        0        0    15336 2023-07-24 18:47:23.676035 pip_audit-2.6.1/pip_audit/_dependency_source/requirement.py
+-rw-r--r--   0        0        0     3683 2023-07-24 18:47:23.676035 pip_audit-2.6.1/pip_audit/_fix.py
+-rw-r--r--   0        0        0      380 2023-07-24 18:47:23.676035 pip_audit-2.6.1/pip_audit/_format/__init__.py
+-rw-r--r--   0        0        0     5318 2023-07-24 18:47:23.676035 pip_audit-2.6.1/pip_audit/_format/columns.py
+-rw-r--r--   0        0        0     2800 2023-07-24 18:47:23.676035 pip_audit-2.6.1/pip_audit/_format/cyclonedx.py
+-rw-r--r--   0        0        0     1119 2023-07-24 18:47:23.676035 pip_audit-2.6.1/pip_audit/_format/interface.py
+-rw-r--r--   0        0        0     3160 2023-07-24 18:47:23.676035 pip_audit-2.6.1/pip_audit/_format/json.py
+-rw-r--r--   0        0        0     4844 2023-07-24 18:47:23.676035 pip_audit-2.6.1/pip_audit/_format/markdown.py
+-rw-r--r--   0        0        0      536 2023-07-24 18:47:23.676035 pip_audit-2.6.1/pip_audit/_service/__init__.py
+-rw-r--r--   0        0        0     5265 2023-07-24 18:47:23.676035 pip_audit-2.6.1/pip_audit/_service/interface.py
+-rw-r--r--   0        0        0     5898 2023-07-24 18:47:23.676035 pip_audit-2.6.1/pip_audit/_service/osv.py
+-rw-r--r--   0        0        0     5047 2023-07-24 18:47:23.676035 pip_audit-2.6.1/pip_audit/_service/pypi.py
+-rw-r--r--   0        0        0     8716 2023-07-24 18:47:23.680034 pip_audit-2.6.1/pip_audit/_state.py
+-rw-r--r--   0        0        0     2332 2023-07-24 18:47:23.680034 pip_audit-2.6.1/pip_audit/_subprocess.py
+-rw-r--r--   0        0        0      662 2023-07-24 18:47:23.680034 pip_audit-2.6.1/pip_audit/_util.py
+-rw-r--r--   0        0        0     6601 2023-07-24 18:47:23.680034 pip_audit-2.6.1/pip_audit/_virtual_env.py
+-rw-r--r--   0        0        0     3166 2023-07-24 18:47:23.680034 pip_audit-2.6.1/pyproject.toml
+-rw-r--r--   0        0        0    23270 1970-01-01 00:00:00.000000 pip_audit-2.6.1/PKG-INFO
```

### Comparing `pip_audit-2.6.0/LICENSE` & `pip_audit-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pip_audit-2.6.0/README.md` & `pip_audit-2.6.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
 `pip-audit` has [`pre-commit`](https://pre-commit.com/) support.
 
 For example, using `pip-audit` via `pre-commit` to audit a requirements file:
 
 ```yaml
   - repo: https://github.com/pypa/pip-audit
-    rev: v2.6.0
+    rev: v2.6.1
     hooks:
       -   id: pip-audit
           args: ["-r", "requirements.txt"]
 
 ci:
   # Leave pip-audit to only run locally and not in CI
   # pre-commit.ci does not allow network calls
```

### Comparing `pip_audit-2.6.0/pip_audit/_audit.py` & `pip_audit-2.6.1/pip_audit/_audit.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.6.0/pip_audit/_cache.py` & `pip_audit-2.6.1/pip_audit/_cache.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.6.0/pip_audit/_cli.py` & `pip_audit-2.6.1/pip_audit/_cli.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.6.0/pip_audit/_dependency_source/__init__.py` & `pip_audit-2.6.1/pip_audit/_dependency_source/__init__.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.6.0/pip_audit/_dependency_source/interface.py` & `pip_audit-2.6.1/pip_audit/_dependency_source/interface.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.6.0/pip_audit/_dependency_source/pip.py` & `pip_audit-2.6.1/pip_audit/_dependency_source/pip.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.6.0/pip_audit/_dependency_source/pyproject.py` & `pip_audit-2.6.1/pip_audit/_dependency_source/pyproject.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,15 +72,21 @@
                 )
                 return
 
             # NOTE(alex): This is probably due for a redesign. Since we're leaning on `pip` for
             # dependency resolution now, we can think about doing `pip install <local-project-dir>`
             # regardless of whether the project has a `pyproject.toml` or not. And if it doesn't
             # have a `pyproject.toml`, we can raise an error if the user provides `--fix`.
-            with NamedTemporaryFile() as req_file, TemporaryDirectory() as ve_dir:
+            with TemporaryDirectory() as ve_dir, NamedTemporaryFile(
+                dir=ve_dir, delete=False
+            ) as req_file:
+                # We use delete=False in creating the tempfile to allow it to be
+                # closed and opened multiple times within the context scope on
+                # windows, see GitHub issue #646.
+
                 # Write the dependencies to a temporary requirements file.
                 req_file.write(os.linesep.join(deps).encode())
                 req_file.flush()
 
                 # Try to install the generated requirements file.
                 ve = VirtualEnv(install_args=["-r", req_file.name], state=self.state)
                 try:
```

### Comparing `pip_audit-2.6.0/pip_audit/_dependency_source/requirement.py` & `pip_audit-2.6.1/pip_audit/_dependency_source/requirement.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.6.0/pip_audit/_fix.py` & `pip_audit-2.6.1/pip_audit/_fix.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.6.0/pip_audit/_format/columns.py` & `pip_audit-2.6.1/pip_audit/_format/columns.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.6.0/pip_audit/_format/cyclonedx.py` & `pip_audit-2.6.1/pip_audit/_format/cyclonedx.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.6.0/pip_audit/_format/interface.py` & `pip_audit-2.6.1/pip_audit/_format/interface.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.6.0/pip_audit/_format/json.py` & `pip_audit-2.6.1/pip_audit/_format/json.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.6.0/pip_audit/_format/markdown.py` & `pip_audit-2.6.1/pip_audit/_format/markdown.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.6.0/pip_audit/_service/__init__.py` & `pip_audit-2.6.1/pip_audit/_service/__init__.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.6.0/pip_audit/_service/interface.py` & `pip_audit-2.6.1/pip_audit/_service/interface.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.6.0/pip_audit/_service/osv.py` & `pip_audit-2.6.1/pip_audit/_service/osv.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.6.0/pip_audit/_service/pypi.py` & `pip_audit-2.6.1/pip_audit/_service/pypi.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.6.0/pip_audit/_state.py` & `pip_audit-2.6.1/pip_audit/_state.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.6.0/pip_audit/_subprocess.py` & `pip_audit-2.6.1/pip_audit/_subprocess.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.6.0/pip_audit/_util.py` & `pip_audit-2.6.1/pip_audit/_util.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.6.0/pip_audit/_virtual_env.py` & `pip_audit-2.6.1/pip_audit/_virtual_env.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 from __future__ import annotations
 
 import json
 import logging
 import venv
-from tempfile import NamedTemporaryFile
+from tempfile import NamedTemporaryFile, TemporaryDirectory
 from types import SimpleNamespace
 from typing import Iterator
 
 from packaging.version import Version
 
 from ._state import AuditState
 from ._subprocess import CalledProcessError, run
@@ -106,15 +106,19 @@
         try:
             run(pip_upgrade_cmd, state=self._state)
         except CalledProcessError as cpe:
             raise VirtualEnvError(f"Failed to upgrade `pip`: {pip_upgrade_cmd}") from cpe
 
         self._state.update_state("Installing package in isolated environment")
 
-        with NamedTemporaryFile() as tmp:
+        with TemporaryDirectory() as ve_dir, NamedTemporaryFile(dir=ve_dir, delete=False) as tmp:
+            # We use delete=False in creating the tempfile to allow it to be
+            # closed and opened multiple times within the context scope on
+            # windows, see GitHub issue #646.
+
             # Install our packages
             package_install_cmd = [
                 context.env_exe,
                 "-m",
                 "pip",
                 "install",
                 *self._index_url_args,
```

### Comparing `pip_audit-2.6.0/pyproject.toml` & `pip_audit-2.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 [project.optional-dependencies]
 test = ["coverage[toml]", "pretend", "pytest", "pytest-cov"]
 lint = [
     "black>=22.3.0",
     # NOTE(ww): ruff is under active development, so we pin conservatively here
     # and let Dependabot periodically perform this update.
-    "ruff < 0.0.276",
+    "ruff < 0.0.281",
     "interrogate",
     "isort",
     "mypy",
     "types-html5lib",
     "types-requests",
     "types-toml",
 ]
```

### Comparing `pip_audit-2.6.0/PKG-INFO` & `pip_audit-2.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip_audit
-Version: 2.6.0
+Version: 2.6.1
 Summary: A tool for scanning Python environments for known vulnerabilities
 Author-email: Alex Cameron <alex.cameron@trailofbits.com>, Dustin Ingram <di@python.org>, William Woodruff <william@trailofbits.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -26,15 +26,15 @@
 Requires-Dist: rich>=12.4
 Requires-Dist: toml>=0.10
 Requires-Dist: build ; extra == "dev"
 Requires-Dist: bump>=1.3.2 ; extra == "dev"
 Requires-Dist: pip-audit[doc,test,lint] ; extra == "dev"
 Requires-Dist: pdoc ; extra == "doc"
 Requires-Dist: black>=22.3.0 ; extra == "lint"
-Requires-Dist: ruff < 0.0.276 ; extra == "lint"
+Requires-Dist: ruff < 0.0.281 ; extra == "lint"
 Requires-Dist: interrogate ; extra == "lint"
 Requires-Dist: isort ; extra == "lint"
 Requires-Dist: mypy ; extra == "lint"
 Requires-Dist: types-html5lib ; extra == "lint"
 Requires-Dist: types-requests ; extra == "lint"
 Requires-Dist: types-toml ; extra == "lint"
 Requires-Dist: coverage[toml] ; extra == "test"
@@ -153,15 +153,15 @@
 
 `pip-audit` has [`pre-commit`](https://pre-commit.com/) support.
 
 For example, using `pip-audit` via `pre-commit` to audit a requirements file:
 
 ```yaml
   - repo: https://github.com/pypa/pip-audit
-    rev: v2.6.0
+    rev: v2.6.1
     hooks:
       -   id: pip-audit
           args: ["-r", "requirements.txt"]
 
 ci:
   # Leave pip-audit to only run locally and not in CI
   # pre-commit.ci does not allow network calls
```

