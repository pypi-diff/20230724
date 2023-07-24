# Comparing `tmp/extension-helpers-1.0.0.tar.gz` & `tmp/extension-helpers-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extension-helpers-1.0.0.tar", last modified: Wed Mar 16 21:44:51 2022, max compression
+gzip compressed data, was "extension-helpers-1.1.0.tar", last modified: Mon Jul 24 20:12:03 2023, max compression
```

## Comparing `extension-helpers-1.0.0.tar` & `extension-helpers-1.1.0.tar`

### file list

```diff
@@ -1,48 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 21:44:51.766397 extension-helpers-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 21:44:51.762397 extension-helpers-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 21:44:51.762397 extension-helpers-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1131 2022-03-16 21:44:31.000000 extension-helpers-1.0.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)      653 2022-03-16 21:44:31.000000 extension-helpers-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-03-16 21:44:31.000000 extension-helpers-1.0.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)      430 2022-03-16 21:44:31.000000 extension-helpers-1.0.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)      493 2022-03-16 21:44:31.000000 extension-helpers-1.0.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1491 2022-03-16 21:44:31.000000 extension-helpers-1.0.0/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-03-16 21:44:31.000000 extension-helpers-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1832 2022-03-16 21:44:51.766397 extension-helpers-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-03-16 21:44:31.000000 extension-helpers-1.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-03-16 21:44:31.000000 extension-helpers-1.0.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 21:44:51.762397 extension-helpers-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-03-16 21:44:31.000000 extension-helpers-1.0.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-03-16 21:44:31.000000 extension-helpers-1.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1579 2022-03-16 21:44:31.000000 extension-helpers-1.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      619 2022-03-16 21:44:31.000000 extension-helpers-1.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      787 2022-03-16 21:44:31.000000 extension-helpers-1.0.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-03-16 21:44:31.000000 extension-helpers-1.0.0/docs/openmp.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1865 2022-03-16 21:44:31.000000 extension-helpers-1.0.0/docs/using.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 21:44:51.762397 extension-helpers-1.0.0/extension_helpers/
--rw-r--r--   0 runner    (1001) docker     (121)      818 2022-03-16 21:44:31.000000 extension-helpers-1.0.0/extension_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9279 2022-03-16 21:44:31.000000 extension-helpers-1.0.0/extension_helpers/_openmp_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)    10169 2022-03-16 21:44:31.000000 extension-helpers-1.0.0/extension_helpers/_setup_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     4161 2022-03-16 21:44:31.000000 extension-helpers-1.0.0/extension_helpers/_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2385 2022-03-16 21:44:31.000000 extension-helpers-1.0.0/extension_helpers/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 21:44:51.766397 extension-helpers-1.0.0/extension_helpers/src/
--rw-r--r--   0 runner    (1001) docker     (121)     2720 2022-03-16 21:44:31.000000 extension-helpers-1.0.0/extension_helpers/src/compiler.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 21:44:51.766397 extension-helpers-1.0.0/extension_helpers/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     4446 2022-03-16 21:44:31.000000 extension-helpers-1.0.0/extension_helpers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1618 2022-03-16 21:44:31.000000 extension-helpers-1.0.0/extension_helpers/tests/test_openmp_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     8648 2022-03-16 21:44:31.000000 extension-helpers-1.0.0/extension_helpers/tests/test_setup_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)      696 2022-03-16 21:44:31.000000 extension-helpers-1.0.0/extension_helpers/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-03-16 21:44:50.000000 extension-helpers-1.0.0/extension_helpers/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 21:44:51.766397 extension-helpers-1.0.0/extension_helpers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1832 2022-03-16 21:44:51.000000 extension-helpers-1.0.0/extension_helpers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      974 2022-03-16 21:44:51.000000 extension-helpers-1.0.0/extension_helpers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-16 21:44:51.000000 extension-helpers-1.0.0/extension_helpers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-03-16 21:44:51.000000 extension-helpers-1.0.0/extension_helpers.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-16 21:44:50.000000 extension-helpers-1.0.0/extension_helpers.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-03-16 21:44:51.000000 extension-helpers-1.0.0/extension_helpers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-03-16 21:44:51.000000 extension-helpers-1.0.0/extension_helpers.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 21:44:51.766397 extension-helpers-1.0.0/licenses/
--rw-r--r--   0 runner    (1001) docker     (121)     1644 2022-03-16 21:44:31.000000 extension-helpers-1.0.0/licenses/LICENSE_ASTROSCRAPPY.rst
--rw-r--r--   0 runner    (1001) docker     (121)      210 2022-03-16 21:44:31.000000 extension-helpers-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2091 2022-03-16 21:44:51.766397 extension-helpers-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1826 2022-03-16 21:44:31.000000 extension-helpers-1.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:12:03.736128 extension-helpers-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:12:03.728129 extension-helpers-1.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-24 20:11:43.000000 extension-helpers-1.1.0/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:12:03.728129 extension-helpers-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-24 20:11:43.000000 extension-helpers-1.1.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-24 20:11:43.000000 extension-helpers-1.1.0/.github/workflows/update-changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-24 20:11:43.000000 extension-helpers-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-24 20:11:43.000000 extension-helpers-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-24 20:11:43.000000 extension-helpers-1.1.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-24 20:11:43.000000 extension-helpers-1.1.0/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-24 20:11:43.000000 extension-helpers-1.1.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-24 20:11:43.000000 extension-helpers-1.1.0/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-24 20:11:43.000000 extension-helpers-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-24 20:12:03.736128 extension-helpers-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-24 20:11:43.000000 extension-helpers-1.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-24 20:11:43.000000 extension-helpers-1.1.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:12:03.732128 extension-helpers-1.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-24 20:11:43.000000 extension-helpers-1.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-24 20:11:43.000000 extension-helpers-1.1.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-24 20:11:43.000000 extension-helpers-1.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-24 20:11:43.000000 extension-helpers-1.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 20:11:43.000000 extension-helpers-1.1.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-24 20:11:43.000000 extension-helpers-1.1.0/docs/openmp.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-24 20:11:43.000000 extension-helpers-1.1.0/docs/using.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:12:03.732128 extension-helpers-1.1.0/extension_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-07-24 20:11:43.000000 extension-helpers-1.1.0/extension_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-07-24 20:11:43.000000 extension-helpers-1.1.0/extension_helpers/_openmp_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-07-24 20:11:43.000000 extension-helpers-1.1.0/extension_helpers/_setup_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-07-24 20:11:43.000000 extension-helpers-1.1.0/extension_helpers/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-24 20:11:43.000000 extension-helpers-1.1.0/extension_helpers/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:12:03.736128 extension-helpers-1.1.0/extension_helpers/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-07-24 20:11:43.000000 extension-helpers-1.1.0/extension_helpers/src/compiler.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:12:03.736128 extension-helpers-1.1.0/extension_helpers/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-07-24 20:11:43.000000 extension-helpers-1.1.0/extension_helpers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-24 20:11:43.000000 extension-helpers-1.1.0/extension_helpers/tests/test_openmp_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9700 2023-07-24 20:11:43.000000 extension-helpers-1.1.0/extension_helpers/tests/test_setup_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-24 20:11:43.000000 extension-helpers-1.1.0/extension_helpers/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-24 20:12:03.000000 extension-helpers-1.1.0/extension_helpers/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:12:03.736128 extension-helpers-1.1.0/extension_helpers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-24 20:12:03.000000 extension-helpers-1.1.0/extension_helpers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-24 20:12:03.000000 extension-helpers-1.1.0/extension_helpers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 20:12:03.000000 extension-helpers-1.1.0/extension_helpers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-24 20:12:03.000000 extension-helpers-1.1.0/extension_helpers.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 20:12:03.000000 extension-helpers-1.1.0/extension_helpers.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-24 20:12:03.000000 extension-helpers-1.1.0/extension_helpers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 20:12:03.000000 extension-helpers-1.1.0/extension_helpers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:12:03.736128 extension-helpers-1.1.0/licenses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-24 20:11:43.000000 extension-helpers-1.1.0/licenses/LICENSE_ASTROSCRAPPY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-24 20:11:43.000000 extension-helpers-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-24 20:12:03.740129 extension-helpers-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-24 20:11:43.000000 extension-helpers-1.1.0/tox.ini
```

### Comparing `extension-helpers-1.0.0/.github/workflows/main.yml` & `extension-helpers-1.1.0/.github/workflows/main.yml`

 * *Files 14% similar despite different names*

```diff
@@ -12,27 +12,29 @@
       coverage: codecov
       envs: |
         # Code style
         - linux: style
         # Docs
         - linux: build_docs
         # Standard tests
-        - linux: py36-test-oldestdeps
-        - linux: py37-test
+        - linux: py37-test-oldestdeps
         - linux: py38-test
-        - linux: py38-test-dev
-        - macos: py38-test-dev
+        - linux: py39-test
+        - linux: py310-test
+        - linux: py311-test
+        - linux: py39-test-dev
+        - macos: py39-test-dev
           posargs: --openmp-expected=False
