# Comparing `tmp/shtab-1.6.2.tar.gz` & `tmp/shtab-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shtab-1.6.2.tar", last modified: Wed Jun 14 16:51:48 2023, max compression
+gzip compressed data, was "shtab-1.6.3.tar", last modified: Mon Jul 24 15:17:58 2023, max compression
```

## Comparing `shtab-1.6.2.tar` & `shtab-1.6.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:51:48.395580 shtab-1.6.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:51:48.391580 shtab-1.6.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:51:48.391580 shtab-1.6.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-14 16:51:26.000000 shtab-1.6.2/.github/workflows/comment-bot.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-06-14 16:51:26.000000 shtab-1.6.2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-14 16:51:26.000000 shtab-1.6.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-14 16:51:26.000000 shtab-1.6.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-06-14 16:51:26.000000 shtab-1.6.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-14 16:51:26.000000 shtab-1.6.2/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-06-14 16:51:48.395580 shtab-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-06-14 16:51:26.000000 shtab-1.6.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:51:48.391580 shtab-1.6.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-06-14 16:51:26.000000 shtab-1.6.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-06-14 16:51:26.000000 shtab-1.6.2/docs/pydoc-markdown.yml
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-14 16:51:26.000000 shtab-1.6.2/docs/pydoc_markdown_shtab.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-14 16:51:26.000000 shtab-1.6.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-06-14 16:51:26.000000 shtab-1.6.2/docs/use.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:51:48.391580 shtab-1.6.2/examples/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2174 2023-06-14 16:51:26.000000 shtab-1.6.2/examples/customcomplete.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      536 2023-06-14 16:51:26.000000 shtab-1.6.2/examples/docopt-greeter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      746 2023-06-14 16:51:26.000000 shtab-1.6.2/examples/pathcomplete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:51:48.391580 shtab-1.6.2/meta/
--rw-r--r--   0 runner    (1001) docker     (123)    16145 2023-06-14 16:51:26.000000 shtab-1.6.2/meta/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-06-14 16:51:26.000000 shtab-1.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 16:51:48.395580 shtab-1.6.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:51:48.391580 shtab-1.6.2/shtab/
--rw-r--r--   0 runner    (1001) docker     (123)    30014 2023-06-14 16:51:26.000000 shtab-1.6.2/shtab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-14 16:51:26.000000 shtab-1.6.2/shtab/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-14 16:51:48.000000 shtab-1.6.2/shtab/_dist_ver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-06-14 16:51:26.000000 shtab-1.6.2/shtab/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-14 16:51:26.000000 shtab-1.6.2/shtab/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:51:48.395580 shtab-1.6.2/shtab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-06-14 16:51:48.000000 shtab-1.6.2/shtab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-14 16:51:48.000000 shtab-1.6.2/shtab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 16:51:48.000000 shtab-1.6.2/shtab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-14 16:51:48.000000 shtab-1.6.2/shtab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-14 16:51:48.000000 shtab-1.6.2/shtab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 16:51:48.000000 shtab-1.6.2/shtab.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:51:48.395580 shtab-1.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:51:26.000000 shtab-1.6.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-06-14 16:51:26.000000 shtab-1.6.2/tests/test_shtab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:17:58.011869 shtab-1.6.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:17:58.003869 shtab-1.6.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:17:58.003869 shtab-1.6.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-24 15:17:37.000000 shtab-1.6.3/.github/workflows/comment-bot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-07-24 15:17:37.000000 shtab-1.6.3/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-24 15:17:37.000000 shtab-1.6.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-24 15:17:37.000000 shtab-1.6.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-07-24 15:17:37.000000 shtab-1.6.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-24 15:17:37.000000 shtab-1.6.3/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-07-24 15:17:58.011869 shtab-1.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-07-24 15:17:37.000000 shtab-1.6.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:17:58.007869 shtab-1.6.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-07-24 15:17:37.000000 shtab-1.6.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-24 15:17:37.000000 shtab-1.6.3/docs/pydoc-markdown.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-24 15:17:37.000000 shtab-1.6.3/docs/pydoc_markdown_shtab.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-24 15:17:37.000000 shtab-1.6.3/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-07-24 15:17:37.000000 shtab-1.6.3/docs/use.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:17:58.007869 shtab-1.6.3/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2174 2023-07-24 15:17:37.000000 shtab-1.6.3/examples/customcomplete.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      536 2023-07-24 15:17:37.000000 shtab-1.6.3/examples/docopt-greeter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      746 2023-07-24 15:17:37.000000 shtab-1.6.3/examples/pathcomplete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:17:58.007869 shtab-1.6.3/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)    16145 2023-07-24 15:17:37.000000 shtab-1.6.3/meta/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-07-24 15:17:37.000000 shtab-1.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 15:17:58.011869 shtab-1.6.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:17:58.007869 shtab-1.6.3/shtab/
+-rw-r--r--   0 runner    (1001) docker     (123)    30588 2023-07-24 15:17:37.000000 shtab-1.6.3/shtab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-24 15:17:37.000000 shtab-1.6.3/shtab/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 15:17:57.000000 shtab-1.6.3/shtab/_dist_ver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-24 15:17:37.000000 shtab-1.6.3/shtab/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-24 15:17:37.000000 shtab-1.6.3/shtab/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:17:58.011869 shtab-1.6.3/shtab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-07-24 15:17:57.000000 shtab-1.6.3/shtab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-24 15:17:57.000000 shtab-1.6.3/shtab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 15:17:57.000000 shtab-1.6.3/shtab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-24 15:17:57.000000 shtab-1.6.3/shtab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-24 15:17:57.000000 shtab-1.6.3/shtab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 15:17:57.000000 shtab-1.6.3/shtab.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:17:58.011869 shtab-1.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 15:17:37.000000 shtab-1.6.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-07-24 15:17:37.000000 shtab-1.6.3/tests/test_shtab.py
```

### Comparing `shtab-1.6.2/.github/workflows/comment-bot.yml` & `shtab-1.6.3/.github/workflows/comment-bot.yml`

 * *Files identical despite different names*

### Comparing `shtab-1.6.2/.github/workflows/test.yml` & `shtab-1.6.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `shtab-1.6.2/.pre-commit-config.yaml` & `shtab-1.6.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `shtab-1.6.2/CONTRIBUTING.md` & `shtab-1.6.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `shtab-1.6.2/LICENCE` & `shtab-1.6.3/LICENCE`

 * *Files identical despite different names*

