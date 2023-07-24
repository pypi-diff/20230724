# Comparing `tmp/setuptools-github-0.2.2b48.tar.gz` & `tmp/setuptools-github-0.3.0b59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setuptools-github-0.2.2b48.tar", last modified: Tue Jun 28 23:43:53 2022, max compression
+gzip compressed data, was "setuptools-github-0.3.0b59.tar", last modified: Mon Jul 24 16:54:02 2023, max compression
```

## Comparing `setuptools-github-0.2.2b48.tar` & `setuptools-github-0.3.0b59.tar`

### file list

```diff
@@ -1,27 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 23:43:53.453850 setuptools-github-0.2.2b48/
--rw-r--r--   0 runner    (1001) docker     (121)     1315 2022-06-28 23:43:23.000000 setuptools-github-0.2.2b48/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-06-28 23:43:23.000000 setuptools-github-0.2.2b48/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6102 2022-06-28 23:43:53.453850 setuptools-github-0.2.2b48/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5379 2022-06-28 23:43:23.000000 setuptools-github-0.2.2b48/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-06-28 23:43:23.000000 setuptools-github-0.2.2b48/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-28 23:43:53.453850 setuptools-github-0.2.2b48/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3122 2022-06-28 23:43:23.000000 setuptools-github-0.2.2b48/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 23:43:53.453850 setuptools-github-0.2.2b48/setuptools_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6102 2022-06-28 23:43:52.000000 setuptools-github-0.2.2b48/setuptools_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      548 2022-06-28 23:43:53.000000 setuptools-github-0.2.2b48/setuptools_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-28 23:43:52.000000 setuptools-github-0.2.2b48/setuptools_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-06-28 23:43:53.000000 setuptools-github-0.2.2b48/setuptools_github.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-06-28 23:43:53.000000 setuptools-github-0.2.2b48/setuptools_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-06-28 23:43:53.000000 setuptools-github-0.2.2b48/setuptools_github.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 23:43:53.449850 setuptools-github-0.2.2b48/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 23:43:53.453850 setuptools-github-0.2.2b48/src/setuptools_github/
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-06-28 23:43:52.000000 setuptools-github-0.2.2b48/src/setuptools_github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5867 2022-06-28 23:43:23.000000 setuptools-github-0.2.2b48/src/setuptools_github/checks.py
--rw-r--r--   0 runner    (1001) docker     (121)     8503 2022-06-28 23:43:23.000000 setuptools-github-0.2.2b48/src/setuptools_github/start_release.py
--rw-r--r--   0 runner    (1001) docker     (121)    13597 2022-06-28 23:43:23.000000 setuptools-github-0.2.2b48/src/setuptools_github/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 23:43:53.453850 setuptools-github-0.2.2b48/tests/
--rw-r--r--   0 runner    (1001) docker     (121)    11052 2022-06-28 23:43:23.000000 setuptools-github-0.2.2b48/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-28 23:43:23.000000 setuptools-github-0.2.2b48/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5764 2022-06-28 23:43:23.000000 setuptools-github-0.2.2b48/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (121)    13189 2022-06-28 23:43:23.000000 setuptools-github-0.2.2b48/tests/test_start_release.py
--rw-r--r--   0 runner    (1001) docker     (121)    10505 2022-06-28 23:43:23.000000 setuptools-github-0.2.2b48/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:02.991473 setuptools-github-0.3.0b59/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-24 16:53:35.000000 setuptools-github-0.3.0b59/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-24 16:53:35.000000 setuptools-github-0.3.0b59/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-07-24 16:54:02.991473 setuptools-github-0.3.0b59/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-07-24 16:53:35.000000 setuptools-github-0.3.0b59/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-24 16:53:35.000000 setuptools-github-0.3.0b59/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 16:54:02.991473 setuptools-github-0.3.0b59/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-24 16:53:35.000000 setuptools-github-0.3.0b59/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:02.991473 setuptools-github-0.3.0b59/setuptools_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-07-24 16:54:02.000000 setuptools-github-0.3.0b59/setuptools_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-24 16:54:02.000000 setuptools-github-0.3.0b59/setuptools_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 16:54:02.000000 setuptools-github-0.3.0b59/setuptools_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-24 16:54:02.000000 setuptools-github-0.3.0b59/setuptools_github.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-24 16:54:02.000000 setuptools-github-0.3.0b59/setuptools_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 16:54:02.000000 setuptools-github-0.3.0b59/setuptools_github.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:02.987473 setuptools-github-0.3.0b59/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:02.991473 setuptools-github-0.3.0b59/src/setuptools_github/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-24 16:54:02.000000 setuptools-github-0.3.0b59/src/setuptools_github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-07-24 16:53:35.000000 setuptools-github-0.3.0b59/src/setuptools_github/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-07-24 16:53:35.000000 setuptools-github-0.3.0b59/src/setuptools_github/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-24 16:53:35.000000 setuptools-github-0.3.0b59/src/setuptools_github/scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-24 16:53:35.000000 setuptools-github-0.3.0b59/src/setuptools_github/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8072 2023-07-24 16:53:35.000000 setuptools-github-0.3.0b59/src/setuptools_github/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:02.991473 setuptools-github-0.3.0b59/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    12555 2023-07-24 16:53:35.000000 setuptools-github-0.3.0b59/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-24 16:53:35.000000 setuptools-github-0.3.0b59/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-07-24 16:53:35.000000 setuptools-github-0.3.0b59/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-24 16:53:35.000000 setuptools-github-0.3.0b59/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-24 16:53:35.000000 setuptools-github-0.3.0b59/tests/test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-07-24 16:53:35.000000 setuptools-github-0.3.0b59/tests/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-07-24 16:53:35.000000 setuptools-github-0.3.0b59/tests/test_tools.py
```

### Comparing `setuptools-github-0.2.2b48/LICENSE` & `setuptools-github-0.3.0b59/LICENSE`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.2.2b48/PKG-INFO` & `setuptools-github-0.3.0b59/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,141 @@
 Metadata-Version: 2.1
 Name: setuptools-github
-Version: 0.2.2b48
+Version: 0.3.0b59
 Summary: supports github releases
 Home-page: https://github.com/cav71/setuptools-github
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
-=================
 setuptools-github
 =================
 
-.. image:: https://img.shields.io/pypi/v/click-plus.svg
-   :target: https://pypi.org/project/click-plus
-   :alt: PyPI version
-
-.. image:: https://img.shields.io/pypi/pyversions/click-plus.svg
-   :target: https://pypi.org/project/click-plus
-   :alt: Python versions
-
-.. image:: https://github.com/cav71/click-plus/actions/workflows/master.yml/badge.svg
-   :target: https://github.com/cav71/click-plus/actions
-   :alt: Build
-
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
-   :alt: Black
-
-.. image:: https://codecov.io/gh/cav71/setuptools-github/branch/master/graph/badge.svg?token=SIUMZ7MT5T
-   :target: https://codecov.io/gh/cav71/setuptools-github
-   :alt: Coverage
-
-Intro
------
-
-**setuptools-github** is both a library and a script to support simple life cycle management for
-software projects.
-
-It is based on a simple and lightweight approach based on a single **master** branch,
-a 'release' branch (**beta/N.M.O**) and finally a 'release' tag (**release/N.M.O**) from which the final
-stable packages are generated from.
+[![PyPI version](https://img.shields.io/pypi/v/setuptools-github.svg?color=blue)](https://pypi.org/project/setuptools-github)
+[![Python versions](https://img.shields.io/pypi/pyversions/setuptools-github.svg)](https://pypi.org/project/setuptools-github)
+[![Build](https://github.com/cav71/setuptools-github/actions/workflows/master.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions)
+[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
+[![Coverage](https://codecov.io/gh/cav71/setuptools-github/branch/master/graph/badge.svg?token=SIUMZ7MT5T)](Coverage)
+
+
+## Intro
+setuptools-github helps to implement a simple project life cycle
+aimed at delivering packages into [PyPI](https://pypi.org): 
+there are three important components.
+
+#### /master branch
+This is the branch for CI build and code quality checks as:
+  - run flake8
+  - mypy
+  - pytest + coverage
+    (see *.github/workflows/master.yml*)
+
+Work from other feature branches get integrated here, for testing.
+
+#### /beta/N.M.O branch
+This branch (on each commit) will generate a 
+beta **package-N.M.O.bX** into [PyPI](https://pypi.org).
+**X** denotes a unique increasing build number.
+  - run flake8
+  - mypy
+  - pytest + coverage
+    (see *.github/workflows/master.yml*)
+  - packaging the wheel for **package-N.M.O.bX**
+  - (optional) publish the 
+
+Changes from **/master** branch get pushed here, to prepare for packaging
+into *beta* packages: these are continuosly released and they can 
+be used for integration testing.
+
+#### /release/N.M.O tag
+On tagging a commit in a **/beta/N.M.O** branch will delivere the 
+formal package **package-N.M.O** into [PyPI](https://pypi.org).
+
+> **NOTE:** All packages include a __version__ and __hash__ variables, used to
+> link the generated package with the source code.
+
+## Quick start
+
+Start from the */master* branch:
+
+**Setup the version file**
+
+We will use src/package_name/__init__.py to store the package information:
+```
+__version__ = "N.M.O"  # replace N, M and O with numerical values (eg. 0.0.0)
+__hash__ = ""  # leave this empty
+```
+
+**Add the setup data**
+
+In setup.py add:
+```
+from setuptools_github import tools
+initfile = pathlib.Path(__file__).parent / "your_package/__init__.py"
+setup(
+  name="package-name",
+  version=tools.update_version(initfile, os.getenv("GITHUB_DUMP")),
+  ...
+```
+
+**Copy the github actions**
+
+Copy all github action files from 
+[workflows](https://github.com/cav71/setuptools-github/tree/release/0.3.0/.github/workflows)
+
+## Development
+Once the setup is done, the workflow is rather simple.
+
+### /master branch
+Commit into the **master** branch and for each commit CI (github) will:
+  - run flake8
+  - mypy
+  - pytest + coverage
+    (see *.github/workflows/master.yml*)
+
+### /beta/N.M.O
+Create a new beta branch to start creating packages on PyPi:
+```bash
+setuptools-github src/package/__init__.py make-beta
+```
+(assuming src/package/__init__.py contains the __version__ variable)
+
+* Create and use a **beta/N.M.O** branch to integrate work from **master** and for each commit CI (github) will:
+  - run flake8
+  - mypy
+  - pytest + coverage
+  - (optional) send the coverage to codecov
+  - create a **beta** wheel as **package-N.M.Ob#1234** (1234 is a sequential build number)
+  - publish it into pypi.org as beta package
+
+* Once ready for full release `setuptools-github-start-release micro src/your_package/__init__.py`:
+  - create the tag **beta/N.M.O** pointing to the latest **releaase/N.M.O** commit
+  - this will trigger the **release** wheel as **package-N.M.Ob** creation
+  - publish it into pypi.org as released package
 
 **setuptools-github** is fully CI/CD integrated (github actions) to eliminate any manual step involved
 with software deployment (except code writing).
 
+
+Project Setup
+=============
+
+First add a "version" file in the source code eg. src/package_name/__init__.py with a content like this:
+
+
 The generated package provides two important variables (auto updated from the code leveraging automation):
 
    #. __version__ with the code version
    #. __hash__ with the has commit where the code originates from
 
 To enable..
 
@@ -141,24 +219,24 @@
     #. unit and integration testing
     #. code coverage
     #. static code check
     #. style check
 
 No package artifact are generated here as the code is not "installable" (eg. is still in source version).
 
-.. image:: maintainer/master-branch.png
+.. image:: https://github.com/cav71/setuptools-github/blob/release/0.2.2/maintainer/master-branch.png?raw=true
    :alt: blha
    :width: 400
 
 The delivery branch
 ~~~~~~~~~~~~~~~~~~~
 
 The next step is branching **master** into a "delivery" branch using the **beta/N.M.O** name convention.
 
-.. image:: maintainer/delivery-branch.png
+.. image:: https://raw.githubusercontent.com/cav71/setuptools-github/release/0.2.2/maintainer/delivery-branch.png
    :alt: blha
    :width: 400
 
 
 package deliveries using beta branches on github:
 in a simple model each (automated) commit on a beta/N.M.O branch will result in a package with a __version__
 of N.M.Ob<build-number> and a __hash__ corresponding to the commit.
```

### Comparing `setuptools-github-0.2.2b48/setuptools_github.egg-info/PKG-INFO` & `setuptools-github-0.3.0b59/setuptools_github.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,141 @@
 Metadata-Version: 2.1
 Name: setuptools-github
-Version: 0.2.2b48
+Version: 0.3.0b59
 Summary: supports github releases
 Home-page: https://github.com/cav71/setuptools-github
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
-=================
 setuptools-github
 =================
 
-.. image:: https://img.shields.io/pypi/v/click-plus.svg
-   :target: https://pypi.org/project/click-plus
-   :alt: PyPI version
-
-.. image:: https://img.shields.io/pypi/pyversions/click-plus.svg
-   :target: https://pypi.org/project/click-plus
-   :alt: Python versions
-
-.. image:: https://github.com/cav71/click-plus/actions/workflows/master.yml/badge.svg
-   :target: https://github.com/cav71/click-plus/actions
-   :alt: Build
-
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
-   :alt: Black
-
-.. image:: https://codecov.io/gh/cav71/setuptools-github/branch/master/graph/badge.svg?token=SIUMZ7MT5T
-   :target: https://codecov.io/gh/cav71/setuptools-github
-   :alt: Coverage
-
-Intro
------
-
-**setuptools-github** is both a library and a script to support simple life cycle management for
-software projects.
-
-It is based on a simple and lightweight approach based on a single **master** branch,
-a 'release' branch (**beta/N.M.O**) and finally a 'release' tag (**release/N.M.O**) from which the final
-stable packages are generated from.
+[![PyPI version](https://img.shields.io/pypi/v/setuptools-github.svg?color=blue)](https://pypi.org/project/setuptools-github)
+[![Python versions](https://img.shields.io/pypi/pyversions/setuptools-github.svg)](https://pypi.org/project/setuptools-github)
+[![Build](https://github.com/cav71/setuptools-github/actions/workflows/master.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions)
+[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
+[![Coverage](https://codecov.io/gh/cav71/setuptools-github/branch/master/graph/badge.svg?token=SIUMZ7MT5T)](Coverage)
+
+
+## Intro
+setuptools-github helps to implement a simple project life cycle
+aimed at delivering packages into [PyPI](https://pypi.org): 
+there are three important components.
+
+#### /master branch
+This is the branch for CI build and code quality checks as:
+  - run flake8
+  - mypy
+  - pytest + coverage
+    (see *.github/workflows/master.yml*)
+
+Work from other feature branches get integrated here, for testing.
+
+#### /beta/N.M.O branch
+This branch (on each commit) will generate a 
+beta **package-N.M.O.bX** into [PyPI](https://pypi.org).
+**X** denotes a unique increasing build number.
+  - run flake8
+  - mypy
+  - pytest + coverage
+    (see *.github/workflows/master.yml*)
+  - packaging the wheel for **package-N.M.O.bX**
+  - (optional) publish the 
+
+Changes from **/master** branch get pushed here, to prepare for packaging
+into *beta* packages: these are continuosly released and they can 
+be used for integration testing.
+
+#### /release/N.M.O tag
+On tagging a commit in a **/beta/N.M.O** branch will delivere the 
+formal package **package-N.M.O** into [PyPI](https://pypi.org).
+
+> **NOTE:** All packages include a __version__ and __hash__ variables, used to
+> link the generated package with the source code.
+
+## Quick start
+
+Start from the */master* branch:
+
+**Setup the version file**
+
+We will use src/package_name/__init__.py to store the package information:
+```
+__version__ = "N.M.O"  # replace N, M and O with numerical values (eg. 0.0.0)
+__hash__ = ""  # leave this empty
+```
+
+**Add the setup data**
+
+In setup.py add:
+```
+from setuptools_github import tools
+initfile = pathlib.Path(__file__).parent / "your_package/__init__.py"
+setup(
+  name="package-name",
+  version=tools.update_version(initfile, os.getenv("GITHUB_DUMP")),
+  ...
+```
+
+**Copy the github actions**
+
+Copy all github action files from 
+[workflows](https://github.com/cav71/setuptools-github/tree/release/0.3.0/.github/workflows)
+
+## Development
+Once the setup is done, the workflow is rather simple.
+
+### /master branch
+Commit into the **master** branch and for each commit CI (github) will:
+  - run flake8
+  - mypy
+  - pytest + coverage
+    (see *.github/workflows/master.yml*)
+
+### /beta/N.M.O
+Create a new beta branch to start creating packages on PyPi:
+```bash
+setuptools-github src/package/__init__.py make-beta
+```
+(assuming src/package/__init__.py contains the __version__ variable)
+
+* Create and use a **beta/N.M.O** branch to integrate work from **master** and for each commit CI (github) will:
+  - run flake8
+  - mypy
+  - pytest + coverage
+  - (optional) send the coverage to codecov
+  - create a **beta** wheel as **package-N.M.Ob#1234** (1234 is a sequential build number)
+  - publish it into pypi.org as beta package
+
+* Once ready for full release `setuptools-github-start-release micro src/your_package/__init__.py`:
+  - create the tag **beta/N.M.O** pointing to the latest **releaase/N.M.O** commit
+  - this will trigger the **release** wheel as **package-N.M.Ob** creation
+  - publish it into pypi.org as released package
 
 **setuptools-github** is fully CI/CD integrated (github actions) to eliminate any manual step involved
 with software deployment (except code writing).
 
+
+Project Setup
+=============
+
+First add a "version" file in the source code eg. src/package_name/__init__.py with a content like this:
+
+
 The generated package provides two important variables (auto updated from the code leveraging automation):
 
    #. __version__ with the code version
    #. __hash__ with the has commit where the code originates from
 
 To enable..
 
@@ -141,24 +219,24 @@
     #. unit and integration testing
     #. code coverage
     #. static code check
     #. style check
 
 No package artifact are generated here as the code is not "installable" (eg. is still in source version).
 
-.. image:: maintainer/master-branch.png
+.. image:: https://github.com/cav71/setuptools-github/blob/release/0.2.2/maintainer/master-branch.png?raw=true
    :alt: blha
    :width: 400
 
 The delivery branch
 ~~~~~~~~~~~~~~~~~~~
 
 The next step is branching **master** into a "delivery" branch using the **beta/N.M.O** name convention.
 
-.. image:: maintainer/delivery-branch.png
+.. image:: https://raw.githubusercontent.com/cav71/setuptools-github/release/0.2.2/maintainer/delivery-branch.png
    :alt: blha
    :width: 400
 
 
 package deliveries using beta branches on github:
 in a simple model each (automated) commit on a beta/N.M.O branch will result in a package with a __version__
 of N.M.Ob<build-number> and a __hash__ corresponding to the commit.
```

### Comparing `setuptools-github-0.2.2b48/setuptools_github.egg-info/SOURCES.txt` & `setuptools-github-0.3.0b59/setuptools_github.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 LICENSE
 MANIFEST.in
-README.rst
+README.md
 pyproject.toml
 setup.py
 setuptools_github.egg-info/PKG-INFO
 setuptools_github.egg-info/SOURCES.txt
 setuptools_github.egg-info/dependency_links.txt
 setuptools_github.egg-info/entry_points.txt
 setuptools_github.egg-info/requires.txt
 setuptools_github.egg-info/top_level.txt
 src/setuptools_github/__init__.py
 src/setuptools_github/checks.py
-src/setuptools_github/start_release.py
+src/setuptools_github/cli.py
+src/setuptools_github/scm.py
+src/setuptools_github/script.py
 src/setuptools_github/tools.py
 tests/conftest.py
 tests/requirements.txt
 tests/test_checks.py
-tests/test_start_release.py
+tests/test_cli.py
+tests/test_conftest.py
+tests/test_scm.py
 tests/test_tools.py
```

### Comparing `setuptools-github-0.2.2b48/src/setuptools_github/checks.py` & `setuptools-github-0.3.0b59/src/setuptools_github/checks.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.2.2b48/src/setuptools_github/tools.py` & `setuptools-github-0.3.0b59/tests/conftest.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,442 +1,374 @@
 from __future__ import annotations
 
+import os
 import io
 import re
-import ast
 import sys
-import json
+import pathlib
+import shutil
+import contextlib
+import collections
 import subprocess
+import dataclasses as dc
+from typing import Union, Optional
 
-from pathlib import Path
-from typing import Any, Union, Tuple, Optional, List, Dict, TextIO
+import pytest
 
 
-class GithubError(Exception):
-    pass
-
-
-class MissingVariable(GithubError):
-    pass
-
-
-class InvalidGithubReference(GithubError):
-    pass
-
-
-class AbortExecution(Exception):
-    @staticmethod
-    def _strip(txt):
-        txt = txt or ""
-        txt = txt[1:] if txt.startswith("\n") else txt
-        txt = indent(txt, pre="")
-        return txt[:-1] if txt.endswith("\n") else txt
-
-    def __init__(
-        self, message: str, explain: Optional[str] = None, hint: Optional[str] = None
-    ):
-        self.message = message.strip()
-        self._explain = explain
-        self._hint = hint
-
-    @property
-    def explain(self):
-        return self._strip(self._explain)
-
-    @property
-    def hint(self):
-        return self._strip(self._hint)
-
-    def __str__(self):
-        result = [self.message]
-        if self.explain:
-            result.append(indent("\n" + self.explain, pre=" " * 2)[2:])
-        if self.hint:
-            result.extend(["\nhint:", indent("\n" + self.hint, pre=" " * 2)[2:]])
-        return "".join(result)
-
-
-def urmtree(path: Path):
-    from os import name
-    from shutil import rmtree
-    from stat import S_IWUSR
-    if name == "nt":
-        for p in path.rglob("*"):
-            p.chmod(S_IWUSR)
-    rmtree(path, ignore_errors=True)
-    assert not path.exists()
-
-
-def indent(txt: str, pre: str = " " * 2) -> str:
-    "simple text indentation"
-
-    from textwrap import dedent
-
-    txt = dedent(txt)
-    if txt.endswith("\n"):
-        last_eol = "\n"
-        txt = txt[:-1]
-    else:
-        last_eol = ""
-
-    return pre + txt.replace("\n", "\n" + pre) + last_eol
+@pytest.fixture()
+def datadir(request):
+    basedir = pathlib.Path(__file__).parent / "data"
+    if os.getenv("DATADIR"):
+        basedir = pathlib.Path(os.getenv("DATADIR"))
+    basedir = basedir / getattr(request.module, "DATADIR", "")
+    return basedir
+
+
+@pytest.fixture()
+def scripter(request, tmp_path_factory, datadir):
+    """handles script (cli) execution
+
+    def test(scripter):
+        script = scripter / "script-file.py"
+        result = script.run(["--help"]) # this will execute:
+                                        #   script-file.py --help
+        assert result.out and result.err
+    """
+    Result = collections.namedtuple("R", "out,err,code")
 
+    class ScripterError(Exception):
+        pass
 
-def hubversion(gdata: Any, fallback: Optional[str]) -> Tuple[Optional[str], str]:
-    """gets a (version, sha) tuple from gdata.
+    class MissingItemError(ScripterError):
+        pass
 
-    GITHUB_DUMP is a json dump of the environment during an action run and
-    we pull the ref, run_number and sha keys.
+    class Exe:
+        def __repr__(self):
+            return (
+                f"<{self.__class__.__name__} script={self.script} at {hex(id(self))}>"
+            )
+
+        def __init__(self, script, workdir, datadir, exe):
+            self.script = script
+            self.workdir = workdir
+            self.datadir = datadir
+            self.exe = exe
+            if not pathlib.Path(script).exists():
+                raise MissingItemError(f"script file {script} not found")
+
+        def run(self, args, cwd=None, load_data=True):
+            cmd = [str(a) for a in [self.exe, self.script, *args]]
+
+            with contextlib.ExitStack() as stack:
+                fpout = stack.enter_context((self.workdir / "stdout.txt").open("w"))
+                fperr = stack.enter_context((self.workdir / "stderr.txt").open("w"))
+                self.p = subprocess.Popen(
+                    cmd,
+                    cwd=self.workdir if cwd is True else cwd,
+                    stdout=fpout,
+                    stderr=fperr,
+                )
+                self.p.communicate()
+            out = (self.workdir / "stdout.txt").read_text()
+            err = (self.workdir / "stderr.txt").read_text()
+            return Result(
+                out.replace("\r\n", "\n"), err.replace("\r\n", "\n"), self.p.returncode
+            )
+
+        def compare(self, refdir, populate=False):
+            src = self.datadir / refdir
+            if not src.exists():
+                raise MissingItemError(f"reference dir {src} not found")
+
+            for name in ["stdout.txt", "stderr.txt"]:
+                left = src / name
+                right = self.workdir / name
+                if populate:
+                    if left.exists():
+                        raise ScripterError(f"cannot overwrite {left} with {right}")
+                    shutil.copyfile(right, left)
+                assert left.read_text() == right.read_text()
+
+    class Scripter:
+        def __init__(self, srcdir, datadir, exe=sys.executable):
+            self.srcdir = srcdir
+            self.datadir = datadir
+            self.exe = exe
+
+        def __truediv__(self, path):
+            tmpdir = tmp_path_factory.mktemp(pathlib.Path(path).with_suffix("").name)
+            return Exe(self.srcdir / path, tmpdir, self.datadir, self.exe)
+
+    return Scripter(pathlib.Path(request.module.__file__).parent, datadir)
+
+
+##########################################################
+# GIT TEST HELPER                                        #
+#                                                        #
+#   def test(git_project_factory):                       #
+#       repo = git_project_factory().create()            #
+#       # clone from repo                                #
+#       repo1 = git_project_factory().create(clone=repo) #
+##########################################################
+
+@dc.dataclass
+class GitRepoBranches:
+    local: list[str]
+    remote: list[str]
+
+
+@pytest.fixture(scope="function")
+def git_project_factory(request, tmp_path):
+    """fixture to generate git working repositories
+
+    def test(git_project_factory):
+        # simple git repo (only 1 .keep file)
+        repo = git_project_factory().create()
 
-    ref can be something like refs/heads/master for the master branch,
-    refs/heads/beta/0.0.4 for a beta branch or refs/tags/release/0.0.3 for
-    a release tag.
+        # git repo with a "version" src/__init__.py file
+        repo1 = git_project_factory().create("0.0.0")
 
-    the version returned is:
-        ("", "<sha-value>") for the master branch
-        ("0.0.4b8", "<sha-value>") for a beta branch (<version>b<build-number>)
-        ("0.0.3", "<sha-value>") for the release
+        # clone from repo
+        repo2 = git_project_factory().create(clone=repo)
 
-    Args:
-        gdata: json dictionary from $GITHUB_DUMP
-        fallback: returns this if a version is not defined in gdata
+        assert repo.workdir != repo1.workdir
+        assert repo.workdir != repo1.workdir
 
-    Returns:
-        (str, str): <update-version>, <shasum>
     """
+    from pathlib import Path
 
-    def validate(txt):
-        return ".".join(str(int(v)) for v in txt.split("."))
+    def indent(txt, pre=" " * 2):
+        "simple text indentation"
 
-    ref = gdata["ref"]  # eg. "refs/tags/release/0.0.3"
-    number = gdata["run_number"]  # eg. 3
-    shasum = gdata["sha"]  # eg. "2169f90c"
+        from textwrap import dedent
 
-    # the logic for the returned version:
-
-    # 1. if we are on master we use the version from the __init__.py module
-    if ref == "refs/heads/master":
-        return (fallback, shasum)
+        txt = dedent(txt)
+        if txt.endswith("\n"):
+            last_eol = "\n"
+            txt = txt[:-1]
+        else:
+            last_eol = ""
 
-    # 2. on a beta branch we add a "b<build-number>" string to the __init__.py version
-    #    the bersion is taken from the refs/heads/beta/<version>
-    if ref.startswith("refs/heads/beta/"):
-        version = validate(ref.rpartition("/")[2])
-        return (f"{version}b{number}", shasum)
+        result = pre + txt.replace("\n", "\n" + pre) + last_eol
+        return result if result.strip() else ""
 
-    # 3. on a release we use the version from the refs/tags/release/<version>
-    if ref.startswith("refs/tags/release/"):
-        version = validate(ref.rpartition("/")[2])
-        return (f"{version}", shasum)
+    def to_list_of_paths(paths: str | Path | list[str | Path]) -> list[Path]:
+        return [Path(s) for s in ([paths] if isinstance(paths, (str, Path)) else paths)]
 
-    raise InvalidGithubReference("unhandled github ref", gdata)
+    class GitRepoBranches:
+        def __init__(self, local: list[str], remote: list[str]):
+            self.local = local
+            self.remote = remote
+
+    class GitRepo:
+        def __init__(
+            self,
+            workdir: Path | str,
+            identity: tuple[str, str] = ("First Last", "user@email"),
+            exe: str = "git",
+            gitdir: Path | str | None = None,
+        ):
+            self.workdir = Path(workdir).absolute()
+            self.identity = identity
+            self.exe = exe
+            self.gitdir = (
+                Path(gitdir) if gitdir else (self.workdir / ".git")
+            ).absolute()
 
+        def __call__(self, cmd: str | Path | list[str | Path]) -> str:
+            cmds = [cmd] if isinstance(cmd, str) else cmd
 
-def get_module_var(
-    path: Union[Path, str], var: str = "__version__", abort=True
-) -> Optional[str]:
-    """extract from a python module in path the module level <var> variable
+            arguments = [
+                self.exe,
+            ]
+            if str(cmds[0]) != "clone":
+                arguments.extend(
+                    [
+                        "--git-dir",
+                        self.gitdir,
+                        "--work-tree",
+                        self.workdir,
+                    ]
+                )
+            arguments.extend(cmds)
+            return subprocess.check_output(
+                [str(a) for a in arguments], encoding="utf-8"
+            )
 
-    Args:
-        path (str,Path): python module file to parse using ast (no code-execution)
-        var (str): module level variable name to extract
-        abort (bool): raise MissingVariable if var is not present
+        def _config(self, identity: tuple[str, str]):
+            self(["config", "user.name", identity[0]])
+            self(["config", "user.email", identity[1]])
 
-    Returns:
-        None or str: the variable value if found or None
+        def init(
+            self,
+            force: bool = False,
+            identity: tuple[str, str] | None = None,
+        ) -> GitRepo:
+            from shutil import rmtree
+
+            if force:
+                rmtree(self.workdir, ignore_errors=True)
+            self.workdir.mkdir(parents=True, exist_ok=True if force else False)
+
+            self(["init", "-b", "master"])
+            self._config(identity or self.identity)
+
+            self(["commit", "-m", "initial", "--allow-empty"])
+            return self
+
+        def clone(
+            self,
+            dest: Union[str, Path],
+            force=False,
+            branch: Optional[str] = None,
+        ) -> GitRepo:
+            from shutil import rmtree
+
+            workdir = Path(dest).absolute()
+            if force:
+                rmtree(workdir, ignore_errors=True)
+            if workdir.exists():
+                raise ValueError(f"target directory present {workdir}")
+
+            self(
+                [
+                    "clone",
+                    *(["--branch", branch] if branch else []),
+                    self.workdir.absolute(),
+                    workdir.absolute(),
+                ],
+            )
+
+            repo = self.__class__(workdir=workdir, identity=self.identity, exe=self.exe)
+            repo._config(self.identity)
+            return repo
+
+        def __truediv__(self, other):
+            return self.workdir.absolute() / other
+
+        def dumps(self, mask=False) -> str:
+            lines = f"REPO: {self.workdir}"
+            lines += "\n [status]\n" + indent(self(["status"]))
+            branches = self(["branch", "-avv"])
+            if mask:
+                branches = re.sub(r"(..\w\s+)\w{7}(\s+.*)", r"\1ABCDEFG\2", branches)
+            lines += "\n [branch]\n" + indent(branches)
+            lines += "\n [tags]\n" + indent(self(["tag", "-l"]))
+            lines += "\n [remote]\n" + indent(self(["remote", "-v"]))
 
-    Raises:
-        MissingVariable: if the var is not found and abort is True
+            buf = io.StringIO()
+            print("\n".join([line.rstrip() for line in lines.split("\n")]), file=buf)
+            return buf.getvalue()
 
-    Notes:
-        this uses ast to parse path, so it doesn't load the module
-    """
+    class GitCommand(GitRepo):
+        BETA_BRANCHES = re.compile(r"/beta/(?P<ver>\d+([.]\d+)*)")
 
-    class V(ast.NodeVisitor):
-        def __init__(self, keys):
-            self.keys = keys
-            self.result = {}
-
-        def visit_Module(self, node):
-            # we extract the module level variables
-            for subnode in ast.iter_child_nodes(node):
-                if not isinstance(subnode, ast.Assign):
+        def commit(
+            self,
+            paths: str | Path | list[str | Path],
+            message: str,
+        ) -> None:
+            paths = [paths] if isinstance(paths, (Path, str)) else paths
+            self(["add", *paths])
+            self(["commit", "-m", message, *paths])
+
+        def branch(self, name: Optional[str] = None, origin: str = "master") -> str:
+            if not name:
+                return self(["rev-parse", "--abbrev-ref", "HEAD"]).strip()
+            assert origin or origin is None
+            old = self.branch()
+            self(["checkout", "-b", name, "--track", origin])
+            return old
+
+        @property
+        def branches(self) -> GitRepoBranches:
+            result = GitRepoBranches([], [])
+            for line in self(["branch", "-a", "--format", "%(refname)"]).split("\n"):
+                if not line.strip():
                     continue
-                for target in subnode.targets:
-                    if target.id not in self.keys:
-                        continue
-                    assert isinstance(
-                        subnode.value, (ast.Num, ast.Str, ast.Constant)
-                    ), (
-                        f"cannot extract non Constant variable "
-                        f"{target.id} ({type(subnode.value)})"
-                    )
-                    if isinstance(subnode.value, ast.Str):
-                        value = subnode.value.s
-                    elif isinstance(subnode.value, ast.Num):
-                        value = subnode.value.n
-                    else:
-                        value = subnode.value.value
-                    self.result[target.id] = value
-            return self.generic_visit(node)
-
-    v = V({var})
-    path = Path(path)
-    if path.exists():
-        tree = ast.parse(Path(path).read_text())
-        v.visit(tree)
-    if var not in v.result and abort:
-        raise MissingVariable(f"cannot find {var} in {path}", path, var)
-    return v.result.get(var, None)
-
-
-def set_module_var(
-    path: Union[str, Path], var: str, value: Any, create: bool = True
-) -> Tuple[Any, str]:
-    """replace var in path with value
-
-    Args:
-        path (str,Path): python module file to parse
-        var (str): module level variable name to extract
-        value (None or Any): if not None replace var in initfile
-        create (bool): create path if not present
+                if line.startswith("refs/heads/"):
+                    result.local.append(line[11:])
+                elif line.startswith("refs/remotes/"):
+                    result.remote.append(line[13:])
+                else:
+                    raise RuntimeError(f"invalid branch {line}")
+            return result
+
+        def revert(self, paths: str | Path | list[str | Path] | None = None):
+            sources = to_list_of_paths(paths or self.workdir)
+            self(["checkout", *sources])
+
+        def status(self) -> dict[str, int]:
+            mapper = {
+                "??": 128,
+                " D": 512,
+                " M": 256,
+            }
+            result = {}
+            for line in self(["status", "--porcelain"]).split("\n"):
+                if not line.strip():
+                    continue
+                tag, filename = line[:2], line[3:]
+                value = mapper[tag]
+                if value:
+                    result[filename] = value
+            return result
+
+    class Project(GitCommand):
+        @property
+        def initfile(self):
+            return self.workdir / "src" / "__init__.py"
 
-    Returns:
-        (str, str) the (<previous-var-value|None>, <the new text>)
-    """
-    # module level var
-    expr = re.compile(f"^{var}\\s*=\\s*['\\\"](?P<value>[^\\\"']*)['\\\"]")
-    fixed = None
-    lines = []
-
-    src = Path(path)
-    if not src.exists() and create:
-        src.parent.mkdir(parents=True, exist_ok=True)
-        src.touch()
-
-    input_lines = src.read_text().split("\n")
-    for line in reversed(input_lines):
-        if fixed:
-            lines.append(line)
-            continue
-        match = expr.search(line)
-        if match:
-            fixed = match.group("value")
+        def version(self, value=None):
             if value is not None:
-                x, y = match.span(1)
-                line = line[:x] + value + line[y:]
-        lines.append(line)
-    txt = "\n".join(reversed(lines))
-    if not fixed and create:
-        if txt and txt[-1] != "\n":
-            txt += "\n"
-        txt += f'{var} = "{value}"'
-
-    with Path(path).open("w") as fp:
-        fp.write(txt)
-    return fixed, txt
-
-
-def update_version(
-    initfile: Union[str, Path], github_dump: Optional[str] = None
-) -> Optional[str]:
-    """extracts version information from github_dump and updates initfile in-place
-
-    Args:
-        initfile (str, Path): path to the __init__.py file with a __version__ variable
-        github_dump (str): the os.getenv("GITHUB_DUMP") value
-
-    Returns:
-        str: the new version for the package
-    """
-
-    path = Path(initfile)
-
-    if not github_dump:
-        return get_module_var(path, "__version__")
-    gdata = json.loads(github_dump) if isinstance(github_dump, str) else github_dump
-
-    version, thehash = hubversion(gdata, get_module_var(path, "__version__"))
-    set_module_var(path, "__version__", version)
-    set_module_var(path, "__hash__", thehash)
-    return version
-
-
-def bump_version(version: str, mode: str) -> str:
-    """given a version str will bump it according to mode
-
-    Arguments:
-        version: text in the N.M.O form
-        mode: major, minor or micro
-
-    Returns:
-        increased text
-
-    >>> bump_version("1.0.3", "micro")
-    "1.0.4"
-    >>> bump_version("1.0.3", "minor")
-    "1.1.0"
-    """
-    newver = [int(n) for n in version.split(".")]
-    if mode == "major":
-        newver[-3] += 1
-        newver[-2] = 0
-        newver[-1] = 0
-    elif mode == "minor":
-        newver[-2] += 1
-        newver[-1] = 0
-    elif mode == "micro":
-        newver[-1] += 1
-    return ".".join(str(v) for v in newver)
-
-
-class GitWrapper:
-    EXE: str = "git"
-    KEEPFILE = ".keep"
-
-    def __init__(
-        self,
-        workdir: Union[Path, str],
-        exe: Optional[str] = None,
-        identity: Tuple[str, str] = ("First Last", "user@email"),
-    ):
-        self.workdir = Path(workdir)
-        self.exe = exe or self.EXE
-        self.identity = identity
-
-    def init(
-        self,
-        force: bool = False,
-        keepfile: Optional[Union[bool, Path]] = True,
-        identity: Optional[Tuple[str, str]] = None,
-    ) -> GitWrapper:
-
-        identity = self.identity if identity is None else identity
-        keepfile = self.workdir / self.KEEPFILE if keepfile is True else keepfile
-
-        if force:
-            urmtree(self.workdir)
-        self.workdir.mkdir(parents=True, exist_ok=True if force else False)
-        self("init")
+                initial = not self.initfile.exists()
+                self.initfile.parent.mkdir(parents=True, exist_ok=True)
+                self.initfile.write_text(f'__version__ = "{value}"\n')
+                self.commit(
+                    [self.initfile], "initial commit" if initial else "update version"
+                )
+
+            if not self.initfile.exists():
+                return None
+
+            lines = [
+                line.partition("=")[2].strip().strip("'").strip('"')
+                for line in self.initfile.read_text().split("\n")
+                if line.strip().startswith("__version__")
+            ]
+            return lines[0] if lines else None
 
-        if identity:
-            self(["config", "user.name", identity[0]])
-            self(["config", "user.email", identity[1]])
+        def create(self, version=None, clone=None, force=False):
+            if clone:
+                clone.clone(self.workdir, force=force)
+            else:
+                self.init(force=force)
+            self.version(version)
+            return self
 
-        if keepfile:
-            keepfile.write_text("# dummy file to create the master branch")
-            self(["add", keepfile])
-            self(["commit", "-m", "initial", keepfile])
-        return self
-
-    def clone(
-        self,
-        dest: Union[str, Path],
-        force=False,
-        branch: Optional[str] = None,
-        exe: Optional[str] = None,
-        identity: Optional[Tuple[str, str]] = None,
-    ) -> GitWrapper:
-        dest = Path(dest)
-        identity = self.identity if identity is None else identity
-        exe = self.exe if exe is None else exe
+    def id_generator(size=6):
+        from string import ascii_uppercase, digits
+        from random import choice
 
-        if force:
-            urmtree(dest)
-        else:
-            if dest.exists():
-                raise ValueError(f"target directory present {dest}")
+        return "".join(choice(ascii_uppercase + digits) for _ in range(size))
 
-        self(
-            [
-                "clone",
-                *(["--branch", branch] if branch else []),
-                self.workdir.absolute(),
-                dest.absolute(),
-            ],
-        )
-
-        result = self.__class__(dest, exe=exe, identity=identity)
-        if identity:
-            result(["config", "user.name", identity[0]])
-            result(["config", "user.email", identity[1]])
-        return result
-
-    def __call__(self, cmd: Union[List[Any], Any], *args) -> str:
-        arguments = []
-        if isinstance(cmd, str):
-            arguments.append(cmd)
-        else:
-            arguments.extend(cmd[:])
+    return lambda subdir="": Project(tmp_path / (subdir or id_generator()))
+    # or request.node.name
 
-        if str(arguments[0]) != "clone":
-            arguments = [
-                self.exe,
-                "--git-dir",
-                str(self.workdir.absolute() / ".git"),
-                "--work-tree",
-                str(self.workdir.absolute()),
-                *[str(a) for a in arguments],
-            ]
-        else:
-            arguments = [self.exe, *[str(a) for a in arguments]]
-        return subprocess.check_output(arguments, encoding="utf-8")
+#####################
+# Main flags/config #
+#####################
 
-    def __truediv__(self, other):
-        return self.workdir.absolute() / other
 
-    def dump(self, fp: TextIO = sys.stdout) -> Optional[str]:
-        lines = f"REPO: {self.workdir}"
-        lines += "\n [status]\n" + indent(self(["status"]))
-        lines += "\n [branch]\n" + indent(self(["branch", "-avv"]))
-        lines += "\n [tags]\n" + indent(self(["tag", "-l"]))
-        lines += "\n [remote]\n" + indent(self(["remote", "-v"]))
-        if fp == io.StringIO:
-            buf = io.StringIO()
-            print(lines, file=buf)
-            return buf.getvalue()
-        else:
-            print(lines, file=fp)
-            return None
+def pytest_configure(config):
+    config.addinivalue_line("markers", "manual: test intented to run manually")
 
 
-class GitCli(GitWrapper):
-    BETA_BRANCHES = re.compile(r"/beta/(?P<ver>\d+([.]\d+)*)")
+def pytest_collection_modifyitems(config, items):
+    if config.option.keyword or config.option.markexpr:
+        return  # let pytest handle this
 
-    def commit(
-        self, paths: Union[str, Path, List[Union[str, Path]]], message: str
-    ) -> None:
-        paths = [paths] if isinstance(paths, (Path, str)) else paths
-        self(["add", *paths])
-        self(["commit", "-m", message, *paths])
-
-    def branch(self, name: Optional[str] = None, origin: str = "master") -> str:
-        if not name:
-            return self(["rev-parse", "--abbrev-ref", "HEAD"]).strip()
-        assert origin or origin is None
-        old = self.branch()
-        self(["checkout", "-b", name, "--track", origin])
-        return old
-
-    def branches(
-        self, expr: Optional[Union[str, re.Pattern]] = None
-    ) -> Tuple[List[str], Dict[str, List[str]]]:
-        branches = self(["branch", "-a", "--format", "%(refname)"]).split()
-        matchobj = re.compile(expr) if isinstance(expr, str) else expr
-
-        if matchobj:
-            branches = [name for name in branches if matchobj.search(name)]
-
-        n = len("refs/heads/")
-        local_branches = [
-            name[n:] for name in branches if name.startswith("refs/heads/")
-        ]
-        remote_branches: Dict[str, List[str]] = {}
-        n = len("refs/remotes/")
-        for name in branches:
-            if not name.startswith("refs/remotes/"):
-                continue
-            origin, _, name = name[n:].partition("/")
-            if origin not in remote_branches:
-                remote_branches[origin] = []
-            remote_branches[origin].append(name)
-        return local_branches, remote_branches
+    for item in items:
+        if "manual" not in item.keywords:
+            continue
+        item.add_marker(pytest.mark.skip(reason="manual not selected"))
```