-        - windows: py36-test
+        - windows: py38-test
           runs-on: windows-2019
-        - windows: py38-test-dev
+        - windows: py39-test-dev
           runs-on: windows-2019
         # Test with more compilers, for the OpenMP helpers
-        - macos: py38-test-osxclang-conda
-        - linux: py38-test-linuxgcc-conda
+        - macos: py39-test-osxclang-conda
+        - linux: py39-test-linuxgcc-conda
         # Test downstream packages
         - linux: py39-downstream
   publish:
     needs: tests
     uses: OpenAstronomy/github-actions-workflows/.github/workflows/publish_pure_python.yml@v1
     with:
       test_extras: test
```

### Comparing `extension-helpers-1.0.0/.gitignore` & `extension-helpers-1.1.0/.gitignore`

 * *Files 18% similar despite different names*

```diff
@@ -52,7 +52,10 @@
 .DS_Store
 
 # PyCharm
 .idea
 
 # Hypothesis
 .hypothesis
+
+# vscode
+settings.json
```

### Comparing `extension-helpers-1.0.0/LICENSE.rst` & `extension-helpers-1.1.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `extension-helpers-1.0.0/PKG-INFO` & `extension-helpers-1.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: extension-helpers
-Version: 1.0.0
+Version: 1.1.0
 Summary: Utilities for building and installing packages with compiled extensions
 Home-page: https://github.com/astropy/extension-helpers
 Author: The Astropy Developers
 Author-email: astropy.team@gmail.com
 License: BSD 3-Clause License
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: Setuptools Plugin
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Archiving :: Packaging
 Provides: extension_helpers
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE.rst
 
 extension-helpers
 =================
 
@@ -38,9 +37,7 @@
 
 The **extension-helpers** package includes convenience helpers to assist with
 building Python packages with compiled C/Cython extensions. It is developed by
 the Astropy project but is intended to be general and usable by any Python
 package.
 
 For more information, see the documentation at http://extension-helpers.readthedocs.io
-
-
```

### Comparing `extension-helpers-1.0.0/README.rst` & `extension-helpers-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `extension-helpers-1.0.0/docs/Makefile` & `extension-helpers-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `extension-helpers-1.0.0/docs/conf.py` & `extension-helpers-1.1.0/docs/conf.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,55 +1,52 @@
-# -*- coding: utf-8 -*-
-
-import sys
 from pkg_resources import get_distribution
 
-project = 'extension-helpers'
-copyright = '2019, The Astropy Developers'
-author = 'The Astropy Developers'
+project = "extension-helpers"
+copyright = "2019, The Astropy Developers"
+author = "The Astropy Developers"
 
 # We need to get the version number from the package
-version = release = get_distribution('extension-helpers').version
+version = release = get_distribution("extension-helpers").version
 
 extensions = [
-    'sphinx.ext.autodoc',
-    'sphinx.ext.doctest',
-    'sphinx.ext.intersphinx',
-    'sphinx.ext.napoleon',
-    'sphinx_automodapi.automodapi'
+    "sphinx.ext.autodoc",
+    "sphinx.ext.doctest",
+    "sphinx.ext.intersphinx",
+    "sphinx.ext.napoleon",
+    "sphinx_automodapi.automodapi",
 ]
 
-intersphinx_mapping = {'https://docs.python.org/3/': None}
+intersphinx_mapping = {"python": ("https://docs.python.org/3/", None)}
 
 # The suffix(es) of source filenames.
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = 'alabaster'
+html_theme = "alabaster"
 
 html_theme_options = {
     "description": "A build time package to simplify C/Cython extensions.",
     "code_font_family": "'Fira Code', monospace",
     "github_user": "astropy",
     "github_repo": "extension-helpers",
-    "sidebar_width": "300px"
+    "sidebar_width": "300px",
 }
 
 # Enable nitpicky mode to pick reference issues
-default_role = 'obj'
+default_role = "obj"
 nitpicky = True
```

### Comparing `extension-helpers-1.0.0/docs/index.rst` & `extension-helpers-1.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `extension-helpers-1.0.0/docs/make.bat` & `extension-helpers-1.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `extension-helpers-1.0.0/docs/openmp.rst` & `extension-helpers-1.1.0/docs/openmp.rst`

 * *Files identical despite different names*

### Comparing `extension-helpers-1.0.0/docs/using.rst` & `extension-helpers-1.1.0/docs/using.rst`

 * *Files 15% similar despite different names*

```diff
@@ -41,7 +41,17 @@
 compilers used.
 
 It is also possible to enable extension-helpers in ``setup.cfg`` instead of
 ``setup.py`` by adding the following configuration to the ``setup.cfg`` file::
 
     [extension-helpers]
     use_extension_helpers = true
+
+Moreover, one can also enable extension-helpers in ``pyproject.toml`` by adding
+the following configuration to the ``pyproject.toml`` file::
+
+    [tool.extension-helpers]
+    use_extension_helpers = true
+
+.. note::
+  For backwards compatibility, the setting of ``use_extension_helpers`` in
+  ``setup.cfg`` will override any setting of it in ``pyproject.toml``.
```

### Comparing `extension-helpers-1.0.0/extension_helpers/_openmp_helpers.py` & `extension-helpers-1.1.0/extension_helpers/_openmp_helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import tempfile
 import subprocess
 
 from setuptools.command.build_ext import customize_compiler, get_config_var, new_compiler
 
 from ._setup_helpers import get_compiler
 
-__all__ = ['add_openmp_flags_if_available']
+__all__ = ["add_openmp_flags_if_available"]
 
 try:
     # Check if this has already been instantiated, only set the default once.
     _EXTENSION_HELPERS_DISABLE_OPENMP_SETUP_
 except NameError:
     import builtins
 
@@ -44,15 +44,22 @@
   #pragma omp parallel
   printf("nthreads=%d\\n", omp_get_num_threads());
   return 0;
 }
 """
 
 
-def _get_flag_value_from_var(flag, var, delim=' '):
+CCODE_ICX = """
+#ifndef __INTEL_LLVM_COMPILER
+#error This is not the Intel oneAPI compiler
+#endif
+"""
+
+
+def _get_flag_value_from_var(flag, var, delim=" "):
     """
     Extract flags from an environment variable.
 
     Parameters
     ----------
     flag : str
         The flag to extract, for example '-I' or '-L'
@@ -73,15 +80,15 @@
     -----
     Environment variables are first checked in ``os.environ[var]``, then in
     ``distutils.sysconfig.get_config_var(var)``.
 
     This function is not supported on Windows.
     """
 
-    if sys.platform.startswith('win'):
+    if sys.platform.startswith("win"):
         return None
 
     # Simple input validation
     if not var or not flag:
         return None
     flag_length = len(flag)
     if not flag_length:
@@ -99,14 +106,52 @@
     # Extract flag from {var:value}
     if flags:
         for item in flags.split(delim):
             if item.startswith(flag):
                 return item[flag_length:]
 
 
+def _check_if_compiler_is_icx():
+    """
+    Check whether the compiler is the Intel oneAPI compiler.
+
+    Returns
+    -------
+    result : bool
+        `True` if the test passed, `False` otherwise.
+    """
+
+    ccompiler = new_compiler()
+    customize_compiler(ccompiler)
+
+    with tempfile.TemporaryDirectory() as tmp_dir:
+        start_dir = os.path.abspath(".")
+
+        try:
+            os.chdir(tmp_dir)
+
+            # Write test program
+            with open("test_icx.c", "w") as f:
+                f.write(CCODE_ICX)
+
+            os.mkdir("objects")
+
+            # Compile program
+            ccompiler.compile(["test_icx.c"], output_dir="objects")
+        except Exception:
+            is_icx = False
+        else:
+            is_icx = True
+
+        finally:
+            os.chdir(start_dir)
+
+    return is_icx
+
+
 def get_openmp_flags():
     """
     Utility for returning compiler and linker flags possibly needed for
     OpenMP support.
 
     Returns
     -------
@@ -117,31 +162,35 @@
     The flags returned are not tested for validity, use
     `check_openmp_support(openmp_flags=get_openmp_flags())` to do so.
     """
 
     compile_flags = []
     link_flags = []
 
-    if get_compiler() == 'msvc':
-        compile_flags.append('-openmp')
+    if get_compiler() == "msvc":
+        compile_flags.append("-openmp")
     else:
-
-        include_path = _get_flag_value_from_var('-I', 'CFLAGS')
+        include_path = _get_flag_value_from_var("-I", "CFLAGS")
         if include_path:
-            compile_flags.append('-I' + include_path)
+            compile_flags.append("-I" + include_path)
 
-        lib_path = _get_flag_value_from_var('-L', 'LDFLAGS')
+        lib_path = _get_flag_value_from_var("-L", "LDFLAGS")
         if lib_path:
-            link_flags.append('-L' + lib_path)
-            link_flags.append('-Wl,-rpath,' + lib_path)
+            link_flags.append("-L" + lib_path)
+            link_flags.append("-Wl,-rpath," + lib_path)
+
+        if _check_if_compiler_is_icx():
+            openmp_flags = "-qopenmp"
+        else:
+            openmp_flags = "-fopenmp"
 
-        compile_flags.append('-fopenmp')
-        link_flags.append('-fopenmp')
+        compile_flags.append(openmp_flags)
+        link_flags.append(openmp_flags)
 
-    return {'compiler_flags': compile_flags, 'linker_flags': link_flags}
+    return {"compiler_flags": compile_flags, "linker_flags": link_flags}
 
 
 def check_openmp_support(openmp_flags=None):
     """
     Check whether OpenMP test code can be compiled and run.
 
     Parameters