### Comparing `shtab-1.6.2/PKG-INFO` & `shtab-1.6.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shtab
-Version: 1.6.2
+Version: 1.6.3
 Summary: Automagic shell tab completion for Python CLI applications
 Author-email: Casper da Costa-Luis <casper.dcl@physics.org>
 Maintainer-email: Iterative <support@iterative.ai>
 License: Apache-2.0
 Project-URL: documentation, https://docs.iterative.ai/shtab
 Project-URL: repository, https://github.com/iterative/shtab
 Project-URL: changelog, https://github.com/iterative/shtab/releases
@@ -63,15 +63,15 @@
 License-File: LICENCE
 
 |Logo|
 
 shtab
 =====
 
-|Tests| |Coverage| |Conda| |PyPI|
+|PyPI-Downloads| |Tests| |Coverage| |PyPI| |Conda|
 
 - What: Automatically generate shell tab completion scripts for Python CLI apps
 - Why: Speed & correctness. Alternatives like
   `argcomplete <https://pypi.org/project/argcomplete>`_ and
   `pyzshcomplete <https://pypi.org/project/pyzshcomplete>`_ are slow and have
   side-effects
 - How: ``shtab`` processes an ``argparse.ArgumentParser`` object to generate a
@@ -120,16 +120,16 @@
 
   - may not require any code modifications whatsoever
   - end-users execute ``shtab your_cli_app.your_parser_object``
 
 - `Library Usage <https://docs.iterative.ai/shtab/use/#library-usage>`_: as a library integrated into your CLI application
 
   - adds a couple of lines to your application
-  - argument mode: end-users execute ``your_cli_app --print-completion {bash,zsh}``
-  - subparser mode: end-users execute ``your_cli_app completion {bash,zsh}``
+  - argument mode: end-users execute ``your_cli_app --print-completion {bash,zsh,tcsh}``
+  - subparser mode: end-users execute ``your_cli_app completion {bash,zsh,tcsh}``
 
 Examples
 --------
 
 See `the docs for usage examples <https://docs.iterative.ai/shtab/use/#main.py>`_.
 
 FAQs
@@ -168,22 +168,25 @@
 See
 `CONTRIBUTING.md <https://github.com/iterative/shtab/tree/main/CONTRIBUTING.md>`_
 for more guidance.
 
 |Hits|
 
 .. |Logo| image:: https://github.com/iterative/shtab/raw/main/meta/logo.png
