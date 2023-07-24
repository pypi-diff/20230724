# Comparing `tmp/upf_tools-0.1.0.tar.gz` & `tmp/upf_tools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upf_tools-0.1.0.tar", last modified: Mon Jul 24 13:49:48 2023, max compression
+gzip compressed data, was "upf_tools-0.1.1.tar", last modified: Mon Jul 24 14:37:40 2023, max compression
```

## Comparing `upf_tools-0.1.0.tar` & `upf_tools-0.1.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 elinscott  (1000) elinscott  (1000)        0 2023-07-24 13:49:48.889146 upf_tools-0.1.0/
--rw-rw-r--   0 elinscott  (1000) elinscott  (1000)     1072 2023-07-24 09:34:26.000000 upf_tools-0.1.0/LICENSE
--rw-rw-r--   0 elinscott  (1000) elinscott  (1000)      446 2023-07-24 13:48:23.000000 upf_tools-0.1.0/MANIFEST.in
--rw-rw-r--   0 elinscott  (1000) elinscott  (1000)     8060 2023-07-24 13:49:48.889146 upf_tools-0.1.0/PKG-INFO
--rw-rw-r--   0 elinscott  (1000) elinscott  (1000)     6760 2023-07-24 13:48:23.000000 upf_tools-0.1.0/README.md
-drwxrwxr-x   0 elinscott  (1000) elinscott  (1000)        0 2023-07-24 13:49:48.885146 upf_tools-0.1.0/docs/
-drwxrwxr-x   0 elinscott  (1000) elinscott  (1000)        0 2023-07-24 13:49:48.885146 upf_tools-0.1.0/docs/source/
--rw-rw-r--   0 elinscott  (1000) elinscott  (1000)      242 2023-07-24 13:48:23.000000 upf_tools-0.1.0/docs/source/cli.rst
--rw-rw-r--   0 elinscott  (1000) elinscott  (1000)     7276 2023-07-24 13:48:23.000000 upf_tools-0.1.0/docs/source/conf.py
--rw-rw-r--   0 elinscott  (1000) elinscott  (1000)      526 2023-07-24 13:48:23.000000 upf_tools-0.1.0/docs/source/index.rst
--rw-rw-r--   0 elinscott  (1000) elinscott  (1000)      520 2023-07-24 09:34:26.000000 upf_tools-0.1.0/docs/source/installation.rst
--rw-rw-r--   0 elinscott  (1000) elinscott  (1000)      181 2023-07-24 13:48:23.000000 upf_tools-0.1.0/docs/source/usage.rst
--rw-rw-r--   0 elinscott  (1000) elinscott  (1000)      377 2023-07-24 09:34:26.000000 upf_tools-0.1.0/pyproject.toml
--rw-rw-r--   0 elinscott  (1000) elinscott  (1000)     2507 2023-07-24 13:49:48.893146 upf_tools-0.1.0/setup.cfg
-drwxrwxr-x   0 elinscott  (1000) elinscott  (1000)        0 2023-07-24 13:49:48.885146 upf_tools-0.1.0/src/
-drwxrwxr-x   0 elinscott  (1000) elinscott  (1000)        0 2023-07-24 13:49:48.889146 upf_tools-0.1.0/src/upf_tools/
--rw-rw-r--   0 elinscott  (1000) elinscott  (1000)      131 2023-07-24 13:48:23.000000 upf_tools-0.1.0/src/upf_tools/__init__.py
--rw-rw-r--   0 elinscott  (1000) elinscott  (1000)      326 2023-07-24 12:39:47.000000 upf_tools-0.1.0/src/upf_tools/__main__.py
--rw-rw-r--   0 elinscott  (1000) elinscott  (1000)       42 2023-07-24 12:39:47.000000 upf_tools-0.1.0/src/upf_tools/api.py
--rw-rw-r--   0 elinscott  (1000) elinscott  (1000)     1473 2023-07-24 13:48:23.000000 upf_tools-0.1.0/src/upf_tools/cli.py
--rw-rw-r--   0 elinscott  (1000) elinscott  (1000)        1 2023-07-24 09:34:26.000000 upf_tools-0.1.0/src/upf_tools/py.typed
--rw-rw-r--   0 elinscott  (1000) elinscott  (1000)     5053 2023-07-24 13:48:23.000000 upf_tools-0.1.0/src/upf_tools/upfdict.py
--rw-rw-r--   0 elinscott  (1000) elinscott  (1000)      584 2023-07-24 13:48:23.000000 upf_tools-0.1.0/src/upf_tools/utils.py
--rw-rw-r--   0 elinscott  (1000) elinscott  (1000)     5486 2023-07-24 09:34:26.000000 upf_tools-0.1.0/src/upf_tools/v1.py
--rw-rw-r--   0 elinscott  (1000) elinscott  (1000)     2485 2023-07-24 09:34:26.000000 upf_tools-0.1.0/src/upf_tools/v2.py
--rw-rw-r--   0 elinscott  (1000) elinscott  (1000)     1012 2023-07-24 13:48:23.000000 upf_tools-0.1.0/src/upf_tools/version.py
-drwxrwxr-x   0 elinscott  (1000) elinscott  (1000)        0 2023-07-24 13:49:48.889146 upf_tools-0.1.0/src/upf_tools.egg-info/
--rw-rw-r--   0 elinscott  (1000) elinscott  (1000)     8060 2023-07-24 13:49:48.000000 upf_tools-0.1.0/src/upf_tools.egg-info/PKG-INFO
--rw-rw-r--   0 elinscott  (1000) elinscott  (1000)      719 2023-07-24 13:49:48.000000 upf_tools-0.1.0/src/upf_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 elinscott  (1000) elinscott  (1000)        1 2023-07-24 13:49:48.000000 upf_tools-0.1.0/src/upf_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 elinscott  (1000) elinscott  (1000)       49 2023-07-24 13:49:48.000000 upf_tools-0.1.0/src/upf_tools.egg-info/entry_points.txt
--rw-rw-r--   0 elinscott  (1000) elinscott  (1000)        1 2023-07-24 11:46:29.000000 upf_tools-0.1.0/src/upf_tools.egg-info/not-zip-safe
--rw-rw-r--   0 elinscott  (1000) elinscott  (1000)      188 2023-07-24 13:49:48.000000 upf_tools-0.1.0/src/upf_tools.egg-info/requires.txt
--rw-rw-r--   0 elinscott  (1000) elinscott  (1000)       10 2023-07-24 13:49:48.000000 upf_tools-0.1.0/src/upf_tools.egg-info/top_level.txt
-drwxrwxr-x   0 elinscott  (1000) elinscott  (1000)        0 2023-07-24 13:49:48.889146 upf_tools-0.1.0/tests/
--rw-rw-r--   0 elinscott  (1000) elinscott  (1000)       59 2023-07-24 09:34:26.000000 upf_tools-0.1.0/tests/__init__.py
--rw-rw-r--   0 elinscott  (1000) elinscott  (1000)      947 2023-07-24 13:48:23.000000 upf_tools-0.1.0/tests/test_upfdict.py
--rw-rw-r--   0 elinscott  (1000) elinscott  (1000)      403 2023-07-24 09:34:26.000000 upf_tools-0.1.0/tests/test_version.py
+drwxrwxr-x   0 elinscott  (1000) elinscott  (1000)        0 2023-07-24 14:37:40.955859 upf_tools-0.1.1/
+-rw-rw-r--   0 elinscott  (1000) elinscott  (1000)     1072 2023-07-24 09:34:26.000000 upf_tools-0.1.1/LICENSE
+-rw-rw-r--   0 elinscott  (1000) elinscott  (1000)      446 2023-07-24 13:48:23.000000 upf_tools-0.1.1/MANIFEST.in
+-rw-rw-r--   0 elinscott  (1000) elinscott  (1000)     8036 2023-07-24 14:37:40.955859 upf_tools-0.1.1/PKG-INFO
+-rw-rw-r--   0 elinscott  (1000) elinscott  (1000)     6736 2023-07-24 14:36:45.000000 upf_tools-0.1.1/README.md
+drwxrwxr-x   0 elinscott  (1000) elinscott  (1000)        0 2023-07-24 14:37:40.951859 upf_tools-0.1.1/docs/
+drwxrwxr-x   0 elinscott  (1000) elinscott  (1000)        0 2023-07-24 14:37:40.951859 upf_tools-0.1.1/docs/source/
+-rw-rw-r--   0 elinscott  (1000) elinscott  (1000)      242 2023-07-24 13:48:23.000000 upf_tools-0.1.1/docs/source/cli.rst
+-rw-rw-r--   0 elinscott  (1000) elinscott  (1000)     7276 2023-07-24 14:36:45.000000 upf_tools-0.1.1/docs/source/conf.py
+-rw-rw-r--   0 elinscott  (1000) elinscott  (1000)      526 2023-07-24 13:48:23.000000 upf_tools-0.1.1/docs/source/index.rst
+-rw-rw-r--   0 elinscott  (1000) elinscott  (1000)      520 2023-07-24 09:34:26.000000 upf_tools-0.1.1/docs/source/installation.rst
+-rw-rw-r--   0 elinscott  (1000) elinscott  (1000)      181 2023-07-24 13:48:23.000000 upf_tools-0.1.1/docs/source/usage.rst
+-rw-rw-r--   0 elinscott  (1000) elinscott  (1000)      377 2023-07-24 09:34:26.000000 upf_tools-0.1.1/pyproject.toml
+-rw-rw-r--   0 elinscott  (1000) elinscott  (1000)     2507 2023-07-24 14:37:40.955859 upf_tools-0.1.1/setup.cfg
+drwxrwxr-x   0 elinscott  (1000) elinscott  (1000)        0 2023-07-24 14:37:40.951859 upf_tools-0.1.1/src/
+drwxrwxr-x   0 elinscott  (1000) elinscott  (1000)        0 2023-07-24 14:37:40.955859 upf_tools-0.1.1/src/upf_tools/
+-rw-rw-r--   0 elinscott  (1000) elinscott  (1000)      131 2023-07-24 13:48:23.000000 upf_tools-0.1.1/src/upf_tools/__init__.py
+-rw-rw-r--   0 elinscott  (1000) elinscott  (1000)      326 2023-07-24 12:39:47.000000 upf_tools-0.1.1/src/upf_tools/__main__.py
+-rw-rw-r--   0 elinscott  (1000) elinscott  (1000)       42 2023-07-24 12:39:47.000000 upf_tools-0.1.1/src/upf_tools/api.py
+-rw-rw-r--   0 elinscott  (1000) elinscott  (1000)     1473 2023-07-24 13:48:23.000000 upf_tools-0.1.1/src/upf_tools/cli.py
+-rw-rw-r--   0 elinscott  (1000) elinscott  (1000)        1 2023-07-24 09:34:26.000000 upf_tools-0.1.1/src/upf_tools/py.typed
+-rw-rw-r--   0 elinscott  (1000) elinscott  (1000)     5053 2023-07-24 13:48:23.000000 upf_tools-0.1.1/src/upf_tools/upfdict.py
+-rw-rw-r--   0 elinscott  (1000) elinscott  (1000)      584 2023-07-24 13:48:23.000000 upf_tools-0.1.1/src/upf_tools/utils.py
+-rw-rw-r--   0 elinscott  (1000) elinscott  (1000)     5486 2023-07-24 09:34:26.000000 upf_tools-0.1.1/src/upf_tools/v1.py
+-rw-rw-r--   0 elinscott  (1000) elinscott  (1000)     2485 2023-07-24 09:34:26.000000 upf_tools-0.1.1/src/upf_tools/v2.py
+-rw-rw-r--   0 elinscott  (1000) elinscott  (1000)     1012 2023-07-24 14:36:45.000000 upf_tools-0.1.1/src/upf_tools/version.py
+drwxrwxr-x   0 elinscott  (1000) elinscott  (1000)        0 2023-07-24 14:37:40.955859 upf_tools-0.1.1/src/upf_tools.egg-info/
+-rw-rw-r--   0 elinscott  (1000) elinscott  (1000)     8036 2023-07-24 14:37:40.000000 upf_tools-0.1.1/src/upf_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 elinscott  (1000) elinscott  (1000)      719 2023-07-24 14:37:40.000000 upf_tools-0.1.1/src/upf_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 elinscott  (1000) elinscott  (1000)        1 2023-07-24 14:37:40.000000 upf_tools-0.1.1/src/upf_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 elinscott  (1000) elinscott  (1000)       49 2023-07-24 14:37:40.000000 upf_tools-0.1.1/src/upf_tools.egg-info/entry_points.txt
+-rw-rw-r--   0 elinscott  (1000) elinscott  (1000)        1 2023-07-24 11:46:29.000000 upf_tools-0.1.1/src/upf_tools.egg-info/not-zip-safe
+-rw-rw-r--   0 elinscott  (1000) elinscott  (1000)      188 2023-07-24 14:37:40.000000 upf_tools-0.1.1/src/upf_tools.egg-info/requires.txt
+-rw-rw-r--   0 elinscott  (1000) elinscott  (1000)       10 2023-07-24 14:37:40.000000 upf_tools-0.1.1/src/upf_tools.egg-info/top_level.txt
+drwxrwxr-x   0 elinscott  (1000) elinscott  (1000)        0 2023-07-24 14:37:40.955859 upf_tools-0.1.1/tests/
+-rw-rw-r--   0 elinscott  (1000) elinscott  (1000)       59 2023-07-24 09:34:26.000000 upf_tools-0.1.1/tests/__init__.py
+-rw-rw-r--   0 elinscott  (1000) elinscott  (1000)      947 2023-07-24 13:48:23.000000 upf_tools-0.1.1/tests/test_upfdict.py
+-rw-rw-r--   0 elinscott  (1000) elinscott  (1000)      403 2023-07-24 09:34:26.000000 upf_tools-0.1.1/tests/test_version.py
```

### Comparing `upf_tools-0.1.0/LICENSE` & `upf_tools-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `upf_tools-0.1.0/PKG-INFO` & `upf_tools-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upf_tools
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tools for handling .upf (Unified Pseudopotential Format) files
 Home-page: https://github.com/elinscott/upf_tools
 Download-URL: https://github.com/elinscott/upf_tools/releases
 Author: Edward Linscott
 Author-email: edwardlinscott@gmail.com
 Maintainer: Edward Linscott
 Maintainer-email: edwardlinscott@gmail.com
@@ -73,19 +73,19 @@
 </p>
 
 Tools for handling `.upf` (Unified Pseudopotential Format) files
 
 ## 💪 Getting Started
 
 ```python