@@ -168,53 +217,52 @@
         # If the key is missing in os.environ it is not extracted from
         # sysconfig.get_config_var(). E.g. 'LDFLAGS' get left out, preventing
         # clang from finding libomp.dylib because -L<path> is not passed to
         # linker. Call get_openmp_flags() to get flags missed by
         # customize_compiler().
         openmp_flags = get_openmp_flags()
 
-    compile_flags = openmp_flags.get('compiler_flags')
-    link_flags = openmp_flags.get('linker_flags')
+    compile_flags = openmp_flags.get("compiler_flags")
+    link_flags = openmp_flags.get("linker_flags")
 
     with tempfile.TemporaryDirectory() as tmp_dir:
-        start_dir = os.path.abspath('.')
+        start_dir = os.path.abspath(".")
 
         try:
             os.chdir(tmp_dir)
 
             # Write test program
-            with open('test_openmp.c', 'w') as f:
+            with open("test_openmp.c", "w") as f:
                 f.write(CCODE)
 
-            os.mkdir('objects')
+            os.mkdir("objects")
 
             # Compile, test program
-            ccompiler.compile(['test_openmp.c'], output_dir='objects',
-                              extra_postargs=compile_flags)
+            ccompiler.compile(["test_openmp.c"], output_dir="objects", extra_postargs=compile_flags)
 
             # Link test program
-            objects = glob.glob(os.path.join('objects', '*' + ccompiler.obj_extension))
-            ccompiler.link_executable(objects, 'test_openmp',
-                                      extra_postargs=link_flags)
+            objects = glob.glob(os.path.join("objects", "*" + ccompiler.obj_extension))
+            ccompiler.link_executable(objects, "test_openmp", extra_postargs=link_flags)
 
             # Run test program
-            output = subprocess.check_output('./test_openmp')
-            output = output.decode(sys.stdout.encoding or 'utf-8').splitlines()
+            output = subprocess.check_output("./test_openmp")
+            output = output.decode(sys.stdout.encoding or "utf-8").splitlines()
 
-            if 'nthreads=' in output[0]:
-                nthreads = int(output[0].strip().split('=')[1])
+            if "nthreads=" in output[0]:
+                nthreads = int(output[0].strip().split("=")[1])
                 if len(output) == nthreads:
                     is_openmp_supported = True
                 else:
-                    log.warn("Unexpected number of lines from output of test OpenMP "
-                             "program (output was {0})".format(output))
+                    log.warn(
+                        "Unexpected number of lines from output of test OpenMP "
+                        "program (output was {})".format(output)
+                    )
                     is_openmp_supported = False
             else:
-                log.warn("Unexpected output from test OpenMP "
-                         "program (output was {0})".format(output))
+                log.warn(f"Unexpected output from test OpenMP program (output was {output})")
                 is_openmp_supported = False
         except Exception:
             is_openmp_supported = False
 
         finally:
             os.chdir(start_dir)
 
@@ -222,77 +270,83 @@
 
 
 def is_openmp_supported():
     """
     Determine whether the build compiler has OpenMP support.
     """
     log_threshold = log.level
-    log.setLevel('CRITICAL')
+    log.setLevel("CRITICAL")
     ret = check_openmp_support()
     log.setLevel(log_threshold)
     return ret
 
 
 def add_openmp_flags_if_available(extension):
     """
     Add OpenMP compilation flags, if supported (if not a warning will be
     printed to the console and no flags will be added.)
 
     Returns `True` if the flags were added, `False` otherwise.
     """
 
-    if _EXTENSION_HELPERS_DISABLE_OPENMP_SETUP_:
+    if _EXTENSION_HELPERS_DISABLE_OPENMP_SETUP_:  # noqa: F821
         log.info("OpenMP support has been explicitly disabled.")
         return False
 
     openmp_flags = get_openmp_flags()
     using_openmp = check_openmp_support(openmp_flags=openmp_flags)
 
     if using_openmp:
-        compile_flags = openmp_flags.get('compiler_flags')
-        link_flags = openmp_flags.get('linker_flags')
+        compile_flags = openmp_flags.get("compiler_flags")
+        link_flags = openmp_flags.get("linker_flags")
         log.info("Compiling Cython/C/C++ extension with OpenMP support")
         extension.extra_compile_args.extend(compile_flags)
         extension.extra_link_args.extend(link_flags)
     else:
-        log.warn("Cannot compile Cython/C/C++ extension with OpenMP, reverting "
-                 "to non-parallel code")
+        log.warn(
+            "Cannot compile Cython/C/C++ extension with OpenMP, reverting to non-parallel code"
+        )
 
     return using_openmp
 
 
 _IS_OPENMP_ENABLED_SRC = """
 # Autogenerated by {packagename}'s setup.py on {timestamp!s}
 
 def is_openmp_enabled():
     \"\"\"
     Determine whether this package was built with OpenMP support.
     \"\"\"
     return {return_bool}
-"""[1:]
+"""[
+    1:
+]
 
 
-def generate_openmp_enabled_py(packagename, srcdir='.', disable_openmp=None):
+def generate_openmp_enabled_py(packagename, srcdir=".", disable_openmp=None):
     """
     Generate ``package.openmp_enabled.is_openmp_enabled``, which can then be used
     to determine, post build, whether the package was built with or without
     OpenMP support.
     """
 
-    epoch = int(os.environ.get('SOURCE_DATE_EPOCH', time.time()))
+    epoch = int(os.environ.get("SOURCE_DATE_EPOCH", time.time()))
     timestamp = datetime.datetime.utcfromtimestamp(epoch)
 
     if disable_openmp is not None:
         import builtins
+
         builtins._EXTENSION_HELPERS_DISABLE_OPENMP_SETUP_ = disable_openmp
-    if _EXTENSION_HELPERS_DISABLE_OPENMP_SETUP_:
+    if _EXTENSION_HELPERS_DISABLE_OPENMP_SETUP_:  # noqa: F821
         log.info("OpenMP support has been explicitly disabled.")
-    openmp_support = False if _EXTENSION_HELPERS_DISABLE_OPENMP_SETUP_ else is_openmp_supported()
+        openmp_support = False
+    else:
+        openmp_support = is_openmp_supported()
 
-    src = _IS_OPENMP_ENABLED_SRC.format(packagename=packagename,
-                                        timestamp=timestamp,
-                                        return_bool=openmp_support)
-
-    package_srcdir = os.path.join(srcdir, *packagename.split('.'))
-    is_openmp_enabled_py = os.path.join(package_srcdir, 'openmp_enabled.py')
-    with open(is_openmp_enabled_py, 'w') as f:
+    src = _IS_OPENMP_ENABLED_SRC.format(
+        packagename=packagename, timestamp=timestamp, return_bool=openmp_support
+    )
+
+    package_srcdir = os.path.join(srcdir, *packagename.split("."))
+    is_openmp_enabled_py = os.path.join(package_srcdir, "openmp_enabled.py")
+    with open(is_openmp_enabled_py, "w") as f:
         f.write(src)
```

### Comparing `extension-helpers-1.0.0/extension_helpers/_setup_helpers.py` & `extension-helpers-1.1.0/extension_helpers/_setup_helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from collections import defaultdict
 
 from setuptools import Extension, find_packages
 from setuptools.command.build_ext import new_compiler
 
 from ._utils import import_file, walk_skip_hidden
 
-__all__ = ['get_compiler', 'get_extensions', 'pkg_config']
+__all__ = ["get_compiler", "get_extensions", "pkg_config"]
 
 log = logging.getLogger(__name__)
 
 
 def get_compiler():
     """
     Determines the compiler that will be used to build extension modules.
@@ -32,15 +32,15 @@
         command; or the default compiler for the platform if none was
         specified.
 
     """
     return new_compiler().compiler_type
 
 
-def get_extensions(srcdir='.'):
+def get_extensions(srcdir="."):
     """
     Collect all extensions from Cython files and ``setup_package.py`` files.
 
     If numpy is importable, the numpy include path will be added to all Cython
     extensions which are automatically generated.
 
     This function obtains that information by iterating through all