-.. |Tests| image:: https://github.com/iterative/shtab/workflows/Test/badge.svg
+.. |Tests| image:: https://img.shields.io/github/actions/workflow/status/iterative/shtab/test.yml?logo=github&label=tests
    :target: https://github.com/iterative/shtab/actions
    :alt: Tests
 .. |Coverage| image:: https://codecov.io/gh/iterative/shtab/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/iterative/shtab
    :alt: Coverage
 .. |Conda| image:: https://img.shields.io/conda/v/conda-forge/shtab.svg?label=conda&logo=conda-forge
    :target: https://anaconda.org/conda-forge/shtab
    :alt: conda-forge
 .. |PyPI| image:: https://img.shields.io/pypi/v/shtab.svg?label=pip&logo=PyPI&logoColor=white
    :target: https://pypi.org/project/shtab
    :alt: PyPI
+.. |PyPI-Downloads| image:: https://img.shields.io/pypi/dm/shtab.svg?label=pypi%20downloads&logo=PyPI&logoColor=white
+   :target: https://pepy.tech/project/shtab
+   :alt: Downloads
 .. |Hits| image:: https://caspersci.uk.to/cgi-bin/hits.cgi?q=shtab&style=social&r=https://github.com/iterative/shtab&a=hidden
    :target: https://caspersci.uk.to/cgi-bin/hits.cgi?q=shtab&a=plot&r=https://github.com/iterative/shtab&style=social
    :alt: Hits
```

### Comparing `shtab-1.6.2/README.rst` & `shtab-1.6.3/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 |Logo|
 
 shtab
 =====
 
-|Tests| |Coverage| |Conda| |PyPI|
+|PyPI-Downloads| |Tests| |Coverage| |PyPI| |Conda|
 
 - What: Automatically generate shell tab completion scripts for Python CLI apps
 - Why: Speed & correctness. Alternatives like
   `argcomplete <https://pypi.org/project/argcomplete>`_ and
   `pyzshcomplete <https://pypi.org/project/pyzshcomplete>`_ are slow and have
   side-effects
 - How: ``shtab`` processes an ``argparse.ArgumentParser`` object to generate a
@@ -56,16 +56,16 @@
 
   - may not require any code modifications whatsoever
   - end-users execute ``shtab your_cli_app.your_parser_object``
 
 - `Library Usage <https://docs.iterative.ai/shtab/use/#library-usage>`_: as a library integrated into your CLI application
 
   - adds a couple of lines to your application
-  - argument mode: end-users execute ``your_cli_app --print-completion {bash,zsh}``
-  - subparser mode: end-users execute ``your_cli_app completion {bash,zsh}``
+  - argument mode: end-users execute ``your_cli_app --print-completion {bash,zsh,tcsh}``
+  - subparser mode: end-users execute ``your_cli_app completion {bash,zsh,tcsh}``
 
 Examples
 --------
 
 See `the docs for usage examples <https://docs.iterative.ai/shtab/use/#main.py>`_.
 
 FAQs
@@ -104,22 +104,25 @@
 See
 `CONTRIBUTING.md <https://github.com/iterative/shtab/tree/main/CONTRIBUTING.md>`_
 for more guidance.
 
 |Hits|
 
 .. |Logo| image:: https://github.com/iterative/shtab/raw/main/meta/logo.png
-.. |Tests| image:: https://github.com/iterative/shtab/workflows/Test/badge.svg
+.. |Tests| image:: https://img.shields.io/github/actions/workflow/status/iterative/shtab/test.yml?logo=github&label=tests
    :target: https://github.com/iterative/shtab/actions
    :alt: Tests
 .. |Coverage| image:: https://codecov.io/gh/iterative/shtab/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/iterative/shtab
    :alt: Coverage
 .. |Conda| image:: https://img.shields.io/conda/v/conda-forge/shtab.svg?label=conda&logo=conda-forge
    :target: https://anaconda.org/conda-forge/shtab
    :alt: conda-forge
 .. |PyPI| image:: https://img.shields.io/pypi/v/shtab.svg?label=pip&logo=PyPI&logoColor=white
    :target: https://pypi.org/project/shtab
    :alt: PyPI