-from upf_tools import Pseudopotential
-psp = Pseudopotential.from_upf('/path/to/file.upf')
+from upf_tools import UPFDict
+psp = UPFDict.from_upf('/path/to/file.upf')
 ```
 
-`Pseudopotential` is a lightweight class that behaves like a dictionary with a few added functionalities.
+`UPFDict` is a lightweight class that behaves like a dictionary with a few added functionalities.
 
 ### Command Line Interface
 
 The `upf_tools` command line tool is automatically installed. It can
 be used from the shell with the `--help` flag to show all subcommands:
 
 ```shell
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: upf_tools Version: 0.1.0 Summary: Tools for
+Metadata-Version: 2.1 Name: upf_tools Version: 0.1.1 Summary: Tools for
 handling .upf (Unified Pseudopotential Format) files Home-page: https://
 github.com/elinscott/upf_tools Download-URL: https://github.com/elinscott/
 upf_tools/releases Author: Edward Linscott Author-email:
 edwardlinscott@gmail.com Maintainer: Edward Linscott Maintainer-email:
 edwardlinscott@gmail.com License: MIT Project-URL: Bug Tracker, https://
 github.com/elinscott/upf_tools/issues Project-URL: Source Code, https://
 github.com/elinscott/upf_tools Keywords: snekpack,cookiecutter Classifier:
@@ -17,57 +17,56 @@
 Only Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-
 Extra: tests Provides-Extra: docs License-File: LICENSE
                             ****** upf-tools ******
 [Tests] [PyPI] [PyPI_-_Python_Version] [PyPI_-_License] [Documentation_Status]
   [Codecov_status] [Cookiecutter_template_from_@cthoyt] [Code_style:_black]
                             [Contributor_Covenant]
 Tools for handling `.upf` (Unified Pseudopotential Format) files ## ðª
-Getting Started ```python from upf_tools import Pseudopotential psp =
-Pseudopotential.from_upf('/path/to/file.upf') ``` `Pseudopotential` is a
-lightweight class that behaves like a dictionary with a few added
-functionalities. ### Command Line Interface The `upf_tools` command line tool
-is automatically installed. It can be used from the shell with the `--help`
-flag to show all subcommands: ```shell $ upf_tools --help ``` For example, you
-can extract the input file that was used to generate a `.upf` file via ```shell
-$ upf_tools to-input /path/to/pseudo.upf > pseudo.in ``` ## ð Installation
-The most recent release can be installed from [PyPI](https://pypi.org/project/
-upf_tools/) with: ```shell $ pip install upf_tools ``` The most recent code and
-data can be installed directly from GitHub with: ```bash $ pip install
-git+https://github.com/elinscott/upf_tools.git ``` ## ð Contributing
-Contributions, whether filing an issue, making a pull request, or forking, are
-appreciated. See [CONTRIBUTING.md](https://github.com/elinscott/upf_tools/blob/
-master/.github/CONTRIBUTING.md) for more information on getting involved. ##
-ð Attribution ### âï¸ License The code in this package is licensed under
-the MIT License.    ### ðª Cookiecutter This package was created with
-[@audreyfeldroy](https://github.com/audreyfeldroy)'s [cookiecutter](https://
-github.com/cookiecutter/cookiecutter) package using [@cthoyt](https://
-github.com/cthoyt)'s [cookiecutter-snekpack](https://github.com/cthoyt/
-cookiecutter-snekpack) template. ## ð ï¸ For Developers  See developer
-instructions The final section of the README is for if you want to get involved
-by making a code contribution. ### Development Installation To install in
-development mode, use the following: ```bash $ git clone git+https://
-github.com/elinscott/upf_tools.git $ cd upf_tools $ pip install -e . ``` ###
-ð¥¼ Testing After cloning the repository and installing `tox` with `pip
-install tox`, the unit tests in the `tests/` folder can be run reproducibly
-with: ```shell $ tox ``` Additionally, these tests are automatically re-run
-with each commit in a [GitHub Action](https://github.com/elinscott/upf_tools/
-actions?query=workflow%3ATests). ### ð Building the Documentation The
-documentation can be built locally using the following: ```shell $ git clone
-git+https://github.com/elinscott/upf_tools.git $ cd upf_tools $ tox -e docs $
-open docs/build/html/index.html ``` The documentation automatically installs
-the package as well as the `docs` extra specified in the [`setup.cfg`]
-(setup.cfg). `sphinx` plugins like `texext` can be added there. Additionally,
-they need to be added to the `extensions` list in [`docs/source/conf.py`](docs/
-source/conf.py). ### ð¦ Making a Release After installing the package in
-development mode and installing `tox` with `pip install tox`, the commands for
-making a new release are contained within the `finish` environment in
-`tox.ini`. Run the following from the shell: ```shell $ tox -e finish ``` This
-script does the following: 1. Uses [Bump2Version](https://github.com/c4urself/
-bump2version) to switch the version number in the `setup.cfg`, `src/upf_tools/
-version.py`, and [`docs/source/conf.py`](docs/source/conf.py) to not have the
-`-dev` suffix 2. Packages the code in both a tar archive and a wheel using
-[`build`](https://github.com/pypa/build) 3. Uploads to PyPI using [`twine`]
-(https://github.com/pypa/twine). Be sure to have a `.pypirc` file configured to
-avoid the need for manual input at this step 4. Push to GitHub. You'll need to
-make a release going with the commit where the version was bumped. 5. Bump the
-version to the next patch. If you made big changes and want to bump the version
-by minor, you can use `tox -e bumpversion -- minor` after.
+Getting Started ```python from upf_tools import UPFDict psp = UPFDict.from_upf
+('/path/to/file.upf') ``` `UPFDict` is a lightweight class that behaves like a
+dictionary with a few added functionalities. ### Command Line Interface The
+`upf_tools` command line tool is automatically installed. It can be used from
+the shell with the `--help` flag to show all subcommands: ```shell $ upf_tools
+--help ``` For example, you can extract the input file that was used to
+generate a `.upf` file via ```shell $ upf_tools to-input /path/to/pseudo.upf >
+pseudo.in ``` ## ð Installation The most recent release can be installed
+from [PyPI](https://pypi.org/project/upf_tools/) with: ```shell $ pip install
+upf_tools ``` The most recent code and data can be installed directly from
+GitHub with: ```bash $ pip install git+https://github.com/elinscott/
+upf_tools.git ``` ## ð Contributing Contributions, whether filing an issue,
+making a pull request, or forking, are appreciated. See [CONTRIBUTING.md]
+(https://github.com/elinscott/upf_tools/blob/master/.github/CONTRIBUTING.md)
+for more information on getting involved. ## ð Attribution ### âï¸
+License The code in this package is licensed under the MIT License.    ### ðª
+Cookiecutter This package was created with [@audreyfeldroy](https://github.com/
+audreyfeldroy)'s [cookiecutter](https://github.com/cookiecutter/cookiecutter)
+package using [@cthoyt](https://github.com/cthoyt)'s [cookiecutter-snekpack]
+(https://github.com/cthoyt/cookiecutter-snekpack) template. ## ð ï¸ For
+Developers  See developer instructions The final section of the README is for
+if you want to get involved by making a code contribution. ### Development
+Installation To install in development mode, use the following: ```bash $ git
+clone git+https://github.com/elinscott/upf_tools.git $ cd upf_tools $ pip
+install -e . ``` ### ð¥¼ Testing After cloning the repository and installing
+`tox` with `pip install tox`, the unit tests in the `tests/` folder can be run
+reproducibly with: ```shell $ tox ``` Additionally, these tests are
+automatically re-run with each commit in a [GitHub Action](https://github.com/
+elinscott/upf_tools/actions?query=workflow%3ATests). ### ð Building the
+Documentation The documentation can be built locally using the following:
+```shell $ git clone git+https://github.com/elinscott/upf_tools.git $ cd
+upf_tools $ tox -e docs $ open docs/build/html/index.html ``` The documentation
+automatically installs the package as well as the `docs` extra specified in the
+[`setup.cfg`](setup.cfg). `sphinx` plugins like `texext` can be added there.
+Additionally, they need to be added to the `extensions` list in [`docs/source/
+conf.py`](docs/source/conf.py). ### ð¦ Making a Release After installing the
+package in development mode and installing `tox` with `pip install tox`, the
+commands for making a new release are contained within the `finish` environment
+in `tox.ini`. Run the following from the shell: ```shell $ tox -e finish ```
+This script does the following: 1. Uses [Bump2Version](https://github.com/
+c4urself/bump2version) to switch the version number in the `setup.cfg`, `src/
+upf_tools/version.py`, and [`docs/source/conf.py`](docs/source/conf.py) to not
+have the `-dev` suffix 2. Packages the code in both a tar archive and a wheel
+using [`build`](https://github.com/pypa/build) 3. Uploads to PyPI using
+[`twine`](https://github.com/pypa/twine). Be sure to have a `.pypirc` file
+configured to avoid the need for manual input at this step 4. Push to GitHub.
+You'll need to make a release going with the commit where the version was
+bumped. 5. Bump the version to the next patch. If you made big changes and want
+to bump the version by minor, you can use `tox -e bumpversion -- minor` after.
```

### Comparing `upf_tools-0.1.0/README.md` & `upf_tools-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -39,19 +39,19 @@
 </p>
 
 Tools for handling `.upf` (Unified Pseudopotential Format) files
 
 ## 💪 Getting Started
 
 ```python
-from upf_tools import Pseudopotential
-psp = Pseudopotential.from_upf('/path/to/file.upf')
+from upf_tools import UPFDict
+psp = UPFDict.from_upf('/path/to/file.upf')
 ```
 
-`Pseudopotential` is a lightweight class that behaves like a dictionary with a few added functionalities.
+`UPFDict` is a lightweight class that behaves like a dictionary with a few added functionalities.
 
 ### Command Line Interface
 
 The `upf_tools` command line tool is automatically installed. It can
 be used from the shell with the `--help` flag to show all subcommands:
 
 ```shell
```

#### html2text {}

```diff
@@ -1,55 +1,54 @@
                             ****** upf-tools ******
 [Tests] [PyPI] [PyPI_-_Python_Version] [PyPI_-_License] [Documentation_Status]
   [Codecov_status] [Cookiecutter_template_from_@cthoyt] [Code_style:_black]
                             [Contributor_Covenant]
 Tools for handling `.upf` (Unified Pseudopotential Format) files ## ðª
-Getting Started ```python from upf_tools import Pseudopotential psp =
-Pseudopotential.from_upf('/path/to/file.upf') ``` `Pseudopotential` is a
-lightweight class that behaves like a dictionary with a few added
-functionalities. ### Command Line Interface The `upf_tools` command line tool
-is automatically installed. It can be used from the shell with the `--help`
-flag to show all subcommands: ```shell $ upf_tools --help ``` For example, you
-can extract the input file that was used to generate a `.upf` file via ```shell
-$ upf_tools to-input /path/to/pseudo.upf > pseudo.in ``` ## ð Installation
-The most recent release can be installed from [PyPI](https://pypi.org/project/
-upf_tools/) with: ```shell $ pip install upf_tools ``` The most recent code and
-data can be installed directly from GitHub with: ```bash $ pip install
-git+https://github.com/elinscott/upf_tools.git ``` ## ð Contributing
-Contributions, whether filing an issue, making a pull request, or forking, are
-appreciated. See [CONTRIBUTING.md](https://github.com/elinscott/upf_tools/blob/
-master/.github/CONTRIBUTING.md) for more information on getting involved. ##
-ð Attribution ### âï¸ License The code in this package is licensed under
-the MIT License.    ### ðª Cookiecutter This package was created with
-[@audreyfeldroy](https://github.com/audreyfeldroy)'s [cookiecutter](https://
-github.com/cookiecutter/cookiecutter) package using [@cthoyt](https://
-github.com/cthoyt)'s [cookiecutter-snekpack](https://github.com/cthoyt/
-cookiecutter-snekpack) template. ## ð ï¸ For Developers  See developer
-instructions The final section of the README is for if you want to get involved
-by making a code contribution. ### Development Installation To install in
-development mode, use the following: ```bash $ git clone git+https://
-github.com/elinscott/upf_tools.git $ cd upf_tools $ pip install -e . ``` ###
-ð¥¼ Testing After cloning the repository and installing `tox` with `pip
-install tox`, the unit tests in the `tests/` folder can be run reproducibly
-with: ```shell $ tox ``` Additionally, these tests are automatically re-run
-with each commit in a [GitHub Action](https://github.com/elinscott/upf_tools/
-actions?query=workflow%3ATests). ### ð Building the Documentation The
-documentation can be built locally using the following: ```shell $ git clone
-git+https://github.com/elinscott/upf_tools.git $ cd upf_tools $ tox -e docs $
-open docs/build/html/index.html ``` The documentation automatically installs
-the package as well as the `docs` extra specified in the [`setup.cfg`]
-(setup.cfg). `sphinx` plugins like `texext` can be added there. Additionally,
-they need to be added to the `extensions` list in [`docs/source/conf.py`](docs/
-source/conf.py). ### ð¦ Making a Release After installing the package in
-development mode and installing `tox` with `pip install tox`, the commands for
-making a new release are contained within the `finish` environment in
-`tox.ini`. Run the following from the shell: ```shell $ tox -e finish ``` This
-script does the following: 1. Uses [Bump2Version](https://github.com/c4urself/
-bump2version) to switch the version number in the `setup.cfg`, `src/upf_tools/
-version.py`, and [`docs/source/conf.py`](docs/source/conf.py) to not have the
-`-dev` suffix 2. Packages the code in both a tar archive and a wheel using
-[`build`](https://github.com/pypa/build) 3. Uploads to PyPI using [`twine`]
-(https://github.com/pypa/twine). Be sure to have a `.pypirc` file configured to
-avoid the need for manual input at this step 4. Push to GitHub. You'll need to
-make a release going with the commit where the version was bumped. 5. Bump the
-version to the next patch. If you made big changes and want to bump the version
-by minor, you can use `tox -e bumpversion -- minor` after.
+Getting Started ```python from upf_tools import UPFDict psp = UPFDict.from_upf
+('/path/to/file.upf') ``` `UPFDict` is a lightweight class that behaves like a
+dictionary with a few added functionalities. ### Command Line Interface The
+`upf_tools` command line tool is automatically installed. It can be used from
+the shell with the `--help` flag to show all subcommands: ```shell $ upf_tools
+--help ``` For example, you can extract the input file that was used to
+generate a `.upf` file via ```shell $ upf_tools to-input /path/to/pseudo.upf >
+pseudo.in ``` ## ð Installation The most recent release can be installed
+from [PyPI](https://pypi.org/project/upf_tools/) with: ```shell $ pip install
+upf_tools ``` The most recent code and data can be installed directly from
+GitHub with: ```bash $ pip install git+https://github.com/elinscott/
+upf_tools.git ``` ## ð Contributing Contributions, whether filing an issue,
+making a pull request, or forking, are appreciated. See [CONTRIBUTING.md]
+(https://github.com/elinscott/upf_tools/blob/master/.github/CONTRIBUTING.md)
+for more information on getting involved. ## ð Attribution ### âï¸
+License The code in this package is licensed under the MIT License.    ### ðª
+Cookiecutter This package was created with [@audreyfeldroy](https://github.com/
+audreyfeldroy)'s [cookiecutter](https://github.com/cookiecutter/cookiecutter)
+package using [@cthoyt](https://github.com/cthoyt)'s [cookiecutter-snekpack]
+(https://github.com/cthoyt/cookiecutter-snekpack) template. ## ð ï¸ For
+Developers  See developer instructions The final section of the README is for
+if you want to get involved by making a code contribution. ### Development
+Installation To install in development mode, use the following: ```bash $ git
+clone git+https://github.com/elinscott/upf_tools.git $ cd upf_tools $ pip
+install -e . ``` ### ð¥¼ Testing After cloning the repository and installing
+`tox` with `pip install tox`, the unit tests in the `tests/` folder can be run
+reproducibly with: ```shell $ tox ``` Additionally, these tests are
+automatically re-run with each commit in a [GitHub Action](https://github.com/
+elinscott/upf_tools/actions?query=workflow%3ATests). ### ð Building the
+Documentation The documentation can be built locally using the following:
+```shell $ git clone git+https://github.com/elinscott/upf_tools.git $ cd
+upf_tools $ tox -e docs $ open docs/build/html/index.html ``` The documentation
+automatically installs the package as well as the `docs` extra specified in the
+[`setup.cfg`](setup.cfg). `sphinx` plugins like `texext` can be added there.
+Additionally, they need to be added to the `extensions` list in [`docs/source/
+conf.py`](docs/source/conf.py). ### ð¦ Making a Release After installing the
+package in development mode and installing `tox` with `pip install tox`, the
+commands for making a new release are contained within the `finish` environment
+in `tox.ini`. Run the following from the shell: ```shell $ tox -e finish ```
+This script does the following: 1. Uses [Bump2Version](https://github.com/
+c4urself/bump2version) to switch the version number in the `setup.cfg`, `src/
+upf_tools/version.py`, and [`docs/source/conf.py`](docs/source/conf.py) to not
+have the `-dev` suffix 2. Packages the code in both a tar archive and a wheel
+using [`build`](https://github.com/pypa/build) 3. Uploads to PyPI using
+[`twine`](https://github.com/pypa/twine). Be sure to have a `.pypirc` file
+configured to avoid the need for manual input at this step 4. Push to GitHub.
+You'll need to make a release going with the commit where the version was
+bumped. 5. Bump the version to the next patch. If you made big changes and want
+to bump the version by minor, you can use `tox -e bumpversion -- minor` after.
```

### Comparing `upf_tools-0.1.0/docs/source/conf.py` & `upf_tools-0.1.1/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "upf_tools"
 copyright = f"{date.today().year}, Edward Linscott"
 author = "Edward Linscott"
 
 # The full version, including alpha/beta/rc tags.
-release = "0.1.0"
+release = "0.1.1"
 
 # The short X.Y version.
 parsed_version = re.match(
     "(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?:-(?P<release>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?(?:\+(?P<build>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?",
     release,
 )
 version = parsed_version.expand("\g<major>.\g<minor>.\g<patch>")
```

### Comparing `upf_tools-0.1.0/docs/source/index.rst` & `upf_tools-0.1.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `upf_tools-0.1.0/docs/source/installation.rst` & `upf_tools-0.1.1/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `upf_tools-0.1.0/setup.cfg` & `upf_tools-0.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = upf_tools
-version = 0.1.0
+version = 0.1.1
 description = Tools for handling .upf (Unified Pseudopotential Format) files
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/elinscott/upf_tools
 download_url = https://github.com/elinscott/upf_tools/releases
 project_urls = 
 	Bug Tracker = https://github.com/elinscott/upf_tools/issues
```

### Comparing `upf_tools-0.1.0/src/upf_tools/cli.py` & `upf_tools-0.1.1/src/upf_tools/cli.py`

 * *Files identical despite different names*

### Comparing `upf_tools-0.1.0/src/upf_tools/upfdict.py` & `upf_tools-0.1.1/src/upf_tools/upfdict.py`

 * *Files identical despite different names*

### Comparing `upf_tools-0.1.0/src/upf_tools/utils.py` & `upf_tools-0.1.1/src/upf_tools/utils.py`

 * *Files identical despite different names*

### Comparing `upf_tools-0.1.0/src/upf_tools/v1.py` & `upf_tools-0.1.1/src/upf_tools/v1.py`

 * *Files identical despite different names*

### Comparing `upf_tools-0.1.0/src/upf_tools/v2.py` & `upf_tools-0.1.1/src/upf_tools/v2.py`

 * *Files identical despite different names*

### Comparing `upf_tools-0.1.0/src/upf_tools/version.py` & `upf_tools-0.1.1/src/upf_tools/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 __all__ = [
     "VERSION",
     "get_version",
     "get_git_hash",
 ]
 
-VERSION = "0.1.0"
+VERSION = "0.1.1"
 
 
 def get_git_hash() -> str:
     """Get the :mod:`upf_tools` git hash."""
     with open(os.devnull, "w") as devnull:
         try:
             ret = check_output(  # noqa: S603,S607
```

### Comparing `upf_tools-0.1.0/src/upf_tools.egg-info/PKG-INFO` & `upf_tools-0.1.1/src/upf_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upf-tools
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tools for handling .upf (Unified Pseudopotential Format) files
 Home-page: https://github.com/elinscott/upf_tools
 Download-URL: https://github.com/elinscott/upf_tools/releases
 Author: Edward Linscott
 Author-email: edwardlinscott@gmail.com
 Maintainer: Edward Linscott
 Maintainer-email: edwardlinscott@gmail.com
@@ -73,19 +73,19 @@
 </p>
 
 Tools for handling `.upf` (Unified Pseudopotential Format) files
 
 ## 💪 Getting Started
 
 ```python
-from upf_tools import Pseudopotential
-psp = Pseudopotential.from_upf('/path/to/file.upf')
+from upf_tools import UPFDict
+psp = UPFDict.from_upf('/path/to/file.upf')
 ```
 
-`Pseudopotential` is a lightweight class that behaves like a dictionary with a few added functionalities.
+`UPFDict` is a lightweight class that behaves like a dictionary with a few added functionalities.
 
 ### Command Line Interface
 
 The `upf_tools` command line tool is automatically installed. It can
 be used from the shell with the `--help` flag to show all subcommands:
 
 ```shell
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: upf-tools Version: 0.1.0 Summary: Tools for
+Metadata-Version: 2.1 Name: upf-tools Version: 0.1.1 Summary: Tools for
 handling .upf (Unified Pseudopotential Format) files Home-page: https://
 github.com/elinscott/upf_tools Download-URL: https://github.com/elinscott/
 upf_tools/releases Author: Edward Linscott Author-email:
 edwardlinscott@gmail.com Maintainer: Edward Linscott Maintainer-email:
 edwardlinscott@gmail.com License: MIT Project-URL: Bug Tracker, https://
 github.com/elinscott/upf_tools/issues Project-URL: Source Code, https://
 github.com/elinscott/upf_tools Keywords: snekpack,cookiecutter Classifier:
@@ -17,57 +17,56 @@
 Only Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-
 Extra: tests Provides-Extra: docs License-File: LICENSE
                             ****** upf-tools ******
 [Tests] [PyPI] [PyPI_-_Python_Version] [PyPI_-_License] [Documentation_Status]
   [Codecov_status] [Cookiecutter_template_from_@cthoyt] [Code_style:_black]
                             [Contributor_Covenant]
 Tools for handling `.upf` (Unified Pseudopotential Format) files ## ðª
-Getting Started ```python from upf_tools import Pseudopotential psp =
-Pseudopotential.from_upf('/path/to/file.upf') ``` `Pseudopotential` is a
-lightweight class that behaves like a dictionary with a few added
-functionalities. ### Command Line Interface The `upf_tools` command line tool
-is automatically installed. It can be used from the shell with the `--help`
-flag to show all subcommands: ```shell $ upf_tools --help ``` For example, you
-can extract the input file that was used to generate a `.upf` file via ```shell
-$ upf_tools to-input /path/to/pseudo.upf > pseudo.in ``` ## ð Installation
-The most recent release can be installed from [PyPI](https://pypi.org/project/
-upf_tools/) with: ```shell $ pip install upf_tools ``` The most recent code and
-data can be installed directly from GitHub with: ```bash $ pip install
-git+https://github.com/elinscott/upf_tools.git ``` ## ð Contributing
-Contributions, whether filing an issue, making a pull request, or forking, are
-appreciated. See [CONTRIBUTING.md](https://github.com/elinscott/upf_tools/blob/
-master/.github/CONTRIBUTING.md) for more information on getting involved. ##
-ð Attribution ### âï¸ License The code in this package is licensed under
-the MIT License.    ### ðª Cookiecutter This package was created with
-[@audreyfeldroy](https://github.com/audreyfeldroy)'s [cookiecutter](https://
-github.com/cookiecutter/cookiecutter) package using [@cthoyt](https://
-github.com/cthoyt)'s [cookiecutter-snekpack](https://github.com/cthoyt/
-cookiecutter-snekpack) template. ## ð ï¸ For Developers  See developer
-instructions The final section of the README is for if you want to get involved
-by making a code contribution. ### Development Installation To install in
-development mode, use the following: ```bash $ git clone git+https://
-github.com/elinscott/upf_tools.git $ cd upf_tools $ pip install -e . ``` ###
-ð¥¼ Testing After cloning the repository and installing `tox` with `pip
-install tox`, the unit tests in the `tests/` folder can be run reproducibly
-with: ```shell $ tox ``` Additionally, these tests are automatically re-run
-with each commit in a [GitHub Action](https://github.com/elinscott/upf_tools/
-actions?query=workflow%3ATests). ### ð Building the Documentation The
-documentation can be built locally using the following: ```shell $ git clone
-git+https://github.com/elinscott/upf_tools.git $ cd upf_tools $ tox -e docs $
-open docs/build/html/index.html ``` The documentation automatically installs
-the package as well as the `docs` extra specified in the [`setup.cfg`]
-(setup.cfg). `sphinx` plugins like `texext` can be added there. Additionally,
-they need to be added to the `extensions` list in [`docs/source/conf.py`](docs/
-source/conf.py). ### ð¦ Making a Release After installing the package in
-development mode and installing `tox` with `pip install tox`, the commands for
-making a new release are contained within the `finish` environment in
-`tox.ini`. Run the following from the shell: ```shell $ tox -e finish ``` This
-script does the following: 1. Uses [Bump2Version](https://github.com/c4urself/
-bump2version) to switch the version number in the `setup.cfg`, `src/upf_tools/
-version.py`, and [`docs/source/conf.py`](docs/source/conf.py) to not have the
-`-dev` suffix 2. Packages the code in both a tar archive and a wheel using
-[`build`](https://github.com/pypa/build) 3. Uploads to PyPI using [`twine`]
-(https://github.com/pypa/twine). Be sure to have a `.pypirc` file configured to
-avoid the need for manual input at this step 4. Push to GitHub. You'll need to
-make a release going with the commit where the version was bumped. 5. Bump the
-version to the next patch. If you made big changes and want to bump the version
-by minor, you can use `tox -e bumpversion -- minor` after.
+Getting Started ```python from upf_tools import UPFDict psp = UPFDict.from_upf
+('/path/to/file.upf') ``` `UPFDict` is a lightweight class that behaves like a
+dictionary with a few added functionalities. ### Command Line Interface The
+`upf_tools` command line tool is automatically installed. It can be used from
+the shell with the `--help` flag to show all subcommands: ```shell $ upf_tools
+--help ``` For example, you can extract the input file that was used to
+generate a `.upf` file via ```shell $ upf_tools to-input /path/to/pseudo.upf >
+pseudo.in ``` ## ð Installation The most recent release can be installed
+from [PyPI](https://pypi.org/project/upf_tools/) with: ```shell $ pip install
+upf_tools ``` The most recent code and data can be installed directly from
+GitHub with: ```bash $ pip install git+https://github.com/elinscott/
+upf_tools.git ``` ## ð Contributing Contributions, whether filing an issue,
+making a pull request, or forking, are appreciated. See [CONTRIBUTING.md]
+(https://github.com/elinscott/upf_tools/blob/master/.github/CONTRIBUTING.md)
+for more information on getting involved. ## ð Attribution ### âï¸
+License The code in this package is licensed under the MIT License.    ### ðª
+Cookiecutter This package was created with [@audreyfeldroy](https://github.com/
+audreyfeldroy)'s [cookiecutter](https://github.com/cookiecutter/cookiecutter)
+package using [@cthoyt](https://github.com/cthoyt)'s [cookiecutter-snekpack]
+(https://github.com/cthoyt/cookiecutter-snekpack) template. ## ð ï¸ For
+Developers  See developer instructions The final section of the README is for
+if you want to get involved by making a code contribution. ### Development
+Installation To install in development mode, use the following: ```bash $ git
+clone git+https://github.com/elinscott/upf_tools.git $ cd upf_tools $ pip
+install -e . ``` ### ð¥¼ Testing After cloning the repository and installing
+`tox` with `pip install tox`, the unit tests in the `tests/` folder can be run
+reproducibly with: ```shell $ tox ``` Additionally, these tests are
+automatically re-run with each commit in a [GitHub Action](https://github.com/
+elinscott/upf_tools/actions?query=workflow%3ATests). ### ð Building the
+Documentation The documentation can be built locally using the following:
+```shell $ git clone git+https://github.com/elinscott/upf_tools.git $ cd
+upf_tools $ tox -e docs $ open docs/build/html/index.html ``` The documentation
+automatically installs the package as well as the `docs` extra specified in the
+[`setup.cfg`](setup.cfg). `sphinx` plugins like `texext` can be added there.
+Additionally, they need to be added to the `extensions` list in [`docs/source/
+conf.py`](docs/source/conf.py). ### ð¦ Making a Release After installing the
+package in development mode and installing `tox` with `pip install tox`, the
+commands for making a new release are contained within the `finish` environment
+in `tox.ini`. Run the following from the shell: ```shell $ tox -e finish ```
+This script does the following: 1. Uses [Bump2Version](https://github.com/
+c4urself/bump2version) to switch the version number in the `setup.cfg`, `src/
+upf_tools/version.py`, and [`docs/source/conf.py`](docs/source/conf.py) to not
+have the `-dev` suffix 2. Packages the code in both a tar archive and a wheel
+using [`build`](https://github.com/pypa/build) 3. Uploads to PyPI using
+[`twine`](https://github.com/pypa/twine). Be sure to have a `.pypirc` file
+configured to avoid the need for manual input at this step 4. Push to GitHub.
+You'll need to make a release going with the commit where the version was
+bumped. 5. Bump the version to the next patch. If you made big changes and want
+to bump the version by minor, you can use `tox -e bumpversion -- minor` after.
```

### Comparing `upf_tools-0.1.0/src/upf_tools.egg-info/SOURCES.txt` & `upf_tools-0.1.1/src/upf_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `upf_tools-0.1.0/tests/test_upfdict.py` & `upf_tools-0.1.1/tests/test_upfdict.py`

 * *Files identical despite different names*