@@ -53,80 +53,83 @@
     packages = []
     package_dir = {}
 
     # Use the find_packages tool to locate all packages and modules
     packages = find_packages(srcdir)
 
     # Update package_dir if the package lies in a subdirectory
-    if srcdir != '.':
-        package_dir[''] = srcdir
+    if srcdir != ".":
+        package_dir[""] = srcdir
 
     for setuppkg in iter_setup_packages(srcdir, packages):
         # get_extensions must include any Cython extensions by their .pyx
         # filename.
-        if hasattr(setuppkg, 'get_extensions'):
+        if hasattr(setuppkg, "get_extensions"):
             ext_modules.extend(setuppkg.get_extensions())
 
     # Locate any .pyx files not already specified, and add their extensions in.
     # The default include dirs include numpy to facilitate numerical work.
     includes = []
     try:
         import numpy
+
         includes = [numpy.get_include()]
     except ImportError:
         pass
 
     ext_modules.extend(get_cython_extensions(srcdir, packages, ext_modules, includes))
 
     # Now remove extensions that have the special name 'skip_cython', as they
     # exist Only to indicate that the cython extensions shouldn't be built
     for i, ext in reversed(list(enumerate(ext_modules))):
-        if ext.name == 'skip_cython':
+        if ext.name == "skip_cython":
             del ext_modules[i]
 
     # On Microsoft compilers, we need to pass the '/MANIFEST'
     # commandline argument.  This was the default on MSVC 9.0, but is
     # now required on MSVC 10.0, but it doesn't seem to hurt to add
     # it unconditionally.
-    if get_compiler() == 'msvc':
+    if get_compiler() == "msvc":
         for ext in ext_modules:
-            ext.extra_link_args.append('/MANIFEST')
+            ext.extra_link_args.append("/MANIFEST")
 
     if len(ext_modules) > 0:
         main_package_dir = min(packages, key=len)
-        src_path = os.path.join(os.path.dirname(__file__), 'src')
-        shutil.copy(os.path.join(src_path, 'compiler.c'),
-                    os.path.join(srcdir, main_package_dir, '_compiler.c'))
-        ext = Extension(main_package_dir + '.compiler_version',
-                        [os.path.join(main_package_dir, '_compiler.c')])
+        src_path = os.path.join(os.path.dirname(__file__), "src")
+        shutil.copy(
+            os.path.join(src_path, "compiler.c"),
+            os.path.join(srcdir, main_package_dir, "_compiler.c"),
+        )
+        ext = Extension(
+            main_package_dir + ".compiler_version", [os.path.join(main_package_dir, "_compiler.c")]
+        )
         ext_modules.append(ext)
 
     return ext_modules
 
 
 def iter_setup_packages(srcdir, packages):
-    """ A generator that finds and imports all of the ``setup_package.py``
+    """A generator that finds and imports all of the ``setup_package.py``
     modules in the source packages.
 
     Returns
     -------
     modgen : generator
         A generator that yields (modname, mod), where `mod` is the module and
         `modname` is the module name for the ``setup_package.py`` modules.
 
     """
 
     for packagename in packages:
-        package_parts = packagename.split('.')
+        package_parts = packagename.split(".")
         package_path = os.path.join(srcdir, *package_parts)
-        setup_package = os.path.join(package_path, 'setup_package.py')
+        setup_package = os.path.join(package_path, "setup_package.py")
 
         if os.path.isfile(setup_package):
-            module = import_file(setup_package,
-                                 name=packagename + '.setup_package')
+            module = import_file(setup_package, name=packagename + ".setup_package")
             yield module
 
 
 def iter_pyx_files(package_dir, package_name):
     """
     A generator that yields Cython source files (ending in '.pyx') in the
     source packages.
@@ -137,25 +140,24 @@
         A generator that yields (extmod, fullfn) where `extmod` is the
         full name of the module that the .pyx file would live in based
         on the source directory structure, and `fullfn` is the path to
         the .pyx file.
     """
     for dirpath, dirnames, filenames in walk_skip_hidden(package_dir):
         for fn in filenames:
-            if fn.endswith('.pyx'):
+            if fn.endswith(".pyx"):
                 fullfn = os.path.join(dirpath, fn)
                 # Package must match file name
-                extmod = '.'.join([package_name, fn[:-4]])
+                extmod = ".".join([package_name, fn[:-4]])
                 yield (extmod, fullfn)
 
         break  # Don't recurse into subdirectories
 
 
-def get_cython_extensions(srcdir, packages, prevextensions=tuple(),
-                          extincludedirs=None):
+def get_cython_extensions(srcdir, packages, prevextensions=tuple(), extincludedirs=None):
     """
     Looks for Cython files and generates Extensions if needed.
 
     Parameters
     ----------
     srcdir : str
         Path to the root of the source directory to search.
@@ -180,32 +182,31 @@
     # for .c files with the same remaining filename. So we look for .pyx and
     # .c files, and we strip the extension.
     prevsourcepaths = []
     ext_modules = []
 
     for ext in prevextensions:
         for s in ext.sources:
-            if s.endswith(('.pyx', '.c', '.cpp')):
+            if s.endswith((".pyx", ".c", ".cpp")):
                 sourcepath = os.path.realpath(os.path.splitext(s)[0])
                 prevsourcepaths.append(sourcepath)
 
     for package_name in packages:
-        package_parts = package_name.split('.')
+        package_parts = package_name.split(".")
         package_path = os.path.join(srcdir, *package_parts)
 
         for extmod, pyxfn in iter_pyx_files(package_path, package_name):
             sourcepath = os.path.realpath(os.path.splitext(pyxfn)[0])
             if sourcepath not in prevsourcepaths:
-                ext_modules.append(Extension(extmod, [pyxfn],
-                                             include_dirs=extincludedirs))
+                ext_modules.append(Extension(extmod, [pyxfn], include_dirs=extincludedirs))
 
     return ext_modules
 
 
-def pkg_config(packages, default_libraries, executable='pkg-config'):
+def pkg_config(packages, default_libraries, executable="pkg-config"):
     """
     Uses pkg-config to update a set of distutils Extension arguments
     to include the flags necessary to link against the given packages.
 
     If the pkg-config lookup fails, default_libraries is applied to
     libraries.
 
@@ -229,54 +230,57 @@
         - ``libraries``: A list of libraries
         - ``define_macros``: A list of macro defines
         - ``undef_macros``: A list of macros to undefine
         - ``extra_compile_args``: A list of extra arguments to pass to
           the compiler
     """
 
-    flag_map = {'-I': 'include_dirs', '-L': 'library_dirs', '-l': 'libraries',
-                '-D': 'define_macros', '-U': 'undef_macros'}
-    command = "{0} --libs --cflags {1}".format(executable, ' '.join(packages)),
+    flag_map = {
+        "-I": "include_dirs",
+        "-L": "library_dirs",
+        "-l": "libraries",
+        "-D": "define_macros",
+        "-U": "undef_macros",
+    }
+    command = f"{executable} --libs --cflags {' '.join(packages)}"
 
     result = defaultdict(list)
 
     try:
         pipe = subprocess.Popen(command, shell=True, stdout=subprocess.PIPE)
         output = pipe.communicate()[0].strip()
     except subprocess.CalledProcessError as e:
         lines = [
-            ("{0} failed. This may cause the build to fail below."
-             .format(executable)),
-            "  command: {0}".format(e.cmd),
-            "  returncode: {0}".format(e.returncode),
-            "  output: {0}".format(e.output)
-            ]
-        log.warn('\n'.join(lines))
-        result['libraries'].extend(default_libraries)
+            (f"{executable} failed. This may cause the build to fail below."),
+            f"  command: {e.cmd}",
+            f"  returncode: {e.returncode}",
+            f"  output: {e.output}",
+        ]
+        log.warn("\n".join(lines))
+        result["libraries"].extend(default_libraries)
     else:
         if pipe.returncode != 0:
             lines = [
-                "pkg-config could not lookup up package(s) {0}.".format(
-                    ", ".join(packages)),
-                "This may cause the build to fail below."
-                ]
-            log.warn('\n'.join(lines))
-            result['libraries'].extend(default_libraries)
+                f"pkg-config could not lookup up package(s) {', '.join(packages)}.",
+                "This may cause the build to fail below.",
+            ]
+            log.warn("\n".join(lines))
+            result["libraries"].extend(default_libraries)
         else:
             for token in output.split():
                 # It's not clear what encoding the output of
                 # pkg-config will come to us in.  It will probably be
                 # some combination of pure ASCII (for the compiler
                 # flags) and the filesystem encoding (for any argument
                 # that includes directories or filenames), but this is
                 # just conjecture, as the pkg-config documentation
                 # doesn't seem to address it.
-                arg = token[:2].decode('ascii')
+                arg = token[:2].decode("ascii")
                 value = token[2:].decode(sys.getfilesystemencoding())
                 if arg in flag_map:
-                    if arg == '-D':
-                        value = tuple(value.split('=', 1))
+                    if arg == "-D":
+                        value = tuple(value.split("=", 1))
                     result[flag_map[arg]].append(value)
                 else:
-                    result['extra_compile_args'].append(value)
+                    result["extra_compile_args"].append(value)
 
     return result
```

### Comparing `extension-helpers-1.0.0/extension_helpers/_utils.py` & `extension-helpers-1.1.0/extension_helpers/_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 
 import os
 import sys
-import glob
-import contextlib
 from importlib import machinery as import_machinery
 
-__all__ = ['write_if_different', 'import_file']
+__all__ = ["write_if_different", "import_file"]
 
 
-if sys.platform == 'win32':
+if sys.platform == "win32":
     import ctypes
 
     def _has_hidden_attribute(filepath):
         """
         Returns True if the given filepath has the hidden attribute on
         MS-Windows.  Based on a post here:
         http://stackoverflow.com/questions/284115/cross-platform-hidden-file-detection
@@ -23,15 +21,17 @@
         try:
             attrs = ctypes.windll.kernel32.GetFileAttributesW(filepath)
             assert attrs != -1
             result = bool(attrs & 2)
         except (AttributeError, AssertionError):
             result = False
         return result
+
 else:
+
     def _has_hidden_attribute(filepath):
         return False
 
 
 def is_path_hidden(filepath):
     """
     Determines if a given file or directory is hidden.
@@ -45,17 +45,17 @@
     -------
     hidden : bool
         Returns `True` if the file is hidden
     """
 
     name = os.path.basename(os.path.abspath(filepath))
     if isinstance(name, bytes):
-        is_dotted = name.startswith(b'.')
+        is_dotted = name.startswith(b".")
     else:
-        is_dotted = name.startswith('.')
+        is_dotted = name.startswith(".")
     return is_dotted or _has_hidden_attribute(filepath)
 
 
 def walk_skip_hidden(top, onerror=None, followlinks=False):
     """
     A wrapper for `os.walk` that skips hidden files and directories.
 
@@ -64,17 +64,15 @@
     using this function.
 
     See also
     --------
     os.walk : For a description of the parameters
     """
 
-    for root, dirs, files in os.walk(
-            top, topdown=True, onerror=onerror,
-            followlinks=followlinks):
+    for root, dirs, files in os.walk(top, topdown=True, onerror=onerror, followlinks=followlinks):
         # These lists must be updated in-place so os.walk will skip
         # hidden directories
         dirs[:] = [d for d in dirs if not is_path_hidden(d)]
         files[:] = [f for f in files if not is_path_hidden(f)]
         yield root, dirs, files
 
 
@@ -92,21 +90,21 @@
     data : bytes
         The data to be written to ``filename``.
     """
 
     assert isinstance(data, bytes)
 
     if os.path.exists(filename):
-        with open(filename, 'rb') as fd:
+        with open(filename, "rb") as fd:
             original_data = fd.read()
     else:
         original_data = None
 
     if original_data != data:
-        with open(filename, 'wb') as fd:
+        with open(filename, "wb") as fd:
             fd.write(data)
 
 
 def import_file(filename, name=None):
     """
     Imports a module from a single file without importing the package that
     the file is in.
@@ -119,20 +117,19 @@
     # Specifying a traditional dot-separated fully qualified name here
     # results in a number of "Parent module '...' not found while
     # handling absolute import" warnings.  Using the same name, the
     # namespaces of the modules get merged together.  So, this
     # generates an underscore-separated name which is more likely to
     # be unique, and it doesn't really matter because the name isn't
     # used directly here anyway.
-    mode = 'r'
 
     if name is None:
         basename = os.path.splitext(filename)[0]
-        name = '_'.join(os.path.abspath(basename).split(os.sep)[1:])
+        name = "_".join(os.path.abspath(basename).split(os.sep)[1:])
 
     if not os.path.exists(filename):
-        raise ImportError('Could not import file {0}'.format(filename))
+        raise ImportError(f"Could not import file {filename}")
 
     loader = import_machinery.SourceFileLoader(name, filename)
     mod = loader.load_module()
 
     return mod
```

### Comparing `extension-helpers-1.0.0/extension_helpers/conftest.py` & `extension-helpers-1.1.0/extension_helpers/conftest.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,55 +11,53 @@
     from coverage import CoverageData
     from coverage import __version__ as coverage_version
 except ImportError:
     HAS_COVERAGE = False
     CoverageData = None
 else:
     # Set to the major version number
-    HAS_COVERAGE = int(coverage_version.split('.')[0])
+    HAS_COVERAGE = int(coverage_version.split(".")[0])
 
 
 SUBPROCESS_COVERAGE = []
 
 
 def pytest_configure(config):
     if HAS_COVERAGE:
         SUBPROCESS_COVERAGE.clear()
 
 
 def pytest_unconfigure(config):
-
     if HAS_COVERAGE:
-
         # Add all files from extension_helpers to make sure we compute the total
         # coverage, not just the coverage of the files that have non-zero
         # coverage.
 
         lines = {}
-        for filename in glob.glob(os.path.join('extension_helpers', '**', '*.py'), recursive=True):
+        for filename in glob.glob(os.path.join("extension_helpers", "**", "*.py"), recursive=True):
             lines[os.path.abspath(filename)] = []
 
         for cdata in SUBPROCESS_COVERAGE:
             # For each CoverageData object, we go through all the files and
             # change the filename from one which might be a temporary path
             # to the local filename. We then only keep files that actually
             # exist.
             for filename in cdata.measured_files():
                 try:
-                    pos = filename.rindex('extension_helpers')
+                    pos = filename.rindex("extension_helpers")
                 except ValueError:
                     continue
                 short_filename = filename[pos:]
                 if os.path.exists(short_filename):
                     lines[os.path.abspath(short_filename)].extend(cdata.lines(filename))
 
         if HAS_COVERAGE >= 5:
             # Support coverage<5 and >=5; see
             # https://github.com/astropy/extension-helpers/issues/24
             # We create an empty coverage data object
-            combined_cdata = CoverageData(suffix='subprocess')
+            combined_cdata = CoverageData(suffix="subprocess")
             combined_cdata.add_lines(lines)
             combined_cdata.write()
         else:
             combined_cdata = CoverageData()
             combined_cdata.add_lines(lines)
-            combined_cdata.write_file('.coverage.subprocess')
+            combined_cdata.write_file(".coverage.subprocess")
```

### Comparing `extension-helpers-1.0.0/extension_helpers/src/compiler.c` & `extension-helpers-1.1.0/extension_helpers/src/compiler.c`

 * *Files identical despite different names*

### Comparing `extension-helpers-1.0.0/extension_helpers/tests/__init__.py` & `extension-helpers-1.1.0/extension_helpers/tests/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,69 +19,69 @@
     If ``raise_error=True`` raise an exception on non-zero exit codes.
     """
 
     if path is not None:
         # Transparently support py.path objects
         path = str(path)
 
-    p = sp.Popen([cmd] + list(args), stdout=sp.PIPE, stderr=sp.PIPE,
-                 cwd=path)
-    streams = tuple(s.decode('latin1').strip() for s in p.communicate())
+    p = sp.Popen([cmd] + list(args), stdout=sp.PIPE, stderr=sp.PIPE, cwd=path)
+    streams = tuple(s.decode("latin1").strip() for s in p.communicate())
     return_code = p.returncode
 
     if raise_error and return_code != 0:
         raise RuntimeError(
-            "The command `{0}` with args {1!r} exited with code {2}.\n"
-            "Stdout:\n\n{3}\n\nStderr:\n\n{4}".format(
-                cmd, list(args), return_code, streams[0], streams[1]))
+            "The command `{}` with args {!r} exited with code {}.\n"
+            "Stdout:\n\n{}\n\nStderr:\n\n{}".format(
+                cmd, list(args), return_code, streams[0], streams[1]
+            )
+        )
 
     return streams + (return_code,)
 
 
 def run_setup(setup_script, args):
-
     # This used to call setuptools.sandbox's run_setup, but due to issues with
     # this and Cython (which caused segmentation faults), we now use subprocess.
 
     setup_script = os.path.abspath(setup_script)
 
     path = os.path.dirname(setup_script)
     setup_script = os.path.basename(setup_script)
 
     if HAS_COVERAGE:
-
         # In this case, we run the command using the coverage command and we
         # then collect the coverage data into a SUBPROCESS_COVERAGE list which
         # is set up at the start of the testing process and is then combined
         # into a single .coverage file at the end of the testing process.
 
-        p = sp.Popen(['coverage', 'run', setup_script] + list(args), cwd=path,
-                     stdout=sp.PIPE, stderr=sp.PIPE)
+        p = sp.Popen(
+            ["coverage", "run", setup_script] + list(args), cwd=path, stdout=sp.PIPE, stderr=sp.PIPE
+        )
         stdout, stderr = p.communicate()
 
         cdata = CoverageData()
         if HAS_COVERAGE >= 5:
             # Support coverage<5 and >=5; see
             # https://github.com/astropy/extension-helpers/issues/24
             cdata.read()
         else:
-            cdata.read_file(os.path.join(path, '.coverage'))
+            cdata.read_file(os.path.join(path, ".coverage"))
 
         SUBPROCESS_COVERAGE.append(cdata)
 
     else:
-
         # Otherwise we just run the tests with Python
 
-        p = sp.Popen([sys.executable, setup_script] + list(args), cwd=path,
-                     stdout=sp.PIPE, stderr=sp.PIPE)
+        p = sp.Popen(
+            [sys.executable, setup_script] + list(args), cwd=path, stdout=sp.PIPE, stderr=sp.PIPE
+        )
         stdout, stderr = p.communicate()
 
-    sys.stdout.write(stdout.decode('utf-8'))
-    sys.stderr.write(stderr.decode('utf-8'))
+    sys.stdout.write(stdout.decode("utf-8"))
+    sys.stderr.write(stderr.decode("utf-8"))
 
     if p.returncode != 0:
         raise SystemExit(p.returncode)
 
 
 TEST_PACKAGE_SETUP_PY = """\
 #!/usr/bin/env python
@@ -93,35 +93,34 @@
 
 setup(name=NAME, version=VERSION,
       packages=['_extension_helpers_test_'],
       zip_safe=False)
 """
 
 
-def create_testpackage(tmpdir, version='0.1'):
-
-    source = tmpdir.mkdir('testpkg')
+def create_testpackage(tmpdir, version="0.1"):
+    source = tmpdir.mkdir("testpkg")
 
     with source.as_cwd():
-        source.mkdir('_extension_helpers_test_')
-        init = source.join('_extension_helpers_test_', '__init__.py')
-        init.write('__version__ = {0!r}'.format(version))
+        source.mkdir("_extension_helpers_test_")
+        init = source.join("_extension_helpers_test_", "__init__.py")
+        init.write(f"__version__ = {version!r}")
         setup_py = TEST_PACKAGE_SETUP_PY.format(version=version)
-        source.join('setup.py').write(setup_py)
+        source.join("setup.py").write(setup_py)
 
         # Make the new test package into a git repo
-        run_cmd('git', ['init'])
-        run_cmd('git', ['add', '--all'])
-        run_cmd('git', ['commit', '-m', 'test package'])
+        run_cmd("git", ["init"])
+        run_cmd("git", ["add", "--all"])
+        run_cmd("git", ["commit", "-m", "test package"])
 
     return source
 
 
 @pytest.fixture
-def testpackage(tmpdir, version='0.1'):
+def testpackage(tmpdir, version="0.1"):
     """
     This fixture creates a simplified package called _extension_helpers_test_
     used primarily for testing ah_boostrap, but without using the
     extension_helpers package directly and getting it confused with the
     extension_helpers package already under test.
     """
 
@@ -131,13 +130,13 @@
 def cleanup_import(package_name):
     """Remove all references to package_name from sys.modules"""
 
     for k in list(sys.modules):
         if not isinstance(k, str):
             # Some things will actually do this =_=
             continue
-        elif k.startswith('extension_helpers.tests'):
+        elif k.startswith("extension_helpers.tests"):
             # Don't delete imported test modules or else the tests will break,
             # badly
             continue
-        if k == package_name or k.startswith(package_name + '.'):
+        if k == package_name or k.startswith(package_name + "."):
             del sys.modules[k]
```

### Comparing `extension-helpers-1.0.0/extension_helpers/tests/test_openmp_helpers.py` & `extension-helpers-1.1.0/extension_helpers/tests/test_openmp_helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,45 @@
-
 import os
-import sys
 import types
-from copy import deepcopy
 from importlib import machinery
 
 import pytest
 from setuptools import Extension
 
 from .._openmp_helpers import add_openmp_flags_if_available, generate_openmp_enabled_py
 
 
 @pytest.fixture
 def openmp_expected(request):
     try:
         openmp_expected = request.config.getoption("--openmp-expected")
         if openmp_expected is not None:
-            return openmp_expected.lower() == 'true'
+            return openmp_expected.lower() == "true"
     except ValueError:
         return None
 
 
 def test_add_openmp_flags_if_available(openmp_expected):
-
-    using_openmp = add_openmp_flags_if_available(Extension('test', []))
+    using_openmp = add_openmp_flags_if_available(Extension("test", []))
 
     # Make sure that on Travis (Linux) and AppVeyor OpenMP does get used (for
     # MacOS X usually it will not work but this will depend on the compiler).
     # Having this is useful because we'll find out if OpenMP no longer works
     # for any reason on platforms on which it does work at the time of writing.
     if openmp_expected is not None:
         assert openmp_expected is using_openmp
 
 
 def test_generate_openmp_enabled_py(openmp_expected):
-
     # Test file generation
-    generate_openmp_enabled_py('')
-    assert os.path.isfile('openmp_enabled.py')
+    generate_openmp_enabled_py("")
+    assert os.path.isfile("openmp_enabled.py")
 
     # Load openmp_enabled file as a module to check the result
-    loader = machinery.SourceFileLoader('openmp_enabled', 'openmp_enabled.py')
+    loader = machinery.SourceFileLoader("openmp_enabled", "openmp_enabled.py")
     mod = types.ModuleType(loader.name)
     loader.exec_module(mod)
 
     is_openmp_enabled = mod.is_openmp_enabled()
 
     # Test is_openmp_enabled()
     assert isinstance(is_openmp_enabled, bool)
```

### Comparing `extension-helpers-1.0.0/extension_helpers/tests/test_setup_helpers.py` & `extension-helpers-1.1.0/extension_helpers/tests/test_setup_helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,274 +6,339 @@
 from textwrap import dedent
 
 import pytest
 
 from .._setup_helpers import get_compiler, get_extensions
 from . import cleanup_import, run_setup
 
-extension_helpers_PATH = os.path.abspath(os.path.join(os.path.dirname(__file__), '..', '..'))  # noqa
+extension_helpers_PATH = os.path.abspath(
+    os.path.join(os.path.dirname(__file__), "..", "..")
+)  # noqa
 
 
 def teardown_module(module):
     # Remove file generated by test_generate_openmp_enabled_py but
     # somehow needed in test_cython_autoextensions
-    tmpfile = 'openmp_enabled.py'
+    tmpfile = "openmp_enabled.py"
     if os.path.exists(tmpfile):
         os.remove(tmpfile)
 
 
-POSSIBLE_COMPILERS = ['unix', 'msvc', 'bcpp', 'cygwin', 'mingw32']
+POSSIBLE_COMPILERS = ["unix", "msvc", "bcpp", "cygwin", "mingw32"]
 
 
 def test_get_compiler():
     assert get_compiler() in POSSIBLE_COMPILERS
 
 
-def _extension_test_package(tmpdir, request, extension_type='c',
-                            include_numpy=False):
+def _extension_test_package(tmpdir, request, extension_type="c", include_numpy=False):
     """Creates a simple test package with an extension module."""
 
-    test_pkg = tmpdir.mkdir('test_pkg')
-    test_pkg.mkdir('helpers_test_package').ensure('__init__.py')
+    test_pkg = tmpdir.mkdir("test_pkg")
+    test_pkg.mkdir("helpers_test_package").ensure("__init__.py")
 
     # TODO: It might be later worth making this particular test package into a
     # reusable fixture for other build_ext tests
 
-    if extension_type in ('c', 'both'):
+    if extension_type in ("c", "both"):
         # A minimal C extension for testing
-        test_pkg.join('helpers_test_package', 'unit01.c').write(dedent("""\
+        test_pkg.join("helpers_test_package", "unit01.c").write(
+            dedent(
+                """\
             #include <Python.h>
 
             static struct PyModuleDef moduledef = {
                 PyModuleDef_HEAD_INIT,
                 "unit01",
                 NULL,
                 -1,
                 NULL
             };
             PyMODINIT_FUNC
             PyInit_unit01(void) {
                 return PyModule_Create(&moduledef);
             }
-        """))
+        """
+            )
+        )
 
-    if extension_type in ('pyx', 'both'):
+    if extension_type in ("pyx", "both"):
         # A minimal Cython extension for testing
-        test_pkg.join('helpers_test_package', 'unit02.pyx').write(dedent("""\
+        test_pkg.join("helpers_test_package", "unit02.pyx").write(
+            dedent(
+                """\
             print("Hello cruel angel.")
-        """))
+        """
+            )
+        )
 
-    if extension_type == 'c':
-        extensions = ['unit01.c']
-    elif extension_type == 'pyx':
-        extensions = ['unit02.pyx']
-    elif extension_type == 'both':
-        extensions = ['unit01.c', 'unit02.pyx']
+    if extension_type == "c":
+        extensions = ["unit01.c"]
+    elif extension_type == "pyx":
+        extensions = ["unit02.pyx"]
+    elif extension_type == "both":
+        extensions = ["unit01.c", "unit02.pyx"]
 
