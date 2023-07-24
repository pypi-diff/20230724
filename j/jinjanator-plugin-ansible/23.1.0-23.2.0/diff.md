# Comparing `tmp/jinjanator_plugin_ansible-23.1.0.tar.gz` & `tmp/jinjanator_plugin_ansible-23.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon Jul 24 18:51:38 2023, max compression
+gzip compressed data, last modified: Mon Jul 24 20:11:46 2023, max compression
```

## Comparing `jinjanator_plugin_ansible-23.1.0.tar` & `jinjanator_plugin_ansible-23.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1009 2023-07-24 18:51:38.000000 jinjanator_plugin_ansible-23.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     2817 2023-07-24 18:51:38.000000 jinjanator_plugin_ansible-23.1.0/README.md
--rw-r--r--   0        0        0        0 2023-07-24 18:51:38.000000 jinjanator_plugin_ansible-23.1.0/src/jinjanator_plugin_ansible/__init__.py
--rw-r--r--   0        0        0      520 2023-07-24 18:51:38.000000 jinjanator_plugin_ansible-23.1.0/src/jinjanator_plugin_ansible/plugin.py
--rw-r--r--   0        0        0        0 2023-07-24 18:51:38.000000 jinjanator_plugin_ansible-23.1.0/src/jinjanator_plugin_ansible/py.typed
--rw-r--r--   0        0        0      967 2023-07-24 18:51:38.000000 jinjanator_plugin_ansible-23.1.0/tests/test_plugin.py
--rw-r--r--   0        0        0       32 2023-07-24 18:51:38.000000 jinjanator_plugin_ansible-23.1.0/.gitignore
--rw-r--r--   0        0        0    11357 2023-07-24 18:51:38.000000 jinjanator_plugin_ansible-23.1.0/LICENSE
--rw-r--r--   0        0        0     6529 2023-07-24 18:51:38.000000 jinjanator_plugin_ansible-23.1.0/pyproject.toml
--rw-r--r--   0        0        0     1797 2023-07-24 18:51:38.000000 jinjanator_plugin_ansible-23.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1430 2023-07-24 20:11:46.000000 jinjanator_plugin_ansible-23.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2817 2023-07-24 20:11:46.000000 jinjanator_plugin_ansible-23.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-24 20:11:46.000000 jinjanator_plugin_ansible-23.2.0/src/jinjanator_plugin_ansible/__init__.py
+-rw-r--r--   0        0        0     1405 2023-07-24 20:11:46.000000 jinjanator_plugin_ansible-23.2.0/src/jinjanator_plugin_ansible/plugin.py
+-rw-r--r--   0        0        0        0 2023-07-24 20:11:46.000000 jinjanator_plugin_ansible-23.2.0/src/jinjanator_plugin_ansible/py.typed
+-rw-r--r--   0        0        0      967 2023-07-24 20:11:46.000000 jinjanator_plugin_ansible-23.2.0/tests/test_plugin.py
+-rw-r--r--   0        0        0       32 2023-07-24 20:11:46.000000 jinjanator_plugin_ansible-23.2.0/.gitignore
+-rw-r--r--   0        0        0    11357 2023-07-24 20:11:46.000000 jinjanator_plugin_ansible-23.2.0/LICENSE
+-rw-r--r--   0        0        0     6477 2023-07-24 20:11:46.000000 jinjanator_plugin_ansible-23.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2125 2023-07-24 20:11:46.000000 jinjanator_plugin_ansible-23.2.0/PKG-INFO
```

### Comparing `jinjanator_plugin_ansible-23.1.0/CHANGELOG.md` & `jinjanator_plugin_ansible-23.2.0/CHANGELOG.md`

 * *Files 15% similar despite different names*

```diff
@@ -24,10 +24,24 @@
 This changelog is managed by towncrier and is compiled at release time.
 
 See https://github.com/kpfleming/jinjanator/blob/main/.github/CONTRIBUTING.md#changelog for details.
 -->
 
 <!-- towncrier release notes start -->
 