+.. |PyPI-Downloads| image:: https://img.shields.io/pypi/dm/shtab.svg?label=pypi%20downloads&logo=PyPI&logoColor=white
+   :target: https://pepy.tech/project/shtab
+   :alt: Downloads
 .. |Hits| image:: https://caspersci.uk.to/cgi-bin/hits.cgi?q=shtab&style=social&r=https://github.com/iterative/shtab&a=hidden
    :target: https://caspersci.uk.to/cgi-bin/hits.cgi?q=shtab&a=plot&r=https://github.com/iterative/shtab&style=social
    :alt: Hits
```

### Comparing `shtab-1.6.2/docs/index.md` & `shtab-1.6.3/docs/index.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 ![shtab](https://static.iterative.ai/img/shtab/banner.png)
 
-[![Tests](https://github.com/iterative/shtab/workflows/Test/badge.svg)](https://github.com/iterative/shtab/actions)
+[![Downloads](https://img.shields.io/pypi/dm/shtab.svg?label=pypi%20downloads&logo=PyPI&logoColor=white)](https://pepy.tech/project/shtab)
+[![Tests](https://img.shields.io/github/actions/workflow/status/iterative/shtab/test.yml?logo=github&label=tests)](https://github.com/iterative/shtab/actions)
 [![Coverage](https://codecov.io/gh/iterative/shtab/branch/main/graph/badge.svg)](https://codecov.io/gh/iterative/shtab)
-[![conda-forge](https://img.shields.io/conda/v/conda-forge/shtab.svg?label=conda&logo=conda-forge)](https://anaconda.org/conda-forge/shtab)
 [![PyPI](https://img.shields.io/pypi/v/shtab.svg?label=pip&logo=PyPI&logoColor=white)](https://pypi.org/project/shtab)
+[![conda-forge](https://img.shields.io/conda/v/conda-forge/shtab.svg?label=conda&logo=conda-forge)](https://anaconda.org/conda-forge/shtab)
 
 - What: Automatically generate shell tab completion scripts for Python CLI apps
 - Why: Speed & correctness. Alternatives like
   [argcomplete](https://pypi.org/project/argcomplete) and
   [pyzshcomplete](https://pypi.org/project/pyzshcomplete) are slow and have side-effects
 - How: `shtab` processes an `argparse.ArgumentParser` object to generate a tab completion script for your shell
```

### Comparing `shtab-1.6.2/docs/pydoc-markdown.yml` & `shtab-1.6.3/docs/pydoc-markdown.yml`

 * *Files identical despite different names*

### Comparing `shtab-1.6.2/docs/pydoc_markdown_shtab.py` & `shtab-1.6.3/docs/pydoc_markdown_shtab.py`

 * *Files identical despite different names*

### Comparing `shtab-1.6.2/docs/use.md` & `shtab-1.6.3/docs/use.md`

 * *Files identical despite different names*

### Comparing `shtab-1.6.2/examples/customcomplete.py` & `shtab-1.6.3/examples/customcomplete.py`

 * *Files identical despite different names*

### Comparing `shtab-1.6.2/examples/docopt-greeter.py` & `shtab-1.6.3/examples/docopt-greeter.py`

 * *Files identical despite different names*

### Comparing `shtab-1.6.2/examples/pathcomplete.py` & `shtab-1.6.3/examples/pathcomplete.py`

 * *Files identical despite different names*

### Comparing `shtab-1.6.2/meta/logo.png` & `shtab-1.6.3/meta/logo.png`

 * *Files identical despite different names*

### Comparing `shtab-1.6.2/pyproject.toml` & `shtab-1.6.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `shtab-1.6.2/shtab/__init__.py` & `shtab-1.6.3/shtab/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -470,81 +470,91 @@
 
     def is_opt_end(opt):
         return isinstance(opt, OPTION_END) or opt.nargs == REMAINDER
 
     def is_opt_multiline(opt):
         return isinstance(opt, OPTION_MULTI)
 
-    def format_optional(opt):
+    def format_optional(opt, parser):
+        get_help = parser._get_formatter()._expand_help
         return (('{nargs}{options}"[{help}]"' if isinstance(
             opt, FLAG_OPTION) else '{nargs}{options}"[{help}]:{dest}:{pattern}"').format(
                 nargs=('"(- : *)"' if is_opt_end(opt) else '"*"' if is_opt_multiline(opt) else ""),
                 options=("{{{}}}".format(",".join(opt.option_strings)) if len(opt.option_strings)
                          > 1 else '"{}"'.format("".join(opt.option_strings))),
-                help=escape_zsh(opt.help or ""),
+                help=escape_zsh(get_help(opt) if opt.help else ""),
                 dest=opt.dest,
                 pattern=complete2pattern(opt.complete, "zsh", choice_type2fn) if hasattr(
                     opt, "complete") else
                 (choice_type2fn[opt.choices[0].type] if isinstance(opt.choices[0], Choice) else
                  "({})".format(" ".join(map(str, opt.choices)))) if opt.choices else "",
             ).replace('""', ""))
 
-    def format_positional(opt):
+    def format_positional(opt, parser):
+        get_help = parser._get_formatter()._expand_help
         return '"{nargs}:{help}:{pattern}"'.format(
             nargs={ONE_OR_MORE: "(*)", ZERO_OR_MORE: "(*):", REMAINDER: "(-)*"}.get(opt.nargs, ""),
-            help=escape_zsh((opt.help or opt.dest).strip().split("\n")[0]),
+            help=escape_zsh((get_help(opt) if opt.help else opt.dest).strip().split("\n")[0]),
             pattern=complete2pattern(opt.complete, "zsh", choice_type2fn) if hasattr(
                 opt, "complete") else
             (choice_type2fn[opt.choices[0].type] if isinstance(opt.choices[0], Choice) else
              "({})".format(" ".join(map(str, opt.choices)))) if opt.choices else "",
         )
 
     # {cmd: {"help": help, "arguments": [arguments]}}
     all_commands = {
         root_prefix: {
             "cmd": prog, "arguments": [
-                format_optional(opt)
+                format_optional(opt, parser)
                 for opt in parser._get_optional_actions() if opt.help != SUPPRESS] + [
-                    format_positional(opt) for opt in parser._get_positional_actions()
+                    format_positional(opt, parser) for opt in parser._get_positional_actions()
                     if opt.help != SUPPRESS and opt.choices is None],
             "help": (parser.description
                      or "").strip().split("\n")[0], "commands": [], "paths": []}}
 
     def recurse(parser, prefix, paths=None):
         paths = paths or []
         subcmds = []
         for sub in parser._get_positional_actions():
             if sub.help == SUPPRESS or not sub.choices:
                 continue
             if not sub.choices or not isinstance(sub.choices, dict):
                 # positional argument
-                all_commands[prefix]["arguments"].append(format_positional(sub))
+                all_commands[prefix]["arguments"].append(format_positional(sub, parser))
             else:  # subparser
                 log.debug(f"choices:{prefix}:{sorted(sub.choices)}")
                 public_cmds = get_public_subcommands(sub)
                 for cmd, subparser in sub.choices.items():
                     if cmd not in public_cmds:
                         log.debug("skip:subcommand:%s", cmd)
                         continue
                     log.debug("subcommand:%s", cmd)
 
                     # optionals
                     arguments = [
-                        format_optional(opt) for opt in subparser._get_optional_actions()
+                        format_optional(opt, parser) for opt in subparser._get_optional_actions()
                         if opt.help != SUPPRESS]
 
                     # positionals
                     arguments.extend(
-                        format_positional(opt) for opt in subparser._get_positional_actions()
+                        format_positional(opt, parser)
+                        for opt in subparser._get_positional_actions()
                         if not isinstance(opt.choices, dict) if opt.help != SUPPRESS)
 
+                    # help text
+                    formatter = subparser._get_formatter()
+                    backup_width = formatter._width
+                    formatter._width = 1234567 # large number to effectively disable wrapping
+                    desc = formatter._format_text(subparser.description or "").strip()
+                    formatter._width = backup_width
+
                     new_pref = f"{prefix}_{wordify(cmd)}"
                     options = all_commands[new_pref] = {
-                        "cmd": cmd, "help": (subparser.description or "").strip().split("\n")[0],
-                        "arguments": arguments, "paths": [*paths, cmd]}
+                        "cmd": cmd, "help": desc.split("\n")[0], "arguments": arguments,
+                        "paths": [*paths, cmd]}
                     new_subcmds = recurse(subparser, new_pref, [*paths, cmd])
                     options["commands"] = {
                         all_commands[pref]["cmd"]: all_commands[pref]
                         for pref in new_subcmds if pref in all_commands}
                     subcmds.extend([*new_subcmds, new_pref])
                     log.debug("subcommands:%s:%s", cmd, options)
         return subcmds
```

### Comparing `shtab-1.6.2/shtab/main.py` & `shtab-1.6.3/shtab/main.py`

 * *Files identical despite different names*

### Comparing `shtab-1.6.2/shtab.egg-info/PKG-INFO` & `shtab-1.6.3/shtab.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shtab
-Version: 1.6.2
+Version: 1.6.3
 Summary: Automagic shell tab completion for Python CLI applications
 Author-email: Casper da Costa-Luis <casper.dcl@physics.org>
 Maintainer-email: Iterative <support@iterative.ai>
 License: Apache-2.0
 Project-URL: documentation, https://docs.iterative.ai/shtab
 Project-URL: repository, https://github.com/iterative/shtab
 Project-URL: changelog, https://github.com/iterative/shtab/releases
@@ -63,15 +63,15 @@
 License-File: LICENCE
 
 |Logo|
 
 shtab
 =====
 
-|Tests| |Coverage| |Conda| |PyPI|
+|PyPI-Downloads| |Tests| |Coverage| |PyPI| |Conda|
 
 - What: Automatically generate shell tab completion scripts for Python CLI apps
 - Why: Speed & correctness. Alternatives like
   `argcomplete <https://pypi.org/project/argcomplete>`_ and
   `pyzshcomplete <https://pypi.org/project/pyzshcomplete>`_ are slow and have
   side-effects
 - How: ``shtab`` processes an ``argparse.ArgumentParser`` object to generate a
@@ -120,16 +120,16 @@
 
   - may not require any code modifications whatsoever
   - end-users execute ``shtab your_cli_app.your_parser_object``
 
 - `Library Usage <https://docs.iterative.ai/shtab/use/#library-usage>`_: as a library integrated into your CLI application
 
   - adds a couple of lines to your application
-  - argument mode: end-users execute ``your_cli_app --print-completion {bash,zsh}``
-  - subparser mode: end-users execute ``your_cli_app completion {bash,zsh}``
+  - argument mode: end-users execute ``your_cli_app --print-completion {bash,zsh,tcsh}``
+  - subparser mode: end-users execute ``your_cli_app completion {bash,zsh,tcsh}``
 
 Examples
 --------
 
 See `the docs for usage examples <https://docs.iterative.ai/shtab/use/#main.py>`_.
 
 FAQs
@@ -168,22 +168,25 @@
 See
 `CONTRIBUTING.md <https://github.com/iterative/shtab/tree/main/CONTRIBUTING.md>`_
 for more guidance.
 
 |Hits|
 
 .. |Logo| image:: https://github.com/iterative/shtab/raw/main/meta/logo.png
-.. |Tests| image:: https://github.com/iterative/shtab/workflows/Test/badge.svg
+.. |Tests| image:: https://img.shields.io/github/actions/workflow/status/iterative/shtab/test.yml?logo=github&label=tests
    :target: https://github.com/iterative/shtab/actions
    :alt: Tests
 .. |Coverage| image:: https://codecov.io/gh/iterative/shtab/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/iterative/shtab
    :alt: Coverage
 .. |Conda| image:: https://img.shields.io/conda/v/conda-forge/shtab.svg?label=conda&logo=conda-forge
    :target: https://anaconda.org/conda-forge/shtab
    :alt: conda-forge
 .. |PyPI| image:: https://img.shields.io/pypi/v/shtab.svg?label=pip&logo=PyPI&logoColor=white
    :target: https://pypi.org/project/shtab
    :alt: PyPI
+.. |PyPI-Downloads| image:: https://img.shields.io/pypi/dm/shtab.svg?label=pypi%20downloads&logo=PyPI&logoColor=white
+   :target: https://pepy.tech/project/shtab
+   :alt: Downloads
 .. |Hits| image:: https://caspersci.uk.to/cgi-bin/hits.cgi?q=shtab&style=social&r=https://github.com/iterative/shtab&a=hidden
    :target: https://caspersci.uk.to/cgi-bin/hits.cgi?q=shtab&a=plot&r=https://github.com/iterative/shtab&style=social
    :alt: Hits
```

### Comparing `shtab-1.6.2/shtab.egg-info/SOURCES.txt` & `shtab-1.6.3/shtab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shtab-1.6.2/tests/test_shtab.py` & `shtab-1.6.3/tests/test_shtab.py`

 * *Files identical despite different names*