-    include_dirs = ['numpy'] if include_numpy else []
+    include_dirs = ["numpy"] if include_numpy else []
 
     extensions_list = [
-        "Extension('helpers_test_package.{0}', "
-        "[join('helpers_test_package', '{1}')], "
-        "include_dirs={2})".format(
-            os.path.splitext(extension)[0], extension, include_dirs)
-        for extension in extensions]
-
-    test_pkg.join('helpers_test_package', 'setup_package.py').write(dedent("""\
+        "Extension('helpers_test_package.{}', "
+        "[join('helpers_test_package', '{}')], "
+        "include_dirs={})".format(os.path.splitext(extension)[0], extension, include_dirs)
+        for extension in extensions
+    ]
+
+    test_pkg.join("helpers_test_package", "setup_package.py").write(
+        dedent(
+            """\
         from setuptools import Extension
         from os.path import join
         def get_extensions():
-            return [{0}]
-    """.format(', '.join(extensions_list))))
+            return [{}]
+    """.format(
+                ", ".join(extensions_list)
+            )
+        )
+    )
 
-    test_pkg.join('setup.py').write(dedent("""\
+    test_pkg.join("setup.py").write(
+        dedent(
+            f"""\
         import sys
         from os.path import join
         from setuptools import setup, find_packages
-        sys.path.insert(0, r'{extension_helpers_path}')
+        sys.path.insert(0, r'{extension_helpers_PATH}')
         from extension_helpers import get_extensions
 
         setup(
             name='helpers_test_package',
             version='0.1',
             packages=find_packages(),
             ext_modules=get_extensions()
         )
-    """.format(extension_helpers_path=extension_helpers_PATH)))
+    """
+        )
+    )
 
-    if '' in sys.path:
-        sys.path.remove('')
+    if "" in sys.path:
+        sys.path.remove("")
 
-    sys.path.insert(0, '')
+    sys.path.insert(0, "")
 
     def finalize():
-        cleanup_import('helpers_test_package')
+        cleanup_import("helpers_test_package")
 
     request.addfinalizer(finalize)
 
     return test_pkg
 
 
 @pytest.fixture
 def extension_test_package(tmpdir, request):
-    return _extension_test_package(tmpdir, request, extension_type='both')
+    return _extension_test_package(tmpdir, request, extension_type="both")
 
 
 @pytest.fixture
 def c_extension_test_package(tmpdir, request):
     # Check whether numpy is installed in the test environment
-    has_numpy = bool(importlib.util.find_spec('numpy'))
-    return _extension_test_package(tmpdir, request, extension_type='c',
-                                   include_numpy=has_numpy)
+    has_numpy = bool(importlib.util.find_spec("numpy"))
+    return _extension_test_package(tmpdir, request, extension_type="c", include_numpy=has_numpy)
 
 
 @pytest.fixture
 def pyx_extension_test_package(tmpdir, request):
-    return _extension_test_package(tmpdir, request, extension_type='pyx')
+    return _extension_test_package(tmpdir, request, extension_type="pyx")
 
 
 def test_cython_autoextensions(tmpdir):
     """
     Regression test for https://github.com/astropy/astropy-helpers/pull/19
 
     Ensures that Cython extensions in sub-packages are discovered and built
     only once.
     """
 
     # Make a simple test package
-    test_pkg = tmpdir.mkdir('test_pkg')
-    test_pkg.mkdir('yoda').mkdir('luke')
-    test_pkg.ensure('yoda', '__init__.py')
-    test_pkg.ensure('yoda', 'luke', '__init__.py')
-    test_pkg.join('yoda', 'luke', 'dagobah.pyx').write(
-        """def testfunc(): pass""")
+    test_pkg = tmpdir.mkdir("test_pkg")
+    test_pkg.mkdir("yoda").mkdir("luke")
+    test_pkg.ensure("yoda", "__init__.py")
+    test_pkg.ensure("yoda", "luke", "__init__.py")
+    test_pkg.join("yoda", "luke", "dagobah.pyx").write("""def testfunc(): pass""")
 
     # Required, currently, for get_extensions to work
     ext_modules = get_extensions(str(test_pkg))
 
     assert len(ext_modules) == 2
-    assert ext_modules[0].name == 'yoda.luke.dagobah'
+    assert ext_modules[0].name == "yoda.luke.dagobah"
 
 
 def test_compiler_module(capsys, c_extension_test_package):
     """
     Test ensuring that the compiler module is built and installed for packages
     that have extension modules.
     """
 
     test_pkg = c_extension_test_package
-    install_temp = test_pkg.mkdir('install_temp')
+    install_temp = test_pkg.mkdir("install_temp")
 
     with test_pkg.as_cwd():
         # This is one of the simplest ways to install just a package into a
         # test directory
-        run_setup('setup.py',
-                  ['install',
-                   '--single-version-externally-managed',
-                   '--install-lib={0}'.format(install_temp),
-                   '--record={0}'.format(install_temp.join('record.txt'))])
+        run_setup(
+            "setup.py",
+            [
+                "install",
+                "--single-version-externally-managed",
+                f"--install-lib={install_temp}",
+                "--record={}".format(install_temp.join("record.txt")),
+            ],
+        )
 
     with install_temp.as_cwd():
         import helpers_test_package
 
         # Make sure we imported the helpers_test_package package from the correct place
         dirname = os.path.abspath(os.path.dirname(helpers_test_package.__file__))
-        assert dirname == str(install_temp.join('helpers_test_package'))
+        assert dirname == str(install_temp.join("helpers_test_package"))
 
         import helpers_test_package.compiler_version
-        assert helpers_test_package.compiler_version != 'unknown'
 
+        assert helpers_test_package.compiler_version != "unknown"
 
-@pytest.mark.parametrize('use_extension_helpers', [None, False, True])
-def test_no_setup_py(tmpdir, use_extension_helpers):
+
+@pytest.mark.parametrize("use_extension_helpers", [None, False, True])
+@pytest.mark.parametrize("pyproject_use_helpers", [None, False, True])
+def test_no_setup_py(tmpdir, use_extension_helpers, pyproject_use_helpers):
     """
     Test that makes sure that extension-helpers can be enabled without a
     setup.py file.
     """
 
-    package_name = 'helpers_test_package_' + str(uuid.uuid4()).replace('-', '_')
+    package_name = "helpers_test_package_" + str(uuid.uuid4()).replace("-", "_")
 
-    test_pkg = tmpdir.mkdir('test_pkg')
-    test_pkg.mkdir(package_name).ensure('__init__.py')
+    test_pkg = tmpdir.mkdir("test_pkg")
+    test_pkg.mkdir(package_name).ensure("__init__.py")
 
-    simple_c = test_pkg.join(package_name, 'simple.c')
+    simple_c = test_pkg.join(package_name, "simple.c")
 
-    simple_c.write(dedent("""\
+    simple_c.write(
+        dedent(
+            """\
         #include <Python.h>
 
         static struct PyModuleDef moduledef = {
             PyModuleDef_HEAD_INIT,
             "simple",
             NULL,
             -1,
             NULL
         };
         PyMODINIT_FUNC
         PyInit_simple(void) {
             return PyModule_Create(&moduledef);
         }
-    """))
+    """
+        )
+    )
 
-    test_pkg.join(package_name, 'setup_package.py').write(dedent(f"""\
+    test_pkg.join(package_name, "setup_package.py").write(
+        dedent(
+            f"""\
         from setuptools import Extension
         from os.path import join
         def get_extensions():
             return [Extension('{package_name}.simple', [join('{package_name}', 'simple.c')])]
-        """))
+        """
+        )
+    )
 
     if use_extension_helpers is None:
-        test_pkg.join('setup.cfg').write(dedent(f"""\
+        test_pkg.join("setup.cfg").write(
+            dedent(
+                f"""\
             [metadata]
             name = {package_name}
             version = 0.1
 
             [options]
             packages = find:
-        """))
+        """
+            )
+        )
     else:
-        test_pkg.join('setup.cfg').write(dedent(f"""\
+        test_pkg.join("setup.cfg").write(
+            dedent(
+                f"""\
             [metadata]
             name = {package_name}
             version = 0.1
 
             [options]
             packages = find:
 
             [extension-helpers]
             use_extension_helpers = {str(use_extension_helpers).lower()}
-        """))
+        """
+            )
+        )
 
-    test_pkg.join('pyproject.toml').write(dedent("""\
-        [build-system]
-        requires = ["setuptools>=43.0.0",
-                    "wheel"]
-        build-backend = 'setuptools.build_meta'
-    """))
+    if pyproject_use_helpers is None:
+        test_pkg.join("pyproject.toml").write(
+            dedent(
+                """\
+            [build-system]
+            requires = ["setuptools>=43.0.0",
+                        "wheel"]
+            build-backend = 'setuptools.build_meta'
+        """
+            )
+        )
+    else:
+        test_pkg.join("pyproject.toml").write(
+            dedent(
+                f"""\
+            [build-system]
+            requires = ["setuptools>=43.0.0",
+                        "wheel"]
+            build-backend = 'setuptools.build_meta'
+
+            [tool.extension-helpers]
+            use_extension_helpers = {str(pyproject_use_helpers).lower()}
+        """
+            )
+        )
 