+## [23.2.0](https://github.com/kpfleming/jinjanator/tree/23.2.0) - 2023-07-24
+
+### Backwards-incompatible Changes
+
+- Increased minimum Python version to 3.9 to ensure Ansible compatibility.
+  [#1](https://github.com/kpfleming/jinjanator-plugin-ansible/issues/1)
+
+
+### Additions
+
+- Add remaining filters and tests from the base Ansible collection.
+  [#1](https://github.com/kpfleming/jinjanator-plugin-ansible/issues/1)
+
+
 ## [23.1.0](https://github.com/kpfleming/jinjanator/tree/23.1.0) - 2023-07-24
 
 Initial release!
```

### Comparing `jinjanator_plugin_ansible-23.1.0/README.md` & `jinjanator_plugin_ansible-23.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # jinjanator-plugin-ansible
 
 <a href="https://opensource.org"><img height="150" align="left" src="https://opensource.org/files/OSIApprovedCropped.png" alt="Open Source Initiative Approved License logo"></a>
 [![CI](https://github.com/kpfleming/jinjanator-plugin-ansible/workflows/CI%20checks/badge.svg)](https://github.com/kpfleming/jinjanator-plugin-ansible/actions?query=workflow%3ACI%20checks)
-[![Python](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-3812/)
+[![Python](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/release/python-3912/)
 [![License - Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-9400d3.svg)](https://spdx.org/licenses/Apache-2.0.html)
 [![Code Style - Black](https://img.shields.io/badge/Code%20Style-Black-000000.svg)](https://github.com/psf/black)
 [![Types - Mypy](https://img.shields.io/badge/Types-Mypy-blue.svg)](https://github.com/python/mypy)
 [![Code Quality - Ruff](https://img.shields.io/badge/Code%20Quality-Ruff-red.svg)](https://github.com/astral-sh/ruff)
 [![Project Management - Hatch](https://img.shields.io/badge/Project%20Management-Hatch-purple.svg)](https://github.com/pypa/hatch)
 [![Testing - Pytest](https://img.shields.io/badge/Testing-Pytest-orange.svg)](https://github.com/pytest-dev/pytest)
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 # jinjanator-plugin-ansible [Open_Source_Initiative_Approved_License_logo] [!
 [CI](https://github.com/kpfleming/jinjanator-plugin-ansible/workflows/
 CI%20checks/badge.svg)](https://github.com/kpfleming/jinjanator-plugin-ansible/
 actions?query=workflow%3ACI%20checks) [![Python](https://img.shields.io/badge/
-python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-3812/)
+python-3.9+-blue.svg)](https://www.python.org/downloads/release/python-3912/)
 [![License - Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-
 9400d3.svg)](https://spdx.org/licenses/Apache-2.0.html) [![Code Style - Black]
 (https://img.shields.io/badge/Code%20Style-Black-000000.svg)](https://
 github.com/psf/black) [![Types - Mypy](https://img.shields.io/badge/Types-Mypy-
 blue.svg)](https://github.com/python/mypy) [![Code Quality - Ruff](https://
 img.shields.io/badge/Code%20Quality-Ruff-red.svg)](https://github.com/astral-
 sh/ruff) [![Project Management - Hatch](https://img.shields.io/badge/
```

### Comparing `jinjanator_plugin_ansible-23.1.0/src/jinjanator_plugin_ansible/plugin.py` & `jinjanator_plugin_ansible-23.2.0/src/jinjanator_plugin_ansible/plugin.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,45 @@
 from __future__ import annotations
 
 from typing import cast
 
-from ansible.plugins.filter.core import FilterModule  # type: ignore[import]
-from ansible.plugins.test.core import TestModule  # type: ignore[import]
+import ansible.plugins.filter.core as filter_core  # type: ignore[import]
+import ansible.plugins.filter.mathstuff as filter_mathstuff  # type: ignore[import]
+import ansible.plugins.filter.urls as filter_urls  # type: ignore[import]
+import ansible.plugins.filter.urlsplit as filter_urlsplit  # type: ignore[import]
+import ansible.plugins.test.core as test_core  # type: ignore[import]
+import ansible.plugins.test.files as test_files  # type: ignore[import]
+import ansible.plugins.test.mathstuff as test_mathstuff  # type: ignore[import]
+import ansible.plugins.test.uri as test_uri  # type: ignore[import]
+
 from jinjanator_plugins import (
     Filters,
     Tests,
     plugin_filters_hook,
     plugin_tests_hook,
 )
 
 
 @plugin_filters_hook
 def plugin_filters() -> Filters:
-    return cast(Filters, FilterModule().filters())
+    return cast(
+        Filters,
+        {
+            **filter_core.FilterModule().filters(),
+            **filter_mathstuff.FilterModule().filters(),
+            **filter_urls.FilterModule().filters(),
+            **filter_urlsplit.FilterModule().filters(),
+        },
+    )
 
 
 @plugin_tests_hook
 def plugin_tests() -> Tests:
-    return cast(Tests, TestModule().tests())
+    return cast(
+        Tests,
+        {
+            **test_core.TestModule().tests(),
+            **test_files.TestModule().tests(),
+            **test_mathstuff.TestModule().tests(),
+            **test_uri.TestModule().tests(),
+        },
+    )
```

### Comparing `jinjanator_plugin_ansible-23.1.0/tests/test_plugin.py` & `jinjanator_plugin_ansible-23.2.0/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `jinjanator_plugin_ansible-23.1.0/LICENSE` & `jinjanator_plugin_ansible-23.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jinjanator_plugin_ansible-23.1.0/pyproject.toml` & `jinjanator_plugin_ansible-23.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,24 +9,23 @@
 [project]
 name = "jinjanator-plugin-ansible"
 description = "Plugin which provides Ansible filters and tests to the Jinjanator tool"
 license = { text="Apache-2.0" }
 authors = [
   { name="Kevin P. Fleming", email="jinjanator@kevin.km6g.us" },
 ]
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Environment :: Console",
   "Intended Audience :: Developers",
   "Intended Audience :: System Administrators",
   "Natural Language :: English",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3 :: Only",
-  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Typing :: Typed",
 ]
 dynamic = [
   "readme",
@@ -114,15 +113,14 @@
     "pytest",
     "pytest-cov",
     "pytest-icdiff",
 ]
 
 [[tool.hatch.envs.ci.matrix]]
 python = [
-"3.8",
 "3.9",
 "3.10",
 "3.11",
 "3.12",
 ]
 
 [tool.hatch.envs.ci.scripts]
@@ -155,15 +153,15 @@
 text = """
 ## Release Information
 """
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
 path = "CHANGELOG.md"
 start-after = "<!-- towncrier release notes start -->"
-# pattern = "\n(###.+?\n)## "
+pattern = "\n(###.+?\n)## "
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
 text = """
 ---
 [→ Full Changelog](https://github.com/kpfleming/jinjanator-plugin-ansible/blob/main/CHANGELOG.md)
 """
 
@@ -177,15 +175,15 @@
 
 [tool.black]
 line-length = 90
 
 [tool.ruff]
 src = ["src", "tests"]
 format = "grouped"
-target-version = "py38"
+target-version = "py39"
 select = ["ALL"]
 
 ignore = [
   "ANN",      # Mypy is better at this.
   "C901",     # Leave complexity to me.
   "COM",      # Leave commas to Black.
   "D",        # We have different ideas about docstrings.
@@ -215,15 +213,15 @@
 ]
 addopts = [
     "-ra",
     "--strict-markers",
 ]
 
 [tool.mypy]
-python_version = 3.8
+python_version = 3.9
 namespace_packages = true
 explicit_package_bases = true
 check_untyped_defs = true
 disallow_any_generics = true
 disallow_incomplete_defs = true
 disallow_subclassing_any = true
 disallow_untyped_calls = true
```

### Comparing `jinjanator_plugin_ansible-23.1.0/PKG-INFO` & `jinjanator_plugin_ansible-23.2.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: jinjanator-plugin-ansible
-Version: 23.1.0
+Version: 23.2.0
 Summary: Plugin which provides Ansible filters and tests to the Jinjanator tool
 Project-URL: Bug Tracker, https://github.com/kpfleming/jinjanator-plugin-ansible/issues
 Project-URL: Homepage, https://github.com/kpfleming/jinjanator-plugin-ansible
 Author-email: "Kevin P. Fleming" <jinjanator@kevin.km6g.us>
 License: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Requires-Dist: ansible-core
 Requires-Dist: jinjanator-plugins==23.1.*
 Description-Content-Type: text/markdown
 
 # *jinjanator-plugin-ansible*: Makes Ansible's filters and tests available in Jinjanator
 
 
@@ -40,14 +39,21 @@
 
 ## Usage
 
 The Ansible filters and tests can be used in templates using the same
 names that would be used if the template was rendered by Ansible
 itself.
 ## Release Information
+### Backwards-incompatible Changes
 
+- Increased minimum Python version to 3.9 to ensure Ansible compatibility.
+  [[#1](https://github.com/kpfleming/jinjanator-plugin-ansible/issues/1)](https://github.com/kpfleming/jinjanator-plugin-ansible/issues/1)
+
+
+### Additions
+
+- Add remaining filters and tests from the base Ansible collection.
+  [[#1](https://github.com/kpfleming/jinjanator-plugin-ansible/issues/1)](https://github.com/kpfleming/jinjanator-plugin-ansible/issues/1)
 
-## [23.1.0](https://github.com/kpfleming/jinjanator/tree/23.1.0) - 2023-07-24
 
-Initial release!
 ---
 [→ Full Changelog](https://github.com/kpfleming/jinjanator-plugin-ansible/blob/main/CHANGELOG.md)
```