-    install_temp = test_pkg.mkdir('install_temp')
+    install_temp = test_pkg.mkdir("install_temp")
 
     with test_pkg.as_cwd():
         # NOTE: we disable build isolation as we need to pick up the current
         # developer version of extension-helpers
-        subprocess.call([sys.executable, '-m', 'pip', 'install', '.',
-                         '--no-build-isolation',
-                         f'--target={install_temp}'])
+        subprocess.call(
+            [
+                sys.executable,
+                "-m",
+                "pip",
+                "install",
+                ".",
+                "--no-build-isolation",
+                f"--target={install_temp}",
+            ]
+        )
 
-    if '' in sys.path:
-        sys.path.remove('')
+    if "" in sys.path:
+        sys.path.remove("")
 
-    sys.path.insert(0, '')
+    sys.path.insert(0, "")
 
     with install_temp.as_cwd():
-
         importlib.import_module(package_name)
 
-        if use_extension_helpers:
-            compiler_version_mod = importlib.import_module(package_name + '.compiler_version')
-            assert compiler_version_mod.compiler != 'unknown'
+        if use_extension_helpers or (use_extension_helpers is None and pyproject_use_helpers):
+            compiler_version_mod = importlib.import_module(package_name + ".compiler_version")
+            assert compiler_version_mod.compiler != "unknown"
         else:
             try:
-                importlib.import_module(package_name + '.compiler_version')
+                importlib.import_module(package_name + ".compiler_version")
             except ImportError:
                 pass
             else:
-                raise AssertionError(package_name + '.compiler_version should not exist')
+                raise AssertionError(package_name + ".compiler_version should not exist")
```

### Comparing `extension-helpers-1.0.0/extension_helpers/tests/test_utils.py` & `extension-helpers-1.1.0/extension_helpers/tests/test_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import os
 import time
 
 from .._utils import import_file, write_if_different
 
 
 def test_import_file(tmpdir):
-    filename = str(tmpdir / 'spam.py')
-    with open(filename, 'w') as f:
-        f.write('magic = 12345')
+    filename = str(tmpdir / "spam.py")
+    with open(filename, "w") as f:
+        f.write("magic = 12345")
     module = import_file(filename)
     assert module.magic == 12345
 
 
 def test_write_if_different(tmpdir):
-    filename = str(tmpdir / 'test.txt')
-    write_if_different(filename, b'abc')
+    filename = str(tmpdir / "test.txt")
+    write_if_different(filename, b"abc")
     time1 = os.path.getmtime(filename)
     time.sleep(0.01)
-    write_if_different(filename, b'abc')
+    write_if_different(filename, b"abc")
     time2 = os.path.getmtime(filename)
     assert time2 == time1
     time.sleep(0.01)
-    write_if_different(filename, b'abcd')
+    write_if_different(filename, b"abcd")
     time3 = os.path.getmtime(filename)
     assert time3 > time1
```

### Comparing `extension-helpers-1.0.0/extension_helpers.egg-info/PKG-INFO` & `extension-helpers-1.1.0/extension_helpers.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: extension-helpers
-Version: 1.0.0
+Version: 1.1.0
 Summary: Utilities for building and installing packages with compiled extensions
 Home-page: https://github.com/astropy/extension-helpers
 Author: The Astropy Developers
 Author-email: astropy.team@gmail.com
 License: BSD 3-Clause License
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: Setuptools Plugin
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Archiving :: Packaging
 Provides: extension_helpers
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE.rst
 
 extension-helpers
 =================
 
@@ -38,9 +37,7 @@
 
 The **extension-helpers** package includes convenience helpers to assist with
 building Python packages with compiled C/Cython extensions. It is developed by
 the Astropy project but is intended to be general and usable by any Python
 package.
 
 For more information, see the documentation at http://extension-helpers.readthedocs.io
-
-
```

### Comparing `extension-helpers-1.0.0/extension_helpers.egg-info/SOURCES.txt` & `extension-helpers-1.1.0/extension_helpers.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 .gitignore
-.readthedocs.yml
-CHANGES.rst
+.pre-commit-config.yaml
+.readthedocs.yaml
+CHANGES.md
 CONTRIBUTING.md
 LICENSE.rst
 MANIFEST.in
 README.rst
 conftest.py
 pyproject.toml
 setup.cfg
 tox.ini
+.github/release.yml
 .github/workflows/main.yml
+.github/workflows/update-changelog.yml
 docs/Makefile
 docs/api.rst
 docs/conf.py
 docs/index.rst
 docs/make.bat
 docs/openmp.rst
 docs/using.rst
```

### Comparing `extension-helpers-1.0.0/licenses/LICENSE_ASTROSCRAPPY.rst` & `extension-helpers-1.1.0/licenses/LICENSE_ASTROSCRAPPY.rst`

 * *Files identical despite different names*

### Comparing `extension-helpers-1.0.0/setup.cfg` & `extension-helpers-1.1.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = extension-helpers
 provides = extension_helpers
 author = The Astropy Developers
 author_email = astropy.team@gmail.com
 license = BSD 3-Clause License
-license_file = LICENSE.rst
+license_files = LICENSE.rst
 url = https://github.com/astropy/extension-helpers
 description = Utilities for building and installing packages with compiled extensions
 long_description = file: README.rst
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	Framework :: Setuptools Plugin
@@ -18,18 +18,19 @@
 	Programming Language :: Python :: 3
 	Topic :: Software Development :: Build Tools
 	Topic :: Software Development :: Libraries :: Python Modules
 	Topic :: System :: Archiving :: Packaging
 
 [options]
 zip_safe = False
-python_requires = >=3.6
+python_requires = >=3.7
 packages = find:
 install_requires = 
 	setuptools>=40.2
+	tomli>=1.0.0
 
 [options.package_data]
 extension_helpers = src/compiler.c
 
 [options.entry_points]
 setuptools.finalize_distribution_options = 
 	extension_helpers_get_extensions = extension_helpers:_finalize_distribution_hook
@@ -41,30 +42,18 @@
 	pytest-cov
 	coverage>=4
 docs = 
 	sphinx
 	sphinx-automodapi
 
 [tool:pytest]
-norecursedirs = 
-	.tox
-	extension_helpers/tests/package_template
-python_functions = test_
-
-[isort]
-line_length = 100
-sections = FUTURE,STDLIB,THIRDPARTY,NUMPY,FIRSTPARTY,LOCALFOLDER
-default_section = THIRDPARTY
-known_first_party = extension_helpers
-known_numpy = numpy
-multi_line_output = 0
-balanced_wrapping = True
-include_trailing_comma = false
-length_sort = False
-length_sort_sections = stdlib
+testpaths = "extension_helpers" "docs"
+
+[flake8]
+max-line-length = 100
 
 [coverage:run]
 omit = 
 	extension_helpers/*/setup_package.py
 	extension_helpers/tests/*
 	extension_helpers/conftest.py
 	*/extension_helpers/*/setup_package.py
```

### Comparing `extension-helpers-1.0.0/tox.ini` & `extension-helpers-1.1.0/tox.ini`

 * *Files 14% similar despite different names*

```diff
@@ -44,21 +44,20 @@
     test: pytest --pyargs extension_helpers {toxinidir}/docs --cov extension_helpers --cov-config={toxinidir}/setup.cfg {posargs}
     build_docs: sphinx-build -W -b html . _build/html
 
 [testenv:py39-downstream]
 changedir = test: .tmp/downstream
 commands =
     pip install setuptools setuptools_scm wheel cython numpy
-    pip install --no-build-isolation "git+https://github.com/astropy/astropy#egg=astropy[test]"
-    pytest --pyargs astropy
-    pip install --no-build-isolation "git+https://github.com/sunpy/sunpy#egg=sunpy[all,tests]"
-    pytest --pyargs sunpy
+    pip install --no-build-isolation "astropy[test]@git+https://github.com/astropy/astropy.git@main"
+    pytest --pyargs astropy -m "not hypothesis"
+    pip install --no-build-isolation "sunpy[all,tests]@git+https://github.com/sunpy/sunpy.git"
+    pip freeze
+    pytest --pyargs sunpy -k "not test_saveframe and not test_hpc_observer_version and not test_hcc_observer_version"
 
 [testenv:style]
 skip_install = true
-description = invoke pycodestyle and isort on package code
 deps =
-    pycodestyle
-    isort
+    pre-commit
 commands =
-    pycodestyle extension_helpers --max-line-length=100
-    isort -c extension_helpers
+    pre-commit install-hooks
+    pre-commit run --color always --all-files --show-diff-on-failure
```

